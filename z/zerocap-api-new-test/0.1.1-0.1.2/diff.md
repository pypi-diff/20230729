# Comparing `tmp/zerocap_api_new_test-0.1.1.tar.gz` & `tmp/zerocap_api_new_test-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zerocap_api_new_test-0.1.1.tar", last modified: Sat Jul 29 08:25:59 2023, max compression
+gzip compressed data, was "dist/zerocap_api_new_test-0.1.2.tar", last modified: Sat Jul 29 08:51:19 2023, max compression
```

## Comparing `zerocap_api_new_test-0.1.1.tar` & `zerocap_api_new_test-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 08:25:59.000000 zerocap_api_new_test-0.1.1/
--rw-r--r--   0 mac        (501) staff       (20)    11323 2023-07-24 01:35:05.000000 zerocap_api_new_test-0.1.1/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)    13885 2023-07-29 08:25:59.000000 zerocap_api_new_test-0.1.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)    13452 2023-07-29 08:06:55.000000 zerocap_api_new_test-0.1.1/README.rst
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-29 08:25:59.000000 zerocap_api_new_test-0.1.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     2018 2023-07-29 08:24:12.000000 zerocap_api_new_test-0.1.1/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 08:25:59.000000 zerocap_api_new_test-0.1.1/zerocap_api_new_test/
--rw-r--r--   0 mac        (501) staff       (20)      121 2023-07-26 05:40:03.000000 zerocap_api_new_test-0.1.1/zerocap_api_new_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     7934 2023-07-29 07:56:08.000000 zerocap_api_new_test-0.1.1/zerocap_api_new_test/main.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 08:25:59.000000 zerocap_api_new_test-0.1.1/zerocap_api_new_test.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)    13885 2023-07-29 08:25:58.000000 zerocap_api_new_test-0.1.1/zerocap_api_new_test.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      312 2023-07-29 08:25:58.000000 zerocap_api_new_test-0.1.1/zerocap_api_new_test.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-29 08:25:58.000000 zerocap_api_new_test-0.1.1/zerocap_api_new_test.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-29 08:25:58.000000 zerocap_api_new_test-0.1.1/zerocap_api_new_test.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       21 2023-07-29 08:25:58.000000 zerocap_api_new_test-0.1.1/zerocap_api_new_test.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 08:51:19.000000 zerocap_api_new_test-0.1.2/
+-rw-r--r--   0 mac        (501) staff       (20)    11323 2023-07-24 01:35:05.000000 zerocap_api_new_test-0.1.2/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)    15377 2023-07-29 08:51:19.000000 zerocap_api_new_test-0.1.2/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)    13452 2023-07-29 08:06:55.000000 zerocap_api_new_test-0.1.2/README.rst
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-29 08:51:19.000000 zerocap_api_new_test-0.1.2/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     2018 2023-07-29 08:50:50.000000 zerocap_api_new_test-0.1.2/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 08:51:19.000000 zerocap_api_new_test-0.1.2/zerocap_api_new_test/
+-rw-r--r--   0 mac        (501) staff       (20)      121 2023-07-26 05:40:03.000000 zerocap_api_new_test-0.1.2/zerocap_api_new_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     7910 2023-07-29 08:36:16.000000 zerocap_api_new_test-0.1.2/zerocap_api_new_test/main.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 08:51:19.000000 zerocap_api_new_test-0.1.2/zerocap_api_new_test.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)    15377 2023-07-29 08:51:19.000000 zerocap_api_new_test-0.1.2/zerocap_api_new_test.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      312 2023-07-29 08:51:19.000000 zerocap_api_new_test-0.1.2/zerocap_api_new_test.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-29 08:51:19.000000 zerocap_api_new_test-0.1.2/zerocap_api_new_test.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-29 08:51:19.000000 zerocap_api_new_test-0.1.2/zerocap_api_new_test.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       21 2023-07-29 08:51:19.000000 zerocap_api_new_test-0.1.2/zerocap_api_new_test.egg-info/top_level.txt
```

### Comparing `zerocap_api_new_test-0.1.1/LICENSE.txt` & `zerocap_api_new_test-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerocap_api_new_test-0.1.1/PKG-INFO` & `zerocap_api_new_test-0.1.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: zerocap_api_new_test
-Version: 0.1.1
-Summary: zerocap_api
-Home-page: https://zerocap.com/
-Author: zerocap
-Author-email: jiayu.gao@eigen.capital
-License: MIT
-Platform: all
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-
 # zerocap-api-test 
 
 # <a href="#testapi">Jump restapi</a>
 # <a href="#test">Jump websocket</a>
 
 
 
@@ -409,7 +392,9 @@
         \"Cost\":\"1000000\",
         \"ExecPrice\":\"\",
         \"OrderFrom\":\"coinroutes\
     "}"
 }
 
 ```
+
+
```

#### html2text {}

