# Comparing `tmp/hivecode-0.0.0.8.21.tar.gz` & `tmp/hivecode-0.0.0.8.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivecode-0.0.0.8.21.tar", last modified: Wed Jul 26 06:37:27 2023, max compression
+gzip compressed data, was "hivecode-0.0.0.8.22.tar", last modified: Sat Jul 29 06:04:04 2023, max compression
```

## Comparing `hivecode-0.0.0.8.21.tar` & `hivecode-0.0.0.8.22.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 06:37:27.537077 hivecode-0.0.0.8.21/
--rw-rw-rw-   0        0        0     3790 2023-07-26 06:37:27.537077 hivecode-0.0.0.8.21/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2023-04-11 20:04:04.000000 hivecode-0.0.0.8.21/README.rst
--rw-rw-rw-   0        0        0     1402 2023-07-26 06:37:02.000000 hivecode-0.0.0.8.21/pyproject.toml
--rw-rw-rw-   0        0        0      226 2023-07-20 05:57:35.000000 hivecode-0.0.0.8.21/requirements.txt
--rw-rw-rw-   0        0        0     1182 2023-07-26 06:37:27.540600 hivecode-0.0.0.8.21/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 06:37:27.474543 hivecode-0.0.0.8.21/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 06:37:27.495233 hivecode-0.0.0.8.21/src/hiveadb/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hiveadb/__init__.py
--rw-rw-rw-   0        0        0     3690 2023-04-12 04:08:02.000000 hivecode-0.0.0.8.21/src/hiveadb/eda.py
--rw-rw-rw-   0        0        0    11500 2023-07-26 06:04:36.000000 hivecode-0.0.0.8.21/src/hiveadb/function.py
--rw-rw-rw-   0        0        0     3694 2023-07-26 06:36:39.000000 hivecode-0.0.0.8.21/src/hiveadb/functions.py
--rw-rw-rw-   0        0        0    86747 2023-04-11 23:45:25.000000 hivecode-0.0.0.8.21/src/hiveadb/io.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hiveadb/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-26 06:37:27.516405 hivecode-0.0.0.8.21/src/hivecode.egg-info/
--rw-rw-rw-   0        0        0     3790 2023-07-26 06:37:27.000000 hivecode-0.0.0.8.21/src/hivecode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      774 2023-07-26 06:37:27.000000 hivecode-0.0.0.8.21/src/hivecode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 06:37:27.000000 hivecode-0.0.0.8.21/src/hivecode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.21/src/hivecode.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      314 2023-07-26 06:37:27.000000 hivecode-0.0.0.8.21/src/hivecode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-26 06:37:27.000000 hivecode-0.0.0.8.21/src/hivecode.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 06:37:27.527993 hivecode-0.0.0.8.21/src/hivecore/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivecore/__init__.py
--rw-rw-rw-   0        0        0     1330 2023-05-08 01:20:28.000000 hivecode-0.0.0.8.21/src/hivecore/constant.py
--rw-rw-rw-   0        0        0     9402 2023-07-15 21:48:03.000000 hivecode-0.0.0.8.21/src/hivecore/decorator.py
--rw-rw-rw-   0        0        0     2744 2023-04-25 03:07:04.000000 hivecode-0.0.0.8.21/src/hivecore/eda.py
--rw-rw-rw-   0        0        0     7676 2023-07-26 05:32:41.000000 hivecode-0.0.0.8.21/src/hivecore/functions.py
--rw-rw-rw-   0        0        0    32180 2023-07-26 05:19:59.000000 hivecode-0.0.0.8.21/src/hivecore/patterns.py
--rw-rw-rw-   0        0        0    28728 2023-07-20 03:05:40.000000 hivecode-0.0.0.8.21/src/hivecore/preprocess.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivecore/py.typed
--rw-rw-rw-   0        0        0     6276 2023-04-25 03:07:19.000000 hivecode-0.0.0.8.21/src/hivecore/visual.py
-drwxrwxrwx   0        0        0        0 2023-07-26 06:37:27.535557 hivecode-0.0.0.8.21/src/hivesignal/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivesignal/__init__.py
--rw-rw-rw-   0        0        0     1683 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivesignal/analysis.py
--rw-rw-rw-   0        0        0      292 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivesignal/eda.py
--rw-rw-rw-   0        0        0     2383 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivesignal/io.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivesignal/py.typed
--rw-rw-rw-   0        0        0     2126 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivesignal/transform.py
+drwxrwxrwx   0        0        0        0 2023-07-29 06:04:04.443242 hivecode-0.0.0.8.22/
+-rw-rw-rw-   0        0        0     3790 2023-07-29 06:04:04.443242 hivecode-0.0.0.8.22/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2023-04-11 20:04:04.000000 hivecode-0.0.0.8.22/README.rst
+-rw-rw-rw-   0        0        0     1402 2023-07-29 06:03:23.000000 hivecode-0.0.0.8.22/pyproject.toml
+-rw-rw-rw-   0        0        0      226 2023-07-20 05:57:35.000000 hivecode-0.0.0.8.22/requirements.txt
+-rw-rw-rw-   0        0        0     1182 2023-07-29 06:04:04.447003 hivecode-0.0.0.8.22/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 06:04:04.339204 hivecode-0.0.0.8.22/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 06:04:04.355309 hivecode-0.0.0.8.22/src/hiveadb/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hiveadb/__init__.py
+-rw-rw-rw-   0        0        0     3690 2023-04-12 04:08:02.000000 hivecode-0.0.0.8.22/src/hiveadb/eda.py
+-rw-rw-rw-   0        0        0    11930 2023-07-29 05:56:28.000000 hivecode-0.0.0.8.22/src/hiveadb/function.py
+-rw-rw-rw-   0        0        0     3694 2023-07-26 06:36:39.000000 hivecode-0.0.0.8.22/src/hiveadb/functions.py
+-rw-rw-rw-   0        0        0    86747 2023-04-11 23:45:25.000000 hivecode-0.0.0.8.22/src/hiveadb/io.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hiveadb/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-29 06:04:04.398388 hivecode-0.0.0.8.22/src/hivecode.egg-info/
+-rw-rw-rw-   0        0        0     3790 2023-07-29 06:04:04.000000 hivecode-0.0.0.8.22/src/hivecode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      774 2023-07-29 06:04:04.000000 hivecode-0.0.0.8.22/src/hivecode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 06:04:04.000000 hivecode-0.0.0.8.22/src/hivecode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.22/src/hivecode.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      314 2023-07-29 06:04:04.000000 hivecode-0.0.0.8.22/src/hivecode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-29 06:04:04.000000 hivecode-0.0.0.8.22/src/hivecode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 06:04:04.432158 hivecode-0.0.0.8.22/src/hivecore/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivecore/__init__.py
+-rw-rw-rw-   0        0        0     1330 2023-05-08 01:20:28.000000 hivecode-0.0.0.8.22/src/hivecore/constant.py
+-rw-rw-rw-   0        0        0     9402 2023-07-15 21:48:03.000000 hivecode-0.0.0.8.22/src/hivecore/decorator.py
+-rw-rw-rw-   0        0        0     2744 2023-04-25 03:07:04.000000 hivecode-0.0.0.8.22/src/hivecore/eda.py
+-rw-rw-rw-   0        0        0    10008 2023-07-29 05:36:22.000000 hivecode-0.0.0.8.22/src/hivecore/functions.py
+-rw-rw-rw-   0        0        0    32180 2023-07-26 05:19:59.000000 hivecode-0.0.0.8.22/src/hivecore/patterns.py
+-rw-rw-rw-   0        0        0    28728 2023-07-20 03:05:40.000000 hivecode-0.0.0.8.22/src/hivecore/preprocess.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivecore/py.typed
+-rw-rw-rw-   0        0        0     6276 2023-04-25 03:07:19.000000 hivecode-0.0.0.8.22/src/hivecore/visual.py
+drwxrwxrwx   0        0        0        0 2023-07-29 06:04:04.441684 hivecode-0.0.0.8.22/src/hivesignal/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivesignal/__init__.py
+-rw-rw-rw-   0        0        0     1683 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivesignal/analysis.py
+-rw-rw-rw-   0        0        0      292 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivesignal/eda.py
+-rw-rw-rw-   0        0        0     2383 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivesignal/io.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivesignal/py.typed
+-rw-rw-rw-   0        0        0     2126 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivesignal/transform.py
```

### Comparing `hivecode-0.0.0.8.21/PKG-INFO` & `hivecode-0.0.0.8.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hivecode
-Version: 0.0.0.8.21
+Version: 0.0.0.8.22
 Summary: Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell.
 Author: Juan Manuel Mejía Botero
 Author-email: Juan Manuel Mejía Botero <juanmam941025@gmail.com>, Sebastian López Valencia <sebaslv12@hotmail.com>
 Project-URL: Homepage, https://github.com/Juanmam/hivecode
 Project-URL: Documentation, https://hivecode.readthedocs.io/en/latest/
 Platform: unix
 Platform: linux
