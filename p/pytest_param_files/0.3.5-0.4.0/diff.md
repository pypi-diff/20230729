# Comparing `tmp/pytest_param_files-0.3.5.tar.gz` & `tmp/pytest_param_files-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_param_files-0.3.5.tar", last modified: Fri Feb 24 04:08:12 2023, max compression
+gzip compressed data, was "pytest_param_files-0.4.0.tar", last modified: Fri Jul 28 21:33:39 2023, max compression
```

## Comparing `pytest_param_files-0.3.5.tar` & `pytest_param_files-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      760 2023-02-24 04:06:50.184127 pytest_param_files-0.3.5/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1815 2022-01-09 04:33:58.784635 pytest_param_files-0.3.5/.gitignore
--rw-r--r--   0        0        0      672 2022-01-09 05:25:01.375450 pytest_param_files-0.3.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1069 2022-01-09 03:41:51.781932 pytest_param_files-0.3.5/LICENSE
--rw-r--r--   0        0        0     1971 2022-01-09 22:30:10.343627 pytest_param_files-0.3.5/README.md
--rw-r--r--   0        0        0      922 2022-01-09 20:35:04.827078 pytest_param_files-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      133 2023-02-24 04:07:22.852094 pytest_param_files-0.3.5/pytest_param_files/__init__.py
--rw-r--r--   0        0        0     9115 2023-02-24 03:53:45.202635 pytest_param_files-0.3.5/pytest_param_files/main.py
--rw-r--r--   0        0        0       85 2022-01-09 23:01:44.150791 pytest_param_files-0.3.5/tests/fixtures/basic.txt
--rw-r--r--   0        0        0      809 2022-01-09 23:02:01.034350 pytest_param_files-0.3.5/tests/test_basic.py
--rw-r--r--   0        0        0     1339 2022-01-09 21:49:11.204000 pytest_param_files-0.3.5/tests/test_isolated.py
--rw-r--r--   0        0        0      513 2022-01-09 05:32:21.297160 pytest_param_files-0.3.5/tox.ini
--rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 pytest_param_files-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      759 2023-07-28 21:00:39.527097 pytest_param_files-0.4.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1815 2022-01-09 04:33:58.784635 pytest_param_files-0.4.0/.gitignore
+-rw-r--r--   0        0        0      671 2023-07-28 18:00:46.619160 pytest_param_files-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1069 2022-01-09 03:41:51.781932 pytest_param_files-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2360 2023-07-28 20:55:46.001778 pytest_param_files-0.4.0/README.md
+-rw-r--r--   0        0        0      983 2023-07-28 21:18:26.992603 pytest_param_files-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      148 2023-07-28 21:25:27.657433 pytest_param_files-0.4.0/pytest_param_files/__init__.py
+-rw-r--r--   0        0        0    13408 2023-07-28 20:58:38.059962 pytest_param_files-0.4.0/pytest_param_files/main.py
+-rw-r--r--   0        0        0       85 2022-01-09 23:01:44.150791 pytest_param_files-0.4.0/tests/fixtures/basic.txt
+-rw-r--r--   0        0        0      162 2023-07-28 20:50:47.084249 pytest_param_files-0.4.0/tests/fixtures/basic.yaml
+-rw-r--r--   0        0        0     1588 2023-07-28 19:30:04.334791 pytest_param_files-0.4.0/tests/test_basic.py
+-rw-r--r--   0        0        0     2203 2023-07-28 21:16:51.743580 pytest_param_files-0.4.0/tests/test_isolated.py
+-rw-r--r--   0        0        0      460 2023-07-28 21:19:51.787702 pytest_param_files-0.4.0/tox.ini
+-rw-r--r--   0        0        0     3158 1970-01-01 00:00:00.000000 pytest_param_files-0.4.0/PKG-INFO
```

### Comparing `pytest_param_files-0.3.5/.github/workflows/python-package.yml` & `pytest_param_files-0.4.0/.github/workflows/tests.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
 
-name: Python package
+name: Tests
 
 on:
   push:
     branches: [ "main" ]
   pull_request:
     branches: [ "main" ]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `pytest_param_files-0.3.5/.gitignore` & `pytest_param_files-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_param_files-0.3.5/.pre-commit-config.yaml` & `pytest_param_files-0.4.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/psf/black
-    rev: 21.12b0
+    rev: 23.7.0
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
+    rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies:
           - flake8-comprehensions
           - flake8-bugbear
```