```diff
@@ -1,15 +1,9 @@
-Metadata-Version: 2.1 Name: zerocap_api_new_test Version: 0.1.1 Summary:
-zerocap_api Home-page: https://zerocap.com/ Author: zerocap Author-email:
-jiayu.gao@eigen.capital License: MIT Platform: all Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE.txt # zerocap-
-api-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install pip
-install zerocap-api-test ã ã ã ``` # restapi get https://dma-
+# zerocap-api-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install
+pip install zerocap-api-test ã ã ã ``` # restapi get https://dma-
 api.defi.wiki/redoc #### 1. Create an order post https://dma-api.defi.wiki/
 orders/create_order è¯·æ±åæ°: | Parameter | required | data type | describe
 | Value range | |-----------------|-----------|-----------|-----------------|--
 ------------| | symbol | true | string | Instrument | USDT/AUD | | side | true
 | string | Side | buy sell | | type | true | string | Type | market limit | |
 amount | true | string | Quantity | | | price | true | string | Price | | |
 client_order_id | true | string | Client order id | | | account_vault | true |
```

### Comparing `zerocap_api_new_test-0.1.1/README.rst` & `zerocap_api_new_test-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,91 @@
-# zerocap-api-test 
+Metadata-Version: 2.1
+Name: zerocap_api_new_test
+Version: 0.1.2
+Summary: zerocap_api
+Home-page: https://zerocap.com/
+Author: zerocap
+Author-email: jiayu.gao@eigen.capital
+License: MIT
+Platform: all
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+# zerocap-api-new-test 
 
 # <a href="#testapi">Jump restapi</a>
 # <a href="#test">Jump websocket</a>
 
 
 
 ```
 
 描述介绍
 
 sdk install
-pip install zerocap-api-test
+pip install zerocap-api-new-test 
 。
 。
 。
 
 ```
 
 
 
 # <a id='testapi' href='https://dma-api.defi.wiki/redoc'>restapi </a>
-get https://dma-api.defi.wiki/redoc
+#### <a href="https://dma-api.defi.wiki/redoc" target="_blank">接口文档</a> 
 
+```
+from zerocap_api_new_test import ZerocapRestClient
+import uuid
+import time
 
+# API key and secret required, 联系zerocap进行注册
+apiKey = "coinroutes" 
+apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
+```
 
 #### 1. Create an order
-post https://dma-api.defi.wiki/orders/create_order
+<!--post https://dma-api.defi.wiki/orders/create_order-->
+
+```
+
+client = ZerocapRestClient(apiKey, apiSecret)
+client_order_id = str(uuid.uuid4())
+
+result = client.create_order(
+                    symbol='USDT/AUD', 
+                    side='buy', 
+                    type='market', 
+                    amount='100', 
+                    price='1000', 
+                    client_order_id=client_order_id, 
+                    note='this is test', 
+                    third_identity_id='ZCStreamingLiquidity1')
 
+```
 
 
 请求参数:
 
 | Parameter       | required  | data type | describe        | Value range  |
 |-----------------|-----------|-----------|-----------------|--------------|
 | symbol          | true      | string    | Instrument      | USDT/AUD     |
 | side            | true      | string    | Side            | buy sell     |
 | type            | true      | string    | Type            | market limit |
 | amount          | true      | string    | Quantity        |              |
 | price           | true      | string    | Price           |              |
 | client_order_id | true      | string    | Client order id |              |
-| account_vault   | true      | json      | accountVault    |              |
+| note | true      | string    | Client order id |              |
+| third_identity_id | true      | string    | Client order id |              |
 
 请求参数：示例（不能直接使用,需要替换自己的参数）
 
 ```
 
 {
     "symbol": "USDT/AUD",
@@ -127,24 +169,25 @@
 
 ```
 
 
 
 
 #### 2. Fetch specific orders
-post https://dma-api.defi.wiki/orders/fetch_order
-
+<!--post https://dma-api.defi.wiki/orders/fetch_order-->
+```
+result = client.fetch_order(id='')
+```
 
 请求参数:
 
 
 | Parameter       | required | data type | describe       | Value range  |
 |-----------------|----------|-----------|----------------|--------------|
 | id              | true     | string    | Transaction ID |              |
