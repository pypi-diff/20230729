# Comparing `tmp/finlogic-0.6.0.tar.gz` & `tmp/finlogic-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlogic-0.6.0.tar", last modified: Sat Jul 22 08:35:15 2023, max compression
+gzip compressed data, was "finlogic-0.6.1.tar", last modified: Sat Jul 29 13:52:44 2023, max compression
```

## Comparing `finlogic-0.6.0.tar` & `finlogic-0.6.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.6.0/LICENSE
--rw-r--r--   0        0        0     9812 2023-07-22 08:24:02.186627 finlogic-0.6.0/README.md
--rw-r--r--   0        0        0      378 2023-07-22 08:24:02.222628 finlogic-0.6.0/finlogic/__init__.py
--rw-r--r--   0        0        0    20400 2023-07-22 08:24:02.223628 finlogic-0.6.0/finlogic/company.py
--rw-r--r--   0        0        0     7580 2023-07-22 08:24:02.223628 finlogic-0.6.0/finlogic/data.py
--rw-r--r--   0        0        0     8017 2023-07-22 08:24:02.223628 finlogic-0.6.0/finlogic/indicators.py
--rw-r--r--   0        0        0      949 2023-07-22 08:35:15.041046 finlogic-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     2880 2023-07-22 08:24:02.223628 finlogic-0.6.0/tests/test_company.py
--rw-r--r--   0        0        0      709 2023-07-22 08:24:02.223628 finlogic-0.6.0/tests/test_data.py
--rw-r--r--   0        0        0    11799 1970-01-01 00:00:00.000000 finlogic-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.6.1/LICENSE
+-rw-r--r--   0        0        0    10694 2023-07-23 09:37:04.852702 finlogic-0.6.1/README.md
+-rw-r--r--   0        0        0      378 2023-07-29 13:51:24.512436 finlogic-0.6.1/finlogic/__init__.py
+-rw-r--r--   0        0        0    20400 2023-07-22 08:24:02.223628 finlogic-0.6.1/finlogic/company.py
+-rw-r--r--   0        0        0     7860 2023-07-29 13:49:54.946534 finlogic-0.6.1/finlogic/data.py
+-rw-r--r--   0        0        0     8017 2023-07-22 08:24:02.223628 finlogic-0.6.1/finlogic/indicators.py
+-rw-r--r--   0        0        0      949 2023-07-29 13:52:44.126217 finlogic-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     2880 2023-07-22 08:24:02.223628 finlogic-0.6.1/tests/test_company.py
+-rw-r--r--   0        0        0      709 2023-07-22 08:24:02.223628 finlogic-0.6.1/tests/test_data.py
+-rw-r--r--   0        0        0    12681 1970-01-01 00:00:00.000000 finlogic-0.6.1/PKG-INFO
```

### Comparing `finlogic-0.6.0/LICENSE` & `finlogic-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `finlogic-0.6.0/README.md` & `finlogic-0.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -161,44 +161,47 @@
 | 2.02.01.03 | Financiamento por Arrendamento |     82.897 |     98.279 |     95.423 |
 
 ```python
 # Show company main indicators:
 >>> petro.indicators(num_years=3)
 ```
 
-| 2021-12-31 | 2022-12-31 | 2023-03-31 |
-|-----------:|-----------:|-----------:|
-|    972.951 |    976.709 |    978.577 |
-|    168.247 |    163.052 |    157.194 |
-|     62.04  |     56.193 |     66.906 |
-|     33.334 |     -0.679 |     28.744 |
-|    655.359 |    588.895 |    607.53  |
-|    134.913 |    163.731 |    128.45  |
-|    327.818 |    280.703 |    271.031 |
-|    265.778 |    224.51  |    204.125 |
-|    389.581 |    364.385 |    403.405 |
-|    452.668 |    641.256 |    638.683 |
-|    219.637 |    334.1   |    332.645 |
-|    107.264 |    189.005 |    182.529 |
-|    273.879 |    362.457 |    355.838 |
-|    210.831 |    294.255 |    289.054 |
-|    151.575 |    274.998 |    263.614 |
-|    -44.311 |    -85.993 |    -81.085 |
-|    203.126 |    255.41  |    256.345 |
-|     63.048 |     68.202 |     66.784 |
-|      0.292 |      0.312 |      0.307 |
-|      0.141 |      0.199 |      0.192 |
-|      0.397 |      0.515 |      0.453 |
-|      0.214 |      0.312 |      0.309 |
-|      0.485 |      0.521 |      0.520 |
-|      0.605 |      0.565 |      0.557 |
-|      0.465 |      0.458 |      0.452 |
-|      0.236 |      0.294 |      0.285 |
-|      8.18  |     14.44  |     13.95  |
+|                           | 2021-12-31 | 2022-12-31 | 2023-03-31 |
+|:--------------------------|-----------:|-----------:|-----------:|
+| total_assets              |    972.951 |    976.709 |    978.577 |
+| current_assets            |    168.247 |    163.052 |    157.194 |
+| total_cash                |     62.040 |     56.193 |     66.906 |
+| working_capital           |     33.334 |     -0.679 |     28.744 |
+| invested_capital          |    655.359 |    588.895 |    607.530 |
+| current_liabilities       |    134.913 |    163.731 |    128.450 |
+| total_debt                |    327.818 |    280.703 |    271.031 |
+| net_debt                  |    265.778 |    224.510 |    204.125 |
+| equity                    |    389.581 |    364.385 |    403.405 |
+| revenues                  |    452.668 |    641.256 |    638.683 |
+| gross_profit              |    219.637 |    334.100 |    332.645 |
+| net_income                |    107.264 |    189.005 |    182.529 |
+| ebitda                    |    273.879 |    362.457 |    355.838 |
+| ebit                      |    210.831 |    294.255 |    289.054 |
+| ebt                       |    151.575 |    274.998 |    263.614 |
+| effective_tax             |    -44.311 |    -85.993 |    -81.085 |
+| operating_cash_flow       |    203.126 |    255.410 |    256.345 |
+| depreciation_amortization |     63.048 |     68.202 |     66.784 |
+| effective_tax_rate        |      0.292 |      0.312 |      0.307 |
+| return_on_assets          |      0.141 |      0.199 |      0.192 |
+| return_on_equity          |      0.397 |      0.515 |      0.453 |
+| roic                      |      0.214 |      0.312 |      0.309 |
+| gross_margin              |      0.485 |      0.521 |      0.520 |
+| ebitda_margin             |      0.605 |      0.565 |      0.557 |
+| operating_margin          |      0.465 |      0.458 |      0.452 |
+| net_margin                |      0.236 |      0.294 |      0.285 |
+| eps                       |      8.180 |     14.440 |     13.950 |
+<<<<<<< HEAD
+=======
 
+>>>>>>> 09ed54610af5e9d61b25dcb3dc8f9157c36a4b81
 ---
 
 P.S.: All contributors are welcome, from beginner to advanced.
 
 **Felipe Costa and Carlos Carvalho**
 
 <table border=1 cellpadding=10><tr><td>
```

