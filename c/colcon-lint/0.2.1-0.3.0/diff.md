# Comparing `tmp/colcon-lint-0.2.1.tar.gz` & `tmp/colcon-lint-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colcon-lint-0.2.1.tar", last modified: Sat Jul  1 04:37:50 2023, max compression
+gzip compressed data, was "colcon-lint-0.3.0.tar", last modified: Sat Jul 29 06:01:44 2023, max compression
```

## Comparing `colcon-lint-0.2.1.tar` & `colcon-lint-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 04:37:50.683274 colcon-lint-0.2.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1547 2023-07-01 04:37:50.683274 colcon-lint-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1082 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 04:37:50.683274 colcon-lint-0.2.1/colcon_lint/
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/colcon_lint/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 04:37:50.683274 colcon-lint-0.2.1/colcon_lint/verb/
--rw-r--r--   0 root         (0) root         (0)      581 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/colcon_lint/verb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15415 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/colcon_lint/verb/lint_depends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 04:37:50.683274 colcon-lint-0.2.1/colcon_lint.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1547 2023-07-01 04:37:50.000000 colcon-lint-0.2.1/colcon_lint.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2023-07-01 04:37:50.000000 colcon-lint-0.2.1/colcon_lint.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 04:37:50.000000 colcon-lint-0.2.1/colcon_lint.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-01 04:37:50.000000 colcon-lint-0.2.1/colcon_lint.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-07-01 04:37:50.000000 colcon-lint-0.2.1/colcon_lint.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-01 04:37:50.000000 colcon-lint-0.2.1/colcon_lint.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      773 2023-07-01 04:37:50.683274 colcon-lint-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      620 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 04:37:50.683274 colcon-lint-0.2.1/test/
--rw-r--r--   0 root         (0) root         (0)     1577 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/test/test_cmake.py
--rw-r--r--   0 root         (0) root         (0)     1070 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/test/test_import.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/test/test_launch.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/test/test_setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:01:44.410220 colcon-lint-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-29 06:01:36.000000 colcon-lint-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-07-29 06:01:44.410220 colcon-lint-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-29 06:01:36.000000 colcon-lint-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:01:44.410220 colcon-lint-0.3.0/colcon_lint/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-29 06:01:36.000000 colcon-lint-0.3.0/colcon_lint/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:01:44.410220 colcon-lint-0.3.0/colcon_lint/verb/
+-rw-r--r--   0 root         (0) root         (0)      581 2023-07-29 06:01:36.000000 colcon-lint-0.3.0/colcon_lint/verb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17830 2023-07-29 06:01:36.000000 colcon-lint-0.3.0/colcon_lint/verb/lint_depends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:01:44.410220 colcon-lint-0.3.0/colcon_lint.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-07-29 06:01:44.000000 colcon-lint-0.3.0/colcon_lint.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2023-07-29 06:01:44.000000 colcon-lint-0.3.0/colcon_lint.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 06:01:44.000000 colcon-lint-0.3.0/colcon_lint.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-29 06:01:44.000000 colcon-lint-0.3.0/colcon_lint.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-29 06:01:44.000000 colcon-lint-0.3.0/colcon_lint.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-29 06:01:44.000000 colcon-lint-0.3.0/colcon_lint.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      773 2023-07-29 06:01:44.410220 colcon-lint-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      620 2023-07-29 06:01:36.000000 colcon-lint-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:01:44.410220 colcon-lint-0.3.0/test/
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-07-29 06:01:36.000000 colcon-lint-0.3.0/test/test_cmake.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-07-29 06:01:36.000000 colcon-lint-0.3.0/test/test_import.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-07-29 06:01:36.000000 colcon-lint-0.3.0/test/test_launch.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-07-29 06:01:36.000000 colcon-lint-0.3.0/test/test_setup.py
```

### Comparing `colcon-lint-0.2.1/LICENSE` & `colcon-lint-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `colcon-lint-0.2.1/README.md` & `colcon-lint-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 # colcon-lint
 
 Colcon extension for linting ROS package dependencies.
 
 This package is an extension of [colcon-core](https://github.com/colcon/colcon-core). Similar to [catkin-lint](https://github.com/fkie/catkin_lint) in ROS, it checks whether the dependencies of ROS2 packages are correctly described in the `package.xml`.
 
-Currently, the extension checks the `exec_depend` section and verifies the launch files and Python scripts' imports.
-The verification of `build_depend` is not yet implemented.
-However, it is recommended to use [ament_cmake_auto](https://github.com/ament/ament_cmake/tree/rolling/ament_cmake_auto) to verify that there are no build errors.
-
 ## Installation
 
 To use this extension, please execute the following:
 
 ```bash
