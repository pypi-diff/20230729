# Comparing `tmp/django_tailwind_cli-1.4.3.tar.gz` & `tmp/django_tailwind_cli-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tailwind_cli-1.4.3.tar", max compression
+gzip compressed data, was "django_tailwind_cli-2.0.1.tar", max compression
```

## Comparing `django_tailwind_cli-1.4.3.tar` & `django_tailwind_cli-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/LICENSE
--rw-r--r--   0        0        0     2836 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/README.md
--rw-r--r--   0        0        0     2725 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/pyproject.toml
--rw-r--r--   0        0        0       78 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/__init__.py
--rw-r--r--   0        0        0      168 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/apps.py
--rw-r--r--   0        0        0        0 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/management/commands/__init__.py
--rw-r--r--   0        0        0     4712 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/management/commands/tailwind.py
--rw-r--r--   0        0        0        0 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/py.typed
--rw-r--r--   0        0        0       79 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/styles.css
--rw-r--r--   0        0        0      436 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/tailwind.config.js
--rw-r--r--   0        0        0      518 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/templates/tailwind_cli/base.html
--rw-r--r--   0        0        0      257 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
--rw-r--r--   0        0        0        0 2023-04-10 14:22:18.817436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/templatetags/__init__.py
--rw-r--r--   0        0        0      463 2023-04-10 14:22:18.821436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/templatetags/tailwind_cli.py
--rw-r--r--   0        0        0     2961 2023-04-10 14:22:18.821436 django_tailwind_cli-1.4.3/src/django_tailwind_cli/utils.py
--rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 django_tailwind_cli-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-29 15:35:32.885572 django_tailwind_cli-2.0.1/LICENSE
+-rw-r--r--   0        0        0     2776 2023-07-29 15:35:32.885572 django_tailwind_cli-2.0.1/README.md
+-rw-r--r--   0        0        0     2670 2023-07-29 15:35:32.885572 django_tailwind_cli-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-07-29 15:35:32.885572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-29 15:35:32.885572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/apps.py
+-rw-r--r--   0        0        0        0 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/management/commands/__init__.py
+-rw-r--r--   0        0        0     7592 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/management/commands/tailwind.py
+-rw-r--r--   0        0        0        0 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/py.typed
+-rw-r--r--   0        0        0       79 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/styles.css
+-rw-r--r--   0        0        0      436 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/tailwind.config.js
+-rw-r--r--   0        0        0      518 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/templates/tailwind_cli/base.html
+-rw-r--r--   0        0        0      257 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
+-rw-r--r--   0        0        0        0 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/templatetags/__init__.py
+-rw-r--r--   0        0        0      420 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/templatetags/tailwind_cli.py
+-rw-r--r--   0        0        0     2905 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/utils.py
+-rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 django_tailwind_cli-2.0.1/PKG-INFO
```

### Comparing `django_tailwind_cli-1.4.3/LICENSE` & `django_tailwind_cli-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-1.4.3/pyproject.toml` & `django_tailwind_cli-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "django-tailwind-cli"
-version = "1.4.3"
+version = "2.0.1"
 description = "Django and Tailwind integration based on the prebuilt Tailwind CSS CLI."
 license = "MIT"
 authors = ["Oliver Andrich <oliver@andrich.me>"]
 readme = "README.md"
 homepage = "https://oliverandrich.github.io/django-tailwind-cli/"
 repository = "https://github.com/oliverandrich/django-tailwind-cli"
 keywords = ["django", "tailwind", "css"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
     "Environment :: Web Environment",
@@ -27,35 +26,35 @@
 ]
 packages = [{ include = "django_tailwind_cli", from = "src" }]
 
 [tool.poetry.urls]
 "Mastodon" = "https://2pxnl.de/@oliver"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4"
+python = ">=3.9,<4"
 django = ">=3.2,<5"
-django-rich = "^1.5.0"
 certifi = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 pytest-django = "^4.5.2"
 django-types = "^0.17.0"
 pytest-randomly = "^3.12.0"
-pytest-timeout = "^2.1.0"
 mkdocs-material = "^9.1.5"
 syrupy = "^4.0.1"
+tox = "^4.6.4"
+tox-gh-actions = "^3.1.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-target-version = ["py38"]
+target-version = ["py39"]
 line-length = 120
 
 [tool.pyright]
 venvPath = "."
 venv = ".venv"
 typeCheckingMode = "strict"
 
@@ -90,15 +89,15 @@
     "dist",
     "migrations",
     "node_modules",
     "static",
 ]
 line-length = 120
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
-target-version = "py38"
+target-version = "py39"
 
 [tool.ruff.mccabe]
 max-complexity = 10
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["D104"]
 "apps.py" = ["D100", "D101"]
