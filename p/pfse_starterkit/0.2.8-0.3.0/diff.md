# Comparing `tmp/pfse_starterkit-0.2.8.tar.gz` & `tmp/pfse_starterkit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfse_starterkit-0.2.8.tar", last modified: Fri Feb 10 00:37:29 2023, max compression
+gzip compressed data, was "pfse_starterkit-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pfse_starterkit-0.2.8.tar` & `pfse_starterkit-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1799 2022-12-13 02:38:41.070429 pfse_starterkit-0.2.8/.gitignore
--rw-r--r--   0        0        0    11357 2022-12-13 02:38:41.070429 pfse_starterkit-0.2.8/LICENSE
--rw-r--r--   0        0        0      563 2023-02-10 00:35:18.263825 pfse_starterkit-0.2.8/README.md
--rw-r--r--   0        0        0      205 2023-02-10 00:35:40.471529 pfse_starterkit-0.2.8/pfse_starterkit/__init__.py
--rw-r--r--   0        0        0     7827 2023-01-28 01:12:07.056834 pfse_starterkit-0.2.8/pfse_starterkit/__main__.py
--rw-r--r--   0        0        0     1497 2023-01-27 19:13:51.754840 pfse_starterkit-0.2.8/pfse_starterkit/sectionproperties_test.py
--rw-r--r--   0        0        0       95 2023-01-27 19:13:51.754840 pfse_starterkit-0.2.8/pfse_starterkit/streamlit_test.py
--rw-r--r--   0        0        0     2512 2023-01-27 19:13:51.754840 pfse_starterkit-0.2.8/pfse_starterkit/vtk_cylinder.py
--rw-r--r--   0        0        0     1073 2023-02-10 00:34:49.096213 pfse_starterkit-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 pfse_starterkit-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1799 2022-12-13 02:38:41.070429 pfse_starterkit-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11357 2022-12-13 02:38:41.070429 pfse_starterkit-0.3.0/LICENSE
+-rw-r--r--   0        0        0      600 2023-07-29 18:54:32.430342 pfse_starterkit-0.3.0/README.md
+-rw-r--r--   0        0        0      205 2023-07-29 18:59:56.850634 pfse_starterkit-0.3.0/pfse_starterkit/__init__.py
+-rw-r--r--   0        0        0     8720 2023-07-29 18:49:22.086100 pfse_starterkit-0.3.0/pfse_starterkit/__main__.py
+-rw-r--r--   0        0        0     1497 2023-07-29 18:23:14.482881 pfse_starterkit-0.3.0/pfse_starterkit/sectionproperties_test.py
+-rw-r--r--   0        0        0       95 2023-01-27 19:13:51.754840 pfse_starterkit-0.3.0/pfse_starterkit/streamlit_test.py
+-rw-r--r--   0        0        0     2512 2023-01-27 19:13:51.754840 pfse_starterkit-0.3.0/pfse_starterkit/vtk_cylinder.py
+-rw-r--r--   0        0        0     1154 2023-07-29 18:21:53.863686 pfse_starterkit-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 pfse_starterkit-0.3.0/PKG-INFO
```

### Comparing `pfse_starterkit-0.2.8/.gitignore` & `pfse_starterkit-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pfse_starterkit-0.2.8/LICENSE` & `pfse_starterkit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pfse_starterkit-0.2.8/README.md` & `pfse_starterkit-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -28,12 +28,13 @@
 * xlwings
 * black
 * jupyterlab
 * IPython
 * ipywidgets
 * ipykernel
 * jupyterlab-katex
+* jupyterlab-mathjax3 (as an option)
 * nbconvert
 * pyperclip
 * typer
 * magicgui[pyside2]
 * flit
```

### Comparing `pfse_starterkit-0.2.8/pfse_starterkit/__main__.py` & `pfse_starterkit-0.3.0/pfse_starterkit/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,17 @@
     header = Markdown("# Python for Structural Engineers ('PfSE')")
     addl_installs = Markdown("## Installing additional package for Linux...")
     addl_installs.style = "yellow"
     console.print(header)
     console.print(addl_installs)
 
     install_extra()
