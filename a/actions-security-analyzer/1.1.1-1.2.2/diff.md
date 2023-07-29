# Comparing `tmp/actions_security_analyzer-1.1.1.tar.gz` & `tmp/actions_security_analyzer-1.2.2.tar.gz`

## Comparing `actions_security_analyzer-1.1.1.tar` & `actions_security_analyzer-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,30 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/__about__.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/colors.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/main.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/requirements.txt
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-using-configure-aws-creds-non-oidc-auth.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-using-github-cache.yml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-using-self-hosted-runner-in-matrix.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-using-self-hosted-runner-referenced-by-group.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-using-self-hosted-runners.yml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-dangerous-gh-context-variables.yml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-dangerous-gh-variables-2.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-dangerous-gh-variables.yml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-inline-script.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-pull-request-target.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-unsecure-command-env-var.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-write-all-permissions.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-write-permissions-all-jobs.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/actions/action-with-write-permissions-one-job.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/analyzer/__init__.py
--rw-r--r--   0        0        0    11295 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/analyzer/analyzer.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/analyzer/analyzer_test.py
--rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/images/asa-stdout.png
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/LICENSE
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/README.md
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/__about__.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/action.yml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/colors.py
+-rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/main.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/requirements.txt
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/.github/workflows/asa-scan.yml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/actions/action-that-creates-or-approves-pr.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/actions/action-using-configure-aws-creds-non-oidc-auth.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/actions/action-using-github-cache.yml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/actions/action-using-self-hosted-runner-in-matrix.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/actions/action-using-self-hosted-runner-referenced-by-group.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/actions/action-using-self-hosted-runners.yml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/actions/action-with-dangerous-gh-context-variables.yml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/actions/action-with-dangerous-gh-variables-2.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/actions/action-with-dangerous-gh-variables.yml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/actions/action-with-inline-script.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/actions/action-with-pull-request-target.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/actions/action-with-unsecure-command-env-var.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/actions/action-with-write-all-permissions.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/actions/action-with-write-permissions-all-jobs.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/actions/action-with-write-permissions-one-job.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/analyzer/__init__.py
+-rw-r--r--   0        0        0    12015 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/analyzer/analyzer.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/analyzer/analyzer_test.py
+-rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/images/asa-stdout.png
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/LICENSE
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/README.md
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 actions_security_analyzer-1.2.2/PKG-INFO
```

### Comparing `actions_security_analyzer-1.1.1/colors.py` & `actions_security_analyzer-1.2.2/colors.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.1/main.py` & `actions_security_analyzer-1.2.2/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,30 +40,38 @@
     parser.add_argument("--verbose", "-v", action="store_true", help="increase tool verbosity")
     parser.add_argument(
         "--ignore-warnings",
         "-i",
         action="store_true",
         help="ignore checks labeled as warning",
     )
+    parser.add_argument(
+        "--ignore-checks",
+        "-k",
+        nargs="+",
+        metavar="CHECK",
+        help="specify checks to ignore",
+    )
     parser.add_argument("--no-summary", "-n", action="store_true", help="don't show tool summary section")
     return parser.parse_args()
 
 
 def _main():
     _rewrite_pyyaml_boolean_recognition_rules()
     args = _parse_args()
 
     file_ = args.file
     dir_ = args.dir
     list_checks = args.list_checks
     verbose = args.verbose
     ignore_warnings = args.ignore_warnings
+    ignore_checks = args.ignore_checks
     no_summary = args.no_summary
 
-    analyzer = Analyzer(ignore_warnings=ignore_warnings, verbose=verbose)
+    analyzer = Analyzer(ignore_checks=ignore_checks, ignore_warnings=ignore_warnings, verbose=verbose)
 
     errored = False
     failed_actions = []
     try:
         if file_:
             file_ = Path(file_)
             if file_.exists():
```

### Comparing `actions_security_analyzer-1.1.1/actions/action-using-configure-aws-creds-non-oidc-auth.yml` & `actions_security_analyzer-1.2.2/actions/action-using-configure-aws-creds-non-oidc-auth.yml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.1/analyzer/analyzer.py` & `actions_security_analyzer-1.2.2/analyzer/analyzer.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,44 +5,50 @@
 
 class Analyzer:
     """Analyzer contains all the checks that will run
     against a specified GitHub Action parsed into a Python
     dictionary.
     """
 