```

### Comparing `hivecode-0.0.0.8.21/README.rst` & `hivecode-0.0.0.8.22/README.rst`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.21/pyproject.toml` & `hivecode-0.0.0.8.22/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "hivecode"
 description = "Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell."
-version = "0.0.0.8.21"
+version = "0.0.0.8.22"
 requires-python = ">=3.8.0"
 readme = "README.rst"
 authors = [
     {name = "Juan Manuel Mejía Botero", email="juanmam941025@gmail.com"},
     {name = "Sebastian López Valencia", email="sebaslv12@hotmail.com"}
 ]
```

### Comparing `hivecode-0.0.0.8.21/setup.cfg` & `hivecode-0.0.0.8.22/setup.cfg`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.21/src/hiveadb/eda.py` & `hivecode-0.0.0.8.22/src/hiveadb/eda.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.21/src/hiveadb/function.py` & `hivecode-0.0.0.8.22/src/hiveadb/function.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,293 +1,292 @@
-from hivecore.constant import PANDAS_TYPES, PYSPARK_TYPES, KOALAS_TYPES, PANDAS_ON_SPARK_TYPES, PANDAS, KOALAS, SPARK, PYSPARK, PANDAS_ON_SPARK, IN_PANDAS_ON_SPARK, IN_PYSPARK
-from hivecore.functions import lib_required, LazyImport
+# from hivecore.constant import PANDAS_TYPES, PYSPARK_TYPES, KOALAS_TYPES, PANDAS_ON_SPARK_TYPES, PANDAS, KOALAS, SPARK, PYSPARK, PANDAS_ON_SPARK, IN_PANDAS_ON_SPARK, IN_PYSPARK
+# from hivecore.functions import lib_required, LazyImport
 
