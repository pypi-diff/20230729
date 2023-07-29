# Comparing `tmp/vigilant_kit-1.2.7.tar.gz` & `tmp/vigilant_kit-1.2.8.tar.gz`

## Comparing `vigilant_kit-1.2.7.tar` & `vigilant_kit-1.2.8.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/.vigilant.env.example
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/vigilant.json.example
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/bin/doc_generator.py
--rw-r--r--   0        0        0    30712 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/actions.md
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/browser_options.md
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/configuration.md
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/native_selenium.md
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/selenium_install.md
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/tutorial_pytest.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/vigilant_pytest.md
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/docs/vigilant_unittest.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vgl_cli/install_dev_kit_command.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vgl_cli/install_standalone_command.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vgl_cli/install_webdriver_command.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vgl_cli/run_selenium_command.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vgl_cli/vgl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/actions/__init__.py
--rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/actions/assertions.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/actions/finder.py
--rw-r--r--   0        0        0    13552 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/actions/vigilant_actions.py
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/actions/waiter.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/driver/__init__.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/src/vigilant/driver/vigilant_driver.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/.gitignore
--rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/LICENSE
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/README.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 vigilant_kit-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/.vigilant.env.example
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/CHANGELOG.md
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/vigilant.json.example
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/bin/doc_generator.py
+-rw-r--r--   0        0        0    30712 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/docs/actions.md
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/docs/browser_options.md
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/docs/configuration.md
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/docs/native_selenium.md
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/docs/selenium_install.md
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/docs/tutorial_pytest.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/docs/vigilant_pytest.md
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/docs/vigilant_unittest.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/src/vgl_cli/install_dev_kit_command.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/src/vgl_cli/install_standalone_command.py
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/src/vgl_cli/install_webdriver_command.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/src/vgl_cli/selenium_commands.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/src/vgl_cli/vgl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/src/vigilant/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/src/vigilant/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/src/vigilant/actions/__init__.py
+-rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/src/vigilant/actions/assertions.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/src/vigilant/actions/finder.py
+-rw-r--r--   0        0        0    13552 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/src/vigilant/actions/vigilant_actions.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/src/vigilant/actions/waiter.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/src/vigilant/driver/__init__.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/src/vigilant/driver/vigilant_driver.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/.gitignore
+-rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/LICENSE
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/README.md
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 vigilant_kit-1.2.8/PKG-INFO
```

### Comparing `vigilant_kit-1.2.7/bin/doc_generator.py` & `vigilant_kit-1.2.8/bin/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/docs/actions.md` & `vigilant_kit-1.2.8/docs/actions.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/docs/browser_options.md` & `vigilant_kit-1.2.8/docs/browser_options.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/docs/configuration.md` & `vigilant_kit-1.2.8/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/docs/native_selenium.md` & `vigilant_kit-1.2.8/docs/native_selenium.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/docs/selenium_install.md` & `vigilant_kit-1.2.8/docs/selenium_install.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/docs/tutorial_pytest.md` & `vigilant_kit-1.2.8/docs/tutorial_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/docs/vigilant_pytest.md` & `vigilant_kit-1.2.8/docs/vigilant_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/docs/vigilant_unittest.md` & `vigilant_kit-1.2.8/docs/vigilant_unittest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/src/vgl_cli/install_dev_kit_command.py` & `vigilant_kit-1.2.8/src/vgl_cli/install_dev_kit_command.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 from .install_webdriver_command import check_version_and_download_driver
 from .install_standalone_command import check_req_and_install_selenium_server
 
 
 @click.command(name='dev-kit', help="Install local development kit (Webdriver, Selenium Server, etc)")
 @click.option('-b', '--browser', type=click.Choice(['chrome', 'firefox', 'edge']), required=True)
 def install_dev_kit(browser):
-    check_version_and_download_driver(browser)
     check_req_and_install_selenium_server()
+    check_version_and_download_driver(browser)
 
 
 if __name__ == "__main__":
     install_dev_kit()
```

### Comparing `vigilant_kit-1.2.7/src/vgl_cli/install_standalone_command.py` & `vigilant_kit-1.2.8/src/vgl_cli/install_standalone_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/src/vgl_cli/install_webdriver_command.py` & `vigilant_kit-1.2.8/src/vgl_cli/install_webdriver_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,20 +71,20 @@
     if download_url is not None:
         response = requests.get(download_url)
         if download_url.endswith(".zip"):
             with open(f"selenium-server/{browser}_driver.zip", "wb") as f:
                 f.write(response.content)
             with zipfile.ZipFile(f"selenium-server/{browser}_driver.zip", 'r') as zip_ref:
                 for member in zip_ref.namelist():
-                    zip_ref.extract(member, f"selenium-server/{browser}_driver/")
+                    zip_ref.extract(member, f"selenium-server/")
         elif download_url.endswith(".tar.gz"):
             with open(f"selenium-server/{browser}_driver.tar.gz", "wb") as f:
                 f.write(response.content)
             with tarfile.open(f"selenium-server/{browser}_driver.tar.gz", 'r:gz') as tar_ref:
