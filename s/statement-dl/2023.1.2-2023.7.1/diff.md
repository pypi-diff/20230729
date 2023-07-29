# Comparing `tmp/statement-dl-2023.1.2.tar.gz` & `tmp/statement-dl-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statement-dl-2023.1.2.tar", last modified: Sat Jan 21 23:22:54 2023, max compression
+gzip compressed data, was "statement-dl-2023.7.1.tar", last modified: Sat Jul 29 21:25:45 2023, max compression
```

## Comparing `statement-dl-2023.1.2.tar` & `statement-dl-2023.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-01-21 23:22:54.306594 statement-dl-2023.1.2/
--rw-rw-rw-   0        0        0     1074 2021-11-08 18:06:52.000000 statement-dl-2023.1.2/LICENSE
--rw-rw-rw-   0        0        0     4415 2023-01-21 23:22:54.306594 statement-dl-2023.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3706 2022-01-31 15:36:23.000000 statement-dl-2023.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-01-21 23:22:54.307595 statement-dl-2023.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1131 2023-01-21 23:22:08.000000 statement-dl-2023.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-21 23:22:54.271594 statement-dl-2023.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-01-21 23:22:54.277594 statement-dl-2023.1.2/src/statement_dl/
--rw-rw-rw-   0        0        0     3262 2023-01-20 21:33:54.000000 statement-dl-2023.1.2/src/statement_dl/__init__.py
--rw-rw-rw-   0        0        0       69 2021-11-15 15:35:08.000000 statement-dl-2023.1.2/src/statement_dl/__main__.py
--rw-rw-rw-   0        0        0    12349 2023-01-21 23:21:17.000000 statement-dl-2023.1.2/src/statement_dl/flatex.py
--rw-rw-rw-   0        0        0     1096 2022-01-31 15:36:23.000000 statement-dl-2023.1.2/src/statement_dl/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-21 23:22:54.305594 statement-dl-2023.1.2/src/statement_dl.egg-info/
--rw-rw-rw-   0        0        0     4415 2023-01-21 23:22:54.000000 statement-dl-2023.1.2/src/statement_dl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      418 2023-01-21 23:22:54.000000 statement-dl-2023.1.2/src/statement_dl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-21 23:22:54.000000 statement-dl-2023.1.2/src/statement_dl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-01-21 23:22:54.000000 statement-dl-2023.1.2/src/statement_dl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2021-11-08 18:59:55.000000 statement-dl-2023.1.2/src/statement_dl.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2023-01-21 23:22:54.000000 statement-dl-2023.1.2/src/statement_dl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-01-21 23:22:54.000000 statement-dl-2023.1.2/src/statement_dl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 21:25:45.651703 statement-dl-2023.7.1/
+-rw-rw-rw-   0        0        0     1095 2023-07-29 11:03:53.000000 statement-dl-2023.7.1/LICENSE
+-rw-rw-rw-   0        0        0     4365 2023-07-29 21:25:45.651703 statement-dl-2023.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3706 2023-07-29 11:03:53.000000 statement-dl-2023.7.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-29 21:25:45.651703 statement-dl-2023.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1071 2023-07-29 21:24:49.000000 statement-dl-2023.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:25:45.646201 statement-dl-2023.7.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 21:25:45.648201 statement-dl-2023.7.1/src/statement_dl/
+-rw-rw-rw-   0        0        0     3262 2023-07-29 11:03:53.000000 statement-dl-2023.7.1/src/statement_dl/__init__.py
+-rw-rw-rw-   0        0        0       73 2023-07-29 11:03:53.000000 statement-dl-2023.7.1/src/statement_dl/__main__.py
+-rw-rw-rw-   0        0        0    13111 2023-07-29 19:50:43.000000 statement-dl-2023.7.1/src/statement_dl/flatex.py
+-rw-rw-rw-   0        0        0     1142 2023-07-29 19:18:00.000000 statement-dl-2023.7.1/src/statement_dl/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 21:25:45.650201 statement-dl-2023.7.1/src/statement_dl.egg-info/
+-rw-rw-rw-   0        0        0     4365 2023-07-29 21:25:45.000000 statement-dl-2023.7.1/src/statement_dl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      418 2023-07-29 21:25:45.000000 statement-dl-2023.7.1/src/statement_dl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 21:25:45.000000 statement-dl-2023.7.1/src/statement_dl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-29 21:25:45.000000 statement-dl-2023.7.1/src/statement_dl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 11:04:19.000000 statement-dl-2023.7.1/src/statement_dl.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-07-29 21:25:45.000000 statement-dl-2023.7.1/src/statement_dl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-29 21:25:45.000000 statement-dl-2023.7.1/src/statement_dl.egg-info/top_level.txt
```

### Comparing `statement-dl-2023.1.2/LICENSE` & `statement-dl-2023.7.1/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 Peter Schmidbauer
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 Peter Schmidbauer
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `statement-dl-2023.1.2/PKG-INFO` & `statement-dl-2023.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: statement-dl
-Version: 2023.1.2
+Version: 2023.7.1
 Summary: Automatic download of banking/broker documents from flatex
 Home-page: https://github.com/pspeter/statement-dl
 Author: Peter Schmidbauer
 Author-email: peter.schmidb@gmail.com
 License: MIT
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # statement-dl
 
 ![PyPI](https://img.shields.io/pypi/v/statement-dl.svg)
 ![calver](https://img.shields.io/badge/calver-YYYY.0M.MICRO-22bfda.svg)
```

