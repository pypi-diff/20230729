# Comparing `tmp/freq_mob-0.1.tar.gz` & `tmp/freq_mob-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freq_mob-0.1.tar", last modified: Wed Jul  5 02:14:54 2023, max compression
+gzip compressed data, was "freq_mob-0.1.4.tar", last modified: Sat Jul 29 20:13:37 2023, max compression
```

## Comparing `freq_mob-0.1.tar` & `freq_mob-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-05 02:14:54.070870 freq_mob-0.1/
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1073 2020-05-13 21:48:18.000000 freq_mob-0.1/LICENSE.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     1718 2023-07-05 02:14:54.065334 freq_mob-0.1/PKG-INFO
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1295 2023-07-05 01:58:22.000000 freq_mob-0.1/README.md
-drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-05 02:14:54.033049 freq_mob-0.1/freq_mob/
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)       69 2023-07-04 21:48:53.000000 freq_mob-0.1/freq_mob/__init__.py
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)    15954 2023-07-05 02:00:23.000000 freq_mob-0.1/freq_mob/freq_mob.py
-drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-05 02:14:54.065334 freq_mob-0.1/freq_mob.egg-info/
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     1718 2023-07-05 02:14:53.000000 freq_mob-0.1/freq_mob.egg-info/PKG-INFO
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)      231 2023-07-05 02:14:53.000000 freq_mob-0.1/freq_mob.egg-info/SOURCES.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        1 2023-07-05 02:14:53.000000 freq_mob-0.1/freq_mob.egg-info/dependency_links.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       38 2023-07-05 02:14:53.000000 freq_mob-0.1/freq_mob.egg-info/requires.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        9 2023-07-05 02:14:53.000000 freq_mob-0.1/freq_mob.egg-info/top_level.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       38 2023-07-05 02:14:54.070870 freq_mob-0.1/setup.cfg
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)      692 2023-07-04 22:00:04.000000 freq_mob-0.1/setup.py
+drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-29 20:13:37.523550 freq_mob-0.1.4/
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1073 2023-07-28 04:54:22.000000 freq_mob-0.1.4/LICENSE.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     2235 2023-07-29 20:13:37.514076 freq_mob-0.1.4/PKG-INFO
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1810 2023-07-29 08:06:21.000000 freq_mob-0.1.4/README.md
+drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-29 20:13:37.480298 freq_mob-0.1.4/freq_mob/
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)       71 2023-07-29 20:11:04.000000 freq_mob-0.1.4/freq_mob/__init__.py
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)    17269 2023-07-29 20:12:35.000000 freq_mob-0.1.4/freq_mob/freq_mob.py
+drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-29 20:13:37.512151 freq_mob-0.1.4/freq_mob.egg-info/
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     2235 2023-07-29 20:13:37.000000 freq_mob-0.1.4/freq_mob.egg-info/PKG-INFO
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)      231 2023-07-29 20:13:37.000000 freq_mob-0.1.4/freq_mob.egg-info/SOURCES.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        1 2023-07-29 20:13:37.000000 freq_mob-0.1.4/freq_mob.egg-info/dependency_links.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       46 2023-07-29 20:13:37.000000 freq_mob-0.1.4/freq_mob.egg-info/requires.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        9 2023-07-29 20:13:37.000000 freq_mob-0.1.4/freq_mob.egg-info/top_level.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       38 2023-07-29 20:13:37.523550 freq_mob-0.1.4/setup.cfg
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)      705 2023-07-29 20:10:30.000000 freq_mob-0.1.4/setup.py
```

### Comparing `freq_mob-0.1/LICENSE.txt` & `freq_mob-0.1.4/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 The MIT License (MIT)
 
