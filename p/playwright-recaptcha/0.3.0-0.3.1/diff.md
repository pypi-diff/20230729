# Comparing `tmp/playwright-recaptcha-0.3.0.tar.gz` & `tmp/playwright-recaptcha-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwright-recaptcha-0.3.0.tar", last modified: Wed Jul 19 02:38:43 2023, max compression
+gzip compressed data, was "playwright-recaptcha-0.3.1.tar", last modified: Sat Jul 29 16:06:56 2023, max compression
```

## Comparing `playwright-recaptcha-0.3.0.tar` & `playwright-recaptcha-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/playwright_recaptcha/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav2/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19244 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav2/async_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav2/recaptcha_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    18050 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav2/sync_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav3/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav3/async_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav3/sync_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/playwright_recaptcha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-19 02:38:43.000000 playwright-recaptcha-0.3.0/playwright_recaptcha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-19 02:38:43.000000 playwright-recaptcha-0.3.0/playwright_recaptcha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:38:43.000000 playwright-recaptcha-0.3.0/playwright_recaptcha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-19 02:38:43.000000 playwright-recaptcha-0.3.0/playwright_recaptcha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 02:38:43.000000 playwright-recaptcha-0.3.0/playwright_recaptcha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/tests/test_async_recaptchav2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/tests/test_async_recaptchav3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/tests/test_sync_recaptchav2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/tests/test_sync_recaptchav3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:06:56.928236 playwright-recaptcha-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-29 16:06:56.928236 playwright-recaptcha-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:06:56.924235 playwright-recaptcha-0.3.1/playwright_recaptcha/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:06:56.924235 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19240 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/async_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/recaptcha_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/sync_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:06:56.924235 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav3/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav3/async_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav3/sync_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:06:56.924235 playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-29 16:06:56.000000 playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-29 16:06:56.000000 playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 16:06:56.000000 playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-29 16:06:56.000000 playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 16:06:56.000000 playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 16:06:56.928236 playwright-recaptcha-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:06:56.928236 playwright-recaptcha-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/tests/test_async_recaptchav2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/tests/test_async_recaptchav3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/tests/test_sync_recaptchav2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-29 16:06:44.000000 playwright-recaptcha-0.3.1/tests/test_sync_recaptchav3.py
```

### Comparing `playwright-recaptcha-0.3.0/LICENSE` & `playwright-recaptcha-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.0/PKG-INFO` & `playwright-recaptcha-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwright-recaptcha
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library for solving reCAPTCHA v2 and v3 with Playwright
 Home-page: https://github.com/Xewdy444/Playwright-reCAPTCHA
 Author: Xewdy444
 Author-email: xewdy@xewdy.tech
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: playwright-recaptcha Version: 0.3.0 Summary: A
+Metadata-Version: 2.1 Name: playwright-recaptcha Version: 0.3.1 Summary: A
 library for solving reCAPTCHA v2 and v3 with Playwright Home-page: https://
 github.com/Xewdy444/Playwright-reCAPTCHA Author: Xewdy444 Author-email:
 xewdy@xewdy.tech License: MIT Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
```

### Comparing `playwright-recaptcha-0.3.0/README.md` & `playwright-recaptcha-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.0/playwright_recaptcha/__init__.py` & `playwright-recaptcha-0.3.1/playwright_recaptcha/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A library for solving reCAPTCHA v2 and v3 with Playwright."""
 
 __author__ = "Xewdy444"
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __license__ = "MIT"
 
 from playwright_recaptcha.errors import (
     CapSolverError,
     RecaptchaError,
     RecaptchaNotFoundError,
     RecaptchaRateLimitError,
```

### Comparing `playwright-recaptcha-0.3.0/playwright_recaptcha/errors.py` & `playwright-recaptcha-0.3.1/playwright_recaptcha/errors.py`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav2/async_solver.py` & `playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/async_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         self, page: Page, *, attempts: int = 5, capsolver_api_key: Optional[str] = None
     ) -> None:
         self._page = page
         self._attempts = attempts
         self._capsolver_api_key = capsolver_api_key or os.getenv("CAPSOLVER_API_KEY")
 
         self._token: Optional[str] = None
-        self._payload_response: Optional[Union[APIResponse, Response]] = None
+        self._payload_response: Union[APIResponse, Response, None] = None
         self._page.on("response", self._response_listener)
 
     def __repr__(self) -> str:
         return (
             f"AsyncSolver(page={self._page!r}, "
             f"attempts={self._attempts!r}, "
             f"capsolver_api_key={self._capsolver_api_key!r})"
```

### Comparing `playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav2/recaptcha_box.py` & `playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/recaptcha_box.py`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav2/sync_solver.py` & `playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav2/sync_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self, page: Page, *, attempts: int = 5, capsolver_api_key: Optional[str] = None
     ) -> None:
         self._page = page
         self._attempts = attempts
         self._capsolver_api_key = capsolver_api_key or os.getenv("CAPSOLVER_API_KEY")
 
         self._token: Optional[str] = None
-        self._payload_response: Optional[Union[APIResponse, Response]] = None
+        self._payload_response: Union[APIResponse, Response, None] = None
         self._page.on("response", self._response_listener)
 
     def __repr__(self) -> str:
         return (
             f"SyncSolver(page={self._page!r}, "
             f"attempts={self._attempts!r}, "
             f"capsolver_api_key={self._capsolver_api_key!r})"
```

### Comparing `playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav3/async_solver.py` & `playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav3/async_solver.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         The solve timeout in seconds, by default 30.
     """
 
     def __init__(self, page: Page, timeout: int = 30) -> None:
         self._page = page
         self._timeout = timeout
 
