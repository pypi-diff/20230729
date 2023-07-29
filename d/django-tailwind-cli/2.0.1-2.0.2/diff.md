# Comparing `tmp/django_tailwind_cli-2.0.1.tar.gz` & `tmp/django_tailwind_cli-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tailwind_cli-2.0.1.tar", max compression
+gzip compressed data, was "django_tailwind_cli-2.0.2.tar", max compression
```

## Comparing `django_tailwind_cli-2.0.1.tar` & `django_tailwind_cli-2.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-07-29 15:35:32.885572 django_tailwind_cli-2.0.1/LICENSE
--rw-r--r--   0        0        0     2776 2023-07-29 15:35:32.885572 django_tailwind_cli-2.0.1/README.md
--rw-r--r--   0        0        0     2670 2023-07-29 15:35:32.885572 django_tailwind_cli-2.0.1/pyproject.toml
--rw-r--r--   0        0        0       78 2023-07-29 15:35:32.885572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/__init__.py
--rw-r--r--   0        0        0      168 2023-07-29 15:35:32.885572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/apps.py
--rw-r--r--   0        0        0        0 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/management/commands/__init__.py
--rw-r--r--   0        0        0     7592 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/management/commands/tailwind.py
--rw-r--r--   0        0        0        0 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/py.typed
--rw-r--r--   0        0        0       79 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/styles.css
--rw-r--r--   0        0        0      436 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/tailwind.config.js
--rw-r--r--   0        0        0      518 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/templates/tailwind_cli/base.html
--rw-r--r--   0        0        0      257 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
--rw-r--r--   0        0        0        0 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/templatetags/__init__.py
--rw-r--r--   0        0        0      420 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/templatetags/tailwind_cli.py
--rw-r--r--   0        0        0     2905 2023-07-29 15:35:32.889572 django_tailwind_cli-2.0.1/src/django_tailwind_cli/utils.py
--rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 django_tailwind_cli-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-29 18:26:46.365417 django_tailwind_cli-2.0.2/LICENSE
+-rw-r--r--   0        0        0     2776 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/README.md
+-rw-r--r--   0        0        0     2559 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/apps.py
+-rw-r--r--   0        0        0        0 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/management/commands/__init__.py
+-rw-r--r--   0        0        0     7592 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/management/commands/tailwind.py
+-rw-r--r--   0        0        0        0 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/py.typed
+-rw-r--r--   0        0        0       79 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/styles.css
+-rw-r--r--   0        0        0      436 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/tailwind.config.js
+-rw-r--r--   0        0        0      518 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/templates/tailwind_cli/base.html
+-rw-r--r--   0        0        0      257 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
+-rw-r--r--   0        0        0        0 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/templatetags/__init__.py
+-rw-r--r--   0        0        0      420 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/templatetags/tailwind_cli.py
+-rw-r--r--   0        0        0     3016 2023-07-29 18:26:46.369417 django_tailwind_cli-2.0.2/src/django_tailwind_cli/utils.py
+-rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 django_tailwind_cli-2.0.2/PKG-INFO
```

### Comparing `django_tailwind_cli-2.0.1/LICENSE` & `django_tailwind_cli-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.0.1/README.md` & `django_tailwind_cli-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.0.1/pyproject.toml` & `django_tailwind_cli-2.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-tailwind-cli"
-version = "2.0.1"
+version = "2.0.2"
 description = "Django and Tailwind integration based on the prebuilt Tailwind CSS CLI."
 license = "MIT"
 authors = ["Oliver Andrich <oliver@andrich.me>"]
 readme = "README.md"
 homepage = "https://oliverandrich.github.io/django-tailwind-cli/"
 repository = "https://github.com/oliverandrich/django-tailwind-cli"
 keywords = ["django", "tailwind", "css"]
@@ -31,21 +31,16 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 django = ">=3.2,<5"
 certifi = "*"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
-pytest-django = "^4.5.2"
 django-types = "^0.17.0"
-pytest-randomly = "^3.12.0"
 mkdocs-material = "^9.1.5"
