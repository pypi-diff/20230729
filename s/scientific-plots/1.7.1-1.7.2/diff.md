# Comparing `tmp/scientific_plots-1.7.1.tar.gz` & `tmp/scientific_plots-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scientific_plots-1.7.1.tar", last modified: Fri Jul 14 13:44:17 2023, max compression
+gzip compressed data, was "scientific_plots-1.7.2.tar", last modified: Sat Jul 29 12:24:25 2023, max compression
```

## Comparing `scientific_plots-1.7.1.tar` & `scientific_plots-1.7.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.160221 scientific_plots-1.7.1/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-25 08:00:18.000000 scientific_plots-1.7.1/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)    11607 2023-07-14 13:44:17.160221 scientific_plots-1.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1683 2023-06-25 08:15:40.000000 scientific_plots-1.7.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.7.1/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 13:44:17.160221 scientific_plots-1.7.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.148221 scientific_plots-1.7.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.152221 scientific_plots-1.7.1/src/cycler-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/cycler-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.152221 scientific_plots-1.7.1/src/hurst-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/hurst-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.152221 scientific_plots-1.7.1/src/matplotlib-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-30 21:18:04.000000 scientific_plots-1.7.1/src/matplotlib-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/matplotlib-stubs/animation.pyi
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.7.1/src/matplotlib-stubs/cm.pyi
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/matplotlib-stubs/colors.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1464 2023-07-12 15:45:02.000000 scientific_plots-1.7.1/src/matplotlib-stubs/figure.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.152221 scientific_plots-1.7.1/src/matplotlib-stubs/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     8988 2023-07-12 15:45:02.000000 scientific_plots-1.7.1/src/matplotlib-stubs/pyplot/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/matplotlib-stubs/pyplot/style.pyi
--rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-24 21:33:21.000000 scientific_plots-1.7.1/src/matplotlib-stubs/ticker.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.152221 scientific_plots-1.7.1/src/mpl_toolkits-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.7.1/src/mpl_toolkits-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.7.1/src/mpl_toolkits-stubs/mplot.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.152221 scientific_plots-1.7.1/src/numba-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/numba-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.152221 scientific_plots-1.7.1/src/python_translator-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/python_translator-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.156221 scientific_plots-1.7.1/src/scientific_plots/
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-07-14 12:17:58.000000 scientific_plots-1.7.1/src/scientific_plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scientific_plots/data_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    18907 2023-06-25 08:00:18.000000 scientific_plots-1.7.1/src/scientific_plots/default_plots.py
--rw-rw-rw-   0 root         (0) root         (0)    20586 2023-07-14 13:33:18.000000 scientific_plots-1.7.1/src/scientific_plots/plot_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 13:43:50.000000 scientific_plots-1.7.1/src/scientific_plots/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scientific_plots/two_d_plot.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scientific_plots/types_.py
--rw-rw-rw-   0 root         (0) root         (0)     8954 2023-06-25 09:05:46.000000 scientific_plots-1.7.1/src/scientific_plots/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.156221 scientific_plots-1.7.1/src/scientific_plots.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11607 2023-07-14 13:44:17.000000 scientific_plots-1.7.1/src/scientific_plots.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1363 2023-07-14 13:44:17.000000 scientific_plots-1.7.1/src/scientific_plots.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 13:44:17.000000 scientific_plots-1.7.1/src/scientific_plots.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-14 13:44:17.000000 scientific_plots-1.7.1/src/scientific_plots.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      126 2023-07-14 13:44:17.000000 scientific_plots-1.7.1/src/scientific_plots.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.156221 scientific_plots-1.7.1/src/scipy-stubs/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scipy-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scipy-stubs/fft.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1134 2023-07-07 14:38:21.000000 scientific_plots-1.7.1/src/scipy-stubs/integrate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3032 2023-07-07 14:38:21.000000 scientific_plots-1.7.1/src/scipy-stubs/interpolate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scipy-stubs/optimize.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.156221 scientific_plots-1.7.1/src/scipy-stubs/signal/
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scipy-stubs/signal/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scipy-stubs/signal/windows.pyi
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scipy-stubs/special.pyi
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scipy-stubs/stats.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.160221 scientific_plots-1.7.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3116 2023-07-14 13:19:44.000000 scientific_plots-1.7.1/tests/test_plot_manual.py
--rw-rw-rw-   0 root         (0) root         (0)     3783 2023-07-12 15:45:02.000000 scientific_plots-1.7.1/tests/test_plots.py
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/tests/test_types.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/tests/test_utilties.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:24:25.155110 scientific_plots-1.7.2/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-25 08:00:18.000000 scientific_plots-1.7.2/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)    11607 2023-07-29 12:24:25.155110 scientific_plots-1.7.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1683 2023-06-25 08:15:40.000000 scientific_plots-1.7.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.7.2/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 12:24:25.155110 scientific_plots-1.7.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:24:25.143111 scientific_plots-1.7.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:24:25.147111 scientific_plots-1.7.2/src/cycler-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/cycler-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:24:25.147111 scientific_plots-1.7.2/src/hurst-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/hurst-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:24:25.147111 scientific_plots-1.7.2/src/matplotlib-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-30 21:18:04.000000 scientific_plots-1.7.2/src/matplotlib-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/matplotlib-stubs/animation.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.7.2/src/matplotlib-stubs/cm.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/matplotlib-stubs/colors.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1464 2023-07-12 15:45:02.000000 scientific_plots-1.7.2/src/matplotlib-stubs/figure.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:24:25.147111 scientific_plots-1.7.2/src/matplotlib-stubs/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     8988 2023-07-12 15:45:02.000000 scientific_plots-1.7.2/src/matplotlib-stubs/pyplot/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/matplotlib-stubs/pyplot/style.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-24 21:33:21.000000 scientific_plots-1.7.2/src/matplotlib-stubs/ticker.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:24:25.147111 scientific_plots-1.7.2/src/mpl_toolkits-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.7.2/src/mpl_toolkits-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.7.2/src/mpl_toolkits-stubs/mplot.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:24:25.147111 scientific_plots-1.7.2/src/numba-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/numba-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:24:25.147111 scientific_plots-1.7.2/src/python_translator-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/python_translator-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:24:25.151111 scientific_plots-1.7.2/src/scientific_plots/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-07-29 12:13:19.000000 scientific_plots-1.7.2/src/scientific_plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/scientific_plots/data_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    18907 2023-06-25 08:00:18.000000 scientific_plots-1.7.2/src/scientific_plots/default_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    22668 2023-07-29 12:13:19.000000 scientific_plots-1.7.2/src/scientific_plots/plot_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-29 12:23:59.000000 scientific_plots-1.7.2/src/scientific_plots/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/scientific_plots/two_d_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/scientific_plots/types_.py
+-rw-rw-rw-   0 root         (0) root         (0)     8954 2023-06-25 09:05:46.000000 scientific_plots-1.7.2/src/scientific_plots/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:24:25.151111 scientific_plots-1.7.2/src/scientific_plots.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11607 2023-07-29 12:24:25.000000 scientific_plots-1.7.2/src/scientific_plots.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-07-29 12:24:25.000000 scientific_plots-1.7.2/src/scientific_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:24:25.000000 scientific_plots-1.7.2/src/scientific_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-29 12:24:25.000000 scientific_plots-1.7.2/src/scientific_plots.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2023-07-29 12:24:25.000000 scientific_plots-1.7.2/src/scientific_plots.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:24:25.151111 scientific_plots-1.7.2/src/scipy-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/scipy-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/scipy-stubs/fft.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2023-07-07 14:38:21.000000 scientific_plots-1.7.2/src/scipy-stubs/integrate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3032 2023-07-07 14:38:21.000000 scientific_plots-1.7.2/src/scipy-stubs/interpolate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/scipy-stubs/optimize.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:24:25.151111 scientific_plots-1.7.2/src/scipy-stubs/signal/
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/scipy-stubs/signal/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/scipy-stubs/signal/windows.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/scipy-stubs/special.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/src/scipy-stubs/stats.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:24:25.155110 scientific_plots-1.7.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3116 2023-07-14 13:19:44.000000 scientific_plots-1.7.2/tests/test_plot_manual.py
+-rw-rw-rw-   0 root         (0) root         (0)     3783 2023-07-12 15:45:02.000000 scientific_plots-1.7.2/tests/test_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/tests/test_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.7.2/tests/test_utilties.py
```

### Comparing `scientific_plots-1.7.1/COPYING.LESSER` & `scientific_plots-1.7.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/PKG-INFO` & `scientific_plots-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientific_plots
-Version: 1.7.1
+Version: 1.7.2
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scientific_plots-1.7.1/pyproject.toml` & `scientific_plots-1.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/readme.md` & `scientific_plots-1.7.2/readme.md`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/cycler-stubs/__init__.pyi` & `scientific_plots-1.7.2/src/cycler-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/matplotlib-stubs/__init__.pyi` & `scientific_plots-1.7.2/src/matplotlib-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/matplotlib-stubs/colors.pyi` & `scientific_plots-1.7.2/src/matplotlib-stubs/colors.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/matplotlib-stubs/figure.pyi` & `scientific_plots-1.7.2/src/matplotlib-stubs/figure.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/matplotlib-stubs/pyplot/__init__.pyi` & `scientific_plots-1.7.2/src/matplotlib-stubs/pyplot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/matplotlib-stubs/ticker.pyi` & `scientific_plots-1.7.2/src/matplotlib-stubs/ticker.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/numba-stubs/__init__.pyi` & `scientific_plots-1.7.2/src/numba-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/scientific_plots/data_analysis.py` & `scientific_plots-1.7.2/src/scientific_plots/data_analysis.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/scientific_plots/default_plots.py` & `scientific_plots-1.7.2/src/scientific_plots/default_plots.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/scientific_plots/plot_settings.py` & `scientific_plots-1.7.2/src/scientific_plots/plot_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from .types_ import Vector
 
 mpl.use("Agg")
 plt.rcParams["axes.unicode_minus"] = False
 
 SPINE_COLOR = "black"
 FIGSIZE = (3.15, 2.35)
+FIGSIZE_SLIM = (3.15, 2.1)
 FIGSIZE_SMALL = (2.2, 2.1)
 _savefig = copy(plt.savefig)  # backup the old save-function
 
 
 def linestyles() -> Generator[str, None, None]:
     """get the line-stiles as an iterator"""
     yield "-"
@@ -263,55 +264,111 @@
         mpl.rcParams.update(mpl.rcParamsDefault)
         plt.style.use("default")
 
 
 old_save = plt.savefig
 
 
+def alternative_save(
+        filename: Path,
+        dpi: Optional[int] = None,
+        bbox_inches: Optional[Union[str, tuple[float, float]]] = None,
+        figsize: tuple[float, float] = FIGSIZE,
+        subfolder: str = "small") -> None:
+    """
+    Create additional saves of the given figsize and save these new figures
+    into subfolder of given names. This function can be used to create
+    additional plots of different sizes without a large overhead.
+    """
+    fig = deepcopy(plt.gcf())
+    fig.set_size_inches(*figsize)
+    with catch_warnings(record=True) as warning:
+        simplefilter("always")
+        fig.tight_layout()
+        if warning:
+            if issubclass(warning[-1].category, UserWarning):
+                plt.close(fig)
+                return
+    folder = filename.parent / subfolder
+    folder.mkdir(exist_ok=True)
+    try:
+        fig.savefig(
+            folder
+            / filename.name, dpi=dpi, bbox_inches=bbox_inches)
+    except PermissionError:
+        fig.savefig(
+            folder
+            / (filename.stem + "_" + filename.suffix),
+            dpi=dpi, bbox_inches=bbox_inches)
+    plt.close(fig)
+
+
 def try_save(filename: Path,
              dpi: Optional[int] = None,
              bbox_inches: Optional[Union[str, tuple[float, float]]] = None, *,
-             small: bool = False) -> None:
+             small: bool = False,
+             slim: bool = False) -> None:
     """Try to save the current figure to the given path, if it is not possible,
     try to save it under a different name.
     If small is set to true, also create
-    a smaller version of the given plot."""
-    try:
-        old_save(filename, dpi=dpi, bbox_inches=bbox_inches)
-    except PermissionError:
-        old_save(filename.parent / (filename.stem + "_" + filename.suffix),
-                 dpi=dpi, bbox_inches=bbox_inches)
-
-    if small:
+    a smaller version of the given plot.
+    If slim is set to true, a slightly slimmer version
+    of the plot is created."""
+
+    def alternative_save(
+            figsize: tuple[float, float] = FIGSIZE,
+            subfolder: str = "small") -> None:
+        """
+        Create additional saves of the given figsize and save these new figures
+        into subfolder of given names. This function can be used to create
+        additional plots of different sizes without a large overhead.
+        """
         fig = deepcopy(plt.gcf())
-        fig.set_size_inches(*FIGSIZE_SMALL)
+        fig.set_size_inches(*figsize)
         with catch_warnings(record=True) as warning:
             simplefilter("always")
             fig.tight_layout()
             if warning:
                 if issubclass(warning[-1].category, UserWarning):
                     plt.close(fig)
                     return
-        folder = filename.parent / "small"
+        folder = filename.parent / subfolder
         folder.mkdir(exist_ok=True)
         try:
             fig.savefig(
                 folder
                 / filename.name, dpi=dpi, bbox_inches=bbox_inches)
         except PermissionError:
             fig.savefig(
                 folder
                 / (filename.stem + "_" + filename.suffix),
                 dpi=dpi, bbox_inches=bbox_inches)
         plt.close(fig)
 
+    try:
+        old_save(filename, dpi=dpi, bbox_inches=bbox_inches)
+    except PermissionError:
+        old_save(filename.parent / (filename.stem + "_" + filename.suffix),
+                 dpi=dpi, bbox_inches=bbox_inches)
+
+    if small:
+        alternative_save(
+            figsize=FIGSIZE_SMALL,
+            subfolder="small")
+
+    if slim:
+        alternative_save(
+            figsize=FIGSIZE_SLIM,
+            subfolder="slim")
+
 
 def new_save_simple(subfolder: Union[str, Path] = "", suffix: str = "", *,
                     german: bool = False, png: bool = True,
-                    pdf: bool = True, small: bool = False)\
+                    pdf: bool = True, small: bool = False,
+                    slim: bool = False)\
         -> Callable[..., None]:
     """
     Return a new save function, which saves the file to a new given name in pdf
     format, and also creates a png version.
     If the argument "german" is set to true, also create German language
     version of the plots.
     """
@@ -351,31 +408,34 @@
 
         try:
             plt.tight_layout()
         except IndexError:
             pass
         # save the figure
         if pdf:
-            try_save(new_path_pdf, bbox_inches=bbox_inches, small=small)
+            try_save(new_path_pdf, bbox_inches=bbox_inches,
+                     small=small, slim=slim)
         if png:
             try_save(new_path_png, bbox_inches=bbox_inches,
-                     dpi=dpi, small=small)
+                     dpi=dpi, small=small, slim=slim)
 
         if german:
             with germanify(plt.gca()):
                 if pdf:
                     try_save(
                         new_path_pdf.parent
                         / (new_path_pdf.stem + "_german.pdf"),
-                        bbox_inches=bbox_inches, small=small)
+                        bbox_inches=bbox_inches, small=small,
+                        slim=slim)
                 if png:
                     try_save(
                         new_path_png.parent
                         / (new_path_png.stem + "_german.png"),
-                        bbox_inches=bbox_inches, dpi=dpi, small=small)
+                        bbox_inches=bbox_inches, dpi=dpi, small=small,
+                        slim=slim)
 
     return savefig_
 
 
 def presentation_settings() -> None:
     """Change the settings of rcParams for presentations."""
     # increase size
@@ -525,15 +585,16 @@
                 if three_d:
                     plt.set_cmap("Greys")
                     new_kwargs = copy(kwargs)
                     new_kwargs["colorscheme"] = "Greys"
                 else:
                     new_kwargs = kwargs
                 plt.savefig = new_save_simple("grayscale", png=False,
-                                              small=not three_d)
+                                              small=not three_d,
+                                              slim=not three_d)
                 _plot_function(*args, **new_kwargs)
                 plt.close("all")
 
             def presentation() -> None:
                 """
                 Create a plot for presentations.
                 """
```