-        self.token: Optional[str] = None
+        self._token: Optional[str] = None
         self._page.on("response", self._extract_token)
 
     def __repr__(self) -> str:
         return f"AsyncSolver(page={self._page!r}, timeout={self._timeout!r})"
 
     async def __aenter__(self) -> AsyncSolver:
         return self
@@ -48,15 +48,15 @@
         """
         if re.search("/recaptcha/(api2|enterprise)/reload", response.url) is None:
             return
 
         token_match = re.search('"rresp","(.*?)"', await response.text())
 
         if token_match is not None:
-            self.token = token_match.group(1)
+            self._token = token_match.group(1)
 
     def close(self) -> None:
         """Remove the reload response listener."""
         try:
             self._page.remove_listener("response", self._extract_token)
         except KeyError:
             pass
@@ -76,18 +76,18 @@
             The `g-recaptcha-response` token.
 
         Raises
         ------
         RecaptchaTimeoutError
             If the solve timeout has been exceeded.
         """
-        self.token = None
+        self._token = None
         timeout = timeout or self._timeout
         start_time = time.time()
 
-        while self.token is None:
+        while self._token is None:
             if time.time() - start_time >= timeout:
                 raise RecaptchaTimeoutError
 
             await self._page.wait_for_timeout(250)
 
-        return self.token
+        return self._token
```

### Comparing `playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav3/sync_solver.py` & `playwright-recaptcha-0.3.1/playwright_recaptcha/recaptchav3/sync_solver.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         The solve timeout in seconds, by default 30.
     """
 
     def __init__(self, page: Page, timeout: int = 30) -> None:
         self._page = page
         self._timeout = timeout
 
-        self.token: Optional[str] = None
+        self._token: Optional[str] = None
         self._page.on("response", self._extract_token)
 
     def __repr__(self) -> str:
         return f"SyncSolver(page={self._page!r}, timeout={self._timeout!r})"
 
     def __enter__(self) -> SyncSolver:
         return self
@@ -48,15 +48,15 @@
         """
         if re.search("/recaptcha/(api2|enterprise)/reload", response.url) is None:
             return
 
         token_match = re.search('"rresp","(.*?)"', response.text())
 
         if token_match is not None:
-            self.token = token_match.group(1)
+            self._token = token_match.group(1)
 
     def close(self) -> None:
         """Remove the reload response listener."""
         try:
             self._page.remove_listener("response", self._extract_token)
         except KeyError:
             pass
@@ -76,20 +76,18 @@
             The `g-recaptcha-response` token.
 
         Raises
         ------
         RecaptchaTimeoutError
             If the solve timeout has been exceeded.
         """
-        self.token = None
-        self._page.on("response", self._extract_token)
-
+        self._token = None
         timeout = timeout or self._timeout
         start_time = time.time()
 
-        while self.token is None:
+        while self._token is None:
             if time.time() - start_time >= timeout:
                 raise RecaptchaTimeoutError
 
             self._page.wait_for_timeout(250)
 
-        return self.token
+        return self._token
```

### Comparing `playwright-recaptcha-0.3.0/playwright_recaptcha.egg-info/PKG-INFO` & `playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwright-recaptcha
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library for solving reCAPTCHA v2 and v3 with Playwright
 Home-page: https://github.com/Xewdy444/Playwright-reCAPTCHA
 Author: Xewdy444
 Author-email: xewdy@xewdy.tech
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: playwright-recaptcha Version: 0.3.0 Summary: A
+Metadata-Version: 2.1 Name: playwright-recaptcha Version: 0.3.1 Summary: A
 library for solving reCAPTCHA v2 and v3 with Playwright Home-page: https://
 github.com/Xewdy444/Playwright-reCAPTCHA Author: Xewdy444 Author-email:
 xewdy@xewdy.tech License: MIT Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
```

### Comparing `playwright-recaptcha-0.3.0/playwright_recaptcha.egg-info/SOURCES.txt` & `playwright-recaptcha-0.3.1/playwright_recaptcha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.0/setup.py` & `playwright-recaptcha-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="utf-8") as file:
     long_description = file.read()
 
 setup(
     name="playwright-recaptcha",
-    version="0.3.0",
+    version="0.3.1",
     author="Xewdy444",
     author_email="xewdy@xewdy.tech",
     description="A library for solving reCAPTCHA v2 and v3 with Playwright",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Xewdy444/Playwright-reCAPTCHA",
```

### Comparing `playwright-recaptcha-0.3.0/tests/test_async_recaptchav2.py` & `playwright-recaptcha-0.3.1/tests/test_async_recaptchav2.py`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.0/tests/test_async_recaptchav3.py` & `playwright-recaptcha-0.3.1/tests/test_async_recaptchav3.py`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.0/tests/test_sync_recaptchav2.py` & `playwright-recaptcha-0.3.1/tests/test_sync_recaptchav2.py`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.3.0/tests/test_sync_recaptchav3.py` & `playwright-recaptcha-0.3.1/tests/test_sync_recaptchav3.py`

 * *Files identical despite different names*

