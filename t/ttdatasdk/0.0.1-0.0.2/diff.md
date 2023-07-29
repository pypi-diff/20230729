# Comparing `tmp/ttdatasdk-0.0.1.tar.gz` & `tmp/ttdatasdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttdatasdk-0.0.1.tar", last modified: Sun Jun 11 16:16:52 2023, max compression
+gzip compressed data, was "ttdatasdk-0.0.2.tar", last modified: Sat Jul 29 03:09:11 2023, max compression
```

## Comparing `ttdatasdk-0.0.1.tar` & `ttdatasdk-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 16:16:52.875157 ttdatasdk-0.0.1/
--rw-rw-rw-   0        0        0    11558 2023-04-30 09:03:54.000000 ttdatasdk-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2901 2023-06-11 16:16:52.875157 ttdatasdk-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2178 2023-06-11 16:08:39.000000 ttdatasdk-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-11 16:16:52.876157 ttdatasdk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2027 2023-06-11 16:15:51.000000 ttdatasdk-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 16:16:52.865157 ttdatasdk-0.0.1/tests/
--rw-rw-rw-   0        0        0     2086 2023-06-11 16:07:43.000000 ttdatasdk-0.0.1/tests/test_thrift_client.py
-drwxrwxrwx   0        0        0        0 2023-06-11 16:16:52.870158 ttdatasdk-0.0.1/ttdatasdk/
--rw-rw-rw-   0        0        0     1128 2023-06-11 11:01:50.000000 ttdatasdk-0.0.1/ttdatasdk/__init__.py
--rw-rw-rw-   0        0        0     5307 2023-06-11 12:06:43.000000 ttdatasdk-0.0.1/ttdatasdk/api.py
--rw-rw-rw-   0        0        0     9944 2023-06-11 11:04:06.000000 ttdatasdk-0.0.1/ttdatasdk/client.py
-drwxrwxrwx   0        0        0        0 2023-06-11 16:16:52.875157 ttdatasdk-0.0.1/ttdatasdk/compat/
--rw-rw-rw-   0        0        0        0 2023-04-01 02:23:36.000000 ttdatasdk-0.0.1/ttdatasdk/compat/__init__.py
--rw-rw-rw-   0        0        0     2187 2023-04-01 02:23:36.000000 ttdatasdk-0.0.1/ttdatasdk/compat/pickle_compat.py
--rw-rw-rw-   0        0        0      175 2023-04-01 02:23:36.000000 ttdatasdk-0.0.1/ttdatasdk/exceptions.py
--rw-rw-rw-   0        0        0      793 2023-05-03 04:32:31.000000 ttdatasdk-0.0.1/ttdatasdk/thrift_client.py
--rw-rw-rw-   0        0        0      587 2023-05-02 09:47:34.000000 ttdatasdk-0.0.1/ttdatasdk/utils.py
--rw-rw-rw-   0        0        0      437 2023-04-30 15:58:01.000000 ttdatasdk-0.0.1/ttdatasdk/version.py
-drwxrwxrwx   0        0        0        0 2023-06-11 16:16:52.873157 ttdatasdk-0.0.1/ttdatasdk.egg-info/
--rw-rw-rw-   0        0        0     2901 2023-06-11 16:16:52.000000 ttdatasdk-0.0.1/ttdatasdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-06-11 16:16:52.000000 ttdatasdk-0.0.1/ttdatasdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 16:16:52.000000 ttdatasdk-0.0.1/ttdatasdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-11 16:16:52.000000 ttdatasdk-0.0.1/ttdatasdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      118 2023-06-11 16:16:52.000000 ttdatasdk-0.0.1/ttdatasdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-11 16:16:52.000000 ttdatasdk-0.0.1/ttdatasdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 03:09:11.709060 ttdatasdk-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3389 2023-07-29 03:09:11.709060 ttdatasdk-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2650 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-29 03:09:11.709060 ttdatasdk-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2004 2023-07-29 03:08:45.000000 ttdatasdk-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 03:09:11.695061 ttdatasdk-0.0.2/tests/
+-rw-rw-rw-   0        0        0      573 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/tests/test_requirements.py
+-rw-rw-rw-   0        0        0     2086 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/tests/test_thrift_client.py
+-rw-rw-rw-   0        0        0     1820 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/tests/test_ttdatasdk.py
+drwxrwxrwx   0        0        0        0 2023-07-29 03:09:11.699060 ttdatasdk-0.0.2/ttdatasdk/
+-rw-rw-rw-   0        0        0     1128 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/ttdatasdk/__init__.py
+-rw-rw-rw-   0        0        0     5390 2023-07-29 01:45:45.000000 ttdatasdk-0.0.2/ttdatasdk/api.py
+-rw-rw-rw-   0        0        0     9944 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/ttdatasdk/client.py
+drwxrwxrwx   0        0        0        0 2023-07-29 03:09:11.708060 ttdatasdk-0.0.2/ttdatasdk/compat/
+-rw-rw-rw-   0        0        0        0 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/ttdatasdk/compat/__init__.py
+-rw-rw-rw-   0        0        0     2187 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/ttdatasdk/compat/pickle_compat.py
+-rw-rw-rw-   0        0        0      175 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/ttdatasdk/exceptions.py
+-rw-rw-rw-   0        0        0      793 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/ttdatasdk/thrift_client.py
+-rw-rw-rw-   0        0        0      587 2023-07-09 16:17:28.000000 ttdatasdk-0.0.2/ttdatasdk/utils.py
+-rw-rw-rw-   0        0        0      437 2023-07-29 03:08:45.000000 ttdatasdk-0.0.2/ttdatasdk/version.py
+drwxrwxrwx   0        0        0        0 2023-07-29 03:09:11.707061 ttdatasdk-0.0.2/ttdatasdk.egg-info/
+-rw-rw-rw-   0        0        0     3389 2023-07-29 03:09:11.000000 ttdatasdk-0.0.2/ttdatasdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2023-07-29 03:09:11.000000 ttdatasdk-0.0.2/ttdatasdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 03:09:11.000000 ttdatasdk-0.0.2/ttdatasdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 03:09:11.000000 ttdatasdk-0.0.2/ttdatasdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      118 2023-07-29 03:09:11.000000 ttdatasdk-0.0.2/ttdatasdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 03:09:11.000000 ttdatasdk-0.0.2/ttdatasdk.egg-info/top_level.txt
```

### Comparing `ttdatasdk-0.0.1/LICENSE` & `ttdatasdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ttdatasdk-0.0.1/PKG-INFO` & `ttdatasdk-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttdatasdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Ticker Trading Factors data access, Backtest and Trading.
 Home-page: https://www.tickertrading.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 License: Apache License v2
