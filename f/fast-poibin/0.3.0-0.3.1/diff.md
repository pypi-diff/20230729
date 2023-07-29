# Comparing `tmp/fast_poibin-0.3.0.tar.gz` & `tmp/fast_poibin-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_poibin-0.3.0.tar", max compression
+gzip compressed data, was "fast_poibin-0.3.1.tar", max compression
```

## Comparing `fast_poibin-0.3.0.tar` & `fast_poibin-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      369 2023-01-08 23:12:58.424504 fast_poibin-0.3.0/fast_poibin/__init__.py
--rw-r--r--   0        0        0     2204 2023-05-12 21:50:23.988697 fast_poibin-0.3.0/fast_poibin/check_accuracy.py
--rw-r--r--   0        0        0     5593 2023-05-12 20:58:01.085858 fast_poibin-0.3.0/fast_poibin/pmf.py
--rw-r--r--   0        0        0     3387 2023-05-12 22:46:57.706988 fast_poibin-0.3.0/fast_poibin/poibin.py
--rw-r--r--   0        0        0        0 2023-01-08 23:02:33.444285 fast_poibin-0.3.0/fast_poibin/py.typed
--rw-r--r--   0        0        0    16725 2023-01-07 04:37:14.459723 fast_poibin-0.3.0/LICENSE
--rw-r--r--   0        0        0     1504 2023-05-12 22:47:47.157221 fast_poibin-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1005 2023-05-12 22:46:57.705989 fast_poibin-0.3.0/README.md
--rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 fast_poibin-0.3.0/setup.py
--rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 fast_poibin-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      369 2023-01-08 23:12:58.424504 fast_poibin-0.3.1/fast_poibin/__init__.py
+-rw-r--r--   0        0        0     2204 2023-05-12 21:50:23.988697 fast_poibin-0.3.1/fast_poibin/check_accuracy.py
+-rw-r--r--   0        0        0     5593 2023-05-12 20:58:01.085858 fast_poibin-0.3.1/fast_poibin/pmf.py
+-rw-r--r--   0        0        0     3431 2023-07-29 12:38:05.257062 fast_poibin-0.3.1/fast_poibin/poibin.py
+-rw-r--r--   0        0        0        0 2023-01-08 23:02:33.444285 fast_poibin-0.3.1/fast_poibin/py.typed
+-rw-r--r--   0        0        0    16725 2023-01-07 04:37:14.459723 fast_poibin-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1503 2023-07-29 12:53:34.916251 fast_poibin-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1008 2023-05-12 22:54:10.047199 fast_poibin-0.3.1/README.md
+-rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 fast_poibin-0.3.1/setup.py
+-rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 fast_poibin-0.3.1/PKG-INFO
```

### Comparing `fast_poibin-0.3.0/fast_poibin/check_accuracy.py` & `fast_poibin-0.3.1/fast_poibin/check_accuracy.py`

 * *Files identical despite different names*

### Comparing `fast_poibin-0.3.0/fast_poibin/pmf.py` & `fast_poibin-0.3.1/fast_poibin/pmf.py`

 * *Files identical despite different names*

### Comparing `fast_poibin-0.3.0/fast_poibin/poibin.py` & `fast_poibin-0.3.1/fast_poibin/poibin.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,17 +50,21 @@
         Statistics & Data Analysis. 122. 10.1016/j.csda.2018.01.007.
 
         A downside of this approach is numerical precision. Since convolution by FFT
         is unreliable in the world under the float epsilon (i.e. 2^-52 ~ 2 * 10^-16),
         the relative errors of the computed PMF could be large though it is still not
         bad w.r.t. the absolute errors. For details, please see the following issue:
         https://github.com/privet-kitty/fast-poibin/issues/9. For situations where the
-        relative precision is required, you may want to use `dp` mode instead. You
-        should also note that neither mode can express a probability mass below the
-        least positive double float (~ 5 * 10^-324).
+        relative precision is required, you may want to use `dp` mode instead, whose
+        time complexity is O(N^2).
+
+        You should also note that neither mode can express a probability mass below
+        the least positive double float (~ 5 * 10^-324).
+
+
     """
 
     def __init__(
         self, probabilities: FloatSequence, mode: Union[Literal["mixed"], Literal["dp"]] = "mixed"
     ) -> None:
         """
         Args:
```

### Comparing `fast_poibin-0.3.0/LICENSE` & `fast_poibin-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_poibin-0.3.0/pyproject.toml` & `fast_poibin-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 [tool.poetry]
 name = "fast-poibin"