-| account_vault   | true     | json      | accountVault   |              |
 
 请求参数：示例（不能直接使用,需要替换自己的参数）
 
 ```
 
 {
     "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
@@ -160,28 +203,32 @@
 
 响应数据 接口报错 待定:
 
 
 | Parameter     | required | data type | describe       | Value range |
 |---------------|----------|-----------|----------------|-------------|
 | id            | true     | string    | Transaction ID |             |
-| account_vault | true     | json      | accountVault   |             |
 
 
 响应例子:
 
 ```
 
 {}
 
 ```
 
 
 #### 3. Batch fetch order
-post https://dma-api.defi.wiki/orders/fetch_orders
+<!--post https://dma-api.defi.wiki/orders/fetch_orders-->
+
+```
+result = client.fetch_orders(symbol='USDT/AUD', start_datetime=int(time.time() * 1000 - 86400), limit=10)
+
+```
 
 
 
 请求参数:
 
 | Parameter      | required | data type | describe        | Value range |
 |----------------|----------|-----------|-----------------|-------------|
@@ -191,15 +238,15 @@
 | page           | true     | string    | page            |             |
 | limit          | true     | string    | limit           |             |
 | ids            | true     | string    | Transaction ids |             |
 | status         | true     | string    | status          |             |
 | sort_order     | true     | string    | sort_order      |             |
 | order_type     | true     | string    | order_type      |             |
 | side           | true     | string    | side            |             |
-| account_vau lt | true     | j son     | accountVault    |             |
+
 
 请求参数：示例（不能直接使用,需要替换自己的参数）
 
 ```
 
 {
     "symbol": "",
@@ -241,20 +288,39 @@
 
 ```
 
 
 
 ## <span id='test'>websocket</span>
 
+```
+from zerocap_api_new_test import ZerocapWebsocketClient
+
+# API key and secret required, 联系zerocap进行注册
+apiKey = "coinroutes" 
+apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
+```
+
 #### 1. Subscribe to Market data
 
+<!--websocket wss://dma-api.defi.wiki/ws/GetMarket-->
+
+```
+market_connect = websocket.get_market()
 
-websocket wss://dma-api.defi.wiki/ws/GetMarket
+while True:
+    # Get  messages
+    message = websocket.get_message(market_connect)
 
+    print(f"Receiving message from server: \n{message}")
+    if not message:
+        print("Connection close")
+        break
 
+```
 
 请求参数:
 
 | Parameter     | required | data type | describe                | Value range |
 |---------------|----------|-----------|-------------------------|-------------|
 | api_key       | true     | string    | key                     |             |
 | signature     | true     | long      | Cryptographic signature |             |
@@ -300,16 +366,29 @@
 }
 
 ```
 
 #### 2.  Subscribe Order updates or transaction records
 
 
-websocket wss://dma-api.defi.wiki/ws/GetOrdersInfo
+<!--websocket url:   wss://dma-api.defi.wiki/ws/GetOrdersInfo-->
 
+```
+orders_connect = websocket.get_orders()
+
+while True:
+    # Get  messages
+    message = websocket.get_message(orders_connect)
+
+    print(f"Receiving message from server: \n{message}")
+    if not message:
+        print("Connection close")
+        break
+
+```
 
 
 请求参数:
 
 
 | Parameter     | required | data type | describe                | Value range |
 |---------------|----------|-----------|-------------------------|-------------|
@@ -392,9 +471,7 @@
         \"Cost\":\"1000000\",
         \"ExecPrice\":\"\",
         \"OrderFrom\":\"coinroutes\
     "}"
 }
 
 ```
-
-
```

#### html2text {}

```diff
@@ -1,17 +1,29 @@
-# zerocap-api-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install
-pip install zerocap-api-test ã ã ã ``` # restapi get https://dma-
-api.defi.wiki/redoc #### 1. Create an order post https://dma-api.defi.wiki/
-orders/create_order è¯·æ±åæ°: | Parameter | required | data type | describe
-| Value range | |-----------------|-----------|-----------|-----------------|--
-------------| | symbol | true | string | Instrument | USDT/AUD | | side | true
-| string | Side | buy sell | | type | true | string | Type | market limit | |
-amount | true | string | Quantity | | | price | true | string | Price | | |
-client_order_id | true | string | Client order id | | | account_vault | true |
-json | accountVault | |
+Metadata-Version: 2.1 Name: zerocap_api_new_test Version: 0.1.2 Summary:
+zerocap_api Home-page: https://zerocap.com/ Author: zerocap Author-email:
+jiayu.gao@eigen.capital License: MIT Platform: all Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE.txt # zerocap-
+api-new-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install pip
+install zerocap-api-new-test ã ã ã ``` # restapi #### æ¥å£ææ¡£ ```
+from zerocap_api_new_test import ZerocapRestClient import uuid import time #
+API key and secret required, èç³»zerocapè¿è¡æ³¨å apiKey = "coinroutes"
+apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a" ``` #### 1. Create an order
+``` client = ZerocapRestClient(apiKey, apiSecret) client_order_id = str
+(uuid.uuid4()) result = client.create_order( symbol='USDT/AUD', side='buy',
+type='market', amount='100', price='1000', client_order_id=client_order_id,
+note='this is test', third_identity_id='ZCStreamingLiquidity1') ```
+è¯·æ±åæ°: | Parameter | required | data type | describe | Value range | |--
+---------------|-----------|-----------|-----------------|--------------| |
+symbol | true | string | Instrument | USDT/AUD | | side | true | string | Side
+| buy sell | | type | true | string | Type | market limit | | amount | true |
+string | Quantity | | | price | true | string | Price | | | client_order_id |
+true | string | Client order id | | | note | true | string | Client order id |
+| | third_identity_id | true | string | Client order id | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "symbol": "USDT/AUD", "side": "buy", "type": "market", "amount": "1000",
 "price": "1000", "client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
 "account_vault": { "third_identity_id": "918d7125916c13191f3674e", "api_key":
 "***", "signature": "***", "note": "" } } ``` ååºæ°æ®: | Parameter |
 required | data type | describe | Value range | |--------------------|---------
 -|-----------|-----------------|-------------| | id | true | long | Transaction
@@ -31,68 +43,74 @@
 "average": "1.685133171", "amount": "9", "filled": "9", "remaining": "0",
 "cost": "15.16619854", "transferId": "12424971-f51d-4144-a205-9e306eb6351c",
 "trades": [ { "id": "12424971-f51d-4144-a205-9e306eb6351c", "timestamp":
 "1690535984000", "datetime": "2023-07-28 09:19:45", "symbol": "USDT/AUD",
 "order": "16ef58d1-677e-489c-8fe0-5acc4a680b6e", "type": "market", "side":
 "buy", "takerOrMaker": "taker", "price": "1.685133171", "amount": "9", "cost":
 "15.16619854", "orderFrom": "coinroutes" } ] } ``` #### 2. Fetch specific
