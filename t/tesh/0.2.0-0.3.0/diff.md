# Comparing `tmp/tesh-0.2.0.tar.gz` & `tmp/tesh-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesh-0.2.0.tar", max compression
+gzip compressed data, was "tesh-0.3.0.tar", max compression
```

## Comparing `tesh-0.2.0.tar` & `tesh-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
--rw-r--r--   0        0        0     1068 2022-12-30 14:07:11.106563 tesh-0.2.0/LICENSE
--rw-r--r--   0        0        0     7942 2022-12-30 14:07:11.106563 tesh-0.2.0/README.md
--rw-r--r--   0        0        0     1862 2022-12-30 14:07:11.106563 tesh-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2081 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/__init__.py
--rw-r--r--   0        0        0      396 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/changedir.py
--rw-r--r--   0        0        0     6727 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/extract.py
--rw-r--r--   0        0        0     5129 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/test.py
--rw-r--r--   0        0        0       35 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/__init__.py
--rw-r--r--   0        0        0       94 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/fixtures/debug.md
--rw-r--r--   0        0        0        0 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/fixtures/empty_folder/.gitkeep
--rw-r--r--   0        0        0      165 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/fixtures/exitcodes.md
--rw-r--r--   0        0        0      208 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/fixtures/exitcodes_multipleblocks.md
--rw-r--r--   0        0        0      116 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/fixtures/fail.md
--rw-r--r--   0        0        0      157 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/fixtures/fixture.md
--rw-r--r--   0        0        0       77 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/fixtures/folder/simple.md
--rw-r--r--   0        0        0      239 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/fixtures/multiple_codeblocks.md
--rw-r--r--   0        0        0     1340 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/fixtures/no_codeblocks.md
--rw-r--r--   0        0        0      133 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/fixtures/prompt.md
--rw-r--r--   0        0        0      113 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/fixtures/setup.md
--rw-r--r--   0        0        0       17 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/fixtures/setup.sh
--rw-r--r--   0        0        0      136 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/fixtures/setup_fail.md
--rw-r--r--   0        0        0      110 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/fixtures/timeout.md
--rw-r--r--   0        0        0     1137 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/test_extract.py
--rw-r--r--   0        0        0     6686 2022-12-30 14:07:11.106563 tesh-0.2.0/src/tesh/tests/test_tesh.py
--rw-r--r--   0        0        0     9083 1970-01-01 00:00:00.000000 tesh-0.2.0/setup.py
--rw-r--r--   0        0        0     8433 1970-01-01 00:00:00.000000 tesh-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-29 08:30:14.937479 tesh-0.3.0/LICENSE
+-rw-r--r--   0        0        0     8165 2023-07-29 08:30:14.937479 tesh-0.3.0/README.md
+-rw-r--r--   0        0        0     1625 2023-07-29 08:30:14.941479 tesh-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2081 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/changedir.py
+-rw-r--r--   0        0        0     6842 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/extract.py
+-rw-r--r--   0        0        0     7219 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/test.py
+-rw-r--r--   0        0        0       35 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/__init__.py
+-rw-r--r--   0        0        0       94 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/debug.md
+-rw-r--r--   0        0        0        0 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/empty_folder/.gitkeep
+-rw-r--r--   0        0        0      165 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/exitcodes.md
+-rw-r--r--   0        0        0      208 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/exitcodes_multipleblocks.md
+-rw-r--r--   0        0        0      116 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/fail.md
+-rw-r--r--   0        0        0      157 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/fixture.md
+-rw-r--r--   0        0        0       85 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/folder/simple.md
+-rw-r--r--   0        0        0     2137 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/long_command.md
+-rw-r--r--   0        0        0      173 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/multiline_command.md
+-rw-r--r--   0        0        0      239 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/multiple_codeblocks.md
+-rw-r--r--   0        0        0     1340 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/no_codeblocks.md
+-rw-r--r--   0        0        0      133 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/prompt.md
+-rw-r--r--   0        0        0      113 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/setup.md
+-rw-r--r--   0        0        0       17 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/setup.sh
+-rw-r--r--   0        0        0      136 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/setup_fail.md
+-rw-r--r--   0        0        0      110 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/timeout.md
+-rw-r--r--   0        0        0     1099 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/whitespace.md
+-rw-r--r--   0        0        0      142 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/fixtures/wildcards.md
+-rw-r--r--   0        0        0     1137 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/test_extract.py
+-rw-r--r--   0        0        0     8705 2023-07-29 08:30:14.941479 tesh-0.3.0/src/tesh/tests/test_tesh.py
+-rw-r--r--   0        0        0     8656 1970-01-01 00:00:00.000000 tesh-0.3.0/PKG-INFO
```

### Comparing `tesh-0.2.0/LICENSE` & `tesh-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tesh-0.2.0/README.md` & `tesh-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <p align="center">
-  <a href="https://circleci.com/gh/OceanSprint/tesh">
-    <img alt="CircleCI for tesh (main branch)"
-         src="https://circleci.com/gh/OceanSprint/tesh.svg?style=shield">
+  <a href="https://github.com/OceanSprint/tesh/actions/workflows/ci.yml">
+    <img alt="CI for tesh (main branch)"
+         src="https://github.com/oceansprint/tesh/actions/workflows/ci.yml/badge.svg">
   </a>
   <img alt="Test coverage (main branch)"
        src="https://img.shields.io/badge/tests_coverage-100%25-brightgreen.svg">
   <img alt="Test coverage (main branch)"
        src="https://img.shields.io/badge/types_coverage-100%25-brightgreen.svg">
   <a href="https://pypi.org/project/tesh/">
     <img alt="latest version of tesh on PyPI"
@@ -103,14 +103,25 @@
 $ printf "Hello \nthere \nfrom \nSpace!"
 Hello
 ...
 Space!
 ```
 ~~~
 
+Commands can continue across multiple lines by prefixing lines with `> `.
+
+~~~
+```console tesh-session="ignore"
+$ echo "Hello from" \
+>   "another" \
+>   "line!"
+Hello from another line!
+```
+~~~
+
 ## Advanced directives
 
 You can set a few other optional directives in the header line:
 
 - `tesh-exitcodes`: a list of exit codes in the order of commands executed inside the code block,
 - `tesh-setup`: a filename of a script to run before running the commands in the code block,
 - `tesh-ps1`: allow an additional PS1 prompt besides the default `$`,
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-[CircleCI_for_tesh_(main_branch)] [Test coverage (main branch)] [Test coverage
- (main branch)] [latest_version_of_tesh_on_PyPI] [Supported_Python_versions]
-                 [License:_MIT] [Built_by_these_great_folks!]
+[CI_for_tesh_(main_branch)] [Test coverage (main branch)] [Test coverage (main
+branch)] [latest_version_of_tesh_on_PyPI] [Supported_Python_versions] [License:
+                      MIT] [Built_by_these_great_folks!]
 # tesh [[tÉÊ]](http://ipa-reader.xyz/?text=t%C9%9B%CA%83&voice=Joanna) -
 TEstable SHell sessions in Markdown Showing shell interactions how to run a
 tool is useful for teaching and explaining. Making sure that example still
 works over the years is painfully hard. Not anymore. ```console $ tesh demo/
 ð Checking demo/happy.md â¨ Running foo â Passed â¨ Running bar â
 Passed ð Checking demo/sad.md â¨ Running foo â Failed Command: echo "foo"
 Expected: sad panda Got: foo Taking you into the shell ... Enter `!!` to rerun