### Comparing `pytest_param_files-0.3.5/LICENSE` & `pytest_param_files-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_param_files-0.3.5/README.md` & `pytest_param_files-0.4.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,46 @@
 # pytest-param-files
 
 [![PyPI][pypi-badge]][pypi-link]
 
 A small package to generate parametrized [pytests](https://docs.pytest.org) from external files.
 
-Simply create a text file with the following (`dot`) format:
+Simply create a text file with an available format:
 
+`dot` format (default):
 ```
 [name1] description
 .
 input content
 .
 expected output content
-,
+.
 
 [name2] description
 .
 input content
 .
 expected output content
-,
+.
+```
+
+`yaml` format:
+```yaml
+- title: name1
+  description: description
+  input: |-
+    input content
+  expected: |-
+    expected output content
+- title: name2
+  description: description
+  input: |-
+    input content
+  expected: |-
+    expected output content
 ```
 
 Then, use the `param_file` pytest marker to create a parametrized test:
 
 ```python
 from pathlib import Path
 import pytest
@@ -81,17 +98,17 @@
 
 ```console
 $ pip install -e .
 ```
 
 ## Regenerating expected output on failures
 
-**EXPERIMENTAL**
-
 Running pytest with the `--regen-file-failure` option will regenerate the parameter file with actual output, if any test fails.
 
+Note, currently regeneration of YAML files may not provide the same formatting as the original file, and will not preserve comments.
+
 ## Other formats
 
 TODO ...
 
 [pypi-badge]: https://img.shields.io/pypi/v/pytest_param_files.svg
 [pypi-link]: https://pypi.org/project/pytest_param_files
```

### Comparing `pytest_param_files-0.3.5/pyproject.toml` & `pytest_param_files-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 dynamic = ["version", "description"]
 authors = [{name = "Chris Sewell", email = "chrisj_sewell@hotmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Framework :: Pytest"
-
 ]
 keywords = ["pytest", "parameterized"]
-requires-python = ">=3.7"
-dependencies = ["pytest"]
+requires-python = ">=3.8"
+dependencies = ["pytest", "pyyaml"]
 
 [project.urls]
 Home = "https://github.com/chrisjsewell/pytest-param-files"
 
 [project.entry-points."pytest11"]
 pytest_param_files = "pytest_param_files.main"
 
 [project.optional-dependencies]
-develop = ["black"]
+codecov = ["pytest-cov"]
 
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
```

### Comparing `pytest_param_files-0.3.5/pytest_param_files/main.py` & `pytest_param_files-0.4.0/pytest_param_files/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """Main module"""
+from __future__ import annotations
+
 from dataclasses import dataclass
 import difflib
 from pathlib import Path
 import re
-from typing import TYPE_CHECKING, Any, Iterator, List, Optional, Tuple, Union, cast
+import traceback
+from typing import TYPE_CHECKING, Any, ClassVar, Iterator, Literal, cast
+
+import yaml
 
 if TYPE_CHECKING:
     from _pytest.python import Metafunc
 
 
 def pytest_addoption(parser):
     """Register command line options to pytest."""
@@ -26,15 +31,15 @@
     config.addinivalue_line(
         "markers",
         "param_file(path, fmt=dot, encoding=utf8, **kwargs): "
         "call a test function multiple times, parametrized by a fixture file (Path|str).",
     )
 
 
-def pytest_generate_tests(metafunc: "Metafunc") -> None:
+def pytest_generate_tests(metafunc: Metafunc) -> None:
     """Generate tests for a pytest param_file decorator."""
     for marker in metafunc.definition.iter_markers(name="param_file"):
         param_files_regen = metafunc.config.getoption("param_files_regen")
         fixture_name, file_params, ids = create_parameters(
             *marker.args, **marker.kwargs, regen_on_failure=param_files_regen
         )
         metafunc.parametrize(argnames=fixture_name, argvalues=file_params, ids=ids)
@@ -44,23 +49,23 @@
 class ParamTestData:
     """Data class for a single test."""
 
     line: int
     """The line number in the source file."""
     title: str
     """The title of the test."""
-    description: Optional[str]
+    description: str | None
     """The description of the test."""
     content: Any
     """The input content of the test."""
     expected: Any
     """The expected result of the test."""
     index: int
     """The index of the test in the file."""
-    fmt: "FormatAbstract"
+    fmt: FormatAbstract
     """The format of the source file."""
 
     def assert_expected(self, actual: Any, **kwargs: Any) -> None:
         """Assert the actual result of the test.
 
         :param actual: The actual result of the test.
         :param kwargs: Additional keyword arguments to parse to the format.
@@ -69,28 +74,29 @@
         error = self.fmt.assert_expected(actual, self, **kwargs)
         if error is None:
             return True
         if self.fmt.regen_on_failure:
             # TODO how to cache regeneration until all test parameters are run?
             try:
                 self.fmt.regen_file(self, actual, **kwargs)
-            except Exception as exc:
-                error += f"\nRegeneration failed: {exc}"
+            except Exception:
+                error += f"\nRegeneration failed:\n{traceback.format_exc()}"
+
             else:
                 error += f"\nREGENERATED FILE: {self.fmt.path}"
         raise AssertionError(error)
 
 
 def create_parameters(
-    path: Union[str, Path],
-    fmt: str = "dot",
+    path: str | Path,
+    fmt: Literal["dot", "yaml"] = "dot",
     encoding="utf8",
     fixture_name: str = "file_params",
     regen_on_failure: bool = False,
-) -> Tuple[str, List[ParamTestData], List[str]]:
+) -> tuple[str, list[ParamTestData], list[str]]:
     """Return a pytest parametrize decorator for a fixture file.
 
     :param path: Path to the fixture file.
     :param format: Format of the fixture file.
     :param encoding: Encoding of the fixture file.
     :param fixture_name: Name of the fixture parameter.
 
@@ -98,17 +104,20 @@
     """
     path = Path(path)
     # check if the file exists
     if not path.is_file():
         raise FileNotFoundError(f"File {path} not found.")
 
     # select read format
-    if fmt != "dot":
-        raise NotImplementedError("Currently only dot format is supported.")
-    fmt_inst = DotFormat(path, encoding, regen_on_failure)
+    if fmt == "dot":
+        fmt_inst = DotFormat(path, encoding, regen_on_failure)
+    elif fmt == "yaml":
+        fmt_inst = YamlFormat(path, encoding, regen_on_failure)
+    else:
+        raise NotImplementedError(f"Unknown format {fmt!r}, set to 'dot' or 'yaml'")
 
     # read fixture file
     file_params = list(fmt_inst.read())
 
     # create pytest parametrize ids
     ids = [f"{p.line}-{p.title}" for p in file_params]
 
@@ -138,30 +147,30 @@
 
         :return: List of test data.
         """
         raise NotImplementedError()
 
     def assert_expected(
         self, actual: Any, data: ParamTestData, **kwargs: Any
-    ) -> Optional[str]:
+    ) -> str | None:
         """Assert the actual result matches the expected.
 
         :param actual: Actual result.
         """
         raise NotImplementedError()
 
-    def regen_file(data: ParamTestData, actual: Any, **kwargs: Any) -> None:
+    def regen_file(self, data: ParamTestData, actual: Any, **kwargs: Any) -> None:
         """Regenerate the fixture file."""
-        raise NotImplementedError()
+        raise NotImplementedError("not implemented")
 
 
 class DotFormat(FormatAbstract):
     """Dot file format."""
 
-    name = "dot"
+    name: ClassVar[str] = "dot"
 
     def read(self) -> Iterator[ParamTestData]:
         text = self.path.read_text(encoding=self.encoding)
         tests = []
         section = 0
         last_pos = 0
         lines = text.splitlines(keepends=True)
@@ -192,34 +201,26 @@
 
     def assert_expected(
         self,
         actual: str,
         data: ParamTestData,
         rstrip: bool = False,
         rstrip_lines: bool = False,
-    ) -> Optional[str]:
+    ) -> str | None:
         """Assert the actual result of the test.
 
         :param rstrip: Whether to apply `str.rstrip` to actual and expected before comparing.
         :param rstrip_lines: Whether to apply `str.rstrip`
             to each line of actual and expected before comparing.
-        """
-        expected = cast(str, data.expected)
-        if rstrip:
-            actual = actual.rstrip()
-            expected = expected.rstrip()
-        if rstrip_lines:
-            actual = "\n".join(line.rstrip() for line in actual.splitlines()).rstrip()
-            expected = "\n".join(
-                line.rstrip() for line in expected.splitlines()
-            ).rstrip()
 