### Comparing `statement-dl-2023.1.2/README.md` & `statement-dl-2023.7.1/README.md`

 * *Files identical despite different names*

### Comparing `statement-dl-2023.1.2/setup.py` & `statement-dl-2023.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setup(
     name="statement-dl",
-    version="2023.01.2",
+    version="2023.07.1",
     description="Automatic download of banking/broker documents from flatex",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pspeter/statement-dl",
     author="Peter Schmidbauer",
     author_email="peter.schmidb@gmail.com",
     license="MIT",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
-    install_requires=["selenium>=3.141.0,<4.0.0"],
-    python_requires=">=3.6",
+    install_requires=["selenium==4.*"],
+    python_requires=">=3.8",
     zip_safe=False,
     entry_points={"console_scripts": ["statement_dl = statement_dl:main"]},
     classifiers=[
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `statement-dl-2023.1.2/src/statement_dl/__init__.py` & `statement-dl-2023.7.1/src/statement_dl/__init__.py`

 * *Files identical despite different names*

### Comparing `statement-dl-2023.1.2/src/statement_dl/flatex.py` & `statement-dl-2023.7.1/src/statement_dl/flatex.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,69 +103,69 @@
             sub_dirs,
             tld,
         )
     finally:
         try:
             _click(
                 driver,
-                driver.find_element_by_xpath('//div[contains(@class, "LogoutArea")]'),
+                driver.find_element(By.XPATH, '//div[contains(@class, "LogoutArea")]'),
             )
         finally:
             driver.close()
 
     print("Done!")
 
 
 def _accept_cookies(driver: webdriver.Firefox) -> None:
     time.sleep(1)
-    driver.find_element_by_xpath('//button[text()="Alle akzeptieren"]').click()
+    driver.find_element(By.XPATH, '//button[text()="Alle akzeptieren"]').click()
     time.sleep(3)
 
 
 def _login(
     driver: webdriver.Firefox, user: Optional[str], pw: Optional[str], de: bool, headless: bool) -> None:
     time.sleep(1)
     
     if de:
         formid_user, formid_pw, formid_btn = "txtUserId", "txtPassword_txtPassword", "btnLogin"
     else:
         formid_user, formid_pw, formid_btn = "userId", "pin", "loginButton"
     