@@ -18,37 +18,39 @@
 session="multiple_blocks" $ export NAME=Earth ``` ~~~ ~~~ ```console tesh-
 session="multiple_blocks" $ echo "Hello $NAME!" Hello Earth! ``` ~~~ ###
 Ignoring parts of the output Parts of the inline output can be ignored with
 `...`: ~~~ ```console tesh-session="ignore" $ echo "Hello from Space!" Hello
 ... Space! ``` ~~~ The same can be done for multiple lines of output. Note that
 trailing whitespace in every line is trimmed. ~~~ ```console tesh-
 session="ignore" $ printf "Hello \nthere \nfrom \nSpace!" Hello ... Space! ```
-~~~ ## Advanced directives You can set a few other optional directives in the
-header line: - `tesh-exitcodes`: a list of exit codes in the order of commands
-executed inside the code block, - `tesh-setup`: a filename of a script to run
-before running the commands in the code block, - `tesh-ps1`: allow an
-additional PS1 prompt besides the default `$`, - `tesh-platform`: specify on
-which platforms this session block should be tested (`linux`, `darwin`,
-`windows`), - `tesh-fixture`: a filename to save the current snippet, - `tesh-
-timeout`: number of seconds before a command timeouts (defaults to 30s), -
-`tesh-long-running`: set to `true` to showcase long-running commands such as
-`docker compose up`. Let's look at all of these through examples! ### Testing
-exit codes `tesh-exitcodes` accepts a list of integers, which represent the
-exit code for every command in the block. ~~~ ```console tesh-
-session="exitcodes" tesh-exitcodes="1 0" $ false $ true ``` ~~~ ### Test setup
-Sometimes you need to do some test setup before running the examples in your
-code blocks. Put those [in a file](./readme.sh) and point to it with the `tesh-
-setup` directive. ~~~ ```console tesh-session="setup" tesh-setup="readme.sh" $
-echo "Hello $NAME!" Hello Gaea! ``` ~~~ ### Custom prompts Every so often you
-need to drop into a virtualenv or similar shell that changes the prompt. `tesh`
-supports this via `test-ps1` directive. ~~~ ```console tesh-session="prompt"
-tesh-ps1="(foo) $" $ PS1="(foo) $ " (foo) $ echo "hello" hello ``` ~~~ ### Only
-run on certain platforms Some examples should only run on certain platforms,
-use `tesh-platform` to declare them as such. ~~~ ```console tesh-
-session="platform" tesh-platform="linux" $ uname ...Linux... ``` ~~~ ~~~
+~~~ Commands can continue across multiple lines by prefixing lines with `> `.
+~~~ ```console tesh-session="ignore" $ echo "Hello from" \ > "another" \ >
+"line!" Hello from another line! ``` ~~~ ## Advanced directives You can set a
+few other optional directives in the header line: - `tesh-exitcodes`: a list of
+exit codes in the order of commands executed inside the code block, - `tesh-
+setup`: a filename of a script to run before running the commands in the code
+block, - `tesh-ps1`: allow an additional PS1 prompt besides the default `$`, -
+`tesh-platform`: specify on which platforms this session block should be tested
+(`linux`, `darwin`, `windows`), - `tesh-fixture`: a filename to save the
+current snippet, - `tesh-timeout`: number of seconds before a command timeouts
+(defaults to 30s), - `tesh-long-running`: set to `true` to showcase long-
+running commands such as `docker compose up`. Let's look at all of these
+through examples! ### Testing exit codes `tesh-exitcodes` accepts a list of
+integers, which represent the exit code for every command in the block. ~~~
+```console tesh-session="exitcodes" tesh-exitcodes="1 0" $ false $ true ``` ~~~
+### Test setup Sometimes you need to do some test setup before running the
+examples in your code blocks. Put those [in a file](./readme.sh) and point to
+it with the `tesh-setup` directive. ~~~ ```console tesh-session="setup" tesh-
+setup="readme.sh" $ echo "Hello $NAME!" Hello Gaea! ``` ~~~ ### Custom prompts
+Every so often you need to drop into a virtualenv or similar shell that changes
+the prompt. `tesh` supports this via `test-ps1` directive. ~~~ ```console tesh-
+session="prompt" tesh-ps1="(foo) $" $ PS1="(foo) $ " (foo) $ echo "hello" hello
+``` ~~~ ### Only run on certain platforms Some examples should only run on
+certain platforms, use `tesh-platform` to declare them as such. ~~~ ```console
+tesh-session="platform" tesh-platform="linux" $ uname ...Linux... ``` ~~~ ~~~
 ```console tesh-session="platform" tesh-platform="darwin" $ uname ...Darwin...
 ``` ~~~ ### Dump file to disk Occasionally your examples consist of first
 showing contents of a file, then executing a command that uses said file. This
 is supported, use the `tesh-fixture` directive. ~~~ ```bash tesh-
 session="fixture" tesh-fixture="foo.sh" echo "foo" ``` ~~~ ~~~ ```console tesh-
 session="fixture" $ chmod +x foo.sh $ ./foo.sh foo ``` ~~~ ### Custom timeout
 By default, `tesh` will fail if an example command does not finish in 30
```

### Comparing `tesh-0.2.0/pyproject.toml` & `tesh-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tesh"
-version = "0.2.0"
+version = "0.3.0"
 description = "TEstable SHell sessions in Markdown"
 readme = "README.md"
 authors = [
 	"Domen Kozar",
   "Nejc Zupan",
 ]
 license = "MIT"
@@ -22,19 +22,19 @@
 
 click = "*"
 pexpect = "*"
 
 
 [tool.poetry.dev-dependencies]
 autoflake = "*"
-black = "==22.6.0"  # remove pin after upgrading to nixpkgs-22.11
-codespell = "==2.1.0"  # remove pin after upgrading to nixpkgs-22.11
+black = "*"
+codespell = "*"
 coverage = "*"
 docutils = "*"
-flake8 = "==5.0.4"
+flake8 = "*"
 flake8-assertive = "*"
 flake8-blind-except = "*"
 flake8-bugbear = "*"
 flake8-builtins = "*"
 flake8-comprehensions = "*"
 flake8-debugger = "*"
 flake8-deprecated = "*"
@@ -43,32 +43,32 @@
 flake8-plone-hasattr = "*"
 flake8-print = "*"
 flake8-self = "*"
 flake8-super-call = "*"
 flake8-tuple = "*"
 isort = "*"
 mccabe = "*"
-mypy = "==0.971"  # remove dependency after upgrading to nixpkgs-22.11
+mypy = "*"
 pdbpp = "*"
 pre-commit = "*"
 pre-commit-hooks = "*"
 pyfakefs = "*"
-pytest = "==7.1.2"  # remove pin after upgrading to nixpkgs-22.11
+pytest = "*"
 pytest-cov = "*"
 pytest-instafail = "*"
 pytest-randomly = "*"
 pytest-socket = "*"
 pyupgrade = "*"
 typecov = "*"
 yamllint = "*"
 
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry>=0.12"]
+build-backend = "poetry.masonry.api"
 
 
 [tool.autoflake]
 remove-all-unused-imports = true
 in-place = true
 recursive = true
```

### Comparing `tesh-0.2.0/src/tesh/__init__.py` & `tesh-0.3.0/src/tesh/__init__.py`

 * *Files identical despite different names*

### Comparing `tesh-0.2.0/src/tesh/extract.py` & `tesh-0.3.0/src/tesh/extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,31 +177,33 @@
             if new_block.command:
                 blocks.append(new_block)
             new_block = Block("")
             new_block.command = re.sub(
                 r"^" + get_prompt_regex(session), "", line
             ).strip()
             new_block.prompt = m.group(0)
+        elif m := re.match("^> (.*)$", line):
+            new_block.command += f"\n{m.group(1)}"
         elif not line.strip():
             continue
         else:
-            new_block.output.append(line.strip())
+            new_block.output.append(line.rstrip("\n"))
     blocks.append(new_block)
     session.blocks = blocks
 
     if session.exitcodes and (len(session.exitcodes) != len(session.blocks)):
         fail(
             "If you're using exit codes for a session, you must specify them for all commands."
         )
 
 
 def get_prompt_regex(session: ShellSession) -> str:
     """Return the regex for the prompt."""
     if session.ps1:
-        return r"(\$|{ps1}) ".format(ps1=re.escape(session.ps1))
+        return r"(^\$$|\$ |{ps1} )".format(ps1=re.escape(session.ps1))
     else:
-        return r"\$ "
+        return r"(^\$$|\$ )"
 
 
 def parse_exitcodes(exitcodes_spec: str) -> list[int]:
     """Parse '0 1 0' spec of exitcodes into a list of ints."""
     return [int(exitcode) for exitcode in exitcodes_spec.split()]