### Comparing `scientific_plots-1.7.1/src/scientific_plots/two_d_plot.py` & `scientific_plots-1.7.2/src/scientific_plots/two_d_plot.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/scientific_plots/types_.py` & `scientific_plots-1.7.2/src/scientific_plots/types_.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/scientific_plots/utilities.py` & `scientific_plots-1.7.2/src/scientific_plots/utilities.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/scientific_plots.egg-info/PKG-INFO` & `scientific_plots-1.7.2/src/scientific_plots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientific-plots
-Version: 1.7.1
+Version: 1.7.2
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scientific_plots-1.7.1/src/scientific_plots.egg-info/SOURCES.txt` & `scientific_plots-1.7.2/src/scientific_plots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/scipy-stubs/fft.pyi` & `scientific_plots-1.7.2/src/scipy-stubs/fft.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/scipy-stubs/integrate.pyi` & `scientific_plots-1.7.2/src/scipy-stubs/integrate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/scipy-stubs/interpolate.pyi` & `scientific_plots-1.7.2/src/scipy-stubs/interpolate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/scipy-stubs/optimize.pyi` & `scientific_plots-1.7.2/src/scipy-stubs/optimize.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/src/scipy-stubs/signal/__init__.pyi` & `scientific_plots-1.7.2/src/scipy-stubs/signal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/tests/test_plot_manual.py` & `scientific_plots-1.7.2/tests/test_plot_manual.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/tests/test_plots.py` & `scientific_plots-1.7.2/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/tests/test_types.py` & `scientific_plots-1.7.2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.1/tests/test_utilties.py` & `scientific_plots-1.7.2/tests/test_utilties.py`

 * *Files identical despite different names*

