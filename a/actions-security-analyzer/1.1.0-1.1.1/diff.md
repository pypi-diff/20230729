# Comparing `tmp/actions_security_analyzer-1.1.0.tar.gz` & `tmp/actions_security_analyzer-1.1.1.tar.gz`

## Comparing `actions_security_analyzer-1.1.0.tar` & `actions_security_analyzer-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/__about__.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/colors.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/main.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/requirements.txt
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-using-configure-aws-creds-non-oidc-auth.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-using-github-cache.yml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-using-self-hosted-runner-in-matrix.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-using-self-hosted-runner-referenced-by-group.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-using-self-hosted-runners.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-with-dangerous-gh-context-variables.yml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-with-inline-script.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-with-pull-request-target.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-with-unsecure-command-env-var.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-with-write-all-permissions.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-with-write-permissions-all-jobs.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-with-write-permissions-one-job.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/analyzer/__init__.py
--rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/analyzer/analyzer.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/analyzer/analyzer_test.py
--rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/images/asa-stdout.png
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/LICENSE
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/README.md
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/__about__.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/colors.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/main.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/requirements.txt
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-using-configure-aws-creds-non-oidc-auth.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-using-github-cache.yml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-using-self-hosted-runner-in-matrix.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-using-self-hosted-runner-referenced-by-group.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-using-self-hosted-runners.yml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-dangerous-gh-context-variables.yml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-dangerous-gh-variables-2.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-dangerous-gh-variables.yml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-inline-script.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-pull-request-target.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-unsecure-command-env-var.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-write-all-permissions.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-write-permissions-all-jobs.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-write-permissions-one-job.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/analyzer/__init__.py
+-rw-r--r--   0        0        0    11295 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/analyzer/analyzer.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/analyzer/analyzer_test.py
+-rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/images/asa-stdout.png
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/README.md
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/PKG-INFO
```

### Comparing `actions_security_analyzer-1.1.0/colors.py` & `actions_security_analyzer-1.1.1/colors.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.0/main.py` & `actions_security_analyzer-1.1.1/main.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.0/actions/action-using-configure-aws-creds-non-oidc-auth.yml` & `actions_security_analyzer-1.1.1/actions/action-using-configure-aws-creds-non-oidc-auth.yml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.0/analyzer/analyzer.py` & `actions_security_analyzer-1.1.1/analyzer/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """analyzer.py contains all the INFOic related to analyzing GitHub Actions"""
 from colors import Colors
-from re import match
+from re import search
 
 
 class Analyzer:
     """Analyzer contains all the checks that will run
     against a specified GitHub Action parsed into a Python
     dictionary.
     """
@@ -50,15 +50,15 @@
     def _check_for_3p_actions_without_hash(self) -> bool:
         passed = True
         ACTION_WITH_VERSION_REGEX = r"([\w-]+)\/([\w-]+)@v\d+(\.\d+)?(\.\d+)?"
         for job in self.jobs.keys():
             for step in self.jobs[job]["steps"]:
                 if "uses" in step:
                     uses = step["uses"]
-                    if match(ACTION_WITH_VERSION_REGEX, uses):
+                    if search(ACTION_WITH_VERSION_REGEX, uses):
                         if self.verbose:
                             print(
                                 f"{Colors.LIGHT_GRAY}INFO{Colors.END} step using action('{uses}') with version number instead of a SHA hash"
                             )
                         passed = False
                         break
         return passed
@@ -80,15 +80,15 @@
         passed = True
         DANGEROUS_GITHUB_CONTEXT_VARIABLE_REGEX = r"\$\{\{.*github.+\}\}"
         for job in self.jobs.keys():
             steps = self.jobs[job]["steps"]
             for step in steps:
                 if "run" in step:
                     script = step["run"]
-                    variable = match(DANGEROUS_GITHUB_CONTEXT_VARIABLE_REGEX, script)
+                    variable = search(DANGEROUS_GITHUB_CONTEXT_VARIABLE_REGEX, script)
                     if variable:
                         if self.verbose:
                             print(
                                 f"{Colors.LIGHT_GRAY}INFO{Colors.END} dangerous variable('{variable.group()}') in inline script"
                             )
                         passed = False
         return passed
@@ -121,15 +121,15 @@
     def _check_for_cache_action_usage(self) -> bool:
         passed = True
         CACHE_ACTION_REGEX = r"actions\/cache@(v\d+(\.\d+)?(\.\d+)?|[a-f0-9]{40})"
         for job in self.jobs.keys():
             steps = self.jobs[job]["steps"]
             for step in steps:
                 if "uses" in step:
-                    action = match(CACHE_ACTION_REGEX, step["uses"])
+                    action = search(CACHE_ACTION_REGEX, step["uses"])
                     if action:
                         if self.verbose:
                             print(
                                 f"{Colors.LIGHT_GRAY}INFO{Colors.END} job('{job}') is using cache action('{action.group()}')"
                             )
                         passed = False
         return passed
@@ -222,15 +222,15 @@
             "aws-access-key-id",
             "web-identity-token-file",
         ]
         for job in self.jobs.keys():
             steps = self.jobs[job]["steps"]
             for step in steps:
                 if "uses" in step:
-                    action = match(CONFIGURE_AWS_CREDS_ACTION_REGEX, step["uses"])
+                    action = search(CONFIGURE_AWS_CREDS_ACTION_REGEX, step["uses"])
                     if action:
                         if any(input in non_oidc_inputs for input in step["with"]):
                             if self.verbose:
                                 print(
                                     f"{Colors.LIGHT_GRAY}INFO{Colors.END} found step('{step['name']}') not using OIDC with `configure-aws-credentials`"
                                 )
                         if passed:
```

### Comparing `actions_security_analyzer-1.1.0/analyzer/analyzer_test.py` & `actions_security_analyzer-1.1.1/analyzer/analyzer_test.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.0/images/asa-stdout.png` & `actions_security_analyzer-1.1.1/images/asa-stdout.png`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.0/.gitignore` & `actions_security_analyzer-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.0/LICENSE` & `actions_security_analyzer-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.0/README.md` & `actions_security_analyzer-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.0/pyproject.toml` & `actions_security_analyzer-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.0/PKG-INFO` & `actions_security_analyzer-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actions-security-analyzer
-Version: 1.1.0
+Version: 1.1.1
 Summary: Analyze the security posture of one or more GitHub Actions
 Project-URL: Documentation, https://github.com/bin3xish477/asa#readme
 Project-URL: Issues, https://github.com/bin3xish477/asa/issues
 Project-URL: Source, https://github.com/bin3xish477/asa
 Author-email: Alexis Rodriguez <arodriguez99@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

