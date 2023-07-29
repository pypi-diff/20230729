# Comparing `tmp/pyvoting-1.0.2.tar.gz` & `tmp/pyvoting-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvoting-1.0.2.tar", last modified: Tue Jul 18 08:51:16 2023, max compression
+gzip compressed data, was "pyvoting-1.0.3.tar", last modified: Sat Jul 29 04:38:51 2023, max compression
```

## Comparing `pyvoting-1.0.2.tar` & `pyvoting-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 08:51:16.880046 pyvoting-1.0.2/
--rw-rw-rw-   0        0        0    34607 2023-07-17 08:47:07.000000 pyvoting-1.0.2/LICENCE
--rw-rw-rw-   0        0        0    14522 2023-07-18 08:51:16.877760 pyvoting-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    13647 2023-07-18 08:12:16.000000 pyvoting-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 08:51:16.858580 pyvoting-1.0.2/pyvoting/
--rw-rw-rw-   0        0        0     3360 2023-07-18 05:22:04.000000 pyvoting-1.0.2/pyvoting/ApprovalVoting.py
--rw-rw-rw-   0        0        0     4001 2023-07-18 05:22:56.000000 pyvoting-1.0.2/pyvoting/NormalizedScoreVoting.py
--rw-rw-rw-   0        0        0     4163 2023-07-18 05:20:39.000000 pyvoting-1.0.2/pyvoting/PluralityVoting.py
--rw-rw-rw-   0        0        0     4946 2023-07-18 05:22:35.000000 pyvoting-1.0.2/pyvoting/RankedChoiceVoting.py
--rw-rw-rw-   0        0        0     5802 2023-07-18 05:22:26.000000 pyvoting-1.0.2/pyvoting/STARVoting.py
--rw-rw-rw-   0        0        0     3569 2023-07-18 05:22:14.000000 pyvoting-1.0.2/pyvoting/ScoreVoting.py
--rw-rw-rw-   0        0        0     3990 2023-07-18 05:23:01.000000 pyvoting-1.0.2/pyvoting/StandardizedScoreVoting.py
--rw-rw-rw-   0        0        0     5573 2023-07-18 08:48:51.000000 pyvoting-1.0.2/pyvoting/TierListVoting.py
--rw-rw-rw-   0        0        0     5578 2023-07-18 05:22:46.000000 pyvoting-1.0.2/pyvoting/TieredPopularityVoting.py
--rw-rw-rw-   0        0        0     8707 2023-07-18 06:57:23.000000 pyvoting-1.0.2/pyvoting/Voting.py
--rw-rw-rw-   0        0        0      466 2023-07-18 08:49:35.000000 pyvoting-1.0.2/pyvoting/__init__.py
--rw-rw-rw-   0        0        0     1311 2023-07-18 08:48:45.000000 pyvoting-1.0.2/pyvoting/main.py
-drwxrwxrwx   0        0        0        0 2023-07-18 08:51:16.869229 pyvoting-1.0.2/pyvoting.egg-info/
--rw-rw-rw-   0        0        0    14522 2023-07-18 08:51:16.000000 pyvoting-1.0.2/pyvoting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2023-07-18 08:51:16.000000 pyvoting-1.0.2/pyvoting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 08:51:16.000000 pyvoting-1.0.2/pyvoting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-18 08:51:16.000000 pyvoting-1.0.2/pyvoting.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 08:51:16.000000 pyvoting-1.0.2/pyvoting.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 08:51:16.880046 pyvoting-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1394 2023-07-18 08:50:31.000000 pyvoting-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:38:51.711434 pyvoting-1.0.3/
+-rw-rw-rw-   0        0        0    34607 2023-07-17 08:47:07.000000 pyvoting-1.0.3/LICENCE
+-rw-rw-rw-   0        0        0    46836 2023-07-29 04:38:51.711434 pyvoting-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    45605 2023-07-29 04:36:23.000000 pyvoting-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 04:38:51.693363 pyvoting-1.0.3/pyvoting/
+-rw-rw-rw-   0        0        0     3360 2023-07-18 05:22:04.000000 pyvoting-1.0.3/pyvoting/ApprovalVoting.py
+-rw-rw-rw-   0        0        0     4001 2023-07-18 05:22:56.000000 pyvoting-1.0.3/pyvoting/NormalizedScoreVoting.py
+-rw-rw-rw-   0        0        0     4163 2023-07-18 05:20:39.000000 pyvoting-1.0.3/pyvoting/PluralityVoting.py
+-rw-rw-rw-   0        0        0     4946 2023-07-25 05:35:03.000000 pyvoting-1.0.3/pyvoting/RankedChoiceVoting.py
+-rw-rw-rw-   0        0        0     5802 2023-07-18 05:22:26.000000 pyvoting-1.0.3/pyvoting/STARVoting.py
+-rw-rw-rw-   0        0        0     3569 2023-07-18 05:22:14.000000 pyvoting-1.0.3/pyvoting/ScoreVoting.py
+-rw-rw-rw-   0        0        0     3990 2023-07-18 05:23:01.000000 pyvoting-1.0.3/pyvoting/StandardizedScoreVoting.py
+-rw-rw-rw-   0        0        0     5573 2023-07-25 05:35:20.000000 pyvoting-1.0.3/pyvoting/TierListVoting.py
+-rw-rw-rw-   0        0        0     5578 2023-07-25 05:35:12.000000 pyvoting-1.0.3/pyvoting/TieredPopularityVoting.py
+-rw-rw-rw-   0        0        0     8707 2023-07-20 05:09:28.000000 pyvoting-1.0.3/pyvoting/Voting.py
+-rw-rw-rw-   0        0        0      466 2023-07-18 08:49:35.000000 pyvoting-1.0.3/pyvoting/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-07-18 08:48:45.000000 pyvoting-1.0.3/pyvoting/main.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:38:51.710426 pyvoting-1.0.3/pyvoting.egg-info/
+-rw-rw-rw-   0        0        0    46836 2023-07-29 04:38:51.000000 pyvoting-1.0.3/pyvoting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      507 2023-07-29 04:38:51.000000 pyvoting-1.0.3/pyvoting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 04:38:51.000000 pyvoting-1.0.3/pyvoting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-29 04:38:51.000000 pyvoting-1.0.3/pyvoting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-29 04:38:51.000000 pyvoting-1.0.3/pyvoting.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 04:38:51.711434 pyvoting-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1395 2023-07-29 04:38:18.000000 pyvoting-1.0.3/setup.py
```

### Comparing `pyvoting-1.0.2/LICENCE` & `pyvoting-1.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `pyvoting-1.0.2/pyvoting/ApprovalVoting.py` & `pyvoting-1.0.3/pyvoting/ApprovalVoting.py`

 * *Files identical despite different names*

