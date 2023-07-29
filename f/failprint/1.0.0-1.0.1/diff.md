# Comparing `tmp/failprint-1.0.0.tar.gz` & `tmp/failprint-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "failprint-1.0.0.tar", last modified: Fri Jul 28 18:51:31 2023, max compression
+gzip compressed data, was "failprint-1.0.1.tar", last modified: Sat Jul 29 14:29:45 2023, max compression
```

## Comparing `failprint-1.0.0.tar` & `failprint-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      754 2023-07-23 09:32:34.916242 failprint-1.0.0/LICENSE
--rw-r--r--   0        0        0     4818 2023-07-23 09:32:37.209566 failprint-1.0.0/README.md
--rw-r--r--   0        0        0     2740 2023-07-28 18:51:31.162042 failprint-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      525 2023-07-27 15:16:34.103795 failprint-1.0.0/src/failprint/__init__.py
--rw-r--r--   0        0        0      343 2023-07-23 09:32:34.719576 failprint-1.0.0/src/failprint/__main__.py
--rw-r--r--   0        0        0     6008 2023-07-27 15:02:19.138784 failprint-1.0.0/src/failprint/capture.py
--rw-r--r--   0        0        0     6157 2023-07-27 15:02:56.211686 failprint-1.0.0/src/failprint/cli.py
--rw-r--r--   0        0        0     5777 2023-07-27 15:04:10.100820 failprint-1.0.0/src/failprint/formats.py
--rw-r--r--   0        0        0     3061 2023-07-27 15:07:47.014907 failprint-1.0.0/src/failprint/lazy.py
--rw-r--r--   0        0        0     2942 2023-07-27 15:16:34.100461 failprint-1.0.0/src/failprint/process.py
--rw-r--r--   0        0        0        0 2023-07-23 09:32:34.722909 failprint-1.0.0/src/failprint/py.typed
--rw-r--r--   0        0        0     7301 2023-07-28 18:50:05.019854 failprint-1.0.0/src/failprint/runners.py
--rw-r--r--   0        0        0      360 2023-07-27 15:09:15.600507 failprint-1.0.0/src/failprint/types.py
--rw-r--r--   0        0        0      162 2023-07-23 09:32:34.692909 failprint-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0       47 2023-07-23 09:32:34.692909 failprint-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0      873 2023-07-25 17:05:37.815840 failprint-1.0.0/tests/test_capture.py
--rw-r--r--   0        0        0     1000 2023-07-23 09:37:38.267685 failprint-1.0.0/tests/test_cli.py
--rw-r--r--   0        0        0     4242 2023-04-10 14:08:12.815777 failprint-1.0.0/tests/test_formats.py
--rw-r--r--   0        0        0      978 2023-04-10 14:08:12.815777 failprint-1.0.0/tests/test_lazy.py
--rw-r--r--   0        0        0     2213 2023-07-27 15:16:34.103795 failprint-1.0.0/tests/test_process.py
--rw-r--r--   0        0        0    10476 2023-07-27 15:16:34.103795 failprint-1.0.0/tests/test_runners.py
--rw-r--r--   0        0        0     6412 1970-01-01 00:00:00.000000 failprint-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-07-23 09:32:34.916242 failprint-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4821 2023-07-29 13:58:44.682016 failprint-1.0.1/README.md
+-rw-r--r--   0        0        0     2767 2023-07-29 14:29:45.093219 failprint-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      525 2023-07-27 15:16:34.103795 failprint-1.0.1/src/failprint/__init__.py
+-rw-r--r--   0        0        0      343 2023-07-23 09:32:34.719576 failprint-1.0.1/src/failprint/__main__.py
+-rw-r--r--   0        0        0     6200 2023-07-29 14:23:27.097307 failprint-1.0.1/src/failprint/capture.py
+-rw-r--r--   0        0        0     6157 2023-07-27 15:02:56.211686 failprint-1.0.1/src/failprint/cli.py
+-rw-r--r--   0        0        0     5777 2023-07-27 15:04:10.100820 failprint-1.0.1/src/failprint/formats.py
+-rw-r--r--   0        0        0     3061 2023-07-27 15:07:47.014907 failprint-1.0.1/src/failprint/lazy.py
+-rw-r--r--   0        0        0     2942 2023-07-27 15:16:34.100461 failprint-1.0.1/src/failprint/process.py
+-rw-r--r--   0        0        0        0 2023-07-23 09:32:34.722909 failprint-1.0.1/src/failprint/py.typed
+-rw-r--r--   0        0        0     7301 2023-07-28 18:50:05.019854 failprint-1.0.1/src/failprint/runners.py
+-rw-r--r--   0        0        0      360 2023-07-27 15:09:15.600507 failprint-1.0.1/src/failprint/types.py
+-rw-r--r--   0        0        0      162 2023-07-23 09:32:34.692909 failprint-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-23 09:32:34.692909 failprint-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0      873 2023-07-25 17:05:37.815840 failprint-1.0.1/tests/test_capture.py
+-rw-r--r--   0        0        0     1000 2023-07-23 09:37:38.267685 failprint-1.0.1/tests/test_cli.py
+-rw-r--r--   0        0        0     4242 2023-04-10 14:08:12.815777 failprint-1.0.1/tests/test_formats.py
+-rw-r--r--   0        0        0      978 2023-04-10 14:08:12.815777 failprint-1.0.1/tests/test_lazy.py
+-rw-r--r--   0        0        0     2213 2023-07-27 15:16:34.103795 failprint-1.0.1/tests/test_process.py
+-rw-r--r--   0        0        0    10772 2023-07-29 14:24:02.316636 failprint-1.0.1/tests/test_runners.py
+-rw-r--r--   0        0        0     6415 1970-01-01 00:00:00.000000 failprint-1.0.1/PKG-INFO
```

### Comparing `failprint-1.0.0/LICENSE` & `failprint-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `failprint-1.0.0/README.md` & `failprint-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,33 +27,33 @@
 The task runner [`duty`](https://github.com/pawamoy/duty) uses `failprint`,
 allowing you to define tasks in Python and run them with minimalist and beautiful output:
 
 ![demo_duty](demo_duty.svg)
 
 ## Requirements
 
-failprint requires Python 3.6 or above.
+failprint requires Python 3.8 or above.
 
 <details>
-<summary>To install Python 3.6, I recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>
+<summary>To install Python 3.8, I recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>
 
 ```bash
 # install pyenv
 git clone https://github.com/pyenv/pyenv ~/.pyenv
 
 # setup pyenv (you should also put these three lines in .bashrc or similar)
 export PATH="${HOME}/.pyenv/bin:${PATH}"
 export PYENV_ROOT="${HOME}/.pyenv"
 eval "$(pyenv init -)"
 