-    def __init__(self, verbose: bool = False, ignore_warnings: bool = False) -> None:
-        self.verbose = verbose
+    def __init__(
+        self,
+        ignore_checks: list,
+        ignore_warnings: bool = False,
+        verbose: bool = False,
+    ) -> None:
         self.ignore_warnings = ignore_warnings
+        self.ignore_checks = ignore_checks or []
+        self.verbose = verbose
         self.checks = {
             "_check_for_3p_actions_without_hash": {"level": "FAIL"},
             "_check_for_allow_unsecure_commands": {"level": "FAIL"},
             "_check_for_cache_action_usage": {"level": "WARN"},
             "_check_for_dangerous_write_permissions": {"level": "FAIL"},
             "_check_for_inline_script": {"level": "WARN"},
             "_check_for_pull_request_target": {"level": "FAIL"},
             "_check_for_script_injection": {"level": "FAIL"},
             "_check_for_self_hosted_runners": {"level": "WARN"},
             "_check_for_aws_configure_credentials_non_oidc": {"level": "WARN"},
+            "_check_for_pull_request_create_or_approve": {"level": "FAIL"},
         }
         self.action = {}
 
     def _print_failed_check_msg(self, check: str, level: str):
+        c = None
         if level == "FAIL":
-            level_color = Colors.RED
+            c = Colors.RED
         elif level == "WARN":
-            level_color = Colors.LIGHT_GREEN
-        else:
-            level_color = Colors.LIGHT_PURPLE
+            c = Colors.LIGHT_GREEN
         print(
-            f"{level_color}{level}{Colors.END} {Colors.YELLOW}{check[1:]}{Colors.END}",
+            f"{c}{level}{Colors.END} {Colors.YELLOW}{check[1:]}{Colors.END}",
         )
 
     def _action_has_required_elements(self) -> bool:
         passed = True
-        # a check for "permissions" is not done here because it is not required
+        # NOTE: a check for "permissions" is not done here because it is not required
         if not all(key in self.action for key in ["name", "on", "jobs"]):
             passed = False
         for job in self.jobs.keys():
             if "steps" not in self.jobs[job]:
                 passed = False
                 break
         return passed
@@ -164,15 +170,15 @@
                             )
                         passed = False
                         return passed
         return passed
 
     def _check_for_self_hosted_runners(self) -> bool:
         passed = True