-        if actual == expected:
-            return None
-        return self._diff(actual, expected, data)
+        :return: An error message if the actual result does not match the expected result.
+        """
+        return assert_expected_strings(
+            actual, cast(str, data.expected), self.path, data.line, rstrip, rstrip_lines
+        )
 
     def regen_file(
         self,
         data: ParamTestData,
         actual: str,
         rstrip: bool = False,
         rstrip_lines: bool = False,
@@ -247,28 +248,152 @@
                 text.append("\n")
             text.append(".\n")
             text.append("\n")
         if text:
             text = text[:-1]
         self.path.write_text("".join(text), encoding=self.encoding)
 
-    def _diff(self, actual: str, expected: str, data: ParamTestData) -> str:
-        """Return a diff string between actual and expected."""
-        diff_lines = list(
-            difflib.unified_diff(
-                expected.splitlines(keepends=True),
-                actual.splitlines(keepends=True),
-                fromfile=f"{self.path}:{data.line}",
-                tofile="(actual)",
-                lineterm="",
-            )
-        )
-        if len(diff_lines) <= 500:
-            return "actual != expected (use --regen-file-failure)\n" + "".join(
-                diff_lines
+
+class YamlFormat(FormatAbstract):
+    """YAML file format."""
+
+    name: ClassVar[str] = "yaml"
+
+    def read(self) -> Iterator[ParamTestData]:
+        """Read the fixture file and return a list of test data.
+
+        :return: List of test data.
+        """
+        text = self.path.read_text(encoding=self.encoding)
+        node = yaml.compose(text, yaml.SafeLoader)
+        if not isinstance(node, yaml.SequenceNode):
+            raise TypeError(f"Expected sequence, got {type(node)}")
+        data = yaml.safe_load(text)
+        assert len(node.value) == len(data), "YAML node count mismatch"
+        item_node: yaml.Node
+        for index, (item_node, item) in enumerate(zip(node.value, data)):
+            line = item_node.start_mark.line + 1
+            if not isinstance(item, dict):
+                raise TypeError(
+                    f"Expected mapping at line {line}, got {type(item_node)}"
+                )
+            for key in ("title", "content", "expected"):
+                if key not in item:
+                    raise KeyError(f"Missing '{key}' key for item at line {line}")
+            yield ParamTestData(
+                line,
+                item["title"],
+                item.get("description"),
+                item["content"],
+                item["expected"],
+                fmt=self,
+                index=index,
             )
-        else:
-            return (
-                "actual != expected (use --regen-file-failure)\n"
-                f"diff too big to show ({len(diff_lines)}): "
-                f"{self.path}:{data.line}"
+
+    def assert_expected(
+        self,
+        actual: Any,
+        data: ParamTestData,
+        rstrip: bool = False,
+        rstrip_lines: bool = False,
+    ) -> str | None:
+        """Assert the actual result of the test.
+
+        :param rstrip: Whether to apply `str.rstrip` to actual and expected,
+            before comparing (strings only).
+        :param rstrip_lines: Whether to apply `str.rstrip`
+            to each line of actual and expected before comparing (strings only).
+        """
+        expected = data.expected
+
+        if type(actual) != type(expected):
+            return f"actual type {type(actual)} != expected type {type(expected)}"
+
+        if isinstance(actual, str) and isinstance(expected, str):
+            return assert_expected_strings(
+                actual, expected, self.path, data.line, rstrip, rstrip_lines
             )
+
+        if actual == expected:
+            return None
+
+        return (
+            f"actual != expected (use --regen-file-failure)\n"
+            f"actual: {actual}\nexpected: {expected}"
+        )
+
+    def regen_file(self, data: ParamTestData, actual: Any, **kwargs: Any) -> None:
+        """Regenerate the fixture file."""
+        # TODO ideally here we would maintain comments and formatting
+        # perhaps using ruamel.yaml, although that is a pain
+        new = yaml.safe_load(self.path.read_text(encoding=self.encoding))
+        new[data.index]["expected"] = actual
+        text = yaml.dump(
+            new, Dumper=CustomDumper, default_flow_style=False, sort_keys=False
+        )
+        self.path.write_text(text, encoding=self.encoding)
+
+
+def assert_expected_strings(
+    actual: str,
+    expected: str,
+    path: Path,
+    line: int,
+    rstrip: bool = False,
+    rstrip_lines: bool = False,
+) -> str | None:
+    """Assert the actual result of the test.
+
+    :param rstrip: Whether to apply `str.rstrip` to actual and expected before comparing.
+    :param rstrip_lines: Whether to apply `str.rstrip`
+        to each line of actual and expected before comparing.
+
+    :return: An error message if the actual result does not match the expected result.
+    """
+    if rstrip:
+        actual = actual.rstrip()
+        expected = expected.rstrip()
+    if rstrip_lines:
+        actual = "\n".join(line.rstrip() for line in actual.splitlines()).rstrip()
+        expected = "\n".join(line.rstrip() for line in expected.splitlines()).rstrip()
+
+    if actual == expected:
+        return None
+    return diff_strings(actual, expected, path, line)
+
+
+def diff_strings(actual: str, expected: str, path: Path, line: int) -> str:
+    """Return a diff string between actual and expected."""
+    diff_lines = list(
+        difflib.unified_diff(
+            (expected + "\n").splitlines(keepends=True),
+            (actual + "\n").splitlines(keepends=True),
+            fromfile=f"{path}:{line}",
+            tofile="(actual)",
+            lineterm="\n",
+        )
+    )
+    if len(diff_lines) <= 500:
+        return "actual != expected (use --regen-file-failure)\n" + "".join(diff_lines)
+    else:
+        return (
+            "actual != expected (use --regen-file-failure)\n"
+            f"diff too big to show ({len(diff_lines)}): "
+            f"{path}:{line}"
+        )
+
+
+class CustomDumper(yaml.SafeDumper):
+    """Custom YAML dumper."""
+
+    def represent_scalar(self, tag, value, style=None):
+        if style is None:
+            # be a bit more clever about the string style,
+            # to get a more readable output
+            if "\n" in value:
+                style = "|"
+            elif len(value) > 80:
+                style = ">"
+        node = yaml.ScalarNode(tag, value, style=style)
+        if self.alias_key is not None:
+            self.represented_objects[self.alias_key] = node
+        return node
```

### Comparing `pytest_param_files-0.3.5/tests/test_basic.py` & `pytest_param_files-0.4.0/tests/test_basic.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,7 +14,24 @@
     assert file_params.title.startswith("name")
     assert file_params.description == "description"
     assert file_params.content.rstrip() == "Something"
     assert file_params.expected.rstrip() == "Other"
     file_params.assert_expected("Other", rstrip=True)
     with pytest.raises(AssertionError, match="basic.txt"):
         file_params.assert_expected("Otherx", rstrip=True)
+
+
+@pytest.mark.param_file(Path(__file__).parent / "fixtures" / "basic.yaml", fmt="yaml")
+def test_basic_yaml(file_params):
+    """Basic parsing test."""
+    assert isinstance(file_params.line, int)
+    assert isinstance(file_params.title, str)
+    assert isinstance(file_params.description, str)
+    assert isinstance(file_params.content, str)
+    assert isinstance(file_params.expected, str)
+    assert file_params.title.startswith("name")
+    assert file_params.description == "description"
+    assert file_params.content.rstrip() == "Something"
+    # assert file_params.expected.rstrip() == "Other"
+    file_params.assert_expected("Other", rstrip=True)
+    # with pytest.raises(AssertionError, match="basic.yaml"):
+    #     file_params.assert_expected("Otherx", rstrip=True)
```

### Comparing `pytest_param_files-0.3.5/PKG-INFO` & `pytest_param_files-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,67 @@
 Metadata-Version: 2.1
 Name: pytest_param_files
-Version: 0.3.5
+Version: 0.4.0
 Summary: Create pytest parametrize decorators from external files.
 Keywords: pytest,parameterized
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Pytest
 Requires-Dist: pytest
-Requires-Dist: black ; extra == "develop"
+Requires-Dist: pyyaml
+Requires-Dist: pytest-cov ; extra == "codecov"
 Project-URL: Home, https://github.com/chrisjsewell/pytest-param-files
-Provides-Extra: develop
+Provides-Extra: codecov
 
 # pytest-param-files
 
 [![PyPI][pypi-badge]][pypi-link]
 
 A small package to generate parametrized [pytests](https://docs.pytest.org) from external files.
 
-Simply create a text file with the following (`dot`) format:
+Simply create a text file with an available format:
 
+`dot` format (default):
 ```
 [name1] description
 .
 input content
 .
 expected output content
-,
+.
 
 [name2] description
 .
 input content
 .
 expected output content
-,
+.
+```
+
+`yaml` format:
+```yaml
+- title: name1
+  description: description
+  input: |-
+    input content
+  expected: |-
+    expected output content
+- title: name2
+  description: description
+  input: |-
+    input content
+  expected: |-
+    expected output content
 ```
 
 Then, use the `param_file` pytest marker to create a parametrized test:
 
 ```python
 from pathlib import Path
 import pytest
@@ -100,18 +119,18 @@
 
 ```console
 $ pip install -e .
 ```
 
 ## Regenerating expected output on failures
 
-**EXPERIMENTAL**
-
 Running pytest with the `--regen-file-failure` option will regenerate the parameter file with actual output, if any test fails.
 
+Note, currently regeneration of YAML files may not provide the same formatting as the original file, and will not preserve comments.
+
 ## Other formats
 
 TODO ...
 
 [pypi-badge]: https://img.shields.io/pypi/v/pytest_param_files.svg
 [pypi-link]: https://pypi.org/project/pytest_param_files
```