-orders post https://dma-api.defi.wiki/orders/fetch_order è¯·æ±åæ°: |
-Parameter | required | data type | describe | Value range | |-----------------
-|----------|-----------|----------------|--------------| | id | true | string |
-Transaction ID | | | account_vault | true | json | accountVault | |
+orders  ``` result = client.fetch_order(id='') ``` è¯·æ±åæ°: | Parameter |
+required | data type | describe | Value range | |-----------------|----------|-
+----------|----------------|--------------| | id | true | string | Transaction
+ID | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e", "account_vault":
 { "third_identity_id": "918d7125916c13191f3674e", "api_key": "***",
 "signature": "***", "note": "" } } ``` ååºæ°æ® æ¥å£æ¥é å¾å®: |
 Parameter | required | data type | describe | Value range | |---------------|--
 --------|-----------|----------------|-------------| | id | true | string |
-Transaction ID | | | account_vault | true | json | accountVault | |
-ååºä¾å­: ``` {} ``` #### 3. Batch fetch order post https://dma-
-api.defi.wiki/orders/fetch_orders è¯·æ±åæ°: | Parameter | required | data
-type | describe | Value range | |----------------|----------|-----------|------
------------|-------------| | symbol | true | string | symbol | | |
-start_datetime | true | string | start_datetime | | | end_datetime | true |
-string | end_datetime | | | page | true | string | page | | | limit | true |
-string | limit | | | ids | true | string | Transaction ids | | | status | true
-| string | status | | | sort_order | true | string | sort_order | | |
-order_type | true | string | order_type | | | side | true | string | side | | |
-account_vau lt | true | j son | accountVault | |
+Transaction ID | | ååºä¾å­: ``` {} ``` #### 3. Batch fetch order  ```
+result = client.fetch_orders(symbol='USDT/AUD', start_datetime=int(time.time()
+* 1000 - 86400), limit=10) ``` è¯·æ±åæ°: | Parameter | required | data type
+| describe | Value range | |----------------|----------|-----------|-----------
+------|-------------| | symbol | true | string | symbol | | | start_datetime |
+true | string | start_datetime | | | end_datetime | true | string |
+end_datetime | | | page | true | string | page | | | limit | true | string |
+limit | | | ids | true | string | Transaction ids | | | status | true | string
+| status | | | sort_order | true | string | sort_order | | | order_type | true
+| string | order_type | | | side | true | string | side | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "symbol": "", "start_datetime": 0, "end_datetime": 0, "page": 0, "limit": 0,
 "ids": "", "status": "", "sort_order": "", "order_type": "", "side": "",
 "account_vault": { "third_identity_id": "918d7125916c13191f3674e", "api_key":
 "***", "signature": "***", "note": "" } } ``` ååºæ°æ® æ¥å£æ¥é å¾å®:
 | Parameter | required | data type | describe | Value range | |---------------
 |----------|-----------|----------------|-------------| | id | true | string |
 Transaction ID | | | account_vault | true | json | accountVault | |
