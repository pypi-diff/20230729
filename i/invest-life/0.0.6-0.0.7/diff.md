# Comparing `tmp/invest_life-0.0.6.tar.gz` & `tmp/invest_life-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invest_life-0.0.6.tar", last modified: Sat Jul 29 01:34:42 2023, max compression
+gzip compressed data, was "invest_life-0.0.7.tar", last modified: Sat Jul 29 10:23:26 2023, max compression
```

## Comparing `invest_life-0.0.6.tar` & `invest_life-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 01:34:42.604053 invest_life-0.0.6/
--rw-r--r--   0 mac        (501) staff       (20)     1073 2023-07-25 13:12:51.000000 invest_life-0.0.6/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-29 01:34:42.603713 invest_life-0.0.6/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      159 2023-07-25 13:12:33.000000 invest_life-0.0.6/README.md
--rw-r--r--   0 mac        (501) staff       (20)      459 2023-07-29 01:34:17.000000 invest_life-0.0.6/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-29 01:34:42.604158 invest_life-0.0.6/setup.cfg
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 01:34:42.597116 invest_life-0.0.6/src/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-07-25 13:00:59.000000 invest_life-0.0.6/src/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 01:34:42.601979 invest_life-0.0.6/src/invest_life.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-29 01:34:42.000000 invest_life-0.0.6/src/invest_life.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      236 2023-07-29 01:34:42.000000 invest_life-0.0.6/src/invest_life.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-29 01:34:42.000000 invest_life-0.0.6/src/invest_life.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       20 2023-07-29 01:34:42.000000 invest_life-0.0.6/src/invest_life.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)   221415 2023-07-27 09:37:40.000000 invest_life-0.0.6/src/investlife.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 01:34:42.602543 invest_life-0.0.6/tests/
--rw-r--r--   0 mac        (501) staff       (20)       24 2023-07-25 14:03:29.000000 invest_life-0.0.6/tests/test.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 10:23:26.002012 invest_life-0.0.7/
+-rw-r--r--   0 mac        (501) staff       (20)     1073 2023-07-25 13:12:51.000000 invest_life-0.0.7/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-29 10:23:26.001517 invest_life-0.0.7/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      159 2023-07-25 13:12:33.000000 invest_life-0.0.7/README.md
+-rw-r--r--   0 mac        (501) staff       (20)      459 2023-07-29 10:21:11.000000 invest_life-0.0.7/pyproject.toml
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-29 10:23:26.002178 invest_life-0.0.7/setup.cfg
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 10:23:25.997624 invest_life-0.0.7/src/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-07-25 13:00:59.000000 invest_life-0.0.7/src/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 10:23:26.000258 invest_life-0.0.7/src/invest_life.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-29 10:23:25.000000 invest_life-0.0.7/src/invest_life.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      236 2023-07-29 10:23:25.000000 invest_life-0.0.7/src/invest_life.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-29 10:23:25.000000 invest_life-0.0.7/src/invest_life.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       20 2023-07-29 10:23:25.000000 invest_life-0.0.7/src/invest_life.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)   217235 2023-07-29 10:11:35.000000 invest_life-0.0.7/src/investlife.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 10:23:26.000809 invest_life-0.0.7/tests/
+-rw-r--r--   0 mac        (501) staff       (20)      173 2023-07-29 10:06:58.000000 invest_life-0.0.7/tests/test.py
```

### Comparing `invest_life-0.0.6/LICENSE` & `invest_life-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `invest_life-0.0.6/PKG-INFO` & `invest_life-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest_life
-Version: 0.0.6
+Version: 0.0.7
 Summary: a package from investor
 Author-email: kelvin <wwwhhitzxt@163.com>
 Project-URL: Homepage, https://investlife.cn/
 Project-URL: Bug Tracker, https://investlife.cn/info/author.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `invest_life-0.0.6/src/invest_life.egg-info/PKG-INFO` & `invest_life-0.0.7/src/invest_life.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest-life
-Version: 0.0.6
+Version: 0.0.7
 Summary: a package from investor
 Author-email: kelvin <wwwhhitzxt@163.com>
 Project-URL: Homepage, https://investlife.cn/
 Project-URL: Bug Tracker, https://investlife.cn/info/author.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `invest_life-0.0.6/src/investlife.py` & `invest_life-0.0.7/src/investlife.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 g_token = None
 
 # 设置token
 def set_token(token = None):
     global g_token
     g_token = token
 