@@ -21,21 +21,37 @@
 # ttdatasdk
 
 #### 介绍
 Ticker Trading Factors data access, Backtest and Trading.
 
 ### 安装方法
 ```shell
-# 首次安装
-pip install ttdatasdk
+# 首次安装, 在项目的根目录下添加requirements.txt文件，增加内容如下：
+Cython==0.29.34
+ply==3.11
+msgpack>=0.4.7
+pandas==1.4.4
+setuptools==66.0.0
+six==1.16.0
+thriftpy2==0.4.16
+wheel==0.38.4
+ttdatasdk==0.0.1
+
+# 在命令行执行：
+pip install -r requirements.txt
+# 如果安装失败，请指定官方镜像源
+pip install -r requirements.txt -i https://pypi.org/simple
 
 # 升级版本
 pip install -U ttdatasdk
+# 如果安装失败，请指定官方镜像源
+pip install -U ttdatasdk -i https://pypi.org/simple
 ```
 
+
 ### 使用方法
 ```python
 import ttdatasdk
 
 """账号认证"""
 ttdatasdk.auth(username, password)
```

### Comparing `ttdatasdk-0.0.1/README.md` & `ttdatasdk-0.0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 # ttdatasdk
 
 #### 介绍
 Ticker Trading Factors data access, Backtest and Trading.
 
 ### 安装方法
 ```shell
-# 首次安装
-pip install ttdatasdk
+# 首次安装, 在项目的根目录下添加requirements.txt文件，增加内容如下：
+Cython==0.29.34
+ply==3.11
+msgpack>=0.4.7
+pandas==1.4.4
+setuptools==66.0.0
+six==1.16.0
+thriftpy2==0.4.16
+wheel==0.38.4
+ttdatasdk==0.0.1
+
+# 在命令行执行：
+pip install -r requirements.txt
+# 如果安装失败，请指定官方镜像源
+pip install -r requirements.txt -i https://pypi.org/simple
 
 # 升级版本
 pip install -U ttdatasdk
+# 如果安装失败，请指定官方镜像源
+pip install -U ttdatasdk -i https://pypi.org/simple
 ```
 
