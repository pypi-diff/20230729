# Comparing `tmp/iamai_adapter_apscheduler-3.2.1.tar.gz` & `tmp/iamai_adapter_apscheduler-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai_adapter_apscheduler-3.2.1.tar", max compression
+gzip compressed data, was "iamai_adapter_apscheduler-3.2.3.tar", max compression
```

## Comparing `iamai_adapter_apscheduler-3.2.1.tar` & `iamai_adapter_apscheduler-3.2.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      253 2023-07-15 05:23:38.793804 iamai_adapter_apscheduler-3.2.1/README.md
--rw-r--r--   0        0        0     4675 2023-07-15 05:23:38.793804 iamai_adapter_apscheduler-3.2.1/iamai/adapter/apscheduler/__init__.py
--rw-r--r--   0        0        0      377 2023-07-15 05:23:38.793804 iamai_adapter_apscheduler-3.2.1/iamai/adapter/apscheduler/config.py
--rw-r--r--   0        0        0      932 2023-07-15 05:23:38.793804 iamai_adapter_apscheduler-3.2.1/iamai/adapter/apscheduler/event.py
--rw-r--r--   0        0        0     1338 2023-07-15 05:23:38.793804 iamai_adapter_apscheduler-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     1383 1970-01-01 00:00:00.000000 iamai_adapter_apscheduler-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-07-29 04:29:08.910201 iamai_adapter_apscheduler-3.2.3/LICENSE
+-rw-r--r--   0        0        0      253 2023-07-29 04:29:08.910201 iamai_adapter_apscheduler-3.2.3/README.md
+-rw-r--r--   0        0        0     4673 2023-07-29 04:29:08.910201 iamai_adapter_apscheduler-3.2.3/iamai/adapter/apscheduler/__init__.py
+-rw-r--r--   0        0        0      377 2023-07-29 04:29:08.910201 iamai_adapter_apscheduler-3.2.3/iamai/adapter/apscheduler/config.py
+-rw-r--r--   0        0        0      932 2023-07-29 04:29:08.910201 iamai_adapter_apscheduler-3.2.3/iamai/adapter/apscheduler/event.py
+-rw-r--r--   0        0        0     1339 2023-07-29 04:29:08.910201 iamai_adapter_apscheduler-3.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 iamai_adapter_apscheduler-3.2.3/PKG-INFO
```

### Comparing `iamai_adapter_apscheduler-3.2.1/iamai/adapter/apscheduler/__init__.py` & `iamai_adapter_apscheduler-3.2.3/iamai/adapter/apscheduler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,17 +104,17 @@
         trigger: APScheduler 触发器。
         trigger_args: APScheduler 触发器参数。
         override_rule: 是否重写 rule() 方法，若为 True，则会在 rule() 方法中添加处理本插件定义的计划任务事件的逻辑。
     """
 
     def _decorator(cls: Type):
         if not inspect.isclass(cls):
-            raise TypeError(f"can only decorate class")
+            raise TypeError("can only decorate class")
         if not issubclass(cls, Plugin):
-            raise TypeError(f"can only decorate Plugin class")
+            raise TypeError("can only decorate Plugin class")
         setattr(cls, "__schedule__", True)
         setattr(cls, "trigger", trigger)
         setattr(cls, "trigger_args", trigger_args)
         if override_rule:
 
             def _rule_decorator(func):
                 @wraps(func)
```

### Comparing `iamai_adapter_apscheduler-3.2.1/iamai/adapter/apscheduler/event.py` & `iamai_adapter_apscheduler-3.2.3/iamai/adapter/apscheduler/event.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_apscheduler-3.2.1/pyproject.toml` & `iamai_adapter_apscheduler-3.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamai-adapter-apscheduler"
-version = "3.2.1"
+version = "3.2.3"
 description = "APScheduler adapter for iamai."
 authors = ["简律纯 <i@jyunko.cn>"]
 license = "GPL-3.0 License"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
@@ -20,15 +20,15 @@
     "Topic :: Communications :: Chat",
 ]
 packages = [{ include = "iamai" }]
 exclude = ["iamai/__init__.py", "iamai/adapter/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-iamai = "^3.2"
+iamai = ">=3.2"
 apscheduler = "^3.7"
 
 [tool.poetry.dev-dependencies]
 iamai = { path = "../../", develop = true }
 
 [tool.pydantic-pycharm-plugin]
 ignore-init-method-arguments = true
```

### Comparing `iamai_adapter_apscheduler-3.2.1/PKG-INFO` & `iamai_adapter_apscheduler-3.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamai-adapter-apscheduler
-Version: 3.2.1
+Version: 3.2.3
 Summary: APScheduler adapter for iamai.
 Home-page: https://retrofor.space/
 License: GPL-3.0 License
 Keywords: bot,chatbot,scheduling,apscheduler
 Author: 简律纯
 Author-email: i@jyunko.cn
 Requires-Python: >=3.8,<4.0
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Chat
 Requires-Dist: apscheduler (>=3.7,<4.0)
-Requires-Dist: iamai (>=3.2,<4.0)
+Requires-Dist: iamai (>=3.2)
 Project-URL: Documentation, https://iamai.retrofor.space/
 Project-URL: Repository, https://github.com/retrofor/iamai
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://docs.iamai.dev/"><img src="https://raw.githubusercontent.com/retrofor/iamai/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: iamai-adapter-apscheduler Version: 3.2.1 Summary:
+Metadata-Version: 2.1 Name: iamai-adapter-apscheduler Version: 3.2.3 Summary:
 APScheduler adapter for iamai. Home-page: https://retrofor.space/ License: GPL-
 3.0 License Keywords: bot,chatbot,scheduling,apscheduler Author: ç®å¾çº¯
 Author-email: i@jyunko.cn Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Framework :: AsyncIO Classifier: Framework ::
 Robot Framework Classifier: Framework :: Robot Framework :: Library Classifier:
 License :: OSI Approved :: MIT License Classifier: License :: Other/Proprietary
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Chat Requires-Dist: apscheduler
-(>=3.7,<4.0) Requires-Dist: iamai (>=3.2,<4.0) Project-URL: Documentation,
-https://iamai.retrofor.space/ Project-URL: Repository, https://github.com/
-retrofor/iamai Description-Content-Type: text/markdown
+(>=3.7,<4.0) Requires-Dist: iamai (>=3.2) Project-URL: Documentation, https://
+iamai.retrofor.space/ Project-URL: Repository, https://github.com/retrofor/
+iamai Description-Content-Type: text/markdown
         [logo] # iamai-Adapter-Apscheduler **Apscheduler åè®®éé**
```

