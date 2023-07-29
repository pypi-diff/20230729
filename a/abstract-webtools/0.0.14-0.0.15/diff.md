# Comparing `tmp/abstract_webtools-0.0.14.tar.gz` & `tmp/abstract_webtools-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_webtools-0.0.14.tar", last modified: Sat Jul 29 19:50:03 2023, max compression
+gzip compressed data, was "abstract_webtools-0.0.15.tar", last modified: Sat Jul 29 19:58:40 2023, max compression
```

## Comparing `abstract_webtools-0.0.14.tar` & `abstract_webtools-0.0.15.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:50:03.590374 abstract_webtools-0.0.14/
--rw-r--r--   0 root         (0) root         (0)     3788 2023-07-29 19:50:03.590374 abstract_webtools-0.0.14/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3111 2023-07-29 19:45:03.000000 abstract_webtools-0.0.14/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_webtools-0.0.14/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-29 19:50:03.590374 abstract_webtools-0.0.14/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1217 2023-07-29 19:49:31.000000 abstract_webtools-0.0.14/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:50:03.590374 abstract_webtools-0.0.14/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:50:03.590374 abstract_webtools-0.0.14/src/abstract_webtools/
--rw-rw-r--   0 root         (0) root         (0)       28 2023-07-29 19:28:16.000000 abstract_webtools-0.0.14/src/abstract_webtools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1329 2023-07-29 19:09:21.000000 abstract_webtools-0.0.14/src/abstract_webtools/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:50:03.590374 abstract_webtools-0.0.14/src/abstract_webtools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3788 2023-07-29 19:50:03.000000 abstract_webtools-0.0.14/src/abstract_webtools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-07-29 19:50:03.000000 abstract_webtools-0.0.14/src/abstract_webtools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 19:50:03.000000 abstract_webtools-0.0.14/src/abstract_webtools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-29 19:50:03.000000 abstract_webtools-0.0.14/src/abstract_webtools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-29 19:50:03.000000 abstract_webtools-0.0.14/src/abstract_webtools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:58:40.894975 abstract_webtools-0.0.15/
+-rw-r--r--   0 root         (0) root         (0)     3818 2023-07-29 19:58:40.894975 abstract_webtools-0.0.15/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3141 2023-07-29 19:58:01.000000 abstract_webtools-0.0.15/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_webtools-0.0.15/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-29 19:58:40.894975 abstract_webtools-0.0.15/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1217 2023-07-29 19:58:06.000000 abstract_webtools-0.0.15/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:58:40.890974 abstract_webtools-0.0.15/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:58:40.894975 abstract_webtools-0.0.15/src/abstract_webtools/
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-07-29 19:28:16.000000 abstract_webtools-0.0.15/src/abstract_webtools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1329 2023-07-29 19:09:21.000000 abstract_webtools-0.0.15/src/abstract_webtools/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 19:58:40.894975 abstract_webtools-0.0.15/src/abstract_webtools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3818 2023-07-29 19:58:40.000000 abstract_webtools-0.0.15/src/abstract_webtools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-07-29 19:58:40.000000 abstract_webtools-0.0.15/src/abstract_webtools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 19:58:40.000000 abstract_webtools-0.0.15/src/abstract_webtools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-29 19:58:40.000000 abstract_webtools-0.0.15/src/abstract_webtools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-29 19:58:40.000000 abstract_webtools-0.0.15/src/abstract_webtools.egg-info/top_level.txt
```

### Comparing `abstract_webtools-0.0.14/PKG-INFO` & `abstract_webtools-0.0.15/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_webtools
-Version: 0.0.14
+Version: 0.0.15
 Summary: Abstract Web Tools is a Python package that provides various utility functions for web scraping tasks. It is built on top of popular libraries such as `requests`, `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing web content.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_webtools
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -96,19 +96,19 @@
 ### Parse All
 
 The `parse_all` function fetches the source code of a URL and extracts information about HTML elements, attribute values, attribute names, and class names.
 
 ```python
 from abstract_webtools import parse_all
 