-git clone https://github.com/Tacha-S/colcon-lint.git
-cd colcon-lint
-sudo pip install .
+sudo apt install apt-rdepends
+pip install colcon-lint
 ```
 
 ## How to use
 
 Please execute as follows. The package specification option is the same as other colcon commands.
 
 ```bash
 colcon lint --packages-select <package-name>
 ```
 
 Replace `<package-name>` with the name of the package you want to check.
+
+### Options
+
+| Option | Description |
+| --- | --- |
+| package specification options | The same as other colcon commands. |
+| logging options | The same as other colcon commands. |
+| `--quick` | This option only checks for directly declared dependencies in the package.xml. It cannot detect dependencies that are resolved through recursively declared packages. |
+
+## Tips
+
+To run faster, you can build with the `-Wno-dev --trace-expand --trace-redirect=trace.log` cmake option.
+
+```bash
+colcon build --cmake-args -Wno-dev --trace-expand --trace-redirect=trace.log
+```
```

### Comparing `colcon-lint-0.2.1/colcon_lint/__init__.py` & `colcon-lint-0.3.0/colcon_lint/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = '0.2.1'
+__version__ = '0.3.0'
```

### Comparing `colcon-lint-0.2.1/colcon_lint/verb/__init__.py` & `colcon-lint-0.3.0/colcon_lint/verb/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-lint-0.2.1/colcon_lint/verb/lint_depends.py` & `colcon-lint-0.3.0/colcon_lint/verb/lint_depends.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import argparse
 import ast
+import os
 import pathlib
 import re
 import shutil
 import subprocess
 from xml.etree import ElementTree
 
 from colcon_core.command import CommandContext
@@ -52,19 +53,21 @@
 class LintVerb(VerbExtensionPoint):
     def __init__(self) -> None:
         super().__init__()
 
     def add_arguments(self, *, parser: argparse.ArgumentParser) -> None:
         add_packages_arguments(parser)
         add_log_level_argument(parser)
+        parser.add_argument('--quick', action='store_true', help='quick check', default=False, required=False)
 
     def main(self, *, context: CommandContext) -> int:
         descriptors = get_package_descriptors(context.args, additional_argument_names=['*'])
         decorators = topological_order_packages(descriptors, recursive_categories=('run', ))
         select_package_decorators(context.args, decorators)
+        self.quick_check = context.args.quick
 
         rc = 0
         for decorator in decorators:
             if not decorator.selected:
                 continue
             pkg = decorator.descriptor
             pkg_path = pathlib.Path(FindPackageShare(pkg.name).find(pkg.name)) / 'launch'
@@ -141,40 +144,84 @@
             root = tree.getroot()
             described_buildtool_depends = set([dep.text for dep in root.iter('buildtool_depend')])
             described_build_depends = set([dep.text for dep in root.iter('build_depend')])
             described_build_export_depends = set([dep.text for dep in root.iter('build_export_depend')])
             described_test_depends = set([dep.text for dep in root.iter('test_depend')])
             described_exec_depends = set([dep.text for dep in root.iter('exec_depend')])
             described_depends = set([dep.text for dep in root.iter('depend')])
-            for dep in buildtool_depends - described_depends - described_buildtool_depends - set([pkg.name]):
+            apt_depends = set()
+            apt_buildtool_depends = set()
+            apt_build_depends = set()
+            apt_build_export_depends = set()
+            apt_test_depends = set()
+            apt_exec_depends = set()
+            if self.quick_check:
+                apt_depends = self.list_up_apt_depends(described_depends)
+                apt_buildtool_depends = self.list_up_apt_depends(described_buildtool_depends)
+                apt_build_depends = self.list_up_apt_depends(described_build_depends)
+                apt_build_export_depends = self.list_up_apt_depends(described_build_export_depends)
+                apt_test_depends = self.list_up_apt_depends(described_test_depends)
+                apt_exec_depends = self.list_up_apt_depends(described_exec_depends)
+            for dep in buildtool_depends - described_depends - described_buildtool_depends \
+                    - apt_depends - apt_buildtool_depends - set([pkg.name]):
                 logger.warn(f'[{pkg.name}] {dep} should add to buildtool_depend.')
                 rc = 1