-LazyImport.import_from("databricks.koalas", from_pandas = 'from_pandas', KoalasDataFrame = 'DataFrame')
-LazyImport.import_from('pyspark.context',  SparkContext = 'SparkContext')
-LazyImport.import_from('pyspark.context',  SparkContext = 'SparkSession')
-LazyImport.import_from('pyspark.context',  SparkContext = 'SparkSession')
-LazyImport.import_from('pyspark.pandas', ps_from_pandas = 'from_pandas')
-
-from typing import List, Union, Any
-
-
-def get_spark() -> SparkSession:
-    """
-    Fetches the current instance of Spark. If none exists, creates a new one.
-
-    :return: The current Spark session.
-    :rtype: pyspark.sql.SparkSession
-    """
-    # Spark
-    sc: SparkContext = SparkContext.getOrCreate()
-    return SparkSession(sc)
-
-
-# DBUtils
-try:
-    # up to DBR 8.2
-    from dbutils import DBUtils  # pylint: disable=import-error,wrong-import-position
-except:
-    # above DBR 8.3
-    from dbruntime.dbutils import DBUtils  # pylint: disable=import-error,wrong-import-position
-
-
-def get_dbutils(spark: SparkSession = None) -> DBUtils:
-    """
-    Fetches the current instance of DBUtils.
-
-    :param spark: The current spark session. Defaults to None.
-    :type spark: pyspark.sql.SparkSession
-
-    :return: An instance of DBUtils.
-    :rtype: databricks.DBUtils
-    """
+# LazyImport().from_("databricks.koalas", from_pandas = 'from_pandas', DataFrame = 'KoalasDataFrame')
+# LazyImport().from_("pyspark.context", "SparkContext")
+# LazyImport().from_("pyspark.sql.session", "SparkSession")
+# LazyImport().from_('pyspark.context',  SparkContext = 'SparkSession')
+# LazyImport().from_('pyspark.pandas', from_pandas = 'ps_from_pandas')
+
+# from typing import List, Union, Any
+
+# def get_spark() -> SparkSession:
+#     """
+#     Fetches the current instance of Spark. If none exists, creates a new one.
+
+#     :return: The current Spark session.
+#     :rtype: pyspark.sql.SparkSession
+#     """
+#     # Spark
+#     sc: SparkContext = SparkContext.getOrCreate()
+#     return SparkSession(sc)
+
+
+# # DBUtils
+# try:
+#     # up to DBR 8.2
+#     from dbutils import DBUtils  # pylint: disable=import-error,wrong-import-position
+# except:
+#     # above DBR 8.3
+#     from dbruntime.dbutils import DBUtils  # pylint: disable=import-error,wrong-import-position
+
+
+# def get_dbutils(spark: SparkSession = None) -> DBUtils:
+#     """
+#     Fetches the current instance of DBUtils.
+
+#     :param spark: The current spark session. Defaults to None.
+#     :type spark: pyspark.sql.SparkSession
+
+#     :return: An instance of DBUtils.
+#     :rtype: databricks.DBUtils
+#     """
         