-        # ***** default runners as of 7/17/23 *****
+        # NOTE: ***** default runners as of 7/17/23 *****
         default_runners = [
             "windows-latest",
             "windows-2022",
             "windows-2019",
             "ubuntu-latest",
             "ubuntu-22.04",
             "ubuntu-20.04",
@@ -206,17 +212,17 @@
                             break
                 elif type_of_runs_on == str:
                     if runs_on not in default_runners:
                         passed = False
                         break
         return passed
 
-    def _check_for_aws_configure_credentials_non_oidc(self):
+    def _check_for_aws_configure_credentials_non_oidc(self) -> bool:
         passed = True
-        # if these are specifed in the configure-aws-credentials action
+        # NOTE: if these are specifed in the configure-aws-credentials action
         # then the action will not use GitHub's OIDC provider
         # see this: https://github.com/aws-actions/configure-aws-credentials#assuming-a-role
         CONFIGURE_AWS_CREDS_ACTION_REGEX = (
             r"aws\-actions\/configure\-aws\-credentials@(v\d+(\.\d+)?(\.\d+)?|[a-f0-9]{40})"
         )
         non_oidc_inputs = [
             "aws-access-key-id",
@@ -233,43 +239,49 @@
                                 print(
                                     f"{Colors.LIGHT_GRAY}INFO{Colors.END} found step('{step['name']}') not using OIDC with `configure-aws-credentials`"
                                 )
                         if passed:
                             passed = False
         return passed
 
-    def get_checks(self) -> list:
-        """Returns all available checks performed against
-        provided GitHub Action.
+    def _check_for_pull_request_create_or_approve(self) -> bool:
+        passed = True
+        GH_CLI_PR_APPROVAL_REGEX = f"gh pr (review.*--approve|create.*)"
+        # TODO: add checks for alternatives ways to create/approve pull request
+        # e.g. via curl or github script ('actions/github-script')
+        for job in self.jobs:
+            steps = self.jobs[job]["steps"]
+            for step in steps:
+                if "run" in step:
+                    script = step["run"]
+                    match = search(GH_CLI_PR_APPROVAL_REGEX, script)
+                    if match:
+                        if self.verbose:
+                            print(
+                                f"{Colors.LIGHT_GRAY}INFO{Colors.END} job('{job}') has a step('{step['name']}') that creates or approves a pull request"
+                            )
+                        passed = False
+        return passed
 
-        Returns:
-            list: all available checks performed by Analzyer
-        """
+    def get_checks(self) -> list:
         return [*self.checks.keys()]
 
     def run_checks(self, action: dict) -> bool:
-        """Run all checks against a GitHub Action
-
-        Args:
-            action (dict): the dict representation of the Action YAML file.
-
-        Returns:
-            bool: returns False if any checks fails.
-        """
-
         self.action = action
         self.jobs = self.action["jobs"]
 
         passed_all_checks = True
         fail_checks = []
         if self._action_has_required_elements():
             for check in self.checks.keys():
                 if self.ignore_warnings:
                     if self.checks[check]["level"] == "WARN":
                         continue
+                if check[1:] in self.ignore_checks:
+                    continue
                 if not Analyzer.__dict__[check](self):
                     fail_checks.append(check)
                     if passed_all_checks:
                         passed_all_checks = False
             for check in fail_checks:
                 self._print_failed_check_msg(check, self.checks[check]["level"])
         return passed_all_checks
```

### Comparing `actions_security_analyzer-1.1.1/analyzer/analyzer_test.py` & `actions_security_analyzer-1.2.2/analyzer/analyzer_test.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.1/images/asa-stdout.png` & `actions_security_analyzer-1.2.2/images/asa-stdout.png`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.1/.gitignore` & `actions_security_analyzer-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.1/LICENSE` & `actions_security_analyzer-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.1/README.md` & `actions_security_analyzer-1.2.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -16,14 +16,40 @@
 ```
 asa --file action.yml
 asa -d directory-with-actions/ --verbose
 asa --file action.yml --ignore-warnings
 asa --list-checks
 ```
 
+### Use `asa` in Your GitHub Workflows
+
+#### Example
+
+```yaml
+name: 'RunActionsSecurityAnalzyer'
+on:
+  push:
+    branches:
+      - main
+      - dev
+jobs:
+  RunAsa:
+    runs-on: ubuntu-latest
+    steps:
+    - name: "Checkout repo"
+      uses: actions/checkout@96f53100ba2a5449eb71d2e6604bbcd94b9449b5 # v3.5.3
+    - name: "Run asa scanner"
+      uses: "bin3xish477/asa@a6f5eb8c20e936c07326a1eb6aa6427b25494045"
+      with:
+        dir: "./actions/"
+        verbose: true
+        no-summary: true
+        ignore-checks: 'check_for_inline_script check_for_cache_action_usage'
+```
+
 ### Checks Performed by `asa`
 
 1. Name: `check_for_3p_actions_without_hash`, Level: `FAIL`
 
     - This check identifies any third-party GitHub Actions in use that have been referenced via a version number such as `v1.1` instead of commit SHA haah. Using a hash can help mitigate supply chain threats in a scenario where a threat actor has compromised the source repository where the 3P action lives.
 
 2. Name: `check_for_allow_unsecure_commands`, Level: `FAIL`
@@ -54,10 +80,14 @@
 
     - This checks attempts to identify the usage of self-hosted runners. Self-hosted runners are dangerous because if the Action is compromised it may allow a threat actor to gain access to on premise environment or establish persistence mechanisms on a server you own/rent.
 
 9. Name: `check_for_aws_configure_credentials_non_oidc`, Level: `WARN`
 
     - This checks looks for the usage of AWS's `aws-actions/configure-aws-credentials` action and attempts to identify non-OIDC authentication parameters. Non-OIDC authentication types are less secure than OIDC because they require the creation of long-term credentials which can be compromised, however, OIDC tokens are short-lived and are usually scoped to only the permissions that are essential to a workflow and thus help reduce the attack surface.
 
+10. Name: `check_for_pull_request_create_or_approve`, Level: `WARN`
+
+    - This check looks for Action that have logic related to creating or improving pull requests. Creating or approving pull requests via automation poses a security risk if sufficient controls aren't in place to protect against malicious code being merged into a repository.
+
 ### References
 
 - [Security hardening for GitHub Actions](https://docs.github.com/en/actions/security-guides/security-hardening-for-github-actions)
```

### Comparing `actions_security_analyzer-1.1.1/pyproject.toml` & `actions_security_analyzer-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.1.1/PKG-INFO` & `actions_security_analyzer-1.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actions-security-analyzer
-Version: 1.1.1
+Version: 1.2.2
 Summary: Analyze the security posture of one or more GitHub Actions
 Project-URL: Documentation, https://github.com/bin3xish477/asa#readme
 Project-URL: Issues, https://github.com/bin3xish477/asa/issues
 Project-URL: Source, https://github.com/bin3xish477/asa
 Author-email: Alexis Rodriguez <arodriguez99@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -43,14 +43,40 @@
 ```
 asa --file action.yml
 asa -d directory-with-actions/ --verbose
 asa --file action.yml --ignore-warnings
 asa --list-checks
 ```
 
+### Use `asa` in Your GitHub Workflows
+
+#### Example
+
+```yaml
+name: 'RunActionsSecurityAnalzyer'
+on:
+  push:
+    branches:
+      - main
+      - dev
+jobs:
+  RunAsa:
+    runs-on: ubuntu-latest
+    steps:
+    - name: "Checkout repo"
+      uses: actions/checkout@96f53100ba2a5449eb71d2e6604bbcd94b9449b5 # v3.5.3
+    - name: "Run asa scanner"
+      uses: "bin3xish477/asa@a6f5eb8c20e936c07326a1eb6aa6427b25494045"
+      with:
+        dir: "./actions/"
+        verbose: true
+        no-summary: true
+        ignore-checks: 'check_for_inline_script check_for_cache_action_usage'
+```
+
 ### Checks Performed by `asa`
 
 1. Name: `check_for_3p_actions_without_hash`, Level: `FAIL`
 
     - This check identifies any third-party GitHub Actions in use that have been referenced via a version number such as `v1.1` instead of commit SHA haah. Using a hash can help mitigate supply chain threats in a scenario where a threat actor has compromised the source repository where the 3P action lives.
 
 2. Name: `check_for_allow_unsecure_commands`, Level: `FAIL`
@@ -81,10 +107,14 @@
 
     - This checks attempts to identify the usage of self-hosted runners. Self-hosted runners are dangerous because if the Action is compromised it may allow a threat actor to gain access to on premise environment or establish persistence mechanisms on a server you own/rent.
 
 9. Name: `check_for_aws_configure_credentials_non_oidc`, Level: `WARN`
 
     - This checks looks for the usage of AWS's `aws-actions/configure-aws-credentials` action and attempts to identify non-OIDC authentication parameters. Non-OIDC authentication types are less secure than OIDC because they require the creation of long-term credentials which can be compromised, however, OIDC tokens are short-lived and are usually scoped to only the permissions that are essential to a workflow and thus help reduce the attack surface.
 
+10. Name: `check_for_pull_request_create_or_approve`, Level: `WARN`
+
+    - This check looks for Action that have logic related to creating or improving pull requests. Creating or approving pull requests via automation poses a security risk if sufficient controls aren't in place to protect against malicious code being merged into a repository.
+
 ### References
 
 - [Security hardening for GitHub Actions](https://docs.github.com/en/actions/security-guides/security-hardening-for-github-actions)
```