### Comparing `pyvoting-1.0.2/pyvoting/NormalizedScoreVoting.py` & `pyvoting-1.0.3/pyvoting/NormalizedScoreVoting.py`

 * *Files identical despite different names*

### Comparing `pyvoting-1.0.2/pyvoting/PluralityVoting.py` & `pyvoting-1.0.3/pyvoting/PluralityVoting.py`

 * *Files identical despite different names*

### Comparing `pyvoting-1.0.2/pyvoting/RankedChoiceVoting.py` & `pyvoting-1.0.3/pyvoting/RankedChoiceVoting.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     def __init__(self, candidates, try_handle_invalid=True, reverse=False, 
                  allowed_rank=0):
         super().__init__(candidates, try_handle_invalid)
         """
         New Parameters
         reverse : bool, default=False
             default is #1 is the most preferred and #2 the second, etc...
-            if set to True, bigger numbers are more preferred instead
+            if set to True, larger numbers are more preferred instead
         allowed_rank : int, default=0
             each ballot can only list the top allowed_rank favorite candidates
             if set to 0, there is no limit on it
         """
         self.reverse = reverse
         if allowed_rank==0:
             allowed_rank = len(candidates)
```

### Comparing `pyvoting-1.0.2/pyvoting/STARVoting.py` & `pyvoting-1.0.3/pyvoting/STARVoting.py`

 * *Files identical despite different names*

### Comparing `pyvoting-1.0.2/pyvoting/ScoreVoting.py` & `pyvoting-1.0.3/pyvoting/ScoreVoting.py`

 * *Files identical despite different names*

### Comparing `pyvoting-1.0.2/pyvoting/StandardizedScoreVoting.py` & `pyvoting-1.0.3/pyvoting/StandardizedScoreVoting.py`

 * *Files identical despite different names*

### Comparing `pyvoting-1.0.2/pyvoting/TierListVoting.py` & `pyvoting-1.0.3/pyvoting/TierListVoting.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     def __init__(self, candidates, try_handle_invalid=True, reverse=False, 
                  allowed_tier=0):
         super().__init__(candidates, try_handle_invalid)
         """
         New Parameters
         reverse : bool, default=False
             default is #1 is the most preferred and #2 the second, etc...
-            if set to True, bigger numbers are more preferred instead
+            if set to True, larger numbers are more preferred instead
         allowed_tier : int, default=0
             the number of tiers each ballot is allowed to list, excluding a 
             default tier at the bottom
             if set to 0, there is no limit on it
         """
         self.reverse = reverse
         if allowed_tier==0:
```

### Comparing `pyvoting-1.0.2/pyvoting/TieredPopularityVoting.py` & `pyvoting-1.0.3/pyvoting/TieredPopularityVoting.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     def __init__(self, candidates, try_handle_invalid=True, reverse=False, 
                  allowed_tier=0):
         super().__init__(candidates, try_handle_invalid)
         """
         New Parameters
         reverse : bool, default=False
             default is #1 is the most preferred and #2 the second, etc...
-            if set to True, bigger numbers are more preferred instead
+            if set to True, larger numbers are more preferred instead
         allowed_tier : int, default=0
             the number of tiers each ballot is allowed to list, excluding a 
             default tier at the bottom
             if set to 0, there is no limit on it
         """
         self.reverse = reverse
         if allowed_tier==0:
```

### Comparing `pyvoting-1.0.2/pyvoting/Voting.py` & `pyvoting-1.0.3/pyvoting/Voting.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         int
             number of candidates to be placed in the upper bracket
         """
         return num_candidates-1
     
     def RunMultiWinnerElection(self, candidates=None):
         """
-        Runs a multi winner election with the given candidates and get the 
+        Runs a multi-winner election with the given candidates and get the 
         results. 
         
         Parameters
         candidates : list, default=None
             a list of unique strings representing the candidates
             if None, all candidates specified in constructor will be included
```

### Comparing `pyvoting-1.0.2/pyvoting/main.py` & `pyvoting-1.0.3/pyvoting/main.py`

 * *Files identical despite different names*

### Comparing `pyvoting-1.0.2/setup.py` & `pyvoting-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # you need to change all these
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'simulating elections with 9 choices of voting methods, including 4 I have invented'
 LONG_DESCRIPTION = 'simulating elections with 9 choices of voting methods, including 4 I have invented'
 
 setup(
     name="pyvoting",
     version=VERSION,
     author="Yichen Zhang",
@@ -23,15 +23,15 @@
     long_description=long_description,
     packages=find_packages(),
     install_requires=["pandas", "numpy"],
     keywords=["python", "vote", "voting", "election", "approval voting",
               "star voting", "ranked choice voting", "rcv", "tier list", 
               "tier list voting"],
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 6 - Mature",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