```

### Comparing `tesh-0.2.0/src/tesh/test.py` & `tesh-0.3.0/src/tesh/test.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,41 +8,98 @@
 import fnmatch
 import os
 import pexpect
 import re
 import sys
 
 
+class NoANSIExpecter(pexpect.Expecter):
+    """Custom Expecter to filter out ANSI escape code."""
+
+    # regex for vt100 from https://stackoverflow.com/a/14693789/5008284
+    ansi_escape = re.compile(r"(\x1B[@-_][0-?]*[ -/]*[@-~]|\\[\[\]])")
+
+    def new_data(self, data: str) -> int:
+        """Filter out ANSI escape code.
+
+        And then call original `pexpect.Expecter.new_data` function.
+        """
+        data = self.ansi_escape.sub("", data)
+        return pexpect.Expecter.new_data(self, data)
+
+
+class spawn(pexpect.spawn):
+    def expect_list(
+        self,
+        pattern_list: list[str],
+        timeout: int = -1,
+        searchwindowsize: int = -1,
+        async_: bool = False,
+        **kw: bool,
+    ) -> int:
+        """Use NoANSIExpecter to filter out ANSI escape code.
+
+        We copied original `expect_list` function to be able to replace the
+        Expecter.
+        """
+        if timeout == -1:
+            timeout = self.timeout
+        if "async" in kw:  # pragma: no cover
+            async_ = kw.pop("async")
+        if kw:  # pragma: no cover
+            raise TypeError("Unknown keyword arguments: {}".format(kw))
+
+        exp = NoANSIExpecter(
+            self, pexpect.expect.searcher_re(pattern_list), searchwindowsize
+        )
+        if async_:  # pragma: no cover
+            from pexpect._async import expect_async
+
+            return expect_async(exp, timeout)
+        else:
+            return exp.expect_loop(timeout)
+
+
 def test(filename: str, session: ShellSession, verbose: bool, debug: bool) -> None:
     """Run testable sessions in a pexpect shell."""
     with Path(filename).parent:
