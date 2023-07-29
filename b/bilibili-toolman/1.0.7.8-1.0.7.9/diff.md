# Comparing `tmp/bilibili-toolman-1.0.7.8.tar.gz` & `tmp/bilibili-toolman-1.0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilibili-toolman-1.0.7.8.tar", last modified: Sat Jun 17 13:42:47 2023, max compression
+gzip compressed data, was "bilibili-toolman-1.0.7.9.tar", last modified: Sat Jul 29 11:42:07 2023, max compression
```

## Comparing `bilibili-toolman-1.0.7.8.tar` & `bilibili-toolman-1.0.7.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/bilibili_toolman/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/common/
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/common/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/bilibili_toolman/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/cli/precentage_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/cli/sanitizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/bilibili_toolman/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/providers/localfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/bilibili_toolman/providers/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-06-17 13:42:47.000000 bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-17 13:42:47.000000 bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 13:42:47.000000 bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-17 13:42:47.000000 bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-17 13:42:47.000000 bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-17 13:42:47.000000 bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 13:42:47.105503 bilibili-toolman-1.0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-17 13:42:17.000000 bilibili-toolman-1.0.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:42:07.308252 bilibili-toolman-1.0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-29 11:42:07.308252 bilibili-toolman-1.0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:42:07.308252 bilibili-toolman-1.0.7.9/bilibili_toolman/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/bilibili_toolman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/bilibili_toolman/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:42:07.308252 bilibili-toolman-1.0.7.9/bilibili_toolman/bilisession/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/bilibili_toolman/bilisession/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/bilibili_toolman/bilisession/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:42:07.308252 bilibili-toolman-1.0.7.9/bilibili_toolman/bilisession/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/bilibili_toolman/bilisession/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/bilibili_toolman/bilisession/common/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21994 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/bilibili_toolman/bilisession/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:42:07.308252 bilibili-toolman-1.0.7.9/bilibili_toolman/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/bilibili_toolman/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/bilibili_toolman/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/bilibili_toolman/cli/precentage_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/bilibili_toolman/cli/sanitizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:42:07.308252 bilibili-toolman-1.0.7.9/bilibili_toolman/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/bilibili_toolman/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/bilibili_toolman/providers/localfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/bilibili_toolman/providers/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 11:42:07.308252 bilibili-toolman-1.0.7.9/bilibili_toolman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-29 11:42:07.000000 bilibili-toolman-1.0.7.9/bilibili_toolman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-29 11:42:07.000000 bilibili-toolman-1.0.7.9/bilibili_toolman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 11:42:07.000000 bilibili-toolman-1.0.7.9/bilibili_toolman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-29 11:42:07.000000 bilibili-toolman-1.0.7.9/bilibili_toolman.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-29 11:42:07.000000 bilibili-toolman-1.0.7.9/bilibili_toolman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 11:42:07.000000 bilibili-toolman-1.0.7.9/bilibili_toolman.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 11:42:07.308252 bilibili-toolman-1.0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-29 11:41:30.000000 bilibili-toolman-1.0.7.9/setup.py
```

### Comparing `bilibili-toolman-1.0.7.8/LICENSE` & `bilibili-toolman-1.0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.8/PKG-INFO` & `bilibili-toolman-1.0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilibili-toolman
-Version: 1.0.7.8
+Version: 1.0.7.9
 Summary: bilibili-toolman 哔哩哔哩搬运工具
 Home-page: https://github.com/greats3an/bilibili-toolman
 Author: greats3an
 Author-email: greats3an@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bilibili-toolman-1.0.7.8/README.md` & `bilibili-toolman-1.0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/client.py` & `bilibili-toolman-1.0.7.9/bilibili_toolman/bilisession/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,17 +73,17 @@
             (_hash + password).encode("utf-8"), key
         )
 
     @staticmethod
     def sign(data: Union[str, dict]) -> str:
         """salted sign funtion for `dict`(converts to qs then parse) & `str`"""
         if isinstance(data, dict):
-            _str = urlencode(data)
+            _str = urlencode(data,quote_via=quote)
         elif type(data) != str:
-            raise TypeError
+            raise TypeError        
         return Crypto.md5(_str + Crypto.APPSECRET)
 
 class SignedDict(dict):
     @property
     def sorted(self):
         """returns a alphabetically sorted version of `self`"""
         return dict(sorted(self.items()))
