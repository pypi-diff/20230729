# Comparing `tmp/openplugincore-0.4.1.tar.gz` & `tmp/openplugincore-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugincore-0.4.1.tar", last modified: Fri Jul  7 03:25:52 2023, max compression
+gzip compressed data, was "openplugincore-0.5.0.tar", last modified: Sat Jul 29 21:03:27 2023, max compression
```

## Comparing `openplugincore-0.4.1.tar` & `openplugincore-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:25:52.299028 openplugincore-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-07 03:25:52.299028 openplugincore-0.4.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:25:52.299028 openplugincore-0.4.1/openplugincore/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-07 03:25:42.000000 openplugincore-0.4.1/openplugincore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-07 03:25:42.000000 openplugincore-0.4.1/openplugincore/openplugincore.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-07 03:25:42.000000 openplugincore-0.4.1/openplugincore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:25:52.299028 openplugincore-0.4.1/openplugincore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-07 03:25:52.000000 openplugincore-0.4.1/openplugincore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-07 03:25:52.000000 openplugincore-0.4.1/openplugincore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 03:25:52.000000 openplugincore-0.4.1/openplugincore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 03:25:52.000000 openplugincore-0.4.1/openplugincore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 03:25:52.000000 openplugincore-0.4.1/openplugincore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 03:25:52.299028 openplugincore-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-07 03:25:42.000000 openplugincore-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:25:52.299028 openplugincore-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 03:25:42.000000 openplugincore-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-07 03:25:42.000000 openplugincore-0.4.1/tests/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-07 03:25:42.000000 openplugincore-0.4.1/tests/test_basicTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-07 03:25:42.000000 openplugincore-0.4.1/tests/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:03:27.782038 openplugincore-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-29 21:03:27.782038 openplugincore-0.5.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:03:27.782038 openplugincore-0.5.0/openplugincore/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-29 21:03:17.000000 openplugincore-0.5.0/openplugincore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-07-29 21:03:17.000000 openplugincore-0.5.0/openplugincore/openplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-29 21:03:17.000000 openplugincore-0.5.0/openplugincore/openplugin_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-29 21:03:17.000000 openplugincore-0.5.0/openplugincore/openplugin_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-29 21:03:17.000000 openplugincore-0.5.0/openplugincore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:03:27.782038 openplugincore-0.5.0/openplugincore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-29 21:03:27.000000 openplugincore-0.5.0/openplugincore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-29 21:03:27.000000 openplugincore-0.5.0/openplugincore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 21:03:27.000000 openplugincore-0.5.0/openplugincore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-29 21:03:27.000000 openplugincore-0.5.0/openplugincore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 21:03:27.000000 openplugincore-0.5.0/openplugincore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 21:03:27.782038 openplugincore-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-29 21:03:17.000000 openplugincore-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 21:03:27.782038 openplugincore-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 21:03:17.000000 openplugincore-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-29 21:03:17.000000 openplugincore-0.5.0/tests/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-07-29 21:03:17.000000 openplugincore-0.5.0/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-29 21:03:17.000000 openplugincore-0.5.0/tests/test_openplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-29 21:03:17.000000 openplugincore-0.5.0/tests/test_openplugin_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-29 21:03:17.000000 openplugincore-0.5.0/tests/test_openplugin_memo.py
```

### Comparing `openplugincore-0.4.1/PKG-INFO` & `openplugincore-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openplugincore
-Version: 0.4.1
+Version: 0.5.0
 Summary: Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openplugincore-0.4.1/openplugincore/openplugincore.py` & `openplugincore-0.5.0/openplugincore/openplugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 from urllib.error import HTTPError
 import requests
 from typing import Any, List, Dict, Union, Tuple, Callable
 import os
 from .types import ChatgptAssistantMessage, ChatgptFunctionMessage, PluginConfigs
+from .utils.constants import openai_models_info
+from .utils.prompting import estimate_tokens, truncate_json_root
 from langchain.chains.openai_functions.openapi import openapi_spec_to_openai_fn
 from langchain.utilities.openapi import OpenAPISpec
 from langchain.output_parsers.openai_functions import JsonOutputFunctionsParser
 from langchain.prompts import ChatPromptTemplate
 from langchain.chat_models import ChatOpenAI
 from langchain.schema import HumanMessage, AIMessage, SystemMessage, FunctionMessage
 from langchain import LLMChain
@@ -156,15 +158,15 @@
             elif openai_message["role"] == "assistant":
                 # set veriable content to "" if it is None
                 content = openai_message["content"] if openai_message["content"] is not None else ""
                 langchain_messages.append(AIMessage(content=content, additional_kwargs={"function_call": openai_message["function_call"]}))
         
         return langchain_messages
 
