# Comparing `tmp/ConsistencyTEST-0.0.1.tar.gz` & `tmp/ConsistencyTEST-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConsistencyTEST-0.0.1.tar", last modified: Thu Dec  1 18:12:20 2022, max compression
+gzip compressed data, was "ConsistencyTEST-0.0.2.tar", last modified: Sat Jul 29 10:14:22 2023, max compression
```

## Comparing `ConsistencyTEST-0.0.1.tar` & `ConsistencyTEST-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-12-01 18:12:20.309056 ConsistencyTEST-0.0.1/
--rw-rw-rw-   0        0        0    11558 2022-06-03 23:42:55.000000 ConsistencyTEST-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     7941 2022-12-01 18:12:20.309056 ConsistencyTEST-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7422 2022-11-24 19:59:36.000000 ConsistencyTEST-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2022-06-03 23:29:06.000000 ConsistencyTEST-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      658 2022-12-01 18:12:20.311051 ConsistencyTEST-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-01 18:12:20.292101 ConsistencyTEST-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2022-12-01 18:12:20.298085 ConsistencyTEST-0.0.1/src/ConTEST/
--rw-rw-rw-   0        0        0    15959 2022-11-23 20:13:17.000000 ConsistencyTEST-0.0.1/src/ConTEST/CONTEST.py
--rw-rw-rw-   0        0        0        0 2022-06-04 12:09:39.000000 ConsistencyTEST-0.0.1/src/ConTEST/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-01 18:12:20.309056 ConsistencyTEST-0.0.1/src/ConsistencyTEST.egg-info/
--rw-rw-rw-   0        0        0     7941 2022-12-01 18:12:20.000000 ConsistencyTEST-0.0.1/src/ConsistencyTEST.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2022-12-01 18:12:20.000000 ConsistencyTEST-0.0.1/src/ConsistencyTEST.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-01 18:12:20.000000 ConsistencyTEST-0.0.1/src/ConsistencyTEST.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-12-01 18:12:20.000000 ConsistencyTEST-0.0.1/src/ConsistencyTEST.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 10:14:22.748188 ConsistencyTEST-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2022-06-03 23:42:55.000000 ConsistencyTEST-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     8436 2023-07-29 10:14:22.761153 ConsistencyTEST-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7691 2023-07-29 09:58:51.000000 ConsistencyTEST-0.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2022-06-03 23:29:06.000000 ConsistencyTEST-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      658 2023-07-29 10:14:22.767138 ConsistencyTEST-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 10:14:22.726248 ConsistencyTEST-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-29 10:14:22.732231 ConsistencyTEST-0.0.2/src/ConTEST/
+-rw-rw-rw-   0        0        0    16802 2023-07-29 09:56:30.000000 ConsistencyTEST-0.0.2/src/ConTEST/CONTEST.py
+-rw-rw-rw-   0        0        0        0 2022-06-04 12:09:39.000000 ConsistencyTEST-0.0.2/src/ConTEST/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:14:22.747193 ConsistencyTEST-0.0.2/src/ConsistencyTEST.egg-info/
+-rw-rw-rw-   0        0        0     8436 2023-07-29 10:14:22.000000 ConsistencyTEST-0.0.2/src/ConsistencyTEST.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-07-29 10:14:22.000000 ConsistencyTEST-0.0.2/src/ConsistencyTEST.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 10:14:22.000000 ConsistencyTEST-0.0.2/src/ConsistencyTEST.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 10:14:22.000000 ConsistencyTEST-0.0.2/src/ConsistencyTEST.egg-info/top_level.txt
```

### Comparing `ConsistencyTEST-0.0.1/LICENSE` & `ConsistencyTEST-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ConsistencyTEST-0.0.1/PKG-INFO` & `ConsistencyTEST-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConsistencyTEST
-Version: 0.0.1
+Version: 0.0.2
 Summary: Consistency test
 Home-page: https://github.com/FiorenST/ConTEST
 Author: Fiorenzo Stoppa
 Author-email: f.stoppa@astro.ru.nl
 Project-URL: Bug Tracker, https://github.com/FiorenST/ConTEST/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -42,51 +42,51 @@
 
 # Step-by-step setup
 
 _Follow the instructions below to install and start using ConTEST in Python._
 
 1. Install ConTEST:
    ```sh
-   pip intall ConTEST
+   pip install ConsistencyTEST
    ```
    or git clone the repository:
     ```sh
    git clone https://github.com/FiorenSt/ConTEST.git
    ```
    
 
  <br/>
 