-Copyright 2020 WenSui Liu
+Copyright 2023 WenSui Liu
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `freq_mob-0.1/PKG-INFO` & `freq_mob-0.1.4/freq_mob.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 Metadata-Version: 2.1
-Name: freq_mob
-Version: 0.1
+Name: freq-mob
+Version: 0.1.4
 Summary: Monotonic Optimal Binning for Frequency Models
 Home-page: https://github.com/statcompute/freq_mob
 Author: WenSui Liu
 Author-email: liuwensui@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 #### Introduction
 
-To mimic the py\_mob package (https://pypi.org/project/py-mob) for binary outcomes, the freq\_mob is a collection of python functions that would generate the monotonic binning and perform the variable transformation for frequency outcomes such that the Pearson correlation between the transformed X and Ln(Y) is equal to 1. 
+To mimic the py\_mob package (https://pypi.org/project/py-mob) for binary outcomes, the freq\_mob is a collection of python functions that would generate the monotonic binning and perform the variable transformation for frequency outcomes such that the Pearson correlation between the transformed $X$ and $Log(Y)$ is equal to 1. In case of frequency count models with $Log()$ link function, the transformation is derived as $F(x)_i = Log \frac{\sum_i Y / \sum_i Exposure}{\sum Y / \sum Exposure}$ in the training sample, where $Exposure$ is the number of cases and $i$ refers to the $ith$ bin groupped by $x$ values.  
+
+
+Should you have any question or suggestion about the freq\_mob package, please feel free to drop me a line. 
 
 #### Core Functions
 
 ```
 freq_mob
   |-- qtl_bin()  : An iterative discretization based on quantiles of X.  
   |-- cnt_bin()  : A revised iterative discretization for records with Y > 0.
   |-- iso_bin()  : A discretization algorthm driven by the isotonic regression between X and Y. 
-  |-- rng_bin()  : A revised iterative discretization based on the range of X values.  
+  |-- rng_bin()  : A revised iterative discretization based on the value range of X.  
   |-- kmn_bin()  : A discretization algorthm based on the kmeans clustering of X.  
   |-- gbm_bin()  : A discretization algorthm based on the gradient boosting machine.  
   |-- view_bin() : Displays the binning outcome in a tabular form. 
-  `-- cal_newx() : Applies the variable transformation to a numeric vector based on the binning outcome.
+  |-- cal_newx() : Applies the variable transformation to a numeric vector based on the binning outcome.
+  `-- mi_score() : Calculates the mutual information score between X and Y.
 ```
 
 ###  Authors
 
 [WenSui Liu](mailto:liuwensui@gmail.com) is a seasoned data scientist with 15-year experience in the financial service industry. 
-[Joyce Liu](mailto:jcl4482@my.utexas.edu) is a college student major in Mathematics. 
+
+[Joyce Liu](mailto:jcl4482@my.utexas.edu) is a college student majoring in Mathematics with a passion for data science.
```

### Comparing `freq_mob-0.1/freq_mob/freq_mob.py` & `freq_mob-0.1.4/freq_mob/freq_mob.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # freq_mob/freq_mob.py
-# version 0.1
-# import freq_mob
+# version 0.1.4, 07/29/2023
 
-import tabulate, numpy
+import tabulate, numpy, cytoolz, operator
 from scipy.stats import spearmanr
 from sklearn.isotonic import IsotonicRegression as isoreg
 from sklearn.cluster import KMeans as kmeans
 from sklearn import metrics 
 from lightgbm import LGBMRegressor as gbmreg
 
+
 ########## 01. qcut() ##########
 
 def qcut(x, n):
   """
   It is an utility function to discretizes a numeric vector into n pieces based on quantiles.
   Parameters:
     x : A numeric vector.
@@ -22,14 +22,15 @@
   """
 
   _q = numpy.linspace(0, 100, n, endpoint = False)[1:]
   _x = [_ for _ in x if not numpy.isnan(_)]
   _c = numpy.unique(numpy.percentile(_x, _q, method = "lower"))
   return([_ for _ in _c])
 
