# Comparing `tmp/pymultinest-2.7.tar.gz` & `tmp/pymultinest-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymultinest-2.7.tar", last modified: Tue Nov 20 13:53:18 2018, max compression
+gzip compressed data, was "dist/pymultinest-2.9.tar", last modified: Tue Feb  4 14:50:04 2020, max compression
```

## Comparing `pymultinest-2.7.tar` & `pymultinest-2.9.tar`

### file list

```diff
@@ -1,57 +1,22 @@
-drwxr-xr-x   0 user      (1000) users      (100)        0 2018-11-20 13:53:18.000000 pymultinest-2.7/
-drwxr-xr-x   0 user      (1000) users      (100)        0 2018-11-20 13:53:18.000000 pymultinest-2.7/doc/
--rw-r--r--   0 user      (1000) users      (100)     1954 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/pymultinest.rst
--rw-r--r--   0 user      (1000) users      (100)     1842 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/pycuba.rst
--rw-r--r--   0 user      (1000) users      (100)     1907 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/index.rst
--rw-r--r--   0 user      (1000) users      (100)     4610 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/Makefile
--rw-r--r--   0 user      (1000) users      (100)      113 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/pymultinest_analyse.rst
--rw-r--r--   0 user      (1000) users      (100)      159 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/pymultinest_watch.rst
--rw-r--r--   0 user      (1000) users      (100)     7192 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/conf.py
--rw-r--r--   0 user      (1000) users      (100)     5667 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/install.rst
-drwxr-xr-x   0 user      (1000) users      (100)        0 2018-11-20 13:53:18.000000 pymultinest-2.7/doc/_static/
--rw-r--r--   0 user      (1000) users      (100)    15068 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/_static/marginals.png
--rw-r--r--   0 user      (1000) users      (100)    27556 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/_static/data.pdf
--rw-r--r--   0 user      (1000) users      (100)      210 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/_static/Makefile
--rw-r--r--   0 user      (1000) users      (100)    21617 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/_static/marginals.pdf
--rw-r--r--   0 user      (1000) users      (100)   133614 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/_static/chain0.png
--rw-r--r--   0 user      (1000) users      (100)    55081 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/_static/data.png
--rw-r--r--   0 user      (1000) users      (100)   581208 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/_static/chain0.pdf
--rw-r--r--   0 user      (1000) users      (100)      163 2018-11-20 13:52:48.000000 pymultinest-2.7/doc/pymultinest_run.rst
--rw-r--r--   0 user      (1000) users      (100)      102 2018-11-20 13:52:47.000000 pymultinest-2.7/.gitignore
--rw-r--r--   0 user      (1000) users      (100)     4657 2018-11-20 13:52:48.000000 pymultinest-2.7/multinest_marginals.py
-drwxr-xr-x   0 user      (1000) users      (100)        0 2018-11-20 13:53:18.000000 pymultinest-2.7/pymultinest/
--rw-r--r--   0 user      (1000) users      (100)     7207 2018-11-20 13:52:48.000000 pymultinest-2.7/pymultinest/analyse.py
--rw-r--r--   0 user      (1000) users      (100)     1088 2018-11-20 13:52:48.000000 pymultinest-2.7/pymultinest/__init__.py
--rw-r--r--   0 user      (1000) users      (100)     3087 2018-11-20 13:52:48.000000 pymultinest-2.7/pymultinest/solve.py
--rw-r--r--   0 user      (1000) users      (100)    10260 2018-11-20 13:52:48.000000 pymultinest-2.7/pymultinest/run.py
--rw-r--r--   0 user      (1000) users      (100)    10144 2018-11-20 13:52:48.000000 pymultinest-2.7/pymultinest/plot.py
--rw-r--r--   0 user      (1000) users      (100)     2761 2018-11-20 13:52:48.000000 pymultinest-2.7/pymultinest/watch.py
-drwxr-xr-x   0 user      (1000) users      (100)        0 2018-11-20 13:53:18.000000 pymultinest-2.7/pycuba/
--rw-r--r--   0 user      (1000) users      (100)    16056 2018-11-20 13:52:48.000000 pymultinest-2.7/pycuba/__init__.py
--rw-r--r--   0 user      (1000) users      (100)      271 2018-11-20 13:52:47.000000 pymultinest-2.7/.coveragerc
--rw-r--r--   0 user      (1000) users      (100)      964 2018-11-20 13:52:48.000000 pymultinest-2.7/pymultinest_demo_minimal.py
--rw-r--r--   0 user      (1000) users      (100)     3036 2018-11-20 13:52:48.000000 pymultinest-2.7/README.rst
--rw-r--r--   0 user      (1000) users      (100)     1752 2018-11-20 13:52:48.000000 pymultinest-2.7/pycuba_demo.py
-drwxr-xr-x   0 user      (1000) users      (100)        0 2018-11-20 13:53:18.000000 pymultinest-2.7/pymultinest.egg-info/
--rw-r--r--   0 user      (1000) users      (100)     4090 2018-11-20 13:53:17.000000 pymultinest-2.7/pymultinest.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) users      (100)        1 2018-11-20 13:53:17.000000 pymultinest-2.7/pymultinest.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) users      (100)     1007 2018-11-20 13:53:17.000000 pymultinest-2.7/pymultinest.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) users      (100)       19 2018-11-20 13:53:17.000000 pymultinest-2.7/pymultinest.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) users      (100)       51 2013-07-03 20:45:24.000000 pymultinest-2.7/MANIFEST.in
--rw-r--r--   0 user      (1000) users      (100)     1844 2018-11-20 13:52:48.000000 pymultinest-2.7/model_compare.py
--rw-r--r--   0 user      (1000) users      (100)       23 2018-11-20 13:52:48.000000 pymultinest-2.7/conda-requirements.txt
--rw-r--r--   0 user      (1000) users      (100)       92 2018-11-20 13:53:18.000000 pymultinest-2.7/setup.cfg
--rw-r--r--   0 user      (1000) users      (100)     4090 2018-11-20 13:53:18.000000 pymultinest-2.7/PKG-INFO
--rw-r--r--   0 user      (1000) users      (100)      928 2018-11-20 13:52:48.000000 pymultinest-2.7/setup.py
--rw-r--r--   0 user      (1000) users      (100)     3881 2018-11-20 13:52:48.000000 pymultinest-2.7/pymultinest_demo_old.py
--rw-r--r--   0 user      (1000) users      (100)     3060 2018-11-20 13:52:47.000000 pymultinest-2.7/.travis.yml
--rw-r--r--   0 user      (1000) users      (100)    35147 2018-11-20 13:52:47.000000 pymultinest-2.7/COPYING
-drwxr-xr-x   0 user      (1000) users      (100)        0 2018-11-20 13:53:18.000000 pymultinest-2.7/tests/
--rw-r--r--   0 user      (1000) users      (100)     1295 2018-11-20 13:52:48.000000 pymultinest-2.7/tests/pymultinest_minimal_test.py
--rw-r--r--   0 user      (1000) users      (100)     1567 2018-11-20 13:52:48.000000 pymultinest-2.7/tests/pycuba_test.py
--rw-r--r--   0 user      (1000) users      (100)     1162 2018-11-20 13:52:48.000000 pymultinest-2.7/tests/pymultinest_test.py
--rw-r--r--   0 user      (1000) users      (100)      889 2018-11-20 13:52:48.000000 pymultinest-2.7/tests/pymultinest_solver_test.py
--rw-r--r--   0 user      (1000) users      (100)       89 2018-11-20 13:52:48.000000 pymultinest-2.7/INSTALL
--rw-r--r--   0 user      (1000) users      (100)     1131 2018-11-20 13:52:48.000000 pymultinest-2.7/pymultinest_demo.py
--rw-r--r--   0 user      (1000) users      (100)      547 2018-11-20 13:52:48.000000 pymultinest-2.7/pymultinest_solver_demo.py
--rw-r--r--   0 user      (1000) users      (100)     1177 2018-11-20 13:52:48.000000 pymultinest-2.7/LICENSE
+drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2020-02-04 14:50:04.000000 pymultinest-2.9/
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     5575 2020-02-04 14:50:04.000000 pymultinest-2.9/PKG-INFO
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     4218 2019-02-27 20:11:26.000000 pymultinest-2.9/README.rst
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     4657 2019-02-27 20:11:26.000000 pymultinest-2.9/multinest_marginals.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     1888 2019-05-07 13:39:15.000000 pymultinest-2.9/multinest_marginals_corner.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)    64130 2019-02-27 20:11:26.000000 pymultinest-2.9/multinest_marginals_fancy.py
+drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2020-02-04 14:50:04.000000 pymultinest-2.9/pycuba/
+-rw-r--r--   0 user      (1000) jbuchner  (1000)    16056 2019-02-27 20:11:26.000000 pymultinest-2.9/pycuba/__init__.py
+drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2020-02-04 14:50:04.000000 pymultinest-2.9/pymultinest/
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     1088 2019-02-27 20:11:26.000000 pymultinest-2.9/pymultinest/__init__.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     7203 2019-02-27 20:11:26.000000 pymultinest-2.9/pymultinest/analyse.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)    10144 2019-02-27 20:11:26.000000 pymultinest-2.9/pymultinest/plot.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)    10542 2019-10-29 17:03:48.000000 pymultinest-2.9/pymultinest/run.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     3136 2020-02-04 14:47:54.000000 pymultinest-2.9/pymultinest/solve.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     2761 2019-02-27 20:11:26.000000 pymultinest-2.9/pymultinest/watch.py
+drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2020-02-04 14:50:04.000000 pymultinest-2.9/pymultinest.egg-info/
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     5575 2020-02-04 14:50:04.000000 pymultinest-2.9/pymultinest.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) jbuchner  (1000)      398 2020-02-04 14:50:04.000000 pymultinest-2.9/pymultinest.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) jbuchner  (1000)        1 2020-02-04 14:50:04.000000 pymultinest-2.9/pymultinest.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) jbuchner  (1000)       19 2020-02-04 14:50:04.000000 pymultinest-2.9/pymultinest.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) jbuchner  (1000)       92 2020-02-04 14:50:04.000000 pymultinest-2.9/setup.cfg
+-rw-r--r--   0 user      (1000) jbuchner  (1000)      980 2020-02-04 14:49:46.000000 pymultinest-2.9/setup.py
```

### Comparing `pymultinest-2.7/multinest_marginals.py` & `pymultinest-2.9/multinest_marginals.py`

 * *Files identical despite different names*

### Comparing `pymultinest-2.7/pymultinest/analyse.py` & `pymultinest-2.9/pymultinest/analyse.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 		self.equal_weighted_file = "%spost_equal_weights.dat" % self.outputfiles_basename
 	
 	def get_data(self):
 		"""
 			fetches self.data_file
 		"""
 		if not hasattr(self, 'data'):