+
 ### 使用方法
 ```python
 import ttdatasdk
 
 """账号认证"""
 ttdatasdk.auth(username, password)
```

### Comparing `ttdatasdk-0.0.1/setup.py` & `ttdatasdk-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,33 +8,33 @@
 
 
 THIS_FOLDER = os.path.dirname(os.path.abspath(__file__))
 
 
 def get_version():
     scope = {}
-    version = '0.0.1'
+    version = '0.0.2'
     version_file = os.path.join(THIS_FOLDER, "ttdatasdk", "version.py")
     if os.path.exists(version_file):
         with open(version_file) as fp:
             exec(fp.read(), scope)
-        version = scope.get('__version__', '0.0.1')
+        version = scope.get('__version__', '0.0.2')
     return version
 
 
 def get_long_description():
     with open(os.path.join(THIS_FOLDER, 'README.md'), 'rb') as f:
         long_description = f.read().decode('utf-8')
     return long_description
 
 
 def _parse_requirement_file(path):
     if not os.path.isfile(path):
         return []
-    with open(path, 'r', encoding='utf-8') as f:
+    with open(path) as f:
         requirements = [line.strip() for line in f if line.strip()]
     return requirements
 
 
 def get_install_requires():
     requirement_file = os.path.join(THIS_FOLDER, "requirements.txt")
     return _parse_requirement_file(requirement_file)