-    def fetch_plugin(self, prompt: str, **chatgpt_args) -> ChatgptFunctionMessage:
+    def fetch_plugin(self, prompt: str, truncate: Union[bool, int] = False, truncate_offset: int = 0, **chatgpt_args) -> ChatgptFunctionMessage:
         if chatgpt_args.get("model", None) not in ["gpt-3.5-turbo-0613", "gpt-4-0613"]:
             raise ValueError("Model must be either gpt-3.5-turbo-0613 or gpt-4-0613")
         
         llm =  ChatOpenAI(
             **chatgpt_args,
         )
         llm_chain = LLMChain(
@@ -207,17 +209,29 @@
         def request_chain(name,arguments):
             res = self.call_api_fn(
                 name, arguments, headers=None, params=None
             )
             return res
         request_out = request_chain(**llm_chain_out)
         json_response = request_out.json()
+
+        if truncate:
+            truncate_to = truncate if not isinstance(truncate, bool) else None
+            if truncate_to is None:
+                token_slack = 56 + 300
+                dummy_chatgpt_message = {
+                    "role": "user",
+                    "content": prompt,
+                }
+                truncate_to = openai_models_info[chatgpt_args['model']]['max_tokens'] - estimate_tokens(json.dumps(dummy_chatgpt_message)) - token_slack - truncate_offset
+            json_response = truncate_json_root(json_response, truncate_to)
+
         if self.verbose:
             print(f"\"{self.name}\" json_response: ", json.dumps(json_response, indent=2))
         try:
             return ChatgptFunctionMessage(
                 role="function",
                 name=llm_chain_out["name"],
                 content=json.dumps(json_response)
             )
         except json.decoder.JSONDecodeError:
-            raise json.decoder.JSONDecodeError(f"API call failed, API returned the following non-JSON response:\n{response.content}")
+            raise json.decoder.JSONDecodeError(f"API call failed, API returned the following non-JSON response:\n{response.content}")
```

### Comparing `openplugincore-0.4.1/openplugincore/types.py` & `openplugincore-0.5.0/openplugincore/types.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.4.1/openplugincore.egg-info/PKG-INFO` & `openplugincore-0.5.0/openplugincore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openplugincore
-Version: 0.4.1
+Version: 0.5.0
 Summary: Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openplugincore-0.4.1/setup.py` & `openplugincore-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name='openplugincore', 
-        version="0.4.1",
+        version="0.5.0",
         author="Sebastian Sosa",
         author_email="1sebastian1sosa1@gmail.com",
         description='Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
         long_description='Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
         packages=find_packages(),
         package_data={
             "openplugincore": ["*.json"],  # include all .json files in the openplugin package
```

### Comparing `openplugincore-0.4.1/tests/mock_data.py` & `openplugincore-0.5.0/tests/mock_data.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.4.1/tests/test_e2e.py` & `openplugincore-0.5.0/tests/test_e2e.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,33 +89,15 @@
 
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
 
     # Replace the line below with a test for the final output in json_content
     assert json_content["stats"]["account_found"] == True
-
-def test_initiate_and_fetch_tailor_erp():
-    plugin = OpenPlugin("tailor_erp")
-    assert plugin.manifest is not None
-
-    # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'create a CRM template with ERP generator'
-    response = plugin.fetch_plugin(
-        prompt=chatgpt_prompt,
-        model="gpt-3.5-turbo-0613",
-        temperature=0,
-    )
-
-    assert response is not None
-    assert response["role"] == "function"
-    json_content = json.loads(response["content"])
-
-    # assert that json_content.applyTemplate.path is not None
-    assert json_content["APP_ID"] is not None
+    
 
 def test_initiate_and_fetch_surge_ai_trends():
     plugin = OpenPlugin("surge_ai_trends")
     assert plugin.manifest is not None
 
     # create chatgpt request that will call the addTodo function
     chatgpt_prompt = 'What are the trnding searches for "gpu" in amazon'
@@ -147,31 +129,30 @@
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
 
     # Replace the line below with a test for the final output in json_content
     assert isinstance(json_content["blog"], str)
 
+@pytest.mark.skip(reason="Not whitelisted")
 def test_initiate_and_fetch_scholarai():
     plugin = OpenPlugin("scholarai")
     assert plugin.manifest is not None
 
-
     # create chatgpt request that will call the addTodo function
-    chatgpt_prompt = 'What scientific research exists for semantic representation of language through brain waves. dont sort.'
+    chatgpt_prompt = 'What scientific research exists for semantic representation of language through brain waves. show me one.'
     response = plugin.fetch_plugin(
         prompt=chatgpt_prompt,
         model="gpt-3.5-turbo-0613",
         temperature=0,
     )
 
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
-
     # Replace the line below with a test for the final output in json_content
     assert isinstance(json_content["total_num_results"], int)
 
 def test_initiate_and_fetch_rephrase():
     plugin = OpenPlugin("rephrase")
     assert plugin.manifest is not None
 
@@ -243,14 +224,15 @@
     assert response is not None
     assert response["role"] == "function"
     json_content = json.loads(response["content"])
 
     # Replace the line below with a test for the final output in json_content
     assert isinstance(json_content["tafs"], list)
 
+@pytest.mark.skip(reason="Could not parse: requests.exceptions.JSONDecodeError: Expecting value: line 1 column 1")
 def test_initiate_and_fetch_Ai_PDF():
     plugin = OpenPlugin("Ai_PDF", verbose=True)
     assert plugin.manifest is not None
     
     # create chatgpt request that will call the addTodo function
     chatgpt_prompt = 'Can I have my data be private according to this pdf https://www.unodc.org/pdf/criminal_justice/UN_Basic_Principles_on_the_Role_of_Lawyers.pdf'
     response = plugin.fetch_plugin(
```