### Comparing `finlogic-0.6.0/finlogic/company.py` & `finlogic-0.6.1/finlogic/company.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.6.0/finlogic/data.py` & `finlogic-0.6.1/finlogic/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 NOT_TRADED_FINANCIALS_URL = "https://raw.githubusercontent.com/crdcj/FinLogic/main/data/not_traded_companies_financials.csv.gz"
 LANGUAGE_DATA_URL = (
     "https://raw.githubusercontent.com/crdcj/FinLogic/main/data/pten_df.csv.gz"
 )
 FINANCIALS_DF = pd.DataFrame()
 TRADES_DF = pd.DataFrame()
 LANGUAGE_DF = pd.DataFrame()
+INDICATORS_DF = pd.DataFrame()
 
 
 def load(is_traded: bool = True, min_volume: int = 100_000):
     """Verify changes in CVM files and update Finlogic Database if necessary.
 
     Args:
         is_traded (bool, optional): If True, only currently traded companies are
@@ -157,15 +158,18 @@
         "is_restructuring",
         "most_traded_stock",
     ]
     return df[show_cols].reset_index(drop=True)
 
 
 def rank(
-    segment: str = None, n: int = 10, rank_by: str = "operating_margin"
+    segment: str = None,
+    n: int = 10,
+    rank_by: str = "operating_margin",
+    is_consolidated: bool = True,
 ) -> pd.DataFrame:
     """Rank companies by a given indicator.
 
     This function returns a DataFrame containing the top n companies in the
     specified segment, ranked by the given indicator.
 
     Args:
