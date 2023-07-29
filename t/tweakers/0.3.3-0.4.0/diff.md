# Comparing `tmp/tweakers-0.3.3.tar.gz` & `tmp/tweakers-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweakers-0.3.3.tar", last modified: Sat Nov 14 09:58:06 2020, max compression
+gzip compressed data, was "tweakers-0.4.0.tar", max compression
```

## Comparing `tweakers-0.3.3.tar` & `tweakers-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1061 2018-09-18 20:30:13.399104 tweakers-0.3.3/LICENSE
--rw-r--r--   0        0        0     1345 2020-03-15 08:37:33.190987 tweakers-0.3.3/README.md
--rw-r--r--   0        0        0      602 2020-11-13 16:58:30.869869 tweakers-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      163 2020-03-14 10:31:55.118987 tweakers-0.3.3/tweakers/__init__.py
--rw-r--r--   0        0        0      353 2018-12-10 21:56:30.043447 tweakers-0.3.3/tweakers/comment.py
--rw-r--r--   0        0        0      293 2020-11-13 16:57:22.765969 tweakers-0.3.3/tweakers/exceptions.py
--rw-r--r--   0        0        0     1048 2020-11-13 16:34:22.655951 tweakers-0.3.3/tweakers/frontpage.py
--rw-r--r--   0        0        0      976 2020-11-13 16:38:07.165729 tweakers-0.3.3/tweakers/gathering.py
--rw-r--r--   0        0        0     3703 2020-03-14 12:06:54.408706 tweakers-0.3.3/tweakers/parsers.py
--rw-r--r--   0        0        0     2774 2020-11-13 16:34:22.670951 tweakers-0.3.3/tweakers/topic.py
--rw-r--r--   0        0        0      392 2019-05-18 13:03:04.787183 tweakers-0.3.3/tweakers/user.py
--rw-r--r--   0        0        0     2725 2020-11-14 09:43:51.785956 tweakers-0.3.3/tweakers/utils.py
--rw-r--r--   0        0        0     2085 2020-11-14 09:58:06.545951 tweakers-0.3.3/setup.py
--rw-r--r--   0        0        0     2115 2020-11-14 09:58:06.546704 tweakers-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-29 18:51:35.750642 tweakers-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1345 2023-07-29 18:51:35.750642 tweakers-0.4.0/README.md
+-rw-r--r--   0        0        0      766 2023-07-29 18:51:35.754642 tweakers-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-07-29 18:51:35.758642 tweakers-0.4.0/tweakers/__init__.py
+-rw-r--r--   0        0        0      997 2023-07-29 18:51:35.758642 tweakers-0.4.0/tweakers/article.py
+-rw-r--r--   0        0        0      325 2023-07-29 18:51:35.758642 tweakers-0.4.0/tweakers/comment.py
+-rw-r--r--   0        0        0      293 2023-07-29 18:51:35.758642 tweakers-0.4.0/tweakers/exceptions.py
+-rw-r--r--   0        0        0      390 2023-07-29 18:51:35.758642 tweakers-0.4.0/tweakers/frontpage.py
+-rw-r--r--   0        0        0      976 2023-07-29 18:51:35.758642 tweakers-0.4.0/tweakers/gathering.py
+-rw-r--r--   0        0        0     5944 2023-07-29 18:51:35.758642 tweakers-0.4.0/tweakers/parsers.py
+-rw-r--r--   0        0        0     3137 2023-07-29 18:51:35.758642 tweakers-0.4.0/tweakers/topic.py
+-rw-r--r--   0        0        0      775 2023-07-29 18:51:35.758642 tweakers-0.4.0/tweakers/user.py
+-rw-r--r--   0        0        0     2687 2023-07-29 18:51:35.758642 tweakers-0.4.0/tweakers/utils.py
+-rw-r--r--   0        0        0     2207 1970-01-01 00:00:00.000000 tweakers-0.4.0/PKG-INFO
```

### Comparing `tweakers-0.3.3/LICENSE` & `tweakers-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tweakers-0.3.3/README.md` & `tweakers-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tweakers-0.3.3/pyproject.toml` & `tweakers-0.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 [tool.poetry]
 name = "tweakers"