-# install Python 3.6
-pyenv install 3.6.12
+# install Python 3.8.17
+pyenv install 3.8.17
 
 # make it available globally
-pyenv global system 3.6.12
+pyenv global system 3.8.17
 ```
 </details>
 
 ## Installation
 
 With `pip`:
 ```bash
```

#### html2text {}

```diff
@@ -11,21 +11,21 @@
 `make check` or `make lint` commands? Tired of finding out that standard output
 and error are mixed up in some of them? Simply run your command through
 `failprint`. If it succeeds, nothing is printed. If it fails, standard error is
 printed. Plus other configuration goodies :wink: ## Example You don't want to
 see output when the command succeeds. ![demo](demo.svg) The task runner
 [`duty`](https://github.com/pawamoy/duty) uses `failprint`, allowing you to
 define tasks in Python and run them with minimalist and beautiful output: !
-[demo_duty](demo_duty.svg) ## Requirements failprint requires Python 3.6 or
-above.  To install Python 3.6, I recommend using pyenv. ```bash # install pyenv
+[demo_duty](demo_duty.svg) ## Requirements failprint requires Python 3.8 or
+above.  To install Python 3.8, I recommend using pyenv. ```bash # install pyenv
 git clone https://github.com/pyenv/pyenv ~/.pyenv # setup pyenv (you should
 also put these three lines in .bashrc or similar) export PATH="${HOME}/.pyenv/
 bin:${PATH}" export PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv init -)" #
