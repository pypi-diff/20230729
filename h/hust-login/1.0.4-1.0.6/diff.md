# Comparing `tmp/hust_login-1.0.4.tar.gz` & `tmp/hust_login-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hust_login-1.0.4.tar", last modified: Thu Jul 27 07:45:12 2023, max compression
+gzip compressed data, was "hust_login-1.0.6.tar", last modified: Sat Jul 29 05:14:01 2023, max compression
```

## Comparing `hust_login-1.0.4.tar` & `hust_login-1.0.6.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:45:12.256513 hust_login-1.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:45:12.248513 hust_login-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:45:12.248513 hust_login-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-27 07:44:55.000000 hust_login-1.0.4/.github/workflows/auto-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-27 07:44:55.000000 hust_login-1.0.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 07:44:55.000000 hust_login-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 07:44:55.000000 hust_login-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 07:44:55.000000 hust_login-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-27 07:45:12.256513 hust_login-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-27 07:44:55.000000 hust_login-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-27 07:44:55.000000 hust_login-1.0.4/README_ZH.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:45:12.252514 hust_login-1.0.4/hust_login/
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-27 07:44:55.000000 hust_login-1.0.4/hust_login/_HustPass.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-27 07:44:55.000000 hust_login-1.0.4/hust_login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-27 07:44:55.000000 hust_login-1.0.4/hust_login/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-27 07:44:55.000000 hust_login-1.0.4/hust_login/autotest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-27 07:44:55.000000 hust_login-1.0.4/hust_login/curriculum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-27 07:44:55.000000 hust_login-1.0.4/hust_login/decaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-27 07:44:55.000000 hust_login-1.0.4/hust_login/ecard_bills.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-27 07:44:55.000000 hust_login-1.0.4/hust_login/free_room.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-27 07:44:55.000000 hust_login-1.0.4/hust_login/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-27 07:44:55.000000 hust_login-1.0.4/hust_login/utility_bills.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:45:12.252514 hust_login-1.0.4/hust_login.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-27 07:45:12.000000 hust_login-1.0.4/hust_login.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-27 07:45:12.000000 hust_login-1.0.4/hust_login.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 07:45:12.000000 hust_login-1.0.4/hust_login.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 07:45:12.000000 hust_login-1.0.4/hust_login.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 07:45:12.000000 hust_login-1.0.4/hust_login.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:45:12.252514 hust_login-1.0.4/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-27 07:44:55.000000 hust_login-1.0.4/images/captcha_code.gif
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-27 07:44:55.000000 hust_login-1.0.4/images/captcha_code_processed.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 07:44:55.000000 hust_login-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 07:45:12.256513 hust_login-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-27 07:44:55.000000 hust_login-1.0.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-27 07:44:55.000000 hust_login-1.0.4/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 05:14:01.740293 hust_login-1.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 05:14:01.736293 hust_login-1.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 05:14:01.736293 hust_login-1.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-29 05:13:44.000000 hust_login-1.0.6/.github/workflows/auto-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-29 05:13:44.000000 hust_login-1.0.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-29 05:13:44.000000 hust_login-1.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-29 05:13:44.000000 hust_login-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 05:13:44.000000 hust_login-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-29 05:14:01.740293 hust_login-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-29 05:13:44.000000 hust_login-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-29 05:13:44.000000 hust_login-1.0.6/README_ZH.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 05:14:01.736293 hust_login-1.0.6/hust_login/
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-29 05:13:44.000000 hust_login-1.0.6/hust_login/_HustPass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-29 05:13:44.000000 hust_login-1.0.6/hust_login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-29 05:13:44.000000 hust_login-1.0.6/hust_login/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-29 05:13:44.000000 hust_login-1.0.6/hust_login/autotest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-29 05:13:44.000000 hust_login-1.0.6/hust_login/curriculum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-29 05:13:44.000000 hust_login-1.0.6/hust_login/decaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-29 05:13:44.000000 hust_login-1.0.6/hust_login/ecard_bills.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-29 05:13:44.000000 hust_login-1.0.6/hust_login/example.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-29 05:13:44.000000 hust_login-1.0.6/hust_login/free_room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-07-29 05:13:44.000000 hust_login-1.0.6/hust_login/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-29 05:13:44.000000 hust_login-1.0.6/hust_login/utility_bills.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 05:14:01.740293 hust_login-1.0.6/hust_login.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-29 05:14:01.000000 hust_login-1.0.6/hust_login.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-29 05:14:01.000000 hust_login-1.0.6/hust_login.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 05:14:01.000000 hust_login-1.0.6/hust_login.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-29 05:14:01.000000 hust_login-1.0.6/hust_login.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 05:14:01.000000 hust_login-1.0.6/hust_login.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 05:14:01.740293 hust_login-1.0.6/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-29 05:13:44.000000 hust_login-1.0.6/images/captcha_code.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-29 05:13:44.000000 hust_login-1.0.6/images/captcha_code_processed.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-29 05:13:44.000000 hust_login-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 05:14:01.740293 hust_login-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-29 05:13:44.000000 hust_login-1.0.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-29 05:13:44.000000 hust_login-1.0.6/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-29 05:13:44.000000 hust_login-1.0.6/test_basic.py
```

### Comparing `hust_login-1.0.4/.github/workflows/auto-test.yml` & `hust_login-1.0.6/.github/workflows/auto-test.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Automated Testing of Interface Availability
 
 on:
   workflow_dispatch:
   schedule:
-    - cron: '0 14 * * 1' # run on every Monday 14:00
+    - cron: '0 6 * * *' # run on every day 14:00
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
 
     strategy:
       matrix:
```

### Comparing `hust_login-1.0.4/.github/workflows/ci.yml` & `hust_login-1.0.6/.github/workflows/ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 
 on: 
   push:
   pull_request:
 
 jobs:
   build:
-    runs-on: ${{ matrix.os }}
-
-    strategy:
-      matrix:
-        os: [ubuntu-latest] #[windows-latest, macos-latest, ubuntu-latest]
+    runs-on: ubuntu-latest
 
     steps:
       - name: Checkout code
         uses: actions/checkout@v3
 
       - name: Set up python
         uses: actions/setup-python@v3
@@ -81,28 +77,25 @@
 
     if: startsWith(github.ref, 'refs/tags/')
 
     permissions:
       contents: write
 
     steps:
-      - name: Check if push is tag
-        run: 
-          echo "Push is a tag"
-
       - name: Download artifacts
         uses: actions/download-artifact@v3
 
       - name: Create Release
         uses: softprops/action-gh-release@v1
         with:
           files: |
-            artifact/hust_login-*.whl
+            artifact/*
 
       - name: Publish package
+        if: (! endsWith(github.ref, 'dev'))
         uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
           packages_dir: artifact
           repository_url: https://upload.pypi.org/legacy/
```

### Comparing `hust_login-1.0.4/LICENSE` & `hust_login-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.4/PKG-INFO` & `hust_login-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hust_login
-Version: 1.0.4
+Version: 1.0.6
 Summary: A python-lib for authenticating HustPass@2023
 Home-page: https://github.com/MarvinTerry/HustLogin
 Author: MarvinTerry
 Author-email: marvinterry2004@gmail.com
 Maintainer: Jackhr
 Maintainer-email: jj2460596@gmail.com
 License: MIT
```

### Comparing `hust_login-1.0.4/README.md` & `hust_login-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.4/README_ZH.md` & `hust_login-1.0.6/README_ZH.md`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.4/hust_login/_HustPass.py` & `hust_login-1.0.6/hust_login/_HustPass.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .login import HustLogin, CheckLoginStatu
 from .utility_bills import GetElectricityBill
-from .curriculum import GetCurriculum
-from .free_room import GetFreeRoom
+from .curriculum import QuerySchedules
+from .free_room import GetFreeRooms
 from .ecard_bills import GetEcardBills
 
 class HustPass_NotLoged(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 class HustPass:
@@ -40,40 +40,40 @@
         \n
         RETURN:\n
         {'RoomName': 'XXX', 'RemainPower': 'XXX', 'DayCost': [{'daycost': 'XXX', 'date': 'YYYY-MM-DD', 'money': 'XXX'}]}
         '''
         self.CheckLoged()
         return GetElectricityBill(self.Session, self.Uid, QueryDates)
     
-    def QueryCurriculum(self, QueryData:str|list[str]|int|tuple[str,str]) -> list:
+    def QuerySchedules(self, QueryData:str|list[str]|int|tuple[str,str]) -> list:
         '''
         PARAMETERS:\n
         session -- should be already logged in\n
         date    -- str  : the day you want, in form of YYYY-MM-DD\n
                 -- list : a list, each item in the same form as above\n
                 -- int  : the week after the semester started\n
                 -- tuple: two str, including the start and the end\n
         \n
         RETURN:\n
         [{'Date':'YYYY-MM-DD','Curriculum':[{'No':'1', 'ClassName': 'XXX', 'TeacherName': 'XXX'}]}]
         '''
         self.CheckLoged()
-        return GetCurriculum(self.Session, QueryData)
+        return QuerySchedules(self.Session, QueryData)
     
-    def QueryFreeRoom(self, QueryData:str) -> dict:
+    def QueryFreeRooms(self, QueryData:str) -> dict:
         '''
         PARAMETERS:\n
         session -- should be already logged in\n
         date    -- str  : the day you want, in form of YYYY-MM-DD\n
         \n
         RETURN:\n
         {'Date':'YYYY-MM-DD','Buildings':['东九楼A':{'No':'1','Roomlist': ['A101','A102']}]}
         '''
         self.CheckLoged()
-        return GetFreeRoom(self.Session, QueryData)
+        return GetFreeRooms(self.Session, QueryData)
     
     def QueryEcardBills(self, QueryData:str|list[str]|tuple[str,str]) -> list:
         '''
         PARAMETERS:\n
         session     -- should be already logged in\n
         Uid         -- str  : your student uid\n
         QueryDates  -- str  : in form of '2023-7-21' or '2023/7/21'\n
```

### Comparing `hust_login-1.0.4/hust_login/autotest.py` & `hust_login-1.0.6/hust_login/autotest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from . import HustPass
-
-def full_test(Uid,Pwd):
-    hpass = HustPass(Uid, Pwd)
+def full_test(hpass):
     try:
         hpass.QueryCurriculum('2023-04-27')
         hpass.QueryCurriculum(['2023-04-27','2023-03-27','2023-04-07'])
         hpass.QueryCurriculum(8)
         hpass.QueryCurriculum(('2023-04-01','2023-04-12'))
     except:
         return 10
@@ -15,8 +12,12 @@
         hpass.QueryElectricityBills(('2023-04-01','2023-04-12'))
     except:
         return 20
     try:
         hpass.QueryFreeRoom('2023-09-02')
     except:
         return 30
+    try:
+        hpass.QueryEcardBills('2023-09-02')
+    except:
+        return 40
     return 0
```

### Comparing `hust_login-1.0.4/hust_login/curriculum.py` & `hust_login-1.0.6/hust_login/curriculum.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     for item in content:
         if item['kc'][0]['JSMC']=='—':
             continue
         class_list.append({'No':item['jcx'],'course':item['kc'][0]['KCMC'],'teacher':item['kc'][0]['XM'],'place':item['kc'][0]['JSMC']})
     ret['curriculum'] = class_list
     return ret
 
-def GetCurriculum(session:requests.Session, _date_query:str|list[str]|int|tuple[str,str]) -> list:
+def QuerySchedules(session:requests.Session, _date_query:str|list[str]|int|tuple[str,str]) -> list:
     '''
     PARAMETERS:\n
     session -- should be already logged in\n
     date    -- str  : the day you want, in form of YYYY-MM-DD\n
             -- list : a list, each item in the same form as above\n
             -- int  : the week after the semester started\n
             -- tuple: two str, including the start and the end\n
```

### Comparing `hust_login-1.0.4/hust_login/decaptcha.py` & `hust_login-1.0.6/hust_login/decaptcha.py`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.4/hust_login/ecard_bills.py` & `hust_login-1.0.6/hust_login/ecard_bills.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     current_page = '1'
     next_page_obt = '1'
     ret = []
     while(next_page_obt != '0'):
         current_page = next_page_obt
         url = '{}?account={}&curpage={}&dateStatus={}&typeStatus=2'.format(url_base,account,current_page,_QueryMonth)    
         resp = session.get(url).text
-        print(resp.strip().strip('callJson(').strip(')'))
         raw = json.loads(resp.strip().strip('callJson(').strip(')'))
         next_page_obt = str(raw['nextpage'])
         entrys = raw['consume']
         ret.extend(entrys)
     selected_col = {
         'name'    :'mercname',
         'money'   :'tranamt',
@@ -108,55 +107,55 @@
                 -- list : a list, each item in the same form\n
                 -- tuple: two str, including the start and the end\n
     \n
     RETURN:\n
     {'RoomName': 'XXX', 'RemainPower': 'XXX', 'DayCost': [{'daycost': 'XXX', 'date': 'YYYY-MM-DD', 'money': 'XXX'}]}
     '''
     if not CheckLoginStatu(session):
-        raise ConnectionRefusedError('HUSTPASS: YOU HAVENT LOGGED IN')
+        raise ConnectionRefusedError('HUSTPASS: YOU HAVEN`T LOGGED IN')
     
     # 抓取校园卡账户
     resp = session.get('http://ecard.m.hust.edu.cn/wechat-web/QueryController/Queryurl.html')
     account = re.search('<input id="account" type="hidden" value="(.*)"/>',resp.text).group(1)
 
     if isinstance(_QueryDate, list):
         _QueryDate = [datetime.strptime(query_date.replace('/','-'),'%Y-%m-%d').date().isoformat() for query_date in _QueryDate] # 格式化
         month_list = set([datetime.fromisoformat(query_date).date().replace(day=1).isoformat() for query_date in _QueryDate]) # 收集需要查询的月份
         ret = []
         for _QueryMonth in month_list:
             ret.extend([entry
                 for entry in _GetMonth(session,account,_QueryMonth)
-                if entry['occtime'][:10] in _QueryDate])
+                if entry['time'][:10] in _QueryDate])
 
     elif isinstance(_QueryDate, tuple):
         _QueryDate = ( # 格式化日期区间
             datetime.strptime(_QueryDate[0].replace('/','-'), '%Y-%m-%d').date().isoformat(),
             datetime.strptime(_QueryDate[1].replace('/','-'), '%Y-%m-%d').date().isoformat()
         )
         ret = []
         month_list = get_yyyy_mm_between_dates(_QueryDate)
         for _QueryMonth in month_list:
             if _QueryMonth is month_list[0] or _QueryMonth is month_list[-1]:
                 ret.extend([entry  # 头尾月份检测是否在日期区间内
                            for entry in _GetMonth(session,account,_QueryMonth)
-                           if is_inbetween_2_dates(entry['occtime'][:10],_QueryDate)])
+                           if is_inbetween_2_dates(entry['time'][:10],_QueryDate)])
             else:
                 ret.extend(_GetMonth(session,account,_QueryMonth))
 
     elif isinstance(_QueryDate, str):
         _QueryDate.replace('/','-')
         # Month
         if _QueryDate.count('-') == 1: 
             _QueryDate = datetime.strptime(_QueryDate, '%Y-%m').date().isoformat() # 格式化月份
             return _GetMonth(session,account,_QueryDate) # 直接返回当月数据
         # Date
         elif _QueryDate.count('-') == 2:
             _QueryDate = datetime.strptime(_QueryDate, '%Y-%m-%d').date().isoformat() # 格式化日期
             return [entry 
                     for entry in _GetMonth(session,account,_QueryDate) 
-                    if entry['occtime'][:10] == _QueryDate] # 检测是否为所需日期
+                    if entry['time'][:10] == _QueryDate] # 检测是否为所需日期
         else:
             raise TypeError('HUSTPASS: UNSUPPORT TYPE')
     else:
         raise TypeError('HUSTPASS: UNSUPPORT TYPE')
 
     return ret
```

### Comparing `hust_login-1.0.4/hust_login/free_room.py` & `hust_login-1.0.6/hust_login/free_room.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import requests
 import json
-# from .login import CheckLoginStatu
-import re
-from datetime import datetime, timedelta
+from datetime import datetime
 
-def GetFreeRoom(session:requests.Session, _date_query:str) -> dict:
+def GetFreeRooms(session:requests.Session, _date_query:str) -> dict:
     '''
     PARAMETERS:\n
     session -- should be already logged in\n
     date    -- str  : the day you want, in form of YYYY-MM-DD\n
     \n
     RETURN:\n
     {'Date':'YYYY-MM-DD','Buildings':['东九楼A':{'No':'1','Roomlist': ['A101','A102']}]}
```

### Comparing `hust_login-1.0.4/hust_login/login.py` & `hust_login-1.0.6/hust_login/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         "https://pass.hust.edu.cn/cas/login",
         data=post_params,
         allow_redirects=False
     )
     try:
         resp.headers['Location']
     except:
-        raise Exception("---HustPass Failed---")
+        raise ConnectionRefusedError("---HustPass Failed---")
     log.info("---HustPass Succeed---")
     log.debug('Thank you for using hust_login')
     return r
 
 def CheckLoginStatu(session:requests.Session) -> bool:
     '''
     Check login statu\n
```

### Comparing `hust_login-1.0.4/hust_login/utility_bills.py` & `hust_login-1.0.6/hust_login/utility_bills.py`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.4/hust_login.egg-info/PKG-INFO` & `hust_login-1.0.6/hust_login.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hust-login
-Version: 1.0.4
+Version: 1.0.6
 Summary: A python-lib for authenticating HustPass@2023
 Home-page: https://github.com/MarvinTerry/HustLogin
 Author: MarvinTerry
 Author-email: marvinterry2004@gmail.com
 Maintainer: Jackhr
 Maintainer-email: jj2460596@gmail.com
 License: MIT
```

### Comparing `hust_login-1.0.4/hust_login.egg-info/SOURCES.txt` & `hust_login-1.0.6/hust_login.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
 README_ZH.md
 requirements.txt
 setup.py
+test.json
 test_basic.py
 .github/workflows/auto-test.yml
 .github/workflows/ci.yml
 hust_login/_HustPass.py
 hust_login/__init__.py
 hust_login/__main__.py
 hust_login/autotest.py
 hust_login/curriculum.py
 hust_login/decaptcha.py
 hust_login/ecard_bills.py
+hust_login/example.json
 hust_login/free_room.py
 hust_login/login.py
 hust_login/utility_bills.py
 hust_login.egg-info/PKG-INFO
 hust_login.egg-info/SOURCES.txt
 hust_login.egg-info/dependency_links.txt
 hust_login.egg-info/requires.txt
```

### Comparing `hust_login-1.0.4/images/captcha_code.gif` & `hust_login-1.0.6/images/captcha_code.gif`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.4/setup.py` & `hust_login-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.4/test_basic.py` & `hust_login-1.0.6/test_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # secret.txt 被ignore了
 with open('secret.txt', 'r') as f:
     Uname,Upass = f.read().split('\n')
 
 
 with HustPass(Uname, Upass) as s:
     with open('curriculum.json','w', encoding='utf-8') as f:
-        f.write(json.dumps(s.QueryCurriculum(('2023-04-03','2023-04-10')), ensure_ascii=False))
+        f.write(json.dumps(s.QuerySchedules(('2023-04-03','2023-04-10')), ensure_ascii=False))
     with open('ecard_bill.json','w', encoding='utf-8') as f:
         f.write(json.dumps(s.QueryEcardBills('2023-04'), ensure_ascii=False))
     with open('free_room.json','w', encoding='utf-8') as f:
-        f.write(json.dumps(s.QueryFreeRoom('2023-04-03'), ensure_ascii=False))
+        f.write(json.dumps(s.QueryFreeRooms('2023-04-03'), ensure_ascii=False))
     with open('electricity_bill.json','w', encoding='utf-8') as f:
         f.write(json.dumps(s.QueryElectricityBills(('2023-04-03','2023-04-10')), ensure_ascii=False))
```