-element_types, attribute_values, attribute_names, class_names = parse_all('https://www.example.com')
-print(element_types)       # Output: List of HTML element types
-print(attribute_values)    # Output: List of attribute values
-print(attribute_names)     # Output: List of attribute names
-print(class_names)         # Output: List of class names
+HTML_components = parse_all('https://www.example.com')
+print(HTML_components["element_types"])       # Output: List of HTML element types
+print(HTML_components["attribute_values"])    # Output: List of attribute values
+print(HTML_components["attribute_names"])     # Output: List of attribute names
+print(HTML_components["class_names"])         # Output: List of class names
 ```
 
 ### Extract Elements
 
 The `extract_elements` function fetches the source code of a URL and extracts portions of the source code based on provided filters.
 
 ```python
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_uvonm49d_/tmp7fude_v0_TarContainer/0/1", line 125, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_uvonm49d_/tmp7fude_v0_TarContainer/0/1", line 125, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: abstract_webtools Version: 0.0.14 Summary: Abstract
+Metadata-Version: 2.1 Name: abstract_webtools Version: 0.0.15 Summary: Abstract
 Web Tools is a Python package that provides various utility functions for web
 scraping tasks. It is built on top of popular libraries such as `requests`,
 `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing
 web content. Home-page: https://github.com/AbstractEndeavors/
 abstract_essentials/tree/main/abstract_webtools Author: putkoff Author-email:
 partners@abstractendeavors.com Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
```