-ååºä¾å­: ``` {} ``` ## websocket #### 1. Subscribe to Market data
-websocket wss://dma-api.defi.wiki/ws/GetMarket è¯·æ±åæ°: | Parameter |
-required | data type | describe | Value range | |---------------|----------|---
---------|-------------------------|-------------| | api_key | true | string |
-key | | | signature | true | long | Cryptographic signature | | | data_type |
-true | string | Subscribed Channels | price |
+ååºä¾å­: ``` {} ``` ## websocket ``` from zerocap_api_new_test import
+ZerocapWebsocketClient # API key and secret required, èç³»zerocapè¿è¡æ³¨å
+apiKey = "coinroutes" apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a" ```
+#### 1. Subscribe to Market data  ``` market_connect = websocket.get_market()
+while True: # Get messages message = websocket.get_message(market_connect)
+print(f"Receiving message from server: \n{message}") if not message: print
+("Connection close") break ``` è¯·æ±åæ°: | Parameter | required | data type
+| describe | Value range | |---------------|----------|-----------|------------
+-------------|-------------| | api_key | true | string | key | | | signature |
+true | long | Cryptographic signature | | | data_type | true | string |
+Subscribed Channels | price |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 wss://dma-api.defi.wiki/ws/
 GetMarket?api_key=coinroutes&signature=2585311b823982b325b266e132cd8cdf88d190ca61706dda5a67d421b23005df&data_type=price
 ``` ååºæ°æ®: | Parameter | required | data type | describe | Value range |
 |----------------------|----------|-----------|----------|--------------------
 | | type | true | long | type | | | channel | true | string | channel |
 dma_price_USDT/AUD | | data | true | jsonstr | data | | | data['sell_price'] |
 true | string | data | sell price | | data['buy_price'] | true | string | data
 | buy price | | data['datetime'] | true | string | data | time | | data
 ['timestamp'] | true | string | data | time | ååºä¾å­: ``` { "type":
 "message", "channel": "dma_price_USDT/AUD", "data": "{ \"sell_price\":
 \"1.322544321902561296\", \"buy_price\": \"1.668209315127094362\",
 \"datetime\": \"2023-07-28 10:03:40\", \"timestamp\": \"1690538620.1056492\" }"
-} ``` #### 2. Subscribe Order updates or transaction records websocket wss://
-dma-api.defi.wiki/ws/GetOrdersInfo è¯·æ±åæ°: | Parameter | required | data
-type | describe | Value range | |---------------|----------|-----------|-------
-------------------|-------------| | api_key | true | string | key | | |
-signature | true | long | Cryptographic signature | | | data_type | true |
-string | Subscribed Channels | order,trade |
+} ``` #### 2. Subscribe Order updates or transaction records  ```
+orders_connect = websocket.get_orders() while True: # Get messages message =
+websocket.get_message(orders_connect) print(f"Receiving message from server: \n
+{message}") if not message: print("Connection close") break ``` è¯·æ±åæ°: |
+Parameter | required | data type | describe | Value range | |---------------|--
+--------|-----------|-------------------------|-------------| | api_key | true
+| string | key | | | signature | true | long | Cryptographic signature | | |
+data_type | true | string | Subscribed Channels | order,trade |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 wss://dma-api.defi.wiki/ws/
 GetOrdersInfo?api_key=coinroutes&signature=2585311b823982b325b266e132cd8cdf88d190ca61706dda5a67d421b23005df&data_type=order,trade
 ``` dma_order_info ååºæ°æ®: | Parameter | required | data type | describe
 | Value range | |-----------------------|------------|-----------|-------------
 --|--------------------------------| | type | true | long | type | | | channel
 | true | string | channel | dma_order_info dma_trader_info | | data | true |
```

### Comparing `zerocap_api_new_test-0.1.1/setup.py` & `zerocap_api_new_test-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         os.system('git tag v{0}'.format(about['__version__']))
         os.system('git push --tags')
 
         sys.exit()
 
 setup(
     name='zerocap_api_new_test',  # 包名
-    version='0.1.1',  # 版本号
+    version='0.1.2',  # 版本号
     description='zerocap_api',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='zerocap',
     author_email='jiayu.gao@eigen.capital',
     url='https://zerocap.com/',
     install_requires=REQUIRED,
```

### Comparing `zerocap_api_new_test-0.1.1/zerocap_api_new_test/main.py` & `zerocap_api_new_test-0.1.2/zerocap_api_new_test/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
                 "signature": signature,
                 "note": note,
             }
         }
         response = requests.post(url, data=json.dumps(data), headers=headers)
         if response.status_code == 200:
             res = response.json()
-            return res["data"]
+            return res
         else:
             raise Exception(response.text)
 
     def fetch_order(
         self, id: str,
         note: str = '', 
         third_identity_id: str = ''
@@ -187,15 +187,15 @@
                 "signature": signature,
                 "note": note,
             }
         }
         response = requests.post(url, data=json.dumps(data), headers=headers)
         if response.status_code == 200:
             res = response.json()
-            return res["data"]
+            return res
         else:
             raise Exception(response.text)
 
     def fetch_orders(
         self, 
         symbol: str = '', 
         start_datetime: int = '', 
@@ -235,10 +235,10 @@
                 "signature": signature,
                 "note": note,
             }
         }
         response = requests.post(url, data=json.dumps(data), headers=headers)
         if response.status_code == 200:
             res = response.json()
-            return res["data"]
+            return res
         else:
             raise Exception(response.text)
```

### Comparing `zerocap_api_new_test-0.1.1/zerocap_api_new_test.egg-info/PKG-INFO` & `zerocap_api_new_test-0.1.2/zerocap_api_new_test.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,91 @@
 Metadata-Version: 2.1
 Name: zerocap-api-new-test
-Version: 0.1.1
+Version: 0.1.2
 Summary: zerocap_api
 Home-page: https://zerocap.com/
 Author: zerocap
 Author-email: jiayu.gao@eigen.capital
 License: MIT
 Platform: all
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
-# zerocap-api-test 
+# zerocap-api-new-test 
 
 # <a href="#testapi">Jump restapi</a>
 # <a href="#test">Jump websocket</a>
 
 
 
 ```
 
 描述介绍
 
 sdk install
-pip install zerocap-api-test
+pip install zerocap-api-new-test 
 。
 。
 。
 
 ```
 
 
 
 # <a id='testapi' href='https://dma-api.defi.wiki/redoc'>restapi </a>
-get https://dma-api.defi.wiki/redoc
+#### <a href="https://dma-api.defi.wiki/redoc" target="_blank">接口文档</a> 
 
+```
+from zerocap_api_new_test import ZerocapRestClient
+import uuid
+import time
 
+# API key and secret required, 联系zerocap进行注册
+apiKey = "coinroutes" 
+apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
+```
 
 #### 1. Create an order