-syrupy = "^4.0.1"
 tox = "^4.6.4"
 tox-gh-actions = "^3.1.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_tailwind_cli-2.0.1/src/django_tailwind_cli/management/commands/tailwind.py` & `django_tailwind_cli-2.0.2/src/django_tailwind_cli/management/commands/tailwind.py`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.0.1/src/django_tailwind_cli/templates/tailwind_cli/base.html` & `django_tailwind_cli-2.0.2/src/django_tailwind_cli/templates/tailwind_cli/base.html`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.0.1/src/django_tailwind_cli/utils.py` & `django_tailwind_cli-2.0.2/src/django_tailwind_cli/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 
 This module contains utility functions to read the configuration, download the CLI and determine
 the various paths.
 """
 
 import platform
 from pathlib import Path
+from typing import Union
 
 from django.conf import settings
 
 
 class Config:
     """Configuration for the Tailwind CSS CLI."""
 
     def __init__(self):
         """Initialize the configuration."""
         self.tailwind_version: str = getattr(settings, "TAILWIND_CLI_VERSION", "3.3.3")
-        self.cli_path: str | None = getattr(settings, "TAILWIND_CLI_PATH", None)
-        self.src_css: str | None = getattr(settings, "TAILWIND_CLI_SRC_CSS", None)
+        self.cli_path: Union[str, None] = getattr(settings, "TAILWIND_CLI_PATH", None)
+        self.src_css: Union[str, None] = getattr(settings, "TAILWIND_CLI_SRC_CSS", None)
         self.dist_css: str = getattr(settings, "TAILWIND_CLI_DIST_CSS", "css/tailwind.css")
         self.config_file: str = getattr(settings, "TAILWIND_CLI_CONFIG_FILE", "tailwind.config.js")
 
     def validate_settings(self) -> None:
         """Validate the settings."""
-        if len(settings.STATICFILES_DIRS) == 0:
+        if settings.STATICFILES_DIRS is None or len(settings.STATICFILES_DIRS) == 0:
             raise ValueError("STATICFILES_DIRS is empty. Please add a path to your static files.")
 
     def get_system_and_machine(self) -> tuple[str, str]:
         """Get the system and machine name."""
         system = platform.system().lower()
         if system == "darwin":  # pragma: no cover
             system = "macos"
@@ -60,15 +61,15 @@
         """Get path to the source css."""
         if self.src_css is None:
             raise ValueError("No source CSS file specified. Please set TAILWIND_SRC_CSS in your settings.")
         return Path(settings.BASE_DIR) / self.src_css
 
     def get_full_dist_css_path(self) -> Path:
         """Get path to the compiled css."""
-        if len(settings.STATICFILES_DIRS) == 0:
+        if settings.STATICFILES_DIRS is None or len(settings.STATICFILES_DIRS) == 0:
             raise ValueError("STATICFILES_DIRS is empty. Please add a path to your static files.")
 
         return Path(settings.STATICFILES_DIRS[0]) / self.dist_css
 
     def get_full_config_file_path(self) -> Path:
         """Get path to the tailwind.config.js file."""
         return Path(settings.BASE_DIR) / self.config_file
```

### Comparing `django_tailwind_cli-2.0.1/PKG-INFO` & `django_tailwind_cli-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tailwind-cli
-Version: 2.0.1
+Version: 2.0.2
 Summary: Django and Tailwind integration based on the prebuilt Tailwind CSS CLI.
 Home-page: https://oliverandrich.github.io/django-tailwind-cli/
 License: MIT
 Keywords: django,tailwind,css
 Author: Oliver Andrich
 Author-email: oliver@andrich.me
 Requires-Python: >=3.9,<4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.0.1 Summary: Django
+Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.0.2 Summary: Django
 and Tailwind integration based on the prebuilt Tailwind CSS CLI. Home-page:
 https://oliverandrich.github.io/django-tailwind-cli/ License: MIT Keywords:
 django,tailwind,css Author: Oliver Andrich Author-email: oliver@andrich.me
 Requires-Python: >=3.9,<4 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Web Environment Classifier: Framework ::
 Django :: 3.2 Classifier: Framework :: Django :: 4.0 Classifier: Framework ::
 Django :: 4.1 Classifier: Framework :: Django :: 4.2 Classifier: Intended
```