```

### Comparing `django_tailwind_cli-1.4.3/src/django_tailwind_cli/templates/tailwind_cli/base.html` & `django_tailwind_cli-2.0.1/src/django_tailwind_cli/templates/tailwind_cli/base.html`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-1.4.3/src/django_tailwind_cli/utils.py` & `django_tailwind_cli-2.0.1/src/django_tailwind_cli/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,93 +2,73 @@
 Utility functions.
 
 This module contains utility functions to read the configuration, download the CLI and determine
 the various paths.
 """
 
 import platform
-import shutil
-import ssl
-import urllib.request
 from pathlib import Path
-from typing import Dict, Union
 
-import certifi
 from django.conf import settings
 
-DEFAULT_TAILWIND_VERSION = "3.3.1"
 
+class Config:
+    """Configuration for the Tailwind CSS CLI."""
 
-def get_config() -> Dict[str, str]:
-    """Extract configuration from settings."""
-    return {
-        "TAILWIND_VERSION": getattr(settings, "TAILWIND_VERSION", DEFAULT_TAILWIND_VERSION),
-        "TAILWIND_CLI_PATH": getattr(settings, "TAILWIND_CLI_PATH", "~/.local/bin/"),
-        "TAILWIND_THEME_APP": getattr(settings, "TAILWIND_THEME_APP", "theme"),
-        "TAILWIND_SRC_CSS": getattr(settings, "TAILWIND_SRC_CSS", "src/styles.css"),
-        "TAILWIND_DIST_CSS": getattr(settings, "TAILWIND_DIST_CSS", "css/styles.css"),
-    }
-
-
-def get_download_url() -> str:
-    """Build download url for the Tailwind CSS CLI."""
-    config = get_config()
-    version = config["TAILWIND_VERSION"]
-
-    system = platform.system().lower()
-    if system == "darwin":  # pragma: no cover
-        system = "macos"
-
-    machine = platform.machine().lower()
-    if machine == "x86_64":  # pragma: no cover
-        machine = "x64"
-
-    return "https://github.com/tailwindlabs/tailwindcss/releases/download/" f"v{version}/tailwindcss-{system}-{machine}"
-
-
-def get_executable_path(basepath: Union[Path, str, None] = None) -> Path:
-    """Build path where to store the Tailwind CSS CLI locally."""
-    config = get_config()
-
-    version = config["TAILWIND_VERSION"]
-
-    system = platform.system().lower()
-    if system == "darwin":  # pragma: no cover
-        system = "macos"
-
-    machine = platform.machine().lower()
-    if machine == "x86_64":  # pragma: no cover
-        machine = "x64"
-
-    executable_name = f"tailwindcss-{system}-{machine}-{version}"
-
-    if basepath is not None:
-        return Path(basepath).expanduser() / executable_name
-    else:
-        return Path(config["TAILWIND_CLI_PATH"]).expanduser() / executable_name
-
-
-def get_theme_app_path() -> Path:
-    """Build path for the theme app."""
-    config = get_config()
-    return Path(settings.BASE_DIR) / config["TAILWIND_THEME_APP"]
-
-
-def get_src_css_path() -> Path:
-    """Build path to the source css."""
-    config = get_config()
-    return get_theme_app_path() / config["TAILWIND_SRC_CSS"]
-
-
-def get_dist_css_path() -> Path:
-    """Build path to the compiled css."""
-    config = get_config()
-    return get_theme_app_path() / "static" / config["TAILWIND_DIST_CSS"]
-
-
-def download_file(src: str, destination: Path):
-    """Download Tailwind CSS CLI to executable path."""
-    certifi_context = ssl.create_default_context(cafile=certifi.where())
-    with urllib.request.urlopen(src, context=certifi_context) as source, destination.open(mode="wb") as dest:
-        shutil.copyfileobj(source, dest)
-    # make cli executable
-    destination.chmod(0o755)
+    def __init__(self):
+        """Initialize the configuration."""
+        self.tailwind_version: str = getattr(settings, "TAILWIND_CLI_VERSION", "3.3.3")
+        self.cli_path: str | None = getattr(settings, "TAILWIND_CLI_PATH", None)
+        self.src_css: str | None = getattr(settings, "TAILWIND_CLI_SRC_CSS", None)
+        self.dist_css: str = getattr(settings, "TAILWIND_CLI_DIST_CSS", "css/tailwind.css")
+        self.config_file: str = getattr(settings, "TAILWIND_CLI_CONFIG_FILE", "tailwind.config.js")
+
+    def validate_settings(self) -> None:
+        """Validate the settings."""
+        if len(settings.STATICFILES_DIRS) == 0:
+            raise ValueError("STATICFILES_DIRS is empty. Please add a path to your static files.")
+
+    def get_system_and_machine(self) -> tuple[str, str]:
+        """Get the system and machine name."""
+        system = platform.system().lower()
+        if system == "darwin":  # pragma: no cover
+            system = "macos"
+
+        machine = platform.machine().lower()
+        if machine == "x86_64":  # pragma: no cover
+            machine = "x64"
+
+        return (system, machine)
+
+    def get_download_url(self) -> str:
+        """Get the download url for the Tailwind CSS CLI."""
+        system, machine = self.get_system_and_machine()
+        return (
+            "https://github.com/tailwindlabs/tailwindcss/releases/download/"
+            f"v{self.tailwind_version}/tailwindcss-{system}-{machine}"
+        )
+
+    def get_full_cli_path(self) -> Path:
+        """Get path to the Tailwind CSS CLI."""
+        system, machine = self.get_system_and_machine()
+        executable_name = f"tailwindcss-{system}-{machine}-{self.tailwind_version}"
+        if self.cli_path is None:
+            return Path(settings.BASE_DIR) / executable_name
+        else:
+            return Path(self.cli_path).expanduser() / executable_name
+
+    def get_full_src_css_path(self) -> Path:
+        """Get path to the source css."""
+        if self.src_css is None:
+            raise ValueError("No source CSS file specified. Please set TAILWIND_SRC_CSS in your settings.")
+        return Path(settings.BASE_DIR) / self.src_css
+
+    def get_full_dist_css_path(self) -> Path:
+        """Get path to the compiled css."""
+        if len(settings.STATICFILES_DIRS) == 0:
+            raise ValueError("STATICFILES_DIRS is empty. Please add a path to your static files.")
+
+        return Path(settings.STATICFILES_DIRS[0]) / self.dist_css
+
+    def get_full_config_file_path(self) -> Path:
+        """Get path to the tailwind.config.js file."""
+        return Path(settings.BASE_DIR) / self.config_file
```

### Comparing `django_tailwind_cli-1.4.3/PKG-INFO` & `django_tailwind_cli-2.0.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 616e  : 2.1.Name: djan
 00000020: 676f 2d74 6169 6c77 696e 642d 636c 690a  go-tailwind-cli.
-00000030: 5665 7273 696f 6e3a 2031 2e34 2e33 0a53  Version: 1.4.3.S
+00000030: 5665 7273 696f 6e3a 2032 2e30 2e31 0a53  Version: 2.0.1.S
 00000040: 756d 6d61 7279 3a20 446a 616e 676f 2061  ummary: Django a
 00000050: 6e64 2054 6169 6c77 696e 6420 696e 7465  nd Tailwind inte
 00000060: 6772 6174 696f 6e20 6261 7365 6420 6f6e  gration based on
 00000070: 2074 6865 2070 7265 6275 696c 7420 5461   the prebuilt Ta
 00000080: 696c 7769 6e64 2043 5353 2043 4c49 2e0a  ilwind CSS CLI..
 00000090: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
 000000a0: 3a2f 2f6f 6c69 7665 7261 6e64 7269 6368  ://oliverandrich
@@ -14,258 +14,238 @@
 000000d0: 4c69 6365 6e73 653a 204d 4954 0a4b 6579  License: MIT.Key
 000000e0: 776f 7264 733a 2064 6a61 6e67 6f2c 7461  words: django,ta
 000000f0: 696c 7769 6e64 2c63 7373 0a41 7574 686f  ilwind,css.Autho
 00000100: 723a 204f 6c69 7665 7220 416e 6472 6963  r: Oliver Andric
 00000110: 680a 4175 7468 6f72 2d65 6d61 696c 3a20  h.Author-email: 
 00000120: 6f6c 6976 6572 4061 6e64 7269 6368 2e6d  oliver@andrich.m
 00000130: 650a 5265 7175 6972 6573 2d50 7974 686f  e.Requires-Pytho