-post https://dma-api.defi.wiki/orders/create_order
+<!--post https://dma-api.defi.wiki/orders/create_order-->
+
+```
 
+client = ZerocapRestClient(apiKey, apiSecret)
+client_order_id = str(uuid.uuid4())
+
+result = client.create_order(
+                    symbol='USDT/AUD', 
+                    side='buy', 
+                    type='market', 
+                    amount='100', 
+                    price='1000', 
+                    client_order_id=client_order_id, 
+                    note='this is test', 
+                    third_identity_id='ZCStreamingLiquidity1')
+
+```
 
 
 请求参数:
 
 | Parameter       | required  | data type | describe        | Value range  |
 |-----------------|-----------|-----------|-----------------|--------------|
 | symbol          | true      | string    | Instrument      | USDT/AUD     |
 | side            | true      | string    | Side            | buy sell     |
 | type            | true      | string    | Type            | market limit |
 | amount          | true      | string    | Quantity        |              |
 | price           | true      | string    | Price           |              |
 | client_order_id | true      | string    | Client order id |              |
-| account_vault   | true      | json      | accountVault    |              |
+| note | true      | string    | Client order id |              |
+| third_identity_id | true      | string    | Client order id |              |
 
 请求参数：示例（不能直接使用,需要替换自己的参数）
 
 ```
 
 {
     "symbol": "USDT/AUD",
@@ -144,24 +169,25 @@
 
 ```
 
 
 
 
 #### 2. Fetch specific orders
-post https://dma-api.defi.wiki/orders/fetch_order
-
+<!--post https://dma-api.defi.wiki/orders/fetch_order-->
+```
+result = client.fetch_order(id='')
+```
 
 请求参数:
 
 
 | Parameter       | required | data type | describe       | Value range  |
 |-----------------|----------|-----------|----------------|--------------|
 | id              | true     | string    | Transaction ID |              |