-			self.data = numpy.loadtxt(self.data_file)
+			self.data = loadtxt2d(self.data_file)
 		return self.data
 	def get_equal_weighted_posterior(self):
 		"""
 			fetches self.data_file
 		"""
 		if not hasattr(self, 'equal_weighted_posterior'):
 			self.equal_weighted_posterior = loadtxt2d(self.equal_weighted_file)
```

### Comparing `pymultinest-2.7/pymultinest/__init__.py` & `pymultinest-2.9/pymultinest/__init__.py`

 * *Files identical despite different names*

### Comparing `pymultinest-2.7/pymultinest/solve.py` & `pymultinest-2.9/pymultinest/solve.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,17 +36,18 @@
 	if 'outputfiles_basename' not in kwargs:
 		files_temporary = True
 		tempdir = tempfile.mkdtemp('pymultinest')
 		kwargs['outputfiles_basename'] = tempdir + '/'
 	outputfiles_basename = kwargs['outputfiles_basename']
 	def SafePrior(cube, ndim, nparams):
 		try:
-			a = numpy.array([cube[i] for i in range(n_dims)])
+			n_params = kwargs.get('n_params', n_dims)
+			a = numpy.array([cube[i] for i in range(n_params)])
 			b = Prior(a)
-			for i in range(n_dims):
+			for i in range(n_params):
 				cube[i] = b[i]
 		except Exception as e:
 			import sys
 			sys.stderr.write('ERROR in prior: %s\n' % e)
 			sys.exit(1)
 	
 	def SafeLoglikelihood(cube, ndim, nparams, lnew):
