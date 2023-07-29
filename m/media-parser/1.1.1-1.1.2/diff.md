# Comparing `tmp/media_parser-1.1.1.tar.gz` & `tmp/media_parser-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media_parser-1.1.1.tar", max compression
+gzip compressed data, was "media_parser-1.1.2.tar", max compression
```

## Comparing `media_parser-1.1.1.tar` & `media_parser-1.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-07-28 12:19:33.647356 media_parser-1.1.1/LICENSE
--rw-r--r--   0        0        0     2994 2023-07-28 12:19:33.647356 media_parser-1.1.1/README.md
--rw-r--r--   0        0        0      273 2023-07-28 12:19:33.647356 media_parser-1.1.1/media_parser/__init__.py
--rw-r--r--   0        0        0     1833 2023-07-28 12:19:33.647356 media_parser-1.1.1/media_parser/client.py
--rw-r--r--   0        0        0       44 2023-07-28 12:19:33.647356 media_parser-1.1.1/media_parser/models/__init__.py
--rw-r--r--   0        0        0     2187 2023-07-28 12:19:33.651356 media_parser-1.1.1/media_parser/models/medias.py
--rw-r--r--   0        0        0     1232 2023-07-28 12:19:33.651356 media_parser-1.1.1/media_parser/models/server.py
--rw-r--r--   0        0        0     2753 2023-07-28 12:19:33.651356 media_parser-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4943 1970-01-01 00:00:00.000000 media_parser-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-29 02:19:44.797637 media_parser-1.1.2/LICENSE
+-rw-r--r--   0        0        0     3046 2023-07-29 02:19:44.797637 media_parser-1.1.2/README.md
+-rw-r--r--   0        0        0      273 2023-07-29 02:19:44.801637 media_parser-1.1.2/media_parser/__init__.py
+-rw-r--r--   0        0        0     2280 2023-07-29 02:19:44.801637 media_parser-1.1.2/media_parser/client.py
+-rw-r--r--   0        0        0      307 2023-07-29 02:19:44.801637 media_parser-1.1.2/media_parser/models/__init__.py
+-rw-r--r--   0        0        0     4358 2023-07-29 02:19:44.801637 media_parser-1.1.2/media_parser/models/medias.py
+-rw-r--r--   0        0        0     1405 2023-07-29 02:19:44.801637 media_parser-1.1.2/media_parser/models/server.py
+-rw-r--r--   0        0        0     3039 2023-07-29 02:19:44.805637 media_parser-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4991 1970-01-01 00:00:00.000000 media_parser-1.1.2/PKG-INFO
```

### Comparing `media_parser-1.1.1/LICENSE` & `media_parser-1.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `media_parser-1.1.1/README.md` & `media_parser-1.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 ```
 
 ### Usage
 
 ```python
 from media_parser import Client, FeedbackTypes
 
-client = Client("http://localhost:8000")
+client = Client(url="http://localhost:8000")
 
 
 async def main():
     # Get all media
     media = await client.parse("https://www.youtube.com/watch?v=9bZkp7q19f0", user="jag-k")
     print(media)
 
@@ -131,8 +131,8 @@
     import asyncio
 
     asyncio.run(main())
 ```
 
 ## License
 
-[MIT](LICENSE)
+[MIT](https://github.com/jag-k/media-parser/blob/main/LICENSE)
```

### Comparing `media_parser-1.1.1/media_parser/client.py` & `media_parser-1.1.2/media_parser/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,42 @@
-from enum import Enum
-
 import httpx
 from pydantic import BaseModel, Field, HttpUrl
 
+from models import FeedbackTypes
 from models.medias import GroupedMedia
 
+__all__ = ("Client",)
 
-class FeedbackTypes(str, Enum):
-    not_found = "not_found"
-    wrong_media = "wrong_media"
 
-    other = "other"
+class Client(BaseModel):
+    """
+    Client for media-parser
 
+    :param url: URL to media-parser
+    :param service: Service name (used for feedback)
+    """
 
-class Client(BaseModel):
     url: HttpUrl
     service: str | None = Field(None, description="X-Service in request")
 
     @property
     def client(self):
         return httpx.AsyncClient(base_url=self.url)
 
-    async def parse(
-        self, url: str, use_cache: bool = True, user: str | None = None
-    ) -> GroupedMedia:
+    async def parse(self, url: str, use_cache: bool = True, user: str | None = None) -> GroupedMedia:
+        """
+        Parse media from url
+
+        :param url: URL to parse
+        :param use_cache: Use cache on server
+        :param user: Username (used for feedback)
+
+        :return: GroupedMedia
+        """
+
         headers = {}
         if self.service:
             headers["X-Service"] = self.service
 
         if user:
             headers["X-User"] = user
 
@@ -43,17 +52,25 @@
         event_id: str | None = response.headers.get("X-Sentry-EventID", None)
 
         result = GroupedMedia.parse_obj(response.json())
         result.event_id = event_id
         result.request_url = url
         return result
 
-    async def send_feedback(
-        self, media: GroupedMedia, user: str, feedback_type: FeedbackTypes
-    ):
+    async def send_feedback(self, media: GroupedMedia, user: str, feedback_type: FeedbackTypes):
+        """
+        Send feedback to media-parser
+
+        Its work only if sentry enabled
+
+        :param media: Media
+        :param user: Username
+        :param feedback_type: Feedback type
+        """
+
         headers = {}
         if self.service:
             headers["X-Service"] = self.service
 
         if user:
             headers["X-User"] = user
```

### Comparing `media_parser-1.1.1/media_parser/models/server.py` & `media_parser-1.1.2/media_parser/models/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 from enum import Enum
 from typing import Literal
 
 from pydantic import BaseModel, Field, HttpUrl
 
 from .medias import ParserType
 
+__all__ = (
+    "StatusResponse",
+    "ParserStatus",
+    "ParserStatusResponse",
+    "ParseRequest",
+    "FeedbackTypes",
+    "FeedbackRequest",
+    "FeedbackResponse",
+)
+
 
 class StatusResponse(BaseModel):
     status: str = "ok"
 
 
 class ParserStatus(BaseModel):
     parser_type: ParserType
```

### Comparing `media_parser-1.1.1/pyproject.toml` & `media_parser-1.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "media-parser"
-version = "1.1.1"
+version = "1.1.2"
 description = "API for parsing media from social networks"
 authors = ["Jag_k <me@jagk.dev>"]
 maintainers = ["Jag_k <me@jagk.dev>"]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Framework :: FastAPI",
     "Framework :: Pydantic",
     "Framework :: Pydantic :: 1",
     "Natural Language :: English",
     "Natural Language :: Russian",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Typing :: Typed",
 ]
 homepage = "https://github.com/jag-k/media-parser#readme"
 repository = "https://github.com/jag-k/media-parser"