-install Python 3.6 pyenv install 3.6.12 # make it available globally pyenv
-global system 3.6.12 ```  ## Installation With `pip`: ```bash pip install
+install Python 3.8.17 pyenv install 3.8.17 # make it available globally pyenv
+global system 3.8.17 ```  ## Installation With `pip`: ```bash pip install
 failprint ``` With [`pipx`](https://github.com/pipxproject/pipx): ```bash
 python3.8 -m pip install --user pipx pipx install failprint ``` ## Usage
 ```console % poetry run failprint -h usage: failprint [-h] [-c
 {stdout,stderr,both,none}] [-f {pretty,tap}] [-y | -Y] [-p | -P] [-q | -Q] [-
 s | -S] [-z | -Z] [-n NUMBER] [-t TITLE] COMMAND [COMMAND ...] positional
 arguments: COMMAND optional arguments: -h, --help show this help message and
 exit -c {stdout,stderr,both,none}, --capture {stdout,stderr,both,none} Which
```

### Comparing `failprint-1.0.0/pyproject.toml` & `failprint-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 ]
 dependencies = [
     "ansimarkup~=1.4",
     "jinja2>=2.11, <4",
     "ptyprocess~=0.6; sys_platform != 'win32'",
     "typing-extensions>=4.1; python_version < '3.10'",
 ]
-version = "1.0.0"
+version = "1.0.1"
 
 [project.license]
 text = "ISC"
 
 [project.urls]
 Homepage = "https://pawamoy.github.io/failprint"
 Documentation = "https://pawamoy.github.io/failprint"