```

### Comparing `pymultinest-2.7/pymultinest/run.py` & `pymultinest-2.9/pymultinest/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from __future__ import absolute_import, unicode_literals, print_function
 from ctypes import cdll
-import sys
+from ctypes.util import find_library 
+import sys, os
 
 libname = 'libmultinest'
 try: # detect if run through mpiexec/mpirun
 	from mpi4py import MPI
 	if MPI.COMM_WORLD.Get_size() > 1: # need parallel capabilities
 		libname = 'libmultinest_mpi'
-except ImportError:
-	pass
+except ImportError as e:
+	if 'PMIX_RANK' in os.environ:
+		print("Not using MPI because import mpi4py failed: '%s'. To debug, run python -c 'import mpi4py'.", e)
 
-libname += {
-	'darwin' : '.dylib',
-	'win32'  : '.dll',
-	'cygwin' : '.dll',
-}.get(sys.platform, '.so')
+libname = {
+	'darwin' : libname[len('lib'):],
+	'win32'  : libname + '.dll',
+	'cygwin' : libname + '.dll',
+}.get(sys.platform, libname + '.so')
 
 try:
+	if sys.platform == 'darwin':
+		libname = find_library(libname)
 	lib = cdll.LoadLibrary(libname)
 except OSError as e:
 	message = str(e)
 	if message == '%s: cannot open shared object file: No such file or directory' % libname:
 		print()
 		print('ERROR:   Could not load MultiNest library "%s"' % libname)
 		print('ERROR:   You have to build it first,')