-documentation = "https://github.com/jag-k/media-parser#clients"
+documentation = "https://media-parser.rtfd.io"
 readme = "README.md"
 license = "MIT"
 keywords = ["media-parser", "poetry", "tiktok", "youtube", "reddit", "twitter"]
 packages = [
     { include = "media_parser/client.py" },
     { include = "media_parser/models" },
     { include = "media_parser/__init__.py" },
@@ -52,14 +52,24 @@
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.280"
 pre-commit = "^3.3.2"
 motor-types = "^1.0.0b2"
 black = { version = "^23.7.0", extras = ["d"] }
 
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^7.1.1"
+furo = "^2023.7.26"
+sphinxext-opengraph = "^0.8.2"
+sphinx-copybutton = "^0.5.2"
+sphinx-inline-tabs = "^2023.4.21"
+myst-parser = "^2.0.0"
+sphinx-autodoc2 = {git = "https://github.com/jag-k/sphinx-autodoc2"}
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 include = '\.pyi?$'
@@ -94,7 +104,8 @@
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402", "F401", "F403", "F405", "F811", "N999"]
 "__main__.py" = ["E402", "F401", "F403", "F405", "F811", "N999"]
+"docs/conf.py" = ["E402"]
```

### Comparing `media_parser-1.1.1/PKG-INFO` & `media_parser-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: media-parser
-Version: 1.1.1
+Version: 1.1.2
 Summary: API for parsing media from social networks
 Home-page: https://github.com/jag-k/media-parser#readme
 License: MIT
 Keywords: media-parser,poetry,tiktok,youtube,reddit,twitter
 Author: Jag_k
 Author-email: me@jagk.dev
 Maintainer: Jag_k
 Maintainer-email: me@jagk.dev
 Requires-Python: >=3.11,<4.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
@@ -33,15 +33,15 @@
 Requires-Dist: jsonref (>=1.1.0,<2.0.0) ; extra == "server" or extra == "all"
 Requires-Dist: motor (>=3.1.2,<4.0.0) ; extra == "server" or extra == "all"
 Requires-Dist: pydantic[dotenv] (>=1.10.9,<2.0.0)
 Requires-Dist: pytube (>=15.0.0,<16.0.0) ; extra == "server" or extra == "all"
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: sentry-sdk[fastapi,httpx,pure-eval,pymongo] (>=1.28.1,<2.0.0) ; extra == "sentry" or extra == "all"
 Requires-Dist: uvicorn (>=0.23.1,<0.24.0) ; extra == "server" or extra == "all"
-Project-URL: Documentation, https://github.com/jag-k/media-parser#clients
+Project-URL: Documentation, https://media-parser.rtfd.io
 Project-URL: Repository, https://github.com/jag-k/media-parser
 Description-Content-Type: text/markdown
 
 # Media Parser
 
 Server for parse Media by URL.
 
@@ -154,15 +154,15 @@
 ```
 
 ### Usage
 
 ```python
 from media_parser import Client, FeedbackTypes
 
-client = Client("http://localhost:8000")
+client = Client(url="http://localhost:8000")
 
 
 async def main():
     # Get all media
     media = await client.parse("https://www.youtube.com/watch?v=9bZkp7q19f0", user="jag-k")
     print(media)
 
@@ -174,9 +174,9 @@
     import asyncio
 
     asyncio.run(main())
 ```
 
 ## License
 
-[MIT](LICENSE)
+[MIT](https://github.com/jag-k/media-parser/blob/main/LICENSE)
```

