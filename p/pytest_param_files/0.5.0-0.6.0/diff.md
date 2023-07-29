# Comparing `tmp/pytest_param_files-0.5.0.tar.gz` & `tmp/pytest_param_files-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_param_files-0.5.0.tar", last modified: Fri Jul 28 23:30:46 2023, max compression
+gzip compressed data, was "pytest_param_files-0.6.0.tar", last modified: Sat Jul 29 12:28:35 2023, max compression
```

## Comparing `pytest_param_files-0.5.0.tar` & `pytest_param_files-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      759 2023-07-28 21:00:39.527097 pytest_param_files-0.5.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1815 2022-01-09 04:33:58.784635 pytest_param_files-0.5.0/.gitignore
--rw-r--r--   0        0        0      671 2023-07-28 18:00:46.619160 pytest_param_files-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1069 2022-01-09 03:41:51.781932 pytest_param_files-0.5.0/LICENSE
--rw-r--r--   0        0        0     2362 2023-07-28 23:26:19.449076 pytest_param_files-0.5.0/README.md
--rw-r--r--   0        0        0      983 2023-07-28 21:18:26.992603 pytest_param_files-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      148 2023-07-28 23:15:53.821074 pytest_param_files-0.5.0/pytest_param_files/__init__.py
--rw-r--r--   0        0        0    13444 2023-07-28 23:26:33.369320 pytest_param_files-0.5.0/pytest_param_files/main.py
--rw-r--r--   0        0        0       85 2022-01-09 23:01:44.150791 pytest_param_files-0.5.0/tests/fixtures/basic.txt
--rw-r--r--   0        0        0      146 2023-07-28 23:27:52.109902 pytest_param_files-0.5.0/tests/fixtures/basic.yaml
--rw-r--r--   0        0        0     1582 2023-07-28 23:24:23.685422 pytest_param_files-0.5.0/tests/test_basic.py
--rw-r--r--   0        0        0     2203 2023-07-28 21:16:51.743580 pytest_param_files-0.5.0/tests/test_isolated.py
--rw-r--r--   0        0        0      460 2023-07-28 21:19:51.787702 pytest_param_files-0.5.0/tox.ini
--rw-r--r--   0        0        0     3160 1970-01-01 00:00:00.000000 pytest_param_files-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      759 2023-07-28 21:00:39.527097 pytest_param_files-0.6.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1815 2022-01-09 04:33:58.784635 pytest_param_files-0.6.0/.gitignore
+-rw-r--r--   0        0        0      671 2023-07-28 18:00:46.619160 pytest_param_files-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1069 2022-01-09 03:41:51.781932 pytest_param_files-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2228 2023-07-29 12:21:12.561838 pytest_param_files-0.6.0/README.md
+-rw-r--r--   0        0        0      994 2023-07-29 12:20:50.587839 pytest_param_files-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      148 2023-07-29 12:25:16.371545 pytest_param_files-0.6.0/pytest_param_files/__init__.py
+-rw-r--r--   0        0        0    13463 2023-07-29 12:24:21.445811 pytest_param_files-0.6.0/pytest_param_files/main.py
+-rw-r--r--   0        0        0       85 2022-01-09 23:01:44.150791 pytest_param_files-0.6.0/tests/fixtures/basic.txt
+-rw-r--r--   0        0        0      165 2023-07-29 12:16:44.502302 pytest_param_files-0.6.0/tests/fixtures/basic.yaml
+-rw-r--r--   0        0        0     1582 2023-07-29 12:16:58.993942 pytest_param_files-0.6.0/tests/test_basic.py
+-rw-r--r--   0        0        0     2203 2023-07-28 21:16:51.743580 pytest_param_files-0.6.0/tests/test_isolated.py
+-rw-r--r--   0        0        0      460 2023-07-28 21:19:51.787702 pytest_param_files-0.6.0/tox.ini
+-rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 pytest_param_files-0.6.0/PKG-INFO
```

### Comparing `pytest_param_files-0.5.0/.github/workflows/tests.yml` & `pytest_param_files-0.6.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pytest_param_files-0.5.0/.gitignore` & `pytest_param_files-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_param_files-0.5.0/.pre-commit-config.yaml` & `pytest_param_files-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest_param_files-0.5.0/LICENSE` & `pytest_param_files-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_param_files-0.5.0/README.md` & `pytest_param_files-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -100,15 +100,13 @@
 $ pip install -e .
 ```
 
 ## Regenerating expected output on failures
 
 Running pytest with the `--regen-file-failure` option will regenerate the parameter file with actual output, if any test fails.
 
-Note, currently regeneration of YAML files may not provide the same formatting as the original file, and will not preserve comments.
-
 ## Other formats
 
 TODO ...
 
 [pypi-badge]: https://img.shields.io/pypi/v/pytest_param_files.svg
 [pypi-link]: https://pypi.org/project/pytest_param_files
```