```

### Comparing `pymultinest-2.7/pymultinest/plot.py` & `pymultinest-2.9/pymultinest/plot.py`

 * *Files identical despite different names*

### Comparing `pymultinest-2.7/pymultinest/watch.py` & `pymultinest-2.9/pymultinest/watch.py`

 * *Files identical despite different names*

### Comparing `pymultinest-2.7/pycuba/__init__.py` & `pymultinest-2.9/pycuba/__init__.py`

 * *Files identical despite different names*

### Comparing `pymultinest-2.7/pymultinest.egg-info/PKG-INFO` & `pymultinest-2.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: pymultinest
-Version: 2.7
+Version: 2.9
 Summary: Access modules for the MultiNest and Cuba integration libraries
 Home-page: http://johannesbuchner.github.com/PyMultiNest/
 Author: Johannes Buchner
 Author-email: johannes.buchner.acad@gmx.com
+Maintainer: Johannes Buchner
+Maintainer-email: johannes.buchner.acad@gmx.com
 License: GPLv3
-Description-Content-Type: UNKNOWN
 Description: PyMultiNest -- Python interface for MultiNest
         ==============================================
         
         This library provides programmatic access to MultiNest and PyCuba.
         
         What is MultiNest?
         -------------------
@@ -50,18 +51,53 @@
         
         The plotting can also be run on existing MultiNest output, and when not using PyMultiNest for running MultiNest.
         
         Citing PyMultiNest
         --------------------------------------------
         See http://johannesbuchner.github.com/PyMultiNest/index.html#citing-pymultinest
         
+        Plotting results, corner and trace plots
+        --------------------------------------------
+        
+        If you got pymultinest running with your likelihood (based on the pymultinest_demo*.py examples),
+        you can create plots of the marginal probability distributions.
+        
+        If you set outputfiles_basename="myprefix-" in the run,
+        you need to create a file myprefix-params.json which gives the names of each parameters,
+        for example::
+        
+        	[
+        	  "param1",
+        	  "param2",
+        	  "$N\_\mathrm{H}$",
+        	  "norm",
+        	]
+        
+        Then you can run::
+        
+        	$ python pymultinest-folder/multinest_marginals.py myprefix-
+        
+        which will create marginal plots for you.
+        
+        Recently I also added support for `corner.py <https://corner.readthedocs.io/>`_ (needs to be installed)::
+        
+        	$ python pymultinest-folder/multinest_marginals_corner.py myprefix-
+        
+        Also possible is trace and corner plots::
+        
+        	$ python pymultinest-folder/multinest_marginals_fancy.py myprefix-
+        
+        This last one has some potential drawbacks however: The code I borrowed here
+        from dynesty is not meant for multi-modal nested sampling which reorders the 
+        points, so the trace plot may not be 100% correct for multi-modal problems.
+        
         Questions and Problems
         --------------------------------------------
         
-        For any questions or problems with the software, please open an issue.
+        For any questions or problems with the software, please `open an issue <https://github.com/JohannesBuchner/PyMultiNest/issues>`_.
         This helps other people google the same question.
         
         Using MultiNest with Python?
         --------------------------------------------
         Look at the documentation available at http://johannesbuchner.github.com/PyMultiNest/index.html
         
         What is PyCuba?
@@ -80,13 +116,12 @@
         achieve full execution speed, as only native code is executed while
         MultiNest runs.
         
         
         
         
 Platform: UNKNOWN