@@ -81,15 +81,15 @@
 ci-tests = [
     "failprint[duty,tests]",
 ]
 docs = [
     "black>=23.1",
     "markdown-callouts>=0.2",
     "markdown-exec>=0.5",
-    "mkdocs>=1.3",
+    "mkdocs>=1.5",
     "mkdocs-coverage>=0.2",
     "mkdocs-gen-files>=0.3",
     "mkdocs-git-committers-plugin-2>=1.1",
     "mkdocs-literate-nav>=0.4",
     "mkdocs-material>=7.3",
     "mkdocs-minify-plugin>=0.6.4",
     "mkdocstrings[python]>=0.18",
@@ -103,14 +103,15 @@
 quality = [
     "ruff>=0.0.246",
 ]
 tests = [
     "pytest>=6.2",
     "pytest-cov>=3.0",
     "pytest-randomly>=3.10",
+    "pytest-timeout>=2.1",
     "pytest-xdist>=2.4",
     "hypothesis>=6.13",
 ]
 typing = [
     "mypy>=0.910",
     "types-markdown>=3.3",
     "types-pyyaml>=6.0",
```

### Comparing `failprint-1.0.0/src/failprint/__init__.py` & `failprint-1.0.1/src/failprint/__init__.py`

 * *Files identical despite different names*

### Comparing `failprint-1.0.0/src/failprint/capture.py` & `failprint-1.0.1/src/failprint/capture.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Enumeration of possible output captures."""
 
 from __future__ import annotations
 
 import enum
 import os
 import sys
+import tempfile
 from contextlib import contextmanager
 from io import StringIO
-from typing import TYPE_CHECKING, Iterator, TextIO
+from typing import IO, TYPE_CHECKING, Iterator, TextIO
 
 if TYPE_CHECKING:
     from types import TracebackType
 
 
 class Capture(enum.Enum):
     """An enum to store the different possible output types."""
@@ -97,16 +98,15 @@
     def __init__(self, capture: Capture = Capture.BOTH, stdin: str | None = None) -> None:
         """Initialize the context manager.
 
         Parameters:
             capture: What to capture.
             stdin: Optional input.
         """
-        self._fdr: int = -1
-        self._fdw: int = -1
+        self._temp_file: IO[str] | None = None
         self._capture = capture
         self._devnull: TextIO | None = None
         self._stdin = stdin
         self._saved_stdin: TextIO | None = None
         self._stdout_fd: int = -1
         self._stderr_fd: int = -1
         self._saved_stdout_fd: int = -1
@@ -126,30 +126,32 @@
             self._saved_stdin = sys.stdin
             sys.stdin = StringIO(self._stdin)
 
         # Open devnull if needed.
         if self._capture in {Capture.STDOUT, Capture.STDERR}:
             self._devnull = open(os.devnull, "w")  # noqa: SIM115
 
-        # Create pipe.
-        self._fdr, self._fdw = os.pipe()
+        # Create temporary file.
+        # Initially we used a pipe but it would hang on writes given enough output.
+        self._temp_file = tempfile.TemporaryFile("w+", encoding="utf8", prefix="failprint-")
+        fdw = self._temp_file.fileno()
 
-        # Copy stdout's file descriptor before it is overwritten.
+        # Redirect stdout to temporary file or devnull.
         self._stdout_fd = sys.stdout.fileno()
         self._saved_stdout_fd = os.dup(self._stdout_fd)
         if self._capture in {Capture.BOTH, Capture.STDOUT}:
-            os.dup2(self._fdw, self._stdout_fd)
+            os.dup2(fdw, self._stdout_fd)
         elif self._capture is Capture.STDERR:
             os.dup2(self._devnull.fileno(), self._stdout_fd)  # type: ignore[union-attr]
 
-        # Copy stderr's file descriptor before it is overwritten.
+        # Redirect stderr to temporary file or devnull.
         self._stderr_fd = sys.stderr.fileno()
         self._saved_stderr_fd = os.dup(self._stderr_fd)
         if self._capture in {Capture.BOTH, Capture.STDERR}:
-            os.dup2(self._fdw, self._stderr_fd)
+            os.dup2(fdw, self._stderr_fd)
         elif self._capture is Capture.STDOUT:
             os.dup2(self._devnull.fileno(), self._stderr_fd)  # type: ignore[union-attr]
 
         return self
 
     def __exit__(
         self,
@@ -172,18 +174,19 @@
         if self._devnull is not None:
             self._devnull.close()
 
         # Restore stdout and stderr to their previous values.
         os.dup2(self._saved_stdout_fd, self._stdout_fd)
         os.dup2(self._saved_stderr_fd, self._stderr_fd)
 
-        # Close the writing end of the pipe, read everything from the reading end.
-        os.close(self._fdw)
-        with os.fdopen(self._fdr) as fd:
-            self._output = fd.read()
+        # Read contents from temporary file, close it.
+        if self._temp_file is not None:
+            self._temp_file.seek(0)
+            self._output = self._temp_file.read()
+            self._temp_file.close()
 
     def __str__(self) -> str:
         return self.output
 
     @property
     def output(self) -> str:
         """Captured output.
```

### Comparing `failprint-1.0.0/src/failprint/cli.py` & `failprint-1.0.1/src/failprint/cli.py`

 * *Files identical despite different names*

### Comparing `failprint-1.0.0/src/failprint/formats.py` & `failprint-1.0.1/src/failprint/formats.py`

 * *Files identical despite different names*

### Comparing `failprint-1.0.0/src/failprint/lazy.py` & `failprint-1.0.1/src/failprint/lazy.py`

 * *Files identical despite different names*

### Comparing `failprint-1.0.0/src/failprint/process.py` & `failprint-1.0.1/src/failprint/process.py`

 * *Files identical despite different names*

### Comparing `failprint-1.0.0/src/failprint/runners.py` & `failprint-1.0.1/src/failprint/runners.py`

 * *Files identical despite different names*

### Comparing `failprint-1.0.0/tests/test_capture.py` & `failprint-1.0.1/tests/test_capture.py`

 * *Files identical despite different names*

### Comparing `failprint-1.0.0/tests/test_cli.py` & `failprint-1.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `failprint-1.0.0/tests/test_formats.py` & `failprint-1.0.1/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `failprint-1.0.0/tests/test_lazy.py` & `failprint-1.0.1/tests/test_lazy.py`

 * *Files identical despite different names*

### Comparing `failprint-1.0.0/tests/test_process.py` & `failprint-1.0.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `failprint-1.0.0/tests/test_runners.py` & `failprint-1.0.1/tests/test_runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,7 +351,19 @@
         subprocess.run(["sh", "-c", "echo sh -c echo"])  # noqa: S603,S607
 
     with capsys.disabled(), Capture.BOTH.here() as captured:
         function()
 
     lines = str(captured).rstrip("\n").split("\n")
     assert lines == ["print", "sys stdout write", "os system", "sh -c echo"]
+
+
+@pytest.mark.timeout(5, method="thread")
+def test_capture_large_output() -> None:
+    """Assert we can capture a relatively large output without hanging."""
+
+    def function() -> None:
+        for _ in range(300):
+            print("0" * 300)
+
+    with Capture.BOTH.here():
+        function()
```

### Comparing `failprint-1.0.0/PKG-INFO` & `failprint-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: failprint
-Version: 1.0.0
+Version: 1.0.1
 Summary: Run a command, print its output only if it fails.
 Keywords: cli failure output runner
 Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -63,33 +63,33 @@
 The task runner [`duty`](https://github.com/pawamoy/duty) uses `failprint`,
 allowing you to define tasks in Python and run them with minimalist and beautiful output:
 
 ![demo_duty](demo_duty.svg)
 
 ## Requirements
 
-failprint requires Python 3.6 or above.
+failprint requires Python 3.8 or above.
 
 <details>
-<summary>To install Python 3.6, I recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>
+<summary>To install Python 3.8, I recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>
 
 ```bash
 # install pyenv
 git clone https://github.com/pyenv/pyenv ~/.pyenv
 
 # setup pyenv (you should also put these three lines in .bashrc or similar)
 export PATH="${HOME}/.pyenv/bin:${PATH}"
 export PYENV_ROOT="${HOME}/.pyenv"
 eval "$(pyenv init -)"
 
-# install Python 3.6
-pyenv install 3.6.12
+# install Python 3.8.17
+pyenv install 3.8.17
 
 # make it available globally
-pyenv global system 3.6.12
+pyenv global system 3.8.17
 ```
 </details>
 
 ## Installation
 
 With `pip`:
 ```bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: failprint Version: 1.0.0 Summary: Run a command,
+Metadata-Version: 2.1 Name: failprint Version: 1.0.1 Summary: Run a command,
 print its output only if it fails. Keywords: cli failure output runner Author-
 Email: TimothÃ©e Mazzucotelli
 pm.me> License: ISC Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -33,46 +33,46 @@
 Tired of finding out that standard output and error are mixed up in some of
 them? Simply run your command through `failprint`. If it succeeds, nothing is
 printed. If it fails, standard error is printed. Plus other configuration
 goodies :wink: ## Example You don't want to see output when the command
 succeeds. ![demo](demo.svg) The task runner [`duty`](https://github.com/
 pawamoy/duty) uses `failprint`, allowing you to define tasks in Python and run
 them with minimalist and beautiful output: ![demo_duty](demo_duty.svg) ##
-Requirements failprint requires Python 3.6 or above.  To install Python 3.6, I
+Requirements failprint requires Python 3.8 or above.  To install Python 3.8, I
 recommend using pyenv. ```bash # install pyenv git clone https://github.com/
 pyenv/pyenv ~/.pyenv # setup pyenv (you should also put these three lines in
 .bashrc or similar) export PATH="${HOME}/.pyenv/bin:${PATH}" export
-PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv init -)" # install Python 3.6 pyenv
-install 3.6.12 # make it available globally pyenv global system 3.6.12 ```  ##
-Installation With `pip`: ```bash pip install failprint ``` With [`pipx`](https:
-//github.com/pipxproject/pipx): ```bash python3.8 -m pip install --user pipx
-pipx install failprint ``` ## Usage ```console % poetry run failprint -h usage:
-failprint [-h] [-c {stdout,stderr,both,none}] [-f {pretty,tap}] [-y | -Y] [-p |
--P] [-q | -Q] [-s | -S] [-z | -Z] [-n NUMBER] [-t TITLE] COMMAND [COMMAND ...]
-positional arguments: COMMAND optional arguments: -h, --help show this help
-message and exit -c {stdout,stderr,both,none}, --capture
-{stdout,stderr,both,none} Which output to capture. Colors are supported with
-'both' only, unless the command has a 'force color' option. -f {pretty,tap}, --
-format {pretty,tap} Output format. Pass your own Jinja2 template as a string
-with '-f custom=TEMPLATE'. Available variables: command, title (command or
-title passed with -t), code (exit status), success (boolean), failure
-(boolean), number (command number passed with -n), output (command output),
-nofail (boolean), quiet (boolean), silent (boolean). Available filters: indent
-(textwrap.indent). -y, --pty Enable the use of a pseudo-terminal. PTY doesn't
-allow programs to use standard input. -Y, --no-pty Disable the use of a pseudo-
-terminal. PTY doesn't allow programs to use standard input. -p, --progress
-Print progress while running a command. -P, --no-progress Don't print progress
-while running a command. -q, --quiet Don't print the command output, even if it
-failed. -Q, --no-quiet Print the command output when it fails. -s, --silent
-Don't print anything. -S, --no-silent Print output as usual. -z, --zero, --
-nofail Don't fail. Always return a success (0) exit code. -Z, --no-zero, --
-strict Return the original exit code. -n NUMBER, --number NUMBER Command
-number. Useful for the 'tap' format. -t TITLE, --title TITLE Command title.
-Default is the command itself. ``` ```python from failprint.runners import run
-cmd = "echo hello" exit_code = run( cmd, # str, list of str, or Python callable
-args=None, # args for callable kwargs=None, # kwargs for callable number=1, #
-command number, useful for tap format capture=None, # stdout, stderr, both,
-none, True or False title=None, # command title fmt=None, # pretty, tap, or
-custom="MY_CUSTOM_FORMAT" pty=False, # use a PTY progress=True, # print the
-"progress" template before running the command nofail=False, # always return
-zero quiet=False, # don't print output when the command fails silent=False, #
-don't print anything ) ```
+PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv init -)" # install Python 3.8.17
+pyenv install 3.8.17 # make it available globally pyenv global system 3.8.17
+```  ## Installation With `pip`: ```bash pip install failprint ``` With
+[`pipx`](https://github.com/pipxproject/pipx): ```bash python3.8 -m pip install
+--user pipx pipx install failprint ``` ## Usage ```console % poetry run
+failprint -h usage: failprint [-h] [-c {stdout,stderr,both,none}] [-f
+{pretty,tap}] [-y | -Y] [-p | -P] [-q | -Q] [-s | -S] [-z | -Z] [-n NUMBER] [-
+t TITLE] COMMAND [COMMAND ...] positional arguments: COMMAND optional
+arguments: -h, --help show this help message and exit -c
+{stdout,stderr,both,none}, --capture {stdout,stderr,both,none} Which output to
+capture. Colors are supported with 'both' only, unless the command has a 'force
+color' option. -f {pretty,tap}, --format {pretty,tap} Output format. Pass your
+own Jinja2 template as a string with '-f custom=TEMPLATE'. Available variables:
+command, title (command or title passed with -t), code (exit status), success
+(boolean), failure (boolean), number (command number passed with -n), output
+(command output), nofail (boolean), quiet (boolean), silent (boolean).
+Available filters: indent (textwrap.indent). -y, --pty Enable the use of a
+pseudo-terminal. PTY doesn't allow programs to use standard input. -Y, --no-pty
+Disable the use of a pseudo-terminal. PTY doesn't allow programs to use
+standard input. -p, --progress Print progress while running a command. -P, --
+no-progress Don't print progress while running a command. -q, --quiet Don't
+print the command output, even if it failed. -Q, --no-quiet Print the command
+output when it fails. -s, --silent Don't print anything. -S, --no-silent Print
+output as usual. -z, --zero, --nofail Don't fail. Always return a success (0)
+exit code. -Z, --no-zero, --strict Return the original exit code. -n NUMBER, --
+number NUMBER Command number. Useful for the 'tap' format. -t TITLE, --title
+TITLE Command title. Default is the command itself. ``` ```python from
+failprint.runners import run cmd = "echo hello" exit_code = run( cmd, # str,
+list of str, or Python callable args=None, # args for callable kwargs=None, #
+kwargs for callable number=1, # command number, useful for tap format
+capture=None, # stdout, stderr, both, none, True or False title=None, # command
+title fmt=None, # pretty, tap, or custom="MY_CUSTOM_FORMAT" pty=False, # use a
+PTY progress=True, # print the "progress" template before running the command
+nofail=False, # always return zero quiet=False, # don't print output when the
+command fails silent=False, # don't print anything ) ```
```