```

### Comparing `ttdatasdk-0.0.1/tests/test_thrift_client.py` & `ttdatasdk-0.0.2/tests/test_thrift_client.py`

 * *Files identical despite different names*

### Comparing `ttdatasdk-0.0.1/ttdatasdk/__init__.py` & `ttdatasdk-0.0.2/ttdatasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ttdatasdk-0.0.1/ttdatasdk/api.py` & `ttdatasdk-0.0.2/ttdatasdk/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
 from .client import TTDataClient
 from .utils import *
 
 
 @assert_auth
 def get_factor(sec_code_list: list = None,
-               factor_list: list = ...,
+               factor_list=None,
                factor_group_list: list = None,
                trade_date: str = None,
                start_date: str = None,
                end_date: str = None,
                start_datetime: str = None,
                end_datetime: str = None,
                stock_pool: list = None,
@@ -37,41 +37,43 @@
                 'back'
                 : 后复权
     :param unit: 单位时间长度，支持1d、1m，默认为1d
     :param expect_df: 是否以DataFrame返回
     :param count: 数量, 返回的结果集的行数
     :return:
     """
+    if factor_list is None:
+        factor_list = ['close']
     return TTDataClient.instance().get_factor(**locals())
 
 
 @assert_auth
 def get_history(count: int,
                 unit: str = '1d',
                 start_date: str = None,
                 end_date: str = None,
                 start_datetime: str = None,
                 end_datetime: str = None,
                 field: str = 'close',
                 security_list=None,
-                df=True,
+                expect_df=True,
                 skip_paused=False,
                 dividend_type='front'):
     """
     获取历史数据，可查询多个标的单个数据字段，返回数据格式为 DataFrame 或 Dict(字典)
 
     :param start_date:
     :param end_date:
     :param count: 数量, 返回的结果集的行数
     :param unit: 单位时间长度, 几天或者几分钟, 现在支持'1d','1m'
     :param start_datetime: 当unit='1m'时有效，格式：2023-03-29 14:57:00
     :param end_datetime: 当unit='1m'时有效，格式：2023-03-29 14:57:00
     :param field: 要获取的数据字段
     :param security_list: 要获取数据的股票列表
-    :param df: df=True: [pandas.DataFrame]对象, 行索引是[datetime.datetime]对象, 列索引是股票代号
+    :param expect_df: df=True: [pandas.DataFrame]对象, 行索引是[datetime.datetime]对象, 列索引是股票代号
                df=False: dict, key是股票代码, value是一个numpy数组[numpy.ndarray]
     :param skip_paused: 是否跳过不交易日期(包括停牌, 未上市或者退市后的日期)
     :param dividend_type: 复权选项(对股票/基金的价格字段、成交量字段及factor字段生效)
                 'front'
                 : 前复权, 默认是前复权
                 none
                 : 不复权, 返回实际价格
@@ -88,29 +90,29 @@
                           unit: str = '1d',
                           start_date: str = None,
                           end_date: str = None,
                           start_datetime: str = None,
                           end_datetime: str = None,
                           fields: list = None,
                           skip_paused: bool = True,
-                          df: bool = True,
+                          expect_df: bool = True,
                           dividend_type: str = 'front'):
     """
     获取历史数据，可查询单个标的多个数据字段，返回数据格式为 DataFrame 或 Dict(字典)
 
     :param start_date:
     :param end_date:
     :param start_datetime: 当unit='1m'时有效，格式：2023-03-29 14:57:00
     :param end_datetime: 当unit='1m'时有效，格式：2023-03-29 14:57:00
     :param security: 股票代码
     :param count: 数量, 返回的结果集的行数
     :param unit: 单位时间长度, 1d, 1m
     :param fields: 股票属性的list, 支持：['open', ' high', 'low', 'close', 'volume', 'amount']
     :param skip_paused: 是否跳过不交易日期(包括停牌, 未上市或者退市后的日期).
-    :param df: 若是True, 返回[pandas.DataFrame], 否则返回一个dict, 具体请看下面的返回值介绍. 默认是True.
+    :param expect_df: 若是True, 返回[pandas.DataFrame], 否则返回一个dict, 具体请看下面的返回值介绍. 默认是True.
     :param dividend_type: 复权选项(对股票/基金的价格字段、成交量字段及factor字段生效)
                 'front'
                 : 前复权, 默认是前复权
                 none
                 : 不复权, 返回实际价格
                 'back'
                 : 后复权
```

### Comparing `ttdatasdk-0.0.1/ttdatasdk/client.py` & `ttdatasdk-0.0.2/ttdatasdk/client.py`

 * *Files identical despite different names*

### Comparing `ttdatasdk-0.0.1/ttdatasdk/compat/pickle_compat.py` & `ttdatasdk-0.0.2/ttdatasdk/compat/pickle_compat.py`

 * *Files identical despite different names*

### Comparing `ttdatasdk-0.0.1/ttdatasdk/thrift_client.py` & `ttdatasdk-0.0.2/ttdatasdk/thrift_client.py`

 * *Files identical despite different names*

### Comparing `ttdatasdk-0.0.1/ttdatasdk/utils.py` & `ttdatasdk-0.0.2/ttdatasdk/utils.py`

 * *Files identical despite different names*

### Comparing `ttdatasdk-0.0.1/ttdatasdk.egg-info/PKG-INFO` & `ttdatasdk-0.0.2/ttdatasdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttdatasdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Ticker Trading Factors data access, Backtest and Trading.
 Home-page: https://www.tickertrading.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 License: Apache License v2
@@ -21,21 +21,37 @@
 # ttdatasdk
 
 #### 介绍
 Ticker Trading Factors data access, Backtest and Trading.
 
 ### 安装方法
 ```shell
-# 首次安装
-pip install ttdatasdk
+# 首次安装, 在项目的根目录下添加requirements.txt文件，增加内容如下：
+Cython==0.29.34
+ply==3.11
+msgpack>=0.4.7
+pandas==1.4.4
+setuptools==66.0.0
+six==1.16.0
+thriftpy2==0.4.16
+wheel==0.38.4
+ttdatasdk==0.0.1
+
+# 在命令行执行：
+pip install -r requirements.txt
+# 如果安装失败，请指定官方镜像源
+pip install -r requirements.txt -i https://pypi.org/simple
 
 # 升级版本
 pip install -U ttdatasdk
+# 如果安装失败，请指定官方镜像源
+pip install -U ttdatasdk -i https://pypi.org/simple
 ```
 
+
 ### 使用方法
 ```python
 import ttdatasdk
 
 """账号认证"""
 ttdatasdk.auth(username, password)
```