-    # We try to create dbutils from spark or by using IPython
-    try:
-        return DBUtils(spark)
-    except:
-        import IPython
-        return IPython.get_ipython().user_ns["dbutils"]
-
-
-spark   = get_spark()
-dbutils = get_dbutils()
-
-
-from typing import List
-
-def mount(
-    storage: str,
-    key: str,
-    mount_point: str = '/mnt/',
-    mounts: List[str] = ["raw", "silver", "gold"],
-    postfix: str = '-zone',
-    include_tqdm: bool = False,
-    verbose: bool = False
-) -> None:
-    """
-    Mounts a set of zones into the system.
+#     # We try to create dbutils from spark or by using IPython
+#     try:
+#         return DBUtils(spark)
+#     except:
+#         import IPython
+#         return IPython.get_ipython().user_ns["dbutils"]
+
+
+# spark   = get_spark()
+# dbutils = get_dbutils()
+
+
+# from typing import List
+
+# def mount(
+#     storage: str,
+#     key: str,
+#     mount_point: str = '/mnt/',
+#     mounts: List[str] = ["raw", "silver", "gold"],
+#     postfix: str = '-zone',
+#     include_tqdm: bool = False,
+#     verbose: bool = False
+# ) -> None:
+#     """
+#     Mounts a set of zones into the system.
 
-    :param storage: The name of the storage to mount. This can be found at keys access in your storage account.
-    :type storage: str
+#     :param storage: The name of the storage to mount. This can be found at keys access in your storage account.
+#     :type storage: str
     
-    :param key: The key of the storage to mount. This can be found at keys access in your storage account.
-    :type key: str
+#     :param key: The key of the storage to mount. This can be found at keys access in your storage account.
+#     :type key: str
     
-    :param mount_point: The mount point to use, defaults to '/mnt/'.
-    :type mount_point: str, optional
+#     :param mount_point: The mount point to use, defaults to '/mnt/'.
+#     :type mount_point: str, optional
     
-    :param mounts: A list of all the mounts you want. This doesn't include the prefix. Check example. 
-        Defaults to ["raw", "silver", "gold"].
-    :type mounts: List[str], optional
+#     :param mounts: A list of all the mounts you want. This doesn't include the prefix. Check example. 
+#         Defaults to ["raw", "silver", "gold"].
+#     :type mounts: List[str], optional
     
-    :param postfix: The postfix is the ending you want to put to your mount zones. Set it to an empty 
-        string if you don't want to apply it, defaults to '-zone'.
-    :type postfix: str, optional
+#     :param postfix: The postfix is the ending you want to put to your mount zones. Set it to an empty 
+#         string if you don't want to apply it, defaults to '-zone'.
+#     :type postfix: str, optional
     
-    :param include_tqdm: A flag to include tqdm bars for mounts, defaults to False.
-    :type include_tqdm: bool, optional
+#     :param include_tqdm: A flag to include tqdm bars for mounts, defaults to False.
+#     :type include_tqdm: bool, optional
     
-    :param verbose: A flag to indicate whether to show tqdm progress bar or not, defaults to False.
-    :type verbose: bool, optional
+#     :param verbose: A flag to indicate whether to show tqdm progress bar or not, defaults to False.
+#     :type verbose: bool, optional
     