+
 ########## 02. manual_bin() ##########
 
 def manual_bin(x, y, cuts):
   """
   It is an utility function to discretize the x vector and summarize
   over the y vector based on the discretization result.
   Parameters:
@@ -51,28 +52,30 @@
   return(sorted([dict(zip(["bin", "freq", "miss", "ysum", "minx", "maxx"],
                           [_1, len(_2), 0,
                            sum([_[2] for _ in _2]),
                            min([_[1] for _ in _2]),
                            max([_[1] for _ in _2])])) for _1, _2 in _l2],
                 key = lambda x: x["bin"]))
 
+
 ########## 03. miss_bin() ##########
 
 def miss_bin(y):
   """
   It is an utility function to summarize the y vector.
   Parameters:
     y : A numeric vector.
   Returns:
     A dictionary.
   """
 
   return({"bin": 0, "freq": len([_ for _ in y]), "miss": len([_ for _ in y]),
           "ysum": sum([_ for _ in y]), "minx": numpy.nan, "maxx": numpy.nan})
 
+
 ########## 04. add_miss() ##########
 
 def add_miss(d, l):
   """
   It is an utility function to append the missing value category, if any, to the binning outcome.
   Parameters:
     d : A list with lists generated by input vectors of binning functions.
@@ -89,14 +92,15 @@
       for _ in ['freq', 'miss', 'ysum']:
         _l[0][_]  = _l[0][_]  + _m[_]
     else:
       _l.append(_m)
 
   return(_l)
 
+
 ########## 05. gen_newx() ##########
 
 def gen_newx(x):
   """
   It is an utility function to generate the variable transformation based on the binning outcome.
   Parameters:
     x : A list of dictionaries for the binning outcome.
@@ -109,14 +113,15 @@
 
   _l1 = sorted([{**_,
                  "yavg": round(_["ysum"] / _["freq"], 8),
                  "newx": round(numpy.log((_["ysum"] / _ysum) / (_["freq"] / _freq)), 8)
                 } for _ in x], key = lambda _x: _x["bin"])
   return(_l1)
 
+
 ########## 06. gen_rule() ##########
 
 def gen_rule(tbl, pts):
   """
   It is an utility function to generate binning rules based on the binning 
   outcome table and the list of cut points.
   Parameters:
@@ -142,21 +147,22 @@
     else:
         _["rule"] = "$X$ > " + str(pts[_["bin"] - 2]) + " and $X$ <= " + str(pts[_["bin"] - 1])
 
   _sel = ["bin", "freq", "miss", "ysum", "yavg", "newx", "rule"]
 
   return([{k: _[k] for k in _sel} for _ in tbl])
 
+
 ########## 07. cal_newx() ##########
 
 def cal_newx(x, bin):
   """
   It applies the transformation to a numeric vector based on the binning outcome.
   Parameters:
-    x   : A numeric vector, which can be a list, 1-D numpy array, or pandas series
+    x   : A numeric vector, which can be a list, 1-D numpy array, or pandas series.
     bin : An object containing the binning outcome.
   Returns:
     A list of dictionaries with three keys
   """
 
   _cut = sorted([_ for _ in bin['cut']] + [numpy.PINF, numpy.NINF])
 
@@ -179,37 +185,84 @@
       _m2 = [l + [0, 0] for l in _m1]
     _l3.extend(_m2)
 
   _key = ['x', 'bin', 'newx']
 
   return(list(dict(zip(_key, _[1:])) for _ in sorted(_l3, key = lambda x: x[0])))
 