+    ipyk_install = Markdown("## Installing pfse Jupyter kernel...")
+    ipyk_install.style = "yellow"
+    install_pfse_kernel()
     validating = Markdown("## Validating installed packages...")
     validating.style = "yellow"
     console.print(validating)
 
     funcs = [
         check_streamlit,
         check_vtk,
@@ -77,22 +80,25 @@
         console.print(close_windows)
 
 
 def check_streamlit():
     st_file = pathlib.Path(__file__).parent / "streamlit_test.py"
     try:
         proc = subprocess.Popen(
-            ["streamlit", "run", str(st_file)], stdout=subprocess.PIPE
+            ["streamlit", "run", str(st_file)],
+            stdout=subprocess.PIPE
         )
         # proc.communicate("\n")
         time.sleep(4)
         proc.kill()
 
-    except ValueError:
+    except Exception as err:
         err_msg = Text("Streamlit did not run properly.")
+        for err_arg in err.args:
+            err_msg.append("\t" + err_arg + "\n")
         err_msg.stylize("bold magenta")
         return err_msg
 
 
 def check_vtk():
     try:
         import vtkmodules.vtkInteractionStyle
@@ -173,19 +179,30 @@
         import numpy as np
     except Exception as err:
         err_msgs = Text("\nnumpy did not import properly:\n")
         for err_arg in err.args:
             err_msgs.append("\t" + err_arg + "\n")
         err_msgs.stylize("bold green")
         return err_msgs
+    
+
+def check_pandas():
+    try:
+        import pandas as pd
+    except Exception as err:
+        err_msgs = Text("\nnumpy did not import properly:\n")
+        for err_arg in err.args:
+            err_msgs.append("\t" + err_arg + "\n")
+        err_msgs.stylize("bold green")
+        return err_msgs
 
 
 def check_shapely():
     try:
-        from shapely.geometry import Polygon
+        from shapely import Polygon
     except Exception as err:
         err_msgs = Text("\nshapely did not import properly:\n")
         for err_arg in err.args:
             err_msgs.append("\t" + err_arg + "\n")
         err_msgs.stylize("bold cyan")
         return err_msgs
 
@@ -236,10 +253,21 @@
         proc.communicate("y\n")
     else:
         msg = Text("No additional installations necessary. Ok.")
         msg.stylize("bold green")
         console.print(msg)
 
 
+def install_pfse_kernel():
+    proc = subprocess.Popen(
+        ["python", "-m", "ipykernel", "install", "--user", "--name", "pfse", "--display-name", "Python 3.10 (pfse)"],
+        stdout=subprocess.PIPE,
+        text=True,
+    )
+    msg = Text("PfSE Jupyter Kernel Installed Successfully")
+    msg.stylize("bold green")
+    console.print(msg)
+
 if __name__ == "__main__":
     install_extra()
+    install_pfse_kernel()
     check_installs()
```

### Comparing `pfse_starterkit-0.2.8/pfse_starterkit/sectionproperties_test.py` & `pfse_starterkit-0.3.0/pfse_starterkit/sectionproperties_test.py`

 * *Files identical despite different names*

### Comparing `pfse_starterkit-0.2.8/pfse_starterkit/vtk_cylinder.py` & `pfse_starterkit-0.3.0/pfse_starterkit/vtk_cylinder.py`

 * *Files identical despite different names*

### Comparing `pfse_starterkit-0.2.8/pyproject.toml` & `pfse_starterkit-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 dependencies = [
     "streamlit",
     "numpy",
     "pandas",
     "openpyxl",
     "lxml",
     "sympy",
-    "shapely",
+    "shapely>=2.0.0",
     "vtk",
     "matplotlib",
     "plotly",
+    "kaleido",
     "sectionproperties",
     "concreteproperties",
-    "pycba",
-    "PyNiteFEA",
+    "pycba>=0.2.0",
+    "PyNiteFEA>=0.0.78",
+    "anastruct",
     "scipy",
     "handcalcs",
     "forallpeople",
     "pytest",
     "ipytest",
     "rich",
     "tqdm",
@@ -36,14 +38,15 @@
     "xlwings",
     "black",
     "jupyterlab",
     "IPython",
     "ipywidgets",
     "ipykernel",
     "jupyterlab-katex",
+    "jupyterlab-mathjax3",
     "nbconvert",
     "pyperclip",
     "typer",
     "magicgui[pyside2]",
     "flit"
 ]
```

### Comparing `pfse_starterkit-0.2.8/PKG-INFO` & `pfse_starterkit-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: pfse_starterkit
-Version: 0.2.8
+Version: 0.3.0
 Summary: A module to designed to perform package installations, and verification of install,
 Author-email: Connor Ferster <connor@structuralpython.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: streamlit
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: openpyxl
 Requires-Dist: lxml
 Requires-Dist: sympy
-Requires-Dist: shapely
+Requires-Dist: shapely>=2.0.0
 Requires-Dist: vtk
 Requires-Dist: matplotlib
 Requires-Dist: plotly
+Requires-Dist: kaleido
 Requires-Dist: sectionproperties
 Requires-Dist: concreteproperties
-Requires-Dist: pycba
-Requires-Dist: PyNiteFEA
+Requires-Dist: pycba>=0.2.0
+Requires-Dist: PyNiteFEA>=0.0.78
+Requires-Dist: anastruct
 Requires-Dist: scipy
 Requires-Dist: handcalcs
 Requires-Dist: forallpeople
 Requires-Dist: pytest
 Requires-Dist: ipytest
 Requires-Dist: rich
 Requires-Dist: tqdm
@@ -30,14 +32,15 @@
 Requires-Dist: xlwings
 Requires-Dist: black
 Requires-Dist: jupyterlab
 Requires-Dist: IPython
 Requires-Dist: ipywidgets
 Requires-Dist: ipykernel
 Requires-Dist: jupyterlab-katex
+Requires-Dist: jupyterlab-mathjax3
 Requires-Dist: nbconvert
 Requires-Dist: pyperclip
 Requires-Dist: typer
 Requires-Dist: magicgui[pyside2]
 Requires-Dist: flit
 Project-URL: Home, https://github.com/connorferster/pfse_starterkit
 
@@ -71,13 +74,14 @@
 * xlwings
 * black
 * jupyterlab
 * IPython
 * ipywidgets
 * ipykernel
 * jupyterlab-katex
+* jupyterlab-mathjax3 (as an option)
 * nbconvert
 * pyperclip
 * typer
 * magicgui[pyside2]
 * flit
```