-Requires: ctypesGsl
 Requires: numpy (>=1.5)
 Requires: matplotlib
 Requires: scipy
 Provides: pymultinest
 Provides: pycuba
```

### Comparing `pymultinest-2.7/PKG-INFO` & `pymultinest-2.9/pymultinest.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: pymultinest
-Version: 2.7
+Version: 2.9
 Summary: Access modules for the MultiNest and Cuba integration libraries
 Home-page: http://johannesbuchner.github.com/PyMultiNest/
 Author: Johannes Buchner
 Author-email: johannes.buchner.acad@gmx.com
+Maintainer: Johannes Buchner
+Maintainer-email: johannes.buchner.acad@gmx.com
 License: GPLv3
-Description-Content-Type: UNKNOWN
 Description: PyMultiNest -- Python interface for MultiNest
         ==============================================
         
         This library provides programmatic access to MultiNest and PyCuba.
         
         What is MultiNest?
         -------------------
@@ -50,18 +51,53 @@
         
         The plotting can also be run on existing MultiNest output, and when not using PyMultiNest for running MultiNest.
         
         Citing PyMultiNest
         --------------------------------------------
         See http://johannesbuchner.github.com/PyMultiNest/index.html#citing-pymultinest
         
+        Plotting results, corner and trace plots
+        --------------------------------------------
+        
+        If you got pymultinest running with your likelihood (based on the pymultinest_demo*.py examples),
+        you can create plots of the marginal probability distributions.
+        
+        If you set outputfiles_basename="myprefix-" in the run,
+        you need to create a file myprefix-params.json which gives the names of each parameters,
+        for example::
+        
+        	[
+        	  "param1",
+        	  "param2",
+        	  "$N\_\mathrm{H}$",
+        	  "norm",
+        	]
+        
+        Then you can run::
+        
+        	$ python pymultinest-folder/multinest_marginals.py myprefix-
+        
+        which will create marginal plots for you.
+        
+        Recently I also added support for `corner.py <https://corner.readthedocs.io/>`_ (needs to be installed)::
+        
+        	$ python pymultinest-folder/multinest_marginals_corner.py myprefix-
+        
+        Also possible is trace and corner plots::
+        
+        	$ python pymultinest-folder/multinest_marginals_fancy.py myprefix-
+        
+        This last one has some potential drawbacks however: The code I borrowed here
+        from dynesty is not meant for multi-modal nested sampling which reorders the 
+        points, so the trace plot may not be 100% correct for multi-modal problems.
+        
         Questions and Problems
         --------------------------------------------
         
-        For any questions or problems with the software, please open an issue.
+        For any questions or problems with the software, please `open an issue <https://github.com/JohannesBuchner/PyMultiNest/issues>`_.
         This helps other people google the same question.
         
         Using MultiNest with Python?
         --------------------------------------------
         Look at the documentation available at http://johannesbuchner.github.com/PyMultiNest/index.html
         
         What is PyCuba?
@@ -80,13 +116,12 @@
         achieve full execution speed, as only native code is executed while
         MultiNest runs.
         
         
         
         
 Platform: UNKNOWN
-Requires: ctypesGsl
 Requires: numpy (>=1.5)
 Requires: matplotlib
 Requires: scipy
 Provides: pymultinest
 Provides: pycuba
```

### Comparing `pymultinest-2.7/setup.py` & `pymultinest-2.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 long_description = None
 with open('README.rst') as file:
     long_description = file.read()
 
 setup(
     name = "pymultinest",
-    version = "2.7",
+    version = "2.9",
     description = "Access modules for the MultiNest and Cuba integration libraries",
     author = "Johannes Buchner",
     author_email = "johannes.buchner.acad@gmx.com",
     maintainer = "Johannes Buchner",
     maintainer_email = "johannes.buchner.acad@gmx.com",
     url = "http://johannesbuchner.github.com/PyMultiNest/",
     license = "GPLv3",
     packages = ["pymultinest", "pycuba"],
     provides = ["pymultinest", "pycuba"],
-    requires = ["ctypesGsl", "numpy (>=1.5)", "matplotlib", "scipy"],
-    scripts=['multinest_marginals.py'],
+    requires = ["numpy (>=1.5)", "matplotlib", "scipy"],
+    scripts=['multinest_marginals.py', 'multinest_marginals_corner.py', 'multinest_marginals_fancy.py'],
     long_description=long_description,
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
 )
```

