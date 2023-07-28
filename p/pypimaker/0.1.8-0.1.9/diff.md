# Comparing `tmp/pypimaker-0.1.8.tar.gz` & `tmp/pypimaker-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypimaker-0.1.8.tar", last modified: Sat Jan  7 04:53:38 2023, max compression
+gzip compressed data, was "dist/pypimaker-0.1.9.tar", last modified: Sat Jan  7 16:54:09 2023, max compression
```

## Comparing `pypimaker-0.1.8.tar` & `pypimaker-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-01-07 04:53:38.902522 pypimaker-0.1.8/
--rw-r--r--   0 holly      (501) staff       (20)     1067 2023-01-06 23:58:32.000000 pypimaker-0.1.8/LICENSE
--rw-r--r--   0 holly      (501) staff       (20)     4357 2023-01-07 04:53:38.902216 pypimaker-0.1.8/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)     3592 2023-01-07 04:52:50.000000 pypimaker-0.1.8/README.md
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-01-07 04:53:38.899933 pypimaker-0.1.8/pypimaker.egg-info/
--rw-r--r--   0 holly      (501) staff       (20)     4357 2023-01-07 04:53:38.000000 pypimaker-0.1.8/pypimaker.egg-info/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)      427 2023-01-07 04:53:38.000000 pypimaker-0.1.8/pypimaker.egg-info/SOURCES.txt
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-01-07 04:53:38.000000 pypimaker-0.1.8/pypimaker.egg-info/dependency_links.txt
--rw-r--r--   0 holly      (501) staff       (20)       48 2023-01-07 04:53:38.000000 pypimaker-0.1.8/pypimaker.egg-info/entry_points.txt
--rw-r--r--   0 holly      (501) staff       (20)       10 2023-01-07 04:53:38.000000 pypimaker-0.1.8/pypimaker.egg-info/top_level.txt
--rw-r--r--   0 holly      (501) staff       (20)       38 2023-01-07 04:53:38.902596 pypimaker-0.1.8/setup.cfg
--rw-r--r--   0 holly      (501) staff       (20)     1192 2023-01-07 04:53:38.000000 pypimaker-0.1.8/setup.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-01-07 04:53:38.900829 pypimaker-0.1.8/src/
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-01-06 23:58:32.000000 pypimaker-0.1.8/src/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     1735 2023-01-07 04:47:12.000000 pypimaker-0.1.8/src/__main__.py
--rw-r--r--   0 holly      (501) staff       (20)    12660 2023-01-07 04:13:56.000000 pypimaker-0.1.8/src/files.py
--rw-r--r--   0 holly      (501) staff       (20)      889 2023-01-06 23:58:32.000000 pypimaker-0.1.8/src/reset.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-01-07 04:53:38.901611 pypimaker-0.1.8/src/ui/
--rw-r--r--   0 holly      (501) staff       (20)     6796 2023-01-06 23:58:32.000000 pypimaker-0.1.8/src/ui/AuthorInfoSelector.py
--rw-r--r--   0 holly      (501) staff       (20)     3257 2023-01-07 04:13:54.000000 pypimaker-0.1.8/src/ui/DialogWindow.py
--rw-r--r--   0 holly      (501) staff       (20)     6283 2023-01-07 03:53:23.000000 pypimaker-0.1.8/src/ui/OptionSelector.py
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-01-06 23:58:32.000000 pypimaker-0.1.8/src/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)      563 2023-01-06 23:58:32.000000 pypimaker-0.1.8/src/ui/navigation.py
--rw-r--r--   0 holly      (501) staff       (20)     7116 2023-01-06 23:58:32.000000 pypimaker-0.1.8/src/upload.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-01-07 04:53:38.901944 pypimaker-0.1.8/tests/
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-01-06 23:58:32.000000 pypimaker-0.1.8/tests/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     2373 2023-01-06 23:58:32.000000 pypimaker-0.1.8/tests/test_exampleTest.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-01-07 16:54:09.489925 pypimaker-0.1.9/
+-rw-r--r--   0 holly      (501) staff       (20)     1067 2023-01-06 23:58:32.000000 pypimaker-0.1.9/LICENSE
+-rw-r--r--   0 holly      (501) staff       (20)     4358 2023-01-07 16:54:09.489651 pypimaker-0.1.9/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)     3593 2023-01-07 16:50:53.000000 pypimaker-0.1.9/README.md
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-01-07 16:54:09.486851 pypimaker-0.1.9/pypimaker.egg-info/
+-rw-r--r--   0 holly      (501) staff       (20)     4358 2023-01-07 16:54:09.000000 pypimaker-0.1.9/pypimaker.egg-info/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)      442 2023-01-07 16:54:09.000000 pypimaker-0.1.9/pypimaker.egg-info/SOURCES.txt
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-01-07 16:54:09.000000 pypimaker-0.1.9/pypimaker.egg-info/dependency_links.txt
+-rw-r--r--   0 holly      (501) staff       (20)       48 2023-01-07 16:54:09.000000 pypimaker-0.1.9/pypimaker.egg-info/entry_points.txt
+-rw-r--r--   0 holly      (501) staff       (20)       10 2023-01-07 16:54:09.000000 pypimaker-0.1.9/pypimaker.egg-info/top_level.txt
+-rw-r--r--   0 holly      (501) staff       (20)       38 2023-01-07 16:54:09.490007 pypimaker-0.1.9/setup.cfg
+-rw-r--r--   0 holly      (501) staff       (20)     1192 2023-01-07 16:54:09.000000 pypimaker-0.1.9/setup.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-01-07 16:54:09.487546 pypimaker-0.1.9/src/
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-01-06 23:58:32.000000 pypimaker-0.1.9/src/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     1735 2023-01-07 04:47:12.000000 pypimaker-0.1.9/src/__main__.py
+-rw-r--r--   0 holly      (501) staff       (20)    12876 2023-01-07 16:50:51.000000 pypimaker-0.1.9/src/files.py
+-rw-r--r--   0 holly      (501) staff       (20)      889 2023-01-06 23:58:32.000000 pypimaker-0.1.9/src/reset.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-01-07 16:54:09.488470 pypimaker-0.1.9/src/ui/
+-rw-r--r--   0 holly      (501) staff       (20)     6796 2023-01-06 23:58:32.000000 pypimaker-0.1.9/src/ui/AuthorInfoSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)     3257 2023-01-07 04:13:54.000000 pypimaker-0.1.9/src/ui/DialogWindow.py
+-rw-r--r--   0 holly      (501) staff       (20)     6588 2023-01-07 16:50:57.000000 pypimaker-0.1.9/src/ui/OptionSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-01-06 23:58:32.000000 pypimaker-0.1.9/src/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)      563 2023-01-06 23:58:32.000000 pypimaker-0.1.9/src/ui/navigation.py
+-rw-r--r--   0 holly      (501) staff       (20)     7116 2023-01-07 05:53:05.000000 pypimaker-0.1.9/src/upload.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-01-07 16:54:09.489210 pypimaker-0.1.9/tests/
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-01-06 23:58:32.000000 pypimaker-0.1.9/tests/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     2612 2023-01-07 05:44:13.000000 pypimaker-0.1.9/tests/test_files.py
+-rw-r--r--   0 holly      (501) staff       (20)     1420 2023-01-07 05:53:07.000000 pypimaker-0.1.9/tests/test_upload.py
```

### Comparing `pypimaker-0.1.8/LICENSE` & `pypimaker-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypimaker-0.1.8/PKG-INFO` & `pypimaker-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypimaker
-Version: 0.1.8
+Version: 0.1.9
 Summary: Software designed for simplifying PyPI Python package setups
 Home-page: https://github.com/bdavis222/pypimaker
 Author: Brian Davis
 Project-URL: Bug Reports, https://github.com/bdavis222/pypimaker/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/
 Classifier: Intended Audience :: Developers