-version = "0.3.0"
+version = "0.3.1"
 description = "Package for computing PMF and CDF of Poisson binomial distribution."
 authors = ["Hugo Sansaqua <privet.kitty99@gmail.com>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository = "https://github.com/privet-kitty/fast-poibin"
 documentation = "https://privet-kitty.github.io/fast-poibin/"
-packages = [{include = "fast_poibin"}]
+packages = [{ include = "fast_poibin" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.23.0"
 numba = "^0.57.0"
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^0.991"
+mypy = "^1.4.1"
 flake8 = "^5.0.4"
 black = "^22.12.0"
 isort = "^5.11.4"
 poethepoet = "^0.17.1"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
-coverage = {extras = ["toml"], version = "^7.0.3"}
+coverage = { extras = ["toml"], version = "^7.0.3" }
 pytest-mock = "^3.10.0"
 sphinx-rtd-theme = "1.2.0rc2"
 Sphinx = "^6.1.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 strict = true
 follow_imports = "silent"
 ignore_missing_imports = true
-python_version = "3.9"
+python_version = "3.10"
 show_column_numbers = true
 
 [tool.black]
 line-length = 100
 exclude = '''
 (
     .venv
@@ -54,16 +54,14 @@
 line_length = 100
 multi_line_output = 3
 use_parentheses = true
 ensure_newline_before_comments = true
 force_grid_wrap = 0
 
 [tool.coverage.report]
-exclude_lines = [
-    "if __name__ == .__main__.:"
-]
+exclude_lines = ["if __name__ == .__main__.:"]
 
 [tool.poe.tasks]
 lint = "flake8 fast_poibin tests"
 test = "pytest --cov=fast_poibin"
 type-check = "mypy fast_poibin tests"
 docs = "sphinx-build docs docs/_build"
```

### Comparing `fast_poibin-0.3.0/README.md` & `fast_poibin-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,19 @@
 - API Reference: https://privet-kitty.github.io/fast-poibin/
 - Repository: https://github.com/privet-kitty/fast-poibin/
 
 
 ## Installation
 
 
-
 ```bash
 pip install fast-poibin
 ```
 
-
-You need Python version 3.8 or later.
+Python versions 3.8 to 3.11 are supported.
 
 ## Basic Usage
 
 
 ```python
 >>> from fast_poibin import PoiBin
 >>> poibin = PoiBin([0.1, 0.2, 0.2])
```

### Comparing `fast_poibin-0.3.0/setup.py` & `fast_poibin-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['numba>=0.57.0,<0.58.0', 'numpy>=1.23.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'fast-poibin',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Package for computing PMF and CDF of Poisson binomial distribution.',
-    'long_description': '# fast-poibin\n\n[![Build Status](https://github.com/privet-kitty/fast-poibin/workflows/CI/badge.svg)](https://github.com/privet-kitty/fast-poibin/actions)\n[![Coverage Status](https://coveralls.io/repos/github/privet-kitty/fast-poibin/badge.svg?branch=main)](https://coveralls.io/github/privet-kitty/fast-poibin?branch=main)\n[![PyPI Version](https://img.shields.io/pypi/v/fast-poibin)](https://pypi.org/project/fast-poibin/)\n\n\nfast-poibin is a Python package for efficiently computing PMF or CDF of Poisson binomial distribution.\n\n\n- API Reference: https://privet-kitty.github.io/fast-poibin/\n- Repository: https://github.com/privet-kitty/fast-poibin/\n\n\n## Installation\n\n\n\n```bash\npip install fast-poibin\n```\n\n\nYou need Python version 3.8 or later.\n\n## Basic Usage\n\n\n```python\n>>> from fast_poibin import PoiBin\n>>> poibin = PoiBin([0.1, 0.2, 0.2])\n>>> poibin.pmf\narray([0.576, 0.352, 0.068, 0.004])\n>>> poibin.cdf\narray([0.576, 0.928, 0.996, 1.   ])\n```\n\n\n\n\n## Copyright\n\nCopyright (c) 2023 Hugo Sansaqua.\n',
+    'long_description': '# fast-poibin\n\n[![Build Status](https://github.com/privet-kitty/fast-poibin/workflows/CI/badge.svg)](https://github.com/privet-kitty/fast-poibin/actions)\n[![Coverage Status](https://coveralls.io/repos/github/privet-kitty/fast-poibin/badge.svg?branch=main)](https://coveralls.io/github/privet-kitty/fast-poibin?branch=main)\n[![PyPI Version](https://img.shields.io/pypi/v/fast-poibin)](https://pypi.org/project/fast-poibin/)\n\n\nfast-poibin is a Python package for efficiently computing PMF or CDF of Poisson binomial distribution.\n\n\n- API Reference: https://privet-kitty.github.io/fast-poibin/\n- Repository: https://github.com/privet-kitty/fast-poibin/\n\n\n## Installation\n\n\n```bash\npip install fast-poibin\n```\n\nPython versions 3.8 to 3.11 are supported.\n\n## Basic Usage\n\n\n```python\n>>> from fast_poibin import PoiBin\n>>> poibin = PoiBin([0.1, 0.2, 0.2])\n>>> poibin.pmf\narray([0.576, 0.352, 0.068, 0.004])\n>>> poibin.cdf\narray([0.576, 0.928, 0.996, 1.   ])\n```\n\n\n\n\n## Copyright\n\nCopyright (c) 2023 Hugo Sansaqua.\n',
     'author': 'Hugo Sansaqua',
     'author_email': 'privet.kitty99@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/privet-kitty/fast-poibin',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fast_poibin-0.3.0/PKG-INFO` & `fast_poibin-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-poibin
-Version: 0.3.0
+Version: 0.3.1
 Summary: Package for computing PMF and CDF of Poisson binomial distribution.
 Home-page: https://github.com/privet-kitty/fast-poibin
 License: MPL-2.0
 Author: Hugo Sansaqua
 Author-email: privet.kitty99@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
@@ -32,21 +32,19 @@
 - API Reference: https://privet-kitty.github.io/fast-poibin/
 - Repository: https://github.com/privet-kitty/fast-poibin/
 
 
 ## Installation
 
 
-
 ```bash
 pip install fast-poibin
 ```
 
-
-You need Python version 3.8 or later.
+Python versions 3.8 to 3.11 are supported.
 
 ## Basic Usage
 
 
 ```python
 >>> from fast_poibin import PoiBin
 >>> poibin = PoiBin([0.1, 0.2, 0.2])
```