-                tar_ref.extractall(f"selenium-server/{browser}_driver/")
+                tar_ref.extractall(f"selenium-server/")
     else:
         click.secho(f"Could not find download URL for {browser} driver.", fg="red")
 
 
 def check_version_and_download_driver(browser):
     version = get_browser_version(browser)
     if version is None:
```

### Comparing `vigilant_kit-1.2.7/src/vgl_cli/vgl.py` & `vigilant_kit-1.2.8/src/vgl_cli/vgl.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 #!/usr/bin/env python
 
 import click
 from .install_webdriver_command import install_webdriver
 from .install_standalone_command import install_selenium_standalone
 from .install_dev_kit_command import install_dev_kit
 
-from .run_selenium_command import run_selenium_server
+from .selenium_commands import run_selenium_server, stop_selenium_server
 
 
 @click.group(name="vgl.py")
 def vgl():
     pass
 
 
 @click.group(name="install", help="Install commands")
 def install_group():
     pass
 
 
-@click.group(name="run", help="Run commands")
-def run_group():
+@click.group(name="selenium", help="Run commands")
+def selenium_group():
     pass
 
 
-run_group.add_command(run_selenium_server)
+selenium_group.add_command(run_selenium_server)
+selenium_group.add_command(stop_selenium_server)
 
 
 install_group.add_command(install_webdriver)
 install_group.add_command(install_selenium_standalone)
 install_group.add_command(install_dev_kit)
 
 vgl.add_command(install_group)
-vgl.add_command(run_group)
+vgl.add_command(selenium_group)
 
 
 if __name__ == '__main__':
     vgl()
```

### Comparing `vigilant_kit-1.2.7/src/vigilant/actions/assertions.py` & `vigilant_kit-1.2.8/src/vigilant/actions/assertions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver import Remote
 
 from vigilant.actions.finder import Finder
 from vigilant.actions.waiter import Waiter
 from vigilant.logger import logger as log
 
+RED = "\033[31m"
+RESET = "\033[0m"
 
 class Assertions:
 
     def __init__(self, driver):
         self.driver: Remote = driver
         self.finder: Finder = Finder(self.driver)
         self.waiter: Waiter = Waiter(self.driver, self.finder)
