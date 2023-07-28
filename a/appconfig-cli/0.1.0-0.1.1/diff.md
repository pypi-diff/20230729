# Comparing `tmp/appconfig_cli-0.1.0.tar.gz` & `tmp/appconfig_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appconfig_cli-0.1.0.tar", max compression
+gzip compressed data, was "appconfig_cli-0.1.1.tar", max compression
```

## Comparing `appconfig_cli-0.1.0.tar` & `appconfig_cli-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-07-05 14:37:28.705062 appconfig_cli-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     1306 2023-07-05 14:46:35.854038 appconfig_cli-0.1.0/README.md
--rw-r--r--   0        0        0       22 2023-07-05 14:46:53.787175 appconfig_cli-0.1.0/appconf/__init__.py
--rw-r--r--   0        0        0     2995 2023-07-05 14:22:43.979476 appconfig_cli-0.1.0/appconf/api.py
--rw-r--r--   0        0        0     2767 2023-07-05 14:22:53.410710 appconfig_cli-0.1.0/appconf/main.py
--rw-r--r--   0        0        0      683 2023-07-05 14:20:18.305905 appconfig_cli-0.1.0/appconf/models.py
--rw-r--r--   0        0        0      644 2023-07-05 14:42:44.125113 appconfig_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1922 1970-01-01 00:00:00.000000 appconfig_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      139 2023-07-28 22:06:16.720517 appconfig_cli-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1061 2023-07-05 14:37:28.705062 appconfig_cli-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     1481 2023-07-28 22:06:12.256504 appconfig_cli-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2023-07-28 16:04:03.210700 appconfig_cli-0.1.1/appconf/__init__.py
+-rw-r--r--   0        0        0     3397 2023-07-28 16:06:47.448450 appconfig_cli-0.1.1/appconf/api.py
+-rw-r--r--   0        0        0       62 2023-07-28 15:56:01.799312 appconfig_cli-0.1.1/appconf/exceptions.py
+-rw-r--r--   0        0        0     3230 2023-07-28 16:07:54.779836 appconfig_cli-0.1.1/appconf/main.py
+-rw-r--r--   0        0        0      726 2023-07-28 16:06:47.438566 appconfig_cli-0.1.1/appconf/models.py
+-rw-r--r--   0        0        0     1159 2023-07-28 22:09:00.784275 appconfig_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 appconfig_cli-0.1.1/PKG-INFO
```

### Comparing `appconfig_cli-0.1.0/LICENSE.md` & `appconfig_cli-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `appconfig_cli-0.1.0/README.md` & `appconfig_cli-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -26,11 +26,12 @@
 Commands:
   get  Get the current hosted configuration for the application & profile
   put  Upload a new hosted configuration version for the application &...
 ```
 
 ## Examples:
 
-Get current config: `appconf get --app <application name> --profile <profile name>`
-Put new config: `appconf put -a <application name> -p <profile name> path/to/config.json`
-
-
+- Get current config: `appconf get --app <application name> --profile <profile name>`
+- Put new config: 
+  - `appconf put -a <application name> -p <profile name> path/to/config.json`
+  - `appconf put -a <application name> -p <profile name> < cat path/to/config.json`
+  - `cat path/to/config.json | appconf put -a <application name> -p <profile name>`
```

### Comparing `appconfig_cli-0.1.0/appconf/api.py` & `appconfig_cli-0.1.1/appconf/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 
 from appconf.models import Application, ConfigurationProfile, HostedConfigurationVersion
+from appconf.exceptions import NoHostedConfigurationVersionsFound
 
 
 def get_application(appconfig_client, app_name):
     """
     Get the application id from the application name
     """
     apps = appconfig_client.list_applications()
@@ -35,14 +36,20 @@
     """
     Get the latest hosted configuration version from the configuration profile id
     """
     config_versions = appconfig_client.list_hosted_configuration_versions(
         ApplicationId=application.Id, ConfigurationProfileId=config_profile.Id
     )
 
+    if len(config_versions["Items"]) == 0:
+        logging.error("No hosted configuration versions found!")
+        raise NoHostedConfigurationVersionsFound(
+            "No hosted configuration versions found!"
+        )
+
     latest_version = config_versions["Items"][0]
 
     for v in config_versions["Items"]:
         if v["VersionNumber"] > latest_version["VersionNumber"]:
             latest_version = v
 
     latest_hosted_config = appconfig_client.get_hosted_configuration_version(
@@ -51,29 +58,38 @@
         VersionNumber=latest_version["VersionNumber"],
     )
 
     return HostedConfigurationVersion.from_dict(latest_hosted_config)
 
 
 def create_configuration(
-    client, application, config_profile, latest_config_profile, config_file, description
+    client,
+    application,
+    config_profile,
+    config_file,
+    description,
+    latest_config_profile=None,
 ):
     """
     Create a new hosted configuration version for the application & profile
     """
     content = config_file.read().encode("utf-8")
 
+    current_version = (
+        latest_config_profile.VersionNumber if latest_config_profile else 0
+    )
+
     try:
         response = client.create_hosted_configuration_version(
             ApplicationId=application.Id,
             ConfigurationProfileId=config_profile.Id,
             Description=description,
             Content=content,
             ContentType="application/json",
-            LatestVersionNumber=latest_config_profile.VersionNumber,
+            LatestVersionNumber=current_version,
         )
     except Exception as e:
         logging.error(f"Error creating hosted configuration version: {e}")
         return
 
     if response["ResponseMetadata"]["HTTPStatusCode"] != 201:
         logging.error(f"Error creating hosted configuration version: {response}")