-            for dep in build_depends - described_depends - described_build_depends - set([pkg.name]):
+            for dep in build_depends - described_depends - described_build_depends \
+                    - apt_depends - apt_build_depends - set([pkg.name]):
                 logger.warn(f'[{pkg.name}] {dep} should add to build_depend.')
                 rc = 1
-            for dep in build_export_depends - described_depends - described_build_export_depends - set([pkg.name]):
+            for dep in build_export_depends - described_depends - described_build_export_depends \
+                    - apt_depends - apt_build_export_depends - set([pkg.name]):
                 logger.warn(f'[{pkg.name}] {dep} should add to build_export_depend.')
                 rc = 1
-            for dep in test_depends - described_depends - described_test_depends - set([pkg.name]):
+            for dep in test_depends - described_depends - described_test_depends \
+                    - apt_depends - apt_test_depends - set([pkg.name]):
                 logger.warn(f'[{pkg.name}] {dep} should add to test_depend.')
                 rc = 1
-            for dep in exec_depends - described_depends - described_exec_depends - set([pkg.name]):
+            for dep in exec_depends - described_depends - described_exec_depends \
+                    - apt_depends - apt_exec_depends - set([pkg.name]):
                 logger.warn(f'[{pkg.name}] {dep} should add to exec_depend.')
                 rc = 1
             for dep in depends - described_depends - \
-                    (described_build_depends & described_exec_depends) - set([pkg.name]):
+                    (described_build_depends & described_exec_depends) - apt_depends - set([pkg.name]):
                 logger.warn(f'[{pkg.name}] {dep} should add to depend.')
                 rc = 1
             described = described_depends | described_buildtool_depends | described_build_depends | \
                 described_build_export_depends | described_test_depends | described_exec_depends
-            for dep in described - depends - buildtool_depends - \
-                    build_depends - build_export_depends - test_depends - exec_depends - set([pkg.name]):
-                logger.warn(f'[{pkg.name}] {dep} cannot be resolved.')
+            implicitly = described - depends - buildtool_depends - \
+                build_depends - build_export_depends - test_depends - exec_depends - set([pkg.name])
+            if implicitly:
+                logger.info(
+                    f'[{pkg.name}] {implicitly} are not included in the explicit dependencies. It may not be necessary.'
+                )
         return rc
 
+    def list_up_apt_depends(self, packages: set[str]) -> set[str]:
+        if shutil.which('apt-rdepends') is None:
+            logger.warn('apt-rdepends is not installed.')
+            return set()
+        result = subprocess.run(["rosdep", "resolve"] + list(packages), capture_output=True, text=True)
+        if result.returncode != 0:
+            return set()
+        pattern = re.compile("#apt\n([^\\s]+)\n")
+        resolved = pattern.findall(result.stdout)
+        result2 = subprocess.run(
+            ["apt-rdepends", "-p", "--follow=Depends,PreDepends,Recommends", "--show=Depends,PreDepends,Recommends"]
+            + resolved,
+            capture_output=True,
+            text=True)
+        if result2.returncode != 0:
+            return set()
+
+        pattern = re.compile("\n([^\\s]+)\n")
+        return set([
+            name.removeprefix(f'ros-{os.getenv("ROS_DISTRO")}-').replace('-', '_')
+            if name.startswith(f'ros-{os.getenv("ROS_DISTRO")}-') else name for name in pattern.findall(result2.stdout)
+        ])
+
     def resolve_python_package(self, package: str) -> bool:
         lookup = RosdepLookup.create_from_rospkg()
         return len(lookup.get_views_that_define(package)) > 0
 
     def resolve_launch_depends(self, path: pathlib.Path) -> set:
         depends = set()
         description = get_launch_description_from_python_launch_file(str(path))
```

### Comparing `colcon-lint-0.2.1/setup.cfg` & `colcon-lint-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `colcon-lint-0.2.1/setup.py` & `colcon-lint-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `colcon-lint-0.2.1/test/test_cmake.py` & `colcon-lint-0.3.0/test/test_cmake.py`

 * *Files identical despite different names*

### Comparing `colcon-lint-0.2.1/test/test_import.py` & `colcon-lint-0.3.0/test/test_import.py`

 * *Files identical despite different names*

### Comparing `colcon-lint-0.2.1/test/test_launch.py` & `colcon-lint-0.3.0/test/test_launch.py`

 * *Files identical despite different names*

### Comparing `colcon-lint-0.2.1/test/test_setup.py` & `colcon-lint-0.3.0/test/test_setup.py`

 * *Files identical despite different names*

