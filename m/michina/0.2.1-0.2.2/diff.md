# Comparing `tmp/michina-0.2.1.tar.gz` & `tmp/michina-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "michina-0.2.1.tar", max compression
+gzip compressed data, was "michina-0.2.2.tar", max compression
```

## Comparing `michina-0.2.1.tar` & `michina-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1451 2023-07-27 00:07:32.206966 michina-0.2.1/README.md
--rw-r--r--   0        0        0      114 2023-07-28 18:07:08.896265 michina-0.2.1/michina/checks/__init__.py
--rw-r--r--   0        0        0      749 2023-07-28 18:47:36.725936 michina-0.2.1/michina/checks/base/check.py
--rw-r--r--   0        0        0      183 2023-07-26 23:55:55.785232 michina-0.2.1/michina/checks/consistency/__init__.py
--rw-r--r--   0        0        0     1801 2023-07-28 18:06:45.360237 michina-0.2.1/michina/checks/consistency/check.py
--rw-r--r--   0        0        0     2611 2023-07-24 23:08:42.323294 michina-0.2.1/michina/checks/consistency/prompt.py
--rw-r--r--   0        0        0      140 2023-07-25 00:01:47.195530 michina-0.2.1/michina/checks/tone/__init__.py
--rw-r--r--   0        0        0     1446 2023-07-28 18:07:00.434977 michina-0.2.1/michina/checks/tone/check.py
--rw-r--r--   0        0        0     2397 2023-07-24 23:13:10.018714 michina-0.2.1/michina/checks/tone/prompt.py
--rw-r--r--   0        0        0      310 2023-07-24 18:35:05.155781 michina-0.2.1/michina/exceptions/exceptions.py
--rw-r--r--   0        0        0      469 2023-07-28 19:11:01.925070 michina-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2131 1970-01-01 00:00:00.000000 michina-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1486 2023-07-29 01:10:41.393337 michina-0.2.2/README.md
+-rw-r--r--   0        0        0      114 2023-07-28 18:07:08.896265 michina-0.2.2/michina/checks/__init__.py
+-rw-r--r--   0        0        0      749 2023-07-28 18:47:36.725936 michina-0.2.2/michina/checks/base/check.py
+-rw-r--r--   0        0        0      183 2023-07-26 23:55:55.785232 michina-0.2.2/michina/checks/consistency/__init__.py
+-rw-r--r--   0        0        0     1801 2023-07-28 18:06:45.360237 michina-0.2.2/michina/checks/consistency/check.py
+-rw-r--r--   0        0        0     2611 2023-07-24 23:08:42.323294 michina-0.2.2/michina/checks/consistency/prompt.py
+-rw-r--r--   0        0        0      141 2023-07-28 19:39:42.831416 michina-0.2.2/michina/checks/tone/__init__.py
+-rw-r--r--   0        0        0     1449 2023-07-28 19:39:43.230436 michina-0.2.2/michina/checks/tone/check.py
+-rw-r--r--   0        0        0     2397 2023-07-24 23:13:10.018714 michina-0.2.2/michina/checks/tone/prompt.py
+-rw-r--r--   0        0        0      310 2023-07-24 18:35:05.155781 michina-0.2.2/michina/exceptions/exceptions.py
+-rw-r--r--   0        0        0      469 2023-07-29 01:11:18.528032 michina-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2166 1970-01-01 00:00:00.000000 michina-0.2.2/PKG-INFO
```

### Comparing `michina-0.2.1/README.md` & `michina-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 - [openai] Can run in a Github Actions for workflow
 
 ## Todo
 - Add monitoring
 
 ## Versions
 
+### v0.2.1 -> v0.2.2
+Fixing typo.
+
 ### v0.1.1 -> v0.2.0
 This change allows you to configure the OpenAI model version to use.
 
 The API was like this
 ```python
 from src.prompts import check_for_political_content, respond_to_customer
 from michina.checks import ToneCheck, ConsistencyCheck
```

### Comparing `michina-0.2.1/michina/checks/base/check.py` & `michina-0.2.2/michina/checks/base/check.py`

 * *Files identical despite different names*

### Comparing `michina-0.2.1/michina/checks/consistency/check.py` & `michina-0.2.2/michina/checks/consistency/check.py`

 * *Files identical despite different names*

### Comparing `michina-0.2.1/michina/checks/consistency/prompt.py` & `michina-0.2.2/michina/checks/consistency/prompt.py`

 * *Files identical despite different names*

### Comparing `michina-0.2.1/michina/checks/tone/check.py` & `michina-0.2.2/michina/checks/tone/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,38 +17,38 @@
 
 
 class ToneCheckInput(BaseModel):
     message: str
     tone: str
 
 
-class ToneCheckReponse(BaseCheckResponse):
+class ToneCheckResponse(BaseCheckResponse):
     input: ToneCheckInput
     reasoning: str
     judgment: float
 
 
 class ToneCheck(BaseCheck):
     description: str = (
         "Checks whether the tone of a given message matches the tone provided."
     )
 
-    def check(self, message: str, tone: str) -> ToneCheckReponse:
+    def check(self, message: str, tone: str) -> ToneCheckResponse:
         prompt = PromptTemplate.from_template(TONE_CHECK_TEMPLATE)
         chain = LLMChain(llm=self.llm, prompt=prompt)
 
         try:
             string_response = chain.run(message=message, tone=tone)
         except Exception as e:
             raise LanguageModelException(e)
 
         try:
             response = xmltodict.parse(string_response)
         except Exception as e:
             raise InvalidXMLException(e)
 
         try:
-            response = ToneCheckReponse(**response["response"])
+            response = ToneCheckResponse(**response["response"])
         except Exception as e:
             raise InvalidTypeException(e)
 
         return response
```

### Comparing `michina-0.2.1/michina/checks/tone/prompt.py` & `michina-0.2.2/michina/checks/tone/prompt.py`

 * *Files identical despite different names*

### Comparing `michina-0.2.1/PKG-INFO` & `michina-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: michina
-Version: 0.2.1
+Version: 0.2.2
 Summary: Integ test framework for LLMs.
 Home-page: https://github.com/michina-ai/michina
 Author: bkitano
 Author-email: briankitano@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -26,14 +26,17 @@
 - [openai] Can run in a Github Actions for workflow
 
 ## Todo
 - Add monitoring
 
 ## Versions
 
+### v0.2.1 -> v0.2.2
+Fixing typo.
+
 ### v0.1.1 -> v0.2.0
 This change allows you to configure the OpenAI model version to use.
 
 The API was like this
 ```python
 from src.prompts import check_for_political_content, respond_to_customer
 from michina.checks import ToneCheck, ConsistencyCheck
```

