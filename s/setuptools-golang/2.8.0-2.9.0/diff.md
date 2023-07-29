# Comparing `tmp/setuptools_golang-2.8.0.tar.gz` & `tmp/setuptools_golang-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools_golang-2.8.0.tar", last modified: Sat Jun 10 19:08:29 2023, max compression
+gzip compressed data, was "setuptools_golang-2.9.0.tar", last modified: Sat Jul 29 20:05:22 2023, max compression
```

## Comparing `setuptools_golang-2.8.0.tar` & `setuptools_golang-2.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 19:08:29.846438 setuptools_golang-2.8.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-10 18:44:26.000000 setuptools_golang-2.8.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4800 2023-06-10 19:08:29.846438 setuptools_golang-2.8.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4147 2023-06-10 18:44:26.000000 setuptools_golang-2.8.0/README.md
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1367 2023-06-10 19:08:29.846438 setuptools_golang-2.8.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-10 18:44:26.000000 setuptools_golang-2.8.0/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 19:08:29.846438 setuptools_golang-2.8.0/setuptools_golang.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4800 2023-06-10 19:08:29.000000 setuptools_golang-2.8.0/setuptools_golang.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      305 2023-06-10 19:08:29.000000 setuptools_golang-2.8.0/setuptools_golang.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-10 19:08:29.000000 setuptools_golang-2.8.0/setuptools_golang.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)      177 2023-06-10 19:08:29.000000 setuptools_golang-2.8.0/setuptools_golang.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       11 2023-06-10 19:08:29.000000 setuptools_golang-2.8.0/setuptools_golang.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       18 2023-06-10 19:08:29.000000 setuptools_golang-2.8.0/setuptools_golang.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7966 2023-06-10 18:44:26.000000 setuptools_golang-2.8.0/setuptools_golang.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 20:05:22.923371 setuptools_golang-2.9.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-07-29 20:05:02.000000 setuptools_golang-2.9.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4800 2023-07-29 20:05:22.923371 setuptools_golang-2.9.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4147 2023-07-29 20:05:02.000000 setuptools_golang-2.9.0/README.md
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1367 2023-07-29 20:05:22.923371 setuptools_golang-2.9.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-07-29 20:05:02.000000 setuptools_golang-2.9.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-29 20:05:22.923371 setuptools_golang-2.9.0/setuptools_golang.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4800 2023-07-29 20:05:22.000000 setuptools_golang-2.9.0/setuptools_golang.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      305 2023-07-29 20:05:22.000000 setuptools_golang-2.9.0/setuptools_golang.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-07-29 20:05:22.000000 setuptools_golang-2.9.0/setuptools_golang.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      177 2023-07-29 20:05:22.000000 setuptools_golang-2.9.0/setuptools_golang.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       11 2023-07-29 20:05:22.000000 setuptools_golang-2.9.0/setuptools_golang.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       18 2023-07-29 20:05:22.000000 setuptools_golang-2.9.0/setuptools_golang.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7947 2023-07-29 20:05:02.000000 setuptools_golang-2.9.0/setuptools_golang.py
```

### Comparing `setuptools_golang-2.8.0/LICENSE` & `setuptools_golang-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools_golang-2.8.0/PKG-INFO` & `setuptools_golang-2.9.0/setuptools_golang.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: setuptools_golang
-Version: 2.8.0
+Name: setuptools-golang
+Version: 2.9.0
 Summary: A setuptools extension for building cpython extensions written in golang.
 Home-page: https://github.com/asottile/setuptools-golang
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![build status](https://github.com/asottile/setuptools-golang/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/setuptools-golang/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setuptools-golang/main.svg)](https://results.pre-commit.ci/latest/github/asottile/setuptools-golang/main)
 
 setuptools-golang
```

### Comparing `setuptools_golang-2.8.0/README.md` & `setuptools_golang-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `setuptools_golang-2.8.0/setup.cfg` & `setuptools_golang-2.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = setuptools_golang
-version = 2.8.0
+version = 2.9.0
 description = A setuptools extension for building cpython extensions written in golang.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/setuptools-golang
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
@@ -16,15 +16,15 @@
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 py_modules = setuptools_golang
 install_requires = 
 	setuptools
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	setuptools-golang-build-manylinux-wheels = setuptools_golang:build_manylinux_wheels
 distutils.setup_keywords = 
 	build_golang = setuptools_golang:set_build_ext
```

### Comparing `setuptools_golang-2.8.0/setuptools_golang.egg-info/PKG-INFO` & `setuptools_golang-2.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: setuptools-golang
-Version: 2.8.0
+Name: setuptools_golang
+Version: 2.9.0
 Summary: A setuptools extension for building cpython extensions written in golang.
 Home-page: https://github.com/asottile/setuptools-golang
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![build status](https://github.com/asottile/setuptools-golang/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/setuptools-golang/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setuptools-golang/main.svg)](https://results.pre-commit.ci/latest/github/asottile/setuptools-golang/main)
 
 setuptools-golang
```

### Comparing `setuptools_golang-2.8.0/setuptools_golang.py` & `setuptools_golang-2.9.0/setuptools_golang.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,43 +72,39 @@
 
 def _get_ldflags() -> str:
     """Determine the correct link flags.  This attempts compiles similar
     to how autotools does feature detection.
     """
     # windows gcc does not support linking with unresolved symbols
     if sys.platform == 'win32':  # pragma: win32 cover
-        prefix = getattr(sys, 'real_prefix', sys.prefix)
-        libs = os.path.join(prefix, 'libs')
-        return '-L{} -lpython{}{}'.format(libs, *sys.version_info[:2])
-
-    cc = subprocess.check_output(('go', 'env', 'CC')).decode('UTF-8').strip()
-
-    with _tmpdir() as tmpdir:
-        testf = os.path.join(tmpdir, 'test.c')
-        with open(testf, 'w') as f:
-            f.write('int f(int); int main(void) { return f(0); }\n')
-
-        for lflag in LFLAGS:  # pragma: no cover (platform specific)
-            try:
-                subprocess.check_call((cc, testf, lflag), cwd=tmpdir)
-                return lflag
-            except subprocess.CalledProcessError:
-                pass
-        else:  # pragma: no cover (platform specific)
-            # wellp, none of them worked, fall back to gcc and they'll get a
-            # hopefully reasonable error message
-            return LFLAG_GCC
+        libs = os.path.join(sys.base_prefix, 'libs')
+        return f'-L{libs} -lpython{sys.version_info[0]}'
+    else:  # pragma: win32 no cover
+        cc = subprocess.check_output(('go', 'env', 'CC')).decode().strip()
+
+        with _tmpdir() as tmpdir:
+            testf = os.path.join(tmpdir, 'test.c')
+            with open(testf, 'w') as f:
+                f.write('int f(int); int main(void) { return f(0); }\n')
+
+            for lflag in LFLAGS:  # pragma: no cover (platform specific)
+                try:
+                    subprocess.check_call((cc, testf, lflag), cwd=tmpdir)
+                    return lflag
+                except subprocess.CalledProcessError:
+                    pass
+            else:  # pragma: no cover (platform specific)
+                # wellp, none of them worked, fall back to gcc and they'll get
+                # a hopefully reasonable error message
+                return LFLAG_GCC
 
 
 def _check_call(cmd: tuple[str, ...], cwd: str, env: dict[str, str]) -> None:
     envparts = [f'{k}={shlex.quote(v)}' for k, v in sorted(tuple(env.items()))]
-    print(
-        '$ {}'.format(' '.join(envparts + [shlex.quote(p) for p in cmd])),
-        file=sys.stderr,
-    )
+    print(f'$ {" ".join(envparts)} {shlex.join(cmd)}', file=sys.stderr)
     subprocess.check_call(cmd, cwd=cwd, env=dict(os.environ, **env))
 
 
 def _get_build_extension_method(
         base: type[_build_ext],
         root: str,
         strip: bool,
```