-version = "0.3.3"
+version = "0.4.0"
 description = "A Python wrapper for tweakers.net"
 authors = ["Timo"]
 license = "MIT"
 
 readme = "README.md"
 
 repository = "https://github.com/timotk/tweakers"
 
 classifiers=[
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.6"
+python = ">=3.7,<3.12"
 requests-html = "^0.10.0"
-dateparser = "^0.7.0"
+dateparser = "1.1.8"
 tenacity = "^6.2.0"
+pydantic = "^2.1.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "^4.0"
-pytest-cov = "^2.6"
-black = "^19.10b0"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
+black = "23.3.0"
```

### Comparing `tweakers-0.3.3/tweakers/gathering.py` & `tweakers-0.4.0/tweakers/gathering.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 gathering.tweakers.net (forums).
 """
 
 from typing import List
 
 from requests_html import HTMLResponse
-from .utils import get
-from .topic import Topic
-from . import parsers
 
+from . import parsers
+from .topic import Topic
+from .utils import get
 
 url = "https://gathering.tweakers.net"
 
 
 def active_topics() -> List[Topic]:
     response: HTMLResponse = get(url=f"{url}/forum/list_activetopics")
     topics: List = [Topic(**d) for d in parsers.active_topics(response.html)]
```

### Comparing `tweakers-0.3.3/tweakers/topic.py` & `tweakers-0.4.0/tweakers/topic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 """
 gathering.tweakers.net topics
 """
 
 import time
+from datetime import datetime
+from typing import Any, Generator, List, Optional, Union
 
-from typing import Union, List, Generator
-
+from pydantic import BaseModel
 from requests_html import HTMLResponse
 
-from .utils import id_from_url, get
-from .comment import Comment
+from tweakers.user import User
+
 from . import parsers
+from .comment import Comment
+from .utils import get, id_from_url
 
 
-class Topic:
-    """
-    A topic on gathering.tweakers.net
-    """
-
-    def __init__(self, url, **kwargs) -> None:
-        self.__dict__.update(kwargs)
-        self.url: str = url
-        self.id: int = id_from_url(self.url)
+class Topic(BaseModel):
+    url: str
+    title: Optional[str] = None
+    author: Optional[Union[User, List[User]]] = None
+    last_reply: Optional[datetime] = None
+    comment_count: Optional[int] = None
+    _html: Optional[Any] = None
+
+    @property
+    def id(self) -> int:
+        return id_from_url(self.url)
+
+    @property
+    def html(self):
+        if self._html is None:
+            response = get(self.url)
+            self._html = response.html
+        return self._html
 
     def comments(self, page: Union[int, str]) -> List[Comment]:
         """
         Get comments for a specific Topic page
 
         :param page: Page number (zero indexed) or 'last' for last page.
         :return: A list of Comment objects.
```

### Comparing `tweakers-0.3.3/tweakers/utils.py` & `tweakers-0.4.0/tweakers/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 """
 Utilities.
 """
 from requests import Response
+from requests_html import HTMLResponse, HTMLSession
 from tenacity import (
     retry,
+    retry_if_exception_type,
     stop_after_attempt,
     wait_exponential,
-    retry_if_exception_type,
 )
-from requests_html import HTMLSession, HTMLResponse
 
 from tweakers.exceptions import (
-    RateLimitException,
-    InvalidCredentialsException,
     CaptchaRequiredException,
+    InvalidCredentialsException,
+    RateLimitException,
 )
 
 session = HTMLSession()
 session.headers.update({"X-Cookies-Accepted": "1"})  # Bypass the cookiewall
 
 
 @retry(
     retry=retry_if_exception_type(),
     wait=wait_exponential(multiplier=1, min=5, max=10),
     stop=stop_after_attempt(3),
 )
 def get(url: str) -> HTMLResponse:
     response = session.get(url)
     if response.status_code == 429:
-        print("429, Rate limited...")
         raise RateLimitException()
     if not 200 <= response.status_code < 300:
         raise Exception(f"Url {url} returned a {response.status_code}")
     return response
 
 
 def id_from_url(url: str) -> int:
```

### Comparing `tweakers-0.3.3/PKG-INFO` & `tweakers-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: tweakers
-Version: 0.3.3
+Version: 0.4.0
 Summary: A Python wrapper for tweakers.net
 Home-page: https://github.com/timotk/tweakers
 License: MIT
 Author: Timo
-Requires-Python: >=3.6
+Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: dateparser (>=0.7.0,<0.8.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: dateparser (==1.1.8)
+Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: requests-html (>=0.10.0,<0.11.0)
 Requires-Dist: tenacity (>=6.2.0,<7.0.0)
 Project-URL: Repository, https://github.com/timotk/tweakers
 Description-Content-Type: text/markdown
 
 # Tweakers
 ![Build](https://github.com/timotk/tweakers/workflows/Build/badge.svg)
```