-########## 08. view_bin() ##########
+
+########## 08. mi_score() ##########
+
+def mi_score(x, y):
+  """
+  It provides the mutual information score between x and y.
+  Parameters:
+    x : A numeric vector, which can be a list, 1-D numpy array, or pandas series.
+    y : A numeric vector, which can be a list, 1-D numpy array, or pandas series.
+  Returns:
+    The mutual information score.
+  """
+  
+  _dt = [_ for _ in zip(x, y) if ~numpy.isnan(_[0]) and ~numpy.isnan(_[1])]
+
+  _cn = len(_dt)
+
+  _l1 = [{"x": i[0][0], "y": i[0][1], "pxy": len(i[1]) / _cn}
+         for i in list(cytoolz.groupby([0, 1], _dt).items())]
+
+  _lx = [{"x": i[0], "px": sum([_["pxy"] for _ in i[1]])}
+         for i in list(cytoolz.groupby("x", _l1).items())]
+
+  _ly = [{"y": i[0], "py": sum([_["pxy"] for _ in i[1]])}
+         for i in list(cytoolz.groupby("y", _l1).items())]
+
+  _l2 = list(dict(_l, **_r) for _l, _r in 
+             cytoolz.join(operator.itemgetter("x"), _l1, operator.itemgetter("x"), _lx))
+
+  _l3 = list(dict(_l, **_r) for _l, _r in 
+             cytoolz.join(operator.itemgetter("y"), _l2, operator.itemgetter("y"), _ly))
+
+  return(sum([_["pxy"] * numpy.log(_["pxy"] / (_["px"] * _["py"])) for _ in _l3]))
+
+
+########## 09. view_bin() ##########
 
 def view_bin(x):
   """
   It displays the binning outcome generated from a binning function, i.e. iso_bin().
   Parameters:
-    x: An object containing the binning outcome.
-  Returns:
-    None
+    x : An object containing the binning outcome.
   """
 
   tabulate.PRESERVE_WHITESPACE = True
 
   _sel = ["bin", "freq", "miss", "ysum", "yavg", "newx"]
 
   _tbl = [{**(lambda v: {k: v[k] for k in _sel})(_), "rule": _["rule"].ljust(45)} for _ in x["tbl"]]
 
   print(tabulate.tabulate(_tbl, headers = "keys", tablefmt = "github",
                           colalign = ["center"] + ["right"] * (len(_sel) - 1),
                           floatfmt = (".0f", ".0f", ".0f", ".4f", ".4f", ".4f")))
 
 
-########## 09. qtl_bin() ##########
+########## 10. head() ##########
+
+def head(seq, n = 3):
+  """
+  It shows first n (3 by default) items in a sequence.
+  Parameters:
+    seq : A list.
+    n   : A non-zero integer.
+  """
+
+  for _ in range(n):
+    print(seq[_])
+
+
+########## 11. qtl_bin() ##########
 
 def qtl_bin(x, y):
   """
   It discretizes the x vector based on percentiles and summarizes
   over the y vector to derive the variable transformation.
   Parameters:
     x : A numeric vector to discretize, e.g. list, numpy array, or pandas series.
@@ -217,15 +270,14 @@
   Returns:
     A dictionary with two keys:
       "cut" : A numeric vector with cut points applied to the x vector.
       "tbl" : A list of dictionaries summarizing the binning outcome.
   """
 
   _data = [_ for _ in zip(x, y, ~numpy.isnan(x))]
-
   _x = [_[0] for _ in _data if _[2] == 1]
   _y = [_[1] for _ in _data if _[2] == 1]
 
   _n = numpy.arange(2, max(3, min(100, len(numpy.unique(_x)) - 1)))
   _p = set(tuple(qcut(_x, _)) for _ in _n)
 
   _l1 = [[_, manual_bin(_x, _y, _)] for _ in _p]
@@ -241,15 +293,16 @@
 
   _l4 = sorted(*[l[1] for l in _l1 if l[0] == _l3], key = lambda x: x["ysum"] / x["freq"])
 
   _l5 = add_miss(_data, _l4)
 
   return({"cut": _l3, "tbl": gen_rule(gen_newx(_l5), _l3)})
 
-########## 10. iso_bin() ##########
+
+########## 12. iso_bin() ##########
 
 def iso_bin(x, y):
   """
   It discretizes the x vector based on the isotonic regression and summarizes
   over the y vector to derive the variable transformation.
   Parameters:
     x : A numeric vector to discretize, e.g. list, numpy array, or pandas series.
@@ -257,15 +310,14 @@
   Returns:
     A dictionary with two keys:
       "cut" : A numeric vector with cut points applied to the x vector.
       "tbl" : A list of dictionaries summarizing the binning outcome.
   """
 
   _data = [_ for _ in zip(x, y, ~numpy.isnan(x))]
-
   _x = [_[0] for _ in _data if _[2] == 1]
   _y = [_[1] for _ in _data if _[2] == 1]
 
   _cor = spearmanr(_x, _y)[0]
   _reg = isoreg()
 
   _f = numpy.abs(_reg.fit_transform(_x, list(map(lambda y:  y * _cor / numpy.abs(_cor), _y))))