### Comparing `abstract_webtools-0.0.14/README.md` & `abstract_webtools-0.0.15/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -131,65 +131,67 @@
 00000820: 7420 4854 4d4c 2065 6c65 6d65 6e74 732c  t HTML elements,
 00000830: 2061 7474 7269 6275 7465 2076 616c 7565   attribute value
 00000840: 732c 2061 7474 7269 6275 7465 206e 616d  s, attribute nam
 00000850: 6573 2c20 616e 6420 636c 6173 7320 6e61  es, and class na
 00000860: 6d65 732e 0d0a 0d0a 6060 6070 7974 686f  mes.....```pytho
 00000870: 6e0d 0a66 726f 6d20 6162 7374 7261 6374  n..from abstract
 00000880: 5f77 6562 746f 6f6c 7320 696d 706f 7274  _webtools import
-00000890: 2070 6172 7365 5f61 6c6c 0d0a 0d0a 656c   parse_all....el
-000008a0: 656d 656e 745f 7479 7065 732c 2061 7474  ement_types, att
-000008b0: 7269 6275 7465 5f76 616c 7565 732c 2061  ribute_values, a
-000008c0: 7474 7269 6275 7465 5f6e 616d 6573 2c20  ttribute_names, 
-000008d0: 636c 6173 735f 6e61 6d65 7320 3d20 7061  class_names = pa
-000008e0: 7273 655f 616c 6c28 2768 7474 7073 3a2f  rse_all('https:/
-000008f0: 2f77 7777 2e65 7861 6d70 6c65 2e63 6f6d  /www.example.com
-00000900: 2729 0d0a 7072 696e 7428 656c 656d 656e  ')..print(elemen
-00000910: 745f 7479 7065 7329 2020 2020 2020 2023  t_types)       #
-00000920: 204f 7574 7075 743a 204c 6973 7420 6f66   Output: List of
-00000930: 2048 544d 4c20 656c 656d 656e 7420 7479   HTML element ty
-00000940: 7065 730d 0a70 7269 6e74 2861 7474 7269  pes..print(attri
-00000950: 6275 7465 5f76 616c 7565 7329 2020 2020  bute_values)    
-00000960: 2320 4f75 7470 7574 3a20 4c69 7374 206f  # Output: List o
-00000970: 6620 6174 7472 6962 7574 6520 7661 6c75  f attribute valu
-00000980: 6573 0d0a 7072 696e 7428 6174 7472 6962  es..print(attrib
-00000990: 7574 655f 6e61 6d65 7329 2020 2020 2023  ute_names)     #
-000009a0: 204f 7574 7075 743a 204c 6973 7420 6f66   Output: List of
-000009b0: 2061 7474 7269 6275 7465 206e 616d 6573   attribute names
-000009c0: 0d0a 7072 696e 7428 636c 6173 735f 6e61  ..print(class_na
-000009d0: 6d65 7329 2020 2020 2020 2020 2023 204f  mes)         # O
-000009e0: 7574 7075 743a 204c 6973 7420 6f66 2063  utput: List of c
-000009f0: 6c61 7373 206e 616d 6573 0d0a 6060 600d  lass names..```.
-00000a00: 0a0d 0a23 2323 2045 7874 7261 6374 2045  ...### Extract E
-00000a10: 6c65 6d65 6e74 730d 0a0d 0a54 6865 2060  lements....The `
-00000a20: 6578 7472 6163 745f 656c 656d 656e 7473  extract_elements
-00000a30: 6020 6675 6e63 7469 6f6e 2066 6574 6368  ` function fetch
-00000a40: 6573 2074 6865 2073 6f75 7263 6520 636f  es the source co
-00000a50: 6465 206f 6620 6120 5552 4c20 616e 6420  de of a URL and 
-00000a60: 6578 7472 6163 7473 2070 6f72 7469 6f6e  extracts portion
-00000a70: 7320 6f66 2074 6865 2073 6f75 7263 6520  s of the source 
-00000a80: 636f 6465 2062 6173 6564 206f 6e20 7072  code based on pr
-00000a90: 6f76 6964 6564 2066 696c 7465 7273 2e0d  ovided filters..
-00000aa0: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
-00000ab0: 6f6d 2061 6273 7472 6163 745f 7765 6274  om abstract_webt
-00000ac0: 6f6f 6c73 2069 6d70 6f72 7420 6578 7472  ools import extr
-00000ad0: 6163 745f 656c 656d 656e 7473 0d0a 0d0a  act_elements....
-00000ae0: 656c 656d 656e 7473 203d 2065 7874 7261  elements = extra
-00000af0: 6374 5f65 6c65 6d65 6e74 7328 2768 7474  ct_elements('htt
-00000b00: 7073 3a2f 2f77 7777 2e65 7861 6d70 6c65  ps://www.example
-00000b10: 2e63 6f6d 272c 2065 6c65 6d65 6e74 5f74  .com', element_t
-00000b20: 7970 653d 2764 6976 272c 2061 7474 7269  ype='div', attri
-00000b30: 6275 7465 5f6e 616d 653d 2763 6c61 7373  bute_name='class
-00000b40: 272c 2063 6c61 7373 5f6e 616d 653d 2763  ', class_name='c
-00000b50: 6f6e 7461 696e 6572 2729 0d0a 7072 696e  ontainer')..prin
-00000b60: 7428 656c 656d 656e 7473 2920 2023 204f  t(elements)  # O
-00000b70: 7574 7075 743a 204c 6973 7420 6f66 2048  utput: List of H
-00000b80: 544d 4c20 656c 656d 656e 7473 2074 6861  TML elements tha
-00000b90: 7420 6d61 7463 6820 7468 6520 7072 6f76  t match the prov
-00000ba0: 6964 6564 2066 696c 7465 7273 0d0a 6060  ided filters..``
-00000bb0: 600d 0a0d 0a23 2320 4c69 6365 6e73 650d  `....## License.
-00000bc0: 0a0d 0a54 6869 7320 7072 6f6a 6563 7420  ...This project 
-00000bd0: 6973 206c 6963 656e 7365 6420 756e 6465  is licensed unde
-00000be0: 7220 7468 6520 4d49 5420 4c69 6365 6e73  r the MIT Licens
-00000bf0: 6520 2d20 7365 6520 7468 6520 5b4c 4943  e - see the [LIC
-00000c00: 454e 5345 5d28 4c49 4345 4e53 4529 2066  ENSE](LICENSE) f
-00000c10: 696c 6520 666f 7220 6465 7461 696c 732e  ile for details.
-00000c20: 0d0a 6060 600d 0a                        ..```..
+00000890: 2070 6172 7365 5f61 6c6c 0d0a 0d0a 4854   parse_all....HT
+000008a0: 4d4c 5f63 6f6d 706f 6e65 6e74 7320 3d20  ML_components = 
+000008b0: 7061 7273 655f 616c 6c28 2768 7474 7073  parse_all('https
+000008c0: 3a2f 2f77 7777 2e65 7861 6d70 6c65 2e63  ://www.example.c
+000008d0: 6f6d 2729 0d0a 7072 696e 7428 4854 4d4c  om')..print(HTML
+000008e0: 5f63 6f6d 706f 6e65 6e74 735b 2265 6c65  _components["ele
+000008f0: 6d65 6e74 5f74 7970 6573 225d 2920 2020  ment_types"])   
+00000900: 2020 2020 2320 4f75 7470 7574 3a20 4c69      # Output: Li
+00000910: 7374 206f 6620 4854 4d4c 2065 6c65 6d65  st of HTML eleme
+00000920: 6e74 2074 7970 6573 0d0a 7072 696e 7428  nt types..print(
+00000930: 4854 4d4c 5f63 6f6d 706f 6e65 6e74 735b  HTML_components[
+00000940: 2261 7474 7269 6275 7465 5f76 616c 7565  "attribute_value
+00000950: 7322 5d29 2020 2020 2320 4f75 7470 7574  s"])    # Output
+00000960: 3a20 4c69 7374 206f 6620 6174 7472 6962  : List of attrib
+00000970: 7574 6520 7661 6c75 6573 0d0a 7072 696e  ute values..prin
+00000980: 7428 4854 4d4c 5f63 6f6d 706f 6e65 6e74  t(HTML_component
+00000990: 735b 2261 7474 7269 6275 7465 5f6e 616d  s["attribute_nam
+000009a0: 6573 225d 2920 2020 2020 2320 4f75 7470  es"])     # Outp
+000009b0: 7574 3a20 4c69 7374 206f 6620 6174 7472  ut: List of attr
+000009c0: 6962 7574 6520 6e61 6d65 730d 0a70 7269  ibute names..pri
+000009d0: 6e74 2848 544d 4c5f 636f 6d70 6f6e 656e  nt(HTML_componen
+000009e0: 7473 5b22 636c 6173 735f 6e61 6d65 7322  ts["class_names"
+000009f0: 5d29 2020 2020 2020 2020 2023 204f 7574  ])         # Out
+00000a00: 7075 743a 204c 6973 7420 6f66 2063 6c61  put: List of cla
+00000a10: 7373 206e 616d 6573 0d0a 6060 600d 0a0d  ss names..```...
+00000a20: 0a23 2323 2045 7874 7261 6374 2045 6c65  .### Extract Ele
+00000a30: 6d65 6e74 730d 0a0d 0a54 6865 2060 6578  ments....The `ex
+00000a40: 7472 6163 745f 656c 656d 656e 7473 6020  tract_elements` 
+00000a50: 6675 6e63 7469 6f6e 2066 6574 6368 6573  function fetches
+00000a60: 2074 6865 2073 6f75 7263 6520 636f 6465   the source code
+00000a70: 206f 6620 6120 5552 4c20 616e 6420 6578   of a URL and ex
+00000a80: 7472 6163 7473 2070 6f72 7469 6f6e 7320  tracts portions 
+00000a90: 6f66 2074 6865 2073 6f75 7263 6520 636f  of the source co
+00000aa0: 6465 2062 6173 6564 206f 6e20 7072 6f76  de based on prov
+00000ab0: 6964 6564 2066 696c 7465 7273 2e0d 0a0d  ided filters....
+00000ac0: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
+00000ad0: 2061 6273 7472 6163 745f 7765 6274 6f6f   abstract_webtoo
+00000ae0: 6c73 2069 6d70 6f72 7420 6578 7472 6163  ls import extrac
+00000af0: 745f 656c 656d 656e 7473 0d0a 0d0a 656c  t_elements....el
+00000b00: 656d 656e 7473 203d 2065 7874 7261 6374  ements = extract
+00000b10: 5f65 6c65 6d65 6e74 7328 2768 7474 7073  _elements('https
+00000b20: 3a2f 2f77 7777 2e65 7861 6d70 6c65 2e63  ://www.example.c
+00000b30: 6f6d 272c 2065 6c65 6d65 6e74 5f74 7970  om', element_typ
+00000b40: 653d 2764 6976 272c 2061 7474 7269 6275  e='div', attribu
+00000b50: 7465 5f6e 616d 653d 2763 6c61 7373 272c  te_name='class',
+00000b60: 2063 6c61 7373 5f6e 616d 653d 2763 6f6e   class_name='con
+00000b70: 7461 696e 6572 2729 0d0a 7072 696e 7428  tainer')..print(
+00000b80: 656c 656d 656e 7473 2920 2023 204f 7574  elements)  # Out
+00000b90: 7075 743a 204c 6973 7420 6f66 2048 544d  put: List of HTM
+00000ba0: 4c20 656c 656d 656e 7473 2074 6861 7420  L elements that 
+00000bb0: 6d61 7463 6820 7468 6520 7072 6f76 6964  match the provid
+00000bc0: 6564 2066 696c 7465 7273 0d0a 6060 600d  ed filters..```.
+00000bd0: 0a0d 0a23 2320 4c69 6365 6e73 650d 0a0d  ...## License...
+00000be0: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
+00000bf0: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
+00000c00: 7468 6520 4d49 5420 4c69 6365 6e73 6520  the MIT License 
+00000c10: 2d20 7365 6520 7468 6520 5b4c 4943 454e  - see the [LICEN
+00000c20: 5345 5d28 4c49 4345 4e53 4529 2066 696c  SE](LICENSE) fil
+00000c30: 6520 666f 7220 6465 7461 696c 732e 0d0a  e for details...
+00000c40: 6060 600d 0a                             ```..
```

### Comparing `abstract_webtools-0.0.14/setup.py` & `abstract_webtools-0.0.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_webtools',
-    version='0.0.14',
+    version='0.0.15',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='Abstract Web Tools is a Python package that provides various utility functions for web scraping tasks. It is built on top of popular libraries such as `requests`, `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing web content.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_webtools',
     classifiers=[
```

### Comparing `abstract_webtools-0.0.14/src/abstract_webtools/main.py` & `abstract_webtools-0.0.15/src/abstract_webtools/main.py`

 * *Files identical despite different names*

### Comparing `abstract_webtools-0.0.14/src/abstract_webtools.egg-info/PKG-INFO` & `abstract_webtools-0.0.15/src/abstract_webtools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-webtools
-Version: 0.0.14
+Version: 0.0.15
 Summary: Abstract Web Tools is a Python package that provides various utility functions for web scraping tasks. It is built on top of popular libraries such as `requests`, `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing web content.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_webtools
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -96,19 +96,19 @@
 ### Parse All
 
 The `parse_all` function fetches the source code of a URL and extracts information about HTML elements, attribute values, attribute names, and class names.
 
 ```python
 from abstract_webtools import parse_all
 
-element_types, attribute_values, attribute_names, class_names = parse_all('https://www.example.com')
-print(element_types)       # Output: List of HTML element types
-print(attribute_values)    # Output: List of attribute values
-print(attribute_names)     # Output: List of attribute names
-print(class_names)         # Output: List of class names
+HTML_components = parse_all('https://www.example.com')
+print(HTML_components["element_types"])       # Output: List of HTML element types
+print(HTML_components["attribute_values"])    # Output: List of attribute values
+print(HTML_components["attribute_names"])     # Output: List of attribute names
+print(HTML_components["class_names"])         # Output: List of class names
 ```
 
 ### Extract Elements
 
 The `extract_elements` function fetches the source code of a URL and extracts portions of the source code based on provided filters.
 
 ```python
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_uvonm49d_/tmp7fude_v0_TarContainer/0/11", line 125, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_uvonm49d_/tmp7fude_v0_TarContainer/0/11", line 125, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: abstract-webtools Version: 0.0.14 Summary: Abstract
+Metadata-Version: 2.1 Name: abstract-webtools Version: 0.0.15 Summary: Abstract
 Web Tools is a Python package that provides various utility functions for web
 scraping tasks. It is built on top of popular libraries such as `requests`,
 `BeautifulSoup`, and `urllib3` to simplify the process of fetching and parsing
 web content. Home-page: https://github.com/AbstractEndeavors/
 abstract_essentials/tree/main/abstract_webtools Author: putkoff Author-email:
 partners@abstractendeavors.com Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
```

