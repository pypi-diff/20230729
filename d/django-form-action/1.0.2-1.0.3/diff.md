# Comparing `tmp/django-form-action-1.0.2.tar.gz` & `tmp/django-form-action-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-form-action-1.0.2.tar", last modified: Sat Jun 24 18:32:48 2023, max compression
+gzip compressed data, was "django-form-action-1.0.3.tar", last modified: Sat Jul 29 20:07:18 2023, max compression
```

## Comparing `django-form-action-1.0.2.tar` & `django-form-action-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 18:32:48.766263 django-form-action-1.0.2/
--rw-rw-rw-   0        0        0     1085 2023-03-30 07:18:01.000000 django-form-action-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1094 2023-06-24 18:32:48.765243 django-form-action-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      492 2023-06-24 18:27:46.000000 django-form-action-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 18:32:48.761223 django-form-action-1.0.2/django_form_action.egg-info/
--rw-rw-rw-   0        0        0       50 2023-06-24 18:32:48.000000 django-form-action-1.0.2/django_form_action.egg-info/SOURCES.txt
-drwxrwxrwx   0        0        0        0 2023-06-24 18:32:48.755205 django-form-action-1.0.2/form_action/
--rw-rw-rw-   0        0        0     2447 2023-06-24 18:31:49.000000 django-form-action-1.0.2/form_action/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-24 18:32:48.768239 django-form-action-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-06-24 18:32:04.000000 django-form-action-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:07:18.893686 django-form-action-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-29 20:07:01.000000 django-form-action-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-29 20:07:18.893686 django-form-action-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-29 20:07:01.000000 django-form-action-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:07:18.889686 django-form-action-1.0.3/django_form_action.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-29 20:07:18.000000 django-form-action-1.0.3/django_form_action.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 20:07:18.889686 django-form-action-1.0.3/form_action/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-29 20:07:01.000000 django-form-action-1.0.3/form_action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 20:07:18.893686 django-form-action-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-29 20:07:01.000000 django-form-action-1.0.3/setup.py
```

### Comparing `django-form-action-1.0.2/LICENSE` & `django-form-action-1.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Sandbox
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Sandbox
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `django-form-action-1.0.2/setup.py` & `django-form-action-1.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="django-form-action",
-    version="1.0.2",
-    author="Pradish Bijukchhe",
-    author_email="pradishbijukchhe@gmail.com",
-    description="Django action to add an intermediate page to parse form data",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/sandbox-pokhara/django-form-action",
-    project_urls={
-        "Bug Tracker": "https://github.com/sandbox-pokhara/django-form-action/issues",
-    },
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: Microsoft :: Windows",
-    ],
-    include_package_data=True,
-    package_dir={"form_action": "form_action"},
-    python_requires=">=3",
-    install_requires=["django"],
-)
+import setuptools
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="django-form-action",
+    version="1.0.3",
+    author="Pradish Bijukchhe",
+    author_email="pradishbijukchhe@gmail.com",
+    description="Django action to add an intermediate page to parse form data",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/sandbox-pokhara/django-form-action",
+    project_urls={
+        "Bug Tracker": "https://github.com/sandbox-pokhara/django-form-action/issues",
+    },
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: Microsoft :: Windows",
+    ],
+    include_package_data=True,
+    package_dir={"form_action": "form_action"},
+    python_requires=">=3",
+    install_requires=["django"],
+)
```