@@ -178,26 +182,31 @@
             'operating_cash_flow', 'eps', 'total_cash', 'total_debt',
             'net_debt', 'ebitda', 'gross_margin', 'ebitda_margin',
             'operating_margin', 'net_margin', 'return_on_assets',
             'return_on_equity', 'roic'.
     """
     show_cols = [
         "name_id",
-        "cvm_id",
         "most_traded_stock",
-        "segment",
+        "cvm_id",
         "is_restructuring",
+        "is_consolidated",
+        "segment",
         "period_end",
         rank_by,
     ]
     df = (
-        ind.get_indicators()
-        .sort_values(by=["cvm_id", "period_end", "is_consolidated"], ignore_index=True)
-        # .query("cvm_id == 922")
+        FINANCIALS_DF.sort_values(
+            by=["cvm_id", "period_end", "is_consolidated"], ignore_index=True
+        )
         .drop_duplicates(subset=["cvm_id"], keep="last")
         .merge(TRADES_DF, on="cvm_id")
-        .query("segment.str.contains(@segment)")
+        .merge(
+            INDICATORS_DF[["cvm_id", rank_by, "is_consolidated", "period_end"]],
+            on=["cvm_id", "period_end", "is_consolidated"],
+        )
+        .query("segment.str.contains(@segment) and is_consolidated == @is_consolidated")
         .sort_values(by=[rank_by], ascending=False, ignore_index=True)
         .head(n)[show_cols]
     )
 
     return df
```

### Comparing `finlogic-0.6.0/finlogic/indicators.py` & `finlogic-0.6.1/finlogic/indicators.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.6.0/pyproject.toml` & `finlogic-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "pandas>=1.5.0",
 ]
-version = "0.6.0"
+version = "0.6.1"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 dev = [
     "pytest",
```

### Comparing `finlogic-0.6.0/tests/test_company.py` & `finlogic-0.6.1/tests/test_company.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.6.0/tests/test_data.py` & `finlogic-0.6.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.6.0/PKG-INFO` & `finlogic-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinLogic
-Version: 0.6.0
+Version: 0.6.1
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Carlos Carvalho
         
@@ -201,44 +201,47 @@
 | 2.02.01.03 | Financiamento por Arrendamento |     82.897 |     98.279 |     95.423 |
 
 ```python
 # Show company main indicators:
 >>> petro.indicators(num_years=3)
 ```
 
-| 2021-12-31 | 2022-12-31 | 2023-03-31 |
-|-----------:|-----------:|-----------:|
-|    972.951 |    976.709 |    978.577 |
-|    168.247 |    163.052 |    157.194 |
-|     62.04  |     56.193 |     66.906 |
-|     33.334 |     -0.679 |     28.744 |
-|    655.359 |    588.895 |    607.53  |
-|    134.913 |    163.731 |    128.45  |
-|    327.818 |    280.703 |    271.031 |
-|    265.778 |    224.51  |    204.125 |
-|    389.581 |    364.385 |    403.405 |
-|    452.668 |    641.256 |    638.683 |
-|    219.637 |    334.1   |    332.645 |
-|    107.264 |    189.005 |    182.529 |
-|    273.879 |    362.457 |    355.838 |
-|    210.831 |    294.255 |    289.054 |
-|    151.575 |    274.998 |    263.614 |
-|    -44.311 |    -85.993 |    -81.085 |
-|    203.126 |    255.41  |    256.345 |
-|     63.048 |     68.202 |     66.784 |
-|      0.292 |      0.312 |      0.307 |
-|      0.141 |      0.199 |      0.192 |
-|      0.397 |      0.515 |      0.453 |
-|      0.214 |      0.312 |      0.309 |
-|      0.485 |      0.521 |      0.520 |
-|      0.605 |      0.565 |      0.557 |
-|      0.465 |      0.458 |      0.452 |
-|      0.236 |      0.294 |      0.285 |
-|      8.18  |     14.44  |     13.95  |
+|                           | 2021-12-31 | 2022-12-31 | 2023-03-31 |
+|:--------------------------|-----------:|-----------:|-----------:|
+| total_assets              |    972.951 |    976.709 |    978.577 |
+| current_assets            |    168.247 |    163.052 |    157.194 |
+| total_cash                |     62.040 |     56.193 |     66.906 |
+| working_capital           |     33.334 |     -0.679 |     28.744 |
+| invested_capital          |    655.359 |    588.895 |    607.530 |
+| current_liabilities       |    134.913 |    163.731 |    128.450 |
+| total_debt                |    327.818 |    280.703 |    271.031 |
+| net_debt                  |    265.778 |    224.510 |    204.125 |
+| equity                    |    389.581 |    364.385 |    403.405 |
+| revenues                  |    452.668 |    641.256 |    638.683 |
+| gross_profit              |    219.637 |    334.100 |    332.645 |
+| net_income                |    107.264 |    189.005 |    182.529 |
+| ebitda                    |    273.879 |    362.457 |    355.838 |
+| ebit                      |    210.831 |    294.255 |    289.054 |
+| ebt                       |    151.575 |    274.998 |    263.614 |
+| effective_tax             |    -44.311 |    -85.993 |    -81.085 |
+| operating_cash_flow       |    203.126 |    255.410 |    256.345 |
+| depreciation_amortization |     63.048 |     68.202 |     66.784 |
+| effective_tax_rate        |      0.292 |      0.312 |      0.307 |
+| return_on_assets          |      0.141 |      0.199 |      0.192 |
+| return_on_equity          |      0.397 |      0.515 |      0.453 |
+| roic                      |      0.214 |      0.312 |      0.309 |
+| gross_margin              |      0.485 |      0.521 |      0.520 |
+| ebitda_margin             |      0.605 |      0.565 |      0.557 |
+| operating_margin          |      0.465 |      0.458 |      0.452 |
+| net_margin                |      0.236 |      0.294 |      0.285 |
+| eps                       |      8.180 |     14.440 |     13.950 |
+<<<<<<< HEAD
+=======
 
+>>>>>>> 09ed54610af5e9d61b25dcb3dc8f9157c36a4b81
 ---
 
 P.S.: All contributors are welcome, from beginner to advanced.
 
 **Felipe Costa and Carlos Carvalho**
 
 <table border=1 cellpadding=10><tr><td>
```