-    :return: None
-    :rtype: None
-    """
-    def __mount(mount_name: str) -> None:
-        """
-        Mounts a single zone to the system.
-
-        :param mount_name: The name of the zone to mount.
-        :type mount_name: str
-
-        :return: None
-        :rtype: None
-        """
-        if not f"{mount_point}{mount_name}" in list(map(lambda mount: mount.mountPoint, dbutils.fs.mounts())):
-            dbutils.fs.mount(
-                source=f"wasbs://{mount_name}@{storage}.blob.core.windows.net/",
-                mount_point=f"{mount_point}{mount_name}",
-                extra_configs={f"fs.azure.account.key.{storage}.blob.core.windows.net": key}
-            )
-
-    lib_required("tqdm")
-    from tqdm import tqdm
-
-    if include_tqdm:
-        mount_iterator = tqdm(mounts, desc="Mounts", position=0, leave=True)
-    else:
-        mount_iterator = mounts
-
-    if verbose:
-        mount_iterator = tqdm(mount_iterator)
-
-    for mount_name in mount_iterator:
-        __mount(mount_name)
-
-import pandas
-import pyspark
-
-
-def data_convert(df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame],
-                 as_type: str) -> Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]:
-    """
-    Converts a DataFrame between Koalas, Pandas, PySpark, and PySpark.pandas.
+#     :return: None
+#     :rtype: None
+#     """
+#     def __mount(mount_name: str) -> None:
+#         """
+#         Mounts a single zone to the system.
+
+#         :param mount_name: The name of the zone to mount.
+#         :type mount_name: str
+
+#         :return: None
+#         :rtype: None
+#         """
+#         if not f"{mount_point}{mount_name}" in list(map(lambda mount: mount.mountPoint, dbutils.fs.mounts())):
+#             dbutils.fs.mount(
+#                 source=f"wasbs://{mount_name}@{storage}.blob.core.windows.net/",
+#                 mount_point=f"{mount_point}{mount_name}",
+#                 extra_configs={f"fs.azure.account.key.{storage}.blob.core.windows.net": key}
+#             )
+
+#     lib_required("tqdm")
+#     from tqdm import tqdm
+
+#     if include_tqdm:
+#         mount_iterator = tqdm(mounts, desc="Mounts", position=0, leave=True)
+#     else:
+#         mount_iterator = mounts
+
+#     if verbose:
+#         mount_iterator = tqdm(mount_iterator)
+
+#     for mount_name in mount_iterator:
+#         __mount(mount_name)
+
+# import pandas
+# import pyspark
+
+
+# def data_convert(df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame],
+#                  as_type: str) -> Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]:
+#     """
+#     Converts a DataFrame between Koalas, Pandas, PySpark, and PySpark.pandas.
 
-    :param df: The DataFrame to be converted.
-    :type df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
+#     :param df: The DataFrame to be converted.
+#     :type df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
     
-    :param as_type: The type of DataFrame to convert to.
-    :type as_type: str
+#     :param as_type: The type of DataFrame to convert to.
+#     :type as_type: str
     
-    :return: The converted DataFrame.
-    :rtype: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
-    """
-    # Koalas
-    if df_type(df) == KOALAS:
-        if as_type.lower() == PANDAS:
-            return df.to_pandas()  # Koalas to Pandas
-        elif as_type.lower() in IN_PYSPARK:
-            return df.to_spark()   # Koalas to Spark
-        elif as_type.lower() in IN_PANDAS_ON_SPARK:
-            try:
-                return data_convert(data_convert(df, as_type = PANDAS), as_type = PANDAS_ON_SPARK)
-            except:
-                try:
-                    return data_convert(data_convert(df, as_type = SPARK), as_type = PANDAS_ON_SPARK)
-                except:
-                    raise
-        elif as_type.lower() == KOALAS:
-            return df
-
-    # Pandas
-    elif df_type(df) == PANDAS:
-        if as_type.lower() == KOALAS:
-            return from_pandas(df) # Pandas to Koalas
-        elif as_type.lower() in IN_PYSPARK:
-            # Pandas to Spark
-            try:
-                return spark.createDataFrame(df)
-            except:
-                return spark.createDataFrame(df.astype(str))
-        elif as_type.lower() in IN_PANDAS_ON_SPARK:
-            return ps_from_pandas(df)
-        elif as_type.lower() == PANDAS:
-            return df
-
-    # Spark
-    elif df_type(df) == PYSPARK:
-        if as_type.lower() == PANDAS:
-            return df.toPandas()   # Spark to Pandas
-        elif as_type.lower() == KOALAS:
-            return KoalasDataFrame(df)
-        elif as_type.lower() in IN_PANDAS_ON_SPARK:
-            try:
-                return df.pandas_api()
-            except:
-                try:
-                    return df.to_pandas_on_spark()
-                except:
-                    raise
-        elif as_type.lower() in IN_PYSPARK:
-            return df
+#     :return: The converted DataFrame.
+#     :rtype: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
+#     """
+#     # Koalas
+#     if df_type(df) == KOALAS:
+#         if as_type.lower() == PANDAS:
+#             return df.to_pandas()  # Koalas to Pandas
+#         elif as_type.lower() in IN_PYSPARK:
+#             return df.to_spark()   # Koalas to Spark
+#         elif as_type.lower() in IN_PANDAS_ON_SPARK:
+#             try:
+#                 return data_convert(data_convert(df, as_type = PANDAS), as_type = PANDAS_ON_SPARK)
+#             except:
+#                 try:
+#                     return data_convert(data_convert(df, as_type = SPARK), as_type = PANDAS_ON_SPARK)
+#                 except:
+#                     raise
+#         elif as_type.lower() == KOALAS:
+#             return df
+
+#     # Pandas
+#     elif df_type(df) == PANDAS:
+#         if as_type.lower() == KOALAS:
+#             return from_pandas(df) # Pandas to Koalas
+#         elif as_type.lower() in IN_PYSPARK:
+#             # Pandas to Spark
+#             try:
+#                 return spark.createDataFrame(df)
+#             except:
+#                 return spark.createDataFrame(df.astype(str))
+#         elif as_type.lower() in IN_PANDAS_ON_SPARK:
+#             return ps_from_pandas(df)
+#         elif as_type.lower() == PANDAS:
+#             return df
+
+#     # Spark
+#     elif df_type(df) == PYSPARK:
+#         if as_type.lower() == PANDAS:
+#             return df.toPandas()   # Spark to Pandas
+#         elif as_type.lower() == KOALAS:
+#             return KoalasDataFrame(df)
+#         elif as_type.lower() in IN_PANDAS_ON_SPARK:
+#             try:
+#                 return df.pandas_api()
+#             except:
+#                 try:
+#                     return df.to_pandas_on_spark()
+#                 except:
+#                     raise
+#         elif as_type.lower() in IN_PYSPARK:
+#             return df
         