-00000140: 6e3a 203e 3d33 2e38 2e31 2c3c 340a 436c  n: >=3.8.1,<4.Cl
-00000150: 6173 7369 6669 6572 3a20 4465 7665 6c6f  assifier: Develo
-00000160: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
-00000170: 3520 2d20 5072 6f64 7563 7469 6f6e 2f53  5 - Production/S
-00000180: 7461 626c 650a 436c 6173 7369 6669 6572  table.Classifier
-00000190: 3a20 456e 7669 726f 6e6d 656e 7420 3a3a  : Environment ::
-000001a0: 2057 6562 2045 6e76 6972 6f6e 6d65 6e74   Web Environment
-000001b0: 0a43 6c61 7373 6966 6965 723a 2046 7261  .Classifier: Fra
-000001c0: 6d65 776f 726b 203a 3a20 446a 616e 676f  mework :: Django
-000001d0: 203a 3a20 332e 320a 436c 6173 7369 6669   :: 3.2.Classifi
-000001e0: 6572 3a20 4672 616d 6577 6f72 6b20 3a3a  er: Framework ::
-000001f0: 2044 6a61 6e67 6f20 3a3a 2034 2e30 0a43   Django :: 4.0.C
-00000200: 6c61 7373 6966 6965 723a 2046 7261 6d65  lassifier: Frame
-00000210: 776f 726b 203a 3a20 446a 616e 676f 203a  work :: Django :
-00000220: 3a20 342e 310a 436c 6173 7369 6669 6572  : 4.1.Classifier
-00000230: 3a20 4672 616d 6577 6f72 6b20 3a3a 2044  : Framework :: D
-00000240: 6a61 6e67 6f20 3a3a 2034 2e32 0a43 6c61  jango :: 4.2.Cla
-00000250: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
-00000260: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-00000270: 7665 6c6f 7065 7273 0a43 6c61 7373 6966  velopers.Classif
-00000280: 6965 723a 204c 6963 656e 7365 203a 3a20  ier: License :: 
-00000290: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-000002a0: 4d49 5420 4c69 6365 6e73 650a 436c 6173  MIT License.Clas
-000002b0: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
-000002c0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-000002d0: 6e64 6570 656e 6465 6e74 0a43 6c61 7373  ndependent.Class
-000002e0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-000002f0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000300: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
-00000310: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000320: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000330: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
-00000340: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000350: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000360: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
-00000370: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000380: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000390: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000003a0: 3131 0a43 6c61 7373 6966 6965 723a 2050  11.Classifier: P
-000003b0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000003c0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000003d0: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
-000003e0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-000003f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000400: 203a 3a20 332e 3131 0a43 6c61 7373 6966   :: 3.11.Classif
-00000410: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000420: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000430: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
-00000440: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000450: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000460: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
-00000470: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
-00000480: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-00000490: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
-000004a0: 6965 730a 436c 6173 7369 6669 6572 3a20  ies.Classifier: 
-000004b0: 546f 7069 6320 3a3a 2055 7469 6c69 7469  Topic :: Utiliti
-000004c0: 6573 0a52 6571 7569 7265 732d 4469 7374  es.Requires-Dist
-000004d0: 3a20 6365 7274 6966 690a 5265 7175 6972  : certifi.Requir
-000004e0: 6573 2d44 6973 743a 2064 6a61 6e67 6f20  es-Dist: django 
-000004f0: 283e 3d33 2e32 2c3c 3529 0a52 6571 7569  (>=3.2,<5).Requi
-00000500: 7265 732d 4469 7374 3a20 646a 616e 676f  res-Dist: django
-00000510: 2d72 6963 6820 283e 3d31 2e35 2e30 2c3c  -rich (>=1.5.0,<
-00000520: 322e 302e 3029 0a50 726f 6a65 6374 2d55  2.0.0).Project-U
-00000530: 524c 3a20 4d61 7374 6f64 6f6e 2c20 6874  RL: Mastodon, ht
-00000540: 7470 733a 2f2f 3270 786e 6c2e 6465 2f40  tps://2pxnl.de/@
-00000550: 6f6c 6976 6572 0a50 726f 6a65 6374 2d55  oliver.Project-U
-00000560: 524c 3a20 5265 706f 7369 746f 7279 2c20  RL: Repository, 
-00000570: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000580: 6f6d 2f6f 6c69 7665 7261 6e64 7269 6368  om/oliverandrich
-00000590: 2f64 6a61 6e67 6f2d 7461 696c 7769 6e64  /django-tailwind
-000005a0: 2d63 6c69 0a44 6573 6372 6970 7469 6f6e  -cli.Description
-000005b0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
-000005c0: 6578 742f 6d61 726b 646f 776e 0a0a 2320  ext/markdown..# 
-000005d0: 646a 616e 676f 2d74 6169 6c77 696e 642d  django-tailwind-
-000005e0: 636c 690a 0a21 5b47 6974 4875 6220 576f  cli..![GitHub Wo
-000005f0: 726b 666c 6f77 2053 7461 7475 735d 2868  rkflow Status](h
-00000600: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000610: 6473 2e69 6f2f 6769 7468 7562 2f61 6374  ds.io/github/act
-00000620: 696f 6e73 2f77 6f72 6b66 6c6f 772f 7374  ions/workflow/st
-00000630: 6174 7573 2f6f 6c69 7665 7261 6e64 7269  atus/oliverandri
-00000640: 6368 2f64 6a61 6e67 6f2d 7461 696c 7769  ch/django-tailwi
-00000650: 6e64 2d63 6c69 2f74 6573 742e 796d 6c3f  nd-cli/test.yml?
-00000660: 7374 796c 653d 666c 6174 2d73 7175 6172  style=flat-squar
-00000670: 6529 0a5b 215b 5079 5049 5d28 6874 7470  e).[![PyPI](http
-00000680: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000690: 696f 2f70 7970 692f 762f 646a 616e 676f  io/pypi/v/django
-000006a0: 2d74 6169 6c77 696e 642d 636c 692e 7376  -tailwind-cli.sv
-000006b0: 673f 7374 796c 653d 666c 6174 2d73 7175  g?style=flat-squ
-000006c0: 6172 6529 5d28 6874 7470 733a 2f2f 7079  are)](https://py
-000006d0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f64  pi.org/project/d
-000006e0: 6a61 6e67 6f2d 7461 696c 7769 6e64 2d63  jango-tailwind-c
-000006f0: 6c69 2f29 0a5b 215b 436f 6465 2073 7479  li/).[![Code sty
-00000700: 6c65 3a20 626c 6163 6b5d 2868 7474 7073  le: black](https
-00000710: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000720: 6f2f 6261 6467 652f 636f 6465 2532 3073  o/badge/code%20s
-00000730: 7479 6c65 2d62 6c61 636b 2d30 3030 3030  tyle-black-00000
-00000740: 302e 7376 673f 7374 796c 653d 666c 6174  0.svg?style=flat
-00000750: 2d73 7175 6172 6529 5d28 6874 7470 733a  -square)](https:
-00000760: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7366  //github.com/psf
-00000770: 2f62 6c61 636b 290a 215b 4769 7448 7562  /black).![GitHub
-00000780: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000790: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-000007a0: 6c69 6365 6e73 652f 6f6c 6976 6572 616e  license/oliveran
-000007b0: 6472 6963 682f 646a 616e 676f 2d74 6169  drich/django-tai
-000007c0: 6c77 696e 642d 636c 693f 7374 796c 653d  lwind-cli?style=
-000007d0: 666c 6174 2d73 7175 6172 6529 0a5b 215b  flat-square).[![
-000007e0: 706f 6574 7279 2d6d 616e 6167 6564 5d28  poetry-managed](
-000007f0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000800: 6c64 732e 696f 2f62 6164 6765 2f70 6f65  lds.io/badge/poe
-00000810: 7472 792d 6d61 6e61 6765 642d 626c 7565  try-managed-blue
-00000820: 3f73 7479 6c65 3d66 6c61 742d 7371 7561  ?style=flat-squa
-00000830: 7265 295d 2868 7474 7073 3a2f 2f70 7974  re)](https://pyt
-00000840: 686f 6e2d 706f 6574 7279 2e6f 7267 290a  hon-poetry.org).
-00000850: 0a54 6869 7320 7072 6f6a 6563 7420 7072  .This project pr
-00000860: 6f76 6964 6573 2061 6e20 696e 7465 6772  ovides an integr
-00000870: 6174 696f 6e20 6f66 2054 6169 6c77 696e  ation of Tailwin
-00000880: 6420 4353 5320 666f 7220 446a 616e 676f  d CSS for Django
-00000890: 2074 6861 7420 6973 2062 6173 6564 206f   that is based o
-000008a0: 6e20 7468 6520 7072 6563 6f6d 7069 6c65  n the precompile
-000008b0: 6420 7665 7273 696f 6e73 206f 6620 7468  d versions of th
-000008c0: 6520 5b54 6169 6c77 696e 6420 4353 5320  e [Tailwind CSS 
-000008d0: 434c 495d 2868 7474 7073 3a2f 2f74 6169  CLI](https://tai
-000008e0: 6c77 696e 6463 7373 2e63 6f6d 2f62 6c6f  lwindcss.com/blo
-000008f0: 672f 7374 616e 6461 6c6f 6e65 2d63 6c69  g/standalone-cli
-00000900: 292e 0a0a 4974 2069 7320 696e 7370 6972  )...It is inspir
-00000910: 6564 2062 7920 7468 6520 696d 706c 656d  ed by the implem
-00000920: 656e 7461 7469 6f6e 206f 6620 7468 6520  entation of the 
-00000930: 5b54 6169 6c77 696e 6420 696e 7465 6772  [Tailwind integr
-00000940: 6174 696f 6e20 666f 7220 5068 6f65 6e69  ation for Phoeni
-00000950: 785d 2868 7474 7073 3a2f 2f67 6974 6875  x](https://githu
-00000960: 622e 636f 6d2f 7068 6f65 6e69 7866 7261  b.com/phoenixfra
-00000970: 6d65 776f 726b 2f74 6169 6c77 696e 6429  mework/tailwind)
-00000980: 2077 6869 6368 2063 6f6d 706c 6574 656c   which completel
-00000990: 7920 736b 6970 7320 7468 6520 6e65 6363  y skips the necc
-000009a0: 6573 6974 7920 6f66 2061 206e 6f64 6520  esity of a node 
-000009b0: 696e 7374 616c 6c61 7469 6f6e 2e20 536f  installation. So
-000009c0: 2069 7420 6973 2061 2070 6572 6665 6374   it is a perfect
-000009d0: 206d 6174 6368 2c20 6966 2079 6f75 2061   match, if you a
-000009e0: 7265 2061 2075 7365 7220 6f66 205b 6874  re a user of [ht
-000009f0: 6d78 5d28 6874 7470 733a 2f2f 6874 6d78  mx](https://htmx
-00000a00: 2e6f 7267 2920 6f72 2061 6e79 206f 7468  .org) or any oth
-00000a10: 6572 2066 7261 6d65 776f 726b 2074 6861  er framework tha
-00000a20: 7420 7472 6965 7320 746f 2061 766f 6964  t tries to avoid
-00000a30: 204a 6176 6153 6372 6970 7420 636f 6469   JavaScript codi
-00000a40: 6e67 2069 6e20 796f 7572 2077 6562 2061  ng in your web a
-00000a50: 7070 2e20 4d79 2070 6572 736f 6e61 6c20  pp. My personal 
-00000a60: 6d6f 7469 7661 7469 6f6e 2077 6173 2c20  motivation was, 
-00000a70: 7468 6174 2049 2064 6973 636f 7665 7265  that I discovere
-00000a80: 6420 7468 6174 2049 206e 6576 6572 206e  d that I never n
-00000a90: 6565 6465 6420 616e 7920 6f74 6865 7220  eeded any other 
-00000aa0: 706c 7567 696e 2062 6573 6964 6573 2074  plugin besides t
-00000ab0: 6865 206f 6666 6963 6961 6c20 706c 7567  he official plug
-00000ac0: 696e 732c 2077 6869 6368 2061 7265 2061  ins, which are a
-00000ad0: 6c72 6561 6479 2069 6e63 6c75 6465 6420  lready included 
-00000ae0: 696e 2074 6865 2043 4c49 2e0a 0a3e 2049  in the CLI...> I
-00000af0: 6620 796f 7520 7761 6e74 2074 6f20 7573  f you want to us
-00000b00: 6520 6e6f 6465 206f 7220 796f 7520 6861  e node or you ha
-00000b10: 7665 2074 6f20 7573 6520 6974 2062 6563  ve to use it bec
-00000b20: 6175 7365 206f 6620 6f74 6865 7220 6465  ause of other de
-00000b30: 7065 6e64 656e 6369 6573 2c20 7468 656e  pendencies, then
-00000b40: 2074 6865 2070 6163 6b61 6765 205b 646a   the package [dj
-00000b50: 616e 676f 2d74 6169 6c77 696e 645d 2868  ango-tailwind](h
-00000b60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000b70: 6d2f 7469 6d6f 6e77 6562 2f64 6a61 6e67  m/timonweb/djang
-00000b80: 6f2d 7461 696c 7769 6e64 2920 6279 205b  o-tailwind) by [
-00000b90: 5469 6d20 4b61 6d61 6d69 6e5d 2868 7474  Tim Kamamin](htt
-00000ba0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000bb0: 7469 6d6f 6e77 6562 2920 6d69 6768 7420  timonweb) might 
-00000bc0: 6265 2061 2062 6574 7465 7220 736f 6c75  be a better solu
-00000bd0: 7469 6f6e 2066 6f72 2079 6f75 2e0a 0a23  tion for you...#
-00000be0: 2320 4665 6174 7572 6573 0a0a 2d20 4d61  # Features..- Ma
-00000bf0: 6e61 6765 6d65 6e74 2043 6f6d 6d61 6e64  nagement Command
-00000c00: 732e 2e2e 0a20 202d 202e 2e2e 746f 2069  s....  - ...to i
-00000c10: 6e73 7461 6c6c 2074 6865 2074 6865 2043  nstall the the C
-00000c20: 4c49 2066 6f72 2079 6f75 7220 6f70 6572  LI for your oper
-00000c30: 6174 696e 6720 7379 7374 656d 2061 6e64  ating system and
-00000c40: 206d 6163 6869 6e65 2061 7263 6869 7465   machine archite
-00000c50: 6374 7572 652e 0a20 202d 202e 2e2e 746f  cture..  - ...to
-00000c60: 2073 7461 7274 2074 6865 2043 4c49 2069   start the CLI i
-00000c70: 6e20 7761 7463 6820 6d6f 6465 2074 6f20  n watch mode to 
-00000c80: 696e 6372 656d 656e 7461 6c6c 7920 636f  incrementally co
-00000c90: 6d70 696c 6520 796f 7572 2073 7479 6c65  mpile your style
-00000ca0: 2073 6865 6574 2e0a 2020 2d20 2e2e 2e74   sheet..  - ...t
-00000cb0: 6f20 6372 6561 7465 2061 2074 6865 6d65  o create a theme
-00000cc0: 2061 7070 2077 6869 6368 2069 6e63 6c75   app which inclu
-00000cd0: 6465 7320 6120 6261 7369 6320 7374 796c  des a basic styl
-00000ce0: 6573 6865 6574 2061 6e64 2061 2074 6169  esheet and a tai
-00000cf0: 6c77 696e 6420 636f 6e66 6967 7572 6174  lwind configurat
-00000d00: 696f 6e20 7768 6963 6820 796f 7520 6361  ion which you ca
-00000d10: 6e20 6578 7465 6e64 2e0a 2020 2d20 2e2e  n extend..  - ..
-00000d20: 2e74 6f20 6275 696c 6420 7468 6520 7072  .to build the pr
-00000d30: 6f64 7563 7469 6f6e 2072 6561 6479 2043  oduction ready C
-00000d40: 5353 2066 696c 652e 0a2d 2041 2074 656d  SS file..- A tem
-00000d50: 706c 6174 6520 7461 6720 746f 2069 6e63  plate tag to inc
-00000d60: 6c75 6465 2074 6865 2043 5353 2066 696c  lude the CSS fil
-00000d70: 6520 696e 2079 6f75 7220 6261 7365 2074  e in your base t
-00000d80: 656d 706c 6174 652e 0a2d 2041 6c6c 2074  emplate..- All t
-00000d90: 6865 206f 6666 6963 6961 6c20 706c 7567  he official plug
-00000da0: 696e 7320 2874 7970 6f67 7261 7068 792c  ins (typography,
-00000db0: 2066 6f72 6d2c 206c 696e 652d 636c 616d   form, line-clam
-00000dc0: 702c 2063 6f6e 7461 696e 6572 2071 7565  p, container que
-00000dd0: 7269 6573 2c20 616e 6420 6173 7065 6374  ries, and aspect
-00000de0: 2d72 6174 696f 2920 696e 7465 6772 6174  -ratio) integrat
-00000df0: 6564 2069 6e20 7468 6520 434c 4920 6172  ed in the CLI ar
-00000e00: 6520 6163 7469 7661 7465 6420 696e 2074  e activated in t
-00000e10: 6865 2064 6566 6175 6c74 2063 6f6e 6669  he default confi
-00000e20: 6775 7261 7469 6f6e 2e0a 0a23 2320 5265  guration...## Re
-00000e30: 7175 6972 656d 656e 7473 0a0a 5079 7468  quirements..Pyth
-00000e40: 6f6e 2033 2e38 206f 7220 6e65 7765 7220  on 3.8 or newer 
-00000e50: 7769 7468 2044 6a61 6e67 6f20 3e3d 2033  with Django >= 3
-00000e60: 2e32 2e0a 0a23 2320 446f 6375 6d65 6e74  .2...## Document
-00000e70: 6174 696f 6e0a 0a54 6865 2064 6f63 756d  ation..The docum
-00000e80: 656e 7461 7469 6f6e 2063 616e 2062 6520  entation can be 
-00000e90: 666f 756e 6420 6174 203c 6874 7470 733a  found at <https:
-00000ea0: 2f2f 6f6c 6976 6572 616e 6472 6963 682e  //oliverandrich.
-00000eb0: 6769 7468 7562 2e69 6f2f 646a 616e 676f  github.io/django
-00000ec0: 2d74 6169 6c77 696e 642d 636c 692f 3e2e  -tailwind-cli/>.
-00000ed0: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-00000ee0: 6e0a 0a60 6060 7368 656c 6c0a 7079 7468  n..```shell.pyth
-00000ef0: 6f6e 202d 6d20 7069 7020 696e 7374 616c  on -m pip instal
-00000f00: 6c20 646a 616e 676f 2d74 6169 6c77 696e  l django-tailwin
-00000f10: 642d 636c 690a 6060 600a 0a43 6865 636b  d-cli.```..Check
-00000f20: 2074 6865 2064 6f63 7320 666f 7220 6465   the docs for de
-00000f30: 7461 696c 6564 205b 696e 7374 616c 6c61  tailed [installa
-00000f40: 7469 6f6e 2069 6e73 7472 7563 7469 6f6e  tion instruction
-00000f50: 735d 2868 7474 7073 3a2f 2f6f 6c69 7665  s](https://olive
-00000f60: 7261 6e64 7269 6368 2e67 6974 6875 622e  randrich.github.
-00000f70: 696f 2f64 6a61 6e67 6f2d 7461 696c 7769  io/django-tailwi
-00000f80: 6e64 2d63 6c69 2f69 6e73 7461 6c6c 6174  nd-cli/installat
-00000f90: 696f 6e2f 292e 0a0a 2323 2042 7567 7320  ion/)...## Bugs 
-00000fa0: 616e 6420 7375 6767 6573 7469 6f6e 730a  and suggestions.
-00000fb0: 0a49 6e20 6361 7365 2079 6f75 2068 6176  .In case you hav
-00000fc0: 6520 666f 756e 6420 6120 6275 6720 6f72  e found a bug or
-00000fd0: 2068 6176 6520 6120 7375 6767 6573 7469   have a suggesti
-00000fe0: 6f6e 2c20 706c 6561 7365 206f 7065 6e20  on, please open 
-00000ff0: 6120 7469 636b 6574 2061 7420 3c68 7474  a ticket at <htt
-00001000: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001010: 6f6c 6976 6572 616e 6472 6963 682f 646a  oliverandrich/dj
-00001020: 616e 676f 2d74 6169 6c77 696e 642d 636c  ango-tailwind-cl
-00001030: 692f 6973 7375 6573 3e2e 0a0a 2323 204c  i/issues>...## L
-00001040: 6963 656e 7365 0a0a 5468 6973 2073 6f66  icense..This sof
-00001050: 7477 6172 6520 6973 206c 6963 656e 7365  tware is license
-00001060: 6420 756e 6465 7220 5b4d 4954 206c 6963  d under [MIT lic
-00001070: 656e 7365 5d28 6874 7470 733a 2f2f 6769  ense](https://gi
-00001080: 7468 7562 2e63 6f6d 2f6f 6c69 7665 7261  thub.com/olivera
-00001090: 6e64 7269 6368 2f64 6a61 6e67 6f2d 7461  ndrich/django-ta
-000010a0: 696c 7769 6e64 2d63 6c69 2f62 6c6f 622f  ilwind-cli/blob/
-000010b0: 6d61 696e 2f4c 4943 454e 5345 292e 2043  main/LICENSE). C
-000010c0: 6f70 7972 6967 6874 2028 6329 2032 3032  opyright (c) 202
-000010d0: 3220 4f6c 6976 6572 2041 6e64 7269 6368  2 Oliver Andrich
-000010e0: 2e0a 0a                                  ...
+00000140: 6e3a 203e 3d33 2e39 2c3c 340a 436c 6173  n: >=3.9,<4.Clas
+00000150: 7369 6669 6572 3a20 4465 7665 6c6f 706d  sifier: Developm
+00000160: 656e 7420 5374 6174 7573 203a 3a20 3520  ent Status :: 5 
+00000170: 2d20 5072 6f64 7563 7469 6f6e 2f53 7461  - Production/Sta
+00000180: 626c 650a 436c 6173 7369 6669 6572 3a20  ble.Classifier: 
+00000190: 456e 7669 726f 6e6d 656e 7420 3a3a 2057  Environment :: W
+000001a0: 6562 2045 6e76 6972 6f6e 6d65 6e74 0a43  eb Environment.C
+000001b0: 6c61 7373 6966 6965 723a 2046 7261 6d65  lassifier: Frame
+000001c0: 776f 726b 203a 3a20 446a 616e 676f 203a  work :: Django :
+000001d0: 3a20 332e 320a 436c 6173 7369 6669 6572  : 3.2.Classifier
+000001e0: 3a20 4672 616d 6577 6f72 6b20 3a3a 2044  : Framework :: D
+000001f0: 6a61 6e67 6f20 3a3a 2034 2e30 0a43 6c61  jango :: 4.0.Cla
+00000200: 7373 6966 6965 723a 2046 7261 6d65 776f  ssifier: Framewo
+00000210: 726b 203a 3a20 446a 616e 676f 203a 3a20  rk :: Django :: 
+00000220: 342e 310a 436c 6173 7369 6669 6572 3a20  4.1.Classifier: 
+00000230: 4672 616d 6577 6f72 6b20 3a3a 2044 6a61  Framework :: Dja
+00000240: 6e67 6f20 3a3a 2034 2e32 0a43 6c61 7373  ngo :: 4.2.Class
+00000250: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
+00000260: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
+00000270: 6c6f 7065 7273 0a43 6c61 7373 6966 6965  lopers.Classifie
+00000280: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
+00000290: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+000002a0: 5420 4c69 6365 6e73 650a 436c 6173 7369  T License.Classi
+000002b0: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+000002c0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+000002d0: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
+000002e0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000002f0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000300: 686f 6e20 3a3a 2033 0a43 6c61 7373 6966  hon :: 3.Classif
+00000310: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000320: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000330: 686f 6e20 3a3a 2033 2e39 0a43 6c61 7373  hon :: 3.9.Class
+00000340: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000350: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000360: 7974 686f 6e20 3a3a 2033 2e31 300a 436c  ython :: 3.10.Cl
+00000370: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000380: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000390: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
+000003a0: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+000003b0: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
+000003c0: 6576 656c 6f70 6d65 6e74 203a 3a20 4c69  evelopment :: Li
+000003d0: 6272 6172 6965 730a 436c 6173 7369 6669  braries.Classifi
+000003e0: 6572 3a20 546f 7069 6320 3a3a 2055 7469  er: Topic :: Uti
+000003f0: 6c69 7469 6573 0a52 6571 7569 7265 732d  lities.Requires-
+00000400: 4469 7374 3a20 6365 7274 6966 690a 5265  Dist: certifi.Re
+00000410: 7175 6972 6573 2d44 6973 743a 2064 6a61  quires-Dist: dja
+00000420: 6e67 6f20 283e 3d33 2e32 2c3c 3529 0a50  ngo (>=3.2,<5).P
+00000430: 726f 6a65 6374 2d55 524c 3a20 4d61 7374  roject-URL: Mast
+00000440: 6f64 6f6e 2c20 6874 7470 733a 2f2f 3270  odon, https://2p
+00000450: 786e 6c2e 6465 2f40 6f6c 6976 6572 0a50  xnl.de/@oliver.P
+00000460: 726f 6a65 6374 2d55 524c 3a20 5265 706f  roject-URL: Repo
+00000470: 7369 746f 7279 2c20 6874 7470 733a 2f2f  sitory, https://
+00000480: 6769 7468 7562 2e63 6f6d 2f6f 6c69 7665  github.com/olive
+00000490: 7261 6e64 7269 6368 2f64 6a61 6e67 6f2d  randrich/django-
+000004a0: 7461 696c 7769 6e64 2d63 6c69 0a44 6573  tailwind-cli.Des
+000004b0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+000004c0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+000004d0: 646f 776e 0a0a 2320 646a 616e 676f 2d74  down..# django-t
+000004e0: 6169 6c77 696e 642d 636c 690a 0a21 5b47  ailwind-cli..![G
+000004f0: 6974 4875 6220 576f 726b 666c 6f77 2053  itHub Workflow S
+00000500: 7461 7475 735d 2868 7474 7073 3a2f 2f69  tatus](https://i
+00000510: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00000520: 7468 7562 2f61 6374 696f 6e73 2f77 6f72  thub/actions/wor
+00000530: 6b66 6c6f 772f 7374 6174 7573 2f6f 6c69  kflow/status/oli
+00000540: 7665 7261 6e64 7269 6368 2f64 6a61 6e67  verandrich/djang
+00000550: 6f2d 7461 696c 7769 6e64 2d63 6c69 2f74  o-tailwind-cli/t
+00000560: 6573 742e 796d 6c3f 7374 796c 653d 666c  est.yml?style=fl
+00000570: 6174 2d73 7175 6172 6529 0a5b 215b 5079  at-square).[![Py
+00000580: 5049 5d28 6874 7470 733a 2f2f 696d 672e  PI](https://img.
+00000590: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+000005a0: 762f 646a 616e 676f 2d74 6169 6c77 696e  v/django-tailwin
+000005b0: 642d 636c 692e 7376 673f 7374 796c 653d  d-cli.svg?style=
+000005c0: 666c 6174 2d73 7175 6172 6529 5d28 6874  flat-square)](ht
+000005d0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+000005e0: 726f 6a65 6374 2f64 6a61 6e67 6f2d 7461  roject/django-ta
+000005f0: 696c 7769 6e64 2d63 6c69 2f29 0a5b 215b  ilwind-cli/).[![
+00000600: 436f 6465 2073 7479 6c65 3a20 626c 6163  Code style: blac
+00000610: 6b5d 2868 7474 7073 3a2f 2f69 6d67 2e73  k](https://img.s
+00000620: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000630: 636f 6465 2532 3073 7479 6c65 2d62 6c61  code%20style-bla
+00000640: 636b 2d30 3030 3030 302e 7376 673f 7374  ck-000000.svg?st
+00000650: 796c 653d 666c 6174 2d73 7175 6172 6529  yle=flat-square)
+00000660: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000670: 2e63 6f6d 2f70 7366 2f62 6c61 636b 290a  .com/psf/black).
+00000680: 215b 4769 7448 7562 5d28 6874 7470 733a  ![GitHub](https:
+00000690: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000006a0: 2f67 6974 6875 622f 6c69 6365 6e73 652f  /github/license/
+000006b0: 6f6c 6976 6572 616e 6472 6963 682f 646a  oliverandrich/dj
+000006c0: 616e 676f 2d74 6169 6c77 696e 642d 636c  ango-tailwind-cl
+000006d0: 693f 7374 796c 653d 666c 6174 2d73 7175  i?style=flat-squ
+000006e0: 6172 6529 0a5b 215b 706f 6574 7279 2d6d  are).[![poetry-m
+000006f0: 616e 6167 6564 5d28 6874 7470 733a 2f2f  anaged](https://
+00000700: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000710: 6164 6765 2f70 6f65 7472 792d 6d61 6e61  adge/poetry-mana
+00000720: 6765 642d 626c 7565 3f73 7479 6c65 3d66  ged-blue?style=f
+00000730: 6c61 742d 7371 7561 7265 295d 2868 7474  lat-square)](htt
+00000740: 7073 3a2f 2f70 7974 686f 6e2d 706f 6574  ps://python-poet
+00000750: 7279 2e6f 7267 290a 0a54 6869 7320 6c69  ry.org)..This li
+00000760: 6272 6172 7920 7072 6f76 6964 6573 2061  brary provides a
+00000770: 6e20 696e 7465 6772 6174 696f 6e20 6f66  n integration of
+00000780: 205b 5461 696c 7769 6e64 2043 5353 5d28   [Tailwind CSS](
+00000790: 6874 7470 733a 2f2f 7461 696c 7769 6e64  https://tailwind
+000007a0: 6373 732e 636f 6d29 2066 6f72 2044 6a61  css.com) for Dja
+000007b0: 6e67 6f20 7468 6174 2069 7320 7573 696e  ngo that is usin
+000007c0: 6720 6f6e 2074 6865 2070 7265 636f 6d70  g on the precomp
+000007d0: 696c 6564 2076 6572 7369 6f6e 7320 6f66  iled versions of
+000007e0: 2074 6865 205b 5461 696c 7769 6e64 2043   the [Tailwind C
+000007f0: 5353 2043 4c49 5d28 6874 7470 733a 2f2f  SS CLI](https://
+00000800: 7461 696c 7769 6e64 6373 732e 636f 6d2f  tailwindcss.com/
+00000810: 626c 6f67 2f73 7461 6e64 616c 6f6e 652d  blog/standalone-
+00000820: 636c 6929 2e0a 0a54 6865 2067 6f61 6c20  cli)...The goal 
+00000830: 6f66 2074 6869 7320 6c69 6272 6172 7920  of this library 
+00000840: 6973 2074 6f20 7072 6f76 6964 6564 2074  is to provided t
+00000850: 6865 2073 696d 706c 6573 7420 706f 7373  he simplest poss
+00000860: 6962 6c65 2054 6169 6c77 696e 6420 696e  ible Tailwind in
+00000870: 7465 6772 6174 696f 6e20 666f 7220 796f  tegration for yo
+00000880: 7572 2044 6a61 6e67 6f20 7072 6f6a 6563  ur Django projec
+00000890: 742e 2049 7420 746f 6f6b 2069 7473 2069  t. It took its i
+000008a0: 6e73 7069 7261 7469 6f6e 2066 726f 6d20  nspiration from 
+000008b0: 7468 6520 5b54 6169 6c77 696e 6420 696e  the [Tailwind in
+000008c0: 7465 6772 6174 696f 6e20 666f 7220 5068  tegration for Ph
+000008d0: 6f65 6e69 785d 2868 7474 7073 3a2f 2f67  oenix](https://g
+000008e0: 6974 6875 622e 636f 6d2f 7068 6f65 6e69  ithub.com/phoeni
+000008f0: 7866 7261 6d65 776f 726b 2f74 6169 6c77  xframework/tailw
+00000900: 696e 6429 2077 6869 6368 2063 6f6d 706c  ind) which compl
+00000910: 6574 656c 7920 736b 6970 7320 7468 6520  etely skips the 
+00000920: 6e65 6363 6573 6974 7920 6f66 2061 206e  neccesity of a n
+00000930: 6f64 6520 696e 7374 616c 6c61 7469 6f6e  ode installation
+00000940: 2e0a 0a23 2320 496e 7374 616c 6c61 7469  ...## Installati
+00000950: 6f6e 0a0a 312e 2049 6e73 7461 6c6c 2074  on..1. Install t
+00000960: 6865 206c 6962 7261 7279 2e0a 0a20 2020  he library...   
+00000970: 2060 6060 7368 656c 6c0a 2020 2020 7079   ```shell.    py
+00000980: 7468 6f6e 202d 6d20 7069 7020 696e 7374  thon -m pip inst
+00000990: 616c 6c20 646a 616e 676f 2d74 6169 6c77  all django-tailw
+000009a0: 696e 642d 636c 690a 2020 2020 6060 600a  ind-cli.    ```.
+000009b0: 0a32 2e20 4164 6420 6064 6a61 6e67 6f5f  .2. Add `django_
+000009c0: 7461 696c 7769 6e64 5f63 6c69 6020 746f  tailwind_cli` to
+000009d0: 2060 494e 5354 414c 4c45 445f 4150 5053   `INSTALLED_APPS
+000009e0: 6020 696e 2060 7365 7474 696e 6773 2e70  ` in `settings.p
+000009f0: 7960 2e0a 0a20 2020 2060 6060 7079 7468  y`...    ```pyth
+00000a00: 6f6e 0a20 2020 2049 4e53 5441 4c4c 4544  on.    INSTALLED
+00000a10: 5f41 5050 5320 3d20 5b0a 2020 2020 2020  _APPS = [.      
+00000a20: 2020 2320 6f74 6865 7220 446a 616e 676f    # other Django
+00000a30: 2061 7070 730a 2020 2020 2020 2020 2264   apps.        "d
+00000a40: 6a61 6e67 6f5f 7461 696c 7769 6e64 5f63  jango_tailwind_c
+00000a50: 6c69 222c 0a20 2020 205d 0a20 2020 2060  li",.    ].    `
+00000a60: 6060 0a0a 332e 2043 6f6e 6669 6775 7265  ``..3. Configure
+00000a70: 2074 6865 2060 5354 4154 4943 4649 4c45   the `STATICFILE
+00000a80: 535f 4449 5253 6020 7061 7261 6d65 7465  S_DIRS` paramete
+00000a90: 7220 696e 2079 6f75 7220 6073 6574 7469  r in your `setti
+00000aa0: 6e67 732e 7079 6020 6966 206e 6f74 2061  ngs.py` if not a
+00000ab0: 6c72 6561 6479 2063 6f6e 6669 6775 7265  lready configure
+00000ac0: 642e 0a0a 2020 2020 6060 6070 7974 686f  d...    ```pytho
+00000ad0: 6e0a 2020 2020 5354 4154 4943 4649 4c45  n.    STATICFILE
+00000ae0: 535f 4449 5253 203d 205b 4241 5345 5f44  S_DIRS = [BASE_D
+00000af0: 4952 202f 2022 6173 7365 7473 225d 0a20  IR / "assets"]. 
+00000b00: 2020 2060 6060 0a0a 342e 2041 6464 2074     ```..4. Add t
+00000b10: 656d 706c 6174 6520 636f 6465 2e0a 0a20  emplate code... 
+00000b20: 2020 2060 6060 6874 6d6c 646a 616e 676f     ```htmldjango
+00000b30: 0a20 2020 207b 2520 6c6f 6164 2074 6169  .    {% load tai
+00000b40: 6c77 696e 645f 636c 6920 257d 0a20 2020  lwind_cli %}.   
+00000b50: 202e 2e2e 0a20 2020 203c 6865 6164 3e0a   ....    <head>.
+00000b60: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+00000b70: 7b25 2074 6169 6c77 696e 645f 6373 7320  {% tailwind_css 
+00000b80: 257d 0a20 2020 2020 202e 2e2e 0a20 2020  %}.      ....   
+00000b90: 203c 2f68 6561 643e 0a20 2020 2060 6060   </head>.    ```
+00000ba0: 0a0a 352e 2053 7461 7274 2074 6865 2064  ..5. Start the d
+00000bb0: 6562 7567 2073 6572 7665 722e 0a0a 2020  ebug server...  
+00000bc0: 2020 6060 6073 6865 6c6c 0a20 2020 2070    ```shell.    p
+00000bd0: 7974 686f 6e20 6d61 6e61 6765 2e70 7920  ython manage.py 
+00000be0: 7461 696c 7769 6e64 2072 756e 7365 7276  tailwind runserv
+00000bf0: 6572 0a20 2020 2060 6060 0a0a 456e 6a6f  er.    ```..Enjo
+00000c00: 7921 0a0a 2323 2046 6561 7475 7265 730a  y!..## Features.
+00000c10: 0a2d 2020 2053 696d 706c 6573 7420 706f  .-   Simplest po
+00000c20: 7373 6962 6c65 2069 6e74 6567 7261 7469  ssible integrati
+00000c30: 6f6e 2e0a 2d20 2020 4d61 6e61 6765 6d65  on..-   Manageme
+00000c40: 6e74 2063 6f6d 6d61 6e64 733a 0a20 2020  nt commands:.   
+00000c50: 202d 2020 2054 6f20 7374 6172 7420 7468   -   To start th
+00000c60: 6520 5461 696c 7769 6e64 2043 4c49 2069  e Tailwind CLI i
+00000c70: 6e20 7761 7463 6820 6d6f 6465 2064 7572  n watch mode dur
+00000c80: 696e 6720 6465 7665 6c6f 706d 656e 742e  ing development.
+00000c90: 0a20 2020 202d 2020 2054 6f20 6275 696c  .    -   To buil
+00000ca0: 6420 7468 6520 7072 6f64 7563 7469 6f6e  d the production
+00000cb0: 2067 7261 6465 2043 5353 2066 696c 6520   grade CSS file 
+00000cc0: 666f 7220 796f 7572 2070 726f 6a65 6374  for your project
+00000cd0: 2e0a 2020 2020 2d20 2020 546f 2073 7461  ..    -   To sta
+00000ce0: 7274 2061 2064 6562 7567 2073 6572 7665  rt a debug serve
+00000cf0: 7220 616c 6f6e 6720 7769 7468 2074 6865  r along with the
+00000d00: 2054 6169 6c77 696e 6420 434c 4920 696e   Tailwind CLI in
+00000d10: 2077 6174 6368 206d 6f64 6520 696e 2061   watch mode in a
+00000d20: 2073 696e 676c 6520 7365 7373 696f 6e2e   single session.
+00000d30: 0a2d 2020 204e 6563 6573 7361 7279 2063  .-   Necessary c
+00000d40: 6f6e 6669 6775 7261 7469 6f6e 2074 6f20  onfiguration to 
+00000d50: 6164 6170 7420 7468 6520 6c69 6272 6172  adapt the librar
+00000d60: 7920 746f 2079 6f75 7220 7072 6f6a 6563  y to your projec
+00000d70: 742c 2077 6865 6e20 7468 6520 6465 6661  t, when the defa
+00000d80: 756c 7473 2064 6f6e 2774 2066 6974 2079  ults don't fit y
+00000d90: 6f75 2e0a 2d20 2020 4120 7465 6d70 6c61  ou..-   A templa
+00000da0: 7465 2074 6167 2074 6f20 696e 636c 7564  te tag to includ
+00000db0: 6520 7468 6520 5461 696c 7769 6e64 2043  e the Tailwind C
+00000dc0: 5353 2066 696c 6520 696e 2079 6f75 7220  SS file in your 
+00000dd0: 7072 6f6a 6563 742e 0a2d 2020 2041 2062  project..-   A b
+00000de0: 6173 6520 7465 6d70 6c61 7465 2066 6f72  ase template for
+00000df0: 2079 6f75 7220 7072 6f6a 6563 742e 0a2d   your project..-
+00000e00: 2020 2041 2073 616e 6520 7461 696c 7769     A sane tailwi
+00000e10: 6e64 2e63 6f6e 6669 672e 6a73 2074 6861  nd.config.js tha
+00000e20: 7420 6163 7469 7661 7465 7320 616c 6c20  t activates all 
+00000e30: 7468 6520 6f66 6669 6369 616c 2070 6c75  the official plu
+00000e40: 6769 6e73 2061 6e64 2069 6e63 6c75 6465  gins and include
+00000e50: 7320 6120 7369 6d70 6c65 2048 544d 5820  s a simple HTMX 
+00000e60: 706c 7567 696e 2e0a 0a23 2320 446f 6375  plugin...## Docu
+00000e70: 6d65 6e74 6174 696f 6e0a 0a54 6865 2064  mentation..The d
+00000e80: 6f63 756d 656e 7461 7469 6f6e 2063 616e  ocumentation can
+00000e90: 2062 6520 666f 756e 6420 6174 205b 6874   be found at [ht
+00000ea0: 7470 733a 2f2f 646a 616e 676f 2d74 6169  tps://django-tai
+00000eb0: 6c77 696e 642d 636c 692e 616e 6472 6963  lwind-cli.andric
+00000ec0: 682e 6d65 2f5d 2868 7474 7073 3a2f 2f64  h.me/](https://d
+00000ed0: 6a61 6e67 6f2d 7461 696c 7769 6e64 2d63  jango-tailwind-c
+00000ee0: 6c69 2e61 6e64 7269 6368 2e6d 652f 290a  li.andrich.me/).
+00000ef0: 0a23 2320 5265 7175 6972 656d 656e 7473  .## Requirements
+00000f00: 0a0a 5079 7468 6f6e 2033 2e39 206f 7220  ..Python 3.9 or 
+00000f10: 6e65 7765 7220 7769 7468 2044 6a61 6e67  newer with Djang
+00000f20: 6f20 3e3d 2033 2e32 2e0a 0a23 2320 4c69  o >= 3.2...## Li
+00000f30: 6365 6e73 650a 0a54 6869 7320 736f 6674  cense..This soft
+00000f40: 7761 7265 2069 7320 6c69 6365 6e73 6564  ware is licensed
+00000f50: 2075 6e64 6572 205b 4d49 5420 6c69 6365   under [MIT lice
+00000f60: 6e73 655d 2868 7474 7073 3a2f 2f67 6974  nse](https://git
+00000f70: 6875 622e 636f 6d2f 6f6c 6976 6572 616e  hub.com/oliveran
+00000f80: 6472 6963 682f 646a 616e 676f 2d74 6169  drich/django-tai
+00000f90: 6c77 696e 642d 636c 692f 626c 6f62 2f6d  lwind-cli/blob/m
+00000fa0: 6169 6e2f 4c49 4345 4e53 4529 2e0a 0a    ain/LICENSE)...
```