+# 设置headers
+def get_headers():
+    return {'Content-Type': 'application/json', 'token': g_token, 'appsource': 'python'}
+
 def get_stock_list(listed_state = None, fields = None):
     """
     记录A股上市、退市股票交易代码、股票名称、上市状态等信息；
 
     输入参数：
     :param str listed_state : 上市状态
     :param str fields : 字段集合
@@ -34,15 +38,15 @@
     结果输出:
          secu_abbr chi_name  listed_state \
 0 平安银行 平安银行股份有限公司 上市
 1 万科Ａ 万科企业股份有限公司 上市
 …
     """
         
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_list'
     param = {'listed_state': listed_state, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
         return pickle.loads(res.content)
@@ -72,15 +76,15 @@
     结果输出:
          if_trading_day if_week_end  if_month_end \
 0 是 否 否
 1 是 否 否
 ...
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_trading_calendar'
 
     param = {'secu_market': secu_market, 'if_trading_day': if_trading_day, 'if_week_end': if_week_end, 'if_month_end': if_month_end, 'start_date': start_date, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -129,15 +133,15 @@
     :param float allot_min : 申购下限,
     :param float esti_issue_price : 预估发行价,
     :param float naps_after : 每股净资产(元),
     :param int issue_system_type : 发行制度类型,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_ipo_list'
 
     param = {'start_date': start_date, 'secu_market': secu_market, 'listed_sector': listed_sector, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -174,15 +178,15 @@
     :param str fax : 传真,
     :param str uniform_social_credit_code : 统一社会信用代码,
     :param int employee_sum : 员工总数,
     :param str controller_name : 实际控制人,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_company_profile'
 
     param = {'en_prod_code': en_prod_code, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -217,15 +221,15 @@
     :param str change_type : 证券存续状态,
     :param int sh_hk_flag : 是否沪港通标的,
     :param int sz_hk_flag : 是否深港通标的,
     :param str en_prod_code : 股票代码,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_Info'
 
     param = {'en_prod_code': en_prod_code, 'trading_date': trading_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -255,15 +259,15 @@
     :param str newest_hold : 最新持股数,
     :param str shareholding_ratio : 持股比例,
     :param str end_date : 年度报酬报告期,
     :param int annual_reward : 年度报酬,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_leader_profile'
 
     param = {'secu_code': secu_code, 'position_type': position_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -287,15 +291,15 @@
     :param str chi_name : 公司名称,
     :param str secu_market : 证券市场,
     :param str secu_category : 证券类型,
     :param str listed_sector : 上市板块,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_st_stock_list'
 
     param = {'secu_market': secu_market, 'secu_category': secu_category, 'listed_sector': listed_sector, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -317,15 +321,15 @@
     :param str secu_abbr : 证券简称,
     :param str secu_category : 证券类别,
     :param str secu_market : 证券市场,
     :param str select_time : 入选股票时间,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_shszhk_stock_list'
 
     param = {'etfcomponent_type': etfcomponent_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -364,15 +368,15 @@
     :param float ratio_adjust_factor : 复权因子,
     :param float business_amount : 成交数量,
     :param str up_down_status : 涨跌停状态,
     :param str turnover_status : 交易状态,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_quote_daily'
 
     param = {'en_prod_code': en_prod_code, 'trading_date': trading_date, 'adjust_way': adjust_way, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -413,15 +417,15 @@
     :param str week_high_price_date : 周最高价日,
     :param str week_low_price_date : 周最低价日,
     :param str week_max_close_price_date : 周最高收盘价日,
     :param str week_min_close_price_date : 周最低收盘价日,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_quote_weekly'
 
     param = {'en_prod_code': en_prod_code, 'trading_date': trading_date, 'adjust_way': adjust_way, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -462,15 +466,15 @@
     :param str month_high_price_date : 月最高价日,
     :param str month_low_price_date : 月最低价日,
     :param str month_max_close_price_date : 月最高收盘价日,
     :param str month_min_close_price_date : 月最低收盘价日,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_quote_monthly'
 
     param = {'en_prod_code': en_prod_code, 'trading_date': trading_date, 'adjust_way': adjust_way, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -511,15 +515,15 @@
     :param str year_high_price_date : 年最高价日,
     :param str year_low_price_date : 年最低价日,
     :param str year_max_close_price_date : 年最高收盘价日,
     :param str year_min_close_price_date : 年最低收盘价日,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_quote_yearly'
 
     param = {'en_prod_code': en_prod_code, 'trading_date': trading_date, 'adjust_way': adjust_way, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -560,15 +564,15 @@
     :param float medium_out : 中单流出,
     :param float medium_amount_out : 主动卖出中单成交量,
     :param float little_out : 小单流出,
     :param float little_amount_out : 主动卖出小单成交量,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_money_flow'
 
     param = {'en_prod_code': en_prod_code, 'trading_date': trading_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -591,15 +595,15 @@
     :param str suspend_time : 停牌时间,
     :param str resumption_date : 复牌日期,
     :param str resumption_time : 复牌时间,
     :param str suspend_reason : 停牌原因,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_suspension_list'
 
     param = {'en_prod_code': en_prod_code, 'trading_date': trading_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -634,15 +638,15 @@
     :param float total_rate : 占总股本比例(%),
     :param float hold_vol_change : 较上期持股变动股数(万股),
     :param float total_rate_change : 较上期变动比例(%),
     :param float aas_change_type : 变动类别,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_shareholder_top10'
 
     param = {'secu_code': secu_code, 'start_date': start_date, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -677,15 +681,15 @@
     :param float float_rate : 占总流通股比例(%),
     :param float hold_vol_change : 较上期持股变动股数(万股),
     :param float total_rate_change : 较上期变动比例(%),
     :param float aas_change_type : 变动类别,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_float_shareholder_top10'
 
     param = {'secu_code': secu_code, 'start_date': start_date, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -712,15 +716,15 @@
     :param float secu_code : 证券代码,
     :param float trading_day : 交易日期,
     :param float net_balance : 净买入额(元),
     :param float mark : 标签,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_lh_daily'
 
     param = {'trading_day': trading_day, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -756,15 +760,15 @@
     :param float sale_rate : 卖出金额占总金额比,
     :param float sale_balance : 卖出金额,
     :param str sales_department_name : 营业部简称,
     :param str list_date : 近十次上榜日期,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_lh_stock'
 
     param = {'secu_code': secu_code, 'trading_day': trading_day, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -792,15 +796,15 @@
     :param float turnover_volume : 成交量,
     :param float turnover_value : 成交额,
     :param float change : 涨跌幅(元),
     :param float change_pct : 涨跌幅(%),
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_quote_minutes'
 
     param = {'en_prod_code': en_prod_code, 'begin_date': begin_date, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -899,15 +903,15 @@
 
     Notes
     -----
     无论股票、可转债、期货还是基金。第一列表头始终叫 ``股票代码``
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_quote_realtime'
 
     param = {}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -937,15 +941,15 @@
     :param str led_stock_name : 领涨股名称,
     :param str secu_market : 证券市场,
     :param float led_stock_chg : 领涨股涨跌幅(%),
     :param float currency : 货币单位,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_shszhk_capitalflow'
 
     param = {'exchange_kind': exchange_kind, 'start_date': start_date, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -974,15 +978,15 @@
     :param float currency : 货币单位,
     :param float close_price : 收盘价,
     :param float px_change_rate : 涨跌幅,
     :param float business_balance : 成交金额,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_shszhk_deal_top10'
 
     param = {'exchange_kind': exchange_kind, 'start_date': start_date, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1004,15 +1008,15 @@
     :param str trade_date : 交易日期,
     :param float up_count : 上涨个数,
     :param float flat_count : 平盘家数,
     :param float down_count : 下跌个数,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_shszhk_distribution'
 
     param = {'exchange_kind': exchange_kind, 'start_date': start_date, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1042,15 +1046,15 @@
     :param float total_mv : A股总市值,
     :param float pe_lyr : 市盈率,
     :param float float_value : A股流通市值(元),
     :param float pe_ttm : 滚动市盈率,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_shszhk_change_top10'
 
     param = {'exchange_kind': exchange_kind, 'trading_data': trading_data, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1068,15 +1072,15 @@
     输出参数：
     :param str prod_code : 证券代码(带后缀),
     :param str secu_code : 证券代码(不带后缀),
     :param str secu_abbr : 证券简称,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_quote_stocklist'
 
     param = {'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1108,15 +1112,15 @@
     :param float business_balance : 成交金额(元),
     :param float turnover_volume : 成交量(股),
     :param float issue_price_change : 距首发价涨幅,
     :param float issue_price_change_rate : 距首发价涨跌幅,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_quote_daily_list'
 
     param = {'en_prod_code': en_prod_code, 'begin_date': begin_date, 'end_date': end_date, 'adjust_way': adjust_way}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1134,15 +1138,15 @@
     输出参数：
     :param str en_prod_code : 证劵代码,
     :param str trading_date : 交易日期,
     :param float close_price : 收盘价,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_index_quote'
 
     param = {'en_prod_code': en_prod_code, 'trading_date': trading_date}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1169,15 +1173,15 @@
     :param str industry_name_sw : 申万行业名称,
     :param str industry_code_sw : 申万行业代码,
     :param str industry_name_citic : 中信行业名称,
     :param str industry_code_citic : 中信行业代码,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_industry_category'
 
     param = {'en_prod_code': en_prod_code, 'level': level, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1200,15 +1204,15 @@
     :param str secu_abbr : 证券简称,
     :param str secu_market : 成份股市场,
     :param str secu_category : 证券类别,
     :param str in_date : 入选日期,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_index_constituent'
 
     param = {'index_stock_code': index_stock_code, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1239,15 +1243,15 @@
     :param str hold_a_sum_up : 加仓数量(万股),
     :param str hold_a_sum_up_rate : 加仓比例(%),
     :param str hold_a_sum_up_type : 加仓类型,
     :param float market_value : 市值(万元),
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_org_hold'
 
     param = {'secu_code': secu_code, 'org_type': org_type, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1274,15 +1278,15 @@
     :param float avg_hold_sum_gr_quarter : 户均持股数季度增长率,
     :param float proportion_gr_quarter : 户均持股比例季度增长率,
     :param float avg_hold_sum_gr_half_a_year : 户均持股数年增长率,
     :param float proportion_gr_half_a_year : 户均持股比例年增长率,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_holder_num'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1308,15 +1312,15 @@
     :param float new_circulation_a_shares_rate : 新增流通A股占已流通A股比例,
     :param float accu_circulation_a_shares : 已流通A股数量,
     :param float non_circulation_a_shares : 未流通A股数量,
     :param str new_circulation_a_shares_type : 新增流通A股类型,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_restricted_schedule'
 
     param = {'en_prod_code': en_prod_code, 'trading_date': trading_date, 'query_direction': query_direction, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1341,15 +1345,15 @@
     :param float pledge_involved_sum : 质押涉及股数,
     :param float pct_of_frozen_pledger : 占冻结质押方持股数比例,
     :param float pct_of_total_shares : 占总股本比例,
     :param str publ_date : 股权质押公告日期,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_holder_pledge'
 
     param = {'en_prod_code': en_prod_code, 'trading_date': trading_date, 'serial_number': serial_number, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1391,15 +1395,15 @@
     :param str tran_date : 股权正式变动日期/过户日期（变动截止日）,
     :param str holder_type : 股东类别,
     :param str relation_description : 与领导人关系,
     :param float involved_chan_vol : 变动后持股数量(股),
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_holder_increase'
 
     param = {'date_type': date_type, 'symbols': symbols, 'listed_sector': listed_sector, 'secu_market': secu_market, 'share_holder_type': share_holder_type, 'state_type': state_type, 'start_date': start_date, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1425,15 +1429,15 @@
     :param float non_pled_volume : 无限售股份质押数量(万股),
     :param float res_pled_volume : 有限售股份质押数量(万股),
     :param float total_share_a : A股总股本(万股),
     :param float pledge_num : 质押笔数,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_pledge_repo'
 
     param = {'secu_code': secu_code, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1457,15 +1461,15 @@
     :param str secu_market : 证券市场,
     :param str info_publ_date : 公告日期,
     :param float involved_sum_br_count : 涉及股数_前复权汇总,
     :param float proportion_totalshares : 占总股本比例,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_pledge'
 
     param = {'secu_code': secu_code, 'start_date': start_date, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1496,15 +1500,15 @@
     :param float trade_price : 成交价单位元/股,
     :param float involved_vol : 成交量单位万/股,
     :param str receiver_name : 买方营业部,
     :param str transferer_name : 卖方营业部,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_block_trade'
 
     param = {'secu_code': secu_code, 'start_date': start_date, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1534,15 +1538,15 @@
     :param float security_sell_amount : 融券卖出量,
     :param float security_refund_amount : 融券偿还量,
     :param float security_amount : 融券余量,
     :param float finance_security_balance : 融资融券余额,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_margin_trading'
 
     param = {'en_prod_code': en_prod_code, 'trading_date': trading_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1574,15 +1578,15 @@
     :param float inter_security_refund_balance : 区间融券偿还额,
     :param float inter_avg_security_amount : 区间融券余量均值,
     :param float inter_avg_security_balance : 区间融券余额均值,
     :param float avg_finance_security_balance : 区间融资融券余额均值,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_interval_margin_trading'
 
     param = {'en_prod_code': en_prod_code, 'begin_date': begin_date, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1618,15 +1622,15 @@
     :param float finance_buy_balance : 融资买入额（元）,
     :param float finance_net_balance : 融资净买入,
     :param float finance_refund_balance : 融资偿还额（元）,
     :param float finance_balance : 融资余额（元）,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_margin_trade_detail'
 
     param = {'symbols': symbols, 'date_type': date_type, 'start_date': start_date, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1658,15 +1662,15 @@
     :param float tol_finance_balance : 沪深融资余额,
     :param float tol_finance_buy_balance : 沪深融资买入额,
     :param float tol_security_balance : 沪深融券余额,
     :param float tol_trading_balance : 沪深融资融券余额,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_margin_trade_total'
 
     param = {'date_type': date_type, 'start_date': start_date, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1701,15 +1705,15 @@
     :param str final_trade_date : 最后交易日,
     :param str procedure_desc : 分红方案进度,
     :param str divi_object : 分红对象,
     :param str if_dividend : 是否分红,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_dividend'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1762,15 +1766,15 @@
     :param float fund_issue_vol : 投资基金配售股数,
     :param float main_income_forecast : 主营业务收入预测,
     :param float net_profit_forecast : 净利润预测,
     :param float diluted_eps_forecast : 全面摊薄每股盈利预测,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_additional'
 
     param = {'en_prod_code': en_prod_code, 'year': year, 'issue_type': issue_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1797,15 +1801,15 @@
     :param float spo_num_going : 增发进行中次数,
     :param float accu_ipo_proceeds : 增发累计募集资金总额,
     :param float accu_net_proceeds : 增发累计募集资金净额,
     :param float accu_issue_cost : 增发累计费用总额,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_additional_all'
 
     param = {'en_prod_code': en_prod_code, 'trading_date': trading_date, 'spo_process': spo_process, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1844,15 +1848,15 @@
     :param str allot_start_date : 配股交款起始日,
     :param str allot_end_date : 配股交款截止日,
     :param str fund_to_account_date : 资金到帐日,
     :param str allot_list_date : 配股上市日,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_allotment'
 
     param = {'en_prod_code': en_prod_code, 'year': year, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1883,15 +1887,15 @@
     :param str eprofit_floor : 预计净利润下限,
     :param str eprofit_ceiling : 预计净利润上限,
     :param float eearning_floor : 预计收入起始(元),
     :param float eearning_ceiling : 预计收入截止(元),
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_asforecastabb'
 
     param = {'secu_code': secu_code, 'forcast_type': forcast_type, 'forecast_object': forecast_object, 'egrowth_rate_floor': egrowth_rate_floor, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1913,15 +1917,15 @@
     :param str sh_name : 股东名称,
     :param str serial_number : 股东序号,
     :param str event_info : 事件描述,
     :param str initial_info_publ_date : 首次信息发布日期,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_asunderweight'
 
     param = {'secu_code': secu_code, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1951,15 +1955,15 @@
     :param float add_hold_ratio_ceiling : 增持比例上限-占总股本,
     :param float add_hold_share_min : 增持股份数量下限,
     :param float add_hold_ratio_min : 增持比例下限-占总股本,
     :param str add_hold_statement : 增持计划说明,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_asoverweight'
 
     param = {'secu_code': secu_code, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -1988,15 +1992,15 @@
     :param str transferer_name : 股权出让方名称,
     :param str tran_date : 过户日期,
     :param str receiver_name : 股权受让方名称,
     :param str if_snafter_tran : 是否第1大股东变更,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_asrighttransfer'
 
     param = {'secu_code': secu_code, 'year': year, 'tran_mode': tran_mode, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2021,15 +2025,15 @@
     :param str start_date : 开始日期,
     :param str date_rang : 周期,
     :param float pledge_involved_sum : 周期内累计交易股数(股),
     :param float pct_of_total_shares : 周期内累计占比,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_asraising'
 
     param = {'tran_mode': tran_mode, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2053,15 +2057,15 @@
     :param float a_shares : A股合计（股）,
     :param float non_restricted_a_shares : 其中：无限售条件的流通A股(股),
     :param float b_shares : B股合计（股）,
     :param float circulation_b_shares : 其中：流通B股（股）,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_share_holders'
 
     param = {'en_prod_code': en_prod_code, 'trading_date': trading_date, 'unit': unit, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2084,15 +2088,15 @@
     :param str secu_code : 证券代码,
     :param str secu_abbr : 证券简称,
     :param str special_trade_time : 特别处理(或撤销)实施日期,
     :param str special_trade_type : 特别处理(或撤销)类别,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_special_tradedate'
 
     param = {'secu_code': secu_code, 'start_date': start_date, 'end_date': end_date, 'special_trade_type': special_trade_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2120,15 +2124,15 @@
     :param str author : 物权作者,
     :param str conclusion : 报告结论,
     :param str rate_type_name : 评级类型名称,
     :param str rate_type : 评级类型,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_org_rate'
 
     param = {'secu_code': secu_code, 'rate_type': rate_type, 'start_date': start_date, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2153,15 +2157,15 @@
     :param str neutral_sum : 中性评级合计,
     :param str reduce_sum : 减持评级合计,
     :param str sale_sum : 卖出额,
     :param str total_sum : 评级合计,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_org_rate_sum'
 
     param = {'date_type': date_type, 'secu_code': secu_code, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2192,15 +2196,15 @@
     :param str buy_num : 买方机构数量,
     :param str sell_num : 卖方机构数量,
     :param str parly_num : 参与本次调研机构数量,
     :param str survey_date : 调研日期,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_investor_statistics'
 
     param = {'symbols': symbols, 'secu_market': secu_market, 'listed_sector': listed_sector, 'start_date': start_date, 'end_date': end_date, 'event_id': event_id, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2233,15 +2237,15 @@
     :param str listed_sector : 上市板类型,
     :param str listing_creper : 上市公司接待人员,
     :param str place : 地点,
     :param 对象 participants : 参与单位及人员集合,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_investor_detail'
 
     param = {'symbols': symbols, 'secu_market': secu_market, 'listed_sector': listed_sector, 'date_type': date_type, 'start_date': start_date, 'end_date': end_date, 'event_id': event_id, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2269,15 +2273,15 @@
     :param str third_industry_code : 三级行业代码,
     :param str third_industry_name : 三级行业名称,
     :param str fourth_industry_code : 四级行业代码,
     :param str furth_industry_name : 四级行业名称,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_financial_industry_list'
 
     param = {'secu_code': secu_code, 'standard': standard, 'first_industry_code': first_industry_code, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2307,15 +2311,15 @@
     :param float net_profit : 归属母公司股东的净利润,
     :param float profit_ps : 每股收益,
     :param float net_asset_ps : 每股净资产,
     :param float net_profit_rate : 净利润增长率,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_industry_compare'
 
     param = {'secu_code': secu_code, 'end_date': end_date, 'sort_field': sort_field, 'sort_type': sort_type, 'second_industry_code': second_industry_code, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2340,15 +2344,15 @@
     :param float industry_net_profit_avg : 行业平均归属母公司股东的净利润,
     :param float industry_profit_ps_avg : 行业平均每股收益,
     :param float industry_netasset_ps_avg : 行业平均每股净资产,
     :param float industry_net_profit_rate_avg : 净利润增长率（行业平均）,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_industry_avg'
 
     param = {'secu_code': secu_code, 'second_industry_code': second_industry_code, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2367,15 +2371,15 @@
     :param str type : 类型,
     :param str first_level_name : 一级名称,
     :param str first_level_code : 一级代码,
     :param 对象 level2_obj_list : 二级名称和代码,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_industry_region_list'
 
     param = {'type': type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2396,15 +2400,15 @@
     :param str prod_code : 证劵代码,
     :param str report_date : 申报日期,
     :param str actual_date : 定期报告实际披露日期,
     :param str plan_date : 计划执行日期,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_schedule_disclosure'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2451,15 +2455,15 @@
     :param float net_profit_yoy : 净利润同比增长率(%),
     :param float operating_revenue_grow_rate : 营业收入同比增长率(%),
     :param float debt_assets_ratio : 资产负债率(%),
     :param float pe_ttm : 市盈率(%),
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_key_indicator'
 
     param = {'secu_code': secu_code, 'start_date': start_date, 'end_date': end_date, 'report_types': report_types, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2553,15 +2557,15 @@
     :param float total_shareholder_equity : 所有者权益合计,
     :param float total_liability_and_equity : 负债和所有者权益（或股东权益）总计,
     :param float naps : 每股净资产BPS,
     :param float se_without_mi_t : 每股净资产BPS（最新股本摊薄）,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_accounting_data'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2669,15 +2673,15 @@
     :param float cash_equivalents_at_beginning : 减:现金等价物的期初余额,
     :param float cash_at_beginning_of_year : 减:现金的期初余额,
     :param float cash_equivalents_at_end_of_year : 加:现金等价物的期末余额,
     :param float cash_at_end_of_year : 现金的期末余额,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_financial_cashflow'
 
     param = {'secu_code': secu_code, 'start_date': start_date, 'end_date': end_date, 'merge_type': merge_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2758,15 +2762,15 @@
     :param float total_profit : 利润总额,
     :param float minority_profit : 少数股东损益,
     :param float net_profit : 净利润,
     :param float np_parent_company_owners : 归属于母公司所有者的净利润,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_financial_income'
 
     param = {'secu_code': secu_code, 'start_date': start_date, 'end_date': end_date, 'merge_type': merge_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2907,15 +2911,15 @@
     :param float specific_reserves : 专项储备,
     :param float se_without_mi : 归属母公司股东权益合计,
     :param float minority_interests : 少数股东权益,
     :param float total_shareholder_equity : 所有者权益合计,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_financial_balance'
 
     param = {'secu_code': secu_code, 'start_date': start_date, 'end_date': end_date, 'merge_type': merge_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -2965,15 +2969,15 @@
     :param float uncertained_investment_loss : 单季度.未确认的投资损失,
     :param float net_profit : 单季度.净利润,
     :param float np_from_parent_company_owners : 单季度.归属于母公司所有者的净利润,
     :param float minority_profit : 单季度.少数股东损益,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_financial_gene_qincome'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -3022,15 +3026,15 @@
     :param float uncertained_investment_loss :  单季度.未确认的投资损失,
     :param float net_profit : 单季度.净利润,
     :param float np_from_parent_company_owners : 单季度.归属于母公司所有者的净利润,
     :param float minority_profit : 单季度.少数股东损益,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_financial_bank_qincome'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -3075,15 +3079,15 @@
     :param float income_tax_cost : 单季度.所得税费用,
     :param float net_profit : 单季度.净利润,
     :param float np_from_parent_company_owners : 单季度.归属于母公司所有者的净利润,
     :param float minority_profit : 单季度.少数股东损益,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_financial_secu_qincome'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -3135,15 +3139,15 @@
     :param float total_profit : 单季度.利润总额,
     :param float net_profit : 单季度.净利润,
     :param float np_from_parent_company_owners : 单季度.归属于母公司所有者的净利润,
     :param float minority_profit : 单季度.少数股东损益,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_financial_insu_qincome'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -3199,15 +3203,15 @@
     :param float subtotal_finance_cash_outflow : 单季度.筹资活动现金流出小计,
     :param float net_finance_cash_flow : 单季度.筹资活动产生的现金流量净额,
     :param float exchange_rate_change_effect : 单季度.汇率变动对现金及现金等价物的影响,
     :param float cash_equivalent_increase : 单季度.现金及现金等价物净增加额,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_financial_gene_qcashflow'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -3267,15 +3271,15 @@
     :param float subtotal_finance_cash_outflow : 单季度.筹资活动现金流出小计,
     :param float net_finance_cash_flow : 单季度.筹资活动产生的现金流量净额,
     :param float exchange_rate_change_effect : 单季度.汇率变动对现金及现金等价物的影响,
     :param float cash_equivalent_increase : 现金及现金等价物净增加额,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_financial_bank_qcashflow'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -3332,15 +3336,15 @@
     :param float subtotal_finance_cash_outflow : 单季度.筹资活动现金流出小计,
     :param float net_finance_cash_flow : 单季度.筹资活动产生的现金流量净额,
     :param float exchange_rate_change_effect : 单季度.汇率变动对现金及现金等价物的影响,
     :param float cash_equivalent_increase : 单季度.现金及现金等价物净增加额,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_financial_secu_qcashflow'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -3401,15 +3405,15 @@
     :param float subtotal_finance_cash_outflow : 单季度.筹资活动现金流出小计,
     :param float net_finance_cash_flow : 单季度.筹资活动产生的现金流量净额,
     :param float exchange_rate_change_effect : 单季度.汇率变动对现金及现金等价物的影响,
     :param float cash_equivalent_increase : 单季度.现金及现金等价物净增加额,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_financial_insu_qcashflow'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -3442,15 +3446,15 @@
     :param float eeps_ceiling : 预计每股收益上限,
     :param float eeps_floor : 预计每股收益下限,
     :param float basic_eps : 去年同期每股收益,
     :param float np_yoy_consistent_forecast : 一致预期净利润增幅,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_performance_forecast'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'forecast_object': forecast_object, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -3495,15 +3499,15 @@
     :param float roe_weighted_yoy : 净资产收益率(加权) 同比,
     :param float net_asset_ps_to_opening : 每股净资产较期初比,
     :param float total_assets_to_opening : 总资产较期初比,
     :param float se_without_mi_to_opening : 归属母公司股东权益较期初比,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_performance_letters'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -3537,15 +3541,15 @@
     :param float operating_profit_mom : 营业利润单季度环比,
     :param float total_profit_mom : 利润总额单季度环比,
     :param float np_parent_company_owners_mom : 归属母公司股东的净利润单季度环比,
     :param float net_profit_cut_div_mom : 扣除非经常性损益后净利润单季度环比,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_performance_letters_q'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -3579,15 +3583,15 @@
     :param str mor_project : 主营构成（按地区）-项目名称,
     :param float mor_main_oper_income : 主营构成（按地区）-项目收入,
     :param float mor_main_oper_cost : 主营构成（按地区）-项目成本,
     :param float mor_moc : 主营构成（按地区）-项目利润,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_main_composition'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'classification': classification, 'order': order, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -3613,15 +3617,15 @@
     :param float main_oper_income_rate_top5_customers : 主营业务收入占比-前5名客户,
     :param float purchase_top5_supplier : 采购额-前5名供应商,
     :param float purchase_rate_top5_supplier : 采购额占比-前5名供应商,
     :param float main_oper_cost_rate_top5_supplier : 主营业务成本占比-前5名供应商,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_trading_parties'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -3643,15 +3647,15 @@
     :param str report_date : 申报日期,
     :param str accounting_firm : 审计单位,
     :param str signature_accountant : 签字注册会计师,
     :param str audit_opinion_type : 审计意见,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_audit_opinion'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -3697,15 +3701,15 @@
     :param float cash_flowps : 每股现金流量净额,
     :param float cash_flowps_ttm : 每股现金流量净额（TTM）,
     :param float enterprise_fcf_ps : 每股企业自由现金流量,
     :param float shareholder_fcf_ps : 每股股东自由现金流量,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_per_share_index'
 
     param = {
 'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
@@ -3771,15 +3775,15 @@
     :param float admini_expense_rate_ttm : 管理费用／营业总收入_TTM,
     :param float financial_expense_rate_ttm : 财务费用／营业总收入_TTM,
     :param float asset_impa_loss_to_tor_ttm : 资产减值损失／营业总收入_TTM,
     :param float asset_impa_loss_or_ttm : 资产减值损失／营业利润（TTM）,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_profitability'
 
     param = {
 'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
@@ -3823,15 +3827,15 @@
     :param float se_without_mi : 净资产（同比增长率）,
     :param float total_liability : 总负债（同比增长率）,
     :param float total_assets : 总资产（同比增长率）,
     :param float cash_equivalent_increase : 现金净流量（同比增长率）,
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_growth_capacity'
 
     param = {
 'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
@@ -3861,15 +3865,15 @@
     :param float ebit_to_tor : 息税前利润／营业总收入,
     :param float operating_revenue_ta : 资产周转率,
     :param float equity_multipler : 权益乘数,
     :param float np_parent_company_owners_ratio : 归属于母公司股东的净利润占比,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_du_pont_analysis'
 
     param = {
 'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
@@ -3933,15 +3937,15 @@
     :param float net_operate_cash_flow_ttm : 经营活动现金净流量(TTM),
     :param float net_invest_cash_flow_ttm : 投资活动现金净流量(TTM),
     :param float net_finance_cash_flow_ttm : 筹资活动现金净流量(TTM),
     :param float net_cash_flow_ttm : 现金净流量(TTM),
 
     """
 
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_deri_fin_indicators'
 
     param = {
 'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
@@ -4017,15 +4021,15 @@
     :param float cash_equivalent_increase_yoy : 单季度.现金净流量同比增长率,
     :param float cash_equivalent_increase_mom : 单季度.现金净流量环比增长率,
     :param float net_operate_cash_flow_yoy : 单季度.经营性现金净流量同比增长率,
     :param float net_operate_cash_flow_mom : 单季度.经营性现金净流量环比增长率,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_q_financial_indicator'
 
     param = {
 'en_prod_code': en_prod_code, 'report_date': report_date, 'report_type': report_type, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
@@ -4063,15 +4067,15 @@
     :param float pcf_net_cashflow_lyr : 市现率PCF（经营净流量LYR）,
     :param float dividend_rate : 股息率（年初至最新报告期）,
     :param float total_cash_divi_com_rate_rmb : 股息率（近12个月）,
     :param float total_cash_divi_com_rate_rmb2 : 股息率,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_valuation_info'
 
     param = {
 'en_prod_code': en_prod_code, 'trading_date': trading_date, 'year': year, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
@@ -4101,15 +4105,15 @@
     :param float b_shares_market_value : B股市值（含限售股，交易币种）,
     :param float b_shares_market_value_rmb : B股市值（含限售股，人民币）,
     :param float b1_shares_market_value : B股市值（不含限售股，交易币种）,
     :param float b1_shares_market_value_rmb : B股市值（不含限售股，人民币）,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_corporation_value'
 
     param = {
 'en_prod_code': en_prod_code, 'trading_date': trading_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
@@ -4143,15 +4147,15 @@
     :param float gross_profit_yoy : 毛利同比,
     :param float gross_profit_per : 毛利占比,
     :param float main_oper_income_rate : 主营业务收入占比,
     :param float main_oper_cost_rate : 主营业务成本占比,
 
     """    
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_main_composition'
 
     param = {'secu_code': secu_code, 'start_date': start_date, 'end_date': end_date, 'classification': classification, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4179,15 +4183,15 @@
     :param float main_oper_profit : 主营业务利润金额,
     :param float main_oper_profit_rate : 主营业务利润所占比率,
     :param float gross_profit_rate : 毛利率,
     :param float main_income_grow_rate_yoy : 收入同比增长,
 
     """    
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_main_business_total'
 
     param = {'secu_code': secu_code, 'classification': classification, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4210,15 +4214,15 @@
     :param float main_oper_profit : 主营业务利润金额,
     :param float main_oper_profit_rate : 主营业务利润所占比率,
     :param float gross_profit_rate : 毛利率,
     :param float main_income_grow_rate_yoy : 收入同比增长,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_stock_main_business_indurstry'
 
     param = {'en_prod_code': en_prod_code}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4242,15 +4246,15 @@
     :param str industry_name_csrc : 所属证监会行业名称,
     :param str sponsor_institution : 保荐机构,
     :param str accounting_firm : 会计师事务所,
     :param str law_firm : 律师事务所,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_star_ipodeclare'
 
     param = {'report_status': report_status, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4282,15 +4286,15 @@
     :param str email : 公司邮箱,
     :param str website : 网址,
     :param str brief_intro : 公司简介,
     :param str industry_name_csrc : 所属证监会行业名称,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_star_companyprofile'
 
     param = {'secu_code': secu_code, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4315,15 +4319,15 @@
     :param str listed_state : 上市状态,
     :param str secu_market : 证券市场,
     :param str listed_sector : 上市板块,
     :param str isin_code : ISIN代码,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_neeq_basic'
 
     param = {'en_prod_code': en_prod_code, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4365,15 +4369,15 @@
     :param str company_cval : 企业属性,
     :param str company_type : 公司类型,
     :param str brief_intro : 公司介绍,
     :param str reg_org : 登记机关,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_neeq_company'
 
     param = {'en_prod_code': en_prod_code, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4397,15 +4401,15 @@
     :param str chief_financial_officer_current : 财务总监(现任),
     :param str chief_financial_officer_former : 财务总监(历任),
     :param str secretary_current : 董事会秘书(现任),
     :param str secretary_former : 董事会秘书(历任),
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_neeq_leader'
 
     param = {'en_prod_code': en_prod_code, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4426,15 +4430,15 @@
     :param str end_date : 截止日期,
     :param float bd_number : 董事会成员数量,
     :param float bs_number : 监事会成员数量,
     :param float manager_number : 高级管理人员数量,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_neeq_leader_num'
 
     param = {'en_prod_code': en_prod_code, 'end_date': end_date, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4460,15 +4464,15 @@
     :param str industry_code_neeq_management : 所属三板管理型行业代码,
     :param str industry_name_neeq_management : 所属三板管理型行业名称,
     :param str industry_code_neeq_investment : 所属三板投资型行业代码,
     :param str industry_name_neeq_investment : 所属三板投资型行业名称,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_neeq_industry'
 
     param = {'en_prod_code': en_prod_code, 'level': level, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4502,15 +4506,15 @@
     :param float eeps_range_ceiling : 预计每股收益幅度上限,
     :param float eeps_range_floor : 预计每股收益幅度下限,
     :param str result_statement : 业绩预计结果说明,
     :param str forcast_content : 业绩预计内容描述,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_neeq_perform_fore'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'unit': unit, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4545,15 +4549,15 @@
     :param float total_operating_revenue : 营业总收入,
     :param float total_assets_avg : 平均资产总额,
     :param float total_debit : 负债总额,
     :param float total_assets : 资产总额,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_neeq_dupont_analysis'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'unit': unit, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4593,15 +4597,15 @@
     :param float restricted_number_h : 有限售:核心员工数量,
     :param float restricted_ratio_h : 有限售:核心员工比例,
     :param float restricted_number_i : 其它有限售数量,
     :param float restricted_ratio_i : 其它有限售比例,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_neeq_share_stru'
 
     param = {'en_prod_code': en_prod_code, 'end_date': end_date, 'unit': unit, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4639,15 +4643,15 @@
     :param float net_operate_cash_flow_ps : 每股经营活动产生的现金流量净额,
     :param float net_operate_cash_flow_ps_ttm : 每股经营活动产生的现金流量净额_TTM,
     :param float cash_flowps : 每股现金流量净额,
     :param float cash_flowps_ttm : 每股现金流量净额_TTM,
 
     """    
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_neeq_per_share_index'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'unit': unit, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4672,15 +4676,15 @@
     :param float issued_plan_number : 增发预案次数,
     :param float issued_impl_number : 增发实施次数,
     :param float accu_ipo_proceeds : 增发累计募集资金总额,
     :param float acc_issue_vol : 增发股份数量,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_neeq_issue_count'
 
     param = {'en_prod_code': en_prod_code, 'date_range': date_range, 'date_type': date_type, 'unit': unit, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4707,15 +4711,15 @@
     :param float average_hold_sum_proportion : 户均持股比例,
     :param float proportion_change : 相对上一报告期户均持股比例差值,
     :param float avg_hold_sum_gr_half_a_year : 户均持股数年增长率,
     :param float proportion_gr_half_a_year : 户均持股比例年增长率,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_neeq_holder_num'
 
     param = {'en_prod_code': en_prod_code, 'report_date': report_date, 'query_direction': query_direction, 'unit': unit, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
@@ -4746,15 +4750,15 @@
     :param float hold_vols_top10_stockholders : 十大股东持股数量,
     :param float hold_vols_top10_fstockholders : 前十大流通股股东持股数量合计,
     :param float total_prop_top10_fstockholders : 前十大流通股股东持股比例合计,
     :param float total_prop_top10_stockholders : 十大股东持股比例,
 
     """
     
-    headers = {'Content-Type': 'application/json', 'token': g_token}
+    headers = get_headers()
     url = base_url + 'get_neeq_holder_info'
 
     param = {'en_prod_code': en_prod_code, 'end_date': end_date, 'serial_number': serial_number, 'share_query_type': share_query_type, 'unit': unit, 'fields': fields}
 
     res = requests.post(url=url, headers=headers, data=json.dumps(param))
 
     if res.ok:
```