-    # Pyspark.pandas
-    elif df_type(df) == PANDAS_ON_SPARK:
-        if as_type.lower() == PANDAS:
-            return df.to_pandas()
-        elif as_type.lower() == KOALAS:
-            # No native support for pyspark.pandas to databrick.koalas.
-            # This needs to be done by a doble transformation.
-            try:
-                return from_pandas(df.to_pandas())
-            except:
-                try:
-                    return KoalasDataFrame(df)
-                except:
-                    raise
-        elif as_type.lower() in IN_PYSPARK:
-            return df.to_spark()
-        elif as_type.lower() in IN_PANDAS_ON_SPARK:
-            return df
-
-
-def select(df: Union[pandas.DataFrame, pyspark.sql.DataFrame, KoalasDataFrame], 
-           columns: List[str]) -> Union[pandas.DataFrame, pyspark.sql.DataFrame, KoalasDataFrame]:
-    """
-    Select columns from a DataFrame.
-
-    :param df: The DataFrame to select columns from.
-    :type df: Union[pandas.DataFrame, pyspark.sql.DataFrame, KoalasDataFrame]
-    :param columns: The columns to select.
-    :type columns: List[str]
-    :return: A new DataFrame with only the selected columns.
-    :rtype: Union[pandas.DataFrame, pyspark.sql.DataFrame, KoalasDataFrame]
-    """
-    if isinstance(df, pandas.DataFrame):
-        return df[columns]
-    elif isinstance(df, pyspark.sql.DataFrame):
-        return df.select(columns)
-    elif isinstance(df, KoalasDataFrame):
-        return df[columns]
-    else:
-        raise ValueError("Unsupported DataFrame type")
-
-
-def to_list(df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame, pandas.Series], 
-            columns: List[str] = None) -> Union[List[Any], List[List[Any]]]:
-    """
-    Convert a DataFrame or Series to a list. If the input is a DataFrame, the output is a list of lists (one for each
-    column), otherwise, the output is a flat list. The input DataFrame can be of type KoalasDataFrame, pandas.DataFrame,
-    pyspark.sql.DataFrame, pyspark.pandas.DataFrame, or pandas.Series.
-
-    :param df: DataFrame or Series to convert.
-    :type df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame, pandas.Series]
-
-    :param columns: Optional list of column names to convert. If not specified, all columns are converted.
-    :type columns: List[str], optional
-
-    :return: A list or list of lists, depending on the input DataFrame type.
-    :rtype: Union[List[Any], List[List[Any]]]
-    """
-    if str(type(df)) in [KOALAS_TYPES.get("series"), PANDAS_TYPES.get("series"), PYSPARK_TYPES.get("series"), PANDAS_ON_SPARK_TYPES.get("series")]:
-        if str(type(df)) == KOALAS_TYPES.get("series"):
-            return df.to_list()
-        elif str(type(df)) == PANDAS_TYPES.get("series"):
-            return df.to_list()
-        elif str(type(df)) == PYSPARK_TYPES.get("series"):
-            return df.rdd.flatMap(lambda x: x).collect()
-        elif str(type(df)) == PANDAS_ON_SPARK_TYPES.get("series"):
-            return df.to_list()
-    elif str(type(df)) in [KOALAS_TYPES.get("df"), PANDAS_TYPES.get("df"), PYSPARK_TYPES.get("df"), PANDAS_ON_SPARK_TYPES.get("df")]:
-        if not isinstance(columns, list):
-            columns = [columns]
-        if str(type(df)) == PANDAS_TYPES.get("df"):
-            return list(map(lambda column: df[column].to_list(), columns))
-        elif str(type(df)) == PYSPARK_TYPES.get("df"):
-            return df.select(columns).rdd.flatMap(lambda x: x).collect()
-        elif str(type(df)) == KOALAS_TYPES.get("df"):
-            return list(map(lambda column: df[column].to_list(), columns))
-        elif str(type(df)) == PANDAS_ON_SPARK_TYPES.get("df"):
-            return list(map(lambda column: df[column].to_list(), columns))
-
-
-def df_type(df: Union[pandas.DataFrame, KoalasDataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]) -> str:
-    """
-    Determines the type of DataFrame object passed as an argument.
+#     # Pyspark.pandas
+#     elif df_type(df) == PANDAS_ON_SPARK:
+#         if as_type.lower() == PANDAS:
+#             return df.to_pandas()
+#         elif as_type.lower() == KOALAS:
+#             # No native support for pyspark.pandas to databrick.koalas.
+#             # This needs to be done by a doble transformation.
+#             try:
+#                 return from_pandas(df.to_pandas())
+#             except:
+#                 try:
+#                     return KoalasDataFrame(df)
+#                 except:
+#                     raise
+#         elif as_type.lower() in IN_PYSPARK:
+#             return df.to_spark()
+#         elif as_type.lower() in IN_PANDAS_ON_SPARK:
+#             return df
+
+
+# def select(df: Union[pandas.DataFrame, pyspark.sql.DataFrame, KoalasDataFrame], 
+#            columns: List[str]) -> Union[pandas.DataFrame, pyspark.sql.DataFrame, KoalasDataFrame]:
+#     """
+#     Select columns from a DataFrame.
+
+#     :param df: The DataFrame to select columns from.
+#     :type df: Union[pandas.DataFrame, pyspark.sql.DataFrame, KoalasDataFrame]
+#     :param columns: The columns to select.
+#     :type columns: List[str]
+#     :return: A new DataFrame with only the selected columns.
+#     :rtype: Union[pandas.DataFrame, pyspark.sql.DataFrame, KoalasDataFrame]
+#     """
+#     if isinstance(df, pandas.DataFrame):
+#         return df[columns]
+#     elif isinstance(df, pyspark.sql.DataFrame):
+#         return df.select(columns)
+#     elif isinstance(df, KoalasDataFrame):
+#         return df[columns]
+#     else:
+#         raise ValueError("Unsupported DataFrame type")
+
+
+# def to_list(df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame, pandas.Series], 
+#             columns: List[str] = None) -> Union[List[Any], List[List[Any]]]:
+#     """
+#     Convert a DataFrame or Series to a list. If the input is a DataFrame, the output is a list of lists (one for each
+#     column), otherwise, the output is a flat list. The input DataFrame can be of type KoalasDataFrame, pandas.DataFrame,
+#     pyspark.sql.DataFrame, pyspark.pandas.DataFrame, or pandas.Series.
+
+#     :param df: DataFrame or Series to convert.
+#     :type df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame, pandas.Series]
+
+#     :param columns: Optional list of column names to convert. If not specified, all columns are converted.
+#     :type columns: List[str], optional
+
+#     :return: A list or list of lists, depending on the input DataFrame type.
+#     :rtype: Union[List[Any], List[List[Any]]]
+#     """
+#     if str(type(df)) in [KOALAS_TYPES.get("series"), PANDAS_TYPES.get("series"), PYSPARK_TYPES.get("series"), PANDAS_ON_SPARK_TYPES.get("series")]:
+#         if str(type(df)) == KOALAS_TYPES.get("series"):
+#             return df.to_list()
+#         elif str(type(df)) == PANDAS_TYPES.get("series"):
+#             return df.to_list()
+#         elif str(type(df)) == PYSPARK_TYPES.get("series"):
+#             return df.rdd.flatMap(lambda x: x).collect()
+#         elif str(type(df)) == PANDAS_ON_SPARK_TYPES.get("series"):
+#             return df.to_list()
+#     elif str(type(df)) in [KOALAS_TYPES.get("df"), PANDAS_TYPES.get("df"), PYSPARK_TYPES.get("df"), PANDAS_ON_SPARK_TYPES.get("df")]:
+#         if not isinstance(columns, list):
+#             columns = [columns]
+#         if str(type(df)) == PANDAS_TYPES.get("df"):
+#             return list(map(lambda column: df[column].to_list(), columns))
+#         elif str(type(df)) == PYSPARK_TYPES.get("df"):
+#             return df.select(columns).rdd.flatMap(lambda x: x).collect()
+#         elif str(type(df)) == KOALAS_TYPES.get("df"):
+#             return list(map(lambda column: df[column].to_list(), columns))
+#         elif str(type(df)) == PANDAS_ON_SPARK_TYPES.get("df"):
+#             return list(map(lambda column: df[column].to_list(), columns))
+
+
+# def df_type(df: Union[pandas.DataFrame, KoalasDataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]) -> str:
+#     """
+#     Determines the type of DataFrame object passed as an argument.
 
