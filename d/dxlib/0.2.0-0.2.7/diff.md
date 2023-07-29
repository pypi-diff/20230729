# Comparing `tmp/dxlib-0.2.0.tar.gz` & `tmp/dxlib-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxlib-0.2.0.tar", last modified: Sat Jul 15 07:42:08 2023, max compression
+gzip compressed data, was "dxlib-0.2.7.tar", last modified: Sat Jul 29 07:59:45 2023, max compression
```

## Comparing `dxlib-0.2.0.tar` & `dxlib-0.2.7.tar`

### file list

```diff
@@ -1,30 +1,48 @@
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.768211 dxlib-0.2.0/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-07-15 07:42:08.765200 dxlib-0.2.0/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      526 2023-04-20 14:34:27.000000 dxlib-0.2.0/README.md
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.358830 dxlib-0.2.0/dxlib/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       19 2023-07-15 07:24:40.000000 dxlib-0.2.0/dxlib/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.636952 dxlib-0.2.0/dxlib/api/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       76 2023-07-15 05:54:39.000000 dxlib-0.2.0/dxlib/api/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1345 2023-07-15 07:08:40.000000 dxlib-0.2.0/dxlib/api/__main__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1343 2023-07-15 05:57:39.000000 dxlib-0.2.0/dxlib/api/alphavantage.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      569 2023-07-15 03:43:22.000000 dxlib-0.2.0/dxlib/api/logger.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      315 2023-07-15 04:34:42.000000 dxlib-0.2.0/dxlib/api/terminal.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1857 2023-07-15 04:12:02.000000 dxlib-0.2.0/dxlib/api/utils.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1448 2023-07-14 03:22:23.000000 dxlib-0.2.0/dxlib/app.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.676041 dxlib-0.2.0/dxlib/db/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-13 23:57:17.000000 dxlib-0.2.0/dxlib/db/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.746335 dxlib-0.2.0/dxlib/db/sql/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.2.0/dxlib/db/sql/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      153 2023-06-30 10:10:39.000000 dxlib-0.2.0/dxlib/db/sql/create.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      761 2023-06-30 10:14:21.000000 dxlib-0.2.0/dxlib/db/sql/queries.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4361 2023-07-14 00:49:31.000000 dxlib-0.2.0/dxlib/db/utils.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      404 2023-04-20 14:41:16.000000 dxlib-0.2.0/dxlib/euler_method.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      274 2023-04-20 14:39:35.000000 dxlib-0.2.0/dxlib/finite_differences.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.484872 dxlib-0.2.0/dxlib.egg-info/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-07-15 07:42:07.000000 dxlib-0.2.0/dxlib.egg-info/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      485 2023-07-15 07:42:08.000000 dxlib-0.2.0/dxlib.egg-info/SOURCES.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-15 07:42:07.000000 dxlib-0.2.0/dxlib.egg-info/dependency_links.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      119 2023-07-15 07:42:07.000000 dxlib-0.2.0/dxlib.egg-info/requires.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-15 07:42:07.000000 dxlib-0.2.0/dxlib.egg-info/top_level.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-15 07:42:08.768211 dxlib-0.2.0/setup.cfg
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:28:39.000000 dxlib-0.2.0/setup.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:45.003340 dxlib-0.2.7/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)    10948 2023-07-16 21:40:36.000000 dxlib-0.2.7/LICENSE
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3244 2023-07-29 07:59:44.999342 dxlib-0.2.7/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2487 2023-07-16 21:40:36.000000 dxlib-0.2.7/README.md
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:43.940454 dxlib-0.2.7/dxlib/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       95 2023-07-15 07:58:04.000000 dxlib-0.2.7/dxlib/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.304341 dxlib-0.2.7/dxlib/api/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      117 2023-07-29 07:41:11.000000 dxlib-0.2.7/dxlib/api/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      777 2023-07-29 07:56:12.000000 dxlib-0.2.7/dxlib/api/alpaca_markets.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1304 2023-07-15 07:58:04.000000 dxlib-0.2.7/dxlib/api/alphavantage.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3117 2023-07-29 07:33:09.000000 dxlib-0.2.7/dxlib/api/core.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:44.000000 dxlib-0.2.7/dxlib/api/logger.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:34.000000 dxlib-0.2.7/dxlib/api/terminal.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.452341 dxlib-0.2.7/dxlib/core/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:09.000000 dxlib-0.2.7/dxlib/core/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      387 2023-07-15 07:58:04.000000 dxlib-0.2.7/dxlib/core/euler_method.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      262 2023-07-15 07:58:04.000000 dxlib-0.2.7/dxlib/core/finite_differences.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     9503 2023-07-25 00:10:53.000000 dxlib-0.2.7/dxlib/core/options.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.528341 dxlib-0.2.7/dxlib/data/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       21 2023-07-15 07:58:04.000000 dxlib-0.2.7/dxlib/data/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2150 2023-07-15 09:26:56.000000 dxlib-0.2.7/dxlib/data/utils.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.603340 dxlib-0.2.7/dxlib/db/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      603 2023-07-17 19:47:05.000000 dxlib-0.2.7/dxlib/db/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.741341 dxlib-0.2.7/dxlib/db/sql/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.2.7/dxlib/db/sql/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      148 2023-07-15 07:58:04.000000 dxlib-0.2.7/dxlib/db/sql/create.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      730 2023-07-15 07:58:04.000000 dxlib-0.2.7/dxlib/db/sql/queries.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4241 2023-07-15 07:58:05.000000 dxlib-0.2.7/dxlib/db/utils.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.818341 dxlib-0.2.7/dxlib/models/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:31.000000 dxlib-0.2.7/dxlib/models/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:26:00.000000 dxlib-0.2.7/dxlib/models/systematic_trading.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     5388 2023-07-29 07:35:54.000000 dxlib-0.2.7/dxlib/portfolio_theory_module.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.854341 dxlib-0.2.7/dxlib/research/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:50:59.000000 dxlib-0.2.7/dxlib/research/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.928341 dxlib-0.2.7/dxlib/simulation/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:15.000000 dxlib-0.2.7/dxlib/simulation/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     7903 2023-07-15 07:58:05.000000 dxlib-0.2.7/dxlib/simulation/backtesting.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       80 2023-07-29 07:56:48.000000 dxlib-0.2.7/dxlib/test.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.965340 dxlib-0.2.7/dxlib/visualization/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:06:43.000000 dxlib-0.2.7/dxlib/visualization/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-29 07:59:44.081452 dxlib-0.2.7/dxlib.egg-info/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     3244 2023-07-29 07:59:43.000000 dxlib-0.2.7/dxlib.egg-info/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      810 2023-07-29 07:59:43.000000 dxlib-0.2.7/dxlib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-29 07:59:43.000000 dxlib-0.2.7/dxlib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       96 2023-07-29 07:59:43.000000 dxlib-0.2.7/dxlib.egg-info/requires.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-29 07:59:43.000000 dxlib-0.2.7/dxlib.egg-info/top_level.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-29 07:59:45.004341 dxlib-0.2.7/setup.cfg
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:44:19.000000 dxlib-0.2.7/setup.py
```

### Comparing `dxlib-0.2.0/dxlib/api/alphavantage.py` & `dxlib-0.2.7/dxlib/api/alphavantage.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import requests
-import pandas
-
-
-class AlphaVantageAPI:
-    def __init__(self, api_key):
-        self.api_key = api_key
-        self.base_url = 'https://www.alphavantage.co/query?'
-
-    def fetch_quote(self, symbol):
-        url = f'{self.base_url}function=GLOBAL_QUOTE&symbol={symbol}&apikey={self.api_key}'
-        response = requests.get(url)
-        data = response.json()
-        return data['Global Quote']
-
-    def fetch_currency_exchange_rates(self, currencies):
-        exchange_rates = []
-
-        for currency in currencies:
-            params = {
-                'function': 'CURRENCY_EXCHANGE_RATE',
-                'from_currency': 'USD',
-                'to_currency': currency,
-                'apikey': self.api_key
-            }
-
-            response = requests.get(self.base_url, params=params)
-            data = response.json()
-
-            try:
-                exchange_rate_data = data['Realtime Currency Exchange Rate']
-                exchange_rates.append({
-                    'Currency': currency,
-                    'Exchange Rate': exchange_rate_data['5. Exchange Rate'],
-                    'Last Refreshed': exchange_rate_data['6. Last Refreshed']
-                })
-            except KeyError:
-                print(data)
-        return pandas.DataFrame(exchange_rates)
+import requests
+import pandas
+
+
+class AlphaVantageAPI:
+    def __init__(self, api_key):
+        self.api_key = api_key
+        self.base_url = 'https://www.alphavantage.co/query?'
+
+    def fetch_quote(self, symbol):
+        url = f'{self.base_url}function=GLOBAL_QUOTE&symbol={symbol}&apikey={self.api_key}'
+        response = requests.get(url)
+        data = response.json()
+        return data['Global Quote']
+
+    def fetch_currency_exchange_rates(self, currencies):
+        exchange_rates = []
+
+        for currency in currencies:
+            params = {
+                'function': 'CURRENCY_EXCHANGE_RATE',
+                'from_currency': 'USD',
+                'to_currency': currency,
+                'apikey': self.api_key
+            }
+
+            response = requests.get(self.base_url, params=params)
+            data = response.json()
+
+            try:
+                exchange_rate_data = data['Realtime Currency Exchange Rate']
+                exchange_rates.append({
+                    'Currency': currency,
+                    'Exchange Rate': exchange_rate_data['5. Exchange Rate'],
+                    'Last Refreshed': exchange_rate_data['6. Last Refreshed']
+                })
+            except KeyError:
+                print(data)
+        return pandas.DataFrame(exchange_rates)
```

### Comparing `dxlib-0.2.0/dxlib/db/sql/queries.py` & `dxlib-0.2.7/dxlib/db/sql/queries.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-def GET_TABLES():
-    return """
-    SELECT table_name FROM user_tables;
-    """
-
-def GET_USERS():
-    return """
-    SELECT P.NOME FROM PESSOA P 
-    JOIN  
-    (SELECT A.CPF FROM ALUNO A WHERE NOT EXISTS (
-        (SELECT M.NOME, M.CURSO FROM MISSAO M
-            WHERE M.CURSO = 'Informatica1')
-            MINUS
-            (SELECT F.MISSAO, F.CURSO FROM FAZ F
-            WHERE F.ALUNO = A.CPF)
-        )
-    ) 
-    X ON P.CPF = X.CPF
-    """
-
-
-def GET_MISSIONS():
-    return """
-    SELECT P.NOME, F.CURSO, MISSOES_FEITAS FROM PESSOA P 
-    JOIN 
-    (SELECT A.CPF, F.CURSO, COUNT(*) AS MISSOES_FEITAS FROM ALUNO A
-        JOIN FAZ F ON (F.ALUNO = A.CPF)
-        GROUP BY A.CPF, F.CURSO 
-    ) 
-    ON P.CPF = A.CPF
-    """
+def GET_TABLES():
+    return """
+    SELECT table_name FROM user_tables;
+    """
+
+def GET_USERS():
+    return """
+    SELECT P.NOME FROM PESSOA P 
+    JOIN  
+    (SELECT A.CPF FROM ALUNO A WHERE NOT EXISTS (
+        (SELECT M.NOME, M.CURSO FROM MISSAO M
+            WHERE M.CURSO = 'Informatica1')
+            MINUS
+            (SELECT F.MISSAO, F.CURSO FROM FAZ F
+            WHERE F.ALUNO = A.CPF)
+        )
+    ) 
+    X ON P.CPF = X.CPF
+    """
+
+
+def GET_MISSIONS():
+    return """
+    SELECT P.NOME, F.CURSO, MISSOES_FEITAS FROM PESSOA P 
+    JOIN 
+    (SELECT A.CPF, F.CURSO, COUNT(*) AS MISSOES_FEITAS FROM ALUNO A
+        JOIN FAZ F ON (F.ALUNO = A.CPF)
+        GROUP BY A.CPF, F.CURSO 
+    ) 
+    ON P.CPF = A.CPF
+    """
```

### Comparing `dxlib-0.2.0/dxlib/db/utils.py` & `dxlib-0.2.7/dxlib/db/utils.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-from pymongo import MongoClient
-
-
-class DatabaseManager:
-    connection = None
-
-    def connect(self, host, port):
-        if not self.connection:
-            self.connection = MongoClient(host, port)
-
-    def create(self, command, cursor=None):
-        if not self.connection:
-            raise ConnectionError("Connect to DB!")
-        with cursor if cursor else self.connection.cursor() as cursor:
-            cursor.execute(command.value)
-
-    def get(self, command, cursor=None):
-        if not self.connection:
-            raise ConnectionError("Connect to DB!")
-        with cursor if cursor else self.connection.cursor() as cursor:
-            return list(cursor.execute(command.value))
-
-    def create_schema(self):
-        with open("sql/create_schema.sql") as file:
-            sql = file.read()
-
-        create = sql.split(";")
-        print(create)
-        print(self.connection)
-
-
-class Menu:
-    def __init__(self, name, identifier, paths: list = None, calls: list[dict] = None,
-                 text="Selecione uma opção para continuar:"):
-        self.name = name
-        self.identifier = identifier
-        self.paths = [] if not paths else paths
-        self.calls = [] if not calls else calls
-        self.text = text
-
-    def select(self, index):
-        if index < 0:
-            raise IndexError("Invalid option")
-        else:
-            return self.paths[index]
-
-    def call(self, index, *args, **kwargs):
-        if index >= len(self.calls):
-            raise IndexError("Invalid option")
-        else:
-            return self.calls[index]["method"](*args, **kwargs)
-
-
-class Navigation:
-    terminal = None
-
-    def __init__(self, starting_menu: Menu, terminal):
-        self.current_menu = starting_menu
-        self.previous_menus = []
-        self.terminal = terminal
-
-    def display(self, output=None):
-        self.terminal.clear()
-        self.terminal.header(f"Menu: { self.current_menu.name}\n")
-
-        if self.previous_menus:
-            self.terminal.print(f"0 - Return. \n")
-
-        for idx, path in enumerate(self.current_menu.paths):
-            self.terminal.print(f"{idx + 1} - {path.identifier}")
-
-        for idx, call in enumerate(self.current_menu.calls):
-            self.terminal.print(f"{len(self.current_menu.paths) + idx + 1} - {call['name']}")
-
-        self.terminal.print(f"{len(self.current_menu.paths) + len(self.current_menu.calls) + 1} - Exit \n")
-
-        if output:
-            self.terminal.log(json=output)
-
-    def listen(self):
-        while True:
-            option = int(self.terminal.get_input(self.current_menu.text + "\n"))
-
-            if option == (len(self.current_menu.paths) + len(self.current_menu.calls)) + 1:
-                raise SystemExit
-
-            if option == 0 and self.previous_menus:
-                self.current_menu = self.previous_menus.pop()
-                break
-
-            option -= 1
-
-            try:
-                if option < len(self.current_menu.paths):
-                    selected_menu = self.current_menu.select(option)
-                    self.enter_menu(selected_menu)
-                    break
-
-                else:
-                    try:
-                        call = self.current_menu.calls[option - len(self.current_menu.paths)]
-                        args = call.get("args", None)
-
-                        if args:
-                            args = self.terminal.get_input(f"Required parameters: {args}\n")
-                            output = self.current_menu.call(option - len(self.current_menu.paths), args.split(" "))
-                        else:
-                            output = self.current_menu.call(option - len(self.current_menu.paths))
-                        return output
-                    except ValueError as params:
-                        self.terminal.print(f"For the selected option {option}, provide the following params: {params}")
-
-            except IndexError:
-                self.terminal.print("Invalid option, please select a number between 0 e {}".format(
-                    len(self.current_menu.paths) + len(self.current_menu.calls) + 1
-                ))
-
-    def enter_menu(self, menu):
-        self.previous_menus.append(self.current_menu)
-        self.current_menu = menu
+from pymongo import MongoClient
+
+
+class DatabaseManager:
+    connection = None
+
+    def connect(self, host, port):
+        if not self.connection:
+            self.connection = MongoClient(host, port)
+
+    def create(self, command, cursor=None):
+        if not self.connection:
+            raise ConnectionError("Connect to DB!")
+        with cursor if cursor else self.connection.cursor() as cursor:
+            cursor.execute(command.value)
+
+    def get(self, command, cursor=None):
+        if not self.connection:
+            raise ConnectionError("Connect to DB!")
+        with cursor if cursor else self.connection.cursor() as cursor:
+            return list(cursor.execute(command.value))
+
+    def create_schema(self):
+        with open("sql/create_schema.sql") as file:
+            sql = file.read()
+
+        create = sql.split(";")
+        print(create)
+        print(self.connection)
+
+
+class Menu:
+    def __init__(self, name, identifier, paths: list = None, calls: list[dict] = None,
+                 text="Selecione uma opção para continuar:"):
+        self.name = name
+        self.identifier = identifier
+        self.paths = [] if not paths else paths
+        self.calls = [] if not calls else calls
+        self.text = text
+
+    def select(self, index):
+        if index < 0:
+            raise IndexError("Invalid option")
+        else:
+            return self.paths[index]
+
+    def call(self, index, *args, **kwargs):
+        if index >= len(self.calls):
+            raise IndexError("Invalid option")
+        else:
+            return self.calls[index]["method"](*args, **kwargs)
+
+
+class Navigation:
+    terminal = None
+
+    def __init__(self, starting_menu: Menu, terminal):
+        self.current_menu = starting_menu
+        self.previous_menus = []
+        self.terminal = terminal
+
+    def display(self, output=None):
+        self.terminal.clear()
+        self.terminal.header(f"Menu: { self.current_menu.name}\n")
+
+        if self.previous_menus:
+            self.terminal.print(f"0 - Return. \n")
+
+        for idx, path in enumerate(self.current_menu.paths):
+            self.terminal.print(f"{idx + 1} - {path.identifier}")
+
+        for idx, call in enumerate(self.current_menu.calls):
+            self.terminal.print(f"{len(self.current_menu.paths) + idx + 1} - {call['name']}")
+
+        self.terminal.print(f"{len(self.current_menu.paths) + len(self.current_menu.calls) + 1} - Exit \n")
+
+        if output:
+            self.terminal.log(json=output)
+
+    def listen(self):
+        while True:
+            option = int(self.terminal.get_input(self.current_menu.text + "\n"))
+
+            if option == (len(self.current_menu.paths) + len(self.current_menu.calls)) + 1:
+                raise SystemExit
+
+            if option == 0 and self.previous_menus:
+                self.current_menu = self.previous_menus.pop()
+                break
+
+            option -= 1
+
+            try:
+                if option < len(self.current_menu.paths):
+                    selected_menu = self.current_menu.select(option)
+                    self.enter_menu(selected_menu)
+                    break
+
+                else:
+                    try:
+                        call = self.current_menu.calls[option - len(self.current_menu.paths)]
+                        args = call.get("args", None)
+
+                        if args:
+                            args = self.terminal.get_input(f"Required parameters: {args}\n")
+                            output = self.current_menu.call(option - len(self.current_menu.paths), args.split(" "))
+                        else:
+                            output = self.current_menu.call(option - len(self.current_menu.paths))
+                        return output
+                    except ValueError as params:
+                        self.terminal.print(f"For the selected option {option}, provide the following params: {params}")
+
+            except IndexError:
+                self.terminal.print("Invalid option, please select a number between 0 e {}".format(
+                    len(self.current_menu.paths) + len(self.current_menu.calls) + 1
+                ))
+
+    def enter_menu(self, menu):
+        self.previous_menus.append(self.current_menu)
+        self.current_menu = menu
```

### Comparing `dxlib-0.2.0/setup.py` & `dxlib-0.2.7/setup.py`

 * *Files identical despite different names*