-| account_vault   | true     | json      | accountVault   |              |
 
 请求参数：示例（不能直接使用,需要替换自己的参数）
 
 ```
 
 {
     "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e",
@@ -177,28 +203,32 @@
 
 响应数据 接口报错 待定:
 
 
 | Parameter     | required | data type | describe       | Value range |
 |---------------|----------|-----------|----------------|-------------|
 | id            | true     | string    | Transaction ID |             |
-| account_vault | true     | json      | accountVault   |             |
 
 
 响应例子:
 
 ```
 
 {}
 
 ```
 
 
 #### 3. Batch fetch order
-post https://dma-api.defi.wiki/orders/fetch_orders
+<!--post https://dma-api.defi.wiki/orders/fetch_orders-->
+
+```
+result = client.fetch_orders(symbol='USDT/AUD', start_datetime=int(time.time() * 1000 - 86400), limit=10)
+
+```
 
 
 
 请求参数:
 
 | Parameter      | required | data type | describe        | Value range |
 |----------------|----------|-----------|-----------------|-------------|
@@ -208,15 +238,15 @@
 | page           | true     | string    | page            |             |
 | limit          | true     | string    | limit           |             |
 | ids            | true     | string    | Transaction ids |             |
 | status         | true     | string    | status          |             |
 | sort_order     | true     | string    | sort_order      |             |
 | order_type     | true     | string    | order_type      |             |
 | side           | true     | string    | side            |             |
-| account_vau lt | true     | j son     | accountVault    |             |
+
 
 请求参数：示例（不能直接使用,需要替换自己的参数）
 
 ```
 
 {
     "symbol": "",
@@ -258,20 +288,39 @@
 
 ```
 
 
 
 ## <span id='test'>websocket</span>
 
+```
+from zerocap_api_new_test import ZerocapWebsocketClient
+
+# API key and secret required, 联系zerocap进行注册
+apiKey = "coinroutes" 
+apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
+```
+
 #### 1. Subscribe to Market data
 
+<!--websocket wss://dma-api.defi.wiki/ws/GetMarket-->
 
-websocket wss://dma-api.defi.wiki/ws/GetMarket
+```
+market_connect = websocket.get_market()
 
+while True:
+    # Get  messages
+    message = websocket.get_message(market_connect)
 
+    print(f"Receiving message from server: \n{message}")
+    if not message:
+        print("Connection close")
+        break
+
+```
 
 请求参数:
 
 | Parameter     | required | data type | describe                | Value range |
 |---------------|----------|-----------|-------------------------|-------------|
 | api_key       | true     | string    | key                     |             |
 | signature     | true     | long      | Cryptographic signature |             |
@@ -317,16 +366,29 @@
 }
 
 ```
 
 #### 2.  Subscribe Order updates or transaction records
 
 
-websocket wss://dma-api.defi.wiki/ws/GetOrdersInfo
+<!--websocket url:   wss://dma-api.defi.wiki/ws/GetOrdersInfo-->
+
+```
+orders_connect = websocket.get_orders()
+
+while True:
+    # Get  messages
+    message = websocket.get_message(orders_connect)
+
+    print(f"Receiving message from server: \n{message}")
+    if not message:
+        print("Connection close")
+        break
 
+```
 
 
 请求参数:
 
 
 | Parameter     | required | data type | describe                | Value range |
 |---------------|----------|-----------|-------------------------|-------------|
```

#### html2text {}

```diff
@@ -1,23 +1,29 @@
-Metadata-Version: 2.1 Name: zerocap-api-new-test Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: zerocap-api-new-test Version: 0.1.2 Summary:
 zerocap_api Home-page: https://zerocap.com/ Author: zerocap Author-email:
 jiayu.gao@eigen.capital License: MIT Platform: all Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt # zerocap-
-api-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install pip
-install zerocap-api-test ã ã ã ``` # restapi get https://dma-
-api.defi.wiki/redoc #### 1. Create an order post https://dma-api.defi.wiki/
-orders/create_order è¯·æ±åæ°: | Parameter | required | data type | describe
-| Value range | |-----------------|-----------|-----------|-----------------|--
-------------| | symbol | true | string | Instrument | USDT/AUD | | side | true
-| string | Side | buy sell | | type | true | string | Type | market limit | |
-amount | true | string | Quantity | | | price | true | string | Price | | |
-client_order_id | true | string | Client order id | | | account_vault | true |
-json | accountVault | |
+api-new-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install pip
+install zerocap-api-new-test ã ã ã ``` # restapi #### æ¥å£ææ¡£ ```
+from zerocap_api_new_test import ZerocapRestClient import uuid import time #
+API key and secret required, èç³»zerocapè¿è¡æ³¨å apiKey = "coinroutes"
+apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a" ``` #### 1. Create an order
+``` client = ZerocapRestClient(apiKey, apiSecret) client_order_id = str
+(uuid.uuid4()) result = client.create_order( symbol='USDT/AUD', side='buy',
+type='market', amount='100', price='1000', client_order_id=client_order_id,
+note='this is test', third_identity_id='ZCStreamingLiquidity1') ```
+è¯·æ±åæ°: | Parameter | required | data type | describe | Value range | |--
+---------------|-----------|-----------|-----------------|--------------| |
+symbol | true | string | Instrument | USDT/AUD | | side | true | string | Side
+| buy sell | | type | true | string | Type | market limit | | amount | true |
+string | Quantity | | | price | true | string | Price | | | client_order_id |
+true | string | Client order id | | | note | true | string | Client order id |
+| | third_identity_id | true | string | Client order id | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "symbol": "USDT/AUD", "side": "buy", "type": "market", "amount": "1000",
 "price": "1000", "client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
 "account_vault": { "third_identity_id": "918d7125916c13191f3674e", "api_key":
 "***", "signature": "***", "note": "" } } ``` ååºæ°æ®: | Parameter |
 required | data type | describe | Value range | |--------------------|---------
 -|-----------|-----------------|-------------| | id | true | long | Transaction
@@ -37,68 +43,74 @@
 "average": "1.685133171", "amount": "9", "filled": "9", "remaining": "0",
 "cost": "15.16619854", "transferId": "12424971-f51d-4144-a205-9e306eb6351c",
 "trades": [ { "id": "12424971-f51d-4144-a205-9e306eb6351c", "timestamp":
 "1690535984000", "datetime": "2023-07-28 09:19:45", "symbol": "USDT/AUD",
 "order": "16ef58d1-677e-489c-8fe0-5acc4a680b6e", "type": "market", "side":
 "buy", "takerOrMaker": "taker", "price": "1.685133171", "amount": "9", "cost":
 "15.16619854", "orderFrom": "coinroutes" } ] } ``` #### 2. Fetch specific
-orders post https://dma-api.defi.wiki/orders/fetch_order è¯·æ±åæ°: |
-Parameter | required | data type | describe | Value range | |-----------------
-|----------|-----------|----------------|--------------| | id | true | string |
-Transaction ID | | | account_vault | true | json | accountVault | |
+orders  ``` result = client.fetch_order(id='') ``` è¯·æ±åæ°: | Parameter |
+required | data type | describe | Value range | |-----------------|----------|-
+----------|----------------|--------------| | id | true | string | Transaction
+ID | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e", "account_vault":
 { "third_identity_id": "918d7125916c13191f3674e", "api_key": "***",
 "signature": "***", "note": "" } } ``` ååºæ°æ® æ¥å£æ¥é å¾å®: |
 Parameter | required | data type | describe | Value range | |---------------|--
 --------|-----------|----------------|-------------| | id | true | string |
-Transaction ID | | | account_vault | true | json | accountVault | |
-ååºä¾å­: ``` {} ``` #### 3. Batch fetch order post https://dma-
-api.defi.wiki/orders/fetch_orders è¯·æ±åæ°: | Parameter | required | data
-type | describe | Value range | |----------------|----------|-----------|------
------------|-------------| | symbol | true | string | symbol | | |
-start_datetime | true | string | start_datetime | | | end_datetime | true |
-string | end_datetime | | | page | true | string | page | | | limit | true |
-string | limit | | | ids | true | string | Transaction ids | | | status | true
-| string | status | | | sort_order | true | string | sort_order | | |
-order_type | true | string | order_type | | | side | true | string | side | | |
-account_vau lt | true | j son | accountVault | |
+Transaction ID | | ååºä¾å­: ``` {} ``` #### 3. Batch fetch order  ```
+result = client.fetch_orders(symbol='USDT/AUD', start_datetime=int(time.time()
+* 1000 - 86400), limit=10) ``` è¯·æ±åæ°: | Parameter | required | data type
+| describe | Value range | |----------------|----------|-----------|-----------
+------|-------------| | symbol | true | string | symbol | | | start_datetime |
+true | string | start_datetime | | | end_datetime | true | string |
+end_datetime | | | page | true | string | page | | | limit | true | string |
+limit | | | ids | true | string | Transaction ids | | | status | true | string
+| status | | | sort_order | true | string | sort_order | | | order_type | true
+| string | order_type | | | side | true | string | side | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "symbol": "", "start_datetime": 0, "end_datetime": 0, "page": 0, "limit": 0,
 "ids": "", "status": "", "sort_order": "", "order_type": "", "side": "",
 "account_vault": { "third_identity_id": "918d7125916c13191f3674e", "api_key":
 "***", "signature": "***", "note": "" } } ``` ååºæ°æ® æ¥å£æ¥é å¾å®:
 | Parameter | required | data type | describe | Value range | |---------------
 |----------|-----------|----------------|-------------| | id | true | string |
 Transaction ID | | | account_vault | true | json | accountVault | |