@@ -83,15 +83,15 @@
 
 ## Authors
 
 Brian Davis
 
 ## Release History
 
-* 0.1.8
+* 0.1.9
 	 * Bug fixes
 * 0.1.0
 	 * Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/pypimaker/blob/main/LICENSE) file for details.
@@ -102,12 +102,12 @@
 
 Tests for PyPI Maker use [Python's built-in unittest framework](https://docs.python.org/3/library/unittest.html), and are stored in the `tests` folder. To run tests, navigate to the top level of PyPI Maker's folder structure and run the following command:
 
 ```
 python -m unittest
 ```
 
-The same test framework can optionally be added to your own project: If there is not yet a folder named `tests` in the top level of your project's directory structure, then a dialog window will pop up asking if you would like to include template unit tests in your project when running `pypimaker generate`. Confirming this selection will create a `test` folder with individual unit tests inside, corresponding to each of the Python files in your project. Of course, until writing test cases within each of these test files, they won't actually test anything.
+The same test framework can optionally be added to your own project: If there is not yet a folder named `tests` in the top level of your project's directory structure, then a dialog window will pop up asking if you would like to include template unit tests in your project when running `pypimaker generate`. Confirming this selection will create a `tests` folder with individual unit tests inside, corresponding to each of the Python files in your project. Of course, until writing test cases within each of these test files, they won't actually test anything.
 
 ### Bug Reports and Feature Requests
 
 To report a bug, visit the [issues page](https://github.com/bdavis222/project_template/issues). New feature requests are also welcome!
```

### Comparing `pypimaker-0.1.8/README.md` & `pypimaker-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 ## Authors
 
 Brian Davis
 
 ## Release History
 
-* 0.1.8
+* 0.1.9
 	 * Bug fixes
 * 0.1.0
 	 * Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/pypimaker/blob/main/LICENSE) file for details.
@@ -83,12 +83,12 @@
 
 Tests for PyPI Maker use [Python's built-in unittest framework](https://docs.python.org/3/library/unittest.html), and are stored in the `tests` folder. To run tests, navigate to the top level of PyPI Maker's folder structure and run the following command:
 
 ```
 python -m unittest
 ```
 
-The same test framework can optionally be added to your own project: If there is not yet a folder named `tests` in the top level of your project's directory structure, then a dialog window will pop up asking if you would like to include template unit tests in your project when running `pypimaker generate`. Confirming this selection will create a `test` folder with individual unit tests inside, corresponding to each of the Python files in your project. Of course, until writing test cases within each of these test files, they won't actually test anything.
+The same test framework can optionally be added to your own project: If there is not yet a folder named `tests` in the top level of your project's directory structure, then a dialog window will pop up asking if you would like to include template unit tests in your project when running `pypimaker generate`. Confirming this selection will create a `tests` folder with individual unit tests inside, corresponding to each of the Python files in your project. Of course, until writing test cases within each of these test files, they won't actually test anything.
 
 ### Bug Reports and Feature Requests
 
 To report a bug, visit the [issues page](https://github.com/bdavis222/project_template/issues). New feature requests are also welcome!
```

### Comparing `pypimaker-0.1.8/pypimaker.egg-info/PKG-INFO` & `pypimaker-0.1.9/pypimaker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypimaker
-Version: 0.1.8
+Version: 0.1.9
 Summary: Software designed for simplifying PyPI Python package setups
 Home-page: https://github.com/bdavis222/pypimaker
 Author: Brian Davis
 Project-URL: Bug Reports, https://github.com/bdavis222/pypimaker/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/
 Classifier: Intended Audience :: Developers
@@ -83,15 +83,15 @@
 
 ## Authors
 
 Brian Davis
 
 ## Release History
 
-* 0.1.8
+* 0.1.9
 	 * Bug fixes
 * 0.1.0
 	 * Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/pypimaker/blob/main/LICENSE) file for details.
@@ -102,12 +102,12 @@
 
 Tests for PyPI Maker use [Python's built-in unittest framework](https://docs.python.org/3/library/unittest.html), and are stored in the `tests` folder. To run tests, navigate to the top level of PyPI Maker's folder structure and run the following command:
 
 ```
 python -m unittest
 ```
 
-The same test framework can optionally be added to your own project: If there is not yet a folder named `tests` in the top level of your project's directory structure, then a dialog window will pop up asking if you would like to include template unit tests in your project when running `pypimaker generate`. Confirming this selection will create a `test` folder with individual unit tests inside, corresponding to each of the Python files in your project. Of course, until writing test cases within each of these test files, they won't actually test anything.
+The same test framework can optionally be added to your own project: If there is not yet a folder named `tests` in the top level of your project's directory structure, then a dialog window will pop up asking if you would like to include template unit tests in your project when running `pypimaker generate`. Confirming this selection will create a `tests` folder with individual unit tests inside, corresponding to each of the Python files in your project. Of course, until writing test cases within each of these test files, they won't actually test anything.
 
 ### Bug Reports and Feature Requests
 
 To report a bug, visit the [issues page](https://github.com/bdavis222/project_template/issues). New feature requests are also welcome!
```

### Comparing `pypimaker-0.1.8/setup.py` & `pypimaker-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
 	name='pypimaker', # Required
-    version='0.1.8', # Required 
+    version='0.1.9', # Required 
     description='Software designed for simplifying PyPI Python package setups',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
     url='https://github.com/bdavis222/pypimaker',
     author='Brian Davis',
 	classifiers=[ # Defined at https://pypi.org/classifiers/
 		'Intended Audience :: Developers',
```

### Comparing `pypimaker-0.1.8/src/__main__.py` & `pypimaker-0.1.9/src/__main__.py`

 * *Files identical despite different names*

### Comparing `pypimaker-0.1.8/src/files.py` & `pypimaker-0.1.9/src/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,18 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE \
 SOFTWARE.'
 	
 	with open(filepath + "/LICENSE", "w") as file:
 		file.write(output)
 
 def getAuthorNamesInline(authorsArray):
-	if len(authorsArray) == 1:
+	if not len(authorsArray):
+		return ""
+	
+	elif len(authorsArray) == 1:
 		return authorsArray[0]
 	
 	elif len(authorsArray) == 2:
 		return f"{authorsArray[0]} and {authorsArray[1]}"
 	
 	else:
 		allButLast = authorsArray[:-1]
@@ -168,14 +171,17 @@
 To report a bug, visit the [issues page](https://github.com/{githubUsername}/{projectName}/issues). \
 New feature requests are also welcome!"
 	
 	output = f"\
 # {projectName}\n\
 {blurbLine}\
 \n\
+This Python package was created and uploaded to PyPI using [PyPI Maker](https://github.com/bdavis222/pypimaker). \
+This is a template README generated by PyPI Maker.\n\
+\n\
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](PAYPAL_DONATE_LINK_GOES_HERE)\n\
 \n\
 OPTIONAL: ENTER A 2-3 SENTENCE DESCRIPTION ABOUT THE SOFTWARE HERE\n\
 \n\
 ## Getting Started\n\
 \n\
 ### Dependencies\n\
```

### Comparing `pypimaker-0.1.8/src/reset.py` & `pypimaker-0.1.9/src/reset.py`

 * *Files identical despite different names*

### Comparing `pypimaker-0.1.8/src/ui/AuthorInfoSelector.py` & `pypimaker-0.1.9/src/ui/AuthorInfoSelector.py`

 * *Files identical despite different names*

### Comparing `pypimaker-0.1.8/src/ui/DialogWindow.py` & `pypimaker-0.1.9/src/ui/DialogWindow.py`

 * *Files identical despite different names*

### Comparing `pypimaker-0.1.8/src/ui/OptionSelector.py` & `pypimaker-0.1.9/src/ui/OptionSelector.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 MISMATCHED_SELECTION_TEXT = "Mismatched folder name and project name.\nAre you sure you selected correctly?"
 NO_PYTHON_FILES_IN_PROJECT_FOLDER_TEXT = "No Python files found in folder.\nSelect a different folder."
 PROJECT_DESCRIPTION_TEXT = 'One-sentence Project Description (e.g., "Software designed for..."):'
 PROJECT_FOLDER_NOT_CHOSEN_TEXT = "You must select your project \nusing the Browse button."
 PROJECT_NAME_NOT_CHOSEN_TEXT = "Project Name is a required field.\nUse folder name as project name?"
 SELECT_FOLDER_TEXT = "Select the top-level folder containing your Python project"
+PROJECT_NAME_DESCRIPTION_TEXT = '(Your package will be installed with the "pip install \
+project_name" command using the project name given above.)'
 
 class OptionSelector:
 	def __init__(self):
 		self.window = tk.Tk()
 		self.window.title("PyPI Maker")
 		centerX = (self.window.winfo_screenwidth() - 650) // 2
 		centerY = (self.window.winfo_screenheight() - 250) // 2
@@ -67,14 +69,16 @@
 		
 		frameProjectName = tk.Frame(self.window)
 		labelProjectName = tk.Label(self.window, text="Project Name:")
 		self.entryProjectName = tk.Entry(self.window, width=25)
 		labelProjectName.pack(in_=frameProjectName, side=tk.LEFT)
 		self.entryProjectName.pack(in_=frameProjectName, side=tk.LEFT)
 		
+		labelProjectNameDescription = tk.Label(self.window, text=PROJECT_NAME_DESCRIPTION_TEXT, font=("Helvetica 9", 10))
+		
 		frameGithubUsername = tk.Frame(self.window)
 		labelGithubUsername = tk.Label(self.window, text="Project GitHub Username:")
 		self.entryGithubUsername = tk.Entry(self.window, width=25)
 		labelGithubUsername.pack(in_=frameGithubUsername, side=tk.LEFT)
 		self.entryGithubUsername.pack(in_=frameGithubUsername, side=tk.LEFT)
 		
 		labelProjectDescription = tk.Label(self.window, text=PROJECT_DESCRIPTION_TEXT)
@@ -85,14 +89,15 @@
 			variable=self.includeAuthorNames, onvalue=True, offvalue=False)
 				
 		buttonDone = tk.Button(self.window, text="Done", command=self.checkDone, fg="blue")
 				
 		filepathFrame.pack()
 		navigation.pack()
 		frameProjectName.pack()
+		labelProjectNameDescription.pack()
 		frameGithubUsername.pack()
 		labelProjectDescription.pack()
 		self.entryProjectDescription.pack()
 		checkboxIncludeAuthorNames.pack()
 		buttonDone.pack()
 		
 		self.window.protocol("WM_DELETE_WINDOW", quit)
```

### Comparing `pypimaker-0.1.8/src/ui/navigation.py` & `pypimaker-0.1.9/src/ui/navigation.py`

 * *Files identical despite different names*

### Comparing `pypimaker-0.1.8/src/upload.py` & `pypimaker-0.1.9/src/upload.py`

 * *Files identical despite different names*