@@ -44,99 +46,99 @@
 
         :param selectors: list of CSS selectors
         """
         if isinstance(selectors, list):
             for element in selectors:
                 log.info(f"Assert: don't see element with selector {element}")
                 assert self.count_visible_elements(element) == 0,\
-                    f"Expected 0 elements with selector {element}, but found {self.count_visible_elements(element)}"
+                    f"{RED}Expected 0 elements with selector {element}, but found {self.count_visible_elements(element)}{RESET}"
         else:
             log.info(f"Assert: don't see element with selector {selectors}")
             assert self.count_visible_elements(selectors) == 0, \
-                f"Expected 0 elements with selector {selectors}, but found {self.count_visible_elements(selectors)}"
+                f"{RED}Expected 0 elements with selector {selectors}, but found {self.count_visible_elements(selectors)}{RESET}"
 
     def dont_see_in_title(self, search_key: str) -> None:
         """
         Assert that the provided search key is not present in the current page title.
 
         :param search_key: string to search for
         """
         log.info(f"Assert: don't see string {search_key} in current page title")
         assert search_key not in self.driver.title, \
-            f"String {search_key} expected to to be missing in current page title but it appear"
+            f"{RED}String {search_key} expected to be missing in current page title, but it appears{RESET}"
 
     def dont_see_in_current_url(self, search_key: str) -> None:
         """
         Assert that the provided search key is not present in the current page URL.
 
         :param search_key: string to search for
         """
         log.info(f"Assert: don't see string {search_key} in current page URL")
         assert search_key not in self.driver.current_url, \
-            f"String {search_key} expected to to be missing in current page URL but it appear"
+            f"{RED}String {search_key} expected to to be missing in current page URL, but it appear{RESET}"
 
     def see(self, selectors: [str | list]) -> None:
         """
         Assert that at least one of the elements matching the provided selectors is visible.
 
         :param selectors: list of CSS selectors
         """
         if isinstance(selectors, list):
             for element in selectors:
                 log.info(f"Assert: see element with selector {element}")
                 assert self.count_visible_elements(element) > 0,\
-                    f"Expected 1 element with selector {element}, but found {self.count_visible_elements(element)}"
+                    f"{RED}Expected 1 element with selector {element}, but found {self.count_visible_elements(element)}{RESET}"
         else:
             log.info(f"Assert: see element with selector {selectors}")
             assert self.count_visible_elements(selectors) > 0, \
-                f"Expected 1 element with selector {selectors}, but found {self.count_visible_elements(selectors)}"
+                f"{RED}Expected 1 element with selector {selectors}, but found {self.count_visible_elements(selectors)}{RESET}"
 
     def see_elements_in_quantity_of(self, selector: str, qty: int):
         """
         Assert that the number of visible elements that match the provided selector is equal to the provided quantity.
 
         :param selector: CSS selector
         :param qty: expected number of elements
         """
         log.info(f"Assert: see elements with selector {selector} in quantity of {qty}")
         assert qty == self.count_visible_elements(selector), \
-            f"Expected {qty} elements with selector {selector}, but found {self.count_visible_elements(selector)}"
+            f"{RED}Expected {qty} elements with selector {selector}, but found {self.count_visible_elements(selector)}{RESET}"
 
     def see_at_least_one(self, selector):
         """
         Assert that at least one element matching the provided selector is visible.
 
         :param selector: CSS selector
         """
         log.info(f"Assert: see at least 1 element with selector {selector}")
         assert self.count_visible_elements(selector) > 1, \
-            f"Expected quantity of elements with selector {selector} be at least 1, but found {self.count_visible_elements(selector)}"
+            f"{RED}Expected quantity of elements with selector {selector} be at least 1, but found {self.count_visible_elements(selector)}{RESET}"
 
     def see_in_title(self, search_key):
         """
         Assert that the provided search key is present in the current page title.
 
         :param search_key: string to search for
         """
         log.info(f"Assert: see string {search_key} in current page title")
         assert search_key in self.driver.title, \
-            f"String {search_key} expected to to be in current page title but it is missing"
+            f"{RED}String {search_key} expected to be in current page title, but it is missing{RESET}"
 
     def see_in_url(self, search_key: str):
         """
         Assert that the provided search key is present in the current page URL.
 
         :param search_key: string to search for
         """
         log.info(f"Assert: see string {search_key} in current page URL")
         assert search_key in self.driver.current_url, \
-            f"String {search_key} expected to to be in current page URL but it is missing"
+            f"{RED}String {search_key} expected to be in current page URL, but it is missing{RESET}"
 
     def see_text(self, text):
         """
         Assert that the provided text is present on the current page.
 
         :param text: text to search for
         """
         selector_with_text = '//*[text()="' + text + '"]'
         assert self.count_visible_elements(selector_with_text) > 0,\
-            f"Text {text} was not found on the current page"
+            f"{RED}Text {text} was not found on the current page{RESET}"
```

### Comparing `vigilant_kit-1.2.7/src/vigilant/actions/finder.py` & `vigilant_kit-1.2.8/src/vigilant/actions/finder.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/src/vigilant/actions/vigilant_actions.py` & `vigilant_kit-1.2.8/src/vigilant/actions/vigilant_actions.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/src/vigilant/actions/waiter.py` & `vigilant_kit-1.2.8/src/vigilant/actions/waiter.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/src/vigilant/driver/__init__.py` & `vigilant_kit-1.2.8/src/vigilant/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/src/vigilant/driver/vigilant_driver.py` & `vigilant_kit-1.2.8/src/vigilant/driver/vigilant_driver.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/.gitignore` & `vigilant_kit-1.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/LICENSE` & `vigilant_kit-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/README.md` & `vigilant_kit-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.7/pyproject.toml` & `vigilant_kit-1.2.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vigilant_kit"
-version = "1.2.7"
+version = "1.2.8"
 authors = [
   { name="Pelykh Ivan", email="ivan.pelykh@protonmail.com" },
 ]
 description = "Library that makes functional testing with Selenium WebDriver fast and easy. "
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
-  "selenium",
-  "python-dotenv",
-  "click",
-  "requests"
+    "selenium",
+    "python-dotenv",
+    "click",
+    "requests",
+    "psutil"
 ]
 
 keywords = ["testing", "selenium", "webdriver", "pytest", "unittest", "bdd", "tdd", "functional", "functional-testing"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/vigilant", "src/vgl_cli"]
```

### Comparing `vigilant_kit-1.2.7/PKG-INFO` & `vigilant_kit-1.2.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: vigilant_kit
-Version: 1.2.7
+Version: 1.2.8
 Summary: Library that makes functional testing with Selenium WebDriver fast and easy. 
 Project-URL: Homepage, https://github.com/ivpel/vigilant
 Project-URL: Bug Tracker, https://github.com/ivpel/vigilant/issues
 Author-email: Pelykh Ivan <ivan.pelykh@protonmail.com>
 License-File: LICENSE
 Keywords: bdd,functional,functional-testing,pytest,selenium,tdd,testing,unittest,webdriver
 Requires-Python: >=3.7
 Requires-Dist: click
+Requires-Dist: psutil
 Requires-Dist: python-dotenv
 Requires-Dist: requests
 Requires-Dist: selenium
 Description-Content-Type: text/markdown
 
 # Vigilant Kit
 Vigilant is a set of tools designed to help write and run robust functional tests using Selenium WebDriver. With
```