-ååºä¾å­: ``` {} ``` ## websocket #### 1. Subscribe to Market data
-websocket wss://dma-api.defi.wiki/ws/GetMarket è¯·æ±åæ°: | Parameter |
-required | data type | describe | Value range | |---------------|----------|---
---------|-------------------------|-------------| | api_key | true | string |
-key | | | signature | true | long | Cryptographic signature | | | data_type |
-true | string | Subscribed Channels | price |
+ååºä¾å­: ``` {} ``` ## websocket ``` from zerocap_api_new_test import
+ZerocapWebsocketClient # API key and secret required, èç³»zerocapè¿è¡æ³¨å
+apiKey = "coinroutes" apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a" ```
+#### 1. Subscribe to Market data  ``` market_connect = websocket.get_market()
+while True: # Get messages message = websocket.get_message(market_connect)
+print(f"Receiving message from server: \n{message}") if not message: print
+("Connection close") break ``` è¯·æ±åæ°: | Parameter | required | data type
+| describe | Value range | |---------------|----------|-----------|------------
+-------------|-------------| | api_key | true | string | key | | | signature |
+true | long | Cryptographic signature | | | data_type | true | string |
+Subscribed Channels | price |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 wss://dma-api.defi.wiki/ws/
 GetMarket?api_key=coinroutes&signature=2585311b823982b325b266e132cd8cdf88d190ca61706dda5a67d421b23005df&data_type=price
 ``` ååºæ°æ®: | Parameter | required | data type | describe | Value range |
 |----------------------|----------|-----------|----------|--------------------
 | | type | true | long | type | | | channel | true | string | channel |
 dma_price_USDT/AUD | | data | true | jsonstr | data | | | data['sell_price'] |
 true | string | data | sell price | | data['buy_price'] | true | string | data
 | buy price | | data['datetime'] | true | string | data | time | | data
 ['timestamp'] | true | string | data | time | ååºä¾å­: ``` { "type":
 "message", "channel": "dma_price_USDT/AUD", "data": "{ \"sell_price\":
 \"1.322544321902561296\", \"buy_price\": \"1.668209315127094362\",
 \"datetime\": \"2023-07-28 10:03:40\", \"timestamp\": \"1690538620.1056492\" }"
-} ``` #### 2. Subscribe Order updates or transaction records websocket wss://
-dma-api.defi.wiki/ws/GetOrdersInfo è¯·æ±åæ°: | Parameter | required | data
-type | describe | Value range | |---------------|----------|-----------|-------
-------------------|-------------| | api_key | true | string | key | | |
-signature | true | long | Cryptographic signature | | | data_type | true |
-string | Subscribed Channels | order,trade |
+} ``` #### 2. Subscribe Order updates or transaction records  ```
+orders_connect = websocket.get_orders() while True: # Get messages message =
+websocket.get_message(orders_connect) print(f"Receiving message from server: \n
+{message}") if not message: print("Connection close") break ``` è¯·æ±åæ°: |
+Parameter | required | data type | describe | Value range | |---------------|--
+--------|-----------|-------------------------|-------------| | api_key | true
+| string | key | | | signature | true | long | Cryptographic signature | | |
+data_type | true | string | Subscribed Channels | order,trade |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 wss://dma-api.defi.wiki/ws/
 GetOrdersInfo?api_key=coinroutes&signature=2585311b823982b325b266e132cd8cdf88d190ca61706dda5a67d421b23005df&data_type=order,trade
 ``` dma_order_info ååºæ°æ®: | Parameter | required | data type | describe
 | Value range | |-----------------------|------------|-----------|-------------
 --|--------------------------------| | type | true | long | type | | | channel
 | true | string | channel | dma_order_info dma_trader_info | | data | true |
```