-    user_input = driver.find_element_by_xpath(f'//input[@id="loginForm_{formid_user}"]')
-    pw_input = driver.find_element_by_xpath(f'//input[@id="loginForm_{formid_pw}"]')
+    user_input = driver.find_element(By.XPATH, f'//input[@id="loginForm_{formid_user}"]')
+    pw_input = driver.find_element(By.XPATH, f'//input[@id="loginForm_{formid_pw}"]')
 
     while not user and headless:
         user = input("Enter your flatex username: ")
 
     while not pw and headless:
         pw = getpass("Enter your flatex password: ")
 
     if user:
         user_input.send_keys(user)
 
     if pw:
         pw_input.send_keys(pw)
 
     if user and pw:
-        driver.find_element_by_xpath(f'//input[@id="loginForm_{formid_btn}"]').click()
+        driver.find_element(By.XPATH, f'//input[@id="loginForm_{formid_btn}"]').click()
     else:
-        driver.find_element_by_xpath(f'//input[@id="loginForm_{formid_user}"]').click()
+        driver.find_element(By.XPATH, f'//input[@id="loginForm_{formid_user}"]').click()
         print("Please login in the browser")
 
     login_timeout = 300
     WebDriverWait(driver, login_timeout).until(ec.title_is("Onlinebanking"))
     time.sleep(1)
 
 
 def _go_to_documents_tab(driver: webdriver.Firefox) -> None:
     mail_button = WebDriverWait(driver, 60).until(
         ec.presence_of_element_located((By.XPATH, '//td[@id="menu_mailMenu"]'))
     )
     mail_button.click()
-    driver.find_element_by_xpath('//*[text()="Dokumentenarchiv"]').click()
+    driver.find_element(By.XPATH, '//*[text()="Dokumentenarchiv"]').click()
     WebDriverWait(driver, 60).until(
         ec.presence_of_element_located(
             (By.XPATH, '//form[@id="documentArchiveListForm"]')
         )
     )
 
 
@@ -185,74 +185,90 @@
     print(f"Downloading files to {str(download_path)}")
 
     # the driver.get call that downloads the pdf does not return normally, so
     # we have to wait for it to time out. Default timeout is a couple minutes,
     # but 3 seconds should be enough to start the download
     driver.set_page_load_timeout(3)
 
-    rows = driver.find_elements_by_xpath(f'//table[@class="Data"]/tbody/tr')
-    num_files = len(rows)
-    max_loaded_files = 100
-
-    while num_files == max_loaded_files:
+    while _check_if_max_documents_displayed(driver):
         # only 100 files are displayed at most, so we need to do some manual
         # paging using the date filters
         print("More than 100 files, paging through results")