```

### Comparing `appconfig_cli-0.1.0/appconf/main.py` & `appconfig_cli-0.1.1/appconf/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 AWS AppConfig CLI
 """
 
 import logging
 import os
+import sys
 
 import boto3
 import click
 from rich.console import Console
 from rich.logging import RichHandler
 from rich.rule import Rule
 
 from appconf import api
+from appconf.exceptions import NoHostedConfigurationVersionsFound
 
 logging.basicConfig(level=logging.INFO, handlers=[RichHandler()])
 
 console = Console()
 
 
 @click.group()
@@ -37,17 +39,25 @@
 @click.option("-p", "--profile", help="Configuration profile name", required=True)
 @click.option("-m", "--meta", help="Display metadata", default=False, is_flag=True)
 def get_config(ctx, app, profile, meta):
     """
     Get the current hosted configuration for the application & profile
     """
     application, config_profile = api.setup(ctx.obj["appconfig"], app, profile)
-    latest_hosted_config = api.get_latest_hosted_configuration_version(
-        ctx.obj["appconfig"], application, config_profile
-    )
+
+    try:
+        latest_hosted_config = api.get_latest_hosted_configuration_version(
+            ctx.obj["appconfig"], application, config_profile
+        )
+    except NoHostedConfigurationVersionsFound:
+        console.print(
+            "[red]No hosted configuration versions found "
+            f"for {application.Name} ({application.Id})![/red]"
+        )
+        return
 
     if meta:
         console.print(
             f"[blue bold]Application:[/blue bold] {application.Name} ({application.Id})"
         )
         console.print(
             f"[blue bold]Configuration:[/blue bold] {profile} ({config_profile.Id})"
@@ -58,34 +68,38 @@
         console.print(Rule())
 
     console.print_json(latest_hosted_config.get_json())
 
 
 @cli.command(name="put")
 @click.pass_context
-@click.argument("config_file", type=click.File("r"))
+@click.argument("config_file", type=click.File("r"), default=sys.stdin)
 @click.option("-a", "--app", help="Application Name", required=True)
 @click.option("-p", "--profile", help="Configuration profile name", required=True)
 @click.option("-d", "--description", help="Description for the version", default="")
 def put_config(ctx, config_file, app, profile, description):
     """
     Upload a new hosted configuration version for the application & profile
     """
     application, config_profile = api.setup(ctx.obj["appconfig"], app, profile)
-    latest_hosted_config = api.get_latest_hosted_configuration_version(
-        ctx.obj["appconfig"], application, config_profile
-    )
+
+    try:
+        latest_hosted_config = api.get_latest_hosted_configuration_version(
+            ctx.obj["appconfig"], application, config_profile
+        )
+    except NoHostedConfigurationVersionsFound:
+        latest_hosted_config = None
 
     version = api.create_configuration(
         ctx.obj["appconfig"],
         application,
         config_profile,
-        latest_hosted_config,
         config_file,
         description,
+        latest_config_profile=latest_hosted_config,
     )
 
     console.print(f"[green]Created new configuration version:[/green] {version}")
 
 
 if __name__ == "__main__":
     cli(obj={})
```

### Comparing `appconfig_cli-0.1.0/appconf/models.py` & `appconfig_cli-0.1.1/appconf/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import dataclasses
+from typing import Optional
 
 
 class Base:
     @classmethod
     def from_dict(cls, d):
         fields = set([f.name for f in dataclasses.fields(cls)])
         return cls(**{k: v for k, v in d.items() if k in fields})
 
 
 @dataclasses.dataclass
 class Application(Base):
     Id: str
     Name: str
-    Description: str
+    Description: Optional[str] = ""
 
 
 @dataclasses.dataclass
 class ConfigurationProfile(Base):
     ApplicationId: str
     Id: str
     Name: str
```

### Comparing `appconfig_cli-0.1.0/PKG-INFO` & `appconfig_cli-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 Metadata-Version: 2.1
 Name: appconfig-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: Unofficial CLI tool for working with AWS AppConfig
+Home-page: https://github.com/nicksnell/appconfig-cli
 License: MIT
+Keywords: appconfig,aws,cli,aws-appconfig,appconfig-cli,cli-tool
 Author: Nick Snell
 Author-email: n@nicksnell.com
 Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
 Requires-Dist: boto3 (>=1.27.0,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
+Project-URL: Repository, https://github.com/nicksnell/appconfig-cli
 Description-Content-Type: text/markdown
 
 # AWS AppConfig CLI
 
 **NOTE: This is still early in development**
 
 > CLI tool for working with AWS AppConfig
@@ -44,12 +54,19 @@
 Commands:
   get  Get the current hosted configuration for the application & profile
   put  Upload a new hosted configuration version for the application &...
 ```
 
 ## Examples:
 
-Get current config: `appconf get --app <application name> --profile <profile name>`
-Put new config: `appconf put -a <application name> -p <profile name> path/to/config.json`
-
-
+- Get current config: `appconf get --app <application name> --profile <profile name>`
+- Put new config: 
+  - `appconf put -a <application name> -p <profile name> path/to/config.json`
+  - `appconf put -a <application name> -p <profile name> < cat path/to/config.json`
+  - `cat path/to/config.json | appconf put -a <application name> -p <profile name>`
+
+# Changelog
+
+**0.1.1**
+- Corrected/caught error when retrieving profiles with no configuration
+- Support for pipes when using "put" config
```