### Comparing `pytest_param_files-0.5.0/pyproject.toml` & `pytest_param_files-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Framework :: Pytest"
 ]
 keywords = ["pytest", "parameterized"]
 requires-python = ">=3.8"
-dependencies = ["pytest", "pyyaml"]
+dependencies = ["pytest", "ruamel.yaml>=0.15"]
 
 [project.urls]
 Home = "https://github.com/chrisjsewell/pytest-param-files"
 
 [project.entry-points."pytest11"]
 pytest_param_files = "pytest_param_files.main"
```

### Comparing `pytest_param_files-0.5.0/pytest_param_files/main.py` & `pytest_param_files-0.6.0/pytest_param_files/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Main module"""
 from __future__ import annotations
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 import difflib
 from pathlib import Path
 import re
 import traceback
 from typing import TYPE_CHECKING, Any, ClassVar, Iterator, Literal, cast
 
-import yaml
+from ruamel.yaml import YAML, MappingNode, Node
 
 if TYPE_CHECKING:
     from _pytest.python import Metafunc
 
 
 def pytest_addoption(parser):
     """Register command line options to pytest."""
@@ -59,14 +59,16 @@
     """The input content of the test."""
     expected: Any
     """The expected result of the test."""
     index: int
     """The index of the test in the file."""
     fmt: FormatAbstract
     """The format of the source file."""
+    extra: dict[str, Any] = field(default_factory=dict)
+    """Additional data for the test."""
 
     def assert_expected(self, actual: Any, **kwargs: Any) -> None:
         """Assert the actual result of the test.
 
         :param actual: The actual result of the test.
         :param kwargs: Additional keyword arguments to parse to the format.
         """
@@ -260,20 +262,21 @@
 
     def read(self) -> Iterator[ParamTestData]:
         """Read the fixture file and return a list of test data.
 
         :return: List of test data.
         """
         text = self.path.read_text(encoding=self.encoding)
-        node = yaml.compose(text, yaml.SafeLoader)
-        if not isinstance(node, yaml.MappingNode):
+        yaml = YAML(typ="safe")
+        node = yaml.compose(text)
+        if not isinstance(node, MappingNode):
             raise TypeError(f"Expected sequence, got {type(node)}")
-        data: dict = yaml.safe_load(text)
+        data: dict = YAML(typ="safe").load(text)
         assert len(node.value) == len(data), "YAML node count mismatch"
-        title_node: yaml.Node
+        title_node: Node
         for index, ((title_node, _), (title, item)) in enumerate(
             zip(node.value, data.items())
         ):
             line = title_node.start_mark.line + 1
             if not isinstance(item, dict):
                 raise TypeError(
                     f"Expected mapping value at line {line}, got {type(item)}"
@@ -285,14 +288,15 @@
                 line,
                 title,
                 item.get("description"),
                 item["content"],
                 item["expected"],
                 fmt=self,
                 index=index,
+                extra=item,
             )
 
     def assert_expected(
         self,
         actual: Any,
         data: ParamTestData,
         rstrip: bool = False,
@@ -321,22 +325,18 @@
         return (
             f"actual != expected (use --regen-file-failure)\n"
             f"actual: {actual}\nexpected: {expected}"
         )
 
     def regen_file(self, data: ParamTestData, actual: Any, **kwargs: Any) -> None:
         """Regenerate the fixture file."""
-        # TODO ideally here we would maintain comments and formatting
-        # perhaps using ruamel.yaml, although that is a pain
-        new = yaml.safe_load(self.path.read_text(encoding=self.encoding))
+        new = YAML(typ="rt").load(self.path.read_text(encoding=self.encoding))
         new[data.title]["expected"] = actual
-        text = yaml.dump(
-            new, Dumper=CustomDumper, default_flow_style=False, sort_keys=False
-        )
-        self.path.write_text(text, encoding=self.encoding)
+        with self.path.open("w", encoding=self.encoding) as handle:
+            YAML(typ="rt").dump(new, handle)
 
 
 def assert_expected_strings(
     actual: str,
     expected: str,
     path: Path,
     line: int,
@@ -380,22 +380,22 @@
         return (
             "actual != expected (use --regen-file-failure)\n"
             f"diff too big to show ({len(diff_lines)}): "
             f"{path}:{line}"
         )
 
 
-class CustomDumper(yaml.SafeDumper):
-    """Custom YAML dumper."""
+# class CustomDumper(yaml.SafeDumper):
+#     """Custom YAML dumper."""
 
-    def represent_scalar(self, tag, value, style=None):
-        if style is None:
-            # be a bit more clever about the string style,
-            # to get a more readable output
-            if "\n" in value:
-                style = "|"
-            elif len(value) > 80:
-                style = ">"
-        node = yaml.ScalarNode(tag, value, style=style)
-        if self.alias_key is not None:
-            self.represented_objects[self.alias_key] = node
-        return node
+#     def represent_scalar(self, tag, value, style=None):
+#         if style is None:
+#             # be a bit more clever about the string style,
+#             # to get a more readable output
+#             if "\n" in value:
+#                 style = "|"
+#             elif len(value) > 80:
+#                 style = ">"
+#         node = yaml.ScalarNode(tag, value, style=style)
+#         if self.alias_key is not None:
+#             self.represented_objects[self.alias_key] = node
+#         return node
```

### Comparing `pytest_param_files-0.5.0/tests/test_basic.py` & `pytest_param_files-0.6.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pytest_param_files-0.5.0/tests/test_isolated.py` & `pytest_param_files-0.6.0/tests/test_isolated.py`

 * *Files identical despite different names*

### Comparing `pytest_param_files-0.5.0/PKG-INFO` & `pytest_param_files-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pytest_param_files
-Version: 0.5.0
+Version: 0.6.0
 Summary: Create pytest parametrize decorators from external files.
 Keywords: pytest,parameterized
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Pytest
 Requires-Dist: pytest
-Requires-Dist: pyyaml
+Requires-Dist: ruamel.yaml>=0.15
 Requires-Dist: pytest-cov ; extra == "codecov"
 Project-URL: Home, https://github.com/chrisjsewell/pytest-param-files
 Provides-Extra: codecov
 
 # pytest-param-files
 
 [![PyPI][pypi-badge]][pypi-link]
@@ -121,16 +121,14 @@
 $ pip install -e .
 ```
 
 ## Regenerating expected output on failures
 
 Running pytest with the `--regen-file-failure` option will regenerate the parameter file with actual output, if any test fails.
 
-Note, currently regeneration of YAML files may not provide the same formatting as the original file, and will not preserve comments.
-
 ## Other formats
 
 TODO ...
 
 [pypi-badge]: https://img.shields.io/pypi/v/pytest_param_files.svg
 [pypi-link]: https://pypi.org/project/pytest_param_files
```