-        shell = pexpect.spawn(
+        shell = spawn(
             "bash --norc --noprofile",
+            encoding="utf-8",
             env={"PS1": "$ ", "PATH": os.environ["PATH"], "HOME": os.getcwd()},
+            # The (height, width) of the TTY commands run in. 24 is the default.
+            # The width needs to be larger than the longest command, as
+            # otherwise the command string gets truncated and the shell.expect
+            # calls fail to match the the pattern's full command against the
+            # truncated output.
+            dimensions=(24, 1000),
         )
         shell.expect(r"\$ ")
         if session.setup:
             shell.sendline("source " + session.setup)
             shell.expect(get_prompt_regex(session))
         for index, block in enumerate(session.blocks):
             if verbose:
                 print(":")
                 print("       Command:", block.command)
                 print("       Output:", block.output)
 
             shell.sendline(block.command)
-            shell.expect(re.escape(block.command))
+            for command_line in block.command.splitlines():
+                shell.expect_exact(command_line + "\r\n")
 
             # we expect the prompt of the next command unless there's no more
             if index + 1 < len(session.blocks):
                 prompt = session.blocks[index + 1].prompt
             else:
                 prompt = session.blocks[index].prompt
+            prompt = re.escape(prompt)
+            prompt = prompt.replace("\\.\\.\\.", "(?=\\r\\n(?!.*\\r\\n)).*")
             try:
-                shell.expect(re.escape(prompt), timeout=session.timeout)
+                shell.expect(prompt, timeout=session.timeout)
 
             # This is tested in test_timeout but coverage doesn't catch it because
             # it is executed in a subshell
             except pexpect.exceptions.TIMEOUT:  # pragma: no cover
                 if session.long_running:
                     if index + 1 == len(session.blocks):
                         compare_outputs(shell, block, debug)
@@ -63,47 +120,50 @@
                     sys.exit(1)
 
             compare_outputs(shell, block, debug)
 
             # handle exit codes
             shell.sendline("echo $?")
             shell.expect("echo [$][?]")
-            shell.expect(re.escape(prompt))
-            exitcode = int(shell.before.decode("utf-8").strip())
+            shell.expect(prompt)
+            assert isinstance(shell.before, str)
+            exitcode = int(shell.before.strip())
             if session.exitcodes and exitcode != session.exitcodes[index]:
                 print("❌ Failed")  # noqa: ENC100
                 print("         Command:", block.command)
                 print()
                 print("         Expected exit code:", session.exitcodes[index])
                 print("         Got exit code:", exitcode)
                 if debug:  # pragma: no cover
                     invoke_debug(shell, block)
                 else:
                     sys.exit(1)
 
 
-def get_actual_output(shell: pexpect.spawn) -> str:
+def get_actual_output(shell: spawn) -> str:
     """Massage shell output to be able to compare it."""
-    actual_output = shell.before.decode("utf-8").strip().replace("\r\n", "\n")
+    assert isinstance(shell.before, str)
+    actual_output = shell.before.rstrip().replace("\r\n", "\n")
     return "\n".join([line.rstrip() for line in actual_output.split("\n")])
 
 
 def get_expected_output(block: Block) -> str:
     """Massage expected output to be able to compare it."""
     expected_output = (
         "\n".join(block.output)
+        .replace("[", "[[]")
         .replace("*", "[*]")
         .replace("?", "[?]")
         .replace("...", "*")
     )
     # trim whitespace in every line
     return "\n".join([line.rstrip() for line in expected_output.split("\n")])
 
 
-def compare_outputs(shell: pexpect.spawn, block: Block, debug: bool) -> None:
+def compare_outputs(shell: spawn, block: Block, debug: bool) -> None:
     """Compare expected and the actual output and fail if they don't match."""
     actual_output = get_actual_output(shell)
     expected_output = get_expected_output(block)
 
     if not fnmatch.fnmatch(actual_output, expected_output):
         print("❌ Failed")  # noqa: ENC100
         print("         Command:", block.command)
@@ -119,15 +179,15 @@
             invoke_debug(shell, block)
         else:
             sys.exit(1)
 
 
 # This is tested in test_debug but coverage doesn't catch it because
 # it is executed in a subshell
-def invoke_debug(shell: pexpect.spawn, block: Block) -> None:  # pragma: no cover
+def invoke_debug(shell: spawn, block: Block) -> None:  # pragma: no cover
     """Take the user to a debug shell."""
     print()
     print("Taking you into the shell ...")
     print()
     print("Enter `!!` to rerun the last command.")
     print()
     print(block.prompt, end="")
```

### Comparing `tesh-0.2.0/src/tesh/tests/fixtures/no_codeblocks.md` & `tesh-0.3.0/src/tesh/tests/fixtures/no_codeblocks.md`

 * *Files identical despite different names*

### Comparing `tesh-0.2.0/src/tesh/tests/test_extract.py` & `tesh-0.3.0/src/tesh/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `tesh-0.2.0/src/tesh/tests/test_tesh.py` & `tesh-0.3.0/src/tesh/tests/test_tesh.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def test_version() -> None:
     """Test printing the current version."""
     runner = CliRunner()
     result = runner.invoke(tesh, "--version")
 
     assert result.exit_code == 0
-    assert "tesh, version 0.2.0\n" == result.output
+    assert "tesh, version 0.3.0\n" == result.output
 
 
 def test_empty_folder() -> None:
     """Test pointing tesh to an empty folder."""
     runner = CliRunner()
     result = runner.invoke(tesh, "src/tesh/tests/fixtures/empty_folder")
 
@@ -69,16 +69,16 @@
     assert result.exit_code == 0
 
     # fmt: off
     expected = (
 """
 📄 Checking src/tesh/tests/fixtures/folder/simple.md
   ✨ Running foo  :
-       Command: echo "foo"
-       Output: ['foo']
+       Command: echo "foo ✨"
+       Output: ['foo ✨']
 ✅ Passed
 """
     ).lstrip("\n")
     # fmt: on
 
     assert expected == result.output
 
@@ -144,26 +144,28 @@
     # fmt: on
 
     assert expected == result.output
 
 
 def test_debug() -> None:  # pragma: no cover
     """Test dropping into an interactive shell on error."""
-    shell = pexpect.spawn("tesh src/tesh/tests/fixtures/debug.md")
+    shell = pexpect.spawn("tesh src/tesh/tests/fixtures/debug.md", encoding="utf-8")
     shell.expect("Taking you into the shell ...")
 
-    assert "✨ Running foo  ❌ Failed".encode() in shell.before
+    assert isinstance(shell.before, str)
+    assert "✨ Running foo  ❌ Failed" in shell.before
 
 
 def test_timeout() -> None:  # pragma: no cover
     """Test dropping into an interactive shell on timeout."""
-    shell = pexpect.spawn("tesh src/tesh/tests/fixtures/timeout.md")
+    shell = pexpect.spawn("tesh src/tesh/tests/fixtures/timeout.md", encoding="utf-8")
     shell.expect("Taking you into the shell ...", timeout=60)
 
-    assert "✨ Running foo  ❌ Timed out after 1s".encode() in shell.before
+    assert isinstance(shell.before, str)
+    assert "✨ Running foo  ❌ Timed out after 1s" in shell.before
 
 
 def test_exitcodes() -> None:
     """Test pointing tesh to a Markdown file using exitcodes."""
     runner = CliRunner()
     result = runner.invoke(tesh, "src/tesh/tests/fixtures/exitcodes.md")
 
@@ -277,7 +279,88 @@
 📄 Checking src/tesh/tests/fixtures/prompt.md
   ✨ Running foo  ✅ Passed
 """
     ).lstrip("\n")
     # fmt: on
 
     assert expected == result.output
+
+
+def test_long_commands() -> None:
+    """Test lengthy commands, which can be truncated if they're too long."""
+    runner = CliRunner()
+    result = runner.invoke(tesh, "src/tesh/tests/fixtures/long_command.md")
+
+    assert result.exit_code == 0
+
+    # fmt: off
+    expected = (
+"""
+📄 Checking src/tesh/tests/fixtures/long_command.md
+  ✨ Running long-cmds  ✅ Passed
+"""
+    ).lstrip("\n")
+    # fmt: on
+
+    assert expected == result.output
+
+
+def test_multiline_command() -> None:
+    """Test using `> ` to extend a command across more than one line."""
+    runner = CliRunner()
+    result = runner.invoke(tesh, "src/tesh/tests/fixtures/multiline_command.md")
+
+    assert result.exit_code == 0
+
+    # fmt: off
+    expected = (
+"""
+📄 Checking src/tesh/tests/fixtures/multiline_command.md
+  ✨ Running readme-example  ✅ Passed
+"""
+    ).lstrip("\n")
+    # fmt: on
+
+    assert expected == result.output
+
+
+def test_wildcards() -> None:
+    """Test using ... to ignore parts of the output."""
+    runner = CliRunner()
+    result = runner.invoke(tesh, "src/tesh/tests/fixtures/wildcards.md")
+
+    assert result.exit_code == 0
+
+    # fmt: off
+    expected = (
+"""
+📄 Checking src/tesh/tests/fixtures/wildcards.md
+  ✨ Running foo  ✅ Passed
+"""
+    ).lstrip("\n")
+    # fmt: on
+
+    assert expected == result.output
+
+
+def test_whitespace() -> None:
+    """Test code blocks with whitespace.
+
+    Both whitespace in command output, and indented code blocks.
+    """
+    runner = CliRunner()
+    result = runner.invoke(tesh, "src/tesh/tests/fixtures/whitespace.md")
+
+    assert result.exit_code == 0
+
+    # fmt: off
+    expected = (
+"""
+📄 Checking src/tesh/tests/fixtures/whitespace.md
+  ✨ Running non-indented-block  ✅ Passed
+  ✨ Running indented-block  ✅ Passed
+  ✨ Running extra-trailing-whitespace  ✅ Passed
+"""
+    ).lstrip("\n")
+    # fmt: on
+
+    assert expected == result.output
```

### Comparing `tesh-0.2.0/setup.py` & `tesh-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,320 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tesh
+Version: 0.3.0
+Summary: TEstable SHell sessions in Markdown
+License: MIT
+Author: Domen Kozar
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click
+Requires-Dist: pexpect
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+<p align="center">
+  <a href="https://github.com/OceanSprint/tesh/actions/workflows/ci.yml">
+    <img alt="CI for tesh (main branch)"
+         src="https://github.com/oceansprint/tesh/actions/workflows/ci.yml/badge.svg">
+  </a>
+  <img alt="Test coverage (main branch)"
+       src="https://img.shields.io/badge/tests_coverage-100%25-brightgreen.svg">
+  <img alt="Test coverage (main branch)"
+       src="https://img.shields.io/badge/types_coverage-100%25-brightgreen.svg">
+  <a href="https://pypi.org/project/tesh/">
+    <img alt="latest version of tesh on PyPI"
+         src="https://img.shields.io/pypi/v/tesh.svg">
+  </a>
+  <a href="https://pypi.org/project/tesh/">
+    <img alt="Supported Python versions"
+         src="https://img.shields.io/pypi/pyversions/tesh.svg">
+  </a>
+  <a href="https://github.com/OceanSprint/tesh/blob/main/LICENSE">
+    <img alt="License: MIT"
+         src="https://img.shields.io/badge/License-MIT-yellow.svg">
+  </a>
+  <a href="https://github.com/OceanSprint/tesh/graphs/contributors">
+    <img alt="Built by these great folks!"
+         src="https://img.shields.io/github/contributors/OceanSprint/tesh.svg">
+  </a>
+</p>
 
-packages = \
-['tesh', 'tesh.tests']
+# tesh [[tɛʃ]](http://ipa-reader.xyz/?text=t%C9%9B%CA%83&voice=Joanna) - TEstable SHell sessions in Markdown
 
-package_data = \
-{'': ['*'],
- 'tesh.tests': ['fixtures/*', 'fixtures/empty_folder/*', 'fixtures/folder/*']}
-
-install_requires = \
-['click', 'pexpect']
-
-entry_points = \
-{'console_scripts': ['tesh = tesh:tesh']}
-
-setup_kwargs = {
-    'name': 'tesh',
-    'version': '0.2.0',
-    'description': 'TEstable SHell sessions in Markdown',
-    'long_description': '<p align="center">\n  <a href="https://circleci.com/gh/OceanSprint/tesh">\n    <img alt="CircleCI for tesh (main branch)"\n         src="https://circleci.com/gh/OceanSprint/tesh.svg?style=shield">\n  </a>\n  <img alt="Test coverage (main branch)"\n       src="https://img.shields.io/badge/tests_coverage-100%25-brightgreen.svg">\n  <img alt="Test coverage (main branch)"\n       src="https://img.shields.io/badge/types_coverage-100%25-brightgreen.svg">\n  <a href="https://pypi.org/project/tesh/">\n    <img alt="latest version of tesh on PyPI"\n         src="https://img.shields.io/pypi/v/tesh.svg">\n  </a>\n  <a href="https://pypi.org/project/tesh/">\n    <img alt="Supported Python versions"\n         src="https://img.shields.io/pypi/pyversions/tesh.svg">\n  </a>\n  <a href="https://github.com/OceanSprint/tesh/blob/main/LICENSE">\n    <img alt="License: MIT"\n         src="https://img.shields.io/badge/License-MIT-yellow.svg">\n  </a>\n  <a href="https://github.com/OceanSprint/tesh/graphs/contributors">\n    <img alt="Built by these great folks!"\n         src="https://img.shields.io/github/contributors/OceanSprint/tesh.svg">\n  </a>\n</p>\n\n# tesh [[tɛʃ]](http://ipa-reader.xyz/?text=t%C9%9B%CA%83&voice=Joanna) - TEstable SHell sessions in Markdown\n\nShowing shell interactions how to run a tool is useful for teaching and explaining.\n\nMaking sure that example still works over the years is painfully hard.\n\nNot anymore.\n\n```console\n$ tesh demo/\n📄 Checking demo/happy.md\n  ✨ Running foo  ✅ Passed\n  ✨ Running bar  ✅ Passed\n📄 Checking demo/sad.md\n  ✨ Running foo  ❌ Failed\n         Command: echo "foo"\n\n         Expected:\nsad panda\n         Got:\nfoo\n\nTaking you into the shell ...\n\nEnter `!!` to rerun the last command.\n\n$\n```\n\n## Syntax\n\nTo mark a code block as testable, append `tesh-session="NAME"` to the header line.\n\nYou can use any syntax highlighting directive, such as `bash`, `shell`, `shell-session`, `console` or others.\n\n~~~\n```console tesh-session="hello"\n$ echo "Hello World!"\nHello World!\n```\n~~~\n\n### Linking multiple code blocks into a single shell session\n\nBesides marking a code block as testable, `tesh-session` is a unique identifier that allows for multiple code blocks to share the same session.\n\n~~~\n```console tesh-session="multiple_blocks"\n$ export NAME=Earth\n\n```\n~~~\n\n~~~\n```console tesh-session="multiple_blocks"\n$ echo "Hello $NAME!"\nHello Earth!\n```\n~~~\n\n### Ignoring parts of the output\n\nParts of the inline output can be ignored with `...`:\n\n~~~\n```console tesh-session="ignore"\n$ echo "Hello from Space!"\nHello ... Space!\n```\n~~~\n\nThe same can be done for multiple lines of output. Note that trailing whitespace in every line is trimmed.\n\n~~~\n```console tesh-session="ignore"\n$ printf "Hello \\nthere \\nfrom \\nSpace!"\nHello\n...\nSpace!\n```\n~~~\n\n## Advanced directives\n\nYou can set a few other optional directives in the header line:\n\n- `tesh-exitcodes`: a list of exit codes in the order of commands executed inside the code block,\n- `tesh-setup`: a filename of a script to run before running the commands in the code block,\n- `tesh-ps1`: allow an additional PS1 prompt besides the default `$`,\n- `tesh-platform`: specify on which platforms this session block should be tested (`linux`, `darwin`, `windows`),\n- `tesh-fixture`: a filename to save the current snippet,\n- `tesh-timeout`: number of seconds before a command timeouts (defaults to 30s),\n- `tesh-long-running`: set to `true` to showcase long-running commands such as `docker compose up`.\n\nLet\'s look at all of these through examples!\n\n### Testing exit codes\n\n`tesh-exitcodes` accepts a list of integers, which represent the exit code for every command in the block.\n\n~~~\n```console tesh-session="exitcodes" tesh-exitcodes="1 0"\n$ false\n\n$ true\n\n```\n~~~\n\n\n### Test setup\n\nSometimes you need to do some test setup before running the examples in your code blocks. Put those [in a file](./readme.sh) and point to it with the `tesh-setup` directive.\n\n~~~\n```console tesh-session="setup" tesh-setup="readme.sh"\n$ echo "Hello $NAME!"\nHello Gaea!\n```\n~~~\n\n\n### Custom prompts\n\nEvery so often you need to drop into a virtualenv or similar shell that changes the prompt. `tesh` supports this via `test-ps1` directive.\n\n~~~\n```console tesh-session="prompt" tesh-ps1="(foo) $"\n$ PS1="(foo) $ "\n\n\n(foo) $ echo "hello"\nhello\n```\n~~~\n\n### Only run on certain platforms\n\nSome examples should only run on certain platforms, use `tesh-platform` to declare them as such.\n\n~~~\n```console tesh-session="platform" tesh-platform="linux"\n$ uname\n...Linux...\n```\n~~~\n\n~~~\n```console tesh-session="platform" tesh-platform="darwin"\n$ uname\n...Darwin...\n```\n~~~\n\n### Dump file to disk\n\nOccasionally your examples consist of first showing contents of a file, then executing a command that uses said file. This is supported, use the `tesh-fixture` directive.\n\n~~~\n```bash tesh-session="fixture" tesh-fixture="foo.sh"\necho "foo"\n```\n~~~\n\n~~~\n```console tesh-session="fixture"\n$ chmod +x foo.sh\n\n$ ./foo.sh\nfoo\n```\n~~~\n\n### Custom timeout\n\nBy default, `tesh` will fail if an example command does not finish in 30 seconds. This number can be modified using the `tesh-timeout` directive.\n\n~~~\n```console tesh-session="timeout" tesh-timeout="3"\n$ sleep 1\n\n```\n~~~\n\n\n### Long running processes\n\nSome processes that you want to show examples for are long-running processes, like `docker compose up`. They are supported in `tesh` blocks using the `tesh-long-running` directive. Note that they need to be the last command in the block.\n\n\n~~~\n```console tesh-session="long-running" tesh-timeout="1" tesh-long-running="true"\n$ nmap 1.1.1.1\nStarting Nmap ...\n```\n~~~\n\n## Installation\n\nThe best way to install `tesh` is with your favorite Python package manager.\n\n```bash\n$ pip install tesh\n```\n\n## Design decisions\n\n- Supports Linux / macOS.\n- Not tied to a specific markdown flavor or tooling.\n- Renders reasonably well on GitHub.\n\n\n## Comparison with other tools\n\n| | tesh | [mdsh](https://github.com/zimbatm/mdsh) | [pandoc filters](http://www.chriswarbo.net/projects/activecode/index.html) |\n|------------------------------------------|---|---|---|\n| Execute shell session                    | ✔️ | ✔️ | ✔️ |\n| Modify markdown file with the new output | 🚧[<sub>[1]</sub>](https://github.com/OceanSprint/tesh/issues/6) | ✔️ | ✔️ |\n| Shared session between code blocks       | ✔️ | ✖️ | ✖️ |\n| Custom PS1 prompts                       | ✔️ | ✖️ | ✖️ |\n| Assert non-zero exit codes               | ✔️ | ✖️ | ✖️ |\n| Setup the shell environment              | ✔️ | ✖️ | ✖️ |\n| Reference fixtures from other snippets   | ✔️ | ✖️ | ✖️ |\n| Wildcard matching of the command output  | ✔️ | ✖️ | ✖️ |\n| Starts the shell in debugging mode       | ✔️ | ✖️ | ✖️ |\n| Specify timeout                          | ✔️ | ✖️ | ✖️ |\n| Support long-running commands            | ✔️ | ✖️ | ✖️ |\n\n* ✔️: Supported\n* C: Possible but you have to write some code yourself\n* 🚧: Under development\n* ✖️: Not supported\n* ?: I don\'t know.\n\n\n## Developing `tesh`\n\nYou need to have [poetry](https://python-poetry.org/) and Python 3.9 through 3.11 installed on your machine.\n\nAlternatively, if you use [nix](https://nix.dev/tutorials/declarative-and-reproducible-developer-environments), run `nix-shell` to drop into a shell that has everything prepared for development.\n\nThen you can run `make tests` to run all tests & checks. Additional `make` commands are available:\n\n```\n# run tesh on all Markdown files\n$ make tesh\n\n# run flake8 linters on changed files only\n$ make lint\n\n# run flake8 linters on all files\n$ make lint all=true\n\n# run mypy type checker\n$ make types\n\n# run unit tests\n$ make unit\n\n# run a subset of unit tests (regex find)\n$ make unit filter=foo\n\n# re-lock Python dependencies (for example after adding or removing one from pyproject.toml)\n$ make lock\n```\n',
-    'author': 'Domen Kozar',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+Showing shell interactions how to run a tool is useful for teaching and explaining.
 
+Making sure that example still works over the years is painfully hard.
+
+Not anymore.
+
+```console
+$ tesh demo/
+📄 Checking demo/happy.md
+  ✨ Running foo  ✅ Passed
+  ✨ Running bar  ✅ Passed
+📄 Checking demo/sad.md
+  ✨ Running foo  ❌ Failed
+         Command: echo "foo"
+
+         Expected:
+sad panda
+         Got:
+foo
+
+Taking you into the shell ...
+
+Enter `!!` to rerun the last command.
+
+$
+```
+
+## Syntax
+
+To mark a code block as testable, append `tesh-session="NAME"` to the header line.
+
+You can use any syntax highlighting directive, such as `bash`, `shell`, `shell-session`, `console` or others.
+
+~~~
+```console tesh-session="hello"
+$ echo "Hello World!"
+Hello World!
+```
+~~~
+
+### Linking multiple code blocks into a single shell session
+
+Besides marking a code block as testable, `tesh-session` is a unique identifier that allows for multiple code blocks to share the same session.
+
+~~~
+```console tesh-session="multiple_blocks"
+$ export NAME=Earth
+
+```
+~~~
+
+~~~
+```console tesh-session="multiple_blocks"
+$ echo "Hello $NAME!"
+Hello Earth!
+```
+~~~
+
+### Ignoring parts of the output
+
+Parts of the inline output can be ignored with `...`:
+
+~~~
+```console tesh-session="ignore"
+$ echo "Hello from Space!"
+Hello ... Space!
+```
+~~~
+
+The same can be done for multiple lines of output. Note that trailing whitespace in every line is trimmed.
+
+~~~
+```console tesh-session="ignore"
+$ printf "Hello \nthere \nfrom \nSpace!"
+Hello
+...
+Space!
+```
+~~~
+
+Commands can continue across multiple lines by prefixing lines with `> `.
+
+~~~
+```console tesh-session="ignore"
+$ echo "Hello from" \
+>   "another" \
+>   "line!"
+Hello from another line!
+```
+~~~
+
+## Advanced directives
+
+You can set a few other optional directives in the header line:
+
+- `tesh-exitcodes`: a list of exit codes in the order of commands executed inside the code block,
+- `tesh-setup`: a filename of a script to run before running the commands in the code block,
+- `tesh-ps1`: allow an additional PS1 prompt besides the default `$`,
+- `tesh-platform`: specify on which platforms this session block should be tested (`linux`, `darwin`, `windows`),
+- `tesh-fixture`: a filename to save the current snippet,
+- `tesh-timeout`: number of seconds before a command timeouts (defaults to 30s),
+- `tesh-long-running`: set to `true` to showcase long-running commands such as `docker compose up`.
+
+Let's look at all of these through examples!
+
+### Testing exit codes
+
+`tesh-exitcodes` accepts a list of integers, which represent the exit code for every command in the block.
+
+~~~
+```console tesh-session="exitcodes" tesh-exitcodes="1 0"
+$ false
+
+$ true
+
+```
+~~~
+
+
+### Test setup
+
+Sometimes you need to do some test setup before running the examples in your code blocks. Put those [in a file](./readme.sh) and point to it with the `tesh-setup` directive.
+
+~~~
+```console tesh-session="setup" tesh-setup="readme.sh"
+$ echo "Hello $NAME!"
+Hello Gaea!
+```
+~~~
+
+
+### Custom prompts
+
+Every so often you need to drop into a virtualenv or similar shell that changes the prompt. `tesh` supports this via `test-ps1` directive.
+
+~~~
+```console tesh-session="prompt" tesh-ps1="(foo) $"
+$ PS1="(foo) $ "
+
+
+(foo) $ echo "hello"
+hello
+```
+~~~
+
+### Only run on certain platforms
+
+Some examples should only run on certain platforms, use `tesh-platform` to declare them as such.
+
+~~~
+```console tesh-session="platform" tesh-platform="linux"
+$ uname
+...Linux...
+```
+~~~
+
+~~~
+```console tesh-session="platform" tesh-platform="darwin"
+$ uname
+...Darwin...
+```
+~~~
+
+### Dump file to disk
+
+Occasionally your examples consist of first showing contents of a file, then executing a command that uses said file. This is supported, use the `tesh-fixture` directive.
+
+~~~
+```bash tesh-session="fixture" tesh-fixture="foo.sh"
+echo "foo"
+```
+~~~
+
+~~~
+```console tesh-session="fixture"
+$ chmod +x foo.sh
+
+$ ./foo.sh
+foo
+```
+~~~
+
+### Custom timeout
+
+By default, `tesh` will fail if an example command does not finish in 30 seconds. This number can be modified using the `tesh-timeout` directive.
+
+~~~
+```console tesh-session="timeout" tesh-timeout="3"
+$ sleep 1
+
+```
+~~~
+
+
+### Long running processes
+
+Some processes that you want to show examples for are long-running processes, like `docker compose up`. They are supported in `tesh` blocks using the `tesh-long-running` directive. Note that they need to be the last command in the block.
+
+
+~~~
+```console tesh-session="long-running" tesh-timeout="1" tesh-long-running="true"
+$ nmap 1.1.1.1
+Starting Nmap ...
+```
+~~~
+
+## Installation
+
+The best way to install `tesh` is with your favorite Python package manager.
+
+```bash
+$ pip install tesh
+```
+
+## Design decisions
+
+- Supports Linux / macOS.
+- Not tied to a specific markdown flavor or tooling.
+- Renders reasonably well on GitHub.
+
+
+## Comparison with other tools
+
+| | tesh | [mdsh](https://github.com/zimbatm/mdsh) | [pandoc filters](http://www.chriswarbo.net/projects/activecode/index.html) |
+|------------------------------------------|---|---|---|
+| Execute shell session                    | ✔️ | ✔️ | ✔️ |
+| Modify markdown file with the new output | 🚧[<sub>[1]</sub>](https://github.com/OceanSprint/tesh/issues/6) | ✔️ | ✔️ |
+| Shared session between code blocks       | ✔️ | ✖️ | ✖️ |
+| Custom PS1 prompts                       | ✔️ | ✖️ | ✖️ |
+| Assert non-zero exit codes               | ✔️ | ✖️ | ✖️ |
+| Setup the shell environment              | ✔️ | ✖️ | ✖️ |
+| Reference fixtures from other snippets   | ✔️ | ✖️ | ✖️ |
+| Wildcard matching of the command output  | ✔️ | ✖️ | ✖️ |
+| Starts the shell in debugging mode       | ✔️ | ✖️ | ✖️ |
+| Specify timeout                          | ✔️ | ✖️ | ✖️ |
+| Support long-running commands            | ✔️ | ✖️ | ✖️ |
+
+* ✔️: Supported
+* C: Possible but you have to write some code yourself
+* 🚧: Under development
+* ✖️: Not supported
+* ?: I don't know.
+
+
+## Developing `tesh`
+
+You need to have [poetry](https://python-poetry.org/) and Python 3.9 through 3.11 installed on your machine.
+
+Alternatively, if you use [nix](https://nix.dev/tutorials/declarative-and-reproducible-developer-environments), run `nix-shell` to drop into a shell that has everything prepared for development.
+
+Then you can run `make tests` to run all tests & checks. Additional `make` commands are available:
+
+```
+# run tesh on all Markdown files
+$ make tesh
+
+# run flake8 linters on changed files only
+$ make lint
+
+# run flake8 linters on all files
+$ make lint all=true
+
+# run mypy type checker
+$ make types
+
+# run unit tests
+$ make unit
+
+# run a subset of unit tests (regex find)
+$ make unit filter=foo
+
+# re-lock Python dependencies (for example after adding or removing one from pyproject.toml)
+$ make lock
+```
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,110 +1,99 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['tesh', 'tesh.tests'] package_data = \ {'': ['*'],
-'tesh.tests': ['fixtures/*', 'fixtures/empty_folder/*', 'fixtures/folder/*']}
-install_requires = \ ['click', 'pexpect'] entry_points = \ {'console_scripts':
-['tesh = tesh:tesh']} setup_kwargs = { 'name': 'tesh', 'version': '0.2.0',
-'description': 'TEstable SHell sessions in Markdown', 'long_description': '
-\n \n_n_src="https://circleci.com/gh/OceanSprint/tesh.svg?style=shield">\n\n n
- src="https://img.shields.io/badge/tests_coverage-100%25-brightgreen.svg">\n n
-src="https://img.shields.io/badge/types_coverage-100%25-brightgreen.svg">\n \n
-    n_src="https://img.shields.io/pypi/v/tesh.svg">\n\n \n_n_src="https://
-img.shields.io/pypi/pyversions/tesh.svg">\n\n \n_n_src="https://img.shields.io/
-  badge/License-MIT-yellow.svg">\n\n \n_n_src="https://img.shields.io/github/
-                    contributors/OceanSprint/tesh.svg">\n\n
-\n\n# tesh [[tÉÊ]](http://ipa-reader.xyz/?text=t%C9%9B%CA%83&voice=Joanna) -
-TEstable SHell sessions in Markdown\n\nShowing shell interactions how to run a
-tool is useful for teaching and explaining.\n\nMaking sure that example still
-works over the years is painfully hard.\n\nNot anymore.\n\n```console\n$ tesh
-demo/\nð Checking demo/happy.md\n â¨ Running foo â Passed\n â¨ Running
-bar â Passed\nð Checking demo/sad.md\n â¨ Running foo â Failed\n
-Command: echo "foo"\n\n Expected:\nsad panda\n Got:\nfoo\n\nTaking you into the
-shell ...\n\nEnter `!!` to rerun the last command.\n\n$\n```\n\n## Syntax\n\nTo
-mark a code block as testable, append `tesh-session="NAME"` to the header
-line.\n\nYou can use any syntax highlighting directive, such as `bash`,
-`shell`, `shell-session`, `console` or others.\n\n~~~\n```console tesh-
-session="hello"\n$ echo "Hello World!"\nHello World!\n```\n~~~\n\n### Linking
-multiple code blocks into a single shell session\n\nBesides marking a code
+Metadata-Version: 2.1 Name: tesh Version: 0.3.0 Summary: TEstable SHell
+sessions in Markdown License: MIT Author: Domen Kozar Requires-Python:
+>=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: click Requires-Dist:
+pexpect Description-Content-Type: text/markdown
+[CI_for_tesh_(main_branch)] [Test coverage (main branch)] [Test coverage (main
+branch)] [latest_version_of_tesh_on_PyPI] [Supported_Python_versions] [License:
+                      MIT] [Built_by_these_great_folks!]
+# tesh [[tÉÊ]](http://ipa-reader.xyz/?text=t%C9%9B%CA%83&voice=Joanna) -
+TEstable SHell sessions in Markdown Showing shell interactions how to run a
+tool is useful for teaching and explaining. Making sure that example still
+works over the years is painfully hard. Not anymore. ```console $ tesh demo/
+ð Checking demo/happy.md â¨ Running foo â Passed â¨ Running bar â
+Passed ð Checking demo/sad.md â¨ Running foo â Failed Command: echo "foo"
+Expected: sad panda Got: foo Taking you into the shell ... Enter `!!` to rerun
+the last command. $ ``` ## Syntax To mark a code block as testable, append
+`tesh-session="NAME"` to the header line. You can use any syntax highlighting
+directive, such as `bash`, `shell`, `shell-session`, `console` or others. ~~~
+```console tesh-session="hello" $ echo "Hello World!" Hello World! ``` ~~~ ###
+Linking multiple code blocks into a single shell session Besides marking a code
 block as testable, `tesh-session` is a unique identifier that allows for
-multiple code blocks to share the same session.\n\n~~~\n```console tesh-
-session="multiple_blocks"\n$ export NAME=Earth\n\n```\n~~~\n\n~~~\n```console
-tesh-session="multiple_blocks"\n$ echo "Hello $NAME!"\nHello
-Earth!\n```\n~~~\n\n### Ignoring parts of the output\n\nParts of the inline
-output can be ignored with `...`:\n\n~~~\n```console tesh-session="ignore"\n$
-echo "Hello from Space!"\nHello ... Space!\n```\n~~~\n\nThe same can be done
-for multiple lines of output. Note that trailing whitespace in every line is
-trimmed.\n\n~~~\n```console tesh-session="ignore"\n$ printf "Hello \\nthere
-\\nfrom \\nSpace!"\nHello\n...\nSpace!\n```\n~~~\n\n## Advanced
-directives\n\nYou can set a few other optional directives in the header line:
-\n\n- `tesh-exitcodes`: a list of exit codes in the order of commands executed
-inside the code block,\n- `tesh-setup`: a filename of a script to run before
-running the commands in the code block,\n- `tesh-ps1`: allow an additional PS1
-prompt besides the default `$`,\n- `tesh-platform`: specify on which platforms
-this session block should be tested (`linux`, `darwin`, `windows`),\n- `tesh-
-fixture`: a filename to save the current snippet,\n- `tesh-timeout`: number of
-seconds before a command timeouts (defaults to 30s),\n- `tesh-long-running`:
-set to `true` to showcase long-running commands such as `docker compose
-up`.\n\nLet\'s look at all of these through examples!\n\n### Testing exit
-codes\n\n`tesh-exitcodes` accepts a list of integers, which represent the exit
-code for every command in the block.\n\n~~~\n```console tesh-
-session="exitcodes" tesh-exitcodes="1 0"\n$ false\n\n$
-true\n\n```\n~~~\n\n\n### Test setup\n\nSometimes you need to do some test
-setup before running the examples in your code blocks. Put those [in a file](./
-readme.sh) and point to it with the `tesh-setup` directive.\n\n~~~\n```console
-tesh-session="setup" tesh-setup="readme.sh"\n$ echo "Hello $NAME!"\nHello
-Gaea!\n```\n~~~\n\n\n### Custom prompts\n\nEvery so often you need to drop into
-a virtualenv or similar shell that changes the prompt. `tesh` supports this via
-`test-ps1` directive.\n\n~~~\n```console tesh-session="prompt" tesh-ps1="(foo)
-$"\n$ PS1="(foo) $ "\n\n\n(foo) $ echo "hello"\nhello\n```\n~~~\n\n### Only run
-on certain platforms\n\nSome examples should only run on certain platforms, use
-`tesh-platform` to declare them as such.\n\n~~~\n```console tesh-
-session="platform" tesh-platform="linux"\n$
-uname\n...Linux...\n```\n~~~\n\n~~~\n```console tesh-session="platform" tesh-
-platform="darwin"\n$ uname\n...Darwin...\n```\n~~~\n\n### Dump file to
-disk\n\nOccasionally your examples consist of first showing contents of a file,
-then executing a command that uses said file. This is supported, use the `tesh-
-fixture` directive.\n\n~~~\n```bash tesh-session="fixture" tesh-
-fixture="foo.sh"\necho "foo"\n```\n~~~\n\n~~~\n```console tesh-
-session="fixture"\n$ chmod +x foo.sh\n\n$ ./foo.sh\nfoo\n```\n~~~\n\n### Custom
-timeout\n\nBy default, `tesh` will fail if an example command does not finish
-in 30 seconds. This number can be modified using the `tesh-timeout`
-directive.\n\n~~~\n```console tesh-session="timeout" tesh-timeout="3"\n$ sleep
-1\n\n```\n~~~\n\n\n### Long running processes\n\nSome processes that you want
-to show examples for are long-running processes, like `docker compose up`. They
-are supported in `tesh` blocks using the `tesh-long-running` directive. Note
-that they need to be the last command in the block.\n\n\n~~~\n```console tesh-
-session="long-running" tesh-timeout="1" tesh-long-running="true"\n$ nmap
-1.1.1.1\nStarting Nmap ...\n```\n~~~\n\n## Installation\n\nThe best way to
-install `tesh` is with your favorite Python package manager.\n\n```bash\n$ pip
-install tesh\n```\n\n## Design decisions\n\n- Supports Linux / macOS.\n- Not
-tied to a specific markdown flavor or tooling.\n- Renders reasonably well on
-GitHub.\n\n\n## Comparison with other tools\n\n| | tesh | [mdsh](https://
-github.com/zimbatm/mdsh) | [pandoc filters](http://www.chriswarbo.net/projects/
-activecode/index.html) |\n|------------------------------------------|---|---|-
---|\n| Execute shell session | âï¸ | âï¸ | âï¸ |\n| Modify markdown
-file with the new output | ð§[[1]](https://github.com/OceanSprint/tesh/
-issues/6) | âï¸ | âï¸ |\n| Shared session between code blocks | âï¸ |
-âï¸ | âï¸ |\n| Custom PS1 prompts | âï¸ | âï¸ | âï¸ |\n| Assert
-non-zero exit codes | âï¸ | âï¸ | âï¸ |\n| Setup the shell environment
-| âï¸ | âï¸ | âï¸ |\n| Reference fixtures from other snippets | âï¸
-| âï¸ | âï¸ |\n| Wildcard matching of the command output | âï¸ |
-âï¸ | âï¸ |\n| Starts the shell in debugging mode | âï¸ | âï¸ |
-âï¸ |\n| Specify timeout | âï¸ | âï¸ | âï¸ |\n| Support long-
-running commands | âï¸ | âï¸ | âï¸ |\n\n* âï¸: Supported\n* C:
-Possible but you have to write some code yourself\n* ð§: Under development\n*
-âï¸: Not supported\n* ?: I don\'t know.\n\n\n## Developing `tesh`\n\nYou
-need to have [poetry](https://python-poetry.org/) and Python 3.9 through 3.11
-installed on your machine.\n\nAlternatively, if you use [nix](https://nix.dev/
-tutorials/declarative-and-reproducible-developer-environments), run `nix-shell`
-to drop into a shell that has everything prepared for development.\n\nThen you
-can run `make tests` to run all tests & checks. Additional `make` commands are
-available:\n\n```\n# run tesh on all Markdown files\n$ make tesh\n\n# run
-flake8 linters on changed files only\n$ make lint\n\n# run flake8 linters on
-all files\n$ make lint all=true\n\n# run mypy type checker\n$ make types\n\n#
-run unit tests\n$ make unit\n\n# run a subset of unit tests (regex find)\n$
-make unit filter=foo\n\n# re-lock Python dependencies (for example after adding
-or removing one from pyproject.toml)\n$ make lock\n```\n', 'author': 'Domen
-Kozar', 'author_email': 'None', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'None', 'package_dir': package_dir, 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'entry_points': entry_points, 'python_requires': '>=3.9,<4.0', } setup
-(**setup_kwargs)
+multiple code blocks to share the same session. ~~~ ```console tesh-
+session="multiple_blocks" $ export NAME=Earth ``` ~~~ ~~~ ```console tesh-
+session="multiple_blocks" $ echo "Hello $NAME!" Hello Earth! ``` ~~~ ###
+Ignoring parts of the output Parts of the inline output can be ignored with
+`...`: ~~~ ```console tesh-session="ignore" $ echo "Hello from Space!" Hello
+... Space! ``` ~~~ The same can be done for multiple lines of output. Note that
+trailing whitespace in every line is trimmed. ~~~ ```console tesh-
+session="ignore" $ printf "Hello \nthere \nfrom \nSpace!" Hello ... Space! ```
+~~~ Commands can continue across multiple lines by prefixing lines with `> `.
+~~~ ```console tesh-session="ignore" $ echo "Hello from" \ > "another" \ >
+"line!" Hello from another line! ``` ~~~ ## Advanced directives You can set a
+few other optional directives in the header line: - `tesh-exitcodes`: a list of
+exit codes in the order of commands executed inside the code block, - `tesh-
+setup`: a filename of a script to run before running the commands in the code
+block, - `tesh-ps1`: allow an additional PS1 prompt besides the default `$`, -
+`tesh-platform`: specify on which platforms this session block should be tested
+(`linux`, `darwin`, `windows`), - `tesh-fixture`: a filename to save the
+current snippet, - `tesh-timeout`: number of seconds before a command timeouts
+(defaults to 30s), - `tesh-long-running`: set to `true` to showcase long-
+running commands such as `docker compose up`. Let's look at all of these
+through examples! ### Testing exit codes `tesh-exitcodes` accepts a list of
+integers, which represent the exit code for every command in the block. ~~~
+```console tesh-session="exitcodes" tesh-exitcodes="1 0" $ false $ true ``` ~~~
+### Test setup Sometimes you need to do some test setup before running the
+examples in your code blocks. Put those [in a file](./readme.sh) and point to
+it with the `tesh-setup` directive. ~~~ ```console tesh-session="setup" tesh-
+setup="readme.sh" $ echo "Hello $NAME!" Hello Gaea! ``` ~~~ ### Custom prompts
+Every so often you need to drop into a virtualenv or similar shell that changes
+the prompt. `tesh` supports this via `test-ps1` directive. ~~~ ```console tesh-
+session="prompt" tesh-ps1="(foo) $" $ PS1="(foo) $ " (foo) $ echo "hello" hello
+``` ~~~ ### Only run on certain platforms Some examples should only run on
+certain platforms, use `tesh-platform` to declare them as such. ~~~ ```console
+tesh-session="platform" tesh-platform="linux" $ uname ...Linux... ``` ~~~ ~~~
+```console tesh-session="platform" tesh-platform="darwin" $ uname ...Darwin...
+``` ~~~ ### Dump file to disk Occasionally your examples consist of first
+showing contents of a file, then executing a command that uses said file. This
+is supported, use the `tesh-fixture` directive. ~~~ ```bash tesh-
+session="fixture" tesh-fixture="foo.sh" echo "foo" ``` ~~~ ~~~ ```console tesh-
+session="fixture" $ chmod +x foo.sh $ ./foo.sh foo ``` ~~~ ### Custom timeout
+By default, `tesh` will fail if an example command does not finish in 30
+seconds. This number can be modified using the `tesh-timeout` directive. ~~~
+```console tesh-session="timeout" tesh-timeout="3" $ sleep 1 ``` ~~~ ### Long
+running processes Some processes that you want to show examples for are long-
+running processes, like `docker compose up`. They are supported in `tesh`
+blocks using the `tesh-long-running` directive. Note that they need to be the
+last command in the block. ~~~ ```console tesh-session="long-running" tesh-
+timeout="1" tesh-long-running="true" $ nmap 1.1.1.1 Starting Nmap ... ``` ~~~
+## Installation The best way to install `tesh` is with your favorite Python
+package manager. ```bash $ pip install tesh ``` ## Design decisions - Supports
+Linux / macOS. - Not tied to a specific markdown flavor or tooling. - Renders
+reasonably well on GitHub. ## Comparison with other tools | | tesh | [mdsh]
+(https://github.com/zimbatm/mdsh) | [pandoc filters](http://www.chriswarbo.net/
+projects/activecode/index.html) | |------------------------------------------|-
+--|---|---| | Execute shell session | âï¸ | âï¸ | âï¸ | | Modify
+markdown file with the new output | ð§[[1]](https://github.com/OceanSprint/
+tesh/issues/6) | âï¸ | âï¸ | | Shared session between code blocks |
+âï¸ | âï¸ | âï¸ | | Custom PS1 prompts | âï¸ | âï¸ | âï¸ | |
+Assert non-zero exit codes | âï¸ | âï¸ | âï¸ | | Setup the shell
+environment | âï¸ | âï¸ | âï¸ | | Reference fixtures from other
+snippets | âï¸ | âï¸ | âï¸ | | Wildcard matching of the command output
+| âï¸ | âï¸ | âï¸ | | Starts the shell in debugging mode | âï¸ |
+âï¸ | âï¸ | | Specify timeout | âï¸ | âï¸ | âï¸ | | Support
+long-running commands | âï¸ | âï¸ | âï¸ | * âï¸: Supported * C:
+Possible but you have to write some code yourself * ð§: Under development *
+âï¸: Not supported * ?: I don't know. ## Developing `tesh` You need to have
+[poetry](https://python-poetry.org/) and Python 3.9 through 3.11 installed on
+your machine. Alternatively, if you use [nix](https://nix.dev/tutorials/
+declarative-and-reproducible-developer-environments), run `nix-shell` to drop
+into a shell that has everything prepared for development. Then you can run
+`make tests` to run all tests & checks. Additional `make` commands are
+available: ``` # run tesh on all Markdown files $ make tesh # run flake8
+linters on changed files only $ make lint # run flake8 linters on all files $
+make lint all=true # run mypy type checker $ make types # run unit tests $ make
+unit # run a subset of unit tests (regex find) $ make unit filter=foo # re-lock
+Python dependencies (for example after adding or removing one from
+pyproject.toml) $ make lock ```
```