@@ -126,23 +126,23 @@
 
 class BiliSession(BiliWebSession):
     """哔哩哔哩上传助手 API"""
 
     TYPE = "client"
 
     UPLOAD_CHUNK_SIZE = 2 * (1 << 20)
-    BUILD_VER = (2, 3, 0, 1088)
+    BUILD_VER = (2, 3, 0, 1092)
     BUILD_NO = int(        
         BUILD_VER[0] * 1e6 + BUILD_VER[1] * 1e5 + BUILD_VER[2] * 1e4 + BUILD_VER[3]
     )
     BUILD_STR = ".".join(map(lambda v: str(v), BUILD_VER))
 
     UPLOAD_PROFILE = "ugcfr/pc3"
 
-    DEFAULT_UA = ""
+    DEFAULT_UA = "PcUploader/2.3.0.1092 os/Windows pc_app/pcUploader build/1092 osVer/10.0_x86_64"
 
     RETRIES_UPLOAD_ID = 5
 
     MISC_MAX_TITLE_LENGTH = 80
     MISC_MAX_DESCRIPTION_LENGTH = 1500  # somehow larger than expected
 
     def __init__(self) -> None:
@@ -336,23 +336,24 @@
             dict
         """
         resp = self.post(
             "https://passport.bilibili.com/x/passport-login/sms/send",
             data=SignedDict(
                 {
                     "appkey": Crypto.APPKEY,
-                    "buvid": "",
+                    "buvid": "00000000-000000000000",
                     "cid": str(cid),
-                    "device_id": "",
-                    "device_name": "",
-                    "device_platform" : "",
+                    "device_id": "000000000000",
+                    "device_name": "ughhh",
+                    "device_platform" : "Windows 10",
                     "platform": "pc",
-                    "tel": str(tel),
-                    "ts": int(time()),
+                    "tel": tel,
+                    "ts": str(int(time())),
                     **(
+            
                         self.login_tokens["gee_captcha"] if "gee_captcha" in self.login_tokens else  {}
                     ),
                 }
             ).signed
         )
         try:
             assert resp.json()["data"]["recaptcha_url"] == ""
```

### Comparing `bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/common/__init__.py` & `bilibili-toolman-1.0.7.9/bilibili_toolman/bilisession/common/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,14 @@
     """__iter__ impl for `FileManager` with i/o usage monitoring"""
 
     tell = None
 
     def __init__(self, path, start, end) -> None:
         self.path, self.start, self.end = path, start, end
 
-    def __getattr__(self, name):  # defining fallback
-        return {}
-
     def __iter__(self):
         start = self.start
         for start in range(self.start, self.end, FileManager.CHUNK_SIZE):
             yield file_manager.read(
                 self.path, start, min(self.end, start + FileManager.CHUNK_SIZE)
             )
         if start + FileManager.CHUNK_SIZE < self.end:
```

### Comparing `bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/common/submission.py` & `bilibili-toolman-1.0.7.9/bilibili_toolman/bilisession/common/submission.py`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.8/bilibili_toolman/bilisession/web.py` & `bilibili-toolman-1.0.7.9/bilibili_toolman/bilisession/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     MISC_MAX_DESCRIPTION_LENGTH = 2000
 
     FORCE_HTTP = False
 
     def request(self, method: str, url, *a, **k):
         if self.FORCE_HTTP and url[:5] == "https":
             url = "http" + url[5:]
-        return super().request(method, url, *a, **k)
+        return super().request(method, url, *a, **k,verify=not self.FORCE_HTTP)
 
     def __init__(self, cookies="") -> None:
         Session.__init__(self)
         self.LoginViaCookiesQueryString(cookies)
         self.headers["User-Agent"] = self.DEFAULT_UA
         self.logger = logger
 
@@ -431,22 +431,27 @@
             data={
                 "cover": "data:{%s};base64," % image_mime
                 + base64.b64encode(image_binary).decode(),
                 "csrf": self.cookies.get("bili_jct"),
             },
         )
 
-    @JSONResponse
     def UploadCover(self, path: str):
         """上传封面"""
         mime = mimetypes.guess_type(path)[0] or "image/png"  # fall back to png
         self.logger.debug("%s -> %s" % (path, mime))
         content = open(path, "rb").read()
         self.logger.debug("上传封面图 (%s B)" % len(content))
-        return self._upload_cover(content, mime)
+        resp = self._upload_cover(content, mime)
+        resp = resp.json()
+        try:
+            return resp["data"]["url"]
+        except KeyError:
+            self.logger.warning("上传失败：%s" % resp)
+            return None
 
     def _submit_submission(self, submission: Submission):
         return self.post(
             "https://member.bilibili.com/x/vu/web/add/v3",
             json={**submission.archive, "csrf": self.cookies.get("bili_jct")},
             params={"csrf": self.cookies.get("bili_jct")},
         )
```

### Comparing `bilibili-toolman-1.0.7.8/bilibili_toolman/cli/__init__.py` & `bilibili-toolman-1.0.7.9/bilibili_toolman/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.8/bilibili_toolman/cli/main.py` & `bilibili-toolman-1.0.7.9/bilibili_toolman/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,27 +96,27 @@
         logger.info("准备上传: %s" % title)
         """Summary trimming"""
         endpoint = None
         for _ in range(0, sess_upload.RETRIES_UPLOAD_ID):
             try:
                 endpoint, bid = sess_upload.UploadVideo(source.video_path)
                 cover_url = (
-                    sess_upload.UploadCover(source.cover_path)["data"]["url"]
+                    sess_upload.UploadCover(source.cover_path)
                     if source.cover_path
                     else ""
                 )
                 break
             except Exception as e:
                 logger.warning("%s 上传失败! - %s - 重试" % (source, e))
         if not endpoint:
             logger.error("URI 获取失败 - 跳过")
             continue
         logger.info("资源已上传")
         from bilibili_toolman.cli import precentage_progress
-
+        cover_url = ''
         precentage_progress.close()
         with Submission() as video:
             """Creatating a video per submission"""
             video.cover_url = cover_url
             video.video_endpoint = endpoint
             video.biz_id = bid
             """Sources identifiers"""
@@ -150,15 +150,15 @@
     """Use title & description from main sources (e.g. Uploading a YT Playlist)"""
     blocks, title, description = format(sources)
     submission.title = title
     submission.description = description  # This is the only description that gets shown
     submission.source = sources.soruce
     """Upload cover images for all our submissions as well"""
     cover_url = (
-        sess_upload.UploadCover(sources.cover_path)["data"]["url"]
+        sess_upload.UploadCover(sources.cover_path)
         if sources.cover_path
         else ""
     )
     submission.cover_url = cover_url
     """Finally submitting the video"""
     if not arg.no_submit:
         submit_result = sess_submit.SubmitSubmission(
```

### Comparing `bilibili-toolman-1.0.7.8/bilibili_toolman/cli/sanitizers.py` & `bilibili-toolman-1.0.7.9/bilibili_toolman/cli/sanitizers.py`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.8/bilibili_toolman/providers/__init__.py` & `bilibili-toolman-1.0.7.9/bilibili_toolman/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.8/bilibili_toolman/providers/localfile.py` & `bilibili-toolman-1.0.7.9/bilibili_toolman/providers/localfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def download_video(res) -> DownloadResult:
     results = DownloadResult()
     if (
         not os.path.isfile(res)
         and not os.path.isdir(res)
-        or (options["cover"] and os.path.isfile(options["cover"]))
+        or not (options["cover"] and os.path.isfile(options["cover"]))
     ):
         raise FileNotFoundError("%s - file not found" % res)
 
     def append(res):
         with DownloadResult() as result:
             result.video_path = res
             result.cover_path = options["cover"]
```

### Comparing `bilibili-toolman-1.0.7.8/bilibili_toolman/providers/youtube.py` & `bilibili-toolman-1.0.7.9/bilibili_toolman/providers/youtube.py`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/PKG-INFO` & `bilibili-toolman-1.0.7.9/bilibili_toolman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilibili-toolman
-Version: 1.0.7.8
+Version: 1.0.7.9
 Summary: bilibili-toolman 哔哩哔哩搬运工具
 Home-page: https://github.com/greats3an/bilibili-toolman
 Author: greats3an
 Author-email: greats3an@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bilibili-toolman-1.0.7.8/bilibili_toolman.egg-info/SOURCES.txt` & `bilibili-toolman-1.0.7.9/bilibili_toolman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bilibili-toolman-1.0.7.8/setup.py` & `bilibili-toolman-1.0.7.9/setup.py`

 * *Files identical despite different names*