@@ -284,33 +336,31 @@
 
   _l4 = sorted(manual_bin(_x, _y, _p), key = lambda x: x["ysum"] / x["freq"])
 
   _l5 = add_miss(_data, _l4)
 
   return({"cut": _p, "tbl": gen_rule(gen_newx(_l5), _p)})
 
-########## 11. gbm_bin() ##########
+
+########## 13. gbm_bin() ##########
 
 def gbm_bin(x, y):
   """
   It discretizes the x vector based on the gradient boosting machine and
   summarizes over the y vector to derive the variable transformation.
   Parameters:
-    x : A numeric vector to discretize. It is a list, 1-D numpy array,
-        or pandas series.
-    y : A numeric vector with binary values of 0/1 and with the same length
-        of x. It is a list, 1-D numpy array, or pandas series.
+    x : A numeric vector to discretize, e.g. list, numpy array, or pandas series.
+    y : A numeric vector of frequency outcomes with the same length of x.
   Returns:
     A dictionary with two keys:
       "cut" : A numeric vector with cut points applied to the x vector.
       "tbl" : A list of dictionaries summarizing the binning outcome.
   """
 
   _data = [_ for _ in zip(x, y, ~numpy.isnan(x))]
-
   _x = [_[0] for _ in _data if _[2] == 1]
   _y = [_[1] for _ in _data if _[2] == 1]
 
   _cor = spearmanr(_x, _y)[0]
   _con = "1" if _cor > 0 else "-1"
 
   _gbm = gbmreg(num_leaves = 100, min_child_samples = 3, n_estimators = 1,
@@ -334,19 +384,20 @@
 
   _l4 = sorted(manual_bin(_x, _y, _p), key = lambda x: x["ysum"] / x["freq"])
 
   _l5 = add_miss(_data, _l4)
 
   return({"cut": _p, "tbl": gen_rule(gen_newx(_l5), _p)})
 
-########## 12. rng_bin() ##########
+
+########## 14. rng_bin() ##########
 
 def rng_bin(x, y):
   """
-  It discretizes the x vector based on the range of x values and summarizes over
+  It discretizes the x vector based on the value range of x and summarizes over
   the y vector to derive the variable transformaton.
   Parameters:
     x : A numeric vector to discretize, e.g. list, numpy array, or pandas series.
     y : A numeric vector of frequency outcomes with the same length of x.
   Returns:
     A dictionary with two keys:
       "cut" : A numeric vector with cut points applied to the x vector.
@@ -377,15 +428,16 @@
 
   _l4 = sorted(*[l[1] for l in _l1 if l[0] == _l3], key = lambda x: x["ysum"] / x["freq"])
 
   _l5 = add_miss(_data, _l4)
 
   return({"cut": _l3, "tbl": gen_rule(gen_newx(_l5), _l3)})
 
-########## 13. kmn_bin() ##########
+
+########## 15. kmn_bin() ##########
 
 def kmn_bin(x, y):
   """
   It discretizes the x vector based on the kmeans clustering and summarizes over 
   the y vector to derive the variable transformation.
   Parameters:
     x : A numeric vector to discretize, e.g. list, numpy array, or pandas series.
@@ -428,15 +480,16 @@
 
   _l4 = sorted(*[l[1] for l in _l1 if l[0] == _l3], key = lambda x: x["ysum"] / x["freq"])
 
   _l5 = add_miss(_data, _l4)
 
   return({"cut": _l3, "tbl": gen_rule(gen_newx(_l5), _l3)})
 
-########## 14. cnt_bin() ##########
+
+########## 16. cnt_bin() ##########
 
 def cnt_bin(x, y):
   """
   It discretizes the x vector based on percentiles and summarizes over
   the y vector with y > 0, i.e. nonzero count, to derive the variable transformation.
   Parameters:
     x : A numeric vector to discretize, e.g. list, numpy array, or pandas series.
@@ -467,8 +520,7 @@
          if numpy.abs(round(l[3], 8)) == 1 and round(l[1], 8) > 0][0]
 
   _l4 = sorted(*[l[1] for l in _l1 if l[0] == _l3], key = lambda x: x["ysum"] / x["freq"])
 
   _l5 = add_miss(_data, _l4)
 
   return({"cut": _l3, "tbl": gen_rule(gen_newx(_l5), _l3)})
-
```

### Comparing `freq_mob-0.1/freq_mob.egg-info/PKG-INFO` & `freq_mob-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 Metadata-Version: 2.1
-Name: freq-mob
-Version: 0.1
+Name: freq_mob
+Version: 0.1.4
 Summary: Monotonic Optimal Binning for Frequency Models
 Home-page: https://github.com/statcompute/freq_mob
 Author: WenSui Liu
 Author-email: liuwensui@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 #### Introduction
 
-To mimic the py\_mob package (https://pypi.org/project/py-mob) for binary outcomes, the freq\_mob is a collection of python functions that would generate the monotonic binning and perform the variable transformation for frequency outcomes such that the Pearson correlation between the transformed X and Ln(Y) is equal to 1. 
+To mimic the py\_mob package (https://pypi.org/project/py-mob) for binary outcomes, the freq\_mob is a collection of python functions that would generate the monotonic binning and perform the variable transformation for frequency outcomes such that the Pearson correlation between the transformed $X$ and $Log(Y)$ is equal to 1. In case of frequency count models with $Log()$ link function, the transformation is derived as $F(x)_i = Log \frac{\sum_i Y / \sum_i Exposure}{\sum Y / \sum Exposure}$ in the training sample, where $Exposure$ is the number of cases and $i$ refers to the $ith$ bin groupped by $x$ values.  
+
+
+Should you have any question or suggestion about the freq\_mob package, please feel free to drop me a line. 
 
 #### Core Functions
 
 ```
 freq_mob
   |-- qtl_bin()  : An iterative discretization based on quantiles of X.  
   |-- cnt_bin()  : A revised iterative discretization for records with Y > 0.
   |-- iso_bin()  : A discretization algorthm driven by the isotonic regression between X and Y. 
-  |-- rng_bin()  : A revised iterative discretization based on the range of X values.  
+  |-- rng_bin()  : A revised iterative discretization based on the value range of X.  
   |-- kmn_bin()  : A discretization algorthm based on the kmeans clustering of X.  
   |-- gbm_bin()  : A discretization algorthm based on the gradient boosting machine.  
   |-- view_bin() : Displays the binning outcome in a tabular form. 
-  `-- cal_newx() : Applies the variable transformation to a numeric vector based on the binning outcome.
+  |-- cal_newx() : Applies the variable transformation to a numeric vector based on the binning outcome.
+  `-- mi_score() : Calculates the mutual information score between X and Y.
 ```
 
 ###  Authors
 
 [WenSui Liu](mailto:liuwensui@gmail.com) is a seasoned data scientist with 15-year experience in the financial service industry. 
-[Joyce Liu](mailto:jcl4482@my.utexas.edu) is a college student major in Mathematics. 
+
+[Joyce Liu](mailto:jcl4482@my.utexas.edu) is a college student majoring in Mathematics with a passion for data science.
```

### Comparing `freq_mob-0.1/setup.py` & `freq_mob-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
  
 with open("README.md", "r") as fh:
   long_description = fh.read()
  
 setuptools.setup(
   name = "freq_mob",
-  version = "0.1",
+  version = "0.1.4",
   author = "WenSui Liu",
   author_email = "liuwensui@gmail.com",
   description = "Monotonic Optimal Binning for Frequency Models",
   long_description = long_description,
   long_description_content_type = "text/markdown",
   url = "https://github.com/statcompute/freq_mob",
   packages = setuptools.find_packages(),
-  install_requires = ['numpy', 'scipy', 'sklearn', 'lightgbm', 'tabulate'], 
+  install_requires = ['numpy', 'scipy', 'sklearn', 'lightgbm', 'tabulate', 'cytoolz'], 
   classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
   ],
 )
```