-2. Install the statistical software [R](https://www.r-project.org/). R is needed to run some internal functions of ConTEST.
+2. (Optional) Install the statistical software [R](https://www.r-project.org/). R is required only if you plan to use the `smoothed_contest_reg()` function. This function employs local linear regression using the `np` package in R.
 <br/>
 
-3. To ensure that Python can access R's libraries, run the three lines below in Python (of course, modify to match your folders):
+3. (Optional) To ensure that Python can access R's libraries, run the three lines below in Python (of course, modify to match your folders). This step is only necessary if you intend to use the `smoothed_contest_reg()` function:
 
    ```sh
     import os
     os.environ['R_HOME'] = '~/Program Files/R/R-4.0.2'  #-> Your installed R folder
     os.environ['R_USER'] = '~/Miniconda3/envs/ConsistencyTest/lib/site-packages/'  #-> Your python environment
     os.environ['R_LIBS_USER'] = "~/Program Files/R/R-4.0.2/library/"  #-> Your R packages library
    ```
 <br/>
 
 
-4. Install Python dependencies (rpy2 needs R already installed):
+4. Install Python dependencies. Note that the `rpy2` package, which facilitates interaction between R and Python, is required only if you plan to use the `smoothed_contest_reg()` function:
    ```sh
    pip intall matplotlib
    pip intall numpy
    pip intall pandas
    pip intall scipy
    pip intall seaborn
    pip intall rpy2
    ```
  <br/>
 
 
-5. If this is the first time you use ConTEST, you need to install the R package used in Smoothed ConTEST. In Python, simply run:
+5. (Optional) If this is the first time you use ConTEST and you plan to use the `smoothed_contest_reg()` function, you need to install the R package used in Smoothed ConTEST. In Python, simply run:
 
    ```sh
     def install_R_functions(packnames=('np')):
         # import R's utility package
         utils = rpackages.importr('utils')
         # select a mirror for R packages
         utils.chooseCRANmirror(ind=1)  # select the first mirror in the list
@@ -132,15 +132,15 @@
 ConTEST can be applied in different case scenarios depending on the nature of the model being tested. 
 <br/>
 For more details check out the paper: _Stoppa et al., in preparation_
 
 There are 4 fundamental functions in ConTEST:
 
 - ConTEST for regression: Test the consistency of a model with respect to an observed dataset and their uncertainties
-- Smoothed ConTEST for regression: Test the consistency of a model with respect to an observed dataset and 
+- Smoothed ConTEST for regression (requires R and the `rpy2` Python package): Test the consistency of a model with respect to an observed dataset and 
   their uncertainties
 - ConTEST for outliers: Test if an observed sample is likely to come from a density model (or a simulated dataset)
 - ConTEST for densities: Test the consistency of a density model (or a simulated dataset) with respect to an observed 
   dataset 
 
 
 ### Intro script 
@@ -188,15 +188,15 @@
  
    ```sh
    Test1 = contest_reg(y_obs = obs, x_obs = x, y_mod = model, y_obs_err = err_obs, K=1000,plot=True)
    ```
 <img src="https://github.com/FiorenSt/ConTEST/blob/main/img/ConTESTforRegression.png " width=80% height=80%>
 
 
-### Smoothed ConTEST for regression
+### Smoothed ConTEST for regression (requires R and the `rpy2` Python package)
  
    ```sh
    Test2 = smoothed_contest_reg(y_obs = obs, x_obs = x, y_mod = model, y_obs_err = err_obs, K=1000,plot=True)   
    ```
 <img src="https://github.com/FiorenSt/ConTEST/blob/main/img/SmoothedConTESTforRegression.png " width=80% height=80%>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ConsistencyTEST Version: 0.0.1 Summary: Consistency
+Metadata-Version: 2.1 Name: ConsistencyTEST Version: 0.0.2 Summary: Consistency
 test Home-page: https://github.com/FiorenST/ConTEST Author: Fiorenzo Stoppa
 Author-email: f.stoppa@astro.ru.nl Project-URL: Bug Tracker, https://
 github.com/FiorenST/ConTEST/issues Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE [https://see.fontimg.com/api/
 renderfont4/KpAp/
@@ -12,29 +12,33 @@
 astrophysical models. It uses a combination of non-parametric methods and
 distance measures to obtain a test statistic that evaluates the closeness of
 the astrophysical model to the observations; hypothesis testing is then
 performed using bootstrap. [https://github.com/FiorenSt/ConTEST/blob/main/img/
 logo_contest_bkg.png] ## Table of Contents - [Step-by-step setup](#step-by-
 step-setup) - [Tutorial](#tutorial) # Step-by-step setup _Follow the
 instructions below to install and start using ConTEST in Python._ 1. Install
-ConTEST: ```sh pip intall ConTEST ``` or git clone the repository: ```sh git
-clone https://github.com/FiorenSt/ConTEST.git ```
-2. Install the statistical software [R](https://www.r-project.org/). R is
-needed to run some internal functions of ConTEST.
-3. To ensure that Python can access R's libraries, run the three lines below in
-Python (of course, modify to match your folders): ```sh import os os.environ
-['R_HOME'] = '~/Program Files/R/R-4.0.2' #-> Your installed R folder os.environ
-['R_USER'] = '~/Miniconda3/envs/ConsistencyTest/lib/site-packages/' #-> Your
-python environment os.environ['R_LIBS_USER'] = "~/Program Files/R/R-4.0.2/
-library/" #-> Your R packages library ```
-4. Install Python dependencies (rpy2 needs R already installed): ```sh pip
-intall matplotlib pip intall numpy pip intall pandas pip intall scipy pip
-intall seaborn pip intall rpy2 ```
-5. If this is the first time you use ConTEST, you need to install the R package
-used in Smoothed ConTEST. In Python, simply run: ```sh def install_R_functions
+ConTEST: ```sh pip install ConsistencyTEST ``` or git clone the repository:
+```sh git clone https://github.com/FiorenSt/ConTEST.git ```
+2. (Optional) Install the statistical software [R](https://www.r-project.org/).
+R is required only if you plan to use the `smoothed_contest_reg()` function.
+This function employs local linear regression using the `np` package in R.
+3. (Optional) To ensure that Python can access R's libraries, run the three
+lines below in Python (of course, modify to match your folders). This step is
+only necessary if you intend to use the `smoothed_contest_reg()` function:
+```sh import os os.environ['R_HOME'] = '~/Program Files/R/R-4.0.2' #-> Your
+installed R folder os.environ['R_USER'] = '~/Miniconda3/envs/ConsistencyTest/
+lib/site-packages/' #-> Your python environment os.environ['R_LIBS_USER'] = "~/
+Program Files/R/R-4.0.2/library/" #-> Your R packages library ```
+4. Install Python dependencies. Note that the `rpy2` package, which facilitates
+interaction between R and Python, is required only if you plan to use the
+`smoothed_contest_reg()` function: ```sh pip intall matplotlib pip intall numpy
+pip intall pandas pip intall scipy pip intall seaborn pip intall rpy2 ```
+5. (Optional) If this is the first time you use ConTEST and you plan to use the
+`smoothed_contest_reg()` function, you need to install the R package used in
+Smoothed ConTEST. In Python, simply run: ```sh def install_R_functions
 (packnames=('np')): # import R's utility package utils = rpackages.importr
 ('utils') # select a mirror for R packages utils.chooseCRANmirror(ind=1) #
 select the first mirror in the list # R package install utils.install_packages
 (packnames) install_R_functions() ``` 3. Use ConTEST in Python! Follow the
 tutorial below for more information about the individual functions.
 [https://github.com/FiorenSt/ConTEST/blob/main/img/MemeConTEST.png ]
 # Dependencies: The following combination of package versions works on most
@@ -44,41 +48,42 @@
 Scipy 1.7.1 * Matplotlib 3.3.4 * Seaborn 0.11.2 * Rpy2 3.5.2 (For R and Python
 interaction) ### R 3.6.0 (or superior) * Np 0.60 # Tutorial ConTEST can be
 applied in different case scenarios depending on the nature of the model being
 tested.
 For more details check out the paper: _Stoppa et al., in preparation_ There are
 4 fundamental functions in ConTEST: - ConTEST for regression: Test the
 consistency of a model with respect to an observed dataset and their
-uncertainties - Smoothed ConTEST for regression: Test the consistency of a
-model with respect to an observed dataset and their uncertainties - ConTEST for
-outliers: Test if an observed sample is likely to come from a density model (or
-a simulated dataset) - ConTEST for densities: Test the consistency of a density
-model (or a simulated dataset) with respect to an observed dataset ### Intro
-script ```sh # ensure that Python can access R import os os.environ['R_HOME'] =
-'~/Program Files/R/R-4.0.2' #-> Your installed R folder os.environ['R_USER'] =
-'~/Miniconda3/envs/ConsistencyTest/lib/site-packages/' #-> Your python
-environment os.environ['R_LIBS_USER'] = "~/Program Files/R/R-4.0.2/library/" #-
-> Your R packages library # load contest functions from ConTEST.CONTEST import
-contest_reg, smoothed_contest_reg, contest_outliers, contest_dens ``` ##
-Regression models Create synthetic model, observations, and uncertainties to
-test the functions: ```sh # random sample n=100 x = np.random.rand(n) #
-synthetic model beta1 = -0.3 beta2 = 8 m = 2 model = np.exp(beta1*x)*np.sin
-(beta2*x) + m # error function (Not known in real scenarios) err_model = model
-* .05 # sample observations from the model with the correct uncertainties obs =
-np.zeros(N) for i in range(N): obs[i] = model[i] +
-stats.multivariate_normal.rvs(mean=0, cov=(err_model[i])**2,size=1) # assign
-correct uncertainties to the observations err_obs = err_model ``` ### ConTEST
-for regression ```sh Test1 = contest_reg(y_obs = obs, x_obs = x, y_mod = model,
-y_obs_err = err_obs, K=1000,plot=True) ``` [https://github.com/FiorenSt/
-ConTEST/blob/main/img/ConTESTforRegression.png ] ### Smoothed ConTEST for
-regression ```sh Test2 = smoothed_contest_reg(y_obs = obs, x_obs = x, y_mod =
-model, y_obs_err = err_obs, K=1000,plot=True) ``` [https://github.com/FiorenSt/
-ConTEST/blob/main/img/SmoothedConTESTforRegression.png ] ## Density models
-Create synthetic model and observations: ```sh n=100 #1D example obs =
-stats.multivariate_normal.rvs(mean=5, cov= [1.5],size=n) model =
+uncertainties - Smoothed ConTEST for regression (requires R and the `rpy2`
+Python package): Test the consistency of a model with respect to an observed
+dataset and their uncertainties - ConTEST for outliers: Test if an observed
+sample is likely to come from a density model (or a simulated dataset) -
+ConTEST for densities: Test the consistency of a density model (or a simulated
+dataset) with respect to an observed dataset ### Intro script ```sh # ensure
+that Python can access R import os os.environ['R_HOME'] = '~/Program Files/R/R-
+4.0.2' #-> Your installed R folder os.environ['R_USER'] = '~/Miniconda3/envs/
+ConsistencyTest/lib/site-packages/' #-> Your python environment os.environ
+['R_LIBS_USER'] = "~/Program Files/R/R-4.0.2/library/" #-> Your R packages
+library # load contest functions from ConTEST.CONTEST import contest_reg,
+smoothed_contest_reg, contest_outliers, contest_dens ``` ## Regression models
+Create synthetic model, observations, and uncertainties to test the functions:
+```sh # random sample n=100 x = np.random.rand(n) # synthetic model beta1 = -
+0.3 beta2 = 8 m = 2 model = np.exp(beta1*x)*np.sin(beta2*x) + m # error
+function (Not known in real scenarios) err_model = model * .05 # sample
+observations from the model with the correct uncertainties obs = np.zeros(N)
+for i in range(N): obs[i] = model[i] + stats.multivariate_normal.rvs(mean=0,
+cov=(err_model[i])**2,size=1) # assign correct uncertainties to the
+observations err_obs = err_model ``` ### ConTEST for regression ```sh Test1 =
+contest_reg(y_obs = obs, x_obs = x, y_mod = model, y_obs_err = err_obs,
+K=1000,plot=True) ``` [https://github.com/FiorenSt/ConTEST/blob/main/img/
+ConTESTforRegression.png ] ### Smoothed ConTEST for regression (requires R and
+the `rpy2` Python package) ```sh Test2 = smoothed_contest_reg(y_obs = obs,
+x_obs = x, y_mod = model, y_obs_err = err_obs, K=1000,plot=True) ``` [https://
+github.com/FiorenSt/ConTEST/blob/main/img/SmoothedConTESTforRegression.png ] ##
+Density models Create synthetic model and observations: ```sh n=100 #1D example
+obs = stats.multivariate_normal.rvs(mean=5, cov= [1.5],size=n) model =
 stats.multivariate_normal.rvs(mean=5, cov= [1.5],size=1000) #2D example obs_2d
 = stats.multivariate_normal.rvs(mean=[5,5], cov= [[1.5,.8],[.8,2.5]],size=n)
 model_2d = stats.multivariate_normal.rvs(mean=[5,5], cov= [[1.5,.8],
 [.8,2.5]],size=1000) ### ConTEST for outliers ```sh Test3 = contest_outliers
 (mod=model, obs=obs, K=10000, plot=True) Test3 = contest_outliers(mod=model_2d,
 obs=obs_2d, K=10000, plot=True) ``` [https://github.com/FiorenSt/ConTEST/blob/
 main/img/ConTESTforOutliers1D.png ] [https://github.com/FiorenSt/ConTEST/blob/
```

### Comparing `ConsistencyTEST-0.0.1/README.md` & `ConsistencyTEST-0.0.2/src/ConsistencyTEST.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: ConsistencyTEST
+Version: 0.0.2
+Summary: Consistency test
+Home-page: https://github.com/FiorenST/ConTEST
+Author: Fiorenzo Stoppa
+Author-email: f.stoppa@astro.ru.nl
+Project-URL: Bug Tracker, https://github.com/FiorenST/ConTEST/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <img src=https://see.fontimg.com/api/renderfont4/KpAp/eyJyIjoiZnMiLCJoIjoxMzAsInciOjEwMDAsImZzIjoxMzAsImZnYyI6IiNGRDhDMDMiLCJiZ2MiOiIjMDYwNTA1IiwidCI6MX0/Q29uVEVTVA/kg-second-chances-sketch.png width=50% height=50%>
 
 
 <!--
 [![DOI](https://zenodo.org/badge/440851447.svg)](https://zenodo.org/badge/latestdoi/440851447) 
 <a href="https://ascl.net/2203.014"><img src="https://img.shields.io/badge/ascl-2203.014-blue.svg?colorB=262255" alt="ascl:2203.014" /></a>
 
@@ -27,51 +42,51 @@
 
 # Step-by-step setup
 
 _Follow the instructions below to install and start using ConTEST in Python._
 
 1. Install ConTEST:
    ```sh
-   pip intall ConTEST
+   pip install ConsistencyTEST
    ```
    or git clone the repository:
     ```sh
    git clone https://github.com/FiorenSt/ConTEST.git
    ```
    
 
  <br/>
 
-2. Install the statistical software [R](https://www.r-project.org/). R is needed to run some internal functions of ConTEST.
+2. (Optional) Install the statistical software [R](https://www.r-project.org/). R is required only if you plan to use the `smoothed_contest_reg()` function. This function employs local linear regression using the `np` package in R.
 <br/>
 
-3. To ensure that Python can access R's libraries, run the three lines below in Python (of course, modify to match your folders):
+3. (Optional) To ensure that Python can access R's libraries, run the three lines below in Python (of course, modify to match your folders). This step is only necessary if you intend to use the `smoothed_contest_reg()` function:
 
    ```sh
     import os
     os.environ['R_HOME'] = '~/Program Files/R/R-4.0.2'  #-> Your installed R folder
     os.environ['R_USER'] = '~/Miniconda3/envs/ConsistencyTest/lib/site-packages/'  #-> Your python environment
     os.environ['R_LIBS_USER'] = "~/Program Files/R/R-4.0.2/library/"  #-> Your R packages library
    ```
 <br/>
 
 
-4. Install Python dependencies (rpy2 needs R already installed):
+4. Install Python dependencies. Note that the `rpy2` package, which facilitates interaction between R and Python, is required only if you plan to use the `smoothed_contest_reg()` function:
    ```sh
    pip intall matplotlib
    pip intall numpy
    pip intall pandas
    pip intall scipy
    pip intall seaborn
    pip intall rpy2
    ```
  <br/>
 
 
-5. If this is the first time you use ConTEST, you need to install the R package used in Smoothed ConTEST. In Python, simply run:
+5. (Optional) If this is the first time you use ConTEST and you plan to use the `smoothed_contest_reg()` function, you need to install the R package used in Smoothed ConTEST. In Python, simply run:
 
    ```sh
     def install_R_functions(packnames=('np')):
         # import R's utility package
         utils = rpackages.importr('utils')
         # select a mirror for R packages
         utils.chooseCRANmirror(ind=1)  # select the first mirror in the list
@@ -117,15 +132,15 @@
 ConTEST can be applied in different case scenarios depending on the nature of the model being tested. 
 <br/>
 For more details check out the paper: _Stoppa et al., in preparation_
 
 There are 4 fundamental functions in ConTEST:
 
 - ConTEST for regression: Test the consistency of a model with respect to an observed dataset and their uncertainties
-- Smoothed ConTEST for regression: Test the consistency of a model with respect to an observed dataset and 
+- Smoothed ConTEST for regression (requires R and the `rpy2` Python package): Test the consistency of a model with respect to an observed dataset and 
   their uncertainties
 - ConTEST for outliers: Test if an observed sample is likely to come from a density model (or a simulated dataset)
 - ConTEST for densities: Test the consistency of a density model (or a simulated dataset) with respect to an observed 
   dataset 
 
 
 ### Intro script 
@@ -173,15 +188,15 @@
  
    ```sh
    Test1 = contest_reg(y_obs = obs, x_obs = x, y_mod = model, y_obs_err = err_obs, K=1000,plot=True)
    ```
 <img src="https://github.com/FiorenSt/ConTEST/blob/main/img/ConTESTforRegression.png " width=80% height=80%>
 
 
-### Smoothed ConTEST for regression
+### Smoothed ConTEST for regression (requires R and the `rpy2` Python package)
  
    ```sh
    Test2 = smoothed_contest_reg(y_obs = obs, x_obs = x, y_mod = model, y_obs_err = err_obs, K=1000,plot=True)   
    ```
 <img src="https://github.com/FiorenSt/ConTEST/blob/main/img/SmoothedConTESTforRegression.png " width=80% height=80%>
```

#### html2text {}

```diff
@@ -1,33 +1,44 @@
-[https://see.fontimg.com/api/renderfont4/KpAp/
+Metadata-Version: 2.1 Name: ConsistencyTEST Version: 0.0.2 Summary: Consistency
+test Home-page: https://github.com/FiorenST/ConTEST Author: Fiorenzo Stoppa
+Author-email: f.stoppa@astro.ru.nl Project-URL: Bug Tracker, https://
+github.com/FiorenST/ConTEST/issues Classifier: Programming Language :: Python
+:: 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
+Type: text/markdown License-File: LICENSE [https://see.fontimg.com/api/
+renderfont4/KpAp/
 eyJyIjoiZnMiLCJoIjoxMzAsInciOjEwMDAsImZzIjoxMzAsImZnYyI6IiNGRDhDMDMiLCJiZ2MiOiIjMDYwNTA1IiwidCI6MX0/
 Q29uVEVTVA/kg-second-chances-sketch.png]  # Description ConTEST is a
 statistical test for assessing the consistency between observations and
 astrophysical models. It uses a combination of non-parametric methods and
 distance measures to obtain a test statistic that evaluates the closeness of
 the astrophysical model to the observations; hypothesis testing is then
 performed using bootstrap. [https://github.com/FiorenSt/ConTEST/blob/main/img/
 logo_contest_bkg.png] ## Table of Contents - [Step-by-step setup](#step-by-
 step-setup) - [Tutorial](#tutorial) # Step-by-step setup _Follow the
 instructions below to install and start using ConTEST in Python._ 1. Install
-ConTEST: ```sh pip intall ConTEST ``` or git clone the repository: ```sh git
-clone https://github.com/FiorenSt/ConTEST.git ```
-2. Install the statistical software [R](https://www.r-project.org/). R is
-needed to run some internal functions of ConTEST.
-3. To ensure that Python can access R's libraries, run the three lines below in
-Python (of course, modify to match your folders): ```sh import os os.environ
-['R_HOME'] = '~/Program Files/R/R-4.0.2' #-> Your installed R folder os.environ
-['R_USER'] = '~/Miniconda3/envs/ConsistencyTest/lib/site-packages/' #-> Your
-python environment os.environ['R_LIBS_USER'] = "~/Program Files/R/R-4.0.2/
-library/" #-> Your R packages library ```
-4. Install Python dependencies (rpy2 needs R already installed): ```sh pip
-intall matplotlib pip intall numpy pip intall pandas pip intall scipy pip
-intall seaborn pip intall rpy2 ```
-5. If this is the first time you use ConTEST, you need to install the R package
-used in Smoothed ConTEST. In Python, simply run: ```sh def install_R_functions
+ConTEST: ```sh pip install ConsistencyTEST ``` or git clone the repository:
+```sh git clone https://github.com/FiorenSt/ConTEST.git ```
+2. (Optional) Install the statistical software [R](https://www.r-project.org/).
+R is required only if you plan to use the `smoothed_contest_reg()` function.
+This function employs local linear regression using the `np` package in R.
+3. (Optional) To ensure that Python can access R's libraries, run the three
+lines below in Python (of course, modify to match your folders). This step is
+only necessary if you intend to use the `smoothed_contest_reg()` function:
+```sh import os os.environ['R_HOME'] = '~/Program Files/R/R-4.0.2' #-> Your
+installed R folder os.environ['R_USER'] = '~/Miniconda3/envs/ConsistencyTest/
+lib/site-packages/' #-> Your python environment os.environ['R_LIBS_USER'] = "~/
+Program Files/R/R-4.0.2/library/" #-> Your R packages library ```
+4. Install Python dependencies. Note that the `rpy2` package, which facilitates
+interaction between R and Python, is required only if you plan to use the
+`smoothed_contest_reg()` function: ```sh pip intall matplotlib pip intall numpy
+pip intall pandas pip intall scipy pip intall seaborn pip intall rpy2 ```
+5. (Optional) If this is the first time you use ConTEST and you plan to use the
+`smoothed_contest_reg()` function, you need to install the R package used in
+Smoothed ConTEST. In Python, simply run: ```sh def install_R_functions
 (packnames=('np')): # import R's utility package utils = rpackages.importr
 ('utils') # select a mirror for R packages utils.chooseCRANmirror(ind=1) #
 select the first mirror in the list # R package install utils.install_packages
 (packnames) install_R_functions() ``` 3. Use ConTEST in Python! Follow the
 tutorial below for more information about the individual functions.
 [https://github.com/FiorenSt/ConTEST/blob/main/img/MemeConTEST.png ]
 # Dependencies: The following combination of package versions works on most
@@ -37,41 +48,42 @@
 Scipy 1.7.1 * Matplotlib 3.3.4 * Seaborn 0.11.2 * Rpy2 3.5.2 (For R and Python
 interaction) ### R 3.6.0 (or superior) * Np 0.60 # Tutorial ConTEST can be
 applied in different case scenarios depending on the nature of the model being
 tested.
 For more details check out the paper: _Stoppa et al., in preparation_ There are
 4 fundamental functions in ConTEST: - ConTEST for regression: Test the
 consistency of a model with respect to an observed dataset and their
-uncertainties - Smoothed ConTEST for regression: Test the consistency of a
-model with respect to an observed dataset and their uncertainties - ConTEST for
-outliers: Test if an observed sample is likely to come from a density model (or
-a simulated dataset) - ConTEST for densities: Test the consistency of a density
-model (or a simulated dataset) with respect to an observed dataset ### Intro
-script ```sh # ensure that Python can access R import os os.environ['R_HOME'] =
-'~/Program Files/R/R-4.0.2' #-> Your installed R folder os.environ['R_USER'] =
-'~/Miniconda3/envs/ConsistencyTest/lib/site-packages/' #-> Your python
-environment os.environ['R_LIBS_USER'] = "~/Program Files/R/R-4.0.2/library/" #-
-> Your R packages library # load contest functions from ConTEST.CONTEST import
-contest_reg, smoothed_contest_reg, contest_outliers, contest_dens ``` ##
-Regression models Create synthetic model, observations, and uncertainties to
-test the functions: ```sh # random sample n=100 x = np.random.rand(n) #
-synthetic model beta1 = -0.3 beta2 = 8 m = 2 model = np.exp(beta1*x)*np.sin
-(beta2*x) + m # error function (Not known in real scenarios) err_model = model
-* .05 # sample observations from the model with the correct uncertainties obs =
-np.zeros(N) for i in range(N): obs[i] = model[i] +
-stats.multivariate_normal.rvs(mean=0, cov=(err_model[i])**2,size=1) # assign
-correct uncertainties to the observations err_obs = err_model ``` ### ConTEST
-for regression ```sh Test1 = contest_reg(y_obs = obs, x_obs = x, y_mod = model,
-y_obs_err = err_obs, K=1000,plot=True) ``` [https://github.com/FiorenSt/
-ConTEST/blob/main/img/ConTESTforRegression.png ] ### Smoothed ConTEST for
-regression ```sh Test2 = smoothed_contest_reg(y_obs = obs, x_obs = x, y_mod =
-model, y_obs_err = err_obs, K=1000,plot=True) ``` [https://github.com/FiorenSt/
-ConTEST/blob/main/img/SmoothedConTESTforRegression.png ] ## Density models
-Create synthetic model and observations: ```sh n=100 #1D example obs =
-stats.multivariate_normal.rvs(mean=5, cov= [1.5],size=n) model =
+uncertainties - Smoothed ConTEST for regression (requires R and the `rpy2`
+Python package): Test the consistency of a model with respect to an observed
+dataset and their uncertainties - ConTEST for outliers: Test if an observed
+sample is likely to come from a density model (or a simulated dataset) -
+ConTEST for densities: Test the consistency of a density model (or a simulated
+dataset) with respect to an observed dataset ### Intro script ```sh # ensure
+that Python can access R import os os.environ['R_HOME'] = '~/Program Files/R/R-
+4.0.2' #-> Your installed R folder os.environ['R_USER'] = '~/Miniconda3/envs/
+ConsistencyTest/lib/site-packages/' #-> Your python environment os.environ
+['R_LIBS_USER'] = "~/Program Files/R/R-4.0.2/library/" #-> Your R packages
+library # load contest functions from ConTEST.CONTEST import contest_reg,
+smoothed_contest_reg, contest_outliers, contest_dens ``` ## Regression models
+Create synthetic model, observations, and uncertainties to test the functions:
+```sh # random sample n=100 x = np.random.rand(n) # synthetic model beta1 = -
+0.3 beta2 = 8 m = 2 model = np.exp(beta1*x)*np.sin(beta2*x) + m # error
+function (Not known in real scenarios) err_model = model * .05 # sample
+observations from the model with the correct uncertainties obs = np.zeros(N)
+for i in range(N): obs[i] = model[i] + stats.multivariate_normal.rvs(mean=0,
+cov=(err_model[i])**2,size=1) # assign correct uncertainties to the
+observations err_obs = err_model ``` ### ConTEST for regression ```sh Test1 =
+contest_reg(y_obs = obs, x_obs = x, y_mod = model, y_obs_err = err_obs,
+K=1000,plot=True) ``` [https://github.com/FiorenSt/ConTEST/blob/main/img/
+ConTESTforRegression.png ] ### Smoothed ConTEST for regression (requires R and
+the `rpy2` Python package) ```sh Test2 = smoothed_contest_reg(y_obs = obs,
+x_obs = x, y_mod = model, y_obs_err = err_obs, K=1000,plot=True) ``` [https://
+github.com/FiorenSt/ConTEST/blob/main/img/SmoothedConTESTforRegression.png ] ##
+Density models Create synthetic model and observations: ```sh n=100 #1D example
+obs = stats.multivariate_normal.rvs(mean=5, cov= [1.5],size=n) model =
 stats.multivariate_normal.rvs(mean=5, cov= [1.5],size=1000) #2D example obs_2d
 = stats.multivariate_normal.rvs(mean=[5,5], cov= [[1.5,.8],[.8,2.5]],size=n)
 model_2d = stats.multivariate_normal.rvs(mean=[5,5], cov= [[1.5,.8],
 [.8,2.5]],size=1000) ### ConTEST for outliers ```sh Test3 = contest_outliers
 (mod=model, obs=obs, K=10000, plot=True) Test3 = contest_outliers(mod=model_2d,
 obs=obs_2d, K=10000, plot=True) ``` [https://github.com/FiorenSt/ConTEST/blob/
 main/img/ConTESTforOutliers1D.png ] [https://github.com/FiorenSt/ConTEST/blob/
```

### Comparing `ConsistencyTEST-0.0.1/setup.cfg` & `ConsistencyTEST-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 6f6e 7369 7374 656e 6379 5445   = ConsistencyTE
 00000020: 5354 0d0a 7665 7273 696f 6e20 3d20 302e  ST..version = 0.
-00000030: 302e 310d 0a61 7574 686f 7220 3d20 4669  0.1..author = Fi
+00000030: 302e 320d 0a61 7574 686f 7220 3d20 4669  0.2..author = Fi
 00000040: 6f72 656e 7a6f 2053 746f 7070 610d 0a61  orenzo Stoppa..a
 00000050: 7574 686f 725f 656d 6169 6c20 3d20 662e  uthor_email = f.
 00000060: 7374 6f70 7061 4061 7374 726f 2e72 752e  stoppa@astro.ru.
 00000070: 6e6c 0d0a 6465 7363 7269 7074 696f 6e20  nl..description 
 00000080: 3d20 436f 6e73 6973 7465 6e63 7920 7465  = Consistency te
 00000090: 7374 0d0a 6c6f 6e67 5f64 6573 6372 6970  st..long_descrip
 000000a0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
```

### Comparing `ConsistencyTEST-0.0.1/src/ConTEST/CONTEST.py` & `ConsistencyTEST-0.0.2/src/ConTEST/CONTEST.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,381 +1,405 @@
-########################################################################################################################
-#                                                                                                                      #
-#         ########      ## ## ##        ##         ##    ############   ## ########       #########     ############   #
-#       ##            ##        ##      ## #       ##         ##        ##               ##                  ##        #
-#      ##            ##          ##     ##  #      ##         ##        ##               ##                  ##        #
-#     ##            ##            ##    ##   #     ##         ##        ##                ##                 ##        #
-#     ##            ##            ##    ##    #    ##         ##        ## ########         ##               ##        #
-#     ##            ##            ##    ##     #   ##         ##        ##                     ##            ##        #
-#      ##            ##          ##     ##      #  ##         ##        ##                       ##          ##        #
-#       ##            ##        ##      ##       # ##         ##        ##                       ##          ##        #
-#         ########      ## ## ##        ##         ##         ##        ## ########     ##########           ##        #
-#                                                                                                                      #
-########################################################################################################################
-
-
-###################
-# PYTHON PACKAGES #
-###################
-
-import matplotlib.pyplot as plt
-import numpy
-import pandas as pd
-import seaborn as sns
-from scipy import stats
-
-
-############################
-# ALLOW R TO ACCESS PYTHON #
-############################
-
-# import os
-#os.environ['R_HOME'] = '~/Program Files/R/R-4.0.2'  #-> Your installed R folder
-# os.environ['R_USER'] = '~/Miniconda3/envs/ConsistencyTest/lib/site-packages/'  #-> Your python environment
-# os.environ['R_LIBS_USER'] = "~/Program Files/R/R-4.0.2/library/"  #-> Your R packages library
-
-import rpy2.robjects.packages as rpackages
-import rpy2.robjects.numpy2ri
-import rpy2.robjects
-
-
-###########################################  REGRESSION  ##############################################
-###########################################    MODELS    ##############################################
-
-
-##########################
-# CONTEST FOR REGRESSION #
-##########################
-
-def contest_reg(y_obs, x_obs, y_mod, y_obs_err, K=10000, seed=1, signif_lev=0.05, plot=False):
-
-    # Observations size
-    n = len(y_obs)
-
-    # Estimate the test statistic
-    t = numpy.sqrt(numpy.sum(((y_mod - y_obs) / y_obs_err) ** 2) / n)
-
-    # Simulate K dataset with the model as ground truth and the observed uncertainties as covariance matrix
-    sim = numpy.zeros((n, K))
-    numpy.random.seed(seed)
-    for i in range(n):
-        sim[i, :] = y_mod[i] + stats.multivariate_normal.rvs(mean=0, cov= (y_obs_err[i])**2,size=K)
-
-    # Estimate the test statistics for the simulated samples
-    t_sim = numpy.sqrt(
-        numpy.sum(((numpy.array([y_mod, ] * K).T - sim) / numpy.array([y_obs_err, ] * K).T) ** 2, axis=0) / n)
-
-    # Calculate the P_value
-    p_value = 2 * min(numpy.mean(t_sim <= t), numpy.mean(t_sim >= t))
-
-    if p_value < signif_lev:
-        print(
-            'Test statistic: {}, P-value: {} \nThe Null Hypothesis in Rejected: the model is not consistent with the '
-            'observations.'.format(
-                numpy.round(t, 4), p_value))
-    else:
-        print(
-            'Test statistic: {}, P-value: {} \nThe Null Hypothesis in Not Rejected: the model is consistent with the '
-            'observations.'.format(
-                numpy.round(t, 4), p_value))
-
-    if plot:
-        plt.figure(figsize=(12,6))
-
-        order = numpy.argsort(x_obs)
-        plt.subplot(1, 2, 1)
-        plt.plot(x_obs[order], y_mod[order],color="#4E84C4", label='Model')
-        plt.errorbar(x_obs[order], y_obs[order], yerr=y_obs_err[order], fmt='.k')
-        plt.scatter(x_obs[order], y_obs[order], s=2, color='black')
-        plt.legend()
-
-        plt.subplot(1, 2, 2)
-        s = sns.kdeplot(t_sim, fill=True, color="gray")
-        plt.vlines(t, ymin=0, ymax=s.dataLim.bounds[3], colors="#D16103",linestyle='--', label='Test stat.')
-        plt.vlines(numpy.quantile(t_sim, q=signif_lev / 2), ymin=0, ymax=s.dataLim.bounds[3], colors="#293352",
-                   linestyle='--', label='97.5%')
-        plt.vlines(numpy.quantile(t_sim, q=1 - (signif_lev / 2)), ymin=0, ymax=s.dataLim.bounds[3],
-                   colors="#293352",linestyle='--', label='2.5%')
-        plt.legend()
-    return pd.DataFrame({'Test': t, 'Bootstrap': t_sim, 'P_value': p_value})
-
-
-
-###################################
-# SMOOTHED CONTEST FOR REGRESSION #
-###################################
-
-def smoothed_contest_reg(y_obs, x_obs, y_mod, y_obs_err, K=1000, seed=1, signif_lev=0.05, bwtype='fixed', plot=False):
-
-    rpy2.robjects.numpy2ri.activate()
-
-    # Observations size
-    n = len(y_obs)
-
-    # Load package for Local Linear Regression
-    np = rpackages.importr('np')
-
-    # Transform observations and model to format suitable for R
-    x_obs_r = rpy2.robjects.r['matrix'](numpy.array(x_obs),ncol=x_obs.ndim)
-    y_obs_r = rpy2.robjects.FloatVector(y_obs)
-
-    # R script for the LLR
-    rpy2.robjects.r('''
-            # create a function `f`
-            f <- function(y_obs_r, x_obs_r, bwtype) {
-                bw.fixed <- npregbw(ydat=y_obs_r,
-                              xdat=x_obs_r,
-                              regtype = "ll",
-                              bwmethod = "cv.aic",
-                              gradients = FALSE,
-                              bwtype= bwtype,
-                              nmulti=1)
-          
-            model.fixed = npreg(bw.fixed)
-          
-            est_fixed=model.fixed$mean
-            unc_fixed=model.fixed$merr
-            
-            return(cbind(est_fixed,unc_fixed))
-            }
-            ''')
-
-    # Run the LLR on the original dataset
-    r_f = rpy2.robjects.globalenv['f']
-    y_obs_smoothed = r_f(y_obs_r, x_obs_r, bwtype)
-
-    # Estimate the test statistic
-    t = numpy.sqrt(numpy.sum(((y_mod - y_obs_smoothed[:,0]) / y_obs_smoothed[:,1]) ** 2) / n)
-
-    # Simulate K dataset with the model as ground truth and the observed uncertainties as covariance matrix
-    sim = numpy.zeros((n, K))
-    numpy.random.seed(seed)
-    for i in range(n):
-        sim[i, :] = y_mod[i] + stats.multivariate_normal.rvs(mean=0, cov= (y_obs_err[i])**2,size=K)
-
-    # Run the LLR on the simulated samples
-    y_obs_smoothed_sim = numpy.zeros((n,K,2))
-    for k in range(K):
-        y_sim = rpy2.robjects.FloatVector(sim[:,k])
-        y_obs_smoothed_sim[:,k,:] = r_f(y_sim, x_obs_r, bwtype)
-
-
-    # Estimate the test statistics for the simulated samples
-    t_sim = numpy.sqrt(
-        numpy.sum(((numpy.array([y_mod, ] * K).T - y_obs_smoothed_sim[:,:,0]) / y_obs_smoothed_sim[:,:,1]) ** 2, axis=0) / n)
-
-    # Calculate the P_value
-    p_value = 2 * min(numpy.mean(t_sim <= t), numpy.mean(t_sim >= t))
-
-    if p_value < signif_lev:
-        print(
-            'Test statistic: {}, P-value: {} \nThe Null Hypothesis in Rejected: the model is not consistent with the '
-            'observations.'.format(
-                numpy.round(t, 4), p_value))
-    else:
-        print(
-            'Test statistic: {}, P-value: {} \nThe Null Hypothesis in Not Rejected: the model is consistent with the '
-            'observations.'.format(
-                numpy.round(t, 4), p_value))
-
-    if plot:
-        plt.figure(figsize=(12,6))
-        order = numpy.argsort(x_obs)
-
-        plt.subplot(1, 2, 1)
-        plt.plot(x_obs[order], y_mod[order],color="#4E84C4", label='Model')
-        plt.plot(x_obs[order], y_obs_smoothed[:,0][order],color="#D16103", label='Obs.')
-        plt.plot(x_obs[order], y_obs_smoothed[:, 0][order]+y_obs_smoothed[:, 1][order],'--',color="#D16103")
-        plt.plot(x_obs[order], y_obs_smoothed[:, 0][order]-y_obs_smoothed[:, 1][order],'--',color="#D16103")
-        plt.errorbar(x_obs[order], y_obs[order], yerr=y_obs_err[order], fmt='.k')
-        plt.scatter(x_obs[order], y_obs[order], s=2, color='black')
-        plt.legend()
-
-        plt.subplot(1, 2, 2)
-        s = sns.kdeplot(t_sim, fill=True, color="gray")
-        plt.vlines(t, ymin=0, ymax=s.dataLim.bounds[3], color="#D16103",linestyle='--', label='Test stat.')
-        plt.vlines(numpy.quantile(t_sim, q=signif_lev / 2), ymin=0, ymax=s.dataLim.bounds[3], color="#293352",
-                   linestyle='--', label='97.5%')
-        plt.vlines(numpy.quantile(t_sim, q=1 - (signif_lev / 2)), ymin=0, ymax=s.dataLim.bounds[3], color="#293352",
-                   linestyle='--', label='2.5%')
-        plt.legend()
-
-    return pd.DataFrame({'Test': t, 'Bootstrap': t_sim, 'P_value': p_value})
-
-
-
-
-###########################################  DENSITY  ##################################################
-###########################################  MODELS   ##################################################
-
-
-########################
-# CONTEST FOR OUTLIERS #
-########################
-
-
-def contest_outliers(mod, obs, K=1000, signif_lev=0.05, plot=False):
-
-    # Sample size
-    n = obs.shape[0]
-
-    # Transformation for scipy multivariate Kernel Density Estimation
-    if obs.ndim == 2:
-        mod = mod.T
-        obs = obs.T
-
-    # Estimate the model's density
-    g = stats.gaussian_kde(mod)
-
-    # Estimate the test statistic
-    t = -numpy.mean(g.logpdf(obs))
-
-    # Simulate K dataset and estimate their test statistics
-    t_sim = numpy.zeros((K))
-    for k in range(K):
-        sim = g.resample(n)
-        t_sim[k] = -numpy.mean(g.logpdf(sim))
-
-    # Calculate the P_value
-    p_value = 2 * min(numpy.mean(t_sim <= t), numpy.mean(t_sim >= t))
-
-    if p_value < signif_lev:
-        print(
-            'Test statistic: {}, P-value: {} \nThe Null Hypothesis in Rejected: the model is not consistent with the '
-            'observations.'.format(
-                numpy.round(t, 4), p_value))
-    else:
-        print(
-            'Test statistic: {}, P-value: {} \nThe Null Hypothesis in Not Rejected: the model is consistent with the '
-            'observations.'.format(
-                numpy.round(t, 4), p_value))
-
-    if plot:
-        if obs.ndim == 1:
-            plt.figure(figsize=(12, 6))
-            plt.subplot(1, 2, 1)
-            sns.kdeplot(x=mod, levels=[0.25,0.50,0.75], color="#4E84C4", linestyle='--', label='Model')
-            plt.plot(obs, -0.00005 * numpy.ones(100), "|", color='black')
-            plt.legend()
-
-            plt.subplot(1, 2, 2)
-            s = sns.kdeplot(t_sim, fill=True, color="gray")
-            plt.vlines(t, ymin=0, ymax=s.dataLim.bounds[3], colors="#D16103", linestyle='--', label='Test stat.')
-            plt.vlines(numpy.quantile(t_sim, q=1 - (signif_lev / 2)), ymin=0, ymax=s.dataLim.bounds[3],
-                       colors="#293352", linestyle='--', label='97.5%')
-            plt.vlines(numpy.quantile(t_sim, q=signif_lev / 2), ymin=0, ymax=s.dataLim.bounds[3], colors="#293352",
-                       linestyle='--', label='2.5%')
-            plt.legend()
-
-
-        if obs.ndim == 2:
-            plt.figure(figsize=(12, 6))
-            plt.subplot(1, 2, 1)
-            sns.kdeplot(x=mod[0,:], y=mod[1,:], levels=[0.25,0.50,0.75], color="#4E84C4", linestyles='--',
-                        label='Model')
-            plt.scatter(x=obs[0,:], y=obs[1,:], s=2, color='black')
-            plt.legend()
-
-            plt.subplot(1, 2, 2)
-            s = sns.kdeplot(t_sim, fill=True, color="gray")
-            plt.vlines(t, ymin=0, ymax=s.dataLim.bounds[3], color="#D16103", linestyle='--', label='Test stat.')
-            plt.vlines(numpy.quantile(t_sim, q=1 - (signif_lev / 2)), ymin=0, ymax=s.dataLim.bounds[3],
-                       color="#293352", linestyle='--', label='97.5%')
-            plt.vlines(numpy.quantile(t_sim, q=signif_lev / 2), ymin=0, ymax=s.dataLim.bounds[3], color="#293352",
-                       linestyle='--', label='2.5%')
-            plt.legend()
-
-    return pd.DataFrame({'Test': t, 'Bootstrap': t_sim, 'P_value': p_value})
-
-
-
-##########################
-# CONTEST FOR DENSITIES #
-##########################
-
-def contest_dens(mod, obs, K=1000, signif_lev=0.05, plot=False):
-    # Sample size
-    n = obs.shape[0]
-
-    # Transformation for scipy multivariate Kernel Density Estimation
-    if obs.ndim == 2:
-        mod = mod.T
-        obs = obs.T
-
-    # Estimate the model's density
-    g = stats.gaussian_kde(mod)
-
-    # Estimate the observations' density
-    f = stats.gaussian_kde(obs)
-
-    # MCMC to estimate the test statistic
-    J = 1000
-    x_g = g.resample(J)
-    d_g = g.pdf(x_g)
-    d_f = f.pdf(x_g)
-
-    # Estimate the test statistics
-    t = sum(abs(d_f / d_g - 1)) / J
-
-    # Simulate K dataset and estimate their test statistics
-    t_sim = numpy.zeros((K))
-    for k in range(K):
-        sim = g.resample(n)
-        f_sim = stats.gaussian_kde(sim)
-        d_f_sim = f_sim.pdf(x_g)
-        t_sim[k] = sum(abs(d_f_sim / d_g - 1)) / J
-
-    # P-value
-    p_value = numpy.mean(t_sim >= t)
-
-    if p_value < signif_lev:
-        print(
-            'Test statistic: {}, P-value: {} \nThe Null hypothesis in Rejected: the model is not consistent with the '
-            'observations.'.format(
-                numpy.round(t, 4),  numpy.round(p_value,4)))
-    else:
-        print(
-            'Test statistic: {}, P-value: {} \nThe Null hypothesis in Not Rejected: the model is consistent with the '
-            'observations.'.format(
-                numpy.round(t, 4),  numpy.round(p_value,4)))
-
-    if plot:
-
-        if obs.ndim == 1:
-            plt.figure(figsize=(12, 6))
-            plt.subplot(1, 2, 1)
-            sns.kdeplot(x=mod, levels=[0.25,0.50,0.75], color="#4E84C4", linestyle='--', label='Model')
-            sns.kdeplot(x=obs, levels=[0.25,0.50,0.75], color="#D16103", label='Obs.')
-            plt.plot(obs, -0.00005 * numpy.ones(100), "|", color='black')
-            plt.legend()
-
-
-            plt.subplot(1, 2, 2)
-            s = sns.kdeplot(t_sim, fill=True, color="gray")
-            plt.vlines(t, ymin=0, ymax=s.dataLim.bounds[3], colors="#D16103", linestyle='--', label='Test stat.')
-            plt.vlines(numpy.quantile(t_sim, q=1 - signif_lev), ymin=0, ymax=s.dataLim.bounds[3], colors="#293352",
-                       linestyle='--', label='95%')
-            plt.legend()
-
-
-        if obs.ndim == 2:
-            plt.figure(figsize=(12, 6))
-            plt.subplot(1, 2, 1)
-            sns.kdeplot(x=mod[0,:], y=mod[1,:], levels=[0.25,0.50,0.75], colors="#4E84C4", linestyles='--',
-                        label='Model')
-            sns.kdeplot(x=obs[0,:], y=obs[1,:], levels=[0.25,0.50,0.75], colors="#D16103", label='Obs.')
-            plt.scatter(x=obs[0,:], y=obs[1,:], s=2, color='black')
-            plt.legend()
-
-            plt.subplot(1, 2, 2)
-            s = sns.kdeplot(t_sim, fill=True, color="gray")
-            plt.vlines(t, ymin=0, ymax=s.dataLim.bounds[3], colors="#D16103",linestyle='--', label='Test stat.')
-            plt.vlines(numpy.quantile(t_sim, q=1 - signif_lev), ymin=0, ymax=s.dataLim.bounds[3], colors="#293352",
-                       linestyle='--', label='95%')
-            plt.legend()
-
-    return pd.DataFrame({'Test': t, 'Bootstrap': t_sim, 'P_value': p_value})
-
-
-
-if __name__ == '__main__':
+########################################################################################################################
+#                                                                                                                      #
+#         ########      ## ## ##        ##         ##    ############   ## ########       #########     ############   #
+#       ##            ##        ##      ## #       ##         ##        ##               ##                  ##        #
+#      ##            ##          ##     ##  #      ##         ##        ##               ##                  ##        #
+#     ##            ##            ##    ##   #     ##         ##        ##                ##                 ##        #
+#     ##            ##            ##    ##    #    ##         ##        ## ########         ##               ##        #
+#     ##            ##            ##    ##     #   ##         ##        ##                     ##            ##        #
+#      ##            ##          ##     ##      #  ##         ##        ##                       ##          ##        #
+#       ##            ##        ##      ##       # ##         ##        ##                       ##          ##        #
+#         ########      ## ## ##        ##         ##         ##        ## ########     ##########           ##        #
+#                                                                                                                      #
+########################################################################################################################
+
+
+###################
+# PYTHON PACKAGES #
+###################
+
+import matplotlib.pyplot as plt
+import numpy
+import pandas as pd
+import seaborn as sns
+from scipy import stats
+
+
+############################
+# ALLOW R TO ACCESS PYTHON #
+############################
+
+# import os
+#os.environ['R_HOME'] = '~/Program Files/R/R-4.0.2'  #-> Your installed R folder
+# os.environ['R_USER'] = '~/Miniconda3/envs/ConsistencyTest/lib/site-packages/'  #-> Your python environment
+# os.environ['R_LIBS_USER'] = "~/Program Files/R/R-4.0.2/library/"  #-> Your R packages library
+
+
+try:
+    import rpy2.robjects.packages as rpackages
+    import rpy2.robjects.numpy2ri
+    import rpy2.robjects
+    rpy2_imported = True
+except ImportError:
+    rpy2_imported = False
+    print("Warning: rpy2 module not found. The function smoothed_contest_reg() will not work without it. If you need this function, please install rpy2.")
+    
+
+###########################################  REGRESSION  ##############################################
+###########################################    MODELS    ##############################################
+
+
+##########################
+# CONTEST FOR REGRESSION #
+##########################
+
+def contest_reg(y_obs, x_obs, y_mod, y_obs_err, K=10000, seed=1, signif_lev=0.05, plot=False):
+
+    # Observations size
+    n = len(y_obs)
+
+    # Check if input is a vector or a matrix
+    if y_obs_err.ndim == 1:
+        y_obs_err = y_obs_err
+        # Estimate the test statistic for 1D case
+        t = numpy.sqrt(numpy.sum(((y_mod - y_obs) / y_obs_err) ** 2) / n)
+
+        # Simulate K dataset with the model as ground truth and the observed uncertainties for 1D case
+        sim = numpy.zeros((n, K))
+        numpy.random.seed(seed)
+        for i in range(n):
+            sim[i, :] = y_mod[i] + stats.multivariate_normal.rvs(mean=0, cov=(y_obs_err[i]) ** 2, size=K)
+
+        # Estimate the test statistics for the simulated samples for 1D case
+        t_sim = numpy.sqrt(
+            numpy.sum(((numpy.array([y_mod, ] * K).T - sim) / numpy.array([y_obs_err, ] * K).T) ** 2, axis=0) / n)
+
+    else:
+        y_obs_cov = y_obs_err
+        # Estimate the test statistic for 2D case
+        t = numpy.sqrt(numpy.dot((y_mod - y_obs).T, numpy.linalg.inv(y_obs_cov)).dot(y_mod - y_obs) / n)
+
+        # Simulate K dataset with the model as ground truth and the observed uncertainties as covariance matrix for 2D case
+        sim = numpy.zeros((n, K))
+        numpy.random.seed(seed)
+        for i in range(K):
+            sim[:, i] = stats.multivariate_normal.rvs(mean=y_mod, cov=y_obs_cov)
+
+        # Estimate the test statistics for the simulated samples for 2D case
+        t_sim = numpy.sqrt(numpy.sum((y_mod[:, None] - sim).T * numpy.linalg.inv(y_obs_cov).dot(y_mod[:, None] - sim).T, axis=1) / n)
+
+    # Calculate the P_value
+    p_value = 2 * min(numpy.mean(t_sim <= t), numpy.mean(t_sim >= t))
+
+    if p_value < signif_lev:
+        print(
+            'Test statistic: {}, P-value: {} \nThe Null Hypothesis in Rejected: the model is not consistent with the '
+            'observations.'.format(
+                numpy.round(t, 4), p_value))
+    else:
+        print(
+            'Test statistic: {}, P-value: {} \nThe Null Hypothesis in Not Rejected: the model is consistent with the '
+            'observations.'.format(
+                numpy.round(t, 4), p_value))
+
+    if plot:
+        plt.figure(figsize=(12,6))
+
+        order = numpy.argsort(x_obs)
+        plt.subplot(1, 2, 1)
+        plt.plot(x_obs[order], y_mod[order],color="#4E84C4", label='Model')
+        plt.errorbar(x_obs[order], y_obs[order], yerr=y_obs_err[order], fmt='.k')
+        plt.scatter(x_obs[order], y_obs[order], s=2, color='black')
+        plt.legend()
+
+        plt.subplot(1, 2, 2)
+        s = sns.kdeplot(t_sim, fill=True, color="gray")
+        plt.vlines(t, ymin=0, ymax=s.dataLim.bounds[3], colors="#D16103",linestyle='--', label='Test stat.')
+        plt.vlines(numpy.nanquantile(t_sim, q=signif_lev / 2), ymin=0, ymax=s.dataLim.bounds[3], colors="#293352",
+                   linestyle='--', label='97.5%')
+        plt.vlines(numpy.nanquantile(t_sim, q=1 - (signif_lev / 2)), ymin=0, ymax=s.dataLim.bounds[3],
+                   colors="#293352",linestyle='--', label='2.5%')
+        plt.legend()
+
+    return pd.DataFrame({'Test': t, 'Bootstrap': t_sim, 'P_value': p_value})
+
+
+
+###################################
+# SMOOTHED CONTEST FOR REGRESSION #
+###################################
+
+def smoothed_contest_reg(y_obs, x_obs, y_mod, y_obs_err, K=1000, seed=1, signif_lev=0.05, bwtype='fixed', plot=False, verbose=0):
+
+    rpy2.robjects.numpy2ri.activate()
+
+    # Observations size
+    n = len(y_obs)
+
+    # Load package for Local Linear Regression
+    np = rpackages.importr('np')
+
+    # Transform observations and model to format suitable for R
+    x_obs_r = rpy2.robjects.r['matrix'](numpy.array(x_obs),ncol=x_obs.ndim)
+    y_obs_r = rpy2.robjects.FloatVector(y_obs)
+
+    # R script for the LLR
+    rpy2.robjects.r('''
+            # create a function `f`
+            f <- function(y_obs_r, x_obs_r, bwtype) {
+                bw.fixed <- npregbw(ydat=y_obs_r,
+                              xdat=x_obs_r,
+                              regtype = "ll",
+                              bwmethod = "cv.aic",
+                              gradients = FALSE,
+                              bwtype= bwtype,
+                              nmulti=1)
+          
+            model.fixed = npreg(bw.fixed)
+          
+            est_fixed=model.fixed$mean
+            unc_fixed=model.fixed$merr
+            
+            return(cbind(est_fixed,unc_fixed))
+            }
+            ''')
+
+    # Run the LLR on the original dataset
+    r_f = rpy2.robjects.globalenv['f']
+    y_obs_smoothed = r_f(y_obs_r, x_obs_r, bwtype)
+
+    # Estimate the test statistic
+    t = numpy.sqrt(numpy.sum(((y_mod - y_obs_smoothed[:,0]) / y_obs_smoothed[:,1]) ** 2) / n)
+
+    # Simulate K dataset with the model as ground truth and the observed uncertainties as covariance matrix
+    sim = numpy.zeros((n, K))
+    numpy.random.seed(seed)
+    for i in range(n):
+        sim[i, :] = y_mod[i] + stats.multivariate_normal.rvs(mean=0, cov= (y_obs_err[i])**2,size=K)
+
+    # Run the LLR on the simulated samples
+    y_obs_smoothed_sim = numpy.zeros((n,K,2))
+    for k in range(K):
+        y_sim = rpy2.robjects.FloatVector(sim[:,k])
+        y_obs_smoothed_sim[:,k,:] = r_f(y_sim, x_obs_r, bwtype)
+        if verbose == 1: print('Iteration:' + k)
+
+    # Estimate the test statistics for the simulated samples
+    t_sim = numpy.sqrt(
+        numpy.sum(((numpy.array([y_mod, ] * K).T - y_obs_smoothed_sim[:,:,0]) / y_obs_smoothed_sim[:,:,1]) ** 2, axis=0) / n)
+
+    # Calculate the P_value
+    p_value = 2 * min(numpy.mean(t_sim <= t), numpy.mean(t_sim >= t))
+
+    if p_value < signif_lev:
+        print(
+            'Test statistic: {}, P-value: {} \nThe Null Hypothesis in Rejected: the model is not consistent with the '
+            'observations.'.format(
+                numpy.round(t, 4), p_value))
+    else:
+        print(
+            'Test statistic: {}, P-value: {} \nThe Null Hypothesis in Not Rejected: the model is consistent with the '
+            'observations.'.format(
+                numpy.round(t, 4), p_value))
+
+    if plot:
+        plt.figure(figsize=(12,6))
+        order = numpy.argsort(x_obs)
+
+        plt.subplot(1, 2, 1)
+        plt.plot(x_obs[order], y_mod[order],color="#4E84C4", label='Model')
+        plt.plot(x_obs[order], y_obs_smoothed[:,0][order],color="#D16103", label='Obs.')
+        plt.plot(x_obs[order], y_obs_smoothed[:, 0][order]+y_obs_smoothed[:, 1][order],'--',color="#D16103")
+        plt.plot(x_obs[order], y_obs_smoothed[:, 0][order]-y_obs_smoothed[:, 1][order],'--',color="#D16103")
+        plt.errorbar(x_obs[order], y_obs[order], yerr=y_obs_err[order], fmt='.k')
+        plt.scatter(x_obs[order], y_obs[order], s=2, color='black')
+        plt.legend()
+
+        plt.subplot(1, 2, 2)
+        s = sns.kdeplot(t_sim, fill=True, color="gray")
+        plt.vlines(t, ymin=0, ymax=s.dataLim.bounds[3], color="#D16103",linestyle='--', label='Test stat.')
+        plt.vlines(numpy.nanquantile(t_sim, q=signif_lev / 2), ymin=0, ymax=s.dataLim.bounds[3], color="#293352",
+                   linestyle='--', label='97.5%')
+        plt.vlines(numpy.nanquantile(t_sim, q=1 - (signif_lev / 2)), ymin=0, ymax=s.dataLim.bounds[3], color="#293352",
+                   linestyle='--', label='2.5%')
+        plt.legend()
+
+    return pd.DataFrame({'Test': t, 'Bootstrap': t_sim, 'P_value': p_value})
+
+
+
+
+###########################################  DENSITY  ##################################################
+###########################################  MODELS   ##################################################
+
+
+########################
+# CONTEST FOR OUTLIERS #
+########################
+
+
+def contest_outliers(mod, obs, K=1000, signif_lev=0.05, plot=False):
+
+    # Sample size
+    n = obs.shape[0]
+
+    # Transformation for scipy multivariate Kernel Density Estimation
+    if obs.ndim == 2:
+        mod = mod.T
+        obs = obs.T
+
+    # Estimate the model's density
+    g = stats.gaussian_kde(mod)
+
+    # Estimate the test statistic
+    t = -numpy.mean(g.logpdf(obs))
+
+    # Simulate K dataset and estimate their test statistics
+    t_sim = numpy.zeros((K))
+    for k in range(K):
+        sim = g.resample(n)
+        t_sim[k] = -numpy.mean(g.logpdf(sim))
+
+    # Calculate the P_value
+    p_value = 2 * min(numpy.mean(t_sim <= t), numpy.mean(t_sim >= t))
+
+    if p_value < signif_lev:
+        print(
+            'Test statistic: {}, P-value: {} \nThe Null Hypothesis in Rejected: the model is not consistent with the '
+            'observations.'.format(
+                numpy.round(t, 4), p_value))
+    else:
+        print(
+            'Test statistic: {}, P-value: {} \nThe Null Hypothesis in Not Rejected: the model is consistent with the '
+            'observations.'.format(
+                numpy.round(t, 4), p_value))
+
+    if plot:
+        if obs.ndim == 1:
+            plt.figure(figsize=(12, 6))
+            plt.subplot(1, 2, 1)
+            sns.kdeplot(x=mod, levels=[0.25,0.50,0.75], color="#4E84C4", linestyle='--', label='Model')
+            plt.plot(obs, -0.00005 * numpy.ones(obs.shape[0]), "|", color='black')
+            plt.legend()
+
+            plt.subplot(1, 2, 2)
+            s = sns.kdeplot(t_sim, fill=True, color="gray")
+            plt.vlines(t, ymin=0, ymax=s.dataLim.bounds[3], colors="#D16103", linestyle='--', label='Test stat.')
+            plt.vlines(numpy.nanquantile(t_sim, q=1 - (signif_lev / 2)), ymin=0, ymax=s.dataLim.bounds[3],
+                       colors="#293352", linestyle='--', label='97.5%')
+            plt.vlines(numpy.nanquantile(t_sim, q=signif_lev / 2), ymin=0, ymax=s.dataLim.bounds[3], colors="#293352",
+                       linestyle='--', label='2.5%')
+            plt.legend()
+
+
+        if obs.ndim == 2:
+            plt.figure(figsize=(12, 6))
+            plt.subplot(1, 2, 1)
+            sns.kdeplot(x=mod[0,:], y=mod[1,:], levels=[0.25,0.50,0.75], color="#4E84C4", linestyles='--',
+                        label='Model')
+            plt.scatter(x=obs[0,:], y=obs[1,:], s=2, color='black')
+            plt.legend()
+
+            plt.subplot(1, 2, 2)
+            s = sns.kdeplot(t_sim, fill=True, color="gray")
+            plt.vlines(t, ymin=0, ymax=s.dataLim.bounds[3], color="#D16103", linestyle='--', label='Test stat.')
+            plt.vlines(numpy.nanquantile(t_sim, q=1 - (signif_lev / 2)), ymin=0, ymax=s.dataLim.bounds[3],
+                       color="#293352", linestyle='--', label='97.5%')
+            plt.vlines(numpy.nanquantile(t_sim, q=signif_lev / 2), ymin=0, ymax=s.dataLim.bounds[3], color="#293352",
+                       linestyle='--', label='2.5%')
+            plt.legend()
+
+    return pd.DataFrame({'Test': t, 'Bootstrap': t_sim, 'P_value': p_value})
+
+
+
+##########################
+# CONTEST FOR DENSITIES #
+##########################
+
+def contest_dens(mod, obs, K=1000, signif_lev=0.05, plot=False):
+    # Sample size
+    n = obs.shape[0]
+
+    # Transformation for scipy multivariate Kernel Density Estimation
+    if obs.ndim == 2:
+        mod = mod.T
+        obs = obs.T
+
+    # Estimate the model's density
+    g = stats.gaussian_kde(mod)
+
+    # Estimate the observations' density
+    f = stats.gaussian_kde(obs)
+
+    # MCMC to estimate the test statistic
+    J = 1000
+    x_g = g.resample(J)
+    d_g = g.pdf(x_g)
+    d_f = f.pdf(x_g)
+
+    # Estimate the test statistics
+    t = sum(abs(d_f / d_g - 1)) / J
+
+    # Simulate K dataset and estimate their test statistics
+    t_sim = numpy.zeros((K))
+    for k in range(K):
+        sim = g.resample(n)
+        f_sim = stats.gaussian_kde(sim)
+        d_f_sim = f_sim.pdf(x_g)
+        t_sim[k] = sum(abs(d_f_sim / d_g - 1)) / J
+
+    # P-value
+    p_value = numpy.mean(t_sim >= t)
+
+    if p_value < signif_lev:
+        print(
+            'Test statistic: {}, P-value: {} \nThe Null hypothesis in Rejected: the model is not consistent with the '
+            'observations.'.format(
+                numpy.round(t, 4),  numpy.round(p_value,4)))
+    else:
+        print(
+            'Test statistic: {}, P-value: {} \nThe Null hypothesis in Not Rejected: the model is consistent with the '
+            'observations.'.format(
+                numpy.round(t, 4),  numpy.round(p_value,4)))
+
+    if plot:
+
+        if obs.ndim == 1:
+            plt.figure(figsize=(12, 6))
+            plt.subplot(1, 2, 1)
+            sns.kdeplot(x=mod, levels=[0.25,0.50,0.75], color="#4E84C4", linestyle='--', label='Model')
+            sns.kdeplot(x=obs, levels=[0.25,0.50,0.75], color="#D16103", label='Obs.')
+            plt.plot(obs, -0.00005 * numpy.ones(obs.shape[0]), "|", color='black')
+            plt.legend()
+
+
+            plt.subplot(1, 2, 2)
+            s = sns.kdeplot(t_sim, fill=True, color="gray")
+            plt.vlines(t, ymin=0, ymax=s.dataLim.bounds[3], colors="#D16103", linestyle='--', label='Test stat.')
+            plt.vlines(numpy.nanquantile(t_sim, q=1 - signif_lev), ymin=0, ymax=s.dataLim.bounds[3], colors="#293352",
+                       linestyle='--', label='95%')
+            plt.legend()
+
+
+        if obs.ndim == 2:
+            plt.figure(figsize=(12, 6))
+            plt.subplot(1, 2, 1)
+            sns.kdeplot(x=mod[0,:], y=mod[1,:], levels=[0.25,0.50,0.75], colors="#4E84C4", linestyles='--',
+                        label='Model')
+            sns.kdeplot(x=obs[0,:], y=obs[1,:], levels=[0.25,0.50,0.75], colors="#D16103", label='Obs.')
+            plt.scatter(x=obs[0,:], y=obs[1,:], s=2, color='black')
+            plt.legend()
+
+            plt.subplot(1, 2, 2)
+            s = sns.kdeplot(t_sim, fill=True, color="gray")
+            plt.vlines(t, ymin=0, ymax=s.dataLim.bounds[3], colors="#D16103",linestyle='--', label='Test stat.')
+            plt.vlines(numpy.nanquantile(t_sim, q=1 - signif_lev), ymin=0, ymax=s.dataLim.bounds[3], colors="#293352",
+                       linestyle='--', label='95%')
+            plt.legend()
+
+    return pd.DataFrame({'Test': t, 'Bootstrap': t_sim, 'P_value': p_value})
+
+
+
+if __name__ == '__main__':
     print('Welcome to ConTEST, check out the github page to learn more about it.')
```

### Comparing `ConsistencyTEST-0.0.1/src/ConsistencyTEST.egg-info/PKG-INFO` & `ConsistencyTEST-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,497 +1,481 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2043 6f6e  : 2.1..Name: Con
-00000020: 7369 7374 656e 6379 5445 5354 0d0a 5665  sistencyTEST..Ve
-00000030: 7273 696f 6e3a 2030 2e30 2e31 0d0a 5375  rsion: 0.0.1..Su
-00000040: 6d6d 6172 793a 2043 6f6e 7369 7374 656e  mmary: Consisten
-00000050: 6379 2074 6573 740d 0a48 6f6d 652d 7061  cy test..Home-pa
-00000060: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
-00000070: 7562 2e63 6f6d 2f46 696f 7265 6e53 542f  ub.com/FiorenST/
-00000080: 436f 6e54 4553 540d 0a41 7574 686f 723a  ConTEST..Author:
-00000090: 2046 696f 7265 6e7a 6f20 5374 6f70 7061   Fiorenzo Stoppa
-000000a0: 0d0a 4175 7468 6f72 2d65 6d61 696c 3a20  ..Author-email: 
-000000b0: 662e 7374 6f70 7061 4061 7374 726f 2e72  f.stoppa@astro.r
-000000c0: 752e 6e6c 0d0a 5072 6f6a 6563 742d 5552  u.nl..Project-UR
-000000d0: 4c3a 2042 7567 2054 7261 636b 6572 2c20  L: Bug Tracker, 
-000000e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000000f0: 6f6d 2f46 696f 7265 6e53 542f 436f 6e54  om/FiorenST/ConT
-00000100: 4553 542f 6973 7375 6573 0d0a 436c 6173  EST/issues..Clas
-00000110: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000120: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000130: 5079 7468 6f6e 203a 3a20 330d 0a43 6c61  Python :: 3..Cla
-00000140: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
-00000150: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000160: 203a 3a20 4170 6163 6865 2053 6f66 7477   :: Apache Softw
-00000170: 6172 6520 4c69 6365 6e73 650d 0a43 6c61  are License..Cla
-00000180: 7373 6966 6965 723a 204f 7065 7261 7469  ssifier: Operati
-00000190: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-000001a0: 496e 6465 7065 6e64 656e 740d 0a52 6571  Independent..Req
-000001b0: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
-000001c0: 332e 360d 0a44 6573 6372 6970 7469 6f6e  3.6..Description
-000001d0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
-000001e0: 6578 742f 6d61 726b 646f 776e 0d0a 4c69  ext/markdown..Li
-000001f0: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-00000200: 4e53 450d 0a0d 0a3c 696d 6720 7372 633d  NSE....<img src=
-00000210: 6874 7470 733a 2f2f 7365 652e 666f 6e74  https://see.font
-00000220: 696d 672e 636f 6d2f 6170 692f 7265 6e64  img.com/api/rend
-00000230: 6572 666f 6e74 342f 4b70 4170 2f65 794a  erfont4/KpAp/eyJ
-00000240: 7949 6a6f 695a 6e4d 694c 434a 6f49 6a6f  yIjoiZnMiLCJoIjo
-00000250: 784d 7a41 7349 6e63 694f 6a45 774d 4441  xMzAsInciOjEwMDA
-00000260: 7349 6d5a 7a49 6a6f 784d 7a41 7349 6d5a  sImZzIjoxMzAsImZ
-00000270: 6e59 7949 3649 694e 4752 4468 444d 444d  nYyI6IiNGRDhDMDM
-00000280: 694c 434a 695a 324d 694f 6949 6a4d 4459  iLCJiZ2MiOiIjMDY
-00000290: 774e 5441 3149 6977 6964 4349 364d 5830  wNTA1IiwidCI6MX0
-000002a0: 2f51 3239 7556 4556 5456 412f 6b67 2d73  /Q29uVEVTVA/kg-s
-000002b0: 6563 6f6e 642d 6368 616e 6365 732d 736b  econd-chances-sk
-000002c0: 6574 6368 2e70 6e67 2077 6964 7468 3d35  etch.png width=5
-000002d0: 3025 2068 6569 6768 743d 3530 253e 0d0a  0% height=50%>..
-000002e0: 0d0a 0d0a 3c21 2d2d 0d0a 5b21 5b44 4f49  ....<!--..[![DOI
-000002f0: 5d28 6874 7470 733a 2f2f 7a65 6e6f 646f  ](https://zenodo
-00000300: 2e6f 7267 2f62 6164 6765 2f34 3430 3835  .org/badge/44085
-00000310: 3134 3437 2e73 7667 295d 2868 7474 7073  1447.svg)](https
-00000320: 3a2f 2f7a 656e 6f64 6f2e 6f72 672f 6261  ://zenodo.org/ba
-00000330: 6467 652f 6c61 7465 7374 646f 692f 3434  dge/latestdoi/44
-00000340: 3038 3531 3434 3729 200d 0a3c 6120 6872  0851447) ..<a hr
-00000350: 6566 3d22 6874 7470 733a 2f2f 6173 636c  ef="https://ascl
-00000360: 2e6e 6574 2f32 3230 332e 3031 3422 3e3c  .net/2203.014"><
-00000370: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000380: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000390: 6261 6467 652f 6173 636c 2d32 3230 332e  badge/ascl-2203.
-000003a0: 3031 342d 626c 7565 2e73 7667 3f63 6f6c  014-blue.svg?col
-000003b0: 6f72 423d 3236 3232 3535 2220 616c 743d  orB=262255" alt=
-000003c0: 2261 7363 6c3a 3232 3033 2e30 3134 2220  "ascl:2203.014" 
-000003d0: 2f3e 3c2f 613e 0d0a 0d0a 3c69 6d67 2073  /></a>....<img s
-000003e0: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
-000003f0: 7562 2e63 6f6d 2f46 696f 7265 6e53 742f  ub.com/FiorenSt/
-00000400: 4175 746f 536f 7572 6365 4944 2d4c 6967  AutoSourceID-Lig
-00000410: 6874 2f62 6c6f 622f 6d61 696e 2f50 6c6f  ht/blob/main/Plo
-00000420: 7473 2f4f 7074 6963 616c 496d 6167 6550  ts/OpticalImageP
-00000430: 6174 6368 2e70 6e67 2022 2077 6964 7468  atch.png " width
-00000440: 3d35 3025 2068 6569 6768 743d 3530 253e  =50% height=50%>
-00000450: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000460: 2f2f 6769 7468 7562 2e63 6f6d 2f46 696f  //github.com/Fio
-00000470: 7265 6e53 742f 4175 746f 536f 7572 6365  renSt/AutoSource
-00000480: 4944 2d4c 6967 6874 2f62 6c6f 622f 6d61  ID-Light/blob/ma
-00000490: 696e 2f50 6c6f 7473 2f4c 6f47 4f6e 4f70  in/Plots/LoGOnOp
-000004a0: 7469 6361 6c2e 706e 6720 2220 7769 6474  tical.png " widt
-000004b0: 683d 3530 2520 6865 6967 6874 3d35 3025  h=50% height=50%
-000004c0: 3e20 0d0a 0d0a 2d2d 3e0d 0a0d 0a0d 0a23  > ....-->......#
-000004d0: 2044 6573 6372 6970 7469 6f6e 0d0a 0d0a   Description....
-000004e0: 436f 6e54 4553 5420 6973 2061 2073 7461  ConTEST is a sta
-000004f0: 7469 7374 6963 616c 2074 6573 7420 666f  tistical test fo
-00000500: 7220 6173 7365 7373 696e 6720 7468 6520  r assessing the 
-00000510: 636f 6e73 6973 7465 6e63 7920 6265 7477  consistency betw
-00000520: 6565 6e20 6f62 7365 7276 6174 696f 6e73  een observations
-00000530: 2061 6e64 2061 7374 726f 7068 7973 6963   and astrophysic
-00000540: 616c 206d 6f64 656c 732e 0d0a 4974 2075  al models...It u
-00000550: 7365 7320 6120 636f 6d62 696e 6174 696f  ses a combinatio
-00000560: 6e20 6f66 206e 6f6e 2d70 6172 616d 6574  n of non-paramet
-00000570: 7269 6320 6d65 7468 6f64 7320 616e 6420  ric methods and 
-00000580: 6469 7374 616e 6365 206d 6561 7375 7265  distance measure
-00000590: 7320 746f 206f 6274 6169 6e20 6120 7465  s to obtain a te
-000005a0: 7374 0d0a 7374 6174 6973 7469 6320 7468  st..statistic th
-000005b0: 6174 2065 7661 6c75 6174 6573 2074 6865  at evaluates the
-000005c0: 2063 6c6f 7365 6e65 7373 206f 6620 7468   closeness of th
-000005d0: 6520 6173 7472 6f70 6879 7369 6361 6c20  e astrophysical 
-000005e0: 6d6f 6465 6c20 746f 2074 6865 206f 6273  model to the obs
-000005f0: 6572 7661 7469 6f6e 733b 2068 7970 6f74  ervations; hypot
-00000600: 6865 7369 7320 7465 7374 696e 6720 6973  hesis testing is
-00000610: 2074 6865 6e20 7065 7266 6f72 6d65 6420   then performed 
-00000620: 7573 696e 6720 626f 6f74 7374 7261 702e  using bootstrap.
-00000630: 0d0a 200d 0a0d 0a3c 696d 6720 7372 633d  .. ....<img src=
-00000640: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000650: 6f6d 2f46 696f 7265 6e53 742f 436f 6e54  om/FiorenSt/ConT
-00000660: 4553 542f 626c 6f62 2f6d 6169 6e2f 696d  EST/blob/main/im
-00000670: 672f 6c6f 676f 5f63 6f6e 7465 7374 5f62  g/logo_contest_b
-00000680: 6b67 2e70 6e67 2077 6964 7468 3d31 3525  kg.png width=15%
-00000690: 2068 6569 6768 743d 3135 253e 0d0a 0d0a   height=15%>....
-000006a0: 0d0a 2323 2054 6162 6c65 206f 6620 436f  ..## Table of Co
-000006b0: 6e74 656e 7473 200d 0a2d 205b 5374 6570  ntents ..- [Step
-000006c0: 2d62 792d 7374 6570 2073 6574 7570 5d28  -by-step setup](
-000006d0: 2373 7465 702d 6279 2d73 7465 702d 7365  #step-by-step-se
-000006e0: 7475 7029 0d0a 2d20 5b54 7574 6f72 6961  tup)..- [Tutoria
-000006f0: 6c5d 2823 7475 746f 7269 616c 290d 0a0d  l](#tutorial)...
-00000700: 0a0d 0a23 2053 7465 702d 6279 2d73 7465  ...# Step-by-ste
-00000710: 7020 7365 7475 700d 0a0d 0a5f 466f 6c6c  p setup...._Foll
-00000720: 6f77 2074 6865 2069 6e73 7472 7563 7469  ow the instructi
-00000730: 6f6e 7320 6265 6c6f 7720 746f 2069 6e73  ons below to ins
-00000740: 7461 6c6c 2061 6e64 2073 7461 7274 2075  tall and start u
-00000750: 7369 6e67 2043 6f6e 5445 5354 2069 6e20  sing ConTEST in 
-00000760: 5079 7468 6f6e 2e5f 0d0a 0d0a 312e 2049  Python._....1. I
-00000770: 6e73 7461 6c6c 2043 6f6e 5445 5354 3a0d  nstall ConTEST:.
-00000780: 0a20 2020 6060 6073 680d 0a20 2020 7069  .   ```sh..   pi
-00000790: 7020 696e 7461 6c6c 2043 6f6e 5445 5354  p intall ConTEST
-000007a0: 0d0a 2020 2060 6060 0d0a 2020 206f 7220  ..   ```..   or 
-000007b0: 6769 7420 636c 6f6e 6520 7468 6520 7265  git clone the re
-000007c0: 706f 7369 746f 7279 3a0d 0a20 2020 2060  pository:..    `
-000007d0: 6060 7368 0d0a 2020 2067 6974 2063 6c6f  ``sh..   git clo
-000007e0: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
-000007f0: 622e 636f 6d2f 4669 6f72 656e 5374 2f43  b.com/FiorenSt/C
-00000800: 6f6e 5445 5354 2e67 6974 0d0a 2020 2060  onTEST.git..   `
-00000810: 6060 0d0a 2020 200d 0a0d 0a20 3c62 722f  ``..   .... <br/
-00000820: 3e0d 0a0d 0a32 2e20 496e 7374 616c 6c20  >....2. Install 
-00000830: 7468 6520 7374 6174 6973 7469 6361 6c20  the statistical 
-00000840: 736f 6674 7761 7265 205b 525d 2868 7474  software [R](htt
-00000850: 7073 3a2f 2f77 7777 2e72 2d70 726f 6a65  ps://www.r-proje
-00000860: 6374 2e6f 7267 2f29 2e20 5220 6973 206e  ct.org/). R is n
-00000870: 6565 6465 6420 746f 2072 756e 2073 6f6d  eeded to run som
-00000880: 6520 696e 7465 726e 616c 2066 756e 6374  e internal funct
-00000890: 696f 6e73 206f 6620 436f 6e54 4553 542e  ions of ConTEST.
-000008a0: 0d0a 3c62 722f 3e0d 0a0d 0a33 2e20 546f  ..<br/>....3. To
-000008b0: 2065 6e73 7572 6520 7468 6174 2050 7974   ensure that Pyt
-000008c0: 686f 6e20 6361 6e20 6163 6365 7373 2052  hon can access R
-000008d0: 2773 206c 6962 7261 7269 6573 2c20 7275  's libraries, ru
-000008e0: 6e20 7468 6520 7468 7265 6520 6c69 6e65  n the three line
-000008f0: 7320 6265 6c6f 7720 696e 2050 7974 686f  s below in Pytho
-00000900: 6e20 286f 6620 636f 7572 7365 2c20 6d6f  n (of course, mo
-00000910: 6469 6679 2074 6f20 6d61 7463 6820 796f  dify to match yo
-00000920: 7572 2066 6f6c 6465 7273 293a 0d0a 0d0a  ur folders):....
-00000930: 2020 2060 6060 7368 0d0a 2020 2020 696d     ```sh..    im
-00000940: 706f 7274 206f 730d 0a20 2020 206f 732e  port os..    os.
-00000950: 656e 7669 726f 6e5b 2752 5f48 4f4d 4527  environ['R_HOME'
-00000960: 5d20 3d20 277e 2f50 726f 6772 616d 2046  ] = '~/Program F
-00000970: 696c 6573 2f52 2f52 2d34 2e30 2e32 2720  iles/R/R-4.0.2' 
-00000980: 2023 2d3e 2059 6f75 7220 696e 7374 616c   #-> Your instal
-00000990: 6c65 6420 5220 666f 6c64 6572 0d0a 2020  led R folder..  
-000009a0: 2020 6f73 2e65 6e76 6972 6f6e 5b27 525f    os.environ['R_
-000009b0: 5553 4552 275d 203d 2027 7e2f 4d69 6e69  USER'] = '~/Mini
-000009c0: 636f 6e64 6133 2f65 6e76 732f 436f 6e73  conda3/envs/Cons
-000009d0: 6973 7465 6e63 7954 6573 742f 6c69 622f  istencyTest/lib/
-000009e0: 7369 7465 2d70 6163 6b61 6765 732f 2720  site-packages/' 
-000009f0: 2023 2d3e 2059 6f75 7220 7079 7468 6f6e   #-> Your python
-00000a00: 2065 6e76 6972 6f6e 6d65 6e74 0d0a 2020   environment..  
-00000a10: 2020 6f73 2e65 6e76 6972 6f6e 5b27 525f    os.environ['R_
-00000a20: 4c49 4253 5f55 5345 5227 5d20 3d20 227e  LIBS_USER'] = "~
-00000a30: 2f50 726f 6772 616d 2046 696c 6573 2f52  /Program Files/R
-00000a40: 2f52 2d34 2e30 2e32 2f6c 6962 7261 7279  /R-4.0.2/library
-00000a50: 2f22 2020 232d 3e20 596f 7572 2052 2070  /"  #-> Your R p
-00000a60: 6163 6b61 6765 7320 6c69 6272 6172 790d  ackages library.
-00000a70: 0a20 2020 6060 600d 0a3c 6272 2f3e 0d0a  .   ```..<br/>..
-00000a80: 0d0a 0d0a 342e 2049 6e73 7461 6c6c 2050  ....4. Install P
-00000a90: 7974 686f 6e20 6465 7065 6e64 656e 6369  ython dependenci
-00000aa0: 6573 2028 7270 7932 206e 6565 6473 2052  es (rpy2 needs R
-00000ab0: 2061 6c72 6561 6479 2069 6e73 7461 6c6c   already install
-00000ac0: 6564 293a 0d0a 2020 2060 6060 7368 0d0a  ed):..   ```sh..
-00000ad0: 2020 2070 6970 2069 6e74 616c 6c20 6d61     pip intall ma
-00000ae0: 7470 6c6f 746c 6962 0d0a 2020 2070 6970  tplotlib..   pip
-00000af0: 2069 6e74 616c 6c20 6e75 6d70 790d 0a20   intall numpy.. 
-00000b00: 2020 7069 7020 696e 7461 6c6c 2070 616e    pip intall pan
-00000b10: 6461 730d 0a20 2020 7069 7020 696e 7461  das..   pip inta
-00000b20: 6c6c 2073 6369 7079 0d0a 2020 2070 6970  ll scipy..   pip
-00000b30: 2069 6e74 616c 6c20 7365 6162 6f72 6e0d   intall seaborn.
-00000b40: 0a20 2020 7069 7020 696e 7461 6c6c 2072  .   pip intall r
-00000b50: 7079 320d 0a20 2020 6060 600d 0a20 3c62  py2..   ```.. <b
-00000b60: 722f 3e0d 0a0d 0a0d 0a35 2e20 4966 2074  r/>......5. If t
-00000b70: 6869 7320 6973 2074 6865 2066 6972 7374  his is the first
-00000b80: 2074 696d 6520 796f 7520 7573 6520 436f   time you use Co
-00000b90: 6e54 4553 542c 2079 6f75 206e 6565 6420  nTEST, you need 
-00000ba0: 746f 2069 6e73 7461 6c6c 2074 6865 2052  to install the R
-00000bb0: 2070 6163 6b61 6765 2075 7365 6420 696e   package used in
-00000bc0: 2053 6d6f 6f74 6865 6420 436f 6e54 4553   Smoothed ConTES
-00000bd0: 542e 2049 6e20 5079 7468 6f6e 2c20 7369  T. In Python, si
-00000be0: 6d70 6c79 2072 756e 3a0d 0a0d 0a20 2020  mply run:....   
-00000bf0: 6060 6073 680d 0a20 2020 2064 6566 2069  ```sh..    def i
-00000c00: 6e73 7461 6c6c 5f52 5f66 756e 6374 696f  nstall_R_functio
-00000c10: 6e73 2870 6163 6b6e 616d 6573 3d28 276e  ns(packnames=('n
-00000c20: 7027 2929 3a0d 0a20 2020 2020 2020 2023  p')):..        #
-00000c30: 2069 6d70 6f72 7420 5227 7320 7574 696c   import R's util
-00000c40: 6974 7920 7061 636b 6167 650d 0a20 2020  ity package..   
-00000c50: 2020 2020 2075 7469 6c73 203d 2072 7061       utils = rpa
-00000c60: 636b 6167 6573 2e69 6d70 6f72 7472 2827  ckages.importr('
-00000c70: 7574 696c 7327 290d 0a20 2020 2020 2020  utils')..       
-00000c80: 2023 2073 656c 6563 7420 6120 6d69 7272   # select a mirr
-00000c90: 6f72 2066 6f72 2052 2070 6163 6b61 6765  or for R package
-00000ca0: 730d 0a20 2020 2020 2020 2075 7469 6c73  s..        utils
-00000cb0: 2e63 686f 6f73 6543 5241 4e6d 6972 726f  .chooseCRANmirro
-00000cc0: 7228 696e 643d 3129 2020 2320 7365 6c65  r(ind=1)  # sele
-00000cd0: 6374 2074 6865 2066 6972 7374 206d 6972  ct the first mir
-00000ce0: 726f 7220 696e 2074 6865 206c 6973 740d  ror in the list.
-00000cf0: 0a20 2020 2020 2020 2023 2052 2070 6163  .        # R pac
-00000d00: 6b61 6765 2069 6e73 7461 6c6c 0d0a 2020  kage install..  
-00000d10: 2020 2020 2020 7574 696c 732e 696e 7374        utils.inst
-00000d20: 616c 6c5f 7061 636b 6167 6573 2870 6163  all_packages(pac
-00000d30: 6b6e 616d 6573 290d 0a20 2020 200d 0a20  knames)..    .. 
-00000d40: 2020 2069 6e73 7461 6c6c 5f52 5f66 756e     install_R_fun
-00000d50: 6374 696f 6e73 2829 0d0a 2020 2060 6060  ctions()..   ```
-00000d60: 0d0a 0d0a 332e 2055 7365 2043 6f6e 5445  ....3. Use ConTE
-00000d70: 5354 2069 6e20 5079 7468 6f6e 2120 466f  ST in Python! Fo
-00000d80: 6c6c 6f77 2074 6865 2074 7574 6f72 6961  llow the tutoria
-00000d90: 6c20 6265 6c6f 7720 666f 7220 6d6f 7265  l below for more
-00000da0: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
-00000db0: 7574 2074 6865 2069 6e64 6976 6964 7561  ut the individua
-00000dc0: 6c20 6675 6e63 7469 6f6e 732e 0d0a 0d0a  l functions.....
-00000dd0: 3c62 722f 3e0d 0a0d 0a0d 0a3c 696d 6720  <br/>......<img 
-00000de0: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
-00000df0: 6875 622e 636f 6d2f 4669 6f72 656e 5374  hub.com/FiorenSt
-00000e00: 2f43 6f6e 5445 5354 2f62 6c6f 622f 6d61  /ConTEST/blob/ma
-00000e10: 696e 2f69 6d67 2f4d 656d 6543 6f6e 5445  in/img/MemeConTE
-00000e20: 5354 2e70 6e67 2022 2077 6964 7468 3d38  ST.png " width=8
-00000e30: 3025 2068 6569 6768 743d 3830 253e 0d0a  0% height=80%>..
-00000e40: 0d0a 3c62 722f 3e0d 0a0d 0a0d 0a0d 0a0d  ..<br/>.........
-00000e50: 0a23 2044 6570 656e 6465 6e63 6965 733a  .# Dependencies:
-00000e60: 0d0a 0d0a 5468 6520 666f 6c6c 6f77 696e  ....The followin
-00000e70: 6720 636f 6d62 696e 6174 696f 6e20 6f66  g combination of
-00000e80: 2070 6163 6b61 6765 2076 6572 7369 6f6e   package version
-00000e90: 7320 776f 726b 7320 6f6e 206d 6f73 7420  s works on most 
-00000ea0: 4c69 6e75 7820 616e 6420 5769 6e64 6f77  Linux and Window
-00000eb0: 7320 636f 6d70 7574 6572 732c 2068 6f77  s computers, how
-00000ec0: 6576 6572 206f 7468 6572 2070 6163 6b61  ever other packa
-00000ed0: 6765 2076 6572 7369 6f6e 7320 6d61 7920  ge versions may 
-00000ee0: 616c 736f 0d0a 776f 726b 2e20 4966 2061  also..work. If a
-00000ef0: 2070 726f 626c 656d 2077 6974 6820 7468   problem with th
-00000f00: 6520 636f 6d62 696e 6174 696f 6e20 6f66  e combination of
-00000f10: 2070 6163 6b61 6765 7320 6f63 6375 7273   packages occurs
-00000f20: 2c20 7261 6973 6520 616e 2069 7373 7565  , raise an issue
-00000f30: 2c20 616e 6420 7765 2077 696c 6c20 6865  , and we will he
-00000f40: 6c70 2079 6f75 2073 6f6c 7665 2069 742e  lp you solve it.
-00000f50: 0d0a 0d0a 0d0a 2323 2320 5079 7468 6f6e  ......### Python
-00000f60: 2033 2028 6f72 2073 7570 6572 696f 7229   3 (or superior)
-00000f70: 0d0a 2a20 4e75 6d70 7920 312e 3231 2e36  ..* Numpy 1.21.6
-00000f80: 0d0a 2a20 5061 6e64 6173 2031 2e34 2e32  ..* Pandas 1.4.2
-00000f90: 0d0a 2a20 5363 6970 7920 312e 372e 310d  ..* Scipy 1.7.1.
-00000fa0: 0a2a 204d 6174 706c 6f74 6c69 6220 332e  .* Matplotlib 3.
-00000fb0: 332e 340d 0a2a 2053 6561 626f 726e 2030  3.4..* Seaborn 0
-00000fc0: 2e31 312e 320d 0a2a 2052 7079 3220 332e  .11.2..* Rpy2 3.
-00000fd0: 352e 3220 2846 6f72 2052 2061 6e64 2050  5.2 (For R and P
-00000fe0: 7974 686f 6e20 696e 7465 7261 6374 696f  ython interactio
-00000ff0: 6e29 0d0a 0d0a 2323 2320 5220 332e 362e  n)....### R 3.6.
-00001000: 3020 286f 7220 7375 7065 7269 6f72 290d  0 (or superior).
-00001010: 0a2a 204e 7020 302e 3630 0d0a 0d0a 0d0a  .* Np 0.60......
-00001020: 0d0a 2320 5475 746f 7269 616c 0d0a 0d0a  ..# Tutorial....
-00001030: 436f 6e54 4553 5420 6361 6e20 6265 2061  ConTEST can be a
-00001040: 7070 6c69 6564 2069 6e20 6469 6666 6572  pplied in differ
-00001050: 656e 7420 6361 7365 2073 6365 6e61 7269  ent case scenari
-00001060: 6f73 2064 6570 656e 6469 6e67 206f 6e20  os depending on 
-00001070: 7468 6520 6e61 7475 7265 206f 6620 7468  the nature of th
-00001080: 6520 6d6f 6465 6c20 6265 696e 6720 7465  e model being te
-00001090: 7374 6564 2e20 0d0a 3c62 722f 3e0d 0a46  sted. ..<br/>..F
-000010a0: 6f72 206d 6f72 6520 6465 7461 696c 7320  or more details 
-000010b0: 6368 6563 6b20 6f75 7420 7468 6520 7061  check out the pa
-000010c0: 7065 723a 205f 5374 6f70 7061 2065 7420  per: _Stoppa et 
-000010d0: 616c 2e2c 2069 6e20 7072 6570 6172 6174  al., in preparat
-000010e0: 696f 6e5f 0d0a 0d0a 5468 6572 6520 6172  ion_....There ar
-000010f0: 6520 3420 6675 6e64 616d 656e 7461 6c20  e 4 fundamental 
-00001100: 6675 6e63 7469 6f6e 7320 696e 2043 6f6e  functions in Con
-00001110: 5445 5354 3a0d 0a0d 0a2d 2043 6f6e 5445  TEST:....- ConTE
-00001120: 5354 2066 6f72 2072 6567 7265 7373 696f  ST for regressio
-00001130: 6e3a 2054 6573 7420 7468 6520 636f 6e73  n: Test the cons
-00001140: 6973 7465 6e63 7920 6f66 2061 206d 6f64  istency of a mod
-00001150: 656c 2077 6974 6820 7265 7370 6563 7420  el with respect 
-00001160: 746f 2061 6e20 6f62 7365 7276 6564 2064  to an observed d
-00001170: 6174 6173 6574 2061 6e64 2074 6865 6972  ataset and their
-00001180: 2075 6e63 6572 7461 696e 7469 6573 0d0a   uncertainties..
-00001190: 2d20 536d 6f6f 7468 6564 2043 6f6e 5445  - Smoothed ConTE
-000011a0: 5354 2066 6f72 2072 6567 7265 7373 696f  ST for regressio
-000011b0: 6e3a 2054 6573 7420 7468 6520 636f 6e73  n: Test the cons
-000011c0: 6973 7465 6e63 7920 6f66 2061 206d 6f64  istency of a mod
-000011d0: 656c 2077 6974 6820 7265 7370 6563 7420  el with respect 
-000011e0: 746f 2061 6e20 6f62 7365 7276 6564 2064  to an observed d
-000011f0: 6174 6173 6574 2061 6e64 200d 0a20 2074  ataset and ..  t
-00001200: 6865 6972 2075 6e63 6572 7461 696e 7469  heir uncertainti
-00001210: 6573 0d0a 2d20 436f 6e54 4553 5420 666f  es..- ConTEST fo
-00001220: 7220 6f75 746c 6965 7273 3a20 5465 7374  r outliers: Test
-00001230: 2069 6620 616e 206f 6273 6572 7665 6420   if an observed 
-00001240: 7361 6d70 6c65 2069 7320 6c69 6b65 6c79  sample is likely
-00001250: 2074 6f20 636f 6d65 2066 726f 6d20 6120   to come from a 
-00001260: 6465 6e73 6974 7920 6d6f 6465 6c20 286f  density model (o
-00001270: 7220 6120 7369 6d75 6c61 7465 6420 6461  r a simulated da
-00001280: 7461 7365 7429 0d0a 2d20 436f 6e54 4553  taset)..- ConTES
-00001290: 5420 666f 7220 6465 6e73 6974 6965 733a  T for densities:
-000012a0: 2054 6573 7420 7468 6520 636f 6e73 6973   Test the consis
-000012b0: 7465 6e63 7920 6f66 2061 2064 656e 7369  tency of a densi
-000012c0: 7479 206d 6f64 656c 2028 6f72 2061 2073  ty model (or a s
-000012d0: 696d 756c 6174 6564 2064 6174 6173 6574  imulated dataset
-000012e0: 2920 7769 7468 2072 6573 7065 6374 2074  ) with respect t
-000012f0: 6f20 616e 206f 6273 6572 7665 6420 0d0a  o an observed ..
-00001300: 2020 6461 7461 7365 7420 0d0a 0d0a 0d0a    dataset ......
-00001310: 2323 2320 496e 7472 6f20 7363 7269 7074  ### Intro script
-00001320: 200d 0a0d 0a20 2020 6060 6073 680d 0a20   ....   ```sh.. 
-00001330: 2020 2023 2065 6e73 7572 6520 7468 6174     # ensure that
-00001340: 2050 7974 686f 6e20 6361 6e20 6163 6365   Python can acce
-00001350: 7373 2052 0d0a 2020 2020 696d 706f 7274  ss R..    import
-00001360: 206f 730d 0a20 2020 206f 732e 656e 7669   os..    os.envi
-00001370: 726f 6e5b 2752 5f48 4f4d 4527 5d20 3d20  ron['R_HOME'] = 
-00001380: 277e 2f50 726f 6772 616d 2046 696c 6573  '~/Program Files
-00001390: 2f52 2f52 2d34 2e30 2e32 2720 2023 2d3e  /R/R-4.0.2'  #->
-000013a0: 2059 6f75 7220 696e 7374 616c 6c65 6420   Your installed 
-000013b0: 5220 666f 6c64 6572 0d0a 2020 2020 6f73  R folder..    os
-000013c0: 2e65 6e76 6972 6f6e 5b27 525f 5553 4552  .environ['R_USER
-000013d0: 275d 203d 2027 7e2f 4d69 6e69 636f 6e64  '] = '~/Minicond
-000013e0: 6133 2f65 6e76 732f 436f 6e73 6973 7465  a3/envs/Consiste
-000013f0: 6e63 7954 6573 742f 6c69 622f 7369 7465  ncyTest/lib/site
-00001400: 2d70 6163 6b61 6765 732f 2720 2023 2d3e  -packages/'  #->
-00001410: 2059 6f75 7220 7079 7468 6f6e 2065 6e76   Your python env
-00001420: 6972 6f6e 6d65 6e74 0d0a 2020 2020 6f73  ironment..    os
-00001430: 2e65 6e76 6972 6f6e 5b27 525f 4c49 4253  .environ['R_LIBS
-00001440: 5f55 5345 5227 5d20 3d20 227e 2f50 726f  _USER'] = "~/Pro
-00001450: 6772 616d 2046 696c 6573 2f52 2f52 2d34  gram Files/R/R-4
-00001460: 2e30 2e32 2f6c 6962 7261 7279 2f22 2020  .0.2/library/"  
-00001470: 232d 3e20 596f 7572 2052 2070 6163 6b61  #-> Your R packa
-00001480: 6765 7320 6c69 6272 6172 790d 0a20 2020  ges library..   
-00001490: 200d 0a20 2020 2023 206c 6f61 6420 636f   ..    # load co
-000014a0: 6e74 6573 7420 6675 6e63 7469 6f6e 730d  ntest functions.
-000014b0: 0a20 2020 2066 726f 6d20 436f 6e54 4553  .    from ConTES
-000014c0: 542e 434f 4e54 4553 5420 696d 706f 7274  T.CONTEST import
-000014d0: 2063 6f6e 7465 7374 5f72 6567 2c20 736d   contest_reg, sm
-000014e0: 6f6f 7468 6564 5f63 6f6e 7465 7374 5f72  oothed_contest_r
-000014f0: 6567 2c20 636f 6e74 6573 745f 6f75 746c  eg, contest_outl
-00001500: 6965 7273 2c20 636f 6e74 6573 745f 6465  iers, contest_de
-00001510: 6e73 0d0a 2020 2060 6060 0d0a 0d0a 0d0a  ns..   ```......
-00001520: 2323 2052 6567 7265 7373 696f 6e20 6d6f  ## Regression mo
-00001530: 6465 6c73 0d0a 0d0a 4372 6561 7465 2073  dels....Create s
-00001540: 796e 7468 6574 6963 206d 6f64 656c 2c20  ynthetic model, 
-00001550: 6f62 7365 7276 6174 696f 6e73 2c20 616e  observations, an
-00001560: 6420 756e 6365 7274 6169 6e74 6965 7320  d uncertainties 
-00001570: 746f 2074 6573 7420 7468 6520 6675 6e63  to test the func
-00001580: 7469 6f6e 733a 0d0a 0d0a 2020 2060 6060  tions:....   ```
-00001590: 7368 0d0a 2020 2023 2072 616e 646f 6d20  sh..   # random 
-000015a0: 7361 6d70 6c65 200d 0a20 2020 6e3d 3130  sample ..   n=10
-000015b0: 300d 0a20 2020 7820 3d20 6e70 2e72 616e  0..   x = np.ran
-000015c0: 646f 6d2e 7261 6e64 286e 290d 0a20 2020  dom.rand(n)..   
-000015d0: 0d0a 2020 2023 2073 796e 7468 6574 6963  ..   # synthetic
-000015e0: 206d 6f64 656c 200d 0a20 2020 6265 7461   model ..   beta
-000015f0: 3120 3d20 2d30 2e33 0d0a 2020 2062 6574  1 = -0.3..   bet
-00001600: 6132 203d 2038 0d0a 2020 206d 203d 2032  a2 = 8..   m = 2
-00001610: 0d0a 2020 206d 6f64 656c 203d 206e 702e  ..   model = np.
-00001620: 6578 7028 6265 7461 312a 7829 2a6e 702e  exp(beta1*x)*np.
-00001630: 7369 6e28 6265 7461 322a 7829 202b 206d  sin(beta2*x) + m
-00001640: 0d0a 2020 200d 0a20 2020 2320 6572 726f  ..   ..   # erro
-00001650: 7220 6675 6e63 7469 6f6e 2028 4e6f 7420  r function (Not 
-00001660: 6b6e 6f77 6e20 696e 2072 6561 6c20 7363  known in real sc
-00001670: 656e 6172 696f 7329 0d0a 2020 2065 7272  enarios)..   err
-00001680: 5f6d 6f64 656c 203d 206d 6f64 656c 202a  _model = model *
-00001690: 202e 3035 0d0a 2020 200d 0a20 2020 2320   .05..   ..   # 
-000016a0: 7361 6d70 6c65 206f 6273 6572 7661 7469  sample observati
-000016b0: 6f6e 7320 6672 6f6d 2074 6865 206d 6f64  ons from the mod
-000016c0: 656c 2077 6974 6820 7468 6520 636f 7272  el with the corr
-000016d0: 6563 7420 756e 6365 7274 6169 6e74 6965  ect uncertaintie
-000016e0: 730d 0a20 2020 6f62 7320 3d20 6e70 2e7a  s..   obs = np.z
-000016f0: 6572 6f73 284e 290d 0a20 2020 2020 2066  eros(N)..      f
-00001700: 6f72 2069 2069 6e20 7261 6e67 6528 4e29  or i in range(N)
-00001710: 3a0d 0a20 2020 2020 6f62 735b 695d 203d  :..     obs[i] =
-00001720: 206d 6f64 656c 5b69 5d20 2b20 7374 6174   model[i] + stat
-00001730: 732e 6d75 6c74 6976 6172 6961 7465 5f6e  s.multivariate_n
-00001740: 6f72 6d61 6c2e 7276 7328 6d65 616e 3d30  ormal.rvs(mean=0
-00001750: 2c20 636f 763d 2865 7272 5f6d 6f64 656c  , cov=(err_model
-00001760: 5b69 5d29 2a2a 322c 7369 7a65 3d31 290d  [i])**2,size=1).
-00001770: 0a20 2020 0d0a 2020 2023 2061 7373 6967  .   ..   # assig
-00001780: 6e20 636f 7272 6563 7420 756e 6365 7274  n correct uncert
-00001790: 6169 6e74 6965 7320 746f 2074 6865 206f  ainties to the o
-000017a0: 6273 6572 7661 7469 6f6e 730d 0a20 2020  bservations..   
-000017b0: 6572 725f 6f62 7320 3d20 6572 725f 6d6f  err_obs = err_mo
-000017c0: 6465 6c0d 0a20 2020 6060 600d 0a0d 0a23  del..   ```....#
-000017d0: 2323 2043 6f6e 5445 5354 2066 6f72 2072  ## ConTEST for r
-000017e0: 6567 7265 7373 696f 6e0d 0a20 0d0a 2020  egression.. ..  
-000017f0: 2060 6060 7368 0d0a 2020 2054 6573 7431   ```sh..   Test1
-00001800: 203d 2063 6f6e 7465 7374 5f72 6567 2879   = contest_reg(y
-00001810: 5f6f 6273 203d 206f 6273 2c20 785f 6f62  _obs = obs, x_ob
-00001820: 7320 3d20 782c 2079 5f6d 6f64 203d 206d  s = x, y_mod = m
-00001830: 6f64 656c 2c20 795f 6f62 735f 6572 7220  odel, y_obs_err 
-00001840: 3d20 6572 725f 6f62 732c 204b 3d31 3030  = err_obs, K=100
-00001850: 302c 706c 6f74 3d54 7275 6529 0d0a 2020  0,plot=True)..  
-00001860: 2060 6060 0d0a 3c69 6d67 2073 7263 3d22   ```..<img src="
-00001870: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001880: 6f6d 2f46 696f 7265 6e53 742f 436f 6e54  om/FiorenSt/ConT
-00001890: 4553 542f 626c 6f62 2f6d 6169 6e2f 696d  EST/blob/main/im
-000018a0: 672f 436f 6e54 4553 5466 6f72 5265 6772  g/ConTESTforRegr
-000018b0: 6573 7369 6f6e 2e70 6e67 2022 2077 6964  ession.png " wid
-000018c0: 7468 3d38 3025 2068 6569 6768 743d 3830  th=80% height=80
-000018d0: 253e 0d0a 0d0a 0d0a 2323 2320 536d 6f6f  %>......### Smoo
-000018e0: 7468 6564 2043 6f6e 5445 5354 2066 6f72  thed ConTEST for
-000018f0: 2072 6567 7265 7373 696f 6e0d 0a20 0d0a   regression.. ..
-00001900: 2020 2060 6060 7368 0d0a 2020 2054 6573     ```sh..   Tes
-00001910: 7432 203d 2073 6d6f 6f74 6865 645f 636f  t2 = smoothed_co
-00001920: 6e74 6573 745f 7265 6728 795f 6f62 7320  ntest_reg(y_obs 
-00001930: 3d20 6f62 732c 2078 5f6f 6273 203d 2078  = obs, x_obs = x
-00001940: 2c20 795f 6d6f 6420 3d20 6d6f 6465 6c2c  , y_mod = model,
-00001950: 2079 5f6f 6273 5f65 7272 203d 2065 7272   y_obs_err = err
-00001960: 5f6f 6273 2c20 4b3d 3130 3030 2c70 6c6f  _obs, K=1000,plo
-00001970: 743d 5472 7565 2920 2020 0d0a 2020 2060  t=True)   ..   `
-00001980: 6060 0d0a 3c69 6d67 2073 7263 3d22 6874  ``..<img src="ht
-00001990: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000019a0: 2f46 696f 7265 6e53 742f 436f 6e54 4553  /FiorenSt/ConTES
-000019b0: 542f 626c 6f62 2f6d 6169 6e2f 696d 672f  T/blob/main/img/
-000019c0: 536d 6f6f 7468 6564 436f 6e54 4553 5466  SmoothedConTESTf
-000019d0: 6f72 5265 6772 6573 7369 6f6e 2e70 6e67  orRegression.png
-000019e0: 2022 2077 6964 7468 3d38 3025 2068 6569   " width=80% hei
-000019f0: 6768 743d 3830 253e 0d0a 0d0a 0d0a 2323  ght=80%>......##
-00001a00: 2044 656e 7369 7479 206d 6f64 656c 730d   Density models.
-00001a10: 0a0d 0a43 7265 6174 6520 7379 6e74 6865  ...Create synthe
-00001a20: 7469 6320 6d6f 6465 6c20 616e 6420 6f62  tic model and ob
-00001a30: 7365 7276 6174 696f 6e73 3a0d 0a0d 0a20  servations:.... 
-00001a40: 2020 6060 6073 680d 0a20 2020 6e3d 3130    ```sh..   n=10
-00001a50: 300d 0a20 2020 0d0a 2020 2023 3144 2065  0..   ..   #1D e
-00001a60: 7861 6d70 6c65 0d0a 2020 206f 6273 203d  xample..   obs =
-00001a70: 2073 7461 7473 2e6d 756c 7469 7661 7269   stats.multivari
-00001a80: 6174 655f 6e6f 726d 616c 2e72 7673 286d  ate_normal.rvs(m
-00001a90: 6561 6e3d 352c 2063 6f76 3d20 5b31 2e35  ean=5, cov= [1.5
-00001aa0: 5d2c 7369 7a65 3d6e 290d 0a20 2020 6d6f  ],size=n)..   mo
-00001ab0: 6465 6c20 3d20 7374 6174 732e 6d75 6c74  del = stats.mult
-00001ac0: 6976 6172 6961 7465 5f6e 6f72 6d61 6c2e  ivariate_normal.
-00001ad0: 7276 7328 6d65 616e 3d35 2c20 636f 763d  rvs(mean=5, cov=
-00001ae0: 205b 312e 355d 2c73 697a 653d 3130 3030   [1.5],size=1000
-00001af0: 290d 0a20 2020 200d 0a20 2020 2332 4420  )..    ..   #2D 
-00001b00: 6578 616d 706c 650d 0a20 2020 6f62 735f  example..   obs_
-00001b10: 3264 203d 2020 7374 6174 732e 6d75 6c74  2d =  stats.mult
-00001b20: 6976 6172 6961 7465 5f6e 6f72 6d61 6c2e  ivariate_normal.
-00001b30: 7276 7328 6d65 616e 3d5b 352c 355d 2c20  rvs(mean=[5,5], 
-00001b40: 636f 763d 205b 5b31 2e35 2c2e 385d 2c5b  cov= [[1.5,.8],[
-00001b50: 2e38 2c32 2e35 5d5d 2c73 697a 653d 6e29  .8,2.5]],size=n)
-00001b60: 0d0a 2020 206d 6f64 656c 5f32 6420 3d20  ..   model_2d = 
-00001b70: 7374 6174 732e 6d75 6c74 6976 6172 6961  stats.multivaria
-00001b80: 7465 5f6e 6f72 6d61 6c2e 7276 7328 6d65  te_normal.rvs(me
-00001b90: 616e 3d5b 352c 355d 2c20 636f 763d 205b  an=[5,5], cov= [
-00001ba0: 5b31 2e35 2c2e 385d 2c5b 2e38 2c32 2e35  [1.5,.8],[.8,2.5
-00001bb0: 5d5d 2c73 697a 653d 3130 3030 290d 0a0d  ]],size=1000)...
-00001bc0: 0a23 2323 2043 6f6e 5445 5354 2066 6f72  .### ConTEST for
-00001bd0: 206f 7574 6c69 6572 7320 0d0a 0d0a 2020   outliers ....  
-00001be0: 2060 6060 7368 0d0a 2020 2054 6573 7433   ```sh..   Test3
-00001bf0: 203d 2063 6f6e 7465 7374 5f6f 7574 6c69   = contest_outli
-00001c00: 6572 7328 6d6f 643d 6d6f 6465 6c2c 206f  ers(mod=model, o
-00001c10: 6273 3d6f 6273 2c20 4b3d 3130 3030 302c  bs=obs, K=10000,
-00001c20: 2070 6c6f 743d 5472 7565 290d 0a20 2020   plot=True)..   
-00001c30: 5465 7374 3320 3d20 636f 6e74 6573 745f  Test3 = contest_
-00001c40: 6f75 746c 6965 7273 286d 6f64 3d6d 6f64  outliers(mod=mod
-00001c50: 656c 5f32 642c 206f 6273 3d6f 6273 5f32  el_2d, obs=obs_2
-00001c60: 642c 204b 3d31 3030 3030 2c20 706c 6f74  d, K=10000, plot
-00001c70: 3d54 7275 6529 0d0a 2020 2060 6060 0d0a  =True)..   ```..
-00001c80: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00001c90: 2f2f 6769 7468 7562 2e63 6f6d 2f46 696f  //github.com/Fio
-00001ca0: 7265 6e53 742f 436f 6e54 4553 542f 626c  renSt/ConTEST/bl
-00001cb0: 6f62 2f6d 6169 6e2f 696d 672f 436f 6e54  ob/main/img/ConT
-00001cc0: 4553 5466 6f72 4f75 746c 6965 7273 3144  ESTforOutliers1D
-00001cd0: 2e70 6e67 2022 2077 6964 7468 3d38 3025  .png " width=80%
-00001ce0: 2068 6569 6768 743d 3830 253e 0d0a 3c69   height=80%>..<i
-00001cf0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00001d00: 6769 7468 7562 2e63 6f6d 2f46 696f 7265  github.com/Fiore
-00001d10: 6e53 742f 436f 6e54 4553 542f 626c 6f62  nSt/ConTEST/blob
-00001d20: 2f6d 6169 6e2f 696d 672f 436f 6e54 4553  /main/img/ConTES
-00001d30: 5466 6f72 4f75 746c 6965 7273 3244 2e70  TforOutliers2D.p
-00001d40: 6e67 2022 2077 6964 7468 3d38 3025 2068  ng " width=80% h
-00001d50: 6569 6768 743d 3830 253e 0d0a 0d0a 0d0a  eight=80%>......
-00001d60: 0d0a 2323 2320 436f 6e54 4553 5420 666f  ..### ConTEST fo
-00001d70: 7220 6465 6e73 6974 6965 7320 0d0a 0d0a  r densities ....
-00001d80: 2020 2060 6060 7368 0d0a 2020 2054 6573     ```sh..   Tes
-00001d90: 7434 203d 2063 6f6e 7465 7374 5f64 656e  t4 = contest_den
-00001da0: 7328 6d6f 643d 6d6f 6465 6c2c 206f 6273  s(mod=model, obs
-00001db0: 3d6f 6273 2c20 4b3d 3130 3030 302c 2070  =obs, K=10000, p
-00001dc0: 6c6f 743d 5472 7565 2920 2020 0d0a 2020  lot=True)   ..  
-00001dd0: 2054 6573 7434 203d 2063 6f6e 7465 7374   Test4 = contest
-00001de0: 5f64 656e 7328 6d6f 643d 6d6f 6465 6c5f  _dens(mod=model_
-00001df0: 3264 2c20 6f62 733d 6f62 735f 3264 2c20  2d, obs=obs_2d, 
-00001e00: 4b3d 3130 3030 302c 2070 6c6f 743d 5472  K=10000, plot=Tr
-00001e10: 7565 290d 0a0d 0a20 2020 6060 600d 0a3c  ue)....   ```..<
-00001e20: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00001e30: 2f67 6974 6875 622e 636f 6d2f 4669 6f72  /github.com/Fior
-00001e40: 656e 5374 2f43 6f6e 5445 5354 2f62 6c6f  enSt/ConTEST/blo
-00001e50: 622f 6d61 696e 2f69 6d67 2f43 6f6e 5445  b/main/img/ConTE
-00001e60: 5354 666f 7244 656e 7369 7469 6573 3144  STforDensities1D
-00001e70: 2e70 6e67 2022 2077 6964 7468 3d38 3025  .png " width=80%
-00001e80: 2068 6569 6768 743d 3830 253e 0d0a 3c69   height=80%>..<i
-00001e90: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00001ea0: 6769 7468 7562 2e63 6f6d 2f46 696f 7265  github.com/Fiore
-00001eb0: 6e53 742f 436f 6e54 4553 542f 626c 6f62  nSt/ConTEST/blob
-00001ec0: 2f6d 6169 6e2f 696d 672f 436f 6e54 4553  /main/img/ConTES
-00001ed0: 5466 6f72 4465 6e73 6974 6965 7332 442e  TforDensities2D.
-00001ee0: 706e 6720 2220 7769 6474 683d 3830 2520  png " width=80% 
-00001ef0: 6865 6967 6874 3d38 3025 3e0d 0a0d 0a0d  height=80%>.....
-00001f00: 0a0d 0a0d 0a                             .....
+00000000: 3c69 6d67 2073 7263 3d68 7474 7073 3a2f  <img src=https:/
+00000010: 2f73 6565 2e66 6f6e 7469 6d67 2e63 6f6d  /see.fontimg.com
+00000020: 2f61 7069 2f72 656e 6465 7266 6f6e 7434  /api/renderfont4
+00000030: 2f4b 7041 702f 6579 4a79 496a 6f69 5a6e  /KpAp/eyJyIjoiZn
+00000040: 4d69 4c43 4a6f 496a 6f78 4d7a 4173 496e  MiLCJoIjoxMzAsIn
+00000050: 6369 4f6a 4577 4d44 4173 496d 5a7a 496a  ciOjEwMDAsImZzIj
+00000060: 6f78 4d7a 4173 496d 5a6e 5979 4936 4969  oxMzAsImZnYyI6Ii
+00000070: 4e47 5244 6844 4d44 4d69 4c43 4a69 5a32  NGRDhDMDMiLCJiZ2
+00000080: 4d69 4f69 496a 4d44 5977 4e54 4131 4969  MiOiIjMDYwNTA1Ii
+00000090: 7769 6443 4936 4d58 302f 5132 3975 5645  widCI6MX0/Q29uVE
+000000a0: 5654 5641 2f6b 672d 7365 636f 6e64 2d63  VTVA/kg-second-c
+000000b0: 6861 6e63 6573 2d73 6b65 7463 682e 706e  hances-sketch.pn
+000000c0: 6720 7769 6474 683d 3530 2520 6865 6967  g width=50% heig
+000000d0: 6874 3d35 3025 3e0a 0a0a 3c21 2d2d 0a5b  ht=50%>...<!--.[
+000000e0: 215b 444f 495d 2868 7474 7073 3a2f 2f7a  ![DOI](https://z
+000000f0: 656e 6f64 6f2e 6f72 672f 6261 6467 652f  enodo.org/badge/
+00000100: 3434 3038 3531 3434 372e 7376 6729 5d28  440851447.svg)](
+00000110: 6874 7470 733a 2f2f 7a65 6e6f 646f 2e6f  https://zenodo.o
+00000120: 7267 2f62 6164 6765 2f6c 6174 6573 7464  rg/badge/latestd
+00000130: 6f69 2f34 3430 3835 3134 3437 2920 0a3c  oi/440851447) .<
+00000140: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000150: 6173 636c 2e6e 6574 2f32 3230 332e 3031  ascl.net/2203.01
+00000160: 3422 3e3c 696d 6720 7372 633d 2268 7474  4"><img src="htt
+00000170: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000180: 2e69 6f2f 6261 6467 652f 6173 636c 2d32  .io/badge/ascl-2
+00000190: 3230 332e 3031 342d 626c 7565 2e73 7667  203.014-blue.svg
+000001a0: 3f63 6f6c 6f72 423d 3236 3232 3535 2220  ?colorB=262255" 
+000001b0: 616c 743d 2261 7363 6c3a 3232 3033 2e30  alt="ascl:2203.0
+000001c0: 3134 2220 2f3e 3c2f 613e 0a0a 3c69 6d67  14" /></a>..<img
+000001d0: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+000001e0: 7468 7562 2e63 6f6d 2f46 696f 7265 6e53  thub.com/FiorenS
+000001f0: 742f 4175 746f 536f 7572 6365 4944 2d4c  t/AutoSourceID-L
+00000200: 6967 6874 2f62 6c6f 622f 6d61 696e 2f50  ight/blob/main/P
+00000210: 6c6f 7473 2f4f 7074 6963 616c 496d 6167  lots/OpticalImag
+00000220: 6550 6174 6368 2e70 6e67 2022 2077 6964  ePatch.png " wid
+00000230: 7468 3d35 3025 2068 6569 6768 743d 3530  th=50% height=50
+00000240: 253e 3c69 6d67 2073 7263 3d22 6874 7470  %><img src="http
+00000250: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f46  s://github.com/F
+00000260: 696f 7265 6e53 742f 4175 746f 536f 7572  iorenSt/AutoSour
+00000270: 6365 4944 2d4c 6967 6874 2f62 6c6f 622f  ceID-Light/blob/
+00000280: 6d61 696e 2f50 6c6f 7473 2f4c 6f47 4f6e  main/Plots/LoGOn
+00000290: 4f70 7469 6361 6c2e 706e 6720 2220 7769  Optical.png " wi
+000002a0: 6474 683d 3530 2520 6865 6967 6874 3d35  dth=50% height=5
+000002b0: 3025 3e20 0a0a 2d2d 3e0a 0a0a 2320 4465  0%> ..-->...# De
+000002c0: 7363 7269 7074 696f 6e0a 0a43 6f6e 5445  scription..ConTE
+000002d0: 5354 2069 7320 6120 7374 6174 6973 7469  ST is a statisti
+000002e0: 6361 6c20 7465 7374 2066 6f72 2061 7373  cal test for ass
+000002f0: 6573 7369 6e67 2074 6865 2063 6f6e 7369  essing the consi
+00000300: 7374 656e 6379 2062 6574 7765 656e 206f  stency between o
+00000310: 6273 6572 7661 7469 6f6e 7320 616e 6420  bservations and 
+00000320: 6173 7472 6f70 6879 7369 6361 6c20 6d6f  astrophysical mo
+00000330: 6465 6c73 2e0a 4974 2075 7365 7320 6120  dels..It uses a 
+00000340: 636f 6d62 696e 6174 696f 6e20 6f66 206e  combination of n
+00000350: 6f6e 2d70 6172 616d 6574 7269 6320 6d65  on-parametric me
+00000360: 7468 6f64 7320 616e 6420 6469 7374 616e  thods and distan
+00000370: 6365 206d 6561 7375 7265 7320 746f 206f  ce measures to o
+00000380: 6274 6169 6e20 6120 7465 7374 0a73 7461  btain a test.sta
+00000390: 7469 7374 6963 2074 6861 7420 6576 616c  tistic that eval
+000003a0: 7561 7465 7320 7468 6520 636c 6f73 656e  uates the closen
+000003b0: 6573 7320 6f66 2074 6865 2061 7374 726f  ess of the astro
+000003c0: 7068 7973 6963 616c 206d 6f64 656c 2074  physical model t
+000003d0: 6f20 7468 6520 6f62 7365 7276 6174 696f  o the observatio
+000003e0: 6e73 3b20 6879 706f 7468 6573 6973 2074  ns; hypothesis t
+000003f0: 6573 7469 6e67 2069 7320 7468 656e 2070  esting is then p
+00000400: 6572 666f 726d 6564 2075 7369 6e67 2062  erformed using b
+00000410: 6f6f 7473 7472 6170 2e0a 200a 0a3c 696d  ootstrap.. ..<im
+00000420: 6720 7372 633d 6874 7470 733a 2f2f 6769  g src=https://gi
+00000430: 7468 7562 2e63 6f6d 2f46 696f 7265 6e53  thub.com/FiorenS
+00000440: 742f 436f 6e54 4553 542f 626c 6f62 2f6d  t/ConTEST/blob/m
+00000450: 6169 6e2f 696d 672f 6c6f 676f 5f63 6f6e  ain/img/logo_con
+00000460: 7465 7374 5f62 6b67 2e70 6e67 2077 6964  test_bkg.png wid
+00000470: 7468 3d31 3525 2068 6569 6768 743d 3135  th=15% height=15
+00000480: 253e 0a0a 0a23 2320 5461 626c 6520 6f66  %>...## Table of
+00000490: 2043 6f6e 7465 6e74 7320 0a2d 205b 5374   Contents .- [St
+000004a0: 6570 2d62 792d 7374 6570 2073 6574 7570  ep-by-step setup
+000004b0: 5d28 2373 7465 702d 6279 2d73 7465 702d  ](#step-by-step-
+000004c0: 7365 7475 7029 0a2d 205b 5475 746f 7269  setup).- [Tutori
+000004d0: 616c 5d28 2374 7574 6f72 6961 6c29 0a0a  al](#tutorial)..
+000004e0: 0a23 2053 7465 702d 6279 2d73 7465 7020  .# Step-by-step 
+000004f0: 7365 7475 700a 0a5f 466f 6c6c 6f77 2074  setup.._Follow t
+00000500: 6865 2069 6e73 7472 7563 7469 6f6e 7320  he instructions 
+00000510: 6265 6c6f 7720 746f 2069 6e73 7461 6c6c  below to install
+00000520: 2061 6e64 2073 7461 7274 2075 7369 6e67   and start using
+00000530: 2043 6f6e 5445 5354 2069 6e20 5079 7468   ConTEST in Pyth
+00000540: 6f6e 2e5f 0a0a 312e 2049 6e73 7461 6c6c  on._..1. Install
+00000550: 2043 6f6e 5445 5354 3a0a 2020 2060 6060   ConTEST:.   ```
+00000560: 7368 0a20 2020 7069 7020 696e 7374 616c  sh.   pip instal
+00000570: 6c20 436f 6e73 6973 7465 6e63 7954 4553  l ConsistencyTES
+00000580: 540a 2020 2060 6060 0a20 2020 6f72 2067  T.   ```.   or g
+00000590: 6974 2063 6c6f 6e65 2074 6865 2072 6570  it clone the rep
+000005a0: 6f73 6974 6f72 793a 0a20 2020 2060 6060  ository:.    ```
+000005b0: 7368 0a20 2020 6769 7420 636c 6f6e 6520  sh.   git clone 
+000005c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000005d0: 6f6d 2f46 696f 7265 6e53 742f 436f 6e54  om/FiorenSt/ConT
+000005e0: 4553 542e 6769 740a 2020 2060 6060 0a20  EST.git.   ```. 
+000005f0: 2020 0a0a 203c 6272 2f3e 0a0a 322e 2028    .. <br/>..2. (
+00000600: 4f70 7469 6f6e 616c 2920 496e 7374 616c  Optional) Instal
+00000610: 6c20 7468 6520 7374 6174 6973 7469 6361  l the statistica
+00000620: 6c20 736f 6674 7761 7265 205b 525d 2868  l software [R](h
+00000630: 7474 7073 3a2f 2f77 7777 2e72 2d70 726f  ttps://www.r-pro
+00000640: 6a65 6374 2e6f 7267 2f29 2e20 5220 6973  ject.org/). R is
+00000650: 2072 6571 7569 7265 6420 6f6e 6c79 2069   required only i
+00000660: 6620 796f 7520 706c 616e 2074 6f20 7573  f you plan to us
+00000670: 6520 7468 6520 6073 6d6f 6f74 6865 645f  e the `smoothed_
+00000680: 636f 6e74 6573 745f 7265 6728 2960 2066  contest_reg()` f
+00000690: 756e 6374 696f 6e2e 2054 6869 7320 6675  unction. This fu
+000006a0: 6e63 7469 6f6e 2065 6d70 6c6f 7973 206c  nction employs l
+000006b0: 6f63 616c 206c 696e 6561 7220 7265 6772  ocal linear regr
+000006c0: 6573 7369 6f6e 2075 7369 6e67 2074 6865  ession using the
+000006d0: 2060 6e70 6020 7061 636b 6167 6520 696e   `np` package in
+000006e0: 2052 2e0a 3c62 722f 3e0a 0a33 2e20 284f   R..<br/>..3. (O
+000006f0: 7074 696f 6e61 6c29 2054 6f20 656e 7375  ptional) To ensu
+00000700: 7265 2074 6861 7420 5079 7468 6f6e 2063  re that Python c
+00000710: 616e 2061 6363 6573 7320 5227 7320 6c69  an access R's li
+00000720: 6272 6172 6965 732c 2072 756e 2074 6865  braries, run the
+00000730: 2074 6872 6565 206c 696e 6573 2062 656c   three lines bel
+00000740: 6f77 2069 6e20 5079 7468 6f6e 2028 6f66  ow in Python (of
+00000750: 2063 6f75 7273 652c 206d 6f64 6966 7920   course, modify 
+00000760: 746f 206d 6174 6368 2079 6f75 7220 666f  to match your fo
+00000770: 6c64 6572 7329 2e20 5468 6973 2073 7465  lders). This ste
+00000780: 7020 6973 206f 6e6c 7920 6e65 6365 7373  p is only necess
+00000790: 6172 7920 6966 2079 6f75 2069 6e74 656e  ary if you inten
+000007a0: 6420 746f 2075 7365 2074 6865 2060 736d  d to use the `sm
+000007b0: 6f6f 7468 6564 5f63 6f6e 7465 7374 5f72  oothed_contest_r
+000007c0: 6567 2829 6020 6675 6e63 7469 6f6e 3a0a  eg()` function:.
+000007d0: 0a20 2020 6060 6073 680a 2020 2020 696d  .   ```sh.    im
+000007e0: 706f 7274 206f 730a 2020 2020 6f73 2e65  port os.    os.e
+000007f0: 6e76 6972 6f6e 5b27 525f 484f 4d45 275d  nviron['R_HOME']
+00000800: 203d 2027 7e2f 5072 6f67 7261 6d20 4669   = '~/Program Fi
+00000810: 6c65 732f 522f 522d 342e 302e 3227 2020  les/R/R-4.0.2'  
+00000820: 232d 3e20 596f 7572 2069 6e73 7461 6c6c  #-> Your install
+00000830: 6564 2052 2066 6f6c 6465 720a 2020 2020  ed R folder.    
+00000840: 6f73 2e65 6e76 6972 6f6e 5b27 525f 5553  os.environ['R_US
+00000850: 4552 275d 203d 2027 7e2f 4d69 6e69 636f  ER'] = '~/Minico
+00000860: 6e64 6133 2f65 6e76 732f 436f 6e73 6973  nda3/envs/Consis
+00000870: 7465 6e63 7954 6573 742f 6c69 622f 7369  tencyTest/lib/si
+00000880: 7465 2d70 6163 6b61 6765 732f 2720 2023  te-packages/'  #
+00000890: 2d3e 2059 6f75 7220 7079 7468 6f6e 2065  -> Your python e
+000008a0: 6e76 6972 6f6e 6d65 6e74 0a20 2020 206f  nvironment.    o
+000008b0: 732e 656e 7669 726f 6e5b 2752 5f4c 4942  s.environ['R_LIB
+000008c0: 535f 5553 4552 275d 203d 2022 7e2f 5072  S_USER'] = "~/Pr
+000008d0: 6f67 7261 6d20 4669 6c65 732f 522f 522d  ogram Files/R/R-
+000008e0: 342e 302e 322f 6c69 6272 6172 792f 2220  4.0.2/library/" 
+000008f0: 2023 2d3e 2059 6f75 7220 5220 7061 636b   #-> Your R pack
+00000900: 6167 6573 206c 6962 7261 7279 0a20 2020  ages library.   
+00000910: 6060 600a 3c62 722f 3e0a 0a0a 342e 2049  ```.<br/>...4. I
+00000920: 6e73 7461 6c6c 2050 7974 686f 6e20 6465  nstall Python de
+00000930: 7065 6e64 656e 6369 6573 2e20 4e6f 7465  pendencies. Note
+00000940: 2074 6861 7420 7468 6520 6072 7079 3260   that the `rpy2`
+00000950: 2070 6163 6b61 6765 2c20 7768 6963 6820   package, which 
+00000960: 6661 6369 6c69 7461 7465 7320 696e 7465  facilitates inte
+00000970: 7261 6374 696f 6e20 6265 7477 6565 6e20  raction between 
+00000980: 5220 616e 6420 5079 7468 6f6e 2c20 6973  R and Python, is
+00000990: 2072 6571 7569 7265 6420 6f6e 6c79 2069   required only i
+000009a0: 6620 796f 7520 706c 616e 2074 6f20 7573  f you plan to us
+000009b0: 6520 7468 6520 6073 6d6f 6f74 6865 645f  e the `smoothed_
+000009c0: 636f 6e74 6573 745f 7265 6728 2960 2066  contest_reg()` f
+000009d0: 756e 6374 696f 6e3a 0a20 2020 6060 6073  unction:.   ```s
+000009e0: 680a 2020 2070 6970 2069 6e74 616c 6c20  h.   pip intall 
+000009f0: 6d61 7470 6c6f 746c 6962 0a20 2020 7069  matplotlib.   pi
+00000a00: 7020 696e 7461 6c6c 206e 756d 7079 0a20  p intall numpy. 
+00000a10: 2020 7069 7020 696e 7461 6c6c 2070 616e    pip intall pan
+00000a20: 6461 730a 2020 2070 6970 2069 6e74 616c  das.   pip intal
+00000a30: 6c20 7363 6970 790a 2020 2070 6970 2069  l scipy.   pip i
+00000a40: 6e74 616c 6c20 7365 6162 6f72 6e0a 2020  ntall seaborn.  
+00000a50: 2070 6970 2069 6e74 616c 6c20 7270 7932   pip intall rpy2
+00000a60: 0a20 2020 6060 600a 203c 6272 2f3e 0a0a  .   ```. <br/>..
+00000a70: 0a35 2e20 284f 7074 696f 6e61 6c29 2049  .5. (Optional) I
+00000a80: 6620 7468 6973 2069 7320 7468 6520 6669  f this is the fi
+00000a90: 7273 7420 7469 6d65 2079 6f75 2075 7365  rst time you use
+00000aa0: 2043 6f6e 5445 5354 2061 6e64 2079 6f75   ConTEST and you
+00000ab0: 2070 6c61 6e20 746f 2075 7365 2074 6865   plan to use the
+00000ac0: 2060 736d 6f6f 7468 6564 5f63 6f6e 7465   `smoothed_conte
+00000ad0: 7374 5f72 6567 2829 6020 6675 6e63 7469  st_reg()` functi
+00000ae0: 6f6e 2c20 796f 7520 6e65 6564 2074 6f20  on, you need to 
+00000af0: 696e 7374 616c 6c20 7468 6520 5220 7061  install the R pa
+00000b00: 636b 6167 6520 7573 6564 2069 6e20 536d  ckage used in Sm
+00000b10: 6f6f 7468 6564 2043 6f6e 5445 5354 2e20  oothed ConTEST. 
+00000b20: 496e 2050 7974 686f 6e2c 2073 696d 706c  In Python, simpl
+00000b30: 7920 7275 6e3a 0a0a 2020 2060 6060 7368  y run:..   ```sh
+00000b40: 0a20 2020 2064 6566 2069 6e73 7461 6c6c  .    def install
+00000b50: 5f52 5f66 756e 6374 696f 6e73 2870 6163  _R_functions(pac
+00000b60: 6b6e 616d 6573 3d28 276e 7027 2929 3a0a  knames=('np')):.
+00000b70: 2020 2020 2020 2020 2320 696d 706f 7274          # import
+00000b80: 2052 2773 2075 7469 6c69 7479 2070 6163   R's utility pac
+00000b90: 6b61 6765 0a20 2020 2020 2020 2075 7469  kage.        uti
+00000ba0: 6c73 203d 2072 7061 636b 6167 6573 2e69  ls = rpackages.i
+00000bb0: 6d70 6f72 7472 2827 7574 696c 7327 290a  mportr('utils').
+00000bc0: 2020 2020 2020 2020 2320 7365 6c65 6374          # select
+00000bd0: 2061 206d 6972 726f 7220 666f 7220 5220   a mirror for R 
+00000be0: 7061 636b 6167 6573 0a20 2020 2020 2020  packages.       
+00000bf0: 2075 7469 6c73 2e63 686f 6f73 6543 5241   utils.chooseCRA
+00000c00: 4e6d 6972 726f 7228 696e 643d 3129 2020  Nmirror(ind=1)  
+00000c10: 2320 7365 6c65 6374 2074 6865 2066 6972  # select the fir
+00000c20: 7374 206d 6972 726f 7220 696e 2074 6865  st mirror in the
+00000c30: 206c 6973 740a 2020 2020 2020 2020 2320   list.        # 
+00000c40: 5220 7061 636b 6167 6520 696e 7374 616c  R package instal
+00000c50: 6c0a 2020 2020 2020 2020 7574 696c 732e  l.        utils.
+00000c60: 696e 7374 616c 6c5f 7061 636b 6167 6573  install_packages
+00000c70: 2870 6163 6b6e 616d 6573 290a 2020 2020  (packnames).    
+00000c80: 0a20 2020 2069 6e73 7461 6c6c 5f52 5f66  .    install_R_f
+00000c90: 756e 6374 696f 6e73 2829 0a20 2020 6060  unctions().   ``
+00000ca0: 600a 0a33 2e20 5573 6520 436f 6e54 4553  `..3. Use ConTES
+00000cb0: 5420 696e 2050 7974 686f 6e21 2046 6f6c  T in Python! Fol
+00000cc0: 6c6f 7720 7468 6520 7475 746f 7269 616c  low the tutorial
+00000cd0: 2062 656c 6f77 2066 6f72 206d 6f72 6520   below for more 
+00000ce0: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
+00000cf0: 7420 7468 6520 696e 6469 7669 6475 616c  t the individual
+00000d00: 2066 756e 6374 696f 6e73 2e0a 0a3c 6272   functions...<br
+00000d10: 2f3e 0a0a 0a3c 696d 6720 7372 633d 2268  />...<img src="h
+00000d20: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000d30: 6d2f 4669 6f72 656e 5374 2f43 6f6e 5445  m/FiorenSt/ConTE
+00000d40: 5354 2f62 6c6f 622f 6d61 696e 2f69 6d67  ST/blob/main/img
+00000d50: 2f4d 656d 6543 6f6e 5445 5354 2e70 6e67  /MemeConTEST.png
+00000d60: 2022 2077 6964 7468 3d38 3025 2068 6569   " width=80% hei
+00000d70: 6768 743d 3830 253e 0a0a 3c62 722f 3e0a  ght=80%>..<br/>.
+00000d80: 0a0a 0a0a 2320 4465 7065 6e64 656e 6369  ....# Dependenci
+00000d90: 6573 3a0a 0a54 6865 2066 6f6c 6c6f 7769  es:..The followi
+00000da0: 6e67 2063 6f6d 6269 6e61 7469 6f6e 206f  ng combination o
+00000db0: 6620 7061 636b 6167 6520 7665 7273 696f  f package versio
+00000dc0: 6e73 2077 6f72 6b73 206f 6e20 6d6f 7374  ns works on most
+00000dd0: 204c 696e 7578 2061 6e64 2057 696e 646f   Linux and Windo
+00000de0: 7773 2063 6f6d 7075 7465 7273 2c20 686f  ws computers, ho
+00000df0: 7765 7665 7220 6f74 6865 7220 7061 636b  wever other pack
+00000e00: 6167 6520 7665 7273 696f 6e73 206d 6179  age versions may
+00000e10: 2061 6c73 6f0a 776f 726b 2e20 4966 2061   also.work. If a
+00000e20: 2070 726f 626c 656d 2077 6974 6820 7468   problem with th
+00000e30: 6520 636f 6d62 696e 6174 696f 6e20 6f66  e combination of
+00000e40: 2070 6163 6b61 6765 7320 6f63 6375 7273   packages occurs
+00000e50: 2c20 7261 6973 6520 616e 2069 7373 7565  , raise an issue
+00000e60: 2c20 616e 6420 7765 2077 696c 6c20 6865  , and we will he
+00000e70: 6c70 2079 6f75 2073 6f6c 7665 2069 742e  lp you solve it.
+00000e80: 0a0a 0a23 2323 2050 7974 686f 6e20 3320  ...### Python 3 
+00000e90: 286f 7220 7375 7065 7269 6f72 290a 2a20  (or superior).* 
+00000ea0: 4e75 6d70 7920 312e 3231 2e36 0a2a 2050  Numpy 1.21.6.* P
+00000eb0: 616e 6461 7320 312e 342e 320a 2a20 5363  andas 1.4.2.* Sc
+00000ec0: 6970 7920 312e 372e 310a 2a20 4d61 7470  ipy 1.7.1.* Matp
+00000ed0: 6c6f 746c 6962 2033 2e33 2e34 0a2a 2053  lotlib 3.3.4.* S
+00000ee0: 6561 626f 726e 2030 2e31 312e 320a 2a20  eaborn 0.11.2.* 
+00000ef0: 5270 7932 2033 2e35 2e32 2028 466f 7220  Rpy2 3.5.2 (For 
+00000f00: 5220 616e 6420 5079 7468 6f6e 2069 6e74  R and Python int
+00000f10: 6572 6163 7469 6f6e 290a 0a23 2323 2052  eraction)..### R
+00000f20: 2033 2e36 2e30 2028 6f72 2073 7570 6572   3.6.0 (or super
+00000f30: 696f 7229 0a2a 204e 7020 302e 3630 0a0a  ior).* Np 0.60..
+00000f40: 0a0a 2320 5475 746f 7269 616c 0a0a 436f  ..# Tutorial..Co
+00000f50: 6e54 4553 5420 6361 6e20 6265 2061 7070  nTEST can be app
+00000f60: 6c69 6564 2069 6e20 6469 6666 6572 656e  lied in differen
+00000f70: 7420 6361 7365 2073 6365 6e61 7269 6f73  t case scenarios
+00000f80: 2064 6570 656e 6469 6e67 206f 6e20 7468   depending on th
+00000f90: 6520 6e61 7475 7265 206f 6620 7468 6520  e nature of the 
+00000fa0: 6d6f 6465 6c20 6265 696e 6720 7465 7374  model being test
+00000fb0: 6564 2e20 0a3c 6272 2f3e 0a46 6f72 206d  ed. .<br/>.For m
+00000fc0: 6f72 6520 6465 7461 696c 7320 6368 6563  ore details chec
+00000fd0: 6b20 6f75 7420 7468 6520 7061 7065 723a  k out the paper:
+00000fe0: 205f 5374 6f70 7061 2065 7420 616c 2e2c   _Stoppa et al.,
+00000ff0: 2069 6e20 7072 6570 6172 6174 696f 6e5f   in preparation_
+00001000: 0a0a 5468 6572 6520 6172 6520 3420 6675  ..There are 4 fu
+00001010: 6e64 616d 656e 7461 6c20 6675 6e63 7469  ndamental functi
+00001020: 6f6e 7320 696e 2043 6f6e 5445 5354 3a0a  ons in ConTEST:.
+00001030: 0a2d 2043 6f6e 5445 5354 2066 6f72 2072  .- ConTEST for r
+00001040: 6567 7265 7373 696f 6e3a 2054 6573 7420  egression: Test 
+00001050: 7468 6520 636f 6e73 6973 7465 6e63 7920  the consistency 
+00001060: 6f66 2061 206d 6f64 656c 2077 6974 6820  of a model with 
+00001070: 7265 7370 6563 7420 746f 2061 6e20 6f62  respect to an ob
+00001080: 7365 7276 6564 2064 6174 6173 6574 2061  served dataset a
+00001090: 6e64 2074 6865 6972 2075 6e63 6572 7461  nd their uncerta
+000010a0: 696e 7469 6573 0a2d 2053 6d6f 6f74 6865  inties.- Smoothe
+000010b0: 6420 436f 6e54 4553 5420 666f 7220 7265  d ConTEST for re
+000010c0: 6772 6573 7369 6f6e 2028 7265 7175 6972  gression (requir
+000010d0: 6573 2052 2061 6e64 2074 6865 2060 7270  es R and the `rp
+000010e0: 7932 6020 5079 7468 6f6e 2070 6163 6b61  y2` Python packa
+000010f0: 6765 293a 2054 6573 7420 7468 6520 636f  ge): Test the co
+00001100: 6e73 6973 7465 6e63 7920 6f66 2061 206d  nsistency of a m
+00001110: 6f64 656c 2077 6974 6820 7265 7370 6563  odel with respec
+00001120: 7420 746f 2061 6e20 6f62 7365 7276 6564  t to an observed
+00001130: 2064 6174 6173 6574 2061 6e64 200a 2020   dataset and .  
+00001140: 7468 6569 7220 756e 6365 7274 6169 6e74  their uncertaint
+00001150: 6965 730a 2d20 436f 6e54 4553 5420 666f  ies.- ConTEST fo
+00001160: 7220 6f75 746c 6965 7273 3a20 5465 7374  r outliers: Test
+00001170: 2069 6620 616e 206f 6273 6572 7665 6420   if an observed 
+00001180: 7361 6d70 6c65 2069 7320 6c69 6b65 6c79  sample is likely
+00001190: 2074 6f20 636f 6d65 2066 726f 6d20 6120   to come from a 
+000011a0: 6465 6e73 6974 7920 6d6f 6465 6c20 286f  density model (o
+000011b0: 7220 6120 7369 6d75 6c61 7465 6420 6461  r a simulated da
+000011c0: 7461 7365 7429 0a2d 2043 6f6e 5445 5354  taset).- ConTEST
+000011d0: 2066 6f72 2064 656e 7369 7469 6573 3a20   for densities: 
+000011e0: 5465 7374 2074 6865 2063 6f6e 7369 7374  Test the consist
+000011f0: 656e 6379 206f 6620 6120 6465 6e73 6974  ency of a densit
+00001200: 7920 6d6f 6465 6c20 286f 7220 6120 7369  y model (or a si
+00001210: 6d75 6c61 7465 6420 6461 7461 7365 7429  mulated dataset)
+00001220: 2077 6974 6820 7265 7370 6563 7420 746f   with respect to
+00001230: 2061 6e20 6f62 7365 7276 6564 200a 2020   an observed .  
+00001240: 6461 7461 7365 7420 0a0a 0a23 2323 2049  dataset ...### I
+00001250: 6e74 726f 2073 6372 6970 7420 0a0a 2020  ntro script ..  
+00001260: 2060 6060 7368 0a20 2020 2023 2065 6e73   ```sh.    # ens
+00001270: 7572 6520 7468 6174 2050 7974 686f 6e20  ure that Python 
+00001280: 6361 6e20 6163 6365 7373 2052 0a20 2020  can access R.   
+00001290: 2069 6d70 6f72 7420 6f73 0a20 2020 206f   import os.    o
+000012a0: 732e 656e 7669 726f 6e5b 2752 5f48 4f4d  s.environ['R_HOM
+000012b0: 4527 5d20 3d20 277e 2f50 726f 6772 616d  E'] = '~/Program
+000012c0: 2046 696c 6573 2f52 2f52 2d34 2e30 2e32   Files/R/R-4.0.2
+000012d0: 2720 2023 2d3e 2059 6f75 7220 696e 7374  '  #-> Your inst
+000012e0: 616c 6c65 6420 5220 666f 6c64 6572 0a20  alled R folder. 
+000012f0: 2020 206f 732e 656e 7669 726f 6e5b 2752     os.environ['R
+00001300: 5f55 5345 5227 5d20 3d20 277e 2f4d 696e  _USER'] = '~/Min
+00001310: 6963 6f6e 6461 332f 656e 7673 2f43 6f6e  iconda3/envs/Con
+00001320: 7369 7374 656e 6379 5465 7374 2f6c 6962  sistencyTest/lib
+00001330: 2f73 6974 652d 7061 636b 6167 6573 2f27  /site-packages/'
+00001340: 2020 232d 3e20 596f 7572 2070 7974 686f    #-> Your pytho
+00001350: 6e20 656e 7669 726f 6e6d 656e 740a 2020  n environment.  
+00001360: 2020 6f73 2e65 6e76 6972 6f6e 5b27 525f    os.environ['R_
+00001370: 4c49 4253 5f55 5345 5227 5d20 3d20 227e  LIBS_USER'] = "~
+00001380: 2f50 726f 6772 616d 2046 696c 6573 2f52  /Program Files/R
+00001390: 2f52 2d34 2e30 2e32 2f6c 6962 7261 7279  /R-4.0.2/library
+000013a0: 2f22 2020 232d 3e20 596f 7572 2052 2070  /"  #-> Your R p
+000013b0: 6163 6b61 6765 7320 6c69 6272 6172 790a  ackages library.
+000013c0: 2020 2020 0a20 2020 2023 206c 6f61 6420      .    # load 
+000013d0: 636f 6e74 6573 7420 6675 6e63 7469 6f6e  contest function
+000013e0: 730a 2020 2020 6672 6f6d 2043 6f6e 5445  s.    from ConTE
+000013f0: 5354 2e43 4f4e 5445 5354 2069 6d70 6f72  ST.CONTEST impor
+00001400: 7420 636f 6e74 6573 745f 7265 672c 2073  t contest_reg, s
+00001410: 6d6f 6f74 6865 645f 636f 6e74 6573 745f  moothed_contest_
+00001420: 7265 672c 2063 6f6e 7465 7374 5f6f 7574  reg, contest_out
+00001430: 6c69 6572 732c 2063 6f6e 7465 7374 5f64  liers, contest_d
+00001440: 656e 730a 2020 2060 6060 0a0a 0a23 2320  ens.   ```...## 
+00001450: 5265 6772 6573 7369 6f6e 206d 6f64 656c  Regression model
+00001460: 730a 0a43 7265 6174 6520 7379 6e74 6865  s..Create synthe
+00001470: 7469 6320 6d6f 6465 6c2c 206f 6273 6572  tic model, obser
+00001480: 7661 7469 6f6e 732c 2061 6e64 2075 6e63  vations, and unc
+00001490: 6572 7461 696e 7469 6573 2074 6f20 7465  ertainties to te
+000014a0: 7374 2074 6865 2066 756e 6374 696f 6e73  st the functions
+000014b0: 3a0a 0a20 2020 6060 6073 680a 2020 2023  :..   ```sh.   #
+000014c0: 2072 616e 646f 6d20 7361 6d70 6c65 200a   random sample .
+000014d0: 2020 206e 3d31 3030 0a20 2020 7820 3d20     n=100.   x = 
+000014e0: 6e70 2e72 616e 646f 6d2e 7261 6e64 286e  np.random.rand(n
+000014f0: 290a 2020 200a 2020 2023 2073 796e 7468  ).   .   # synth
+00001500: 6574 6963 206d 6f64 656c 200a 2020 2062  etic model .   b
+00001510: 6574 6131 203d 202d 302e 330a 2020 2062  eta1 = -0.3.   b
+00001520: 6574 6132 203d 2038 0a20 2020 6d20 3d20  eta2 = 8.   m = 
+00001530: 320a 2020 206d 6f64 656c 203d 206e 702e  2.   model = np.
+00001540: 6578 7028 6265 7461 312a 7829 2a6e 702e  exp(beta1*x)*np.
+00001550: 7369 6e28 6265 7461 322a 7829 202b 206d  sin(beta2*x) + m
+00001560: 0a20 2020 0a20 2020 2320 6572 726f 7220  .   .   # error 
+00001570: 6675 6e63 7469 6f6e 2028 4e6f 7420 6b6e  function (Not kn
+00001580: 6f77 6e20 696e 2072 6561 6c20 7363 656e  own in real scen
+00001590: 6172 696f 7329 0a20 2020 6572 725f 6d6f  arios).   err_mo
+000015a0: 6465 6c20 3d20 6d6f 6465 6c20 2a20 2e30  del = model * .0
+000015b0: 350a 2020 200a 2020 2023 2073 616d 706c  5.   .   # sampl
+000015c0: 6520 6f62 7365 7276 6174 696f 6e73 2066  e observations f
+000015d0: 726f 6d20 7468 6520 6d6f 6465 6c20 7769  rom the model wi
+000015e0: 7468 2074 6865 2063 6f72 7265 6374 2075  th the correct u
+000015f0: 6e63 6572 7461 696e 7469 6573 0a20 2020  ncertainties.   
+00001600: 6f62 7320 3d20 6e70 2e7a 6572 6f73 284e  obs = np.zeros(N
+00001610: 290a 2020 2020 2020 666f 7220 6920 696e  ).      for i in
+00001620: 2072 616e 6765 284e 293a 0a20 2020 2020   range(N):.     
+00001630: 6f62 735b 695d 203d 206d 6f64 656c 5b69  obs[i] = model[i
+00001640: 5d20 2b20 7374 6174 732e 6d75 6c74 6976  ] + stats.multiv
+00001650: 6172 6961 7465 5f6e 6f72 6d61 6c2e 7276  ariate_normal.rv
+00001660: 7328 6d65 616e 3d30 2c20 636f 763d 2865  s(mean=0, cov=(e
+00001670: 7272 5f6d 6f64 656c 5b69 5d29 2a2a 322c  rr_model[i])**2,
+00001680: 7369 7a65 3d31 290a 2020 200a 2020 2023  size=1).   .   #
+00001690: 2061 7373 6967 6e20 636f 7272 6563 7420   assign correct 
+000016a0: 756e 6365 7274 6169 6e74 6965 7320 746f  uncertainties to
+000016b0: 2074 6865 206f 6273 6572 7661 7469 6f6e   the observation
+000016c0: 730a 2020 2065 7272 5f6f 6273 203d 2065  s.   err_obs = e
+000016d0: 7272 5f6d 6f64 656c 0a20 2020 6060 600a  rr_model.   ```.
+000016e0: 0a23 2323 2043 6f6e 5445 5354 2066 6f72  .### ConTEST for
+000016f0: 2072 6567 7265 7373 696f 6e0a 200a 2020   regression. .  
+00001700: 2060 6060 7368 0a20 2020 5465 7374 3120   ```sh.   Test1 
+00001710: 3d20 636f 6e74 6573 745f 7265 6728 795f  = contest_reg(y_
+00001720: 6f62 7320 3d20 6f62 732c 2078 5f6f 6273  obs = obs, x_obs
+00001730: 203d 2078 2c20 795f 6d6f 6420 3d20 6d6f   = x, y_mod = mo
+00001740: 6465 6c2c 2079 5f6f 6273 5f65 7272 203d  del, y_obs_err =
+00001750: 2065 7272 5f6f 6273 2c20 4b3d 3130 3030   err_obs, K=1000
+00001760: 2c70 6c6f 743d 5472 7565 290a 2020 2060  ,plot=True).   `
+00001770: 6060 0a3c 696d 6720 7372 633d 2268 7474  ``.<img src="htt
+00001780: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001790: 4669 6f72 656e 5374 2f43 6f6e 5445 5354  FiorenSt/ConTEST
+000017a0: 2f62 6c6f 622f 6d61 696e 2f69 6d67 2f43  /blob/main/img/C
+000017b0: 6f6e 5445 5354 666f 7252 6567 7265 7373  onTESTforRegress
+000017c0: 696f 6e2e 706e 6720 2220 7769 6474 683d  ion.png " width=
+000017d0: 3830 2520 6865 6967 6874 3d38 3025 3e0a  80% height=80%>.
+000017e0: 0a0a 2323 2320 536d 6f6f 7468 6564 2043  ..### Smoothed C
+000017f0: 6f6e 5445 5354 2066 6f72 2072 6567 7265  onTEST for regre
+00001800: 7373 696f 6e20 2872 6571 7569 7265 7320  ssion (requires 
+00001810: 5220 616e 6420 7468 6520 6072 7079 3260  R and the `rpy2`
+00001820: 2050 7974 686f 6e20 7061 636b 6167 6529   Python package)
+00001830: 0a20 0a20 2020 6060 6073 680a 2020 2054  . .   ```sh.   T
+00001840: 6573 7432 203d 2073 6d6f 6f74 6865 645f  est2 = smoothed_
+00001850: 636f 6e74 6573 745f 7265 6728 795f 6f62  contest_reg(y_ob
+00001860: 7320 3d20 6f62 732c 2078 5f6f 6273 203d  s = obs, x_obs =
+00001870: 2078 2c20 795f 6d6f 6420 3d20 6d6f 6465   x, y_mod = mode
+00001880: 6c2c 2079 5f6f 6273 5f65 7272 203d 2065  l, y_obs_err = e
+00001890: 7272 5f6f 6273 2c20 4b3d 3130 3030 2c70  rr_obs, K=1000,p
+000018a0: 6c6f 743d 5472 7565 2920 2020 0a20 2020  lot=True)   .   
+000018b0: 6060 600a 3c69 6d67 2073 7263 3d22 6874  ```.<img src="ht
+000018c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000018d0: 2f46 696f 7265 6e53 742f 436f 6e54 4553  /FiorenSt/ConTES
+000018e0: 542f 626c 6f62 2f6d 6169 6e2f 696d 672f  T/blob/main/img/
+000018f0: 536d 6f6f 7468 6564 436f 6e54 4553 5466  SmoothedConTESTf
+00001900: 6f72 5265 6772 6573 7369 6f6e 2e70 6e67  orRegression.png
+00001910: 2022 2077 6964 7468 3d38 3025 2068 6569   " width=80% hei
+00001920: 6768 743d 3830 253e 0a0a 0a23 2320 4465  ght=80%>...## De
+00001930: 6e73 6974 7920 6d6f 6465 6c73 0a0a 4372  nsity models..Cr
+00001940: 6561 7465 2073 796e 7468 6574 6963 206d  eate synthetic m
+00001950: 6f64 656c 2061 6e64 206f 6273 6572 7661  odel and observa
+00001960: 7469 6f6e 733a 0a0a 2020 2060 6060 7368  tions:..   ```sh
+00001970: 0a20 2020 6e3d 3130 300a 2020 200a 2020  .   n=100.   .  
+00001980: 2023 3144 2065 7861 6d70 6c65 0a20 2020   #1D example.   
+00001990: 6f62 7320 3d20 7374 6174 732e 6d75 6c74  obs = stats.mult
+000019a0: 6976 6172 6961 7465 5f6e 6f72 6d61 6c2e  ivariate_normal.
+000019b0: 7276 7328 6d65 616e 3d35 2c20 636f 763d  rvs(mean=5, cov=
+000019c0: 205b 312e 355d 2c73 697a 653d 6e29 0a20   [1.5],size=n). 
+000019d0: 2020 6d6f 6465 6c20 3d20 7374 6174 732e    model = stats.
+000019e0: 6d75 6c74 6976 6172 6961 7465 5f6e 6f72  multivariate_nor
+000019f0: 6d61 6c2e 7276 7328 6d65 616e 3d35 2c20  mal.rvs(mean=5, 
+00001a00: 636f 763d 205b 312e 355d 2c73 697a 653d  cov= [1.5],size=
+00001a10: 3130 3030 290a 2020 2020 0a20 2020 2332  1000).    .   #2
+00001a20: 4420 6578 616d 706c 650a 2020 206f 6273  D example.   obs
+00001a30: 5f32 6420 3d20 2073 7461 7473 2e6d 756c  _2d =  stats.mul
+00001a40: 7469 7661 7269 6174 655f 6e6f 726d 616c  tivariate_normal
+00001a50: 2e72 7673 286d 6561 6e3d 5b35 2c35 5d2c  .rvs(mean=[5,5],
+00001a60: 2063 6f76 3d20 5b5b 312e 352c 2e38 5d2c   cov= [[1.5,.8],
+00001a70: 5b2e 382c 322e 355d 5d2c 7369 7a65 3d6e  [.8,2.5]],size=n
+00001a80: 290a 2020 206d 6f64 656c 5f32 6420 3d20  ).   model_2d = 
+00001a90: 7374 6174 732e 6d75 6c74 6976 6172 6961  stats.multivaria
+00001aa0: 7465 5f6e 6f72 6d61 6c2e 7276 7328 6d65  te_normal.rvs(me
+00001ab0: 616e 3d5b 352c 355d 2c20 636f 763d 205b  an=[5,5], cov= [
+00001ac0: 5b31 2e35 2c2e 385d 2c5b 2e38 2c32 2e35  [1.5,.8],[.8,2.5
+00001ad0: 5d5d 2c73 697a 653d 3130 3030 290a 0a23  ]],size=1000)..#
+00001ae0: 2323 2043 6f6e 5445 5354 2066 6f72 206f  ## ConTEST for o
+00001af0: 7574 6c69 6572 7320 0a0a 2020 2060 6060  utliers ..   ```
+00001b00: 7368 0a20 2020 5465 7374 3320 3d20 636f  sh.   Test3 = co
+00001b10: 6e74 6573 745f 6f75 746c 6965 7273 286d  ntest_outliers(m
+00001b20: 6f64 3d6d 6f64 656c 2c20 6f62 733d 6f62  od=model, obs=ob
+00001b30: 732c 204b 3d31 3030 3030 2c20 706c 6f74  s, K=10000, plot
+00001b40: 3d54 7275 6529 0a20 2020 5465 7374 3320  =True).   Test3 
+00001b50: 3d20 636f 6e74 6573 745f 6f75 746c 6965  = contest_outlie
+00001b60: 7273 286d 6f64 3d6d 6f64 656c 5f32 642c  rs(mod=model_2d,
+00001b70: 206f 6273 3d6f 6273 5f32 642c 204b 3d31   obs=obs_2d, K=1
+00001b80: 3030 3030 2c20 706c 6f74 3d54 7275 6529  0000, plot=True)
+00001b90: 0a20 2020 6060 600a 3c69 6d67 2073 7263  .   ```.<img src
+00001ba0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00001bb0: 2e63 6f6d 2f46 696f 7265 6e53 742f 436f  .com/FiorenSt/Co
+00001bc0: 6e54 4553 542f 626c 6f62 2f6d 6169 6e2f  nTEST/blob/main/
+00001bd0: 696d 672f 436f 6e54 4553 5466 6f72 4f75  img/ConTESTforOu
+00001be0: 746c 6965 7273 3144 2e70 6e67 2022 2077  tliers1D.png " w
+00001bf0: 6964 7468 3d38 3025 2068 6569 6768 743d  idth=80% height=
+00001c00: 3830 253e 0a3c 696d 6720 7372 633d 2268  80%>.<img src="h
+00001c10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001c20: 6d2f 4669 6f72 656e 5374 2f43 6f6e 5445  m/FiorenSt/ConTE
+00001c30: 5354 2f62 6c6f 622f 6d61 696e 2f69 6d67  ST/blob/main/img
+00001c40: 2f43 6f6e 5445 5354 666f 724f 7574 6c69  /ConTESTforOutli
+00001c50: 6572 7332 442e 706e 6720 2220 7769 6474  ers2D.png " widt
+00001c60: 683d 3830 2520 6865 6967 6874 3d38 3025  h=80% height=80%
+00001c70: 3e0a 0a0a 0a23 2323 2043 6f6e 5445 5354  >....### ConTEST
+00001c80: 2066 6f72 2064 656e 7369 7469 6573 200a   for densities .
+00001c90: 0a20 2020 6060 6073 680a 2020 2054 6573  .   ```sh.   Tes
+00001ca0: 7434 203d 2063 6f6e 7465 7374 5f64 656e  t4 = contest_den
+00001cb0: 7328 6d6f 643d 6d6f 6465 6c2c 206f 6273  s(mod=model, obs
+00001cc0: 3d6f 6273 2c20 4b3d 3130 3030 302c 2070  =obs, K=10000, p
+00001cd0: 6c6f 743d 5472 7565 2920 2020 0a20 2020  lot=True)   .   
+00001ce0: 5465 7374 3420 3d20 636f 6e74 6573 745f  Test4 = contest_
+00001cf0: 6465 6e73 286d 6f64 3d6d 6f64 656c 5f32  dens(mod=model_2
+00001d00: 642c 206f 6273 3d6f 6273 5f32 642c 204b  d, obs=obs_2d, K
+00001d10: 3d31 3030 3030 2c20 706c 6f74 3d54 7275  =10000, plot=Tru
+00001d20: 6529 0a0a 2020 2060 6060 0a3c 696d 6720  e)..   ```.<img 
+00001d30: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+00001d40: 6875 622e 636f 6d2f 4669 6f72 656e 5374  hub.com/FiorenSt
+00001d50: 2f43 6f6e 5445 5354 2f62 6c6f 622f 6d61  /ConTEST/blob/ma
+00001d60: 696e 2f69 6d67 2f43 6f6e 5445 5354 666f  in/img/ConTESTfo
+00001d70: 7244 656e 7369 7469 6573 3144 2e70 6e67  rDensities1D.png
+00001d80: 2022 2077 6964 7468 3d38 3025 2068 6569   " width=80% hei
+00001d90: 6768 743d 3830 253e 0a3c 696d 6720 7372  ght=80%>.<img sr
+00001da0: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00001db0: 622e 636f 6d2f 4669 6f72 656e 5374 2f43  b.com/FiorenSt/C
+00001dc0: 6f6e 5445 5354 2f62 6c6f 622f 6d61 696e  onTEST/blob/main
+00001dd0: 2f69 6d67 2f43 6f6e 5445 5354 666f 7244  /img/ConTESTforD
+00001de0: 656e 7369 7469 6573 3244 2e70 6e67 2022  ensities2D.png "
+00001df0: 2077 6964 7468 3d38 3025 2068 6569 6768   width=80% heigh
+00001e00: 743d 3830 253e 0a0a 0a0a 0a              t=80%>.....
```