-        last_date_string = driver.find_element_by_xpath(
+        last_date_string = driver.find_element(By.XPATH, 
             f"//table[@class='Data']/tbody/tr[last()]/td[3]"
         ).text
         last_date = _parse_list_date(last_date_string)
         day_after_last_date = last_date + timedelta(days=1)
         _set_download_filter(driver, day_after_last_date, to_date, all_files)
         _download_current_pdfs(driver, download_path, dest, all_files, keep_filenames, sub_dirs, tld)
         # set filter to cover the range of files we haven't downloaded yet
-        _set_download_filter(driver, from_date, last_date, all_files)
-        rows = driver.find_elements_by_xpath(f'//table[@class="Data"]/tbody/tr')
-        num_files = len(rows)
+        to_date = last_date
+        _set_download_filter(driver, from_date, to_date, all_files)
 
     _download_current_pdfs(driver, download_path, dest, all_files, keep_filenames, sub_dirs, tld)
 
 
+def _check_if_max_documents_displayed(driver: webdriver.Firefox) -> bool:
+    max_documents_displayed_txt = 'Es werden nur die ersten 100 Dokumente dargestellt.'
+    max_documents_elems = driver.find_elements(By.XPATH, f'//div[text()="{max_documents_displayed_txt}"]')
+    are_max_documents_displayed = len(max_documents_elems) != 0
+    return are_max_documents_displayed
+
+
 def _set_download_filter(
     driver: webdriver.Firefox, from_date: date, to_date: date, all_files: bool
 ) -> None:
+    print(f"Setting download filter to {from_date} - {to_date}, {all_files=}")
     # select all or unread
-    _click(driver, driver.find_element_by_xpath('//div[contains(@id, "readState")]'))
+    _click(driver, driver.find_element(By.XPATH, '//div[contains(@id, "readState")]'))
     selected_option = "0" if all_files else "2"
     _click(
         driver,
-        driver.find_element_by_xpath(
+        driver.find_element(
+            By.XPATH,
             f'//div[@id="documentArchiveListForm_readState_item_{selected_option}"]'
         ),
     )
+    # activate individual date range
+    date_range_picker = driver.find_element(
+        By.ID, "documentArchiveListForm_dateRangeComponent_retrievalPeriodSelection"
+    )
+    _click(driver, date_range_picker)
+    individual_range_item = driver.find_element(
+        By.ID, "documentArchiveListForm_dateRangeComponent_retrievalPeriodSelection_item_6"
+    )
+    _click(driver, individual_range_item)
+
+    time.sleep(1)
     # expand date range
-    date_from_elem = driver.find_element_by_xpath(
+    date_from_elem = driver.find_element(
+        By.XPATH,
         '//input[contains(@id, "dateRangeComponent_startDate")]'
     )
-    date_to_elem = driver.find_element_by_xpath(
+    date_to_elem = driver.find_element(
+        By.XPATH,
         '//input[contains(@id, "dateRangeComponent_endDate")]'
     )
-    time.sleep(1)
     _enter_date(driver, date_from_elem, from_date)
     time.sleep(1)
     _enter_date(driver, date_to_elem, to_date)
 
     try:
-        wait_elem = driver.find_element_by_xpath(
+        wait_elem = driver.find_element(By.XPATH, 
             "//table[@class='Data']/tbody/tr[last()]"
         )
     except NoSuchElementException:
-        wait_elem = driver.find_element_by_xpath(
+        wait_elem = driver.find_element(By.XPATH, 
             "//div[text()='Keine Dokumente vorhanden.']"
         )
 
     # hit search
     _click(
         driver,
-        driver.find_element_by_xpath('//input[contains(@id, "applyFilterButton")]'),
+        driver.find_element(By.XPATH, '//input[contains(@id, "applyFilterButton")]'),
     )
     try:
         timeout = 5
         WebDriverWait(driver, timeout).until(ec.staleness_of(wait_elem))
     except TimeoutException:
         pass  # filter hasn't changed elements
 
@@ -266,47 +282,50 @@
     date_elem.send_keys(desired_date.strftime("%d.%m.%Y"))
     date_elem.send_keys(Keys.ENTER)
     time.sleep(0.1)
 
 
 def _download_current_pdfs(driver, download_path, dest, all_files, keep_filenames, sub_dirs: bool, tld):
     driver.execute_script(onfinished)
-    num_files = len(driver.find_elements_by_xpath(f'//table[@class="Data"]/tbody/tr'))
+    num_files = len(driver.find_elements(By.XPATH, f'//table[@class="Data"]/tbody/tr'))
 
     for file_idx in range(num_files):
         driver.execute_script("window.pdf_download_url = ''")
         url = ""
         # when we read a previously unread file, it disappears from the list, so
         # have to keep reading the first file
         download_idx = file_idx + 1 if all_files else 1
         
-        dmy_date_string = driver.find_element_by_xpath(
+        dmy_date_string = driver.find_element(
+            By.XPATH,
             f"//table[@class='Data']/tbody/tr[{download_idx}]/td[3]"
         ).text
 
-        doc_type = driver.find_element_by_xpath(
+        doc_type = driver.find_element(
+            By.XPATH,
             f"//table[@class='Data']/tbody/tr[{download_idx}]/td[4]"
         ).text
 
-        raw_doc_title = driver.find_element_by_xpath(
+        raw_doc_title = driver.find_element(
+            By.XPATH,
             f"//table[@class='Data']/tbody/tr[{download_idx}]/td[5]"
         ).text
 
         file_date = _parse_list_date(dmy_date_string)
         ymd_date_string = file_date.strftime("%Y-%m-%d")
 
         print()
         print("Date:", dmy_date_string)
         print("Type:", doc_type)
         print("Name:", raw_doc_title)
 
-        row = driver.find_element_by_xpath(
+        row = driver.find_element(By.XPATH, 
             f'//table[@class="Data"]/tbody/tr[{download_idx}]'
         )
-        driver.execute_script(onclick.format(file_idx), row)
+        driver.execute_script(onclick.format(download_idx - 1), row)
 
         time.sleep(0.3)
         while not url or url == "none":
             time.sleep(0.1)
             url = driver.execute_script("return window.pdf_download_url")
 
         if sub_dirs:
@@ -360,15 +379,15 @@
         else f"{date_string}_{file_name}.pdf"
     )
 
     return file_name
 
 
 def _click(driver: webdriver.Firefox, elem: WebElement) -> None:
-    retry = driver.find_elements_by_xpath(
+    retry = driver.find_elements(By.XPATH, 
         "//input[@id='previousActionNotFinishedOverlayForm_retryButton']"
     )
     if retry:
         retry[0].click()
 
     elem.click()
```

### Comparing `statement-dl-2023.1.2/src/statement_dl/utils.py` & `statement-dl-2023.7.1/src/statement_dl/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from datetime import date, datetime
 from typing import Optional
 
 from selenium import webdriver
-from selenium.webdriver.firefox.options import Options
+from selenium.webdriver.firefox.service import Service
 
 
 def parse_date(date_string: str) -> date:
     if date_string == "today":
         return date.today()
     return datetime.strptime(date_string, "%Y-%m-%d").date()
 
 
 def get_driver(
     geckodriver: Optional[str], download_dir: str, headless: bool
 ) -> webdriver.Firefox:
-    fp = webdriver.FirefoxProfile()
-    fp.set_preference("browser.download.folderList", 2)
-    fp.set_preference("browser.helperApps.alwaysAsk.force", False)
-    fp.set_preference("browser.download.dir", download_dir)
-    fp.set_preference("pdfjs.disabled", True)
-    fp.set_preference("browser.helperApps.neverAsk.saveToDisk", "application/pdf")
-    fp.set_preference("browser.download.manager.showWhenStarting", False)
-
-    options = Options()
+    options = webdriver.FirefoxOptions()
     options.headless = headless
+    options.set_preference("browser.download.folderList", 2)
+    options.set_preference("browser.helperApps.alwaysAsk.force", False)
+    options.set_preference("browser.download.dir", download_dir)
+    options.set_preference("pdfjs.disabled", True)
+    options.set_preference("browser.helperApps.neverAsk.saveToDisk", "application/pdf")
+    options.set_preference("browser.download.manager.showWhenStarting", False)
 
     geckodriver = geckodriver if geckodriver else "geckodriver"
-    driver = webdriver.Firefox(fp, options=options, executable_path=geckodriver)
+    service = Service(executable_path=geckodriver)
+
+    driver = webdriver.Firefox(options=options, service=service)
     return driver
```

### Comparing `statement-dl-2023.1.2/src/statement_dl.egg-info/PKG-INFO` & `statement-dl-2023.7.1/src/statement_dl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: statement-dl
-Version: 2023.1.2
+Version: 2023.7.1
 Summary: Automatic download of banking/broker documents from flatex
 Home-page: https://github.com/pspeter/statement-dl
 Author: Peter Schmidbauer
 Author-email: peter.schmidb@gmail.com
 License: MIT
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # statement-dl
 
 ![PyPI](https://img.shields.io/pypi/v/statement-dl.svg)
 ![calver](https://img.shields.io/badge/calver-YYYY.0M.MICRO-22bfda.svg)
```