-    :param df: A pandas DataFrame, Koalas DataFrame, Spark DataFrame, or PandasOnSpark DataFrame object.
-    :type df: Union[pandas.DataFrame, databricks.koalas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
+#     :param df: A pandas DataFrame, Koalas DataFrame, Spark DataFrame, or PandasOnSpark DataFrame object.
+#     :type df: Union[pandas.DataFrame, databricks.koalas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
     
-    :return: A string representing the type of the input DataFrame.
-    :rtype: str
-    """
-
-    if str(type(df)) == "<class 'pandas.core.frame.DataFrame'>":
-        return PANDAS
-    elif str(type(df)) == "<class 'pyspark.sql.dataframe.DataFrame'>":
-        return PYSPARK
-    elif str(type(df)) == "<class 'databricks.koalas.frame.DataFrame'>":
-        return KOALAS
-    elif str(type(df)) == "<class 'pyspark.pandas.frame.DataFrame'>":
-        return PANDAS_ON_SPARK
+#     :return: A string representing the type of the input DataFrame.
+#     :rtype: str
+#     """
+
+#     if str(type(df)) == "<class 'pandas.core.frame.DataFrame'>":
+#         return PANDAS
+#     elif str(type(df)) == "<class 'pyspark.sql.dataframe.DataFrame'>":
+#         return PYSPARK
+#     elif str(type(df)) == "<class 'databricks.koalas.frame.DataFrame'>":
+#         return KOALAS
+#     elif str(type(df)) == "<class 'pyspark.pandas.frame.DataFrame'>":
+#         return PANDAS_ON_SPARK
```

### Comparing `hivecode-0.0.0.8.21/src/hiveadb/functions.py` & `hivecode-0.0.0.8.22/src/hiveadb/functions.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.21/src/hiveadb/io.py` & `hivecode-0.0.0.8.22/src/hiveadb/io.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.21/src/hivecode.egg-info/PKG-INFO` & `hivecode-0.0.0.8.22/src/hivecode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hivecode
-Version: 0.0.0.8.21
+Version: 0.0.0.8.22
 Summary: Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell.
 Author: Juan Manuel Mejía Botero
 Author-email: Juan Manuel Mejía Botero <juanmam941025@gmail.com>, Sebastian López Valencia <sebaslv12@hotmail.com>
 Project-URL: Homepage, https://github.com/Juanmam/hivecode
 Project-URL: Documentation, https://hivecode.readthedocs.io/en/latest/
 Platform: unix
 Platform: linux
```

### Comparing `hivecode-0.0.0.8.21/src/hivecode.egg-info/SOURCES.txt` & `hivecode-0.0.0.8.22/src/hivecode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.21/src/hivecore/constant.py` & `hivecode-0.0.0.8.22/src/hivecore/constant.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.21/src/hivecore/decorator.py` & `hivecode-0.0.0.8.22/src/hivecore/decorator.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.21/src/hivecore/eda.py` & `hivecode-0.0.0.8.22/src/hivecore/eda.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.21/src/hivecore/patterns.py` & `hivecode-0.0.0.8.22/src/hivecore/patterns.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.21/src/hivecore/preprocess.py` & `hivecode-0.0.0.8.22/src/hivecore/preprocess.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.21/src/hivecore/visual.py` & `hivecode-0.0.0.8.22/src/hivecore/visual.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.21/src/hivesignal/analysis.py` & `hivecode-0.0.0.8.22/src/hivesignal/analysis.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.21/src/hivesignal/io.py` & `hivecode-0.0.0.8.22/src/hivesignal/io.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.21/src/hivesignal/transform.py` & `hivecode-0.0.0.8.22/src/hivesignal/transform.py`

 * *Files identical despite different names*

