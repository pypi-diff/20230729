# Comparing `tmp/pyphe-0.981.tar.gz` & `tmp/pyphe-0.982.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyphe-0.981.tar", last modified: Fri Feb 25 08:37:57 2022, max compression
+gzip compressed data, was "dist/pyphe-0.982.tar", last modified: Sat Jul 29 08:46:44 2023, max compression
```

## Comparing `pyphe-0.981.tar` & `pyphe-0.982.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-02-25 08:37:57.000000 pyphe-0.981/
--rw-rw-rw-   0        0        0     1088 2019-11-14 22:46:00.000000 pyphe-0.981/LICENSE
--rw-rw-rw-   0        0        0    32817 2022-02-25 08:37:57.000000 pyphe-0.981/PKG-INFO
--rw-rw-rw-   0        0        0    32247 2021-05-17 17:14:54.000000 pyphe-0.981/README.md
-drwxrwxrwx   0        0        0        0 2022-02-25 08:37:57.000000 pyphe-0.981/bin/
--rw-rw-rw-   0        0        0     3824 2020-04-13 20:53:15.000000 pyphe-0.981/bin/pyphe-analyse
--rw-rw-rw-   0        0        0     1997 2020-03-19 15:37:04.000000 pyphe-0.981/bin/pyphe-analyse-gui
--rwxrwxrwx   0        0        0      289 2020-03-29 13:15:33.000000 pyphe-0.981/bin/pyphe-analyse.bat
--rw-rw-rw-   0        0        0     3622 2022-02-24 12:09:45.000000 pyphe-0.981/bin/pyphe-growthcurves
--rwxrwxrwx   0        0        0      294 2020-03-29 13:15:32.000000 pyphe-0.981/bin/pyphe-growthcurves.bat
--rw-rw-rw-   0        0        0     4461 2020-05-29 12:05:11.000000 pyphe-0.981/bin/pyphe-interpret
--rwxrwxrwx   0        0        0      291 2020-03-29 13:15:30.000000 pyphe-0.981/bin/pyphe-interpret.bat
--rw-rw-rw-   0        0        0    10563 2022-02-24 16:52:42.000000 pyphe-0.981/bin/pyphe-quantify
--rwxrwxrwx   0        0        0      290 2020-03-29 13:15:29.000000 pyphe-0.981/bin/pyphe-quantify.bat
--rw-rw-rw-   0        0        0     2628 2021-05-17 17:14:54.000000 pyphe-0.981/bin/pyphe-scan
--rw-rw-rw-   0        0        0     2668 2021-05-17 17:14:54.000000 pyphe-0.981/bin/pyphe-scan-timecourse
-drwxrwxrwx   0        0        0        0 2022-02-25 08:37:57.000000 pyphe-0.981/pyphe/
--rw-rw-rw-   0        0        0        0 2019-11-14 22:46:00.000000 pyphe-0.981/pyphe/__init__.py
--rw-rw-rw-   0        0        0    30014 2021-03-30 11:06:37.000000 pyphe-0.981/pyphe/analysis.py
--rw-rw-rw-   0        0        0     8431 2022-02-24 14:10:27.000000 pyphe-0.981/pyphe/growthcurves.py
--rw-rw-rw-   0        0        0     6526 2021-05-17 17:14:54.000000 pyphe-0.981/pyphe/interpret.py
--rw-rw-rw-   0        0        0    16911 2021-05-17 17:14:54.000000 pyphe-0.981/pyphe/quantify.py
--rw-rw-rw-   0        0        0     6120 2021-05-17 17:14:54.000000 pyphe-0.981/pyphe/scan.py
-drwxrwxrwx   0        0        0        0 2022-02-25 08:37:57.000000 pyphe-0.981/pyphe.egg-info/
--rw-rw-rw-   0        0        0    32817 2022-02-25 08:37:57.000000 pyphe-0.981/pyphe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2022-02-25 08:37:57.000000 pyphe-0.981/pyphe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-25 08:37:57.000000 pyphe-0.981/pyphe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2022-02-25 08:37:57.000000 pyphe-0.981/pyphe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-02-25 08:37:57.000000 pyphe-0.981/pyphe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-02-25 08:37:57.000000 pyphe-0.981/setup.cfg
--rw-rw-rw-   0        0        0     1282 2022-02-25 08:37:36.000000 pyphe-0.981/setup.py
+drwxr-xr-x   0 stekam    (1000) stekam    (1000)        0 2023-07-29 08:46:44.000000 pyphe-0.982/
+-rw-r--r--   0 stekam    (1000) stekam    (1000)    36261 2023-07-29 08:46:44.000000 pyphe-0.982/PKG-INFO
+-rw-r--r--   0 stekam    (1000) stekam    (1000)    31937 2023-07-29 08:46:18.000000 pyphe-0.982/README.md
+drwxr-xr-x   0 stekam    (1000) stekam    (1000)        0 2023-07-29 08:46:44.000000 pyphe-0.982/bin/
+-rw-r--r--   0 stekam    (1000) stekam    (1000)     3943 2023-07-29 08:46:18.000000 pyphe-0.982/bin/pyphe-analyse
+-rw-r--r--   0 stekam    (1000) stekam    (1000)     1997 2023-07-29 08:46:18.000000 pyphe-0.982/bin/pyphe-analyse-gui
+-rw-r--r--   0 stekam    (1000) stekam    (1000)      277 2023-07-29 08:46:18.000000 pyphe-0.982/bin/pyphe-analyse.bat
+-rw-r--r--   0 stekam    (1000) stekam    (1000)     3622 2023-07-29 08:46:18.000000 pyphe-0.982/bin/pyphe-growthcurves
+-rw-r--r--   0 stekam    (1000) stekam    (1000)      282 2023-07-29 08:46:18.000000 pyphe-0.982/bin/pyphe-growthcurves.bat
+-rw-r--r--   0 stekam    (1000) stekam    (1000)     4461 2023-07-29 08:46:18.000000 pyphe-0.982/bin/pyphe-interpret
+-rw-r--r--   0 stekam    (1000) stekam    (1000)      279 2023-07-29 08:46:18.000000 pyphe-0.982/bin/pyphe-interpret.bat
+-rw-r--r--   0 stekam    (1000) stekam    (1000)    10563 2023-07-29 08:46:18.000000 pyphe-0.982/bin/pyphe-quantify
+-rw-r--r--   0 stekam    (1000) stekam    (1000)      278 2023-07-29 08:46:18.000000 pyphe-0.982/bin/pyphe-quantify.bat
+-rw-r--r--   0 stekam    (1000) stekam    (1000)     2628 2023-07-29 08:46:18.000000 pyphe-0.982/bin/pyphe-scan
+-rw-r--r--   0 stekam    (1000) stekam    (1000)     2668 2023-07-29 08:46:18.000000 pyphe-0.982/bin/pyphe-scan-timecourse
+drwxr-xr-x   0 stekam    (1000) stekam    (1000)        0 2023-07-29 08:46:44.000000 pyphe-0.982/pyphe/
+-rw-r--r--   0 stekam    (1000) stekam    (1000)        0 2023-07-29 08:46:18.000000 pyphe-0.982/pyphe/__init__.py
+-rw-r--r--   0 stekam    (1000) stekam    (1000)    29726 2023-07-29 08:46:18.000000 pyphe-0.982/pyphe/analysis.py
+-rw-r--r--   0 stekam    (1000) stekam    (1000)     8261 2023-07-29 08:46:18.000000 pyphe-0.982/pyphe/growthcurves.py
+-rw-r--r--   0 stekam    (1000) stekam    (1000)     6375 2023-07-29 08:46:18.000000 pyphe-0.982/pyphe/interpret.py
+-rw-r--r--   0 stekam    (1000) stekam    (1000)    16493 2023-07-29 08:46:18.000000 pyphe-0.982/pyphe/quantify.py
+-rw-r--r--   0 stekam    (1000) stekam    (1000)     5974 2023-07-29 08:46:18.000000 pyphe-0.982/pyphe/scan.py
+drwxr-xr-x   0 stekam    (1000) stekam    (1000)        0 2023-07-29 08:46:44.000000 pyphe-0.982/pyphe.egg-info/
+-rw-r--r--   0 stekam    (1000) stekam    (1000)    36261 2023-07-29 08:46:43.000000 pyphe-0.982/pyphe.egg-info/PKG-INFO
+-rw-r--r--   0 stekam    (1000) stekam    (1000)      510 2023-07-29 08:46:44.000000 pyphe-0.982/pyphe.egg-info/SOURCES.txt
+-rw-r--r--   0 stekam    (1000) stekam    (1000)        1 2023-07-29 08:46:43.000000 pyphe-0.982/pyphe.egg-info/dependency_links.txt
+-rw-r--r--   0 stekam    (1000) stekam    (1000)       64 2023-07-29 08:46:43.000000 pyphe-0.982/pyphe.egg-info/requires.txt
+-rw-r--r--   0 stekam    (1000) stekam    (1000)        6 2023-07-29 08:46:43.000000 pyphe-0.982/pyphe.egg-info/top_level.txt
+-rw-r--r--   0 stekam    (1000) stekam    (1000)       38 2023-07-29 08:46:44.000000 pyphe-0.982/setup.cfg
+-rw-r--r--   0 stekam    (1000) stekam    (1000)     1245 2023-07-29 08:46:18.000000 pyphe-0.982/setup.py
```

### Comparing `pyphe-0.981/PKG-INFO` & `pyphe-0.982/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,491 +1,474 @@
-Metadata-Version: 2.1
-Name: pyphe
-Version: 0.981
-Summary: Python toolbox for phenotype analysis of arrayed microbial colonies
-Home-page: https://github.com/Bahler-Lab/pyphe
-Author: Stephan Kamrad
-Author-email: stephan.kamrad@crick.ac.uk
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![pyphe logo](https://github.com/Bahler-Lab/pyphe/blob/master/icons/toolbox-72dpi_white.png)
-
-# Welcome to the pyphe toolbox
-A python toolbox for phenotype analysis of arrayed microbial colonies written by Stephan Kamrad (stephan.kamrad at crick.ac.uk).
-
-For a quick overview, please see our [10 minute video tutorial](https://www.youtube.com/watch?v=lQ3lXIdhA1c&t=5s).
-
-For a more detailed protocol, including growth curves and viability assays, please see our [protocol preprint](https://www.researchsquare.com/article/rs-401914/v1).
-
-For more background information, please see our [_eLife_ paper](https://elifesciences.org/articles/55160).
-
-Please cite as:
-> Kamrad, S., RodrÃ­guez-LÃ³pez, M., Cotobal, C., Correia-Melo, C., Ralser M., BÃ¤hler J. (2020). Pyphe, a python toolbox for assessing microbial growth and cell viability in high-throughput colony screens. eLife 9:e55160
-
-## Installation
-1. Most tools are cross-platform compatible but scanning will only work on a Linux OS. The scanners need to be accessible by [SANE](http://www.sane-project.org/) and [ImageMagick](https://imagemagick.org/) needs to be installed and accessible from the command line.
-2. Pyphe requires Python 3 and a few common packages, available through the [anaconda distribution](https://www.anaconda.com/distribution/).
-3. Install pyphe by running 'pip install pyphe' in your terminal.
-4. Open a new terminal and try and run 'pyphe-quantify -h' which should show the help page of one of pyphe's command line tools. On Windows, make sure you are using the Anaconda Prompt, not the Anaconda Powershell Prompt.
-
-
-## Overview
-A typical fitness screen with pyphe will involve:
-1. Image acquisition with [_pyphe-scan_](#pyphe-scan), or [_pyphe-scan-timecourse_](#pyphe-scan-timecourse)
-2. Quantification of colony properties from images using [_pyphe-quantify_](#pyphe-quantify). In the case of growth curves, parameters are additionally extracted with [_pyphe-growthcurves_](#pyphe-growthcurves).
-3. Normalisation and data aggregation using [_pyphe-analyse_](#pyphe-analyse).
-4. Statistics and hit calling using [_pyphe-interpret_](#pyphe-interpret)
-Please see our paper for a detailed protocol and explanations of the algorithms.
-
-
-## Support
-Please check the manuals below carefully, they are also available in the terminal by running the command with the -h option only. If things are still not working, please email me (stephan.kamrad@crick.ac.uk) and I will try and help. If you think you have discovered a bug, or would like to request a new feature, please raise an issue on www.github.com/Bahler-Lab/pyphe.
-
-If you get an error like this, make sure you are not using the Anaconda Powershell Prompt:
-```python: can't open file 'C:\Users\user1\Anaconda3\Scripts"C:\Users\user1\Anaconda3\Scripts\pyphe-quantify.bat  -h ': [Errno 22] Invalid argument```
-
-## Manual
-
-All pyphe tools have a similar command line interface, based on the python argparse package. Generally, parameters are set using --<parameter_name> optionally followed by a value. All _pyphe_ tools can be used with relative file paths so make sure to navigate to the correct working directory before running a _pyphe_ command.
-
- 
-### Pyphe-scan
-This tools allows you to take consecutive scans of sets of plates, which are then automatically cropped, rotated and named in in a continuos filename scheme of your choice. 
-
-#### Prerequisites
-1. This tool will only run on Linux operating systems and uses the SANE library for image acquisition.
-
-2. Make sure your scanner is installed correctly and you can acquire images using the scanimage command. The Gray mode will only work on Epson V800 and V850 scanners (potentially the V700 and V750 model as well) and the TPU8x10 transmission scanning source must be enabled. This should work by default if you are using the V800/850 model and a recent Linux OS. Otherwise, there is excellent documentation available from Zackrisson et al. and the [scanomatics pipeline](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5015956/) for how to make this work using a hacked SANE driver. Please see the instructions in their [wiki](https://github.com/Scan-o-Matic/scanomatic/wiki/Installing-scanners).
-
-2. Make sure [ImageMagick](https://imagemagick.org/index.php) is installed and the 'convert' tool can be called from the command line.
-
-3. If the Pyphe toolbox has been installed correctly, you should be able to run _pyphe-scan_ in your terminal. 
-
-4. With a laser cutter, make a fixture to hold your plates in place. We provide an svg file with the cutting shape in the Documentation directory. Use tape to hold your fixture into place, it should be pushed against the back of the scanner (where the cables are) with the top of the plates facing left. Pyphe-scan and pyphe-quantify come pre-configured for using the provided fixture on an Epson V800/V850 scanner but it is easy to add your own fixture and cropping settings. If you want to use your own fixture, see below of how to add the geometry information to pyphe-scan. 
-
-#### Scanning plate batches
-
-1. Open the file manager and navigate to the folder in which you want to save your images. The script will create a sub-folder that begins with the current date to save all your images. 
-
-2. Right click and select 'Open in Terminal'
-
-3. Run scanplates with the options as detaild below. 
-
-```
-usage: pyphe-scan [-h] [--nplates NPLATES] [--start START] [--prefix PREFIX]
-                  [--postfix POSTFIX] [--fixture {som3_edge,som3}]
-                  [--resolution {150,300,600,900,1200}] [--scanner {1,2,3}]
-                  [--mode {Gray,Color}]
-
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --nplates NPLATES     Number of plates to scan. This defaults to 100 and the
-                        script can be terminated by Ctr+C when done.
-  --start START         Where to start numbering from. Defaults to 1.
-  --prefix PREFIX       Name prefix for output files. The default is the
-                        current date YYYYMMDD.
-  --postfix POSTFIX     Name postfix for output files. Defaults to empty
-                        string.
-  --fixture {som3_edge,som3,som3-color}
-                        ID of the fixture you are using.
-  --resolution {150,300,600,900,1200}
-                        Resolution for scanning in dpi. Default is 600.
-  --scanner {1,2,3}     Which scanner to use. Scanners are not uniquely
-                        identified and may switch when turned off/unplugged.
-                        This option does not need to be set when only one
-                        scanner is connected.
-  --mode {Gray,Color}   Which color mode to use for scanning. Defaults to
-                        Gray.
-```
-
-All arguments except the fixture have default values and are optional. A folder prefix_postfix will be created in your current directory and the program will abort if a folder with this name already exists. 
-
-
-
-### Pyphe-scan-timecourse
-
-This tool acquires image timeseries by scanning in fixed time intervals. For each position in the fixture, a folder is created. Image names contain number of scan. Other options for this tool are similar to [_pyphe-scan_](#pyphe-scan). More than one scanner can be connected and used at the same time. Scanner numbers are defined by the order in which they are connected to the computer. Proceed as follows: (1) disconnect all scanners, (2) prepare the first scanner with plates, connect it and turn it on. (3) start scanning with --scanner 1 option, (4) prepare the second scanner, connect it and turn it on, (5) start scanning with --scanner 2 option. Repeat step (4) and (5), each time incrementing the --scanner argument. 
-
-```
-usage: pyphe-scan-timecourse [-h] [--nscans NSCANS] [--interval INTERVAL]
-                             [--prefix PREFIX] [--postfix POSTFIX]
-                             [--fixture {som3_edge,som3}]
-                             [--resolution {150,300,600,900,1200}]
-                             [--scanner {1,2,3}] [--mode {Gray,Color}]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --nscans NSCANS       Number of time points to scan. This defaults to 100
-                        and the script can be terminated by Ctr+C when done.
-  --interval INTERVAL   Time in minutes between scans. Defaults to 20.
-  --prefix PREFIX       Name prefix for output files. The default is the
-                        current date YYYYMMDD.
-  --postfix POSTFIX     Name postfix for output files. Defaults to empty
-                        string.
-  --fixture {som3_edge,som3,som3-color}
-                        ID of the fixture you are using.
-  --resolution {150,300,600,900,1200}
-                        Resolution for scanning in dpi. Default is 600.
-  --scanner {1,2,3}     Which scanner to use. Scanners are not uniquely
-                        identified and may switch when turned off/unplugged.
-                        This option does not need to be set when only one
-                        scanner is connected.
-  --mode {Gray,Color}   Which color mode to use for scanning. Defaults to
-                        Gray.
-```
-
-
-### Pyphe-growthcurves
-This tool performs non-parametric analysis of growth curves. It was written specifically to analyse colony size timeseries data obtained with _pyphe-quantify_ _timeseries_.
-
-It is important that your csv with the growth data is in the right format. The file must contain one growth curve per column. The first column must be the timepoints and there must be a header row with unique identifiers for each curve. For example data and expected outputs, check out the files included in this Documentation folder. Sensible default parameters are set for all options but, depending on your data, you may wish to customise these, so check out the help section below. 
-
-```
-usage: pyphe-growthcurves [-h] --input INPUT [--fitrange FITRANGE]
-                          [--lag-method {abs,rel}]
-                          [--lag-threshold LAG_THRESHOLD]
-                          [--t0-fitrange T0_FITRANGE] [--plots]
-                          [--plot-ylim PLOT_YLIM]
-
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --input INPUT         Path to the growth curve file to analyse. This file
-                        contains one growth curve per column. The first column
-                        must be the timepoints and there must be a header row
-                        with unique identifiers for each curve.
-  --fitrange FITRANGE   Number of timepoint over which to fit linear
-                        regression. Defaults to 4. Please adjust this to the
-                        density of your timepoints and use higher values for
-                        more noisy data.
-  --lag-method {abs,rel}
-                        Method to use for determining lag. "abs" will measure
-                        time until the defined biomass threshold is crossed.
-                        "rel" will fist determine the inital biomass and
-                        measure the time until the biomass has passed this
-                        value times the threshold. Defaults to "rel".
-  --lag-threshold LAG_THRESHOLD
-                        Threshold to use for determining lag. With method
-                        "abs", this will measure time until the defined
-                        biomass threshold is crossed. With "rel" will fist
-                        determine the inital biomass and measure the time
-                        until the biomass has passed this value times the
-                        threshold. Defaults to 2.0, so with method "rel", this
-                        will measure the time taken for the first doubling.
-  --t0-fitrange T0_FITRANGE
-                        Specify the number of timepoint to use at the
-                        beginning of the growth curve to determine the initial
-                        biomass by averaging them. Defaults to 3.
-  --plots               Set this option (no argument required) to produce a
-                        plot of all growthcurves as pdf.
-  --plot-ylim PLOT_YLIM
-                        Specify the upper limit of the y-axis of growth curve
-                        plots. Useful if you want curves to be directly
-                        comparable. If not set, the axis of each curve is
-                        scaled to the data.
-```
-
-
-#### Interpreting results
-Pyphe-growthcurves will produce a csv file with extracted growth parameters. The maximum slope is determined by fitting all possible linear regressions in sliding windows of length n and chosing the one with the highest slope. The lag phase is determined as the first timepoint which exceeds a settable relative or absolute threshold. 
-
-| Parameter        | Explanation  |
-| ---------------- |---------------|
-|initial biomass|The average of the first n timepoints of the growth curve|
-|lag |  Lag phase |
-| max_slope| The maximum slope of the growth curve|
-| r2 | The R2 parameter of the linear regression that produced the highest maximum slope |
-|t_max | Time at which maximum growth slope is reached (center of the sliding window)|
-|y-intercept|Y-intercept of the regression which produced the maximum slope|
-|x-intercept|X-intercept of the regression which produced the maximum slope. This is interpreted as lag phase by some people|
-
-                            
-
-### Pyphe-quantify
-
-Pyphe quantify extracts colony parameters from images. In can operate in three distinct modes analysing colony sizes for each image individually (batch mode), analysing redness for each image individually (redness mode) or obtaining a growth curve from an image timeseries (timeseries mode).
-The --grid parameter is required define the position of colonies on the plate. You can either use automatic grid detection, one of our preconfigured positions if you are using the pp3 fixture or define your own (see the manual below). Images can be in any format (e.g. jpg, tiff, png). Images should be cropped closely to the colonies (this is important for good thresholding and automatic grid detection), i.e. not contain parts of the plate edges or surroundings. In batch and timecourse mode, pyphe-quantify assumes that images were acquired using transmission scanning, where colonies appear darker then the surrounding agar. If this is not the case and you took images by reflective scanning or with a camera, use --negate False. In batch and timecourse mode, images are epxected to be grayscale. If they are not, they will be converted (by simply summing all channels) and a warning will be thrown. 
-
-
-```
-usage: pyphe-quantify [-h] --grid GRID [--pattern PATTERN] [--t T] [--d D]
-                      [--s S] [--negate NEGATE] [--localThresh] [--convexhull]
-                      [--reportAll] [--reportFileNames]
-                      [--hardImageThreshold HARDIMAGETHRESHOLD]
-                      [--hardSizeThreshold HARDSIZETHRESHOLD] [--qc QC]
-                      [--calibrate CALIBRATE] [--timepoints TIMEPOINTS]
-                      [--out OUT]
-                      {batch,timecourse,redness}
-
-Welcome to pyphe-quantify, part of the pyphe toolbox. Written by
-stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
-Lab/pyphe
-
-positional arguments:
-  {batch,timecourse,redness}
-                        Pyphe-quantify can be run in three different modes. In
-                        batch mode, it quantifies colony sizes for all images
-                        matching the pattern individually. A separate results
-                        table and qc image is produced for each. Redness mode
-                        is similar except that the redness of each colony is
-                        quantified. In timecourse mode, all images matching
-                        the pattern are analysed jointly. The final image
-                        matching the pattern is used to create a mask of where
-                        the colonies are and this mask is then applied to all
-                        previous images in the timeseries. A single output
-                        table, where the timepoints are the rows and each
-                        individual colony is a row.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --grid GRID           This option is required (all others have defaults set)
-                        and specifies the grid in which the colonies are
-                        arranged. You can use automatic grid detection using
-                        one of the following parameters: auto_96, auto_384 or
-                        auto_1536. Automatic grid correction will not work if
-                        the colony grid is not aligned with the image borders.
-                        Images should contain only agar and colonies, avaoid
-                        having borders. It might fail or produce unexpected
-                        results if there are whole rows/columns missing. In
-                        those cases, it is easy to define hard-wired grid
-                        positions. If you are using the fixture provided with
-                        pyphe, we have preconfigured these for you. Depending
-                        on the pinning density, use pp3_96, pp3_384 or
-                        pp3_1536. Otherwise, the argument has to be in the
-                        form of 6 integer numbers separated by "-": <number of
-                        colony rows>-<number of colony columns>-<x-position of
-                        the top left colony>-<y-position of the top left
-                        colony>-<x-position of the bottom right
-                        colony>-<y-position of the bottom right colony>.
-                        Positions must be integers and are the distance in
-                        number of pixels from the image origin in each
-                        dimension (x is width dimension, y is height
-                        dimension). The image origin is, in line with scikit-
-                        image, in the top left corner. Pixel positions are
-                        easily determined using programs such as Microsoft
-                        Paint, by simply hovering the mouse over a position.
-  --pattern PATTERN     Pattern describing files to analyse. This follows
-                        standard unix convention and can be used to specify
-                        subfolders in which to look for images
-                        (<subfolder>/*.jpg) or the image format (*.tiff,
-                        *.png, etc.). By default, all jpg images in the
-                        working directory are analysed.
-  --t T                 By default the intensity threshold to distinguish
-                        colonies from the background is determined by the Otsu
-                        method. The determined value will be multiplied by
-                        this argument to give the final threshold. Useful for
-                        easily fine-tuning colony detection.
-  --d D                 The distance between two grid positions will be
-                        divided by this number to compute the maximum distance
-                        a putative colony can be away from its reference grid
-                        position. Decreasing this number towards 2 makes
-                        colony-to-grid-matching more permissive (might help
-                        when some of your plates are at a slight angle or out
-                        of position).
-  --s S                 Detected putative colonies will be filtered by size
-                        and small components (usually image noise) will be
-                        excluded. The default threshold is the image
-                        area*0.00005 and is therefore independent of scanning
-                        resolution. This default is then multiplied by this
-                        argument to give the final threshold. Useful for when
-                        colonies have unusual sizes.
-  --negate NEGATE       In images acquired by transmission scanning, the
-                        colonies are darker than the background. Before
-                        thresholding, the image needs to be inverted/negated.
-                        Defaults to True in timecourse and batch mode, ignored
-                        in redness mode.
-  --localThresh         Use local thresholding in batch and timecourse mode.
-                        This can help when image brightness is very uneven.
-                        Ignored in redness mode where local thresholding is
-                        always applied.
-  --convexhull          Apply convex hull transformation to identified
-                        colonies to fill holes. Useful when working with spots
-                        rather than colonies. Ignored in redness mode.
-                        WARNING: Using this options results in much longer
-                        analysis times.
-  --reportAll           Sometimes, two putative colonies are identified that
-                        are within the distance threshold of a grid position.
-                        By default, only the closest colony is reported. This
-                        can be changed by setting this option (without
-                        parameter). This option allows pyphe quantify to be
-                        used even if colonies are not arrayed in a regular
-                        grid (you still need to provide a grid parameter
-                        though that spans the colonies you are interested i).
-  --reportFileNames     Only for timecourse mode, otherwise ignored. Use
-                        filenames as index for output table instead of
-                        timepoints. Useful when the ordering of timepoints is
-                        not the same as returned by the pattern. Setting this
-                        option overrides the --timepoints argument.
-  --hardImageThreshold HARDIMAGETHRESHOLD
-                        Allows a hard (fixed) intensity threshold in the range
-                        [0,1] to be used instead of Otsu thresholding. Images
-                        intensities are re-scaled to [0,1] before
-                        thresholding. Ignored in timecourse mode.
-  --hardSizeThreshold HARDSIZETHRESHOLD
-                        Allows a hard (fixed) size threshold [number of
-                        pixels] to be used for filtering small colonies.
-  --qc QC               Directory to save qc images in. Defaults to
-                        "qc_images".
-  --calibrate CALIBRATE
-                        Transform background subtracted intensity values by
-                        this function. Function needs to be a single term with
-                        x as the variable and that is valid python code. E.g.
-                        use "2*x**2+1" to square each pixels intensity,
-                        multiply by two and add 1. Defaults to "x", i.e. use
-                        of no calibration. Used only in timecourse mode.
-  --timepoints TIMEPOINTS
-                        In timecourse mode only. Path to a file that specifies
-                        the timepoints of all images in the timeseries. This
-                        is usually the timepoints.txt file created by pyphe-
-                        scan-timecourse. It must contain one entry per line
-                        and have the same number of lines as number of images.
-  --out OUT             Directory to save output files in. Defaults to
-                        "pyphe_quant".
-```
-
-
-
-### Pyphe-analyse
-_Pyphe-analyse_ is a tool for spatial normalisation and data aggregation across many plates. It implements a grid normalisation based on the concept proposed by [Zackrisson et al. 2016](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5015956/) and row/column median normalisation. Please see our paper and the protocol in it to find out more. _Pyphe-analyse_ can be run from the command line, with options below, or using the graphical user interface by running _pyphe-analyse-gui_.
-
-
-```
-usage: pyphe-analyse.txt [-h] --edt EDT --format
-                         {gitter,pyphe-redness,pyphe-growthcurves} [--out OUT]
-                         [--load_layouts]
-                         [--gridnorm {standard384,standard1536}]
-                         [--extrapolate_corners] [--rcmedian] [--check CHECK]
-                         [--qc_plots QC_PLOTS]
-
-Welcome to pyphe-analyse, part of the pyphe toolbox. Written by
-stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
-Lab/pyphe
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --edt EDT             Path to the Experimental Design Table (EDT) listing
-                        all plates of the experiment. The table must be in csv
-                        format, the first column must contain unique plate IDs
-                        and there must be a column named 'Data_path' that
-                        contains abolute or relative file paths to each
-                        plate's data file. A 'Layout_path' column can be
-                        included, see below. Any additional columns included
-                        in this file will bestored in each plate's meta-data
-                        and included in the final data output.
-  --format {gitter,pyphe-redness,pyphe-growthcurves}
-                        Type of inout data.
-  --out OUT             Specifies the path where to save the output data
-                        result. By default, the data report is saved in the
-                        working directory as "pyphe-analyse_data_report.csv"
-                        and will overwrite the file if it exists.
-  --load_layouts        Set this option (without parameters) to load layouts
-                        (requires Layout_path column in the EDT).
-  --gridnorm {standard384,standard1536}
-                        Perform reference grid normalisation. Standard384
-                        refers to plates which are in 384 (16x24) format with
-                        the reference grid in 96 format in the top left
-                        corner. Standard1536 refers to plates in 1536 format
-                        (32x48( with two 96 reference grids in the top left
-                        and bottom right corners.
-  --extrapolate_corners
-                        If working in standard1536 format, set this option to
-                        extrapolate the reference grid in the bottom left and
-                        top right corner. A linear regression will be trained
-                        across all top left and bottom right corners on plates
-                        in the experiment to predict hypothetical grid colony
-                        sizes in the other two corners.
-  --rcmedian            Perform row/column median normalisation. If --gridnorm
-                        will be performed first if both parameters are set.
-  --check CHECK         Check colony sizes after normalisation for negative
-                        and infinite colony sizes *(normalisation artefacts),
-                        throw a warning and set to NA.
-  --qc_plots QC_PLOTS   Specify a folder in which to save qc plots for each
-                        plate.
-
-```
-
-
-### Pyphe-interpret
-
-Pyphe-interpret reports summary statistics and tests for differential fitness using t-tests. It is flexible and can in theory be used with any dataset in tidy format.
-
-```
-usage: pyphe-interpret [-h] --ld LD [--out OUT] --grouping_column
-                       GROUPING_COLUMN --axis_column AXIS_COLUMN
-                       [--values_column VALUES_COLUMN] --control CONTROL
-                       [--ld_encoding LD_ENCODING] [--circularity CIRCULARITY]
-                       [--set_missing_na]
-
-Welcome to pyphe-interpret, part of the pyphe toolbox. Written by
-stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
-Lab/pyphe. Pyphe-interpret calculates summary statistics and p-values from the
-data reports generated by pyphe-analyse. For this, specifiying your column
-names correctly is crucial. Let us assume you have measured many strains in
-many conditions. Now you would like to know for each strain in each condition
-(for each condition-strain pair) if it is "significant". There are essentially
-two ways of doing this, asking different biological questions. (1) Check for
-each condition separately (--grouping_column <condition_column>) if there is a
-significant difference in means between a mutant strain and a control strain
-(--axis_column <strain_id_column>). Or (2) Check for each strain separately
-(--grouping_column <strain_id_column>) if there is a significant difference in
-the means of the strain in the assay condition versus the control condition
-(--axis_column <condition_column>). The second option tests for condition-
-specific growth effects (i.e. is does not return significant results if a
-strain is always faster or always slower growing than the grid strain). In
-both cases you need to specify the control against which to test using
---control and this has to be a value that appears in the axis column. You
-should define the dependent variable of the t-test using --values_column. FDR
-correction with the Benjamini-Hochberg method will be applied on each level
-set of the grouping_column separately, ie for case (1) p-values will be
-corrected across each strain separately, ie more conditions means more
-stringent correction, and for case (2) p-values will be corrected for each
-condition separately, ie more strains means mpre stringent correction.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --ld LD               Path to the Data Report Table produced by pyphe-
-                        analyse.
-  --out OUT             Specifies the path where to save the output data
-                        result. By default, a table with all replicates will
-                        be saved as pyphe-interpret-report_reps.csv and the
-                        statistic table will be saved as pyphe-interpret-
-                        report_summaryStats.csv in the current working
-                        directory. Existing files will be overwritten.
-  --grouping_column GROUPING_COLUMN
-                        Name of the column in the data report to use for
-                        forming groups on which to perform independent sets of
-                        t-tests.
-  --axis_column AXIS_COLUMN
-                        Name of the column in the data report to repeat
-                        t-tests along within each group. Levels in this column
-                        will be the explanatory/independent variable used for
-                        t-tests.
-  --values_column VALUES_COLUMN
-                        Name of the column in the data report to use as
-                        fitness values. This will be the dependent variable
-                        for t-tests. Defaults to "Colony_size_corr_checked".
-  --control CONTROL     Name of the control to compare against. This must be a
-                        value found in the axis column.
-  --ld_encoding LD_ENCODING
-                        Encoding of the data report table to be passed to
-                        pandas.read_csv().
-  --circularity CIRCULARITY
-                        Exclude colonies from the analysis with a circularity
-                        below the one specified. A circularity of 1
-                        corresponds to a perfect circle. We recommend a
-                        threshold around 0.85.
-  --set_missing_na      Set 0-sized colonies to NA. This is recommended if you
-                        expect no missing colonies in your data, which means
-                        these are probably due to pinning errors.
-```
-
-
-
+![pyphe logo](https://github.com/Bahler-Lab/pyphe/blob/master/icons/toolbox-72dpi_white.png)
+
+# Welcome to the pyphe toolbox
+A python toolbox for phenotype analysis of arrayed microbial colonies written by Stephan Kamrad (stephan.kamrad at crick.ac.uk).
+
+For a quick overview, please see our [10 minute video tutorial](https://www.youtube.com/watch?v=lQ3lXIdhA1c&t=5s).
+
+For a more detailed protocol, including growth curves and viability assays, please see our [protocol preprint](https://www.researchsquare.com/article/rs-401914/v1).
+
+For more background information, please see our [_eLife_ paper](https://elifesciences.org/articles/55160).
+
+Please cite as:
+> Kamrad, S., Rodríguez-López, M., Cotobal, C., Correia-Melo, C., Ralser M., Bähler J. (2020). Pyphe, a python toolbox for assessing microbial growth and cell viability in high-throughput colony screens. eLife 9:e55160
+
+## Installation
+1. Most tools are cross-platform compatible but scanning will only work on a Linux OS. The scanners need to be accessible by [SANE](http://www.sane-project.org/) and [ImageMagick](https://imagemagick.org/) needs to be installed and accessible from the command line.
+2. Pyphe requires Python 3 and a few common packages, available through the [anaconda distribution](https://www.anaconda.com/distribution/).
+3. Install pyphe by running 'pip install pyphe' in your terminal.
+4. Open a new terminal and try and run 'pyphe-quantify -h' which should show the help page of one of pyphe's command line tools. On Windows, make sure you are using the Anaconda Prompt, not the Anaconda Powershell Prompt.
+
+
+## Overview
+A typical fitness screen with pyphe will involve:
+1. Image acquisition with [_pyphe-scan_](#pyphe-scan), or [_pyphe-scan-timecourse_](#pyphe-scan-timecourse)
+2. Quantification of colony properties from images using [_pyphe-quantify_](#pyphe-quantify). In the case of growth curves, parameters are additionally extracted with [_pyphe-growthcurves_](#pyphe-growthcurves).
+3. Normalisation and data aggregation using [_pyphe-analyse_](#pyphe-analyse).
+4. Statistics and hit calling using [_pyphe-interpret_](#pyphe-interpret)
+Please see our paper for a detailed protocol and explanations of the algorithms.
+
+
+## Support
+Please check the manuals below carefully, they are also available in the terminal by running the command with the -h option only. If things are still not working, please email me (stephan.kamrad@gmail.com) and I will try and help. If you think you have discovered a bug, or would like to request a new feature, please raise an issue on www.github.com/Bahler-Lab/pyphe.
+
+If you get an error like this, make sure you are not using the Anaconda Powershell Prompt:
+```python: can't open file 'C:\Users\user1\Anaconda3\Scripts"C:\Users\user1\Anaconda3\Scripts\pyphe-quantify.bat  -h ': [Errno 22] Invalid argument```
+
+## Manual
+
+All pyphe tools have a similar command line interface, based on the python argparse package. Generally, parameters are set using --<parameter_name> optionally followed by a value. All _pyphe_ tools can be used with relative file paths so make sure to navigate to the correct working directory before running a _pyphe_ command.
+
+ 
+### Pyphe-scan
+This tools allows you to take consecutive scans of sets of plates, which are then automatically cropped, rotated and named in in a continuos filename scheme of your choice. 
+
+#### Prerequisites
+1. This tool will only run on Linux operating systems and uses the SANE library for image acquisition.
+
+2. Make sure your scanner is installed correctly and you can acquire images using the scanimage command. The Gray mode will only work on Epson V800 and V850 scanners (potentially the V700 and V750 model as well) and the TPU8x10 transmission scanning source must be enabled. This should work by default if you are using the V800/850 model and a recent Linux OS. Otherwise, there is excellent documentation available from Zackrisson et al. and the [scanomatics pipeline](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5015956/) for how to make this work using a hacked SANE driver. Please see the instructions in their [wiki](https://github.com/Scan-o-Matic/scanomatic/wiki/Installing-scanners).
+
+2. Make sure [ImageMagick](https://imagemagick.org/index.php) is installed and the 'convert' tool can be called from the command line.
+
+3. If the Pyphe toolbox has been installed correctly, you should be able to run _pyphe-scan_ in your terminal. 
+
+4. With a laser cutter, make a fixture to hold your plates in place. We provide an svg file with the cutting shape in the Documentation directory. Use tape to hold your fixture into place, it should be pushed against the back of the scanner (where the cables are) with the top of the plates facing left. Pyphe-scan and pyphe-quantify come pre-configured for using the provided fixture on an Epson V800/V850 scanner but it is easy to add your own fixture and cropping settings. If you want to use your own fixture, see below of how to add the geometry information to pyphe-scan. 
+
+#### Scanning plate batches
+
+1. Open the file manager and navigate to the folder in which you want to save your images. The script will create a sub-folder that begins with the current date to save all your images. 
+
+2. Right click and select 'Open in Terminal'
+
+3. Run scanplates with the options as detaild below. 
+
+```
+usage: pyphe-scan [-h] [--nplates NPLATES] [--start START] [--prefix PREFIX]
+                  [--postfix POSTFIX] [--fixture {som3_edge,som3}]
+                  [--resolution {150,300,600,900,1200}] [--scanner {1,2,3}]
+                  [--mode {Gray,Color}]
+
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --nplates NPLATES     Number of plates to scan. This defaults to 100 and the
+                        script can be terminated by Ctr+C when done.
+  --start START         Where to start numbering from. Defaults to 1.
+  --prefix PREFIX       Name prefix for output files. The default is the
+                        current date YYYYMMDD.
+  --postfix POSTFIX     Name postfix for output files. Defaults to empty
+                        string.
+  --fixture {som3_edge,som3,som3-color}
+                        ID of the fixture you are using.
+  --resolution {150,300,600,900,1200}
+                        Resolution for scanning in dpi. Default is 600.
+  --scanner {1,2,3}     Which scanner to use. Scanners are not uniquely
+                        identified and may switch when turned off/unplugged.
+                        This option does not need to be set when only one
+                        scanner is connected.
+  --mode {Gray,Color}   Which color mode to use for scanning. Defaults to
+                        Gray.
+```
+
+All arguments except the fixture have default values and are optional. A folder prefix_postfix will be created in your current directory and the program will abort if a folder with this name already exists. 
+
+
+
+### Pyphe-scan-timecourse
+
+This tool acquires image timeseries by scanning in fixed time intervals. For each position in the fixture, a folder is created. Image names contain number of scan. Other options for this tool are similar to [_pyphe-scan_](#pyphe-scan). More than one scanner can be connected and used at the same time. Scanner numbers are defined by the order in which they are connected to the computer. Proceed as follows: (1) disconnect all scanners, (2) prepare the first scanner with plates, connect it and turn it on. (3) start scanning with --scanner 1 option, (4) prepare the second scanner, connect it and turn it on, (5) start scanning with --scanner 2 option. Repeat step (4) and (5), each time incrementing the --scanner argument. 
+
+```
+usage: pyphe-scan-timecourse [-h] [--nscans NSCANS] [--interval INTERVAL]
+                             [--prefix PREFIX] [--postfix POSTFIX]
+                             [--fixture {som3_edge,som3}]
+                             [--resolution {150,300,600,900,1200}]
+                             [--scanner {1,2,3}] [--mode {Gray,Color}]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --nscans NSCANS       Number of time points to scan. This defaults to 100
+                        and the script can be terminated by Ctr+C when done.
+  --interval INTERVAL   Time in minutes between scans. Defaults to 20.
+  --prefix PREFIX       Name prefix for output files. The default is the
+                        current date YYYYMMDD.
+  --postfix POSTFIX     Name postfix for output files. Defaults to empty
+                        string.
+  --fixture {som3_edge,som3,som3-color}
+                        ID of the fixture you are using.
+  --resolution {150,300,600,900,1200}
+                        Resolution for scanning in dpi. Default is 600.
+  --scanner {1,2,3}     Which scanner to use. Scanners are not uniquely
+                        identified and may switch when turned off/unplugged.
+                        This option does not need to be set when only one
+                        scanner is connected.
+  --mode {Gray,Color}   Which color mode to use for scanning. Defaults to
+                        Gray.
+```
+
+
+### Pyphe-growthcurves
+This tool performs non-parametric analysis of growth curves. It was written specifically to analyse colony size timeseries data obtained with _pyphe-quantify_ _timeseries_.
+
+It is important that your csv with the growth data is in the right format. The file must contain one growth curve per column. The first column must be the timepoints and there must be a header row with unique identifiers for each curve. For example data and expected outputs, check out the files included in this Documentation folder. Sensible default parameters are set for all options but, depending on your data, you may wish to customise these, so check out the help section below. 
+
+```
+usage: pyphe-growthcurves [-h] --input INPUT [--fitrange FITRANGE]
+                          [--lag-method {abs,rel}]
+                          [--lag-threshold LAG_THRESHOLD]
+                          [--t0-fitrange T0_FITRANGE] [--plots]
+                          [--plot-ylim PLOT_YLIM]
+
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --input INPUT         Path to the growth curve file to analyse. This file
+                        contains one growth curve per column. The first column
+                        must be the timepoints and there must be a header row
+                        with unique identifiers for each curve.
+  --fitrange FITRANGE   Number of timepoint over which to fit linear
+                        regression. Defaults to 4. Please adjust this to the
+                        density of your timepoints and use higher values for
+                        more noisy data.
+  --lag-method {abs,rel}
+                        Method to use for determining lag. "abs" will measure
+                        time until the defined biomass threshold is crossed.
+                        "rel" will fist determine the inital biomass and
+                        measure the time until the biomass has passed this
+                        value times the threshold. Defaults to "rel".
+  --lag-threshold LAG_THRESHOLD
+                        Threshold to use for determining lag. With method
+                        "abs", this will measure time until the defined
+                        biomass threshold is crossed. With "rel" will fist
+                        determine the inital biomass and measure the time
+                        until the biomass has passed this value times the
+                        threshold. Defaults to 2.0, so with method "rel", this
+                        will measure the time taken for the first doubling.
+  --t0-fitrange T0_FITRANGE
+                        Specify the number of timepoint to use at the
+                        beginning of the growth curve to determine the initial
+                        biomass by averaging them. Defaults to 3.
+  --plots               Set this option (no argument required) to produce a
+                        plot of all growthcurves as pdf.
+  --plot-ylim PLOT_YLIM
+                        Specify the upper limit of the y-axis of growth curve
+                        plots. Useful if you want curves to be directly
+                        comparable. If not set, the axis of each curve is
+                        scaled to the data.
+```
+
+
+#### Interpreting results
+Pyphe-growthcurves will produce a csv file with extracted growth parameters. The maximum slope is determined by fitting all possible linear regressions in sliding windows of length n and chosing the one with the highest slope. The lag phase is determined as the first timepoint which exceeds a settable relative or absolute threshold. 
+
+| Parameter        | Explanation  |
+| ---------------- |---------------|
+|initial biomass|The average of the first n timepoints of the growth curve|
+|lag |  Lag phase |
+| max_slope| The maximum slope of the growth curve|
+| r2 | The R2 parameter of the linear regression that produced the highest maximum slope |
+|t_max | Time at which maximum growth slope is reached (center of the sliding window)|
+|y-intercept|Y-intercept of the regression which produced the maximum slope|
+|x-intercept|X-intercept of the regression which produced the maximum slope. This is interpreted as lag phase by some people|
+
+                            
+
+### Pyphe-quantify
+
+Pyphe quantify extracts colony parameters from images. In can operate in three distinct modes analysing colony sizes for each image individually (batch mode), analysing redness for each image individually (redness mode) or obtaining a growth curve from an image timeseries (timeseries mode).
+The --grid parameter is required define the position of colonies on the plate. You can either use automatic grid detection, one of our preconfigured positions if you are using the pp3 fixture or define your own (see the manual below). Images can be in any format (e.g. jpg, tiff, png). Images should be cropped closely to the colonies (this is important for good thresholding and automatic grid detection), i.e. not contain parts of the plate edges or surroundings. In batch and timecourse mode, pyphe-quantify assumes that images were acquired using transmission scanning, where colonies appear darker then the surrounding agar. If this is not the case and you took images by reflective scanning or with a camera, use --negate False. In batch and timecourse mode, images are epxected to be grayscale. If they are not, they will be converted (by simply summing all channels) and a warning will be thrown. 
+
+
+```
+usage: pyphe-quantify [-h] --grid GRID [--pattern PATTERN] [--t T] [--d D]
+                      [--s S] [--negate NEGATE] [--localThresh] [--convexhull]
+                      [--reportAll] [--reportFileNames]
+                      [--hardImageThreshold HARDIMAGETHRESHOLD]
+                      [--hardSizeThreshold HARDSIZETHRESHOLD] [--qc QC]
+                      [--calibrate CALIBRATE] [--timepoints TIMEPOINTS]
+                      [--out OUT]
+                      {batch,timecourse,redness}
+
+Welcome to pyphe-quantify, part of the pyphe toolbox. Written by
+stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
+Lab/pyphe
+
+positional arguments:
+  {batch,timecourse,redness}
+                        Pyphe-quantify can be run in three different modes. In
+                        batch mode, it quantifies colony sizes for all images
+                        matching the pattern individually. A separate results
+                        table and qc image is produced for each. Redness mode
+                        is similar except that the redness of each colony is
+                        quantified. In timecourse mode, all images matching
+                        the pattern are analysed jointly. The final image
+                        matching the pattern is used to create a mask of where
+                        the colonies are and this mask is then applied to all
+                        previous images in the timeseries. A single output
+                        table, where the timepoints are the rows and each
+                        individual colony is a row.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --grid GRID           This option is required (all others have defaults set)
+                        and specifies the grid in which the colonies are
+                        arranged. You can use automatic grid detection using
+                        one of the following parameters: auto_96, auto_384 or
+                        auto_1536. Automatic grid correction will not work if
+                        the colony grid is not aligned with the image borders.
+                        Images should contain only agar and colonies, avaoid
+                        having borders. It might fail or produce unexpected
+                        results if there are whole rows/columns missing. In
+                        those cases, it is easy to define hard-wired grid
+                        positions. If you are using the fixture provided with
+                        pyphe, we have preconfigured these for you. Depending
+                        on the pinning density, use pp3_96, pp3_384 or
+                        pp3_1536. Otherwise, the argument has to be in the
+                        form of 6 integer numbers separated by "-": <number of
+                        colony rows>-<number of colony columns>-<x-position of
+                        the top left colony>-<y-position of the top left
+                        colony>-<x-position of the bottom right
+                        colony>-<y-position of the bottom right colony>.
+                        Positions must be integers and are the distance in
+                        number of pixels from the image origin in each
+                        dimension (x is width dimension, y is height
+                        dimension). The image origin is, in line with scikit-
+                        image, in the top left corner. Pixel positions are
+                        easily determined using programs such as Microsoft
+                        Paint, by simply hovering the mouse over a position.
+  --pattern PATTERN     Pattern describing files to analyse. This follows
+                        standard unix convention and can be used to specify
+                        subfolders in which to look for images
+                        (<subfolder>/*.jpg) or the image format (*.tiff,
+                        *.png, etc.). By default, all jpg images in the
+                        working directory are analysed.
+  --t T                 By default the intensity threshold to distinguish
+                        colonies from the background is determined by the Otsu
+                        method. The determined value will be multiplied by
+                        this argument to give the final threshold. Useful for
+                        easily fine-tuning colony detection.
+  --d D                 The distance between two grid positions will be
+                        divided by this number to compute the maximum distance
+                        a putative colony can be away from its reference grid
+                        position. Decreasing this number towards 2 makes
+                        colony-to-grid-matching more permissive (might help
+                        when some of your plates are at a slight angle or out
+                        of position).
+  --s S                 Detected putative colonies will be filtered by size
+                        and small components (usually image noise) will be
+                        excluded. The default threshold is the image
+                        area*0.00005 and is therefore independent of scanning
+                        resolution. This default is then multiplied by this
+                        argument to give the final threshold. Useful for when
+                        colonies have unusual sizes.
+  --negate NEGATE       In images acquired by transmission scanning, the
+                        colonies are darker than the background. Before
+                        thresholding, the image needs to be inverted/negated.
+                        Defaults to True in timecourse and batch mode, ignored
+                        in redness mode.
+  --localThresh         Use local thresholding in batch and timecourse mode.
+                        This can help when image brightness is very uneven.
+                        Ignored in redness mode where local thresholding is
+                        always applied.
+  --convexhull          Apply convex hull transformation to identified
+                        colonies to fill holes. Useful when working with spots
+                        rather than colonies. Ignored in redness mode.
+                        WARNING: Using this options results in much longer
+                        analysis times.
+  --reportAll           Sometimes, two putative colonies are identified that
+                        are within the distance threshold of a grid position.
+                        By default, only the closest colony is reported. This
+                        can be changed by setting this option (without
+                        parameter). This option allows pyphe quantify to be
+                        used even if colonies are not arrayed in a regular
+                        grid (you still need to provide a grid parameter
+                        though that spans the colonies you are interested i).
+  --reportFileNames     Only for timecourse mode, otherwise ignored. Use
+                        filenames as index for output table instead of
+                        timepoints. Useful when the ordering of timepoints is
+                        not the same as returned by the pattern. Setting this
+                        option overrides the --timepoints argument.
+  --hardImageThreshold HARDIMAGETHRESHOLD
+                        Allows a hard (fixed) intensity threshold in the range
+                        [0,1] to be used instead of Otsu thresholding. Images
+                        intensities are re-scaled to [0,1] before
+                        thresholding. Ignored in timecourse mode.
+  --hardSizeThreshold HARDSIZETHRESHOLD
+                        Allows a hard (fixed) size threshold [number of
+                        pixels] to be used for filtering small colonies.
+  --qc QC               Directory to save qc images in. Defaults to
+                        "qc_images".
+  --calibrate CALIBRATE
+                        Transform background subtracted intensity values by
+                        this function. Function needs to be a single term with
+                        x as the variable and that is valid python code. E.g.
+                        use "2*x**2+1" to square each pixels intensity,
+                        multiply by two and add 1. Defaults to "x", i.e. use
+                        of no calibration. Used only in timecourse mode.
+  --timepoints TIMEPOINTS
+                        In timecourse mode only. Path to a file that specifies
+                        the timepoints of all images in the timeseries. This
+                        is usually the timepoints.txt file created by pyphe-
+                        scan-timecourse. It must contain one entry per line
+                        and have the same number of lines as number of images.
+  --out OUT             Directory to save output files in. Defaults to
+                        "pyphe_quant".
+```
+
+
+
+### Pyphe-analyse
+_Pyphe-analyse_ is a tool for spatial normalisation and data aggregation across many plates. It implements a grid normalisation based on the concept proposed by [Zackrisson et al. 2016](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5015956/) and row/column median normalisation. Please see our paper and the protocol in it to find out more. _Pyphe-analyse_ can be run from the command line, with options below, or using the graphical user interface by running _pyphe-analyse-gui_.
+
+
+```
+usage: pyphe-analyse.txt [-h] --edt EDT --format
+                         {gitter,pyphe-redness,pyphe-growthcurves} [--out OUT]
+                         [--load_layouts]
+                         [--gridnorm {standard384,standard1536}]
+                         [--extrapolate_corners] [--rcmedian] [--check CHECK]
+                         [--qc_plots QC_PLOTS]
+
+Welcome to pyphe-analyse, part of the pyphe toolbox. Written by
+stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
+Lab/pyphe
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --edt EDT             Path to the Experimental Design Table (EDT) listing
+                        all plates of the experiment. The table must be in csv
+                        format, the first column must contain unique plate IDs
+                        and there must be a column named 'Data_path' that
+                        contains abolute or relative file paths to each
+                        plate's data file. A 'Layout_path' column can be
+                        included, see below. Any additional columns included
+                        in this file will bestored in each plate's meta-data
+                        and included in the final data output.
+  --format {gitter,pyphe-redness,pyphe-growthcurves}
+                        Type of inout data.
+  --out OUT             Specifies the path where to save the output data
+                        result. By default, the data report is saved in the
+                        working directory as "pyphe-analyse_data_report.csv"
+                        and will overwrite the file if it exists.
+  --load_layouts        Set this option (without parameters) to load layouts
+                        (requires Layout_path column in the EDT).
+  --gridnorm {standard384,standard1536,1536with384grid}
+                        Perform reference grid normalisation. Standard384
+                        refers to plates which are in 384 (16x24) format with
+                        the reference grid in 96 format in the top left
+                        corner. Standard1536 refers to plates in 1536 format
+                        (32x48( with two 96 reference grids in the top left
+                        and bottom right corners. 1536with384grid refers to
+                        plates in 1536 format with a 384 reference grid in
+                        the top left position.
+  --extrapolate_corners
+                        If working in standard1536 format, set this option to
+                        extrapolate the reference grid in the bottom left and
+                        top right corner. A linear regression will be trained
+                        across all top left and bottom right corners on plates
+                        in the experiment to predict hypothetical grid colony
+                        sizes in the other two corners.
+  --rcmedian            Perform row/column median normalisation. If --gridnorm
+                        will be performed first if both parameters are set.
+  --check CHECK         Check colony sizes after normalisation for negative
+                        and infinite colony sizes *(normalisation artefacts),
+                        throw a warning and set to NA.
+  --qc_plots QC_PLOTS   Specify a folder in which to save qc plots for each
+                        plate.
+
+```
+
+
+### Pyphe-interpret
+
+Pyphe-interpret reports summary statistics and tests for differential fitness using t-tests. It is flexible and can in theory be used with any dataset in tidy format.
+
+```
+usage: pyphe-interpret [-h] --ld LD [--out OUT] --grouping_column
+                       GROUPING_COLUMN --axis_column AXIS_COLUMN
+                       [--values_column VALUES_COLUMN] --control CONTROL
+                       [--ld_encoding LD_ENCODING] [--circularity CIRCULARITY]
+                       [--set_missing_na]
+
+Welcome to pyphe-interpret, part of the pyphe toolbox. Written by
+stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
+Lab/pyphe. Pyphe-interpret calculates summary statistics and p-values from the
+data reports generated by pyphe-analyse. For this, specifiying your column
+names correctly is crucial. Let us assume you have measured many strains in
+many conditions. Now you would like to know for each strain in each condition
+(for each condition-strain pair) if it is "significant". There are essentially
+two ways of doing this, asking different biological questions. (1) Check for
+each condition separately (--grouping_column <condition_column>) if there is a
+significant difference in means between a mutant strain and a control strain
+(--axis_column <strain_id_column>). Or (2) Check for each strain separately
+(--grouping_column <strain_id_column>) if there is a significant difference in
+the means of the strain in the assay condition versus the control condition
+(--axis_column <condition_column>). The second option tests for condition-
+specific growth effects (i.e. is does not return significant results if a
+strain is always faster or always slower growing than the grid strain). In
+both cases you need to specify the control against which to test using
+--control and this has to be a value that appears in the axis column. You
+should define the dependent variable of the t-test using --values_column. FDR
+correction with the Benjamini-Hochberg method will be applied on each level
+set of the grouping_column separately, ie for case (1) p-values will be
+corrected across each strain separately, ie more conditions means more
+stringent correction, and for case (2) p-values will be corrected for each
+condition separately, ie more strains means mpre stringent correction.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --ld LD               Path to the Data Report Table produced by pyphe-
+                        analyse.
+  --out OUT             Specifies the path where to save the output data
+                        result. By default, a table with all replicates will
+                        be saved as pyphe-interpret-report_reps.csv and the
+                        statistic table will be saved as pyphe-interpret-
+                        report_summaryStats.csv in the current working
+                        directory. Existing files will be overwritten.
+  --grouping_column GROUPING_COLUMN
+                        Name of the column in the data report to use for
+                        forming groups on which to perform independent sets of
+                        t-tests.
+  --axis_column AXIS_COLUMN
+                        Name of the column in the data report to repeat
+                        t-tests along within each group. Levels in this column
+                        will be the explanatory/independent variable used for
+                        t-tests.
+  --values_column VALUES_COLUMN
+                        Name of the column in the data report to use as
+                        fitness values. This will be the dependent variable
+                        for t-tests. Defaults to "Colony_size_corr_checked".
+  --control CONTROL     Name of the control to compare against. This must be a
+                        value found in the axis column.
+  --ld_encoding LD_ENCODING
+                        Encoding of the data report table to be passed to
+                        pandas.read_csv().
+  --circularity CIRCULARITY
+                        Exclude colonies from the analysis with a circularity
+                        below the one specified. A circularity of 1
+                        corresponds to a perfect circle. We recommend a
+                        threshold around 0.85.
+  --set_missing_na      Set 0-sized colonies to NA. This is recommended if you
+                        expect no missing colonies in your data, which means
+                        these are probably due to pinning errors.
+```
+
```

### Comparing `pyphe-0.981/README.md` & `pyphe-0.982/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,472 +1,490 @@
-![pyphe logo](https://github.com/Bahler-Lab/pyphe/blob/master/icons/toolbox-72dpi_white.png)
-
-# Welcome to the pyphe toolbox
-A python toolbox for phenotype analysis of arrayed microbial colonies written by Stephan Kamrad (stephan.kamrad at crick.ac.uk).
-
-For a quick overview, please see our [10 minute video tutorial](https://www.youtube.com/watch?v=lQ3lXIdhA1c&t=5s).
-
-For a more detailed protocol, including growth curves and viability assays, please see our [protocol preprint](https://www.researchsquare.com/article/rs-401914/v1).
-
-For more background information, please see our [_eLife_ paper](https://elifesciences.org/articles/55160).
-
-Please cite as:
-> Kamrad, S., Rodríguez-López, M., Cotobal, C., Correia-Melo, C., Ralser M., Bähler J. (2020). Pyphe, a python toolbox for assessing microbial growth and cell viability in high-throughput colony screens. eLife 9:e55160
-
-## Installation
-1. Most tools are cross-platform compatible but scanning will only work on a Linux OS. The scanners need to be accessible by [SANE](http://www.sane-project.org/) and [ImageMagick](https://imagemagick.org/) needs to be installed and accessible from the command line.
-2. Pyphe requires Python 3 and a few common packages, available through the [anaconda distribution](https://www.anaconda.com/distribution/).
-3. Install pyphe by running 'pip install pyphe' in your terminal.
-4. Open a new terminal and try and run 'pyphe-quantify -h' which should show the help page of one of pyphe's command line tools. On Windows, make sure you are using the Anaconda Prompt, not the Anaconda Powershell Prompt.
-
-
-## Overview
-A typical fitness screen with pyphe will involve:
-1. Image acquisition with [_pyphe-scan_](#pyphe-scan), or [_pyphe-scan-timecourse_](#pyphe-scan-timecourse)
-2. Quantification of colony properties from images using [_pyphe-quantify_](#pyphe-quantify). In the case of growth curves, parameters are additionally extracted with [_pyphe-growthcurves_](#pyphe-growthcurves).
-3. Normalisation and data aggregation using [_pyphe-analyse_](#pyphe-analyse).
-4. Statistics and hit calling using [_pyphe-interpret_](#pyphe-interpret)
-Please see our paper for a detailed protocol and explanations of the algorithms.
-
-
-## Support
-Please check the manuals below carefully, they are also available in the terminal by running the command with the -h option only. If things are still not working, please email me (stephan.kamrad@crick.ac.uk) and I will try and help. If you think you have discovered a bug, or would like to request a new feature, please raise an issue on www.github.com/Bahler-Lab/pyphe.
-
-If you get an error like this, make sure you are not using the Anaconda Powershell Prompt:
-```python: can't open file 'C:\Users\user1\Anaconda3\Scripts"C:\Users\user1\Anaconda3\Scripts\pyphe-quantify.bat  -h ': [Errno 22] Invalid argument```
-
-## Manual
-
-All pyphe tools have a similar command line interface, based on the python argparse package. Generally, parameters are set using --<parameter_name> optionally followed by a value. All _pyphe_ tools can be used with relative file paths so make sure to navigate to the correct working directory before running a _pyphe_ command.
-
- 
-### Pyphe-scan
-This tools allows you to take consecutive scans of sets of plates, which are then automatically cropped, rotated and named in in a continuos filename scheme of your choice. 
-
-#### Prerequisites
-1. This tool will only run on Linux operating systems and uses the SANE library for image acquisition.
-
-2. Make sure your scanner is installed correctly and you can acquire images using the scanimage command. The Gray mode will only work on Epson V800 and V850 scanners (potentially the V700 and V750 model as well) and the TPU8x10 transmission scanning source must be enabled. This should work by default if you are using the V800/850 model and a recent Linux OS. Otherwise, there is excellent documentation available from Zackrisson et al. and the [scanomatics pipeline](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5015956/) for how to make this work using a hacked SANE driver. Please see the instructions in their [wiki](https://github.com/Scan-o-Matic/scanomatic/wiki/Installing-scanners).
-
-2. Make sure [ImageMagick](https://imagemagick.org/index.php) is installed and the 'convert' tool can be called from the command line.
-
-3. If the Pyphe toolbox has been installed correctly, you should be able to run _pyphe-scan_ in your terminal. 
-
-4. With a laser cutter, make a fixture to hold your plates in place. We provide an svg file with the cutting shape in the Documentation directory. Use tape to hold your fixture into place, it should be pushed against the back of the scanner (where the cables are) with the top of the plates facing left. Pyphe-scan and pyphe-quantify come pre-configured for using the provided fixture on an Epson V800/V850 scanner but it is easy to add your own fixture and cropping settings. If you want to use your own fixture, see below of how to add the geometry information to pyphe-scan. 
-
-#### Scanning plate batches
-
-1. Open the file manager and navigate to the folder in which you want to save your images. The script will create a sub-folder that begins with the current date to save all your images. 
-
-2. Right click and select 'Open in Terminal'
-
-3. Run scanplates with the options as detaild below. 
-
-```
-usage: pyphe-scan [-h] [--nplates NPLATES] [--start START] [--prefix PREFIX]
-                  [--postfix POSTFIX] [--fixture {som3_edge,som3}]
-                  [--resolution {150,300,600,900,1200}] [--scanner {1,2,3}]
-                  [--mode {Gray,Color}]
-
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --nplates NPLATES     Number of plates to scan. This defaults to 100 and the
-                        script can be terminated by Ctr+C when done.
-  --start START         Where to start numbering from. Defaults to 1.
-  --prefix PREFIX       Name prefix for output files. The default is the
-                        current date YYYYMMDD.
-  --postfix POSTFIX     Name postfix for output files. Defaults to empty
-                        string.
-  --fixture {som3_edge,som3,som3-color}
-                        ID of the fixture you are using.
-  --resolution {150,300,600,900,1200}
-                        Resolution for scanning in dpi. Default is 600.
-  --scanner {1,2,3}     Which scanner to use. Scanners are not uniquely
-                        identified and may switch when turned off/unplugged.
-                        This option does not need to be set when only one
-                        scanner is connected.
-  --mode {Gray,Color}   Which color mode to use for scanning. Defaults to
-                        Gray.
-```
-
-All arguments except the fixture have default values and are optional. A folder prefix_postfix will be created in your current directory and the program will abort if a folder with this name already exists. 
-
-
-
-### Pyphe-scan-timecourse
-
-This tool acquires image timeseries by scanning in fixed time intervals. For each position in the fixture, a folder is created. Image names contain number of scan. Other options for this tool are similar to [_pyphe-scan_](#pyphe-scan). More than one scanner can be connected and used at the same time. Scanner numbers are defined by the order in which they are connected to the computer. Proceed as follows: (1) disconnect all scanners, (2) prepare the first scanner with plates, connect it and turn it on. (3) start scanning with --scanner 1 option, (4) prepare the second scanner, connect it and turn it on, (5) start scanning with --scanner 2 option. Repeat step (4) and (5), each time incrementing the --scanner argument. 
-
-```
-usage: pyphe-scan-timecourse [-h] [--nscans NSCANS] [--interval INTERVAL]
-                             [--prefix PREFIX] [--postfix POSTFIX]
-                             [--fixture {som3_edge,som3}]
-                             [--resolution {150,300,600,900,1200}]
-                             [--scanner {1,2,3}] [--mode {Gray,Color}]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --nscans NSCANS       Number of time points to scan. This defaults to 100
-                        and the script can be terminated by Ctr+C when done.
-  --interval INTERVAL   Time in minutes between scans. Defaults to 20.
-  --prefix PREFIX       Name prefix for output files. The default is the
-                        current date YYYYMMDD.
-  --postfix POSTFIX     Name postfix for output files. Defaults to empty
-                        string.
-  --fixture {som3_edge,som3,som3-color}
-                        ID of the fixture you are using.
-  --resolution {150,300,600,900,1200}
-                        Resolution for scanning in dpi. Default is 600.
-  --scanner {1,2,3}     Which scanner to use. Scanners are not uniquely
-                        identified and may switch when turned off/unplugged.
-                        This option does not need to be set when only one
-                        scanner is connected.
-  --mode {Gray,Color}   Which color mode to use for scanning. Defaults to
-                        Gray.
-```
-
-
-### Pyphe-growthcurves
-This tool performs non-parametric analysis of growth curves. It was written specifically to analyse colony size timeseries data obtained with _pyphe-quantify_ _timeseries_.
-
-It is important that your csv with the growth data is in the right format. The file must contain one growth curve per column. The first column must be the timepoints and there must be a header row with unique identifiers for each curve. For example data and expected outputs, check out the files included in this Documentation folder. Sensible default parameters are set for all options but, depending on your data, you may wish to customise these, so check out the help section below. 
-
-```
-usage: pyphe-growthcurves [-h] --input INPUT [--fitrange FITRANGE]
-                          [--lag-method {abs,rel}]
-                          [--lag-threshold LAG_THRESHOLD]
-                          [--t0-fitrange T0_FITRANGE] [--plots]
-                          [--plot-ylim PLOT_YLIM]
-
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --input INPUT         Path to the growth curve file to analyse. This file
-                        contains one growth curve per column. The first column
-                        must be the timepoints and there must be a header row
-                        with unique identifiers for each curve.
-  --fitrange FITRANGE   Number of timepoint over which to fit linear
-                        regression. Defaults to 4. Please adjust this to the
-                        density of your timepoints and use higher values for
-                        more noisy data.
-  --lag-method {abs,rel}
-                        Method to use for determining lag. "abs" will measure
-                        time until the defined biomass threshold is crossed.
-                        "rel" will fist determine the inital biomass and
-                        measure the time until the biomass has passed this
-                        value times the threshold. Defaults to "rel".
-  --lag-threshold LAG_THRESHOLD
-                        Threshold to use for determining lag. With method
-                        "abs", this will measure time until the defined
-                        biomass threshold is crossed. With "rel" will fist
-                        determine the inital biomass and measure the time
-                        until the biomass has passed this value times the
-                        threshold. Defaults to 2.0, so with method "rel", this
-                        will measure the time taken for the first doubling.
-  --t0-fitrange T0_FITRANGE
-                        Specify the number of timepoint to use at the
-                        beginning of the growth curve to determine the initial
-                        biomass by averaging them. Defaults to 3.
-  --plots               Set this option (no argument required) to produce a
-                        plot of all growthcurves as pdf.
-  --plot-ylim PLOT_YLIM
-                        Specify the upper limit of the y-axis of growth curve
-                        plots. Useful if you want curves to be directly
-                        comparable. If not set, the axis of each curve is
-                        scaled to the data.
-```
-
-
-#### Interpreting results
-Pyphe-growthcurves will produce a csv file with extracted growth parameters. The maximum slope is determined by fitting all possible linear regressions in sliding windows of length n and chosing the one with the highest slope. The lag phase is determined as the first timepoint which exceeds a settable relative or absolute threshold. 
-
-| Parameter        | Explanation  |
-| ---------------- |---------------|
-|initial biomass|The average of the first n timepoints of the growth curve|
-|lag |  Lag phase |
-| max_slope| The maximum slope of the growth curve|
-| r2 | The R2 parameter of the linear regression that produced the highest maximum slope |
-|t_max | Time at which maximum growth slope is reached (center of the sliding window)|
-|y-intercept|Y-intercept of the regression which produced the maximum slope|
-|x-intercept|X-intercept of the regression which produced the maximum slope. This is interpreted as lag phase by some people|
-
-                            
-
-### Pyphe-quantify
-
-Pyphe quantify extracts colony parameters from images. In can operate in three distinct modes analysing colony sizes for each image individually (batch mode), analysing redness for each image individually (redness mode) or obtaining a growth curve from an image timeseries (timeseries mode).
-The --grid parameter is required define the position of colonies on the plate. You can either use automatic grid detection, one of our preconfigured positions if you are using the pp3 fixture or define your own (see the manual below). Images can be in any format (e.g. jpg, tiff, png). Images should be cropped closely to the colonies (this is important for good thresholding and automatic grid detection), i.e. not contain parts of the plate edges or surroundings. In batch and timecourse mode, pyphe-quantify assumes that images were acquired using transmission scanning, where colonies appear darker then the surrounding agar. If this is not the case and you took images by reflective scanning or with a camera, use --negate False. In batch and timecourse mode, images are epxected to be grayscale. If they are not, they will be converted (by simply summing all channels) and a warning will be thrown. 
-
-
-```
-usage: pyphe-quantify [-h] --grid GRID [--pattern PATTERN] [--t T] [--d D]
-                      [--s S] [--negate NEGATE] [--localThresh] [--convexhull]
-                      [--reportAll] [--reportFileNames]
-                      [--hardImageThreshold HARDIMAGETHRESHOLD]
-                      [--hardSizeThreshold HARDSIZETHRESHOLD] [--qc QC]
-                      [--calibrate CALIBRATE] [--timepoints TIMEPOINTS]
-                      [--out OUT]
-                      {batch,timecourse,redness}
-
-Welcome to pyphe-quantify, part of the pyphe toolbox. Written by
-stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
-Lab/pyphe
-
-positional arguments:
-  {batch,timecourse,redness}
-                        Pyphe-quantify can be run in three different modes. In
-                        batch mode, it quantifies colony sizes for all images
-                        matching the pattern individually. A separate results
-                        table and qc image is produced for each. Redness mode
-                        is similar except that the redness of each colony is
-                        quantified. In timecourse mode, all images matching
-                        the pattern are analysed jointly. The final image
-                        matching the pattern is used to create a mask of where
-                        the colonies are and this mask is then applied to all
-                        previous images in the timeseries. A single output
-                        table, where the timepoints are the rows and each
-                        individual colony is a row.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --grid GRID           This option is required (all others have defaults set)
-                        and specifies the grid in which the colonies are
-                        arranged. You can use automatic grid detection using
-                        one of the following parameters: auto_96, auto_384 or
-                        auto_1536. Automatic grid correction will not work if
-                        the colony grid is not aligned with the image borders.
-                        Images should contain only agar and colonies, avaoid
-                        having borders. It might fail or produce unexpected
-                        results if there are whole rows/columns missing. In
-                        those cases, it is easy to define hard-wired grid
-                        positions. If you are using the fixture provided with
-                        pyphe, we have preconfigured these for you. Depending
-                        on the pinning density, use pp3_96, pp3_384 or
-                        pp3_1536. Otherwise, the argument has to be in the
-                        form of 6 integer numbers separated by "-": <number of
-                        colony rows>-<number of colony columns>-<x-position of
-                        the top left colony>-<y-position of the top left
-                        colony>-<x-position of the bottom right
-                        colony>-<y-position of the bottom right colony>.
-                        Positions must be integers and are the distance in
-                        number of pixels from the image origin in each
-                        dimension (x is width dimension, y is height
-                        dimension). The image origin is, in line with scikit-
-                        image, in the top left corner. Pixel positions are
-                        easily determined using programs such as Microsoft
-                        Paint, by simply hovering the mouse over a position.
-  --pattern PATTERN     Pattern describing files to analyse. This follows
-                        standard unix convention and can be used to specify
-                        subfolders in which to look for images
-                        (<subfolder>/*.jpg) or the image format (*.tiff,
-                        *.png, etc.). By default, all jpg images in the
-                        working directory are analysed.
-  --t T                 By default the intensity threshold to distinguish
-                        colonies from the background is determined by the Otsu
-                        method. The determined value will be multiplied by
-                        this argument to give the final threshold. Useful for
-                        easily fine-tuning colony detection.
-  --d D                 The distance between two grid positions will be
-                        divided by this number to compute the maximum distance
-                        a putative colony can be away from its reference grid
-                        position. Decreasing this number towards 2 makes
-                        colony-to-grid-matching more permissive (might help
-                        when some of your plates are at a slight angle or out
-                        of position).
-  --s S                 Detected putative colonies will be filtered by size
-                        and small components (usually image noise) will be
-                        excluded. The default threshold is the image
-                        area*0.00005 and is therefore independent of scanning
-                        resolution. This default is then multiplied by this
-                        argument to give the final threshold. Useful for when
-                        colonies have unusual sizes.
-  --negate NEGATE       In images acquired by transmission scanning, the
-                        colonies are darker than the background. Before
-                        thresholding, the image needs to be inverted/negated.
-                        Defaults to True in timecourse and batch mode, ignored
-                        in redness mode.
-  --localThresh         Use local thresholding in batch and timecourse mode.
-                        This can help when image brightness is very uneven.
-                        Ignored in redness mode where local thresholding is
-                        always applied.
-  --convexhull          Apply convex hull transformation to identified
-                        colonies to fill holes. Useful when working with spots
-                        rather than colonies. Ignored in redness mode.
-                        WARNING: Using this options results in much longer
-                        analysis times.
-  --reportAll           Sometimes, two putative colonies are identified that
-                        are within the distance threshold of a grid position.
-                        By default, only the closest colony is reported. This
-                        can be changed by setting this option (without
-                        parameter). This option allows pyphe quantify to be
-                        used even if colonies are not arrayed in a regular
-                        grid (you still need to provide a grid parameter
-                        though that spans the colonies you are interested i).
-  --reportFileNames     Only for timecourse mode, otherwise ignored. Use
-                        filenames as index for output table instead of
-                        timepoints. Useful when the ordering of timepoints is
-                        not the same as returned by the pattern. Setting this
-                        option overrides the --timepoints argument.
-  --hardImageThreshold HARDIMAGETHRESHOLD
-                        Allows a hard (fixed) intensity threshold in the range
-                        [0,1] to be used instead of Otsu thresholding. Images
-                        intensities are re-scaled to [0,1] before
-                        thresholding. Ignored in timecourse mode.
-  --hardSizeThreshold HARDSIZETHRESHOLD
-                        Allows a hard (fixed) size threshold [number of
-                        pixels] to be used for filtering small colonies.
-  --qc QC               Directory to save qc images in. Defaults to
-                        "qc_images".
-  --calibrate CALIBRATE
-                        Transform background subtracted intensity values by
-                        this function. Function needs to be a single term with
-                        x as the variable and that is valid python code. E.g.
-                        use "2*x**2+1" to square each pixels intensity,
-                        multiply by two and add 1. Defaults to "x", i.e. use
-                        of no calibration. Used only in timecourse mode.
-  --timepoints TIMEPOINTS
-                        In timecourse mode only. Path to a file that specifies
-                        the timepoints of all images in the timeseries. This
-                        is usually the timepoints.txt file created by pyphe-
-                        scan-timecourse. It must contain one entry per line
-                        and have the same number of lines as number of images.
-  --out OUT             Directory to save output files in. Defaults to
-                        "pyphe_quant".
-```
-
-
-
-### Pyphe-analyse
-_Pyphe-analyse_ is a tool for spatial normalisation and data aggregation across many plates. It implements a grid normalisation based on the concept proposed by [Zackrisson et al. 2016](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5015956/) and row/column median normalisation. Please see our paper and the protocol in it to find out more. _Pyphe-analyse_ can be run from the command line, with options below, or using the graphical user interface by running _pyphe-analyse-gui_.
-
-
-```
-usage: pyphe-analyse.txt [-h] --edt EDT --format
-                         {gitter,pyphe-redness,pyphe-growthcurves} [--out OUT]
-                         [--load_layouts]
-                         [--gridnorm {standard384,standard1536}]
-                         [--extrapolate_corners] [--rcmedian] [--check CHECK]
-                         [--qc_plots QC_PLOTS]
-
-Welcome to pyphe-analyse, part of the pyphe toolbox. Written by
-stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
-Lab/pyphe
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --edt EDT             Path to the Experimental Design Table (EDT) listing
-                        all plates of the experiment. The table must be in csv
-                        format, the first column must contain unique plate IDs
-                        and there must be a column named 'Data_path' that
-                        contains abolute or relative file paths to each
-                        plate's data file. A 'Layout_path' column can be
-                        included, see below. Any additional columns included
-                        in this file will bestored in each plate's meta-data
-                        and included in the final data output.
-  --format {gitter,pyphe-redness,pyphe-growthcurves}
-                        Type of inout data.
-  --out OUT             Specifies the path where to save the output data
-                        result. By default, the data report is saved in the
-                        working directory as "pyphe-analyse_data_report.csv"
-                        and will overwrite the file if it exists.
-  --load_layouts        Set this option (without parameters) to load layouts
-                        (requires Layout_path column in the EDT).
-  --gridnorm {standard384,standard1536}
-                        Perform reference grid normalisation. Standard384
-                        refers to plates which are in 384 (16x24) format with
-                        the reference grid in 96 format in the top left
-                        corner. Standard1536 refers to plates in 1536 format
-                        (32x48( with two 96 reference grids in the top left
-                        and bottom right corners.
-  --extrapolate_corners
-                        If working in standard1536 format, set this option to
-                        extrapolate the reference grid in the bottom left and
-                        top right corner. A linear regression will be trained
-                        across all top left and bottom right corners on plates
-                        in the experiment to predict hypothetical grid colony
-                        sizes in the other two corners.
-  --rcmedian            Perform row/column median normalisation. If --gridnorm
-                        will be performed first if both parameters are set.
-  --check CHECK         Check colony sizes after normalisation for negative
-                        and infinite colony sizes *(normalisation artefacts),
-                        throw a warning and set to NA.
-  --qc_plots QC_PLOTS   Specify a folder in which to save qc plots for each
-                        plate.
-
-```
-
-
-### Pyphe-interpret
-
-Pyphe-interpret reports summary statistics and tests for differential fitness using t-tests. It is flexible and can in theory be used with any dataset in tidy format.
-
-```
-usage: pyphe-interpret [-h] --ld LD [--out OUT] --grouping_column
-                       GROUPING_COLUMN --axis_column AXIS_COLUMN
-                       [--values_column VALUES_COLUMN] --control CONTROL
-                       [--ld_encoding LD_ENCODING] [--circularity CIRCULARITY]
-                       [--set_missing_na]
-
-Welcome to pyphe-interpret, part of the pyphe toolbox. Written by
-stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
-Lab/pyphe. Pyphe-interpret calculates summary statistics and p-values from the
-data reports generated by pyphe-analyse. For this, specifiying your column
-names correctly is crucial. Let us assume you have measured many strains in
-many conditions. Now you would like to know for each strain in each condition
-(for each condition-strain pair) if it is "significant". There are essentially
-two ways of doing this, asking different biological questions. (1) Check for
-each condition separately (--grouping_column <condition_column>) if there is a
-significant difference in means between a mutant strain and a control strain
-(--axis_column <strain_id_column>). Or (2) Check for each strain separately
-(--grouping_column <strain_id_column>) if there is a significant difference in
-the means of the strain in the assay condition versus the control condition
-(--axis_column <condition_column>). The second option tests for condition-
-specific growth effects (i.e. is does not return significant results if a
-strain is always faster or always slower growing than the grid strain). In
-both cases you need to specify the control against which to test using
---control and this has to be a value that appears in the axis column. You
-should define the dependent variable of the t-test using --values_column. FDR
-correction with the Benjamini-Hochberg method will be applied on each level
-set of the grouping_column separately, ie for case (1) p-values will be
-corrected across each strain separately, ie more conditions means more
-stringent correction, and for case (2) p-values will be corrected for each
-condition separately, ie more strains means mpre stringent correction.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --ld LD               Path to the Data Report Table produced by pyphe-
-                        analyse.
-  --out OUT             Specifies the path where to save the output data
-                        result. By default, a table with all replicates will
-                        be saved as pyphe-interpret-report_reps.csv and the
-                        statistic table will be saved as pyphe-interpret-
-                        report_summaryStats.csv in the current working
-                        directory. Existing files will be overwritten.
-  --grouping_column GROUPING_COLUMN
-                        Name of the column in the data report to use for
-                        forming groups on which to perform independent sets of
-                        t-tests.
-  --axis_column AXIS_COLUMN
-                        Name of the column in the data report to repeat
-                        t-tests along within each group. Levels in this column
-                        will be the explanatory/independent variable used for
-                        t-tests.
-  --values_column VALUES_COLUMN
-                        Name of the column in the data report to use as
-                        fitness values. This will be the dependent variable
-                        for t-tests. Defaults to "Colony_size_corr_checked".
-  --control CONTROL     Name of the control to compare against. This must be a
-                        value found in the axis column.
-  --ld_encoding LD_ENCODING
-                        Encoding of the data report table to be passed to
-                        pandas.read_csv().
-  --circularity CIRCULARITY
-                        Exclude colonies from the analysis with a circularity
-                        below the one specified. A circularity of 1
-                        corresponds to a perfect circle. We recommend a
-                        threshold around 0.85.
-  --set_missing_na      Set 0-sized colonies to NA. This is recommended if you
-                        expect no missing colonies in your data, which means
-                        these are probably due to pinning errors.
-```
-
+Metadata-Version: 2.1
+Name: pyphe
+Version: 0.982
+Summary: Python toolbox for phenotype analysis of arrayed microbial colonies
+Home-page: https://github.com/Bahler-Lab/pyphe
+Author: Stephan Kamrad
+Author-email: stephan.kamrad@gmail.com
+License: MIT
+Description: ![pyphe logo](https://github.com/Bahler-Lab/pyphe/blob/master/icons/toolbox-72dpi_white.png)
+        
+        # Welcome to the pyphe toolbox
+        A python toolbox for phenotype analysis of arrayed microbial colonies written by Stephan Kamrad (stephan.kamrad at crick.ac.uk).
+        
+        For a quick overview, please see our [10 minute video tutorial](https://www.youtube.com/watch?v=lQ3lXIdhA1c&t=5s).
+        
+        For a more detailed protocol, including growth curves and viability assays, please see our [protocol preprint](https://www.researchsquare.com/article/rs-401914/v1).
+        
+        For more background information, please see our [_eLife_ paper](https://elifesciences.org/articles/55160).
+        
+        Please cite as:
+        > Kamrad, S., Rodríguez-López, M., Cotobal, C., Correia-Melo, C., Ralser M., Bähler J. (2020). Pyphe, a python toolbox for assessing microbial growth and cell viability in high-throughput colony screens. eLife 9:e55160
+        
+        ## Installation
+        1. Most tools are cross-platform compatible but scanning will only work on a Linux OS. The scanners need to be accessible by [SANE](http://www.sane-project.org/) and [ImageMagick](https://imagemagick.org/) needs to be installed and accessible from the command line.
+        2. Pyphe requires Python 3 and a few common packages, available through the [anaconda distribution](https://www.anaconda.com/distribution/).
+        3. Install pyphe by running 'pip install pyphe' in your terminal.
+        4. Open a new terminal and try and run 'pyphe-quantify -h' which should show the help page of one of pyphe's command line tools. On Windows, make sure you are using the Anaconda Prompt, not the Anaconda Powershell Prompt.
+        
+        
+        ## Overview
+        A typical fitness screen with pyphe will involve:
+        1. Image acquisition with [_pyphe-scan_](#pyphe-scan), or [_pyphe-scan-timecourse_](#pyphe-scan-timecourse)
+        2. Quantification of colony properties from images using [_pyphe-quantify_](#pyphe-quantify). In the case of growth curves, parameters are additionally extracted with [_pyphe-growthcurves_](#pyphe-growthcurves).
+        3. Normalisation and data aggregation using [_pyphe-analyse_](#pyphe-analyse).
+        4. Statistics and hit calling using [_pyphe-interpret_](#pyphe-interpret)
+        Please see our paper for a detailed protocol and explanations of the algorithms.
+        
+        
+        ## Support
+        Please check the manuals below carefully, they are also available in the terminal by running the command with the -h option only. If things are still not working, please email me (stephan.kamrad@gmail.com) and I will try and help. If you think you have discovered a bug, or would like to request a new feature, please raise an issue on www.github.com/Bahler-Lab/pyphe.
+        
+        If you get an error like this, make sure you are not using the Anaconda Powershell Prompt:
+        ```python: can't open file 'C:\Users\user1\Anaconda3\Scripts"C:\Users\user1\Anaconda3\Scripts\pyphe-quantify.bat  -h ': [Errno 22] Invalid argument```
+        
+        ## Manual
+        
+        All pyphe tools have a similar command line interface, based on the python argparse package. Generally, parameters are set using --<parameter_name> optionally followed by a value. All _pyphe_ tools can be used with relative file paths so make sure to navigate to the correct working directory before running a _pyphe_ command.
+        
+         
+        ### Pyphe-scan
+        This tools allows you to take consecutive scans of sets of plates, which are then automatically cropped, rotated and named in in a continuos filename scheme of your choice. 
+        
+        #### Prerequisites
+        1. This tool will only run on Linux operating systems and uses the SANE library for image acquisition.
+        
+        2. Make sure your scanner is installed correctly and you can acquire images using the scanimage command. The Gray mode will only work on Epson V800 and V850 scanners (potentially the V700 and V750 model as well) and the TPU8x10 transmission scanning source must be enabled. This should work by default if you are using the V800/850 model and a recent Linux OS. Otherwise, there is excellent documentation available from Zackrisson et al. and the [scanomatics pipeline](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5015956/) for how to make this work using a hacked SANE driver. Please see the instructions in their [wiki](https://github.com/Scan-o-Matic/scanomatic/wiki/Installing-scanners).
+        
+        2. Make sure [ImageMagick](https://imagemagick.org/index.php) is installed and the 'convert' tool can be called from the command line.
+        
+        3. If the Pyphe toolbox has been installed correctly, you should be able to run _pyphe-scan_ in your terminal. 
+        
+        4. With a laser cutter, make a fixture to hold your plates in place. We provide an svg file with the cutting shape in the Documentation directory. Use tape to hold your fixture into place, it should be pushed against the back of the scanner (where the cables are) with the top of the plates facing left. Pyphe-scan and pyphe-quantify come pre-configured for using the provided fixture on an Epson V800/V850 scanner but it is easy to add your own fixture and cropping settings. If you want to use your own fixture, see below of how to add the geometry information to pyphe-scan. 
+        
+        #### Scanning plate batches
+        
+        1. Open the file manager and navigate to the folder in which you want to save your images. The script will create a sub-folder that begins with the current date to save all your images. 
+        
+        2. Right click and select 'Open in Terminal'
+        
+        3. Run scanplates with the options as detaild below. 
+        
+        ```
+        usage: pyphe-scan [-h] [--nplates NPLATES] [--start START] [--prefix PREFIX]
+                          [--postfix POSTFIX] [--fixture {som3_edge,som3}]
+                          [--resolution {150,300,600,900,1200}] [--scanner {1,2,3}]
+                          [--mode {Gray,Color}]
+        
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --nplates NPLATES     Number of plates to scan. This defaults to 100 and the
+                                script can be terminated by Ctr+C when done.
+          --start START         Where to start numbering from. Defaults to 1.
+          --prefix PREFIX       Name prefix for output files. The default is the
+                                current date YYYYMMDD.
+          --postfix POSTFIX     Name postfix for output files. Defaults to empty
+                                string.
+          --fixture {som3_edge,som3,som3-color}
+                                ID of the fixture you are using.
+          --resolution {150,300,600,900,1200}
+                                Resolution for scanning in dpi. Default is 600.
+          --scanner {1,2,3}     Which scanner to use. Scanners are not uniquely
+                                identified and may switch when turned off/unplugged.
+                                This option does not need to be set when only one
+                                scanner is connected.
+          --mode {Gray,Color}   Which color mode to use for scanning. Defaults to
+                                Gray.
+        ```
+        
+        All arguments except the fixture have default values and are optional. A folder prefix_postfix will be created in your current directory and the program will abort if a folder with this name already exists. 
+        
+        
+        
+        ### Pyphe-scan-timecourse
+        
+        This tool acquires image timeseries by scanning in fixed time intervals. For each position in the fixture, a folder is created. Image names contain number of scan. Other options for this tool are similar to [_pyphe-scan_](#pyphe-scan). More than one scanner can be connected and used at the same time. Scanner numbers are defined by the order in which they are connected to the computer. Proceed as follows: (1) disconnect all scanners, (2) prepare the first scanner with plates, connect it and turn it on. (3) start scanning with --scanner 1 option, (4) prepare the second scanner, connect it and turn it on, (5) start scanning with --scanner 2 option. Repeat step (4) and (5), each time incrementing the --scanner argument. 
+        
+        ```
+        usage: pyphe-scan-timecourse [-h] [--nscans NSCANS] [--interval INTERVAL]
+                                     [--prefix PREFIX] [--postfix POSTFIX]
+                                     [--fixture {som3_edge,som3}]
+                                     [--resolution {150,300,600,900,1200}]
+                                     [--scanner {1,2,3}] [--mode {Gray,Color}]
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --nscans NSCANS       Number of time points to scan. This defaults to 100
+                                and the script can be terminated by Ctr+C when done.
+          --interval INTERVAL   Time in minutes between scans. Defaults to 20.
+          --prefix PREFIX       Name prefix for output files. The default is the
+                                current date YYYYMMDD.
+          --postfix POSTFIX     Name postfix for output files. Defaults to empty
+                                string.
+          --fixture {som3_edge,som3,som3-color}
+                                ID of the fixture you are using.
+          --resolution {150,300,600,900,1200}
+                                Resolution for scanning in dpi. Default is 600.
+          --scanner {1,2,3}     Which scanner to use. Scanners are not uniquely
+                                identified and may switch when turned off/unplugged.
+                                This option does not need to be set when only one
+                                scanner is connected.
+          --mode {Gray,Color}   Which color mode to use for scanning. Defaults to
+                                Gray.
+        ```
+        
+        
+        ### Pyphe-growthcurves
+        This tool performs non-parametric analysis of growth curves. It was written specifically to analyse colony size timeseries data obtained with _pyphe-quantify_ _timeseries_.
+        
+        It is important that your csv with the growth data is in the right format. The file must contain one growth curve per column. The first column must be the timepoints and there must be a header row with unique identifiers for each curve. For example data and expected outputs, check out the files included in this Documentation folder. Sensible default parameters are set for all options but, depending on your data, you may wish to customise these, so check out the help section below. 
+        
+        ```
+        usage: pyphe-growthcurves [-h] --input INPUT [--fitrange FITRANGE]
+                                  [--lag-method {abs,rel}]
+                                  [--lag-threshold LAG_THRESHOLD]
+                                  [--t0-fitrange T0_FITRANGE] [--plots]
+                                  [--plot-ylim PLOT_YLIM]
+        
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --input INPUT         Path to the growth curve file to analyse. This file
+                                contains one growth curve per column. The first column
+                                must be the timepoints and there must be a header row
+                                with unique identifiers for each curve.
+          --fitrange FITRANGE   Number of timepoint over which to fit linear
+                                regression. Defaults to 4. Please adjust this to the
+                                density of your timepoints and use higher values for
+                                more noisy data.
+          --lag-method {abs,rel}
+                                Method to use for determining lag. "abs" will measure
+                                time until the defined biomass threshold is crossed.
+                                "rel" will fist determine the inital biomass and
+                                measure the time until the biomass has passed this
+                                value times the threshold. Defaults to "rel".
+          --lag-threshold LAG_THRESHOLD
+                                Threshold to use for determining lag. With method
+                                "abs", this will measure time until the defined
+                                biomass threshold is crossed. With "rel" will fist
+                                determine the inital biomass and measure the time
+                                until the biomass has passed this value times the
+                                threshold. Defaults to 2.0, so with method "rel", this
+                                will measure the time taken for the first doubling.
+          --t0-fitrange T0_FITRANGE
+                                Specify the number of timepoint to use at the
+                                beginning of the growth curve to determine the initial
+                                biomass by averaging them. Defaults to 3.
+          --plots               Set this option (no argument required) to produce a
+                                plot of all growthcurves as pdf.
+          --plot-ylim PLOT_YLIM
+                                Specify the upper limit of the y-axis of growth curve
+                                plots. Useful if you want curves to be directly
+                                comparable. If not set, the axis of each curve is
+                                scaled to the data.
+        ```
+        
+        
+        #### Interpreting results
+        Pyphe-growthcurves will produce a csv file with extracted growth parameters. The maximum slope is determined by fitting all possible linear regressions in sliding windows of length n and chosing the one with the highest slope. The lag phase is determined as the first timepoint which exceeds a settable relative or absolute threshold. 
+        
+        | Parameter        | Explanation  |
+        | ---------------- |---------------|
+        |initial biomass|The average of the first n timepoints of the growth curve|
+        |lag |  Lag phase |
+        | max_slope| The maximum slope of the growth curve|
+        | r2 | The R2 parameter of the linear regression that produced the highest maximum slope |
+        |t_max | Time at which maximum growth slope is reached (center of the sliding window)|
+        |y-intercept|Y-intercept of the regression which produced the maximum slope|
+        |x-intercept|X-intercept of the regression which produced the maximum slope. This is interpreted as lag phase by some people|
+        
+                                    
+        
+        ### Pyphe-quantify
+        
+        Pyphe quantify extracts colony parameters from images. In can operate in three distinct modes analysing colony sizes for each image individually (batch mode), analysing redness for each image individually (redness mode) or obtaining a growth curve from an image timeseries (timeseries mode).
+        The --grid parameter is required define the position of colonies on the plate. You can either use automatic grid detection, one of our preconfigured positions if you are using the pp3 fixture or define your own (see the manual below). Images can be in any format (e.g. jpg, tiff, png). Images should be cropped closely to the colonies (this is important for good thresholding and automatic grid detection), i.e. not contain parts of the plate edges or surroundings. In batch and timecourse mode, pyphe-quantify assumes that images were acquired using transmission scanning, where colonies appear darker then the surrounding agar. If this is not the case and you took images by reflective scanning or with a camera, use --negate False. In batch and timecourse mode, images are epxected to be grayscale. If they are not, they will be converted (by simply summing all channels) and a warning will be thrown. 
+        
+        
+        ```
+        usage: pyphe-quantify [-h] --grid GRID [--pattern PATTERN] [--t T] [--d D]
+                              [--s S] [--negate NEGATE] [--localThresh] [--convexhull]
+                              [--reportAll] [--reportFileNames]
+                              [--hardImageThreshold HARDIMAGETHRESHOLD]
+                              [--hardSizeThreshold HARDSIZETHRESHOLD] [--qc QC]
+                              [--calibrate CALIBRATE] [--timepoints TIMEPOINTS]
+                              [--out OUT]
+                              {batch,timecourse,redness}
+        
+        Welcome to pyphe-quantify, part of the pyphe toolbox. Written by
+        stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
+        Lab/pyphe
+        
+        positional arguments:
+          {batch,timecourse,redness}
+                                Pyphe-quantify can be run in three different modes. In
+                                batch mode, it quantifies colony sizes for all images
+                                matching the pattern individually. A separate results
+                                table and qc image is produced for each. Redness mode
+                                is similar except that the redness of each colony is
+                                quantified. In timecourse mode, all images matching
+                                the pattern are analysed jointly. The final image
+                                matching the pattern is used to create a mask of where
+                                the colonies are and this mask is then applied to all
+                                previous images in the timeseries. A single output
+                                table, where the timepoints are the rows and each
+                                individual colony is a row.
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --grid GRID           This option is required (all others have defaults set)
+                                and specifies the grid in which the colonies are
+                                arranged. You can use automatic grid detection using
+                                one of the following parameters: auto_96, auto_384 or
+                                auto_1536. Automatic grid correction will not work if
+                                the colony grid is not aligned with the image borders.
+                                Images should contain only agar and colonies, avaoid
+                                having borders. It might fail or produce unexpected
+                                results if there are whole rows/columns missing. In
+                                those cases, it is easy to define hard-wired grid
+                                positions. If you are using the fixture provided with
+                                pyphe, we have preconfigured these for you. Depending
+                                on the pinning density, use pp3_96, pp3_384 or
+                                pp3_1536. Otherwise, the argument has to be in the
+                                form of 6 integer numbers separated by "-": <number of
+                                colony rows>-<number of colony columns>-<x-position of
+                                the top left colony>-<y-position of the top left
+                                colony>-<x-position of the bottom right
+                                colony>-<y-position of the bottom right colony>.
+                                Positions must be integers and are the distance in
+                                number of pixels from the image origin in each
+                                dimension (x is width dimension, y is height
+                                dimension). The image origin is, in line with scikit-
+                                image, in the top left corner. Pixel positions are
+                                easily determined using programs such as Microsoft
+                                Paint, by simply hovering the mouse over a position.
+          --pattern PATTERN     Pattern describing files to analyse. This follows
+                                standard unix convention and can be used to specify
+                                subfolders in which to look for images
+                                (<subfolder>/*.jpg) or the image format (*.tiff,
+                                *.png, etc.). By default, all jpg images in the
+                                working directory are analysed.
+          --t T                 By default the intensity threshold to distinguish
+                                colonies from the background is determined by the Otsu
+                                method. The determined value will be multiplied by
+                                this argument to give the final threshold. Useful for
+                                easily fine-tuning colony detection.
+          --d D                 The distance between two grid positions will be
+                                divided by this number to compute the maximum distance
+                                a putative colony can be away from its reference grid
+                                position. Decreasing this number towards 2 makes
+                                colony-to-grid-matching more permissive (might help
+                                when some of your plates are at a slight angle or out
+                                of position).
+          --s S                 Detected putative colonies will be filtered by size
+                                and small components (usually image noise) will be
+                                excluded. The default threshold is the image
+                                area*0.00005 and is therefore independent of scanning
+                                resolution. This default is then multiplied by this
+                                argument to give the final threshold. Useful for when
+                                colonies have unusual sizes.
+          --negate NEGATE       In images acquired by transmission scanning, the
+                                colonies are darker than the background. Before
+                                thresholding, the image needs to be inverted/negated.
+                                Defaults to True in timecourse and batch mode, ignored
+                                in redness mode.
+          --localThresh         Use local thresholding in batch and timecourse mode.
+                                This can help when image brightness is very uneven.
+                                Ignored in redness mode where local thresholding is
+                                always applied.
+          --convexhull          Apply convex hull transformation to identified
+                                colonies to fill holes. Useful when working with spots
+                                rather than colonies. Ignored in redness mode.
+                                WARNING: Using this options results in much longer
+                                analysis times.
+          --reportAll           Sometimes, two putative colonies are identified that
+                                are within the distance threshold of a grid position.
+                                By default, only the closest colony is reported. This
+                                can be changed by setting this option (without
+                                parameter). This option allows pyphe quantify to be
+                                used even if colonies are not arrayed in a regular
+                                grid (you still need to provide a grid parameter
+                                though that spans the colonies you are interested i).
+          --reportFileNames     Only for timecourse mode, otherwise ignored. Use
+                                filenames as index for output table instead of
+                                timepoints. Useful when the ordering of timepoints is
+                                not the same as returned by the pattern. Setting this
+                                option overrides the --timepoints argument.
+          --hardImageThreshold HARDIMAGETHRESHOLD
+                                Allows a hard (fixed) intensity threshold in the range
+                                [0,1] to be used instead of Otsu thresholding. Images
+                                intensities are re-scaled to [0,1] before
+                                thresholding. Ignored in timecourse mode.
+          --hardSizeThreshold HARDSIZETHRESHOLD
+                                Allows a hard (fixed) size threshold [number of
+                                pixels] to be used for filtering small colonies.
+          --qc QC               Directory to save qc images in. Defaults to
+                                "qc_images".
+          --calibrate CALIBRATE
+                                Transform background subtracted intensity values by
+                                this function. Function needs to be a single term with
+                                x as the variable and that is valid python code. E.g.
+                                use "2*x**2+1" to square each pixels intensity,
+                                multiply by two and add 1. Defaults to "x", i.e. use
+                                of no calibration. Used only in timecourse mode.
+          --timepoints TIMEPOINTS
+                                In timecourse mode only. Path to a file that specifies
+                                the timepoints of all images in the timeseries. This
+                                is usually the timepoints.txt file created by pyphe-
+                                scan-timecourse. It must contain one entry per line
+                                and have the same number of lines as number of images.
+          --out OUT             Directory to save output files in. Defaults to
+                                "pyphe_quant".
+        ```
+        
+        
+        
+        ### Pyphe-analyse
+        _Pyphe-analyse_ is a tool for spatial normalisation and data aggregation across many plates. It implements a grid normalisation based on the concept proposed by [Zackrisson et al. 2016](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5015956/) and row/column median normalisation. Please see our paper and the protocol in it to find out more. _Pyphe-analyse_ can be run from the command line, with options below, or using the graphical user interface by running _pyphe-analyse-gui_.
+        
+        
+        ```
+        usage: pyphe-analyse.txt [-h] --edt EDT --format
+                                 {gitter,pyphe-redness,pyphe-growthcurves} [--out OUT]
+                                 [--load_layouts]
+                                 [--gridnorm {standard384,standard1536}]
+                                 [--extrapolate_corners] [--rcmedian] [--check CHECK]
+                                 [--qc_plots QC_PLOTS]
+        
+        Welcome to pyphe-analyse, part of the pyphe toolbox. Written by
+        stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
+        Lab/pyphe
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --edt EDT             Path to the Experimental Design Table (EDT) listing
+                                all plates of the experiment. The table must be in csv
+                                format, the first column must contain unique plate IDs
+                                and there must be a column named 'Data_path' that
+                                contains abolute or relative file paths to each
+                                plate's data file. A 'Layout_path' column can be
+                                included, see below. Any additional columns included
+                                in this file will bestored in each plate's meta-data
+                                and included in the final data output.
+          --format {gitter,pyphe-redness,pyphe-growthcurves}
+                                Type of inout data.
+          --out OUT             Specifies the path where to save the output data
+                                result. By default, the data report is saved in the
+                                working directory as "pyphe-analyse_data_report.csv"
+                                and will overwrite the file if it exists.
+          --load_layouts        Set this option (without parameters) to load layouts
+                                (requires Layout_path column in the EDT).
+          --gridnorm {standard384,standard1536,1536with384grid}
+                                Perform reference grid normalisation. Standard384
+                                refers to plates which are in 384 (16x24) format with
+                                the reference grid in 96 format in the top left
+                                corner. Standard1536 refers to plates in 1536 format
+                                (32x48( with two 96 reference grids in the top left
+                                and bottom right corners. 1536with384grid refers to
+                                plates in 1536 format with a 384 reference grid in
+                                the top left position.
+          --extrapolate_corners
+                                If working in standard1536 format, set this option to
+                                extrapolate the reference grid in the bottom left and
+                                top right corner. A linear regression will be trained
+                                across all top left and bottom right corners on plates
+                                in the experiment to predict hypothetical grid colony
+                                sizes in the other two corners.
+          --rcmedian            Perform row/column median normalisation. If --gridnorm
+                                will be performed first if both parameters are set.
+          --check CHECK         Check colony sizes after normalisation for negative
+                                and infinite colony sizes *(normalisation artefacts),
+                                throw a warning and set to NA.
+          --qc_plots QC_PLOTS   Specify a folder in which to save qc plots for each
+                                plate.
+        
+        ```
+        
+        
+        ### Pyphe-interpret
+        
+        Pyphe-interpret reports summary statistics and tests for differential fitness using t-tests. It is flexible and can in theory be used with any dataset in tidy format.
+        
+        ```
+        usage: pyphe-interpret [-h] --ld LD [--out OUT] --grouping_column
+                               GROUPING_COLUMN --axis_column AXIS_COLUMN
+                               [--values_column VALUES_COLUMN] --control CONTROL
+                               [--ld_encoding LD_ENCODING] [--circularity CIRCULARITY]
+                               [--set_missing_na]
+        
+        Welcome to pyphe-interpret, part of the pyphe toolbox. Written by
+        stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
+        Lab/pyphe. Pyphe-interpret calculates summary statistics and p-values from the
+        data reports generated by pyphe-analyse. For this, specifiying your column
+        names correctly is crucial. Let us assume you have measured many strains in
+        many conditions. Now you would like to know for each strain in each condition
+        (for each condition-strain pair) if it is "significant". There are essentially
+        two ways of doing this, asking different biological questions. (1) Check for
+        each condition separately (--grouping_column <condition_column>) if there is a
+        significant difference in means between a mutant strain and a control strain
+        (--axis_column <strain_id_column>). Or (2) Check for each strain separately
+        (--grouping_column <strain_id_column>) if there is a significant difference in
+        the means of the strain in the assay condition versus the control condition
+        (--axis_column <condition_column>). The second option tests for condition-
+        specific growth effects (i.e. is does not return significant results if a
+        strain is always faster or always slower growing than the grid strain). In
+        both cases you need to specify the control against which to test using
+        --control and this has to be a value that appears in the axis column. You
+        should define the dependent variable of the t-test using --values_column. FDR
+        correction with the Benjamini-Hochberg method will be applied on each level
+        set of the grouping_column separately, ie for case (1) p-values will be
+        corrected across each strain separately, ie more conditions means more
+        stringent correction, and for case (2) p-values will be corrected for each
+        condition separately, ie more strains means mpre stringent correction.
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --ld LD               Path to the Data Report Table produced by pyphe-
+                                analyse.
+          --out OUT             Specifies the path where to save the output data
+                                result. By default, a table with all replicates will
+                                be saved as pyphe-interpret-report_reps.csv and the
+                                statistic table will be saved as pyphe-interpret-
+                                report_summaryStats.csv in the current working
+                                directory. Existing files will be overwritten.
+          --grouping_column GROUPING_COLUMN
+                                Name of the column in the data report to use for
+                                forming groups on which to perform independent sets of
+                                t-tests.
+          --axis_column AXIS_COLUMN
+                                Name of the column in the data report to repeat
+                                t-tests along within each group. Levels in this column
+                                will be the explanatory/independent variable used for
+                                t-tests.
+          --values_column VALUES_COLUMN
+                                Name of the column in the data report to use as
+                                fitness values. This will be the dependent variable
+                                for t-tests. Defaults to "Colony_size_corr_checked".
+          --control CONTROL     Name of the control to compare against. This must be a
+                                value found in the axis column.
+          --ld_encoding LD_ENCODING
+                                Encoding of the data report table to be passed to
+                                pandas.read_csv().
+          --circularity CIRCULARITY
+                                Exclude colonies from the analysis with a circularity
+                                below the one specified. A circularity of 1
+                                corresponds to a perfect circle. We recommend a
+                                threshold around 0.85.
+          --set_missing_na      Set 0-sized colonies to NA. This is recommended if you
+                                expect no missing colonies in your data, which means
+                                these are probably due to pinning errors.
+        ```
+        
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
```

### Comparing `pyphe-0.981/bin/pyphe-analyse` & `pyphe-0.982/bin/pyphe-analyse`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     parser = argparse.ArgumentParser(description='Welcome to pyphe-analyse, part of the pyphe toolbox. Written by stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-Lab/pyphe')
   
    
     parser.add_argument('--edt', type=str, required=True, help="Path to the Experimental Design Table (EDT) listing all plates of the experiment. The table must be in csv format, the first column must contain unique plate IDs and there must be a column named 'Data_path' that contains absolute or relative file paths to each plate's data file. A 'Layout_path' column can be included, see below. Any additional columns included in this file will be stored in each plate's meta-data and included in the final data output.")
     parser.add_argument('--format', required=True, type=str, choices=['gitter', 'pyphe-quantify-redness', 'pyphe-quantify-batch', 'pyphe-growthcurves'], help='Type of inout data.')
     parser.add_argument('--out', default='pyphe-analyse_data_report.csv', type=str, help='Specifies the path where to save the output data result. By default, the data report is saved in the working directory as "pyphe-analyse_data_report.csv" and will overwrite the file if it exists.')
     parser.add_argument('--load_layouts', default=False, action='store_true', help='Set this option (without parameters) to load layouts (requires Layout_path column in the EDT). Layouts must be a single csv table per plate in the same layout as the plate and without headers or row labels.')
-    parser.add_argument('--gridnorm', type=str, choices=['standard384', 'standard1536'], help='Perform reference grid normalisation. Standard384 refers to plates which are in 384 (16x24) format with the reference grid in 96 format in the top left corner. Standard1536 refers to plates in 1536 format (32x48( with two 96 reference grids in the top left and bottom right corners.')
+    parser.add_argument('--gridnorm', type=str, choices=['standard384', 'standard1536', '1536with384grid'], help='Perform reference grid normalisation. Standard384 refers to plates which are in 384 (16x24) format with the reference grid in 96 format in the top left corner. Standard1536 refers to plates in 1536 format (32x48( with two 96 reference grids in the top left and bottom right corners. 1536with384grid refers to plates in 1536 format with a 384 reference grid in the top left position.')
     parser.add_argument('--extrapolate_corners', default=False, action='store_true', help='If working in standard1536 format, set this option to extrapolate the reference grid in the bottom left and top right corner. A linear regression will be trained across all top left and bottom right corners on plates in the experiment to predict hypothetical grid colony sizes in the other two corners.')
     parser.add_argument('--rcmedian', default=False, action='store_true', help='Perform row/column median normalisation. If --gridnorm will be performed first if both parameters are set.')
     parser.add_argument('--nocheck', default=False, action='store_true', help='Check colony sizes after normalisation for negative and infinite colony sizes *(normalisation artefacts), throw a warning and set to NA.')
     parser.add_argument('--qc_plots', type=str, help='Specify a folder in which to save qc plots for each plate.')
 
 
     args = parser.parse_args()
```

### Comparing `pyphe-0.981/bin/pyphe-analyse-gui` & `pyphe-0.982/bin/pyphe-analyse-gui`

 * *Files identical despite different names*

### Comparing `pyphe-0.981/bin/pyphe-growthcurves` & `pyphe-0.982/bin/pyphe-growthcurves`

 * *Files identical despite different names*

### Comparing `pyphe-0.981/bin/pyphe-interpret` & `pyphe-0.982/bin/pyphe-interpret`

 * *Files identical despite different names*

### Comparing `pyphe-0.981/bin/pyphe-quantify` & `pyphe-0.982/bin/pyphe-quantify`

 * *Files identical despite different names*

### Comparing `pyphe-0.981/bin/pyphe-scan` & `pyphe-0.982/bin/pyphe-scan`

 * *Files identical despite different names*

### Comparing `pyphe-0.981/bin/pyphe-scan-timecourse` & `pyphe-0.982/bin/pyphe-scan-timecourse`

 * *Files identical despite different names*

### Comparing `pyphe-0.981/pyphe/analysis.py` & `pyphe-0.982/pyphe/analysis.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,589 +1,594 @@
-import pandas as pd
-from warnings import warn
-import os
-from scipy import interpolate
-import numpy as np
-
-from matplotlib.backends.backend_pdf import PdfPages
-from matplotlib import pyplot as plt
-import seaborn as sns
-sns.set_style('white')
-
-class Experiment():
-    '''
-A pyphe Experiment object facilitates working with a large number of plates/images at the same time. The constructor takes a single argument which is a pandas DataFrame containing some basic information about your experiment. This table should have one line per plate image and should normally contain at least two columns (although column names are not strictly enforced): Assay_plate (which specifies the layout of the plate which we will later read in from a different file) and Image_path (the relative or absolute path to the image file). Normally this file will have additional columns which you can use to keep track of any additional information about the plates, e.g. batch numbers, dates, condition. This information will be retained and propagated into the final output file.  
-It is highly advisable to use a meaningful and unique index for this DataFrame which we can later be used to easily identify individual plots. Alternatively, the pandas default of using interger ranges as index can be used.
-
-Required arguments for creating an Experiment object:
-exp_data (DataFrame) - A DataFrame holding experiment meta-data
-
-An Experiment object has the following attributes:
-exp_data - A DataFrame holding experiment meta-data
-plates - A pandas Series of Plate objects, the index is identical to exp_data
-    '''
-
-    def __init__(self, exp_data):
-        assert not exp_data.index.duplicated().any(), 'Plate IDs must be unique'
-        self.exp_data = exp_data
-
-        self.plates = pd.Series({i : Plate(plateid=i, meta_data=r) for i, r in self.exp_data.iterrows()})
-
-    def update_meta_data(self):
-        '''Update plate meta_data when exp_data has been modified. This is not ideal and could pose a risk of information being overwritten if the user manually edits plate meta-data.'''
-        for i,p in self.plates.iteritems():
-            p.meta_data = self.exp_data.loc[i]
-
-    def generate_long_data(self):
-        '''Make a summary table with all data from all Plates for stats and plotting.
-        Returns:
-        summary_long (pandas DataFrame)
-        '''
-
-        longs = []
-        for i,p in self.plates.iteritems():
-            p_long = p.make_long_data()
-
-            for m in self.exp_data:
-                p_long[m] = [self.exp_data.loc[i,m] for l in p_long.index]
-
-            p_long['Plate'] = i
-            longs.append(p_long)
-
-        summary_long = pd.concat(longs)
-        summary_long.index = range(len(summary_long.index))
-
-        return summary_long
-
-    def batch_gitter(self, plate_format, grid_image_folder='grid_images', dat_file_folder='dat_files', inverse='TRUE', remove_noise='TRUE', autorotate='FALSE', gitter_script_name='gitter_script.R'):
-        '''
-        Wrapper script for gitter. The Experiment object's exp_data must have an Image_path column for this to work.
-        This will write a gitter script into the current directory, which you can execute with Rscr
-
-        Required arguments:
-        plate_format (int) - Plate format in gitter convention 96/384/1536
-
-        Keyword arguments:
-        grid_image_folder (str) - Path of the folder to save the grid images in. Defaults to grid_images
-        dat_file_folder (str) - Path of the folder to save the dat files in. Defaults to dat_files
-        gitter_script_name (str) - Path of the gitter script to be outputted. Defaults to gitter_script.R
-        inverse (str) - Has to be TRUE/FALSE. Invert image before analysis (reuqired for transmission scanning). See gitter documentation.
-        remove_noise (str) - Has to be TRUE/FALSE. Reduce image noise before analysis. See gitter documentation.
-
-        Returns:
-        None
-        '''
-        check_mkdir(grid_image_folder)
-        check_mkdir(dat_file_folder)
-
-        with open(gitter_script_name, 'w') as gs:
-            gs.write('library("gitter")\n')
-            for fpath in self.exp_data['Image_path']:
-                gitter_cmd = 'gitter("%s", plate.format=%i, inverse="%s", remove.noise="%s", grid.save="%s", dat.save="%s", autorotate="%s")'%(fpath, plate_format, inverse, remove_noise, grid_image_folder, dat_file_folder, autorotate)
-                gs.write(gitter_cmd+'\n')
-
-        self.exp_data['Data_path'] = dat_file_folder + '/' + self.exp_data['Image_path'].map(lambda x: x.split('/')[-1]) + '.dat'
-        self.exp_data['Gitter_grid_path'] = grid_image_folder + '/gridded_' + self.exp_data['Image_path'].map(lambda x: x.split('/')[-1])
-
-        self.update_meta_data()
-
-        print('Gitter script created, please run the following command: Rscript %s'%gitter_script_name)
-
-
-class Plate():
-    '''This object holds all data for a single plate. Two empty, all-purpose pandas series are initilased to hold the bulk of the data associated with the Plate object: Plate.meta_data can be used to store meta data of all sorts and these will be included in the output report. Plate.pos_data is used to store pandas dataframes that have the same shape as the gridformat and are used to store actual growth data and analysis results.
-    Keyword arguments:
-    meta_data (Series) - A pandas series containing meta-information about the plate.
-    '''
-    
-    def __init__(self, meta_data=None, plateid=None):
-        self.plateid = plateid
-        self.meta_data = meta_data
-        self.pos_data = pd.Series()
-
-    def read_gitter_single_image(self):
-        '''Read gitter data from file. Adds two new DataFrames to the Plate's pos_data Series, for colony size and one for circularity. The path of the dat file is taken from the PLate's meta_data.'''
-
-        dat = pd.read_csv(self.meta_data['Data_path'], comment='#', header=None, names=['row', 'col', 'size', 'circularity', 'flags'], sep='\t')
-        
-        size = dat.pivot(index='row', columns='col', values='size')
-        size.index.name = None
-        size.index = size.index.map(str)
-        size.columns.name = None
-        size.columns = size.columns.map(str)
-        self.pos_data['Colony_size'] = size
-        
-        circularity = dat.pivot(index='row', columns='col', values='circularity')
-        circularity.index.name = None
-        circularity.index = circularity.index.map(str)
-        circularity.columns.name = None
-        circularity.columns = circularity.columns.map(str)
-        self.pos_data['Colony_circularity'] = circularity
-        
-    def read_pypheredness_single_image(self):
-        '''Read  column from pyphe-quantify redness output file'''
-        
-        dat = pd.read_csv(self.meta_data['Data_path'])
-
-        size = dat.pivot(index='row', columns='column', values='mean_intensity')
-        size.index.name = None
-        size.index = size.index.map(str)
-        size.columns.name = None
-        size.columns = size.columns.map(str)
-        self.pos_data['Colony_size'] = size
-
-        circularity = dat.pivot(index='row', columns='column', values='circularity')
-        circularity.index.name = None
-        circularity.index = circularity.index.map(str)
-        circularity.columns.name = None
-        circularity.columns = circularity.columns.map(str)
-        self.pos_data['Colony_circularity'] = circularity
-    
-    def read_pyphebatch_single_image(self):
-        '''Read  column from pyphe-quantify redness output file'''
-        
-        dat = pd.read_csv(self.meta_data['Data_path'])
-
-        size = dat.pivot(index='row', columns='column', values='area')
-        size.index.name = None
-        size.index = size.index.map(str)
-        size.columns.name = None
-        size.columns = size.columns.map(str)        
-        self.pos_data['Colony_size'] = size
-             
-        circularity = dat.pivot(index='row', columns='column', values='circularity')
-        circularity.index.name = None
-        circularity.index = circularity.index.map(str)
-        circularity.columns.name = None
-        circularity.columns = circularity.columns.map(str)
-        self.pos_data['Colony_circularity'] = circularity
-        
-    def read_pgc_single_image(self):
-        '''Read pyphe-growthcurves output file'''
-        
-        dat = pd.read_csv(self.meta_data['Data_path'], index_col=0).transpose()
-        
-        dat['Row'] = dat.index.map(lambda x: int(x.split('-')[0]))
-        dat['Column'] = dat.index.map(lambda x: int(x.split('-')[1]))
-
-        for c in ['initial biomass', 'lag', 'r2', 't_max', 'y-intercept', 'x-intercept', 'max_slope']:
-            tf = dat.pivot(index='Row', columns='Column', values=c)
-            tf = tf.sort_index().sort_index(axis=1)
-            tf.index = tf.index.map(str)
-            tf.columns = tf.columns.map(str)
-            
-            if c == 'max_slope':
-                self.pos_data['Colony_size'] = tf.astype(float)
-            else:
-                self.pos_data[c] = tf.astype(float)
-
-        
-    def read_layout_single_plate(self, kwargs={'header':None}):
-        '''Read the layout of a single file in wide format. This is essentially a wrapper for pandas' read_csv() function which will store returned DataFrame in the pos_data Series of the plate instance. The path of the layout file needs to be provided in the exp_data file in a column named Layout_path. The layout file should not have any header or index information but this can be overriden by supplying keyword arguments as a dictionary to the kwargs argument. Any keyword arguments provided will be passed to pandas' read_csv() function.'''
-        
-        imported = pd.read_csv(self.meta_data['Layout_path'], **kwargs)
-        imported.index = map(str, range(1, len(imported.index)+1))
-        imported.columns = map(str, range(1, len(imported.columns)+1))
-
-        self.pos_data['Strain'] = imported
-        
-    def rcmedian_normalisation(self, inkey='Colony_size', outkey='Colony_size_corr'):
-        '''This function implements row/column median normalisation with smoothing of row/column medians across plates.
-
-        Required aguments:
-        inkey (str) -- The key in pos_data which to use as input
-        outkey (str) -- The key in pos_data under which to store the result
-        Returns:
-        None
-        '''
-
-        col_medians = self.pos_data[inkey].median(axis=0)
-        row_medians = self.pos_data[inkey].median(axis=1)
-
-        normed = self.pos_data[inkey].div(row_medians, axis='index')
-        normed = normed.div(col_medians, axis='columns')
-        normed = normed/normed.stack().median()
-        self.pos_data[outkey] = normed
-
-    def grid_normalisation(self, gridpos_list, inkey='Colony_size', outkey='Colony_size_corr', set_missing_nan=True, remove_grid_outliers=False, k=3, extrapolate_corners=False, horizontal_neighbour_coeff=None, vertical_neighbour_coeff=None,  intercept_coeff=None):
-        
-        '''Apply reference-grid normalisation to quantitative colony data stored in pos_data. First, the data of the grid colonies is extracted from pos_data[inkey], based on the provided list of control positions. There is an option to filter out extreme grid outliers (e.g. due to pinning errors) using a z-score cut-off based on the overall distribution of grid colony values. In this implementation of the grid normalisation it is only possible to extrapolate the lower left and upper right corners of 1536 plates. The grid must be placed as two 96 grids, in the upper left and lower right corner. Please do not use this option if those conditions are not met. Finally, the grid is interpolated using 2d cubic interpolation as implemented in scipy's interpolate.griddata() function. The corrected values are computed by dividing the acutal colony value by the expected (interpolated) value and the result is stored as a new DataFrame in the plate's pos_data.
-
-        Required arguments:
-
-        gridpos_list (list) -- list of two-length tuples, containing row and column positions as integers)
-        remove_grid_outliers (bool) -- Should extreme outliers in reference grid be removed? This leads to loss of data if positions are on edge of grid.  
-
-        Keyword arguments:
-        set_missing_nan (bool) - Set colonies near grid positions which are 0 or nan (usually indicating pinning errors) to nan (Recommended).
-        inkey (str) -- The key in pos_data which to use as input. Defaults to Colony_size.
-        outkey (str) -- The key in pos_data under which to store the result. Defaults to Colony_size_corr.
-        remove_outliers (bool) -- Reemove grid outliers with a z-score of more than k, if they are not on the edge.
-        k (float) -- Grid positions with a Z-score of greater than k will be removed from grid. Only required when remove_grid_outliers is True, otherwise ignored.
-
-        Returns:
-        None
-        '''
-            
-        grid = pd.DataFrame(index=self.pos_data[inkey].index, columns=self.pos_data[inkey].columns, dtype=float)
-        for row, col in gridpos_list:
-            grid.loc[str(row), str(col)] = self.pos_data[inkey].loc[str(row), str(col)]
-
-        #Look for areas where the grid is nan or 0
-        na_mask = pd.DataFrame(False, index=self.pos_data[inkey].index, columns=self.pos_data[inkey].columns, dtype=bool)
-        nan_zero_count = 0
-        for row, col in gridpos_list:
-            if (pd.isnull(grid.loc[str(row), str(col)])) or (grid.loc[str(row), str(col)] == 0.0):
-                nan_zero_count += 1
-                
-                #Set this to NA in the grid itself
-                grid.loc[str(row), str(col)] = np.nan
-
-                #Set the neighbours and the field itself in the NA_mask to NAN
-                na_mask.loc[str(row), str(col)] = True
-                na_mask.loc[str(row), str(col+1)] = True
-                na_mask.loc[str(row), str(col-1)] = True
-                na_mask.loc[str(row+1), str(col)] = True
-                na_mask.loc[str(row-1), str(col)] = True
-                na_mask.loc[str(row+1), str(col+1)] = True
-                na_mask.loc[str(row-1), str(col+1)] = True
-                na_mask.loc[str(row+1), str(col-1)] = True
-                na_mask.loc[str(row-1), str(col-1)] = True
-                
-        #Need to remove any new columns/rows added on the edge and need to recast type to bool
-        na_mask = na_mask.loc[self.pos_data[inkey].index, self.pos_data[inkey].columns].astype(bool)
-                
-        self.pos_data['Near_missing_grid'] = pd.DataFrame(na_mask, index=self.pos_data[inkey].index, columns=self.pos_data[inkey].columns, dtype=bool)
-
-        if nan_zero_count > 0:
-            if set_missing_nan:
-                #Check for grid colonies that didn't grow and report
-                print('Plate %s: %i grid colonies have size 0, probably due to pinning errors. These and neighbouring colonies will be set to nan.'%(self.plateid, nan_zero_count))
-            else:
-                #Check for grid colonies that didn't grow and throw a warning
-                print('Plate %s: %i grid colonies have size 0, probably due to pinning errors. I will ignore this for now and interpolate grid values based on surrounding grid colonies. However, it is recommended that you set these to nan. Affected colonies are marked in the Near_missing_grid column.'%(self.plateid, nan_zero_count))
-
-        if remove_grid_outliers:
-            #Calculate z-scores
-            sigma = grid.unstack().std()  # std dev of all ref colonies
-            mu = grid.unstack().mean()    # mean  of all ref colonies
-
-            z_scores = grid - mu
-            z_scores = z_scores / sigma
-            z_score_mask = z_scores.abs()>k
-
-            #Whatever the z-score, dont remove grid positions on edges of plate, this leads to missing data and these are more variable in general
-            z_score_mask.iloc[:,0] = False
-            z_score_mask.iloc[0,:] = False
-            z_score_mask.iloc[:,-1] = False
-            z_score_mask.iloc[-1,:] = False
-
-            grid[z_score_mask] = np.nan
-            print('Plate %s: Removed %i outlier grid colonies'%(self.plateid, z_score_mask.unstack().sum()))
-
-        if extrapolate_corners:
-            #warn('In this implementation of the grid normalisation it is only possible to extrapolate the lower left and upper right corners of 1536 plates. The grid must be placed as two 96 grids, in the upper left and lower right corner. Please do not use this option if those conditions are not met.')
-            grid.loc['32','1'] = intercept_coeff + horizontal_neighbour_coeff*grid.loc['32','4'] + vertical_neighbour_coeff*grid.loc['29','1']
-            grid.loc['1','48'] = intercept_coeff + horizontal_neighbour_coeff*grid.loc['1','45'] + vertical_neighbour_coeff*grid.loc['4','48']
-
-
-        self.pos_data['Grid'] = grid
-
-
-        #Calculate reference surface
-        #Get new list of grid positions after extrapolation and noise filtering
-        grid_us = grid.unstack().dropna().reset_index()
-        grid_us.columns = ['col', 'row', 'val']
-        gridpos_list_new = grid_us[['row', 'col']].values
-        values = grid_us['val'].values
-
-        #Points to interpolate
-        xi = grid.unstack()
-        xi = xi[pd.isnull(xi)]
-        xi = xi.reset_index()
-        xi.columns = ['col', 'row', 'val']
-        xi = xi[['row', 'col']].values
-
-        #interpolate
-        interpolated = interpolate.griddata(gridpos_list_new, values, xi, method='cubic')
-
-        ref_surface = pd.DataFrame(index=self.pos_data[inkey].index, columns=self.pos_data[inkey].columns, dtype=float)
-        for i,p in enumerate(gridpos_list_new):
-            ref_surface.loc[str(p[0]), str(p[1])] = grid.loc[str(p[0]), str(p[1])]
-        for i,p in enumerate(xi):
-            ref_surface.loc[str(p[0]), str(p[1])] = interpolated[i]
-        self.pos_data['Reference_surface'] = ref_surface
-
-        #Get ratio of max slope to wild type
-        corr_data = self.pos_data[inkey]/ref_surface
-        if set_missing_nan:
-            corr_data[na_mask] = np.nan
-        self.pos_data[outkey] = corr_data
-        
-    def plot_pos_data(self, pdf_path=None, toPlot=None):
-        '''Plot DataFrames containing numerical values as heatmaps using seaborn and matplotlib.
-        Keyword arguments:
-        pdf_path -- This option is highly recommended when you are dealing with large batches of Plates. It saves figures to pdf and then closes them so that they do not build up in memory. Please provide the name of a folder to save pdfs in, the filename is identical to the plateid.
-        toPlot (list) -- List of data to plot. Must be keys of Plate.pos_data. If not set, all DataFrames in pos_data which contain numeric values will be plotted.
-
-        Returns:
-        None
-        '''
-        
-        if not toPlot:
-            toPlot = []
-            for i, fr in self.pos_data.iteritems():
-                try:
-                    fr.astype(float)#Select only DataFrames which can be cast to numeric.
-                    toPlot.append(i)
-                except Exception:
-                    pass
-
-        if pdf_path:
-            pdf = PdfPages(os.path.join(pdf_path, str(self.plateid))+'.pdf')
-
-        for key in toPlot:
-            fig, ax = plt.subplots()
-            sns.heatmap(data=self.pos_data[key], ax=ax)
-            ax.set_title(key)
-            if pdf:
-                pdf.savefig()
-                fig.clf()
-                plt.close(fig)
-                
-        if pdf_path:
-            pdf.close()
-            
-    def check_values(self, inkey='Colony_size_corr', outkey='Colony_size_corr_checked', negative_action=0, inf_action=10):
-        ''' This function checks for invalid values in plate pos data. Normalisation procedures can produce invalid values 
-        as side effect, such as negative or infinite fitness values. This function detects those and deals with them in 
-        a custamisable way.
-
-        Keyworkd arguments:
-        inkey (str) -- The data to use (must be a key in exp.plates.pos_data)
-        negative_action (float) -- Value to assign to negative fitness. Defaults to 0. np.nan is allowed too. Set to None if no action required.
-        inf_action (float) -- Value to assign to inf values. Defaults to 10. np.nan is allowed too. Set to None if no action required.
-
-        Returns:
-        None (exp.plates.pos_data is modified in place)
-        '''
-
-        data = self.pos_data[inkey]
-        ##In some rare cases the input DataFrame can be empty. In that case, just set to an empty DataFrame
-        if data.empty:
-            self.pos_data[outkey] = pd.DataFrame([[]])
-            return None
-        data = data.unstack()
-
-        #Ignore na
-        data = data.dropna()
-
-        #Check for inf
-        isneginf = data[np.isneginf(data.values)]
-        if len(isneginf.index) != 0:
-            print('Plate %s - The following positions are minus infinity: %s'%(self.plateid, str(dict(isneginf))))
-        isposinf = data[np.isposinf(data.values)]
-        if len(isposinf.index) != 0:
-            print('Plate %s - The following positions are plus infinity: %s'%(self.plateid, str(dict(isposinf))))
-
-        #Check for negative
-        neg = data[~np.isinf(data.values)]
-        neg = neg[neg<0]
-        if len(neg.index) != 0:
-            print('Plate %s - The following positions are negative: %s'%(self.plateid, str(dict(neg))))
-
-        #Actions
-        if inf_action is not None:
-            inf_action = float(inf_action)            
-            if pd.isnull(inf_action):
-                self.pos_data[inkey][np.isinf(self.pos_data[inkey])] = inf_action
-            else:
-                self.pos_data[inkey][np.isneginf(self.pos_data[inkey])] = -inf_action
-                self.pos_data[inkey][np.isposinf(self.pos_data[inkey])] = inf_action
-
-        if negative_action is not None:
-            negative_action = float(negative_action)
-            self.pos_data[outkey] = self.pos_data[inkey].copy()
-            self.pos_data[outkey][self.pos_data[outkey].replace(-np.inf, 1).replace(np.inf, 1).replace(np.nan, 1)<0] = negative_action
-
-
-
-    def make_long_data(self):
-        '''Generate a summary table of all Data stored in this Plate object.
-        Returns:
-        long_data (pandas DataFrame)
-        '''
-        unstacked = []
-        for k, frame in self.pos_data.iteritems():
-            if frame.empty:
-                continue
-            l_unstacked = frame.copy()
-            l_unstacked.columns.name = 'Column'
-            l_unstacked.index.name = 'Row'
-            l_unstacked = l_unstacked.unstack()
-            l_unstacked.name = k
-            unstacked.append(l_unstacked)
-        if len(unstacked) == 0:
-            warn('No data associated with Plate %s. Please check input data'%self.plateid)
-            return pd.DataFrame([[]])
-        else:
-            long_data = pd.concat(unstacked, axis=1)
-            long_data = long_data.reset_index()
-
-        return long_data
-
-def check_mkdir(dirPath):
-    '''
-Create a directory if it does not exist already.
-
-Required arguments:
-dirPath (str) - path of the directory to create.
-'''
-
-    if os.path.exists(dirPath):
-        warn('Directory exist, not doing anything.')
-    else:
-        os.mkdir(dirPath)
-
-
-
-def check_exp_data(exp_data, layouts=False):
-    print('Checking exp_data table')
-    
-    print('Checking if plate IDs (first column) are unique')
-    assert not exp_data.index.duplicated().any(), 'Error, Plate IDs are not unique'
-    print('....OK')
-    
-    print('Checking for mandatory columns')
-    assert 'Data_path' in exp_data.columns, 'Error, table must have Data_path column'
-    if layouts:
-        assert 'Layout_path' in exp_data.columns, 'Error, table must have Layout_path column'
-    print('....OK')
-    
-    print('Checking if data files are unique')
-    assert not exp_data['Data_path'].duplicated().any(), 'Error, data paths are not unique (plates with the same ID have been assigned the same data file).'
-    print('....OK')
-    
-    print('Checking all data files exist')
-    for ip in exp_data['Data_path']:
-        if not os.path.isfile(ip):
-            raise IOError('Data file does not exist: %s'%ip)
-    print('...OK')
-    
-    if layouts:
-        print('Checking all layout files exist')
-        for ip in exp_data['Layout_path']:
-            if not os.path.isfile(ip):
-                raise IOError('Layout file does not exist: %s'%ip)
-        print('...OK')
-
-def pyphe_cmd(wdirectory=None, grid_norm=None, out_ld=None, qcplots=None, check_setNA=None, qcplot_dir=None, exp_data_path=None, extrapolate_corners=None, grid_pos=None, rcmedian=None, input_type=None, load_layouts=None):
-    '''
-    This function was written to be called from the GUI script provided. But it can also be used to run the entire standard pipeline in one place.
-    '''
-    
-    print('###Step 1: Load data###')
-
-    #Set working directory
-    if wdirectory:
-        os.chdir(wdirectory)
-        print('Working directory changed to: %s'%wdirectory)
-    #Import exp_data
-    exp_data = pd.read_csv(exp_data_path, index_col=0)
-    check_exp_data(exp_data, layouts=load_layouts)
-    print('Table checks completed')
-    
-    exp = Experiment(exp_data)
-    print('Created pyphe experiment object')
-    
-    #Load the data
-    if input_type == 'gitter':
-        exp.plates.map(Plate.read_gitter_single_image)
-
-    elif input_type == 'pyphe-quantify-redness':
-        exp.plates.map(Plate.read_pypheredness_single_image)
-        
-    elif input_type == 'pyphe-growthcurves':
-        exp.plates.map(Plate.read_pgc_single_image)
-        
-    elif input_type == 'pyphe-quantify-batch':
-                exp.plates.map(Plate.read_pyphebatch_single_image)
-    
-    else:
-        raise ValueError('Unrecignised input_type')
-    print('Plate data loaded sucessfully')
-    
-    
-    #Load the layouts
-    if load_layouts:
-        exp.plates.map(Plate.read_layout_single_plate)
-        print('Layouts loaded sucessfully')
-    
-    #Perform norms
-    if grid_norm:
-        if input_type == 'pyphe-quantify-redness':
-            raise ValueError('Grid normalisation does not make sense for redness input')
-            
-        print('Performing grid norm')
-
-        if (grid_pos == 'Standard 384 (top left)') or (grid_pos == 'standard384'):
-            gridpos_list = [(row, col) for row in range(1, 16, 2) for col in range(1, 24, 2)]
-        elif (grid_pos == 'Standard 1536 (top left and bottom right)') or (grid_pos == 'standard1536'):
-            gridpos_list = [(row, col) for row in range(1, 32, 4) for col in range(1, 48, 4)]
-            gridpos_list += [(row, col) for row in range(4, 33, 4) for col in range(4, 49, 4)]
-        else:
-            raise ValueError('grid_pos must be one of ["Standard 384 (top left)", "standard384", "Standard 1536 (top left and bottom right)", "standard1536"]')
-
-
-        if extrapolate_corners:
-            from sklearn.linear_model import LinearRegression
-            #Make a table of  features
-            vals = pd.DataFrame(columns=['thisCorner', 'horizontalNeighbour', 'verticalNeighbour'])
-            for i,p in exp.plates.iteritems():
-                vals.loc[i+'_topLeft'] = [p.pos_data['Colony_size'].loc['1','1'], p.pos_data['Colony_size'].loc['1','5'], p.pos_data['Colony_size'].loc['5','1']]
-                vals.loc[i+'_bottomRight'] = [p.pos_data['Colony_size'].loc['32','48'], p.pos_data['Colony_size'].loc['32','44'], p.pos_data['Colony_size'].loc['28','48']]
-            mlm = LinearRegression()
-            mlm.fit(vals.iloc[:,1:], vals.iloc[:,0])
-            print('Extrapolating missing corners based on the following regression: ')
-            print('    horizontal_neighbour_coeff: ' +  str(mlm.coef_[0]))
-            print('    vertical_neighbour_coeff: ' +  str(mlm.coef_[1]))
-            print('    intercept_coeff: ' +  str(mlm.intercept_))
-            print('    accuracy: ' +str(mlm.score(vals.iloc[:,1:], vals.iloc[:,0])))
-                        
-            exp.plates.map(lambda x: x.grid_normalisation(gridpos_list, 
-                                                  extrapolate_corners=True, horizontal_neighbour_coeff=mlm.coef_[0], 
-                                                  vertical_neighbour_coeff=mlm.coef_[1],  intercept_coeff=mlm.intercept_))
-                              
-        else:
-            exp.plates.map(lambda x: x.grid_normalisation(gridpos_list) )
-            
-        
-    if rcmedian:
-        print('Performing row/column median normalisation')
-        if grid_norm:
-            ikey = 'Colony_size_corr'
-            okey = 'Colony_size_corr'
-        else:
-            ikey = 'Colony_size'
-            okey = 'Colony_size_corr'
-
-        exp.plates.map(lambda x: x.rcmedian_normalisation(inkey=ikey, outkey=okey))
-    
-    #Perform checks and qc
-    if check_setNA:
-        print('Checking for infinite and negative fitness values')
-        if (not grid_norm) and (not rcmedian):
-            exp.plates.map(lambda x: x.check_values(inkey='Colony_size', outkey='Colony_size_checked', negative_action=np.nan, inf_action=np.nan))
-        else:
-            exp.plates.map(lambda x: x.check_values(inkey='Colony_size_corr', outkey='Colony_size_corr_checked', negative_action=np.nan, inf_action=np.nan))
-        
-    if qcplots:
-        print('Making qc plots')
-        exp.plates.map(lambda x: x.plot_pos_data(pdf_path=qcplot_dir))
-        
-    #Export
-    print('Exporting data')
-    ld = exp.generate_long_data()
-    ld.to_csv(out_ld)
-    print('Done')
-    
-    
+import pandas as pd
+from warnings import warn
+import os
+from scipy import interpolate
+import numpy as np
+
+from matplotlib.backends.backend_pdf import PdfPages
+from matplotlib import pyplot as plt
+import seaborn as sns
+sns.set_style('white')
+
+class Experiment():
+    '''
+A pyphe Experiment object facilitates working with a large number of plates/images at the same time. The constructor takes a single argument which is a pandas DataFrame containing some basic information about your experiment. This table should have one line per plate image and should normally contain at least two columns (although column names are not strictly enforced): Assay_plate (which specifies the layout of the plate which we will later read in from a different file) and Image_path (the relative or absolute path to the image file). Normally this file will have additional columns which you can use to keep track of any additional information about the plates, e.g. batch numbers, dates, condition. This information will be retained and propagated into the final output file.  
+It is highly advisable to use a meaningful and unique index for this DataFrame which we can later be used to easily identify individual plots. Alternatively, the pandas default of using interger ranges as index can be used.
+
+Required arguments for creating an Experiment object:
+exp_data (DataFrame) - A DataFrame holding experiment meta-data
+
+An Experiment object has the following attributes:
+exp_data - A DataFrame holding experiment meta-data
+plates - A pandas Series of Plate objects, the index is identical to exp_data
+    '''
+
+    def __init__(self, exp_data):
+        assert not exp_data.index.duplicated().any(), 'Plate IDs must be unique'
+        self.exp_data = exp_data
+
+        self.plates = pd.Series({i : Plate(plateid=i, meta_data=r) for i, r in self.exp_data.iterrows()})
+
+    def update_meta_data(self):
+        '''Update plate meta_data when exp_data has been modified. This is not ideal and could pose a risk of information being overwritten if the user manually edits plate meta-data.'''
+        for i,p in self.plates.iteritems():
+            p.meta_data = self.exp_data.loc[i]
+
+    def generate_long_data(self):
+        '''Make a summary table with all data from all Plates for stats and plotting.
+        Returns:
+        summary_long (pandas DataFrame)
+        '''
+
+        longs = []
+        for i,p in self.plates.iteritems():
+            p_long = p.make_long_data()
+
+            for m in self.exp_data:
+                p_long[m] = [self.exp_data.loc[i,m] for l in p_long.index]
+
+            p_long['Plate'] = i
+            longs.append(p_long)
+
+        summary_long = pd.concat(longs)
+        summary_long.index = range(len(summary_long.index))
+
+        return summary_long
+
+    def batch_gitter(self, plate_format, grid_image_folder='grid_images', dat_file_folder='dat_files', inverse='TRUE', remove_noise='TRUE', autorotate='FALSE', gitter_script_name='gitter_script.R'):
+        '''
+        Wrapper script for gitter. The Experiment object's exp_data must have an Image_path column for this to work.
+        This will write a gitter script into the current directory, which you can execute with Rscr
+
+        Required arguments:
+        plate_format (int) - Plate format in gitter convention 96/384/1536
+
+        Keyword arguments:
+        grid_image_folder (str) - Path of the folder to save the grid images in. Defaults to grid_images
+        dat_file_folder (str) - Path of the folder to save the dat files in. Defaults to dat_files
+        gitter_script_name (str) - Path of the gitter script to be outputted. Defaults to gitter_script.R
+        inverse (str) - Has to be TRUE/FALSE. Invert image before analysis (reuqired for transmission scanning). See gitter documentation.
+        remove_noise (str) - Has to be TRUE/FALSE. Reduce image noise before analysis. See gitter documentation.
+
+        Returns:
+        None
+        '''
+        check_mkdir(grid_image_folder)
+        check_mkdir(dat_file_folder)
+
+        with open(gitter_script_name, 'w') as gs:
+            gs.write('library("gitter")\n')
+            for fpath in self.exp_data['Image_path']:
+                gitter_cmd = 'gitter("%s", plate.format=%i, inverse="%s", remove.noise="%s", grid.save="%s", dat.save="%s", autorotate="%s")'%(fpath, plate_format, inverse, remove_noise, grid_image_folder, dat_file_folder, autorotate)
+                gs.write(gitter_cmd+'\n')
+
+        self.exp_data['Data_path'] = dat_file_folder + '/' + self.exp_data['Image_path'].map(lambda x: x.split('/')[-1]) + '.dat'
+        self.exp_data['Gitter_grid_path'] = grid_image_folder + '/gridded_' + self.exp_data['Image_path'].map(lambda x: x.split('/')[-1])
+
+        self.update_meta_data()
+
+        print('Gitter script created, please run the following command: Rscript %s'%gitter_script_name)
+
+
+class Plate():
+    '''This object holds all data for a single plate. Two empty, all-purpose pandas series are initilased to hold the bulk of the data associated with the Plate object: Plate.meta_data can be used to store meta data of all sorts and these will be included in the output report. Plate.pos_data is used to store pandas dataframes that have the same shape as the gridformat and are used to store actual growth data and analysis results.
+    Keyword arguments:
+    meta_data (Series) - A pandas series containing meta-information about the plate.
+    '''
+    
+    def __init__(self, meta_data=None, plateid=None):
+        self.plateid = plateid
+        self.meta_data = meta_data
+        self.pos_data = pd.Series()
+
+    def read_gitter_single_image(self):
+        '''Read gitter data from file. Adds two new DataFrames to the Plate's pos_data Series, for colony size and one for circularity. The path of the dat file is taken from the PLate's meta_data.'''
+
+        dat = pd.read_csv(self.meta_data['Data_path'], comment='#', header=None, names=['row', 'col', 'size', 'circularity', 'flags'], sep='\t')
+        
+        size = dat.pivot(index='row', columns='col', values='size')
+        size.index.name = None
+        size.index = size.index.map(str)
+        size.columns.name = None
+        size.columns = size.columns.map(str)
+        self.pos_data['Colony_size'] = size
+        
+        circularity = dat.pivot(index='row', columns='col', values='circularity')
+        circularity.index.name = None
+        circularity.index = circularity.index.map(str)
+        circularity.columns.name = None
+        circularity.columns = circularity.columns.map(str)
+        self.pos_data['Colony_circularity'] = circularity
+        
+    def read_pypheredness_single_image(self):
+        '''Read  column from pyphe-quantify redness output file'''
+        
+        dat = pd.read_csv(self.meta_data['Data_path'])
+
+        size = dat.pivot(index='row', columns='column', values='mean_intensity')
+        size.index.name = None
+        size.index = size.index.map(str)
+        size.columns.name = None
+        size.columns = size.columns.map(str)
+        self.pos_data['Colony_size'] = size
+
+        circularity = dat.pivot(index='row', columns='column', values='circularity')
+        circularity.index.name = None
+        circularity.index = circularity.index.map(str)
+        circularity.columns.name = None
+        circularity.columns = circularity.columns.map(str)
+        self.pos_data['Colony_circularity'] = circularity
+    
+    def read_pyphebatch_single_image(self):
+        '''Read  column from pyphe-quantify redness output file'''
+        
+        dat = pd.read_csv(self.meta_data['Data_path'])
+
+        size = dat.pivot(index='row', columns='column', values='area')
+        size.index.name = None
+        size.index = size.index.map(str)
+        size.columns.name = None
+        size.columns = size.columns.map(str)        
+        self.pos_data['Colony_size'] = size
+             
+        circularity = dat.pivot(index='row', columns='column', values='circularity')
+        circularity.index.name = None
+        circularity.index = circularity.index.map(str)
+        circularity.columns.name = None
+        circularity.columns = circularity.columns.map(str)
+        self.pos_data['Colony_circularity'] = circularity
+        
+    def read_pgc_single_image(self):
+        '''Read pyphe-growthcurves output file'''
+        
+        dat = pd.read_csv(self.meta_data['Data_path'], index_col=0).transpose()
+        
+        dat['Row'] = dat.index.map(lambda x: int(x.split('-')[0]))
+        dat['Column'] = dat.index.map(lambda x: int(x.split('-')[1]))
+
+        resvars = ['initial biomass', 'lag', 'r2', 't_max', 'y-intercept', 'x-intercept', 'max_slope', 'sum of values (AUC)', 'maximum']
+        resvars = [s for s in resvars if s in dat.columns]
+        
+        for c in resvars:
+            tf = dat.pivot(index='Row', columns='Column', values=c)
+            tf = tf.sort_index().sort_index(axis=1)
+            tf.index = tf.index.map(str)
+            tf.columns = tf.columns.map(str)
+            
+            if c == 'max_slope':
+                self.pos_data['Colony_size'] = tf.astype(float)
+            else:
+                self.pos_data[c] = tf.astype(float)
+                
+        
+    def read_layout_single_plate(self, kwargs={'header':None}):
+        '''Read the layout of a single file in wide format. This is essentially a wrapper for pandas' read_csv() function which will store returned DataFrame in the pos_data Series of the plate instance. The path of the layout file needs to be provided in the exp_data file in a column named Layout_path. The layout file should not have any header or index information but this can be overriden by supplying keyword arguments as a dictionary to the kwargs argument. Any keyword arguments provided will be passed to pandas' read_csv() function.'''
+        
+        imported = pd.read_csv(self.meta_data['Layout_path'], **kwargs)
+        imported.index = map(str, range(1, len(imported.index)+1))
+        imported.columns = map(str, range(1, len(imported.columns)+1))
+
+        self.pos_data['Strain'] = imported
+        
+    def rcmedian_normalisation(self, inkey='Colony_size', outkey='Colony_size_corr'):
+        '''This function implements row/column median normalisation with smoothing of row/column medians across plates.
+
+        Required aguments:
+        inkey (str) -- The key in pos_data which to use as input
+        outkey (str) -- The key in pos_data under which to store the result
+        Returns:
+        None
+        '''
+
+        col_medians = self.pos_data[inkey].median(axis=0)
+        row_medians = self.pos_data[inkey].median(axis=1)
+
+        normed = self.pos_data[inkey].div(row_medians, axis='index')
+        normed = normed.div(col_medians, axis='columns')
+        normed = normed/normed.stack().median()
+        self.pos_data[outkey] = normed
+
+    def grid_normalisation(self, gridpos_list, inkey='Colony_size', outkey='Colony_size_corr', set_missing_nan=True, remove_grid_outliers=False, k=3, extrapolate_corners=False, horizontal_neighbour_coeff=None, vertical_neighbour_coeff=None,  intercept_coeff=None):
+        
+        '''Apply reference-grid normalisation to quantitative colony data stored in pos_data. First, the data of the grid colonies is extracted from pos_data[inkey], based on the provided list of control positions. There is an option to filter out extreme grid outliers (e.g. due to pinning errors) using a z-score cut-off based on the overall distribution of grid colony values. In this implementation of the grid normalisation it is only possible to extrapolate the lower left and upper right corners of 1536 plates. The grid must be placed as two 96 grids, in the upper left and lower right corner. Please do not use this option if those conditions are not met. Finally, the grid is interpolated using 2d cubic interpolation as implemented in scipy's interpolate.griddata() function. The corrected values are computed by dividing the acutal colony value by the expected (interpolated) value and the result is stored as a new DataFrame in the plate's pos_data.
+
+        Required arguments:
+
+        gridpos_list (list) -- list of two-length tuples, containing row and column positions as integers)
+        remove_grid_outliers (bool) -- Should extreme outliers in reference grid be removed? This leads to loss of data if positions are on edge of grid.  
+
+        Keyword arguments:
+        set_missing_nan (bool) - Set colonies near grid positions which are 0 or nan (usually indicating pinning errors) to nan (Recommended).
+        inkey (str) -- The key in pos_data which to use as input. Defaults to Colony_size.
+        outkey (str) -- The key in pos_data under which to store the result. Defaults to Colony_size_corr.
+        remove_outliers (bool) -- Reemove grid outliers with a z-score of more than k, if they are not on the edge.
+        k (float) -- Grid positions with a Z-score of greater than k will be removed from grid. Only required when remove_grid_outliers is True, otherwise ignored.
+
+        Returns:
+        None
+        '''
+            
+        grid = pd.DataFrame(index=self.pos_data[inkey].index, columns=self.pos_data[inkey].columns, dtype=float)
+        for row, col in gridpos_list:
+            grid.loc[str(row), str(col)] = self.pos_data[inkey].loc[str(row), str(col)]
+
+        #Look for areas where the grid is nan or 0
+        na_mask = pd.DataFrame(False, index=self.pos_data[inkey].index, columns=self.pos_data[inkey].columns, dtype=bool)
+        nan_zero_count = 0
+        for row, col in gridpos_list:
+            if (pd.isnull(grid.loc[str(row), str(col)])) or (grid.loc[str(row), str(col)] == 0.0):
+                nan_zero_count += 1
+                
+                #Set this to NA in the grid itself
+                grid.loc[str(row), str(col)] = np.nan
+
+                #Set the neighbours and the field itself in the NA_mask to NAN
+                na_mask.loc[str(row), str(col)] = True
+                na_mask.loc[str(row), str(col+1)] = True
+                na_mask.loc[str(row), str(col-1)] = True
+                na_mask.loc[str(row+1), str(col)] = True
+                na_mask.loc[str(row-1), str(col)] = True
+                na_mask.loc[str(row+1), str(col+1)] = True
+                na_mask.loc[str(row-1), str(col+1)] = True
+                na_mask.loc[str(row+1), str(col-1)] = True
+                na_mask.loc[str(row-1), str(col-1)] = True
+                
+        #Need to remove any new columns/rows added on the edge and need to recast type to bool
+        na_mask = na_mask.loc[self.pos_data[inkey].index, self.pos_data[inkey].columns].astype(bool)
+                
+        self.pos_data['Near_missing_grid'] = pd.DataFrame(na_mask, index=self.pos_data[inkey].index, columns=self.pos_data[inkey].columns, dtype=bool)
+
+        if nan_zero_count > 0:
+            if set_missing_nan:
+                #Check for grid colonies that didn't grow and report
+                print('Plate %s: %i grid colonies have size 0, probably due to pinning errors. These and neighbouring colonies will be set to nan.'%(self.plateid, nan_zero_count))
+            else:
+                #Check for grid colonies that didn't grow and throw a warning
+                print('Plate %s: %i grid colonies have size 0, probably due to pinning errors. I will ignore this for now and interpolate grid values based on surrounding grid colonies. However, it is recommended that you set these to nan. Affected colonies are marked in the Near_missing_grid column.'%(self.plateid, nan_zero_count))
+
+        if remove_grid_outliers:
+            #Calculate z-scores
+            sigma = grid.unstack().std()  # std dev of all ref colonies
+            mu = grid.unstack().mean()    # mean  of all ref colonies
+
+            z_scores = grid - mu
+            z_scores = z_scores / sigma
+            z_score_mask = z_scores.abs()>k
+
+            #Whatever the z-score, dont remove grid positions on edges of plate, this leads to missing data and these are more variable in general
+            z_score_mask.iloc[:,0] = False
+            z_score_mask.iloc[0,:] = False
+            z_score_mask.iloc[:,-1] = False
+            z_score_mask.iloc[-1,:] = False
+
+            grid[z_score_mask] = np.nan
+            print('Plate %s: Removed %i outlier grid colonies'%(self.plateid, z_score_mask.unstack().sum()))
+
+        if extrapolate_corners:
+            #warn('In this implementation of the grid normalisation it is only possible to extrapolate the lower left and upper right corners of 1536 plates. The grid must be placed as two 96 grids, in the upper left and lower right corner. Please do not use this option if those conditions are not met.')
+            grid.loc['32','1'] = intercept_coeff + horizontal_neighbour_coeff*grid.loc['32','4'] + vertical_neighbour_coeff*grid.loc['29','1']
+            grid.loc['1','48'] = intercept_coeff + horizontal_neighbour_coeff*grid.loc['1','45'] + vertical_neighbour_coeff*grid.loc['4','48']
+
+
+        self.pos_data['Grid'] = grid
+
+
+        #Calculate reference surface
+        #Get new list of grid positions after extrapolation and noise filtering
+        grid_us = grid.unstack().dropna().reset_index()
+        grid_us.columns = ['col', 'row', 'val']
+        gridpos_list_new = grid_us[['row', 'col']].values
+        values = grid_us['val'].values
+
+        #Points to interpolate
+        xi = grid.unstack()
+        xi = xi[pd.isnull(xi)]
+        xi = xi.reset_index()
+        xi.columns = ['col', 'row', 'val']
+        xi = xi[['row', 'col']].values
+
+        #interpolate
+        interpolated = interpolate.griddata(gridpos_list_new, values, xi, method='cubic')
+
+        ref_surface = pd.DataFrame(index=self.pos_data[inkey].index, columns=self.pos_data[inkey].columns, dtype=float)
+        for i,p in enumerate(gridpos_list_new):
+            ref_surface.loc[str(p[0]), str(p[1])] = grid.loc[str(p[0]), str(p[1])]
+        for i,p in enumerate(xi):
+            ref_surface.loc[str(p[0]), str(p[1])] = interpolated[i]
+        self.pos_data['Reference_surface'] = ref_surface
+
+        #Get ratio of max slope to wild type
+        corr_data = self.pos_data[inkey]/ref_surface
+        if set_missing_nan:
+            corr_data[na_mask] = np.nan
+        self.pos_data[outkey] = corr_data
+        
+    def plot_pos_data(self, pdf_path=None, toPlot=None):
+        '''Plot DataFrames containing numerical values as heatmaps using seaborn and matplotlib.
+        Keyword arguments:
+        pdf_path -- This option is highly recommended when you are dealing with large batches of Plates. It saves figures to pdf and then closes them so that they do not build up in memory. Please provide the name of a folder to save pdfs in, the filename is identical to the plateid.
+        toPlot (list) -- List of data to plot. Must be keys of Plate.pos_data. If not set, all DataFrames in pos_data which contain numeric values will be plotted.
+
+        Returns:
+        None
+        '''
+        
+        if not toPlot:
+            toPlot = []
+            for i, fr in self.pos_data.iteritems():
+                try:
+                    fr.astype(float)#Select only DataFrames which can be cast to numeric.
+                    toPlot.append(i)
+                except Exception:
+                    pass
+
+        if pdf_path:
+            pdf = PdfPages(os.path.join(pdf_path, str(self.plateid))+'.pdf')
+
+        for key in toPlot:
+            fig, ax = plt.subplots()
+            sns.heatmap(data=self.pos_data[key], ax=ax)
+            ax.set_title(key)
+            if pdf:
+                pdf.savefig()
+                fig.clf()
+                plt.close(fig)
+                
+        if pdf_path:
+            pdf.close()
+            
+    def check_values(self, inkey='Colony_size_corr', outkey='Colony_size_corr_checked', negative_action=0, inf_action=10):
+        ''' This function checks for invalid values in plate pos data. Normalisation procedures can produce invalid values 
+        as side effect, such as negative or infinite fitness values. This function detects those and deals with them in 
+        a custamisable way.
+
+        Keyworkd arguments:
+        inkey (str) -- The data to use (must be a key in exp.plates.pos_data)
+        negative_action (float) -- Value to assign to negative fitness. Defaults to 0. np.nan is allowed too. Set to None if no action required.
+        inf_action (float) -- Value to assign to inf values. Defaults to 10. np.nan is allowed too. Set to None if no action required.
+
+        Returns:
+        None (exp.plates.pos_data is modified in place)
+        '''
+
+        data = self.pos_data[inkey]
+        ##In some rare cases the input DataFrame can be empty. In that case, just set to an empty DataFrame
+        if data.empty:
+            self.pos_data[outkey] = pd.DataFrame([[]])
+            return None
+        data = data.unstack()
+
+        #Ignore na
+        data = data.dropna()
+
+        #Check for inf
+        isneginf = data[np.isneginf(data.values)]
+        if len(isneginf.index) != 0:
+            print('Plate %s - The following positions are minus infinity: %s'%(self.plateid, str(dict(isneginf))))
+        isposinf = data[np.isposinf(data.values)]
+        if len(isposinf.index) != 0:
+            print('Plate %s - The following positions are plus infinity: %s'%(self.plateid, str(dict(isposinf))))
+
+        #Check for negative
+        neg = data[~np.isinf(data.values)]
+        neg = neg[neg<0]
+        if len(neg.index) != 0:
+            print('Plate %s - The following positions are negative: %s'%(self.plateid, str(dict(neg))))
+
+        #Actions
+        if inf_action is not None:
+            inf_action = float(inf_action)            
+            if pd.isnull(inf_action):
+                self.pos_data[inkey][np.isinf(self.pos_data[inkey])] = inf_action
+            else:
+                self.pos_data[inkey][np.isneginf(self.pos_data[inkey])] = -inf_action
+                self.pos_data[inkey][np.isposinf(self.pos_data[inkey])] = inf_action
+
+        if negative_action is not None:
+            negative_action = float(negative_action)
+            self.pos_data[outkey] = self.pos_data[inkey].copy()
+            self.pos_data[outkey][self.pos_data[outkey].replace(-np.inf, 1).replace(np.inf, 1).replace(np.nan, 1)<0] = negative_action
+
+
+
+    def make_long_data(self):
+        '''Generate a summary table of all Data stored in this Plate object.
+        Returns:
+        long_data (pandas DataFrame)
+        '''
+        unstacked = []
+        for k, frame in self.pos_data.iteritems():
+            if frame.empty:
+                continue
+            l_unstacked = frame.copy()
+            l_unstacked.columns.name = 'Column'
+            l_unstacked.index.name = 'Row'
+            l_unstacked = l_unstacked.unstack()
+            l_unstacked.name = k
+            unstacked.append(l_unstacked)
+        if len(unstacked) == 0:
+            warn('No data associated with Plate %s. Please check input data'%self.plateid)
+            return pd.DataFrame([[]])
+        else:
+            long_data = pd.concat(unstacked, axis=1)
+            long_data = long_data.reset_index()
+
+        return long_data
+
+def check_mkdir(dirPath):
+    '''
+Create a directory if it does not exist already.
+
+Required arguments:
+dirPath (str) - path of the directory to create.
+'''
+
+    if os.path.exists(dirPath):
+        warn('Directory exist, not doing anything.')
+    else:
+        os.mkdir(dirPath)
+
+
+
+def check_exp_data(exp_data, layouts=False):
+    print('Checking exp_data table')
+    
+    print('Checking if plate IDs (first column) are unique')
+    assert not exp_data.index.duplicated().any(), 'Error, Plate IDs are not unique'
+    print('....OK')
+    
+    print('Checking for mandatory columns')
+    assert 'Data_path' in exp_data.columns, 'Error, table must have Data_path column'
+    if layouts:
+        assert 'Layout_path' in exp_data.columns, 'Error, table must have Layout_path column'
+    print('....OK')
+    
+    print('Checking if data files are unique')
+    assert not exp_data['Data_path'].duplicated().any(), 'Error, data paths are not unique (plates with the same ID have been assigned the same data file).'
+    print('....OK')
+    
+    print('Checking all data files exist')
+    for ip in exp_data['Data_path']:
+        if not os.path.isfile(ip):
+            raise IOError('Data file does not exist: %s'%ip)
+    print('...OK')
+    
+    if layouts:
+        print('Checking all layout files exist')
+        for ip in exp_data['Layout_path']:
+            if not os.path.isfile(ip):
+                raise IOError('Layout file does not exist: %s'%ip)
+        print('...OK')
+
+def pyphe_cmd(wdirectory=None, grid_norm=None, out_ld=None, qcplots=None, check_setNA=None, qcplot_dir=None, exp_data_path=None, extrapolate_corners=None, grid_pos=None, rcmedian=None, input_type=None, load_layouts=None):
+    '''
+    This function was written to be called from the GUI script provided. But it can also be used to run the entire standard pipeline in one place.
+    '''
+    
+    print('###Step 1: Load data###')
+
+    #Set working directory
+    if wdirectory:
+        os.chdir(wdirectory)
+        print('Working directory changed to: %s'%wdirectory)
+    #Import exp_data
+    exp_data = pd.read_csv(exp_data_path, index_col=0)
+    check_exp_data(exp_data, layouts=load_layouts)
+    print('Table checks completed')
+    
+    exp = Experiment(exp_data)
+    print('Created pyphe experiment object')
+    
+    #Load the data
+    if input_type == 'gitter':
+        exp.plates.map(Plate.read_gitter_single_image)
+
+    elif input_type == 'pyphe-quantify-redness':
+        exp.plates.map(Plate.read_pypheredness_single_image)
+        
+    elif input_type == 'pyphe-growthcurves':
+        exp.plates.map(Plate.read_pgc_single_image)
+        
+    elif input_type == 'pyphe-quantify-batch':
+                exp.plates.map(Plate.read_pyphebatch_single_image)
+    
+    else:
+        raise ValueError('Unrecignised input_type')
+    print('Plate data loaded sucessfully')
+    
+    
+    #Load the layouts
+    if load_layouts:
+        exp.plates.map(Plate.read_layout_single_plate)
+        print('Layouts loaded sucessfully')
+    
+    #Perform norms
+    if grid_norm:
+        if input_type == 'pyphe-quantify-redness':
+            raise ValueError('Grid normalisation does not make sense for redness input')
+            
+        print('Performing grid norm')
+
+        if (grid_pos == 'Standard 384 (top left)') or (grid_pos == 'standard384'):
+            gridpos_list = [(row, col) for row in range(1, 16, 2) for col in range(1, 24, 2)]
+        elif (grid_pos == 'Standard 1536 (top left and bottom right)') or (grid_pos == 'standard1536'):
+            gridpos_list = [(row, col) for row in range(1, 32, 4) for col in range(1, 48, 4)]
+            gridpos_list += [(row, col) for row in range(4, 33, 4) for col in range(4, 49, 4)]
+        elif grid_pos == '1536with384grid':
+            gridpos_list = [(row, col) for row in range(1, 32, 2) for col in range(1, 48, 2)]
+        else:
+            raise ValueError('grid_pos must be one of ["Standard 384 (top left)", "standard384", "Standard 1536 (top left and bottom right)", "standard1536", "1536with384grid"]')
+
+
+        if extrapolate_corners:
+            from sklearn.linear_model import LinearRegression
+            #Make a table of  features
+            vals = pd.DataFrame(columns=['thisCorner', 'horizontalNeighbour', 'verticalNeighbour'])
+            for i,p in exp.plates.iteritems():
+                vals.loc[i+'_topLeft'] = [p.pos_data['Colony_size'].loc['1','1'], p.pos_data['Colony_size'].loc['1','5'], p.pos_data['Colony_size'].loc['5','1']]
+                vals.loc[i+'_bottomRight'] = [p.pos_data['Colony_size'].loc['32','48'], p.pos_data['Colony_size'].loc['32','44'], p.pos_data['Colony_size'].loc['28','48']]
+            mlm = LinearRegression()
+            mlm.fit(vals.iloc[:,1:], vals.iloc[:,0])
+            print('Extrapolating missing corners based on the following regression: ')
+            print('    horizontal_neighbour_coeff: ' +  str(mlm.coef_[0]))
+            print('    vertical_neighbour_coeff: ' +  str(mlm.coef_[1]))
+            print('    intercept_coeff: ' +  str(mlm.intercept_))
+            print('    accuracy: ' +str(mlm.score(vals.iloc[:,1:], vals.iloc[:,0])))
+                        
+            exp.plates.map(lambda x: x.grid_normalisation(gridpos_list, 
+                                                  extrapolate_corners=True, horizontal_neighbour_coeff=mlm.coef_[0], 
+                                                  vertical_neighbour_coeff=mlm.coef_[1],  intercept_coeff=mlm.intercept_))
+                              
+        else:
+            exp.plates.map(lambda x: x.grid_normalisation(gridpos_list) )
+            
+        
+    if rcmedian:
+        print('Performing row/column median normalisation')
+        if grid_norm:
+            ikey = 'Colony_size_corr'
+            okey = 'Colony_size_corr'
+        else:
+            ikey = 'Colony_size'
+            okey = 'Colony_size_corr'
+
+        exp.plates.map(lambda x: x.rcmedian_normalisation(inkey=ikey, outkey=okey))
+    
+    #Perform checks and qc
+    if check_setNA:
+        print('Checking for infinite and negative fitness values')
+        if (not grid_norm) and (not rcmedian):
+            exp.plates.map(lambda x: x.check_values(inkey='Colony_size', outkey='Colony_size_checked', negative_action=np.nan, inf_action=np.nan))
+        else:
+            exp.plates.map(lambda x: x.check_values(inkey='Colony_size_corr', outkey='Colony_size_corr_checked', negative_action=np.nan, inf_action=np.nan))
+        
+    if qcplots:
+        print('Making qc plots')
+        exp.plates.map(lambda x: x.plot_pos_data(pdf_path=qcplot_dir))
+        
+    #Export
+    print('Exporting data')
+    ld = exp.generate_long_data()
+    ld.to_csv(out_ld)
+    print('Done')
+    
+
```

### Comparing `pyphe-0.981/pyphe/growthcurves.py` & `pyphe-0.982/pyphe/growthcurves.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-import pandas as pd
-import numpy as np
-from scipy import stats
-
-def analyse_growthcurve(gdata, fitrange, t0_fitrange, lag_method, lag_threshold, plots, plot_ylim, outdir, in_baseStr, plot_individual_data):
-    '''
-    Function for analysing a csv containing growthcurves.
-    
-    Arguments:
-    gdata (pandas.DataFrame) -- DataFrame containing growth data. The index must be the timepoints and column IDs must be unique.
-    fitrange (int) -- The number of timepoints over which to fit the linear regression.
-    t0_fitrange (int) -- The number of timepoints to use to estimate the initial biomass which is the mean over those timepoints.
-    lag_method (str) -- Method to use to determine lag phase. Currently supported: rel_threshold and abs_threshold.
-    lag_threshold (float) -- The threshold value to use. The lag phase will be determined as the time it takes for the biomass to exceed this value (for abs_threshold) or t0*threshold for rel_threshold.
-    plots (bool) --  Produce pdf document of growth curve plots.
-    plot_ylim (float) -- Set plot upper limits of y-axis.
-    '''
-    
-    t = gdata.index.tolist()
-    
-    def find_lag(x):
-        '''Find the lag phase for a single growthcurve.
-        Required arguments:
-        x (array-like) -- 1D array-like containing the population/colony sizes
-        t (array-like) -- 1D array-like containing the timepoints, must have same dimensions as x
-        t0 (float) -- Inoculation biomass
-        method (str) -- method to use to determine lag phase. Currently supported: rel_threshold and abs_threshold.
-        thresh (float) -- The threshold value to use. The lag phase will be determined as the time it takes for the biomass to exceed this value (for abs_threshold) or t0*threshold for rel_threshold.
-        Returns:
-        lag (float) -- lag time
-        '''
-        t0 = np.array(x)[0:t0_fitrange].mean()
-
-        if lag_method=='rel':
-            for i, val in enumerate(x):
-                if val > lag_threshold*t0:
-                    return pd.Series([t0, t[i]], index=['initial biomass', 'lag'])
-
-        elif lag_method=='abs':
-            for i, val in enumerate(x):
-                if val > lag_threshold:
-                    return pd.Series([t0, t[i]], index=['initial biomass', 'lag'])              
-
-        else:
-            raise ValueError('Unknown lag method %s' %method)
-
-    #Analyse lags
-    lags = gdata.apply(find_lag)
-    
-    def find_max_slope(x, find_min_instead=False):
-        '''Find max_slope, t_max, intercept and r2 for a single growthcurve. The regression is aware of the timepoints so this will work with unevenly samples growthcurves.
-        Required arguments:
-        x (array-like) -- 1D array-like containing the population/colony sizes
-        t (array-like) -- 1D array-like containing the timepoints, must have same dimensions as x
-        reg_fitrange (int) -- The number of timepoints over which to fit the linear regression
-        Returns:
-        {
-        max_slope -- The slope of the regression
-        t_max -- The mid-point of the fitrange of the regression
-        intercept -- The y-inyercept of the regression
-        r2 -- The R^2 value of the regression
-        }
-        '''
-        regression_results = []
-        x = x.tolist()
-        
-        for i in range(len(x)-fitrange):
-            slope, intercept, r_value, p_value, std_err = stats.linregress(t[i:i+fitrange], x[i:i+fitrange])
-            regression_results.append({'t_max':np.mean(t[i:i+fitrange]), 'max_slope':slope, 'r2':r_value**2, 'y-intercept':intercept})
-            
-        if find_min_instead:
-            slope_result = pd.Series(min(regression_results, key=lambda x: x['max_slope']))
-        else:
-            slope_result = pd.Series(max(regression_results, key=lambda x: x['max_slope']))
-            
-        slope_result['x-intercept'] = -slope_result['y-intercept']/slope_result['max_slope']
-        return slope_result
-        
-    #Get max slopes    
-    slopes = gdata.apply(find_max_slope)
-    
-    
-    #Get area under the curve (AUC)
-    aucs = gdata.sum()
-    aucs.name = 'sum of values (AUC)'
-    aucs = pd.DataFrame(aucs).transpose()
-
-    #Get maximum value
-    maxgrowth = gdata.max()
-    maxgrowth.name = 'maximum'
-    maxgrowth = pd.DataFrame(maxgrowth).transpose()
-
-    
-    ###Perform some simple QC
-    #flag cases where min slope is < - 7.5% of max slope in entire input data
-    min_slopes = gdata.apply(find_max_slope, find_min_instead=True)
-    min_slopes = min_slopes.loc['max_slope']   
-    neg_slope_warning = min_slopes < -(slopes.loc['max_slope'].max() * 0.075)
-    neg_slope_warning.name = 'warning_negative_slope'
-    if neg_slope_warning.sum() > 0:
-        print('The following growth curves appear to have significant negative slopes. This is also flagged in the output file:  %s)'%','.join(neg_slope_warning[neg_slope_warning].index))
-    neg_slope_warning = pd.DataFrame(neg_slope_warning).transpose()
-    neg_slope_warning.loc['warning_negative_slope'] = neg_slope_warning.loc['warning_negative_slope'].map({True:'WARNING', False:''})
-
-    #flag cases where the tangent fit is poor (R^2<0.95)
-    r2_warning = slopes.loc['r2'] < 0.95
-    r2_warning.name = 'warning_bad_fit'
-    if r2_warning.sum() > 0:
-        print('For the following growth curves the R^2 of the fitted tangent is < 0.95. This is also flagged in the output file:  %s)'%','.join(r2_warning[r2_warning].index))
-    r2_warning = pd.DataFrame(r2_warning).transpose()
-    r2_warning.loc['warning_bad_fit'] = r2_warning.loc['warning_bad_fit'].map({True:'WARNING', False:''})
-
-    ###Plotting
-    if plots:
-        from matplotlib import pyplot as plt
-        import seaborn as sns
-        sns.set(style='ticks', font_scale=0.75)
-        plt.rcParams['svg.fonttype'] = 'none'
-        from matplotlib.backends.backend_pdf import PdfPages
-        
-        with PdfPages(outdir + '/' + in_baseStr + '_curves.pdf') as pdf:
-            layout=(8,4)
-            raw_kwargs={'color':'C0', 'linewidth':1}
-            smoothed_kwargs={'color':'r', 'linewidth':0.5}
-            regr_kwargs={'color':'k', 'linewidth':0.5, 'linestyle':'--'}
-            
-            toPlot = list(gdata)
-            while toPlot:
-                fig, ax = plt.subplots(layout[0], layout[1], figsize=(8.27,11.69))
-                for a in ax.flat:
-                    
-                    a.plot(t, gdata[toPlot[0]], **raw_kwargs, zorder=1)
-                    if plot_individual_data:
-                        a.scatter(t, gdata[toPlot[0]], color='k', marker='.', s=1, zorder=2)
-                    #Get ylim
-                    ylim = a.get_ylim()
-
-                    tmax = slopes.loc['t_max', toPlot[0]]
-                    maxslope = slopes.loc['max_slope', toPlot[0]] 
-                    intercept = slopes.loc['y-intercept', toPlot[0]]
-                    if not pd.isnull([tmax, maxslope, intercept]).any():
-                        x = np.array(t)
-                        y = x*maxslope + intercept
-                        a.plot(x, y, **regr_kwargs)
-
-                    t0 = lags.loc['initial biomass', toPlot[0]]
-                    lag = lags.loc['lag', toPlot[0]]
-                    if not pd.isnull([t0, lag]).any():
-                        a.axhline(t0, color='k', xmin=0, xmax=lag, linewidth=0.75, alpha=0.6)
-                        a.axvline(lag, color='k', linewidth=0.75, alpha=0.6)
-                        if 'lag_method' == 'abs':
-                            a.axhline(lag_threshold, color='k', xmin=0, xmax=lag, linewidth=0.75, alpha=0.6)
-                        else:
-                            a.axhline(lag_threshold * t0, color='k', xmin=0, xmax=lag, linewidth=0.75, alpha=0.6)
-                        
-                    a.set_title(str(toPlot[0]))
-                    if plot_ylim:
-                        a.set_ylim([0,plot_ylim])
-                    else: 
-                        a.set_ylim(ylim)
-                    toPlot.pop(0)
-                    if not toPlot:
-                        break
-                        
-                plt.tight_layout()                    
-                pdf.savefig()
-                plt.close()
-                plt.clf()
-
-    return pd.concat([lags, slopes, aucs, maxgrowth, neg_slope_warning, r2_warning], axis=0)
+import pandas as pd
+import numpy as np
+from scipy import stats
+
+def analyse_growthcurve(gdata, fitrange, t0_fitrange, lag_method, lag_threshold, plots, plot_ylim, outdir, in_baseStr, plot_individual_data):
+    '''
+    Function for analysing a csv containing growthcurves.
+    
+    Arguments:
+    gdata (pandas.DataFrame) -- DataFrame containing growth data. The index must be the timepoints and column IDs must be unique.
+    fitrange (int) -- The number of timepoints over which to fit the linear regression.
+    t0_fitrange (int) -- The number of timepoints to use to estimate the initial biomass which is the mean over those timepoints.
+    lag_method (str) -- Method to use to determine lag phase. Currently supported: rel_threshold and abs_threshold.
+    lag_threshold (float) -- The threshold value to use. The lag phase will be determined as the time it takes for the biomass to exceed this value (for abs_threshold) or t0*threshold for rel_threshold.
+    plots (bool) --  Produce pdf document of growth curve plots.
+    plot_ylim (float) -- Set plot upper limits of y-axis.
+    '''
+    
+    t = gdata.index.tolist()
+    
+    def find_lag(x):
+        '''Find the lag phase for a single growthcurve.
+        Required arguments:
+        x (array-like) -- 1D array-like containing the population/colony sizes
+        t (array-like) -- 1D array-like containing the timepoints, must have same dimensions as x
+        t0 (float) -- Inoculation biomass
+        method (str) -- method to use to determine lag phase. Currently supported: rel_threshold and abs_threshold.
+        thresh (float) -- The threshold value to use. The lag phase will be determined as the time it takes for the biomass to exceed this value (for abs_threshold) or t0*threshold for rel_threshold.
+        Returns:
+        lag (float) -- lag time
+        '''
+        t0 = np.array(x)[0:t0_fitrange].mean()
+
+        if lag_method=='rel':
+            for i, val in enumerate(x):
+                if val > lag_threshold*t0:
+                    return pd.Series([t0, t[i]], index=['initial biomass', 'lag'])
+
+        elif lag_method=='abs':
+            for i, val in enumerate(x):
+                if val > lag_threshold:
+                    return pd.Series([t0, t[i]], index=['initial biomass', 'lag'])              
+
+        else:
+            raise ValueError('Unknown lag method %s' %method)
+
+    #Analyse lags
+    lags = gdata.apply(find_lag)
+    
+    def find_max_slope(x, find_min_instead=False):
+        '''Find max_slope, t_max, intercept and r2 for a single growthcurve. The regression is aware of the timepoints so this will work with unevenly samples growthcurves.
+        Required arguments:
+        x (array-like) -- 1D array-like containing the population/colony sizes
+        t (array-like) -- 1D array-like containing the timepoints, must have same dimensions as x
+        reg_fitrange (int) -- The number of timepoints over which to fit the linear regression
+        Returns:
+        {
+        max_slope -- The slope of the regression
+        t_max -- The mid-point of the fitrange of the regression
+        intercept -- The y-inyercept of the regression
+        r2 -- The R^2 value of the regression
+        }
+        '''
+        regression_results = []
+        x = x.tolist()
+        
+        for i in range(len(x)-fitrange):
+            slope, intercept, r_value, p_value, std_err = stats.linregress(t[i:i+fitrange], x[i:i+fitrange])
+            regression_results.append({'t_max':np.mean(t[i:i+fitrange]), 'max_slope':slope, 'r2':r_value**2, 'y-intercept':intercept})
+            
+        if find_min_instead:
+            slope_result = pd.Series(min(regression_results, key=lambda x: x['max_slope']))
+        else:
+            slope_result = pd.Series(max(regression_results, key=lambda x: x['max_slope']))
+            
+        slope_result['x-intercept'] = -slope_result['y-intercept']/slope_result['max_slope']
+        return slope_result
+        
+    #Get max slopes    
+    slopes = gdata.apply(find_max_slope)
+    
+    
+    #Get area under the curve (AUC)
+    aucs = gdata.sum()
+    aucs.name = 'sum of values (AUC)'
+    aucs = pd.DataFrame(aucs).transpose()
+
+    #Get maximum value
+    maxgrowth = gdata.max()
+    maxgrowth.name = 'maximum'
+    maxgrowth = pd.DataFrame(maxgrowth).transpose()
+
+    
+    ###Perform some simple QC
+    #flag cases where min slope is < - 7.5% of max slope in entire input data
+    min_slopes = gdata.apply(find_max_slope, find_min_instead=True)
+    min_slopes = min_slopes.loc['max_slope']   
+    neg_slope_warning = min_slopes < -(slopes.loc['max_slope'].max() * 0.075)
+    neg_slope_warning.name = 'warning_negative_slope'
+    if neg_slope_warning.sum() > 0:
+        print('The following growth curves appear to have significant negative slopes. This is also flagged in the output file:  %s)'%','.join(neg_slope_warning[neg_slope_warning].index))
+    neg_slope_warning = pd.DataFrame(neg_slope_warning).transpose()
+    neg_slope_warning.loc['warning_negative_slope'] = neg_slope_warning.loc['warning_negative_slope'].map({True:'WARNING', False:''})
+
+    #flag cases where the tangent fit is poor (R^2<0.95)
+    r2_warning = slopes.loc['r2'] < 0.95
+    r2_warning.name = 'warning_bad_fit'
+    if r2_warning.sum() > 0:
+        print('For the following growth curves the R^2 of the fitted tangent is < 0.95. This is also flagged in the output file:  %s)'%','.join(r2_warning[r2_warning].index))
+    r2_warning = pd.DataFrame(r2_warning).transpose()
+    r2_warning.loc['warning_bad_fit'] = r2_warning.loc['warning_bad_fit'].map({True:'WARNING', False:''})
+
+    ###Plotting
+    if plots:
+        from matplotlib import pyplot as plt
+        import seaborn as sns
+        sns.set(style='ticks', font_scale=0.75)
+        plt.rcParams['svg.fonttype'] = 'none'
+        from matplotlib.backends.backend_pdf import PdfPages
+        
+        with PdfPages(outdir + '/' + in_baseStr + '_curves.pdf') as pdf:
+            layout=(8,4)
+            raw_kwargs={'color':'C0', 'linewidth':1}
+            smoothed_kwargs={'color':'r', 'linewidth':0.5}
+            regr_kwargs={'color':'k', 'linewidth':0.5, 'linestyle':'--'}
+            
+            toPlot = list(gdata)
+            while toPlot:
+                fig, ax = plt.subplots(layout[0], layout[1], figsize=(8.27,11.69))
+                for a in ax.flat:
+                    
+                    a.plot(t, gdata[toPlot[0]], **raw_kwargs, zorder=1)
+                    if plot_individual_data:
+                        a.scatter(t, gdata[toPlot[0]], color='k', marker='.', s=1, zorder=2)
+                    #Get ylim
+                    ylim = a.get_ylim()
+
+                    tmax = slopes.loc['t_max', toPlot[0]]
+                    maxslope = slopes.loc['max_slope', toPlot[0]] 
+                    intercept = slopes.loc['y-intercept', toPlot[0]]
+                    if not pd.isnull([tmax, maxslope, intercept]).any():
+                        x = np.array(t)
+                        y = x*maxslope + intercept
+                        a.plot(x, y, **regr_kwargs)
+
+                    t0 = lags.loc['initial biomass', toPlot[0]]
+                    lag = lags.loc['lag', toPlot[0]]
+                    if not pd.isnull([t0, lag]).any():
+                        a.axhline(t0, color='k', xmin=0, xmax=lag, linewidth=0.75, alpha=0.6)
+                        a.axvline(lag, color='k', linewidth=0.75, alpha=0.6)
+                        if 'lag_method' == 'abs':
+                            a.axhline(lag_threshold, color='k', xmin=0, xmax=lag, linewidth=0.75, alpha=0.6)
+                        else:
+                            a.axhline(lag_threshold * t0, color='k', xmin=0, xmax=lag, linewidth=0.75, alpha=0.6)
+                        
+                    a.set_title(str(toPlot[0]))
+                    if plot_ylim:
+                        a.set_ylim([0,plot_ylim])
+                    else: 
+                        a.set_ylim(ylim)
+                    toPlot.pop(0)
+                    if not toPlot:
+                        break
+                        
+                plt.tight_layout()                    
+                pdf.savefig()
+                plt.close()
+                plt.clf()
+
+    return pd.concat([lags, slopes, aucs, maxgrowth, neg_slope_warning, r2_warning], axis=0)
```

### Comparing `pyphe-0.981/pyphe/interpret.py` & `pyphe-0.982/pyphe/interpret.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-import pandas as pd
-from scipy.stats import ttest_ind
-import numpy as np
-from statsmodels.stats.multitest import multipletests as multit
-from warnings import warn
-
-def count_reps(inseries):
-    inseries = inseries.tolist()
-    counts = {k:0 for k in list(set(inseries))}
-    out = [878 for i in range(len(inseries))]
-    for ind, ite in enumerate(inseries):
-        out[ind] = counts[ite]
-        counts[ite] += 1
-    return out
-    
-
-from scipy.stats import mstats_basic
-
-def interpret(ld, condition_column, strain_column, values_column, control_condition, out_prefix, circularity=None, set_missing_na=False):
-    '''
-    Interpret experimental data report produced by pyphe-analyse. 
-    '''
-    
-    ###Check if essential columns exist
-    print('Checking input table')
-    print('Checking if axis_column exists')
-    if condition_column not in list(ld):
-        raise NameError('Axis_column not found in table.')
-    print('....OK')
-
-    print('Checking if grouping_column exists')
-    if strain_column not in list(ld):
-        raise NameError('grouping_column not found in table.')
-    print('....OK')
-
-    print('Checking if values_column exists')
-    if values_column not in list(ld):
-        raise NameError('values_column not found in table.')
-    print('....OK')
-
-    print('Checking if control exists in axis_column')
-    if control_condition not in ld[condition_column].unique():
-        raise NameError('control not found in axis_column.')
-    print('....OK')
-
-    if circularity:
-        print('Circularity filter is set. Checking if Colony_circularity column exists')
-        if 'Colony_circularity' not in list(ld):
-            raise NameError('Input data has no column named Colony_circularity. Cannot apply circularity filter.')
-
-
-    ###Report some simple numbers
-    print('Data report loaded successfully')
-
-    initial_conditions = ld[condition_column].unique()
-    print('Number of unique elements in axis column: %i'%len(initial_conditions))
-
-    initial_strains = ld[strain_column].unique()
-    print('Number of unique elements in grouping column: %i'%len(initial_strains))
-
-    print('Number of plates: %i'%len(ld['Plate'].unique()))
-
-    print('Number of non-NA data points: %i'%len(ld.loc[~pd.isnull(ld[values_column])].index))
-
-    ###Simple QC filters
-    n_datapoints = (~ld[values_column].isnull()).sum()
-    if circularity:
-        ld.loc[ld['Colony_circularity']<circularity, values_column] = np.nan
-        nn_datapoints = (~ld[values_column].isnull()).sum()
-        print('Removed %i entries with circularity < %f'%(n_datapoints-nn_datapoints, circularity))
-        n_datapoints = nn_datapoints
-    if set_missing_na:
-        ld.loc[ld[values_column]==0, values_column] = np.nan
-        nn_datapoints = (~ld[values_column].isnull()).sum()
-        print('Removed %i entries with fitness 0'%(n_datapoints-nn_datapoints))
-        n_datapoints = nn_datapoints
-
-    ###Group by replicates
-    ld_stats = ld.copy()
-    #drop any NA
-    ld_stats = ld_stats.loc[~ld_stats[values_column].isnull()]
-    #Recompute number of axis and grouping elements
-    conditions = ld_stats[condition_column].unique()
-    print('Number of unique elements in axis column after filtering: %i'%len(conditions))
-    strains = ld_stats[strain_column].unique()
-    print('Number of unique elements in grouping column: %i'%len(strains))
-
-    ld_stats['condition---strain'] = ld_stats[condition_column] + '---' + ld_stats[strain_column]
-    ld_stats['rep'] = count_reps(ld_stats['condition---strain'])
-
-    #Pivot this into wide format
-    ld_stats_piv = ld_stats.pivot_table(index=strain_column, columns=[condition_column,'rep'], values=values_column)
-
-    #assert that there are no duplicates, i.e. that count_reps() worked as expected
-    assert (ld_stats.pivot_table(index=strain_column, columns=[condition_column,'rep'], values=values_column, aggfunc=len).unstack().dropna()==1.0).all()
-
-    #Save this table:
-    ld_stats_piv.to_csv(out_prefix+'_reps.csv')
-    ###Compute summary stats
-    mean_fitness = ld_stats_piv.mean(axis=1, level=0)
-    median_fitness = ld_stats_piv.median(axis=1, level=0)
-    fitness_stdev = ld_stats_piv.std(axis=1, level=0)
-    obs_count = ld_stats_piv.count(axis=1, level=0)
-
-    #Compute effect sizes
-    median_effect_size = median_fitness.div(median_fitness[control_condition], axis=0)
-    mean_effect_size = mean_fitness.div(mean_fitness[control_condition], axis=0)
-
-    ###run Welch's t-test
-    print('Running t-tests')
-    p_Welch = {}
-    b = ld_stats_piv.xs(control_condition,axis=1, level=0).values
-    b = np.ma.masked_invalid(b)
-
-    for co in conditions:
-        a = ld_stats_piv.xs(co, axis=1, level=0).values
-        a = np.ma.masked_invalid(a)
-        pvals_temp = mstats_basic.ttest_ind(a, b, axis=1, equal_var=False)[1].filled(np.nan)
-        p_Welch[co] = pd.Series(pvals_temp, index=ld_stats_piv.index)
-    p_Welch = pd.concat(p_Welch, axis=1)
-    #multiple testing correction by BH
-    p_Welch_BH = p_Welch.copy()
-    for c in p_Welch_BH:
-        if p_Welch_BH[c].isnull().all():
-            warn('No p-values obtained for %s (probably not enaough replicates)'%c)
-        else:
-            p_Welch_BH.loc[~p_Welch_BH[c].isnull(), c] = multit(p_Welch_BH.loc[~p_Welch_BH[c].isnull(), c], method='fdr_bh')[1]
-
-
-    #aggregate data in table and save
-    #And join together in one big data frame
-    combined_data = pd.concat({'mean_fitness' : mean_fitness,
-                               'mean_fitness_log2' : mean_fitness.applymap(np.log2),
-                'median_fitness' : median_fitness,
-                  'median_fitness_log2' : median_fitness.applymap(np.log2),
-                'mean_effect_size' : mean_effect_size,
-                'mean_effect_size_log2' : mean_effect_size.applymap(np.log2),
-                'median_effect_size' : median_effect_size,
-                'median_effect_size_log2' : median_effect_size.applymap(np.log2),
-                'observation_count' : obs_count,
-               'stdev_fitness' : fitness_stdev,
-               'p_Welch' : p_Welch,
-                'p_Welch_BH' : p_Welch_BH,
-                'p_Welch_BH_-log10' : -p_Welch_BH.applymap(np.log10)}, axis=1)
-
-
-    combined_data = combined_data.swaplevel(axis=1).sort_index(axis=1)
-    combined_data.to_csv(out_prefix+'_summaryStats.csv')
-    print('Interpretation completed and results saved.')
-    return combined_data
-        
+import pandas as pd
+from scipy.stats import ttest_ind
+import numpy as np
+from statsmodels.stats.multitest import multipletests as multit
+from warnings import warn
+
+def count_reps(inseries):
+    inseries = inseries.tolist()
+    counts = {k:0 for k in list(set(inseries))}
+    out = [878 for i in range(len(inseries))]
+    for ind, ite in enumerate(inseries):
+        out[ind] = counts[ite]
+        counts[ite] += 1
+    return out
+    
+
+from scipy.stats import mstats_basic
+
+def interpret(ld, condition_column, strain_column, values_column, control_condition, out_prefix, circularity=None, set_missing_na=False):
+    '''
+    Interpret experimental data report produced by pyphe-analyse. 
+    '''
+    
+    ###Check if essential columns exist
+    print('Checking input table')
+    print('Checking if axis_column exists')
+    if condition_column not in list(ld):
+        raise NameError('Axis_column not found in table.')
+    print('....OK')
+
+    print('Checking if grouping_column exists')
+    if strain_column not in list(ld):
+        raise NameError('grouping_column not found in table.')
+    print('....OK')
+
+    print('Checking if values_column exists')
+    if values_column not in list(ld):
+        raise NameError('values_column not found in table.')
+    print('....OK')
+
+    print('Checking if control exists in axis_column')
+    if control_condition not in ld[condition_column].unique():
+        raise NameError('control not found in axis_column.')
+    print('....OK')
+
+    if circularity:
+        print('Circularity filter is set. Checking if Colony_circularity column exists')
+        if 'Colony_circularity' not in list(ld):
+            raise NameError('Input data has no column named Colony_circularity. Cannot apply circularity filter.')
+
+
+    ###Report some simple numbers
+    print('Data report loaded successfully')
+
+    initial_conditions = ld[condition_column].unique()
+    print('Number of unique elements in axis column: %i'%len(initial_conditions))
+
+    initial_strains = ld[strain_column].unique()
+    print('Number of unique elements in grouping column: %i'%len(initial_strains))
+
+    print('Number of plates: %i'%len(ld['Plate'].unique()))
+
+    print('Number of non-NA data points: %i'%len(ld.loc[~pd.isnull(ld[values_column])].index))
+
+    ###Simple QC filters
+    n_datapoints = (~ld[values_column].isnull()).sum()
+    if circularity:
+        ld.loc[ld['Colony_circularity']<circularity, values_column] = np.nan
+        nn_datapoints = (~ld[values_column].isnull()).sum()
+        print('Removed %i entries with circularity < %f'%(n_datapoints-nn_datapoints, circularity))
+        n_datapoints = nn_datapoints
+    if set_missing_na:
+        ld.loc[ld[values_column]==0, values_column] = np.nan
+        nn_datapoints = (~ld[values_column].isnull()).sum()
+        print('Removed %i entries with fitness 0'%(n_datapoints-nn_datapoints))
+        n_datapoints = nn_datapoints
+
+    ###Group by replicates
+    ld_stats = ld.copy()
+    #drop any NA
+    ld_stats = ld_stats.loc[~ld_stats[values_column].isnull()]
+    #Recompute number of axis and grouping elements
+    conditions = ld_stats[condition_column].unique()
+    print('Number of unique elements in axis column after filtering: %i'%len(conditions))
+    strains = ld_stats[strain_column].unique()
+    print('Number of unique elements in grouping column: %i'%len(strains))
+
+    ld_stats['condition---strain'] = ld_stats[condition_column] + '---' + ld_stats[strain_column]
+    ld_stats['rep'] = count_reps(ld_stats['condition---strain'])
+
+    #Pivot this into wide format
+    ld_stats_piv = ld_stats.pivot_table(index=strain_column, columns=[condition_column,'rep'], values=values_column)
+
+    #assert that there are no duplicates, i.e. that count_reps() worked as expected
+    assert (ld_stats.pivot_table(index=strain_column, columns=[condition_column,'rep'], values=values_column, aggfunc=len).unstack().dropna()==1.0).all()
+
+    #Save this table:
+    ld_stats_piv.to_csv(out_prefix+'_reps.csv')
+    ###Compute summary stats
+    mean_fitness = ld_stats_piv.mean(axis=1, level=0)
+    median_fitness = ld_stats_piv.median(axis=1, level=0)
+    fitness_stdev = ld_stats_piv.std(axis=1, level=0)
+    obs_count = ld_stats_piv.count(axis=1, level=0)
+
+    #Compute effect sizes
+    median_effect_size = median_fitness.div(median_fitness[control_condition], axis=0)
+    mean_effect_size = mean_fitness.div(mean_fitness[control_condition], axis=0)
+
+    ###run Welch's t-test
+    print('Running t-tests')
+    p_Welch = {}
+    b = ld_stats_piv.xs(control_condition,axis=1, level=0).values
+    b = np.ma.masked_invalid(b)
+
+    for co in conditions:
+        a = ld_stats_piv.xs(co, axis=1, level=0).values
+        a = np.ma.masked_invalid(a)
+        pvals_temp = mstats_basic.ttest_ind(a, b, axis=1, equal_var=False)[1].filled(np.nan)
+        p_Welch[co] = pd.Series(pvals_temp, index=ld_stats_piv.index)
+    p_Welch = pd.concat(p_Welch, axis=1)
+    #multiple testing correction by BH
+    p_Welch_BH = p_Welch.copy()
+    for c in p_Welch_BH:
+        if p_Welch_BH[c].isnull().all():
+            warn('No p-values obtained for %s (probably not enaough replicates)'%c)
+        else:
+            p_Welch_BH.loc[~p_Welch_BH[c].isnull(), c] = multit(p_Welch_BH.loc[~p_Welch_BH[c].isnull(), c], method='fdr_bh')[1]
+
+
+    #aggregate data in table and save
+    #And join together in one big data frame
+    combined_data = pd.concat({'mean_fitness' : mean_fitness,
+                               'mean_fitness_log2' : mean_fitness.applymap(np.log2),
+                'median_fitness' : median_fitness,
+                  'median_fitness_log2' : median_fitness.applymap(np.log2),
+                'mean_effect_size' : mean_effect_size,
+                'mean_effect_size_log2' : mean_effect_size.applymap(np.log2),
+                'median_effect_size' : median_effect_size,
+                'median_effect_size_log2' : median_effect_size.applymap(np.log2),
+                'observation_count' : obs_count,
+               'stdev_fitness' : fitness_stdev,
+               'p_Welch' : p_Welch,
+                'p_Welch_BH' : p_Welch_BH,
+                'p_Welch_BH_-log10' : -p_Welch_BH.applymap(np.log10)}, axis=1)
+
+
+    combined_data = combined_data.swaplevel(axis=1).sort_index(axis=1)
+    combined_data.to_csv(out_prefix+'_summaryStats.csv')
+    print('Interpretation completed and results saved.')
+    return combined_data
+
```

### Comparing `pyphe-0.981/pyphe/quantify.py` & `pyphe-0.982/pyphe/quantify.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,418 +1,418 @@
-import os
-import numpy as np
-import pandas as pd
-import math
-from warnings import warn
-from matplotlib import pyplot as plt
-from scipy.spatial import distance
-from scipy.signal import find_peaks
-from scipy.stats import trim_mean
-import math
-
-from skimage.filters import threshold_otsu, gaussian, threshold_local
-from skimage.morphology import remove_small_objects, convex_hull_object
-from skimage.segmentation import clear_border
-from skimage.util import invert
-from skimage.measure import regionprops, label
-from skimage.color import label2rgb
-from skimage.draw import rectangle_perimeter
-
-def make_grid(gd):
-    '''
-    Converts a grid definition to a list (x,y positions) of all vertices in the grid.
-    '''
-    
-    rows, cols, x1, y1, x2, y2 = gd
-    xpos = np.linspace(x1, x2, num=cols)
-    ypos = np.linspace(y1, y2, num=rows)
-    
-    griddistx = xpos[1] - xpos[0]
-    griddisty = ypos[1] - ypos[0]
-    
-    #Check if spacing similar
-    if (abs(griddistx-griddisty)/(0.5*(griddistx+griddisty))) > 0.1:
-        warn('Uneven spacing between rows and columns. Are you sure this is intended?')
-   
-    #Make dictionary of grid positions
-    grid = {}
-    for r in range(rows):
-        for c in range(cols):
-            grid[(r+1,c+1)] = (ypos[r], xpos[c])
-            
-    return grid, 0.5*(griddistx+griddisty)
-
-
-def make_grid_auto(im, grid):
-
-    nrows, ncols = map(int,grid.split('-'))
-    
-    def find_grid_positions_1d(image, axis, n):
-
-        #extract means across axis
-        imvals = image.mean(axis=axis)
-        imvals = imvals - imvals.min()
-        imvals = imvals / imvals.max()
-
-        #find peaks. Define minimum distance based on image dimension
-        peaks = find_peaks(imvals, distance=(len(imvals)-0.2*len(imvals))/n)[0]
-
-        #find distance between colonies. Use trimmed mean which is robust to outliers. Median is not precise enough (need sub-pixel resolution)
-        med = trim_mean(peaks[1:] - peaks[:-1], 0.2)
-        #for bad input images the distance between colonies times the number of rows/columns can exceed image dimensions. 
-        #In this case, guess the distance based on image dimensions and number of colonies
-        if med*(n-1) > len(imvals):
-            print('Could not detect enough peaks. Guessing grid positions. Please check QC images carefully.')
-            med = (len(imvals)-0.1*len(imvals))/(n-1)
-
-        #create hypothetical, ideal grid based on mean distance
-        to_fit = np.linspace(0, med*(n-1),n)
-
-        #Find the maximum offset and all offset positions to try
-        max_offset = len(imvals)-to_fit[-1]
-        pos_to_try = np.linspace(0,int(max_offset),int(max_offset)+1)
-
-        #Make a cosine function with the same period as the mean distance between colonies
-        b = 2 * math.pi / med
-        x = np.linspace(0,(n-1)*med,int((n-1)*med))
-        y = (1+np.cos(x*b))/2#scale roughly to data
-        errors = [((y - imvals[o:len(y)+o])**2).sum() for o in pos_to_try.astype(int)]
-
-        return to_fit + np.argmin(errors), med
-
-    cols, colmed = find_grid_positions_1d(im,0,ncols)
-    rows, rowmed = find_grid_positions_1d(im,1,nrows)
-
-    grid = {}
-    for ri,r in enumerate(rows):
-        for ci,c in enumerate(cols):
-            grid[(ri+1, ci+1)] = (r, c)
-               
-    return grid, 0.5*(colmed+rowmed)
-    
-
-def match_to_grid(labels, centroids, grid, griddist, d=3, reportAll=False):
-    '''
-    From a list of grid positions and a list of centroids, construct a distance matrix between all pairs and return the best fits as a dictionary.
-    '''
-    
-    #Construct distance matrix as pandas table
-    dm = distance.cdist(np.array(list(centroids)), np.array(list(grid.values())), metric='euclidean')
-    dm = pd.DataFrame(dm, index=labels, columns=map(lambda x: '-'.join(map(str,x)),grid.keys()))
-            
-    #Select matches
-    dm[dm>(griddist/d)] = np.nan
-
-    if not reportAll:
-        #Find best match for each grid position
-        dm = dm.idxmin(axis=0)
-        dm = dm.dropna().astype(int)
-        #Swap index and values
-        #There should never be a blob associated to two blob positions since d>2 is enforced in the command line interface
-        dm = pd.Series(dm.index.values, index=dm)
-        dm = dm.to_dict()        
-        
-    else:
-        #Find best match for each blob
-        dm = dm.idxmin(axis=1)
-        dm = dm.dropna()
-        dm = dm.to_dict()
-            
-    return dm
-
-
-def make_mask(image, t=1, s=1, hardImageThreshold=None, hardSizeThreshold=None, local=False, convexhull=False):
-    '''
-    Identifies suitable morphological components from image by thresholding.
-    '''
-    
-    if local:
-        mask = image > t*threshold_local(image, 151)
-
-    else:
-        if hardImageThreshold:
-            thresh = hardImageThreshold
-        else:
-            thresh = t*threshold_otsu(image)
-            
-        mask = image>thresh
-    
-    #Fill holes. Warning: takes a long time
-    if convexhull:
-        mask = convex_hull_object(mask)
-        
-    #Filter small components. The default threshold is 0.00005 of the image area 
-    if hardSizeThreshold:
-        size_thresh = hardSizeThreshold
-    else:
-        size_thresh = s * np.prod(image.shape) * 0.00005
-    mask = remove_small_objects(mask, min_size=size_thresh)
-    
-    
-    #Clear border
-    mask = clear_border(mask)
-    
-    #Label connected components
-    mask = label(mask)
-    
-    return mask
-
-def check_and_negate(orig_image, negate=True):
-    '''
-    Check if image is greyscale, convert if it isn't. Convert to float and invert intensities.
-    '''
-    image = np.copy(orig_image)
-    
-    #Check if images are grayscale and convert if necessary
-    if len(image.shape) == 3:
-        warn('Image is not in greyscale, converting before processing')
-        image = image.astype(int).mean(axis=2)
-
-    #Convert to float and re-scale to [0,1]            
-    image = image.astype(float)
-    image = image / 255.0
-    
-    #Negate images if required
-    if negate:
-        image = invert(image)
-        
-    return image
-
-def quantify_single_image_size(orig_image, grid, auto, t=1, d=3, s=1, negate=True, reportAll=False, hardImageThreshold=None, hardSizeThreshold=None, localThresh=None, convexhull=False):
-    '''
-    Process a single image to extract colony sizes.
-    '''
-    
-    #Prepare image
-    image = check_and_negate(orig_image, negate=negate)
-    
-    #Create grid
-    if auto:
-        grid, griddist = make_grid_auto(image, grid)
-    else:
-        grid, griddist = make_grid(grid)
-        
-    #Make mask
-    mask = make_mask(image, t=t, s=s, hardImageThreshold=hardImageThreshold, hardSizeThreshold=hardSizeThreshold, local=localThresh, convexhull=convexhull)
-    
-    #Measure regionprobs
-    data = {r.label : {p : r[p] for p in ['label', 'area', 'centroid', 'mean_intensity', 'perimeter']} for r in regionprops(mask, intensity_image=image)}
-    data = pd.DataFrame(data).transpose()
-    
-    blob_to_pos = match_to_grid(data['label'], data['centroid'], grid, griddist, d=d, reportAll=reportAll)
-    
-    #Select only those blobs which have a corresponding grid position
-    data = data.loc[[l in blob_to_pos for l in data['label']]]
-    
-    #Add grid position information to table
-    data['row'] = data['label'].map(lambda x: blob_to_pos[x].split('-')[0])
-    data['column'] = data['label'].map(lambda x: blob_to_pos[x].split('-')[1])
-    
-    #Add circularity
-    data['circularity'] = (4 * math.pi * data['area']) / (data['perimeter']**2)
-    
-    #Make qc image
-    qc = label2rgb(mask, image=orig_image, bg_label=0)
-    
-    return (data, qc)
-
-def quantify_single_image_redness(orig_image, grid, auto, t=1, d=3, s=1, negate=True, reportAll=False, hardImageThreshold=None, hardSizeThreshold=None):
-    '''
-    Process a single image (phloxine mode).
-    '''
-    
-    #Prepare image
-    image = prepare_redness_image(orig_image)
-    
-    #Create grid
-    if auto:
-        grid, griddist = make_grid_auto(image, grid)
-    else:
-        grid, griddist = make_grid(grid)
-    
-    #Make mask
-    #Adjust threshold for redness images slightly, just what works in practise. t parameter is still applied as additional coefficient
-    mask = make_mask(image, t=1.02*t, s=s, hardImageThreshold=hardImageThreshold, hardSizeThreshold=hardSizeThreshold, local=True)
-    
-    #Measure regionprobs
-    data = {r.label : {p : r[p] for p in ['label', 'area', 'centroid', 'mean_intensity', 'perimeter']} for r in regionprops(mask, intensity_image=image)}
-    data = pd.DataFrame(data).transpose()
-    
-    blob_to_pos = match_to_grid(data['label'], data['centroid'], grid, griddist, d=d, reportAll=reportAll)
-    
-    #Select only those blobs which have a corresponding grid position
-    data = data.loc[[l in blob_to_pos for l in data['label']]]
-    
-    #Add grid position information to table
-    data['row'] = data['label'].map(lambda x: blob_to_pos[x].split('-')[0])
-    data['column'] = data['label'].map(lambda x: blob_to_pos[x].split('-')[1])
-    
-    #Add circularity
-    data['circularity'] = (4 * math.pi * data['area']) / (data['perimeter']**2)
-    
-    #Make qc image, add bounding boxes to blobs with grid assigned
-    qc = np.copy(orig_image)
-    for region in regionprops(mask):
-        if region.label in data['label']: 
-            minr, minc, maxr, maxc = region.bbox
-            bboxrows, bboxcols = rectangle_perimeter([minr, minc], end=[maxr, maxc], shape=image.shape, clip=True)
-            qc[bboxrows, bboxcols,:] = np.array((255,255,255))
-
-    return (data, qc)
-    
-def quantify_batch(images, grid, auto, mode, qc='qc_images', out='pyphe_quant', t=1, d=3, s=1, negate=True, reportAll=False, reportFileNames=None, hardImageThreshold=None, hardSizeThreshold=None, localThresh=None, convexhull=False):
-    '''
-    Analyse colony size for batch of plates. Depending on mode, either the quantify_single_image_grey or quantify_single_image_redness function is applied to all images.
-    '''
-
-    for fname, im in zip(images.files, images):
-        
-        if mode == 'batch':
-            data, qc_image = quantify_single_image_size(np.copy(im), grid, auto, t=t, d=d, s=s, negate=negate, reportAll=reportAll, hardImageThreshold=hardImageThreshold, hardSizeThreshold=hardSizeThreshold, localThresh=localThresh, convexhull=convexhull)
-        elif mode == 'redness':
-            data, qc_image = quantify_single_image_redness(np.copy(im), grid, auto, t=t, d=d, s=s, negate=negate, reportAll=reportAll, hardImageThreshold=hardImageThreshold, hardSizeThreshold=hardSizeThreshold)
-        else:
-            raise ValueError('Mode must be batch or redness.')
-        
-        image_name = os.path.basename(fname)
-        if not reportAll:
-            data.drop('label', axis=1).to_csv(os.path.join(out, image_name+'.csv'))
-        else:
-            data.to_csv(os.path.join(out, image_name+'.csv'))
-    
-        #Add labels and grid positions to qc image and save
-        fig, ax = plt.subplots()
-        ax.imshow(qc_image)
-        if not reportAll:
-            data['annot'] = data['row'].astype(str) + '-' + data['column'].astype(str)
-        else:
-            data['annot'] = data['label']
-        if mode == 'redness':
-            data['annot'] = data['annot'] + '\n' + data['mean_intensity'].astype(float).round(4).astype(str)
-        for i,r in data.iterrows():
-            ax.text(r['centroid'][1], r['centroid'][0], r['annot'], fontdict={'size':1.5, 'color':'w'})
-                
-        plt.savefig(os.path.join(qc, 'qc_'+image_name+'.png'), dpi=900)
-        plt.clf()
-        plt.close()
-
-def quantify_single_image_fromTimecourse(orig_image, mask, negate=True, calibrate='x'):
-    '''
-    Apply a previously determined mask to an image from a timeseries.
-    '''
-    
-    #Prepare image. Don't do any scaling. The scaling depends on the maximum and minimum pixel intensity which is not very stable.
-    #Negate images if required
-    if negate:
-        image = invert(orig_image)
-    else:
-        image = orig_image
-
-    #Get background intensity
-    bgmask = (mask==0).astype(int)
-    bgdata = {r.label : r['mean_intensity'] for r in regionprops(bgmask, intensity_image=image)}
-    bgmean = bgdata[1]
-    #subtract mean background from image, floor again to avoid rare case of negative values
-    image = image - bgmean
-    image[image<0] = 0
-
-    #transform with calibration function
-    image_trafo = eval(calibrate.replace('x', 'image'))
-    
-    #Get intensity data for each blob
-    data = {r.label : r['mean_intensity']*r['area'] for r in regionprops(mask, intensity_image=image_trafo)}
-
-    return data
-
-        
-def quantify_timecourse(images, grid, auto, qc='qc_images', out='pyphe_quant', t=1, d=3, s=1, negate=True, reportAll=False, reportFileNames=False, hardImageThreshold=None, hardSizeThreshold=None, calibrate='x', timepoints=None, localThresh=None, convexhull=False):
-    '''
-    Analyse a timeseries of images. Make the mask based on the last image and extract intensity information from all previous images based on that.
-    '''
-    #Get final image
-    if negate:
-        fimage = invert(images[-1])   
-    else: 
-        fimage = images[-1]
-    
-    #Create grid
-    if auto:
-        grid, griddist = make_grid_auto(fimage, grid)
-    else:
-        grid, griddist = make_grid(grid)
-    
-    #Make mask
-    mask = make_mask(fimage, t=t, s=s, hardSizeThreshold=hardSizeThreshold, convexhull=convexhull)
-    
-    #Make table of intensities over time
-    data = {fname : quantify_single_image_fromTimecourse(orig_image, mask, negate=negate, calibrate=calibrate) for fname,orig_image in zip(images.files, images)}
-    data = pd.DataFrame(data).transpose()
-    
-    #Get centroids and match to positions
-    centroids = {r.label : r['centroid'] for r in regionprops(mask)}
-    blob_to_pos = match_to_grid(centroids.keys(), centroids.values(), grid, griddist, d=d, reportAll=reportAll)
-    
-    #Select only those blobs which have a corresponding grid position
-    data = data.loc[:,[l in blob_to_pos for l in data.columns]]
-    
-    #If not reportAll, replace blobs by grid position information and sort
-    if not reportAll:
-        data.columns = data.columns.map(lambda x: blob_to_pos[x])
-        data = data[sorted(list(data), key=lambda x: 100*int(x.split('-')[0]) + int(x.split('-')[1]))]
-    
-    #Set correct index
-    if not reportFileNames:
-        if timepoints:
-            with open(timepoints, 'r') as tpfile:
-                tps = tpfile.readlines()
-                tps = [s.strip() for s in tps]
-            if len(tps) == len(data.index):
-                data.index = tps
-            else:
-                warn('Could not read timepoints from file as the file has the wrong number of entries. Falling back to simple numbering.')
-                data.index = range(1,len(data.index)+1)
-        else:
-            data.index = range(1,len(data.index)+1)
-
-    #Save table
-    image_name = os.path.basename(images.files[-1])
-    data.to_csv(os.path.join(out, image_name+'.csv'))
-
-    #make qc image
-    qc_image = label2rgb(mask, image=images[-1], bg_label=0)
-    fig, ax = plt.subplots()
-    ax.imshow(qc_image)
-    if not reportAll:
-        for blob in blob_to_pos:
-            ax.text(centroids[blob][1], centroids[blob][0], blob_to_pos[blob], fontdict={'size':1.5, 'color':'w'})
-    else:
-        for blob in blob_to_pos:
-            ax.text(centroids[blob][1], centroids[blob][0], blob, fontdict={'size':1.5, 'color':'w'})
-
-    plt.savefig(os.path.join(qc, 'qc_'+image_name+'.png'), dpi=900)
-    plt.clf()
-    plt.close()
-
-def prepare_redness_image(orig_image):
-    '''
-    Prepare image for thresholding and analysis. Channels are weighted by (0, 0.5, 1) and summed. The background is estimated by gaussian blur and subtracted. The image is inverted.
-    '''
-    image = np.copy(orig_image)
-
-    #Color channel transformations and convert to grey
-    image = 0.5*image[:,:,1] + 1*image[:,:,2]
-    #Convert to float and rescale to range [0,1]
-    #I don't think other fancier methods for histogram normalisation are suitable or required since simple thresholding is applied later
-
-    #Estimate background by gaussian. Scale sigma with image area to compensate for different resolutions
-    background = gaussian(image, sigma=np.prod(image.shape)/10000, truncate=4) 
-    image = image - background #This may contain some negative values
-
-    #Scale image to [0,1] in invert
-    image = image.astype(float)
-    image = image - np.min(image)
-    image = image/np.max(image)
-    image = 1 - image
-    
-    return image
-  
-
+import os
+import numpy as np
+import pandas as pd
+import math
+from warnings import warn
+from matplotlib import pyplot as plt
+from scipy.spatial import distance
+from scipy.signal import find_peaks
+from scipy.stats import trim_mean
+import math
+
+from skimage.filters import threshold_otsu, gaussian, threshold_local
+from skimage.morphology import remove_small_objects, convex_hull_object
+from skimage.segmentation import clear_border
+from skimage.util import invert
+from skimage.measure import regionprops, label
+from skimage.color import label2rgb
+from skimage.draw import rectangle_perimeter
+
+def make_grid(gd):
+    '''
+    Converts a grid definition to a list (x,y positions) of all vertices in the grid.
+    '''
+    
+    rows, cols, x1, y1, x2, y2 = gd
+    xpos = np.linspace(x1, x2, num=cols)
+    ypos = np.linspace(y1, y2, num=rows)
+    
+    griddistx = xpos[1] - xpos[0]
+    griddisty = ypos[1] - ypos[0]
+    
+    #Check if spacing similar
+    if (abs(griddistx-griddisty)/(0.5*(griddistx+griddisty))) > 0.1:
+        warn('Uneven spacing between rows and columns. Are you sure this is intended?')
+   
+    #Make dictionary of grid positions
+    grid = {}
+    for r in range(rows):
+        for c in range(cols):
+            grid[(r+1,c+1)] = (ypos[r], xpos[c])
+            
+    return grid, 0.5*(griddistx+griddisty)
+
+
+def make_grid_auto(im, grid):
+
+    nrows, ncols = map(int,grid.split('-'))
+    
+    def find_grid_positions_1d(image, axis, n):
+
+        #extract means across axis
+        imvals = image.mean(axis=axis)
+        imvals = imvals - imvals.min()
+        imvals = imvals / imvals.max()
+
+        #find peaks. Define minimum distance based on image dimension
+        peaks = find_peaks(imvals, distance=(len(imvals)-0.2*len(imvals))/n)[0]
+
+        #find distance between colonies. Use trimmed mean which is robust to outliers. Median is not precise enough (need sub-pixel resolution)
+        med = trim_mean(peaks[1:] - peaks[:-1], 0.2)
+        #for bad input images the distance between colonies times the number of rows/columns can exceed image dimensions. 
+        #In this case, guess the distance based on image dimensions and number of colonies
+        if med*(n-1) > len(imvals):
+            print('Could not detect enough peaks. Guessing grid positions. Please check QC images carefully.')
+            med = (len(imvals)-0.1*len(imvals))/(n-1)
+
+        #create hypothetical, ideal grid based on mean distance
+        to_fit = np.linspace(0, med*(n-1),n)
+
+        #Find the maximum offset and all offset positions to try
+        max_offset = len(imvals)-to_fit[-1]
+        pos_to_try = np.linspace(0,int(max_offset),int(max_offset)+1)
+
+        #Make a cosine function with the same period as the mean distance between colonies
+        b = 2 * math.pi / med
+        x = np.linspace(0,(n-1)*med,int((n-1)*med))
+        y = (1+np.cos(x*b))/2#scale roughly to data
+        errors = [((y - imvals[o:len(y)+o])**2).sum() for o in pos_to_try.astype(int)]
+
+        return to_fit + np.argmin(errors), med
+
+    cols, colmed = find_grid_positions_1d(im,0,ncols)
+    rows, rowmed = find_grid_positions_1d(im,1,nrows)
+
+    grid = {}
+    for ri,r in enumerate(rows):
+        for ci,c in enumerate(cols):
+            grid[(ri+1, ci+1)] = (r, c)
+               
+    return grid, 0.5*(colmed+rowmed)
+    
+
+def match_to_grid(labels, centroids, grid, griddist, d=3, reportAll=False):
+    '''
+    From a list of grid positions and a list of centroids, construct a distance matrix between all pairs and return the best fits as a dictionary.
+    '''
+    
+    #Construct distance matrix as pandas table
+    dm = distance.cdist(np.array(list(centroids)), np.array(list(grid.values())), metric='euclidean')
+    dm = pd.DataFrame(dm, index=labels, columns=map(lambda x: '-'.join(map(str,x)),grid.keys()))
+            
+    #Select matches
+    dm[dm>(griddist/d)] = np.nan
+
+    if not reportAll:
+        #Find best match for each grid position
+        dm = dm.idxmin(axis=0)
+        dm = dm.dropna().astype(int)
+        #Swap index and values
+        #There should never be a blob associated to two blob positions since d>2 is enforced in the command line interface
+        dm = pd.Series(dm.index.values, index=dm)
+        dm = dm.to_dict()        
+        
+    else:
+        #Find best match for each blob
+        dm = dm.idxmin(axis=1)
+        dm = dm.dropna()
+        dm = dm.to_dict()
+            
+    return dm
+
+
+def make_mask(image, t=1, s=1, hardImageThreshold=None, hardSizeThreshold=None, local=False, convexhull=False):
+    '''
+    Identifies suitable morphological components from image by thresholding.
+    '''
+    
+    if local:
+        mask = image > t*threshold_local(image, 151)
+
+    else:
+        if hardImageThreshold:
+            thresh = hardImageThreshold
+        else:
+            thresh = t*threshold_otsu(image)
+            
+        mask = image>thresh
+    
+    #Fill holes. Warning: takes a long time
+    if convexhull:
+        mask = convex_hull_object(mask)
+        
+    #Filter small components. The default threshold is 0.00005 of the image area 
+    if hardSizeThreshold:
+        size_thresh = hardSizeThreshold
+    else:
+        size_thresh = s * np.prod(image.shape) * 0.00005
+    mask = remove_small_objects(mask, min_size=size_thresh)
+    
+    
+    #Clear border
+    mask = clear_border(mask)
+    
+    #Label connected components
+    mask = label(mask)
+    
+    return mask
+
+def check_and_negate(orig_image, negate=True):
+    '''
+    Check if image is greyscale, convert if it isn't. Convert to float and invert intensities.
+    '''
+    image = np.copy(orig_image)
+    
+    #Check if images are grayscale and convert if necessary
+    if len(image.shape) == 3:
+        warn('Image is not in greyscale, converting before processing')
+        image = image.astype(int).mean(axis=2)
+
+    #Convert to float and re-scale to [0,1]            
+    image = image.astype(float)
+    image = image / 255.0
+    
+    #Negate images if required
+    if negate:
+        image = invert(image)
+        
+    return image
+
+def quantify_single_image_size(orig_image, grid, auto, t=1, d=3, s=1, negate=True, reportAll=False, hardImageThreshold=None, hardSizeThreshold=None, localThresh=None, convexhull=False):
+    '''
+    Process a single image to extract colony sizes.
+    '''
+    
+    #Prepare image
+    image = check_and_negate(orig_image, negate=negate)
+    
+    #Create grid
+    if auto:
+        grid, griddist = make_grid_auto(image, grid)
+    else:
+        grid, griddist = make_grid(grid)
+        
+    #Make mask
+    mask = make_mask(image, t=t, s=s, hardImageThreshold=hardImageThreshold, hardSizeThreshold=hardSizeThreshold, local=localThresh, convexhull=convexhull)
+    
+    #Measure regionprobs
+    data = {r.label : {p : r[p] for p in ['label', 'area', 'centroid', 'mean_intensity', 'perimeter']} for r in regionprops(mask, intensity_image=image)}
+    data = pd.DataFrame(data).transpose()
+    
+    blob_to_pos = match_to_grid(data['label'], data['centroid'], grid, griddist, d=d, reportAll=reportAll)
+    
+    #Select only those blobs which have a corresponding grid position
+    data = data.loc[[l in blob_to_pos for l in data['label']]]
+    
+    #Add grid position information to table
+    data['row'] = data['label'].map(lambda x: blob_to_pos[x].split('-')[0])
+    data['column'] = data['label'].map(lambda x: blob_to_pos[x].split('-')[1])
+    
+    #Add circularity
+    data['circularity'] = (4 * math.pi * data['area']) / (data['perimeter']**2)
+    
+    #Make qc image
+    qc = label2rgb(mask, image=orig_image, bg_label=0)
+    
+    return (data, qc)
+
+def quantify_single_image_redness(orig_image, grid, auto, t=1, d=3, s=1, negate=True, reportAll=False, hardImageThreshold=None, hardSizeThreshold=None):
+    '''
+    Process a single image (phloxine mode).
+    '''
+    
+    #Prepare image
+    image = prepare_redness_image(orig_image)
+    
+    #Create grid
+    if auto:
+        grid, griddist = make_grid_auto(image, grid)
+    else:
+        grid, griddist = make_grid(grid)
+    
+    #Make mask
+    #Adjust threshold for redness images slightly, just what works in practise. t parameter is still applied as additional coefficient
+    mask = make_mask(image, t=1.02*t, s=s, hardImageThreshold=hardImageThreshold, hardSizeThreshold=hardSizeThreshold, local=True)
+    
+    #Measure regionprobs
+    data = {r.label : {p : r[p] for p in ['label', 'area', 'centroid', 'mean_intensity', 'perimeter']} for r in regionprops(mask, intensity_image=image)}
+    data = pd.DataFrame(data).transpose()
+    
+    blob_to_pos = match_to_grid(data['label'], data['centroid'], grid, griddist, d=d, reportAll=reportAll)
+    
+    #Select only those blobs which have a corresponding grid position
+    data = data.loc[[l in blob_to_pos for l in data['label']]]
+    
+    #Add grid position information to table
+    data['row'] = data['label'].map(lambda x: blob_to_pos[x].split('-')[0])
+    data['column'] = data['label'].map(lambda x: blob_to_pos[x].split('-')[1])
+    
+    #Add circularity
+    data['circularity'] = (4 * math.pi * data['area']) / (data['perimeter']**2)
+    
+    #Make qc image, add bounding boxes to blobs with grid assigned
+    qc = np.copy(orig_image)
+    for region in regionprops(mask):
+        if region.label in data['label']: 
+            minr, minc, maxr, maxc = region.bbox
+            bboxrows, bboxcols = rectangle_perimeter([minr, minc], end=[maxr, maxc], shape=image.shape, clip=True)
+            qc[bboxrows, bboxcols,:] = np.array((255,255,255))
+
+    return (data, qc)
+    
+def quantify_batch(images, grid, auto, mode, qc='qc_images', out='pyphe_quant', t=1, d=3, s=1, negate=True, reportAll=False, reportFileNames=None, hardImageThreshold=None, hardSizeThreshold=None, localThresh=None, convexhull=False):
+    '''
+    Analyse colony size for batch of plates. Depending on mode, either the quantify_single_image_grey or quantify_single_image_redness function is applied to all images.
+    '''
+
+    for fname, im in zip(images.files, images):
+        
+        if mode == 'batch':
+            data, qc_image = quantify_single_image_size(np.copy(im), grid, auto, t=t, d=d, s=s, negate=negate, reportAll=reportAll, hardImageThreshold=hardImageThreshold, hardSizeThreshold=hardSizeThreshold, localThresh=localThresh, convexhull=convexhull)
+        elif mode == 'redness':
+            data, qc_image = quantify_single_image_redness(np.copy(im), grid, auto, t=t, d=d, s=s, negate=negate, reportAll=reportAll, hardImageThreshold=hardImageThreshold, hardSizeThreshold=hardSizeThreshold)
+        else:
+            raise ValueError('Mode must be batch or redness.')
+        
+        image_name = os.path.basename(fname)
+        if not reportAll:
+            data.drop('label', axis=1).to_csv(os.path.join(out, image_name+'.csv'))
+        else:
+            data.to_csv(os.path.join(out, image_name+'.csv'))
+    
+        #Add labels and grid positions to qc image and save
+        fig, ax = plt.subplots()
+        ax.imshow(qc_image)
+        if not reportAll:
+            data['annot'] = data['row'].astype(str) + '-' + data['column'].astype(str)
+        else:
+            data['annot'] = data['label']
+        if mode == 'redness':
+            data['annot'] = data['annot'] + '\n' + data['mean_intensity'].astype(float).round(4).astype(str)
+        for i,r in data.iterrows():
+            ax.text(r['centroid'][1], r['centroid'][0], r['annot'], fontdict={'size':1.5, 'color':'w'})
+                
+        plt.savefig(os.path.join(qc, 'qc_'+image_name+'.png'), dpi=900)
+        plt.clf()
+        plt.close()
+
+def quantify_single_image_fromTimecourse(orig_image, mask, negate=True, calibrate='x'):
+    '''
+    Apply a previously determined mask to an image from a timeseries.
+    '''
+    
+    #Prepare image. Don't do any scaling. The scaling depends on the maximum and minimum pixel intensity which is not very stable.
+    #Negate images if required
+    if negate:
+        image = invert(orig_image)
+    else:
+        image = orig_image
+
+    #Get background intensity
+    bgmask = (mask==0).astype(int)
+    bgdata = {r.label : r['mean_intensity'] for r in regionprops(bgmask, intensity_image=image)}
+    bgmean = bgdata[1]
+    #subtract mean background from image, floor again to avoid rare case of negative values
+    image = image - bgmean
+    image[image<0] = 0
+
+    #transform with calibration function
+    image_trafo = eval(calibrate.replace('x', 'image'))
+    
+    #Get intensity data for each blob
+    data = {r.label : r['mean_intensity']*r['area'] for r in regionprops(mask, intensity_image=image_trafo)}
+
+    return data
+
+        
+def quantify_timecourse(images, grid, auto, qc='qc_images', out='pyphe_quant', t=1, d=3, s=1, negate=True, reportAll=False, reportFileNames=False, hardImageThreshold=None, hardSizeThreshold=None, calibrate='x', timepoints=None, localThresh=None, convexhull=False):
+    '''
+    Analyse a timeseries of images. Make the mask based on the last image and extract intensity information from all previous images based on that.
+    '''
+    #Get final image
+    if negate:
+        fimage = invert(images[-1])   
+    else: 
+        fimage = images[-1]
+    
+    #Create grid
+    if auto:
+        grid, griddist = make_grid_auto(fimage, grid)
+    else:
+        grid, griddist = make_grid(grid)
+    
+    #Make mask
+    mask = make_mask(fimage, t=t, s=s, hardSizeThreshold=hardSizeThreshold, convexhull=convexhull)
+    
+    #Make table of intensities over time
+    data = {fname : quantify_single_image_fromTimecourse(orig_image, mask, negate=negate, calibrate=calibrate) for fname,orig_image in zip(images.files, images)}
+    data = pd.DataFrame(data).transpose()
+    
+    #Get centroids and match to positions
+    centroids = {r.label : r['centroid'] for r in regionprops(mask)}
+    blob_to_pos = match_to_grid(centroids.keys(), centroids.values(), grid, griddist, d=d, reportAll=reportAll)
+    
+    #Select only those blobs which have a corresponding grid position
+    data = data.loc[:,[l in blob_to_pos for l in data.columns]]
+    
+    #If not reportAll, replace blobs by grid position information and sort
+    if not reportAll:
+        data.columns = data.columns.map(lambda x: blob_to_pos[x])
+        data = data[sorted(list(data), key=lambda x: 100*int(x.split('-')[0]) + int(x.split('-')[1]))]
+    
+    #Set correct index
+    if not reportFileNames:
+        if timepoints:
+            with open(timepoints, 'r') as tpfile:
+                tps = tpfile.readlines()
+                tps = [s.strip() for s in tps]
+            if len(tps) == len(data.index):
+                data.index = tps
+            else:
+                warn('Could not read timepoints from file as the file has the wrong number of entries. Falling back to simple numbering.')
+                data.index = range(1,len(data.index)+1)
+        else:
+            data.index = range(1,len(data.index)+1)
+
+    #Save table
+    image_name = os.path.basename(images.files[-1])
+    data.to_csv(os.path.join(out, image_name+'.csv'))
+
+    #make qc image
+    qc_image = label2rgb(mask, image=images[-1], bg_label=0)
+    fig, ax = plt.subplots()
+    ax.imshow(qc_image)
+    if not reportAll:
+        for blob in blob_to_pos:
+            ax.text(centroids[blob][1], centroids[blob][0], blob_to_pos[blob], fontdict={'size':1.5, 'color':'w'})
+    else:
+        for blob in blob_to_pos:
+            ax.text(centroids[blob][1], centroids[blob][0], blob, fontdict={'size':1.5, 'color':'w'})
+
+    plt.savefig(os.path.join(qc, 'qc_'+image_name+'.png'), dpi=900)
+    plt.clf()
+    plt.close()
+
+def prepare_redness_image(orig_image):
+    '''
+    Prepare image for thresholding and analysis. Channels are weighted by (0, 0.5, 1) and summed. The background is estimated by gaussian blur and subtracted. The image is inverted.
+    '''
+    image = np.copy(orig_image)
+
+    #Color channel transformations and convert to grey
+    image = 0.5*image[:,:,1] + 1*image[:,:,2]
+    #Convert to float and rescale to range [0,1]
+    #I don't think other fancier methods for histogram normalisation are suitable or required since simple thresholding is applied later
+
+    #Estimate background by gaussian. Scale sigma with image area to compensate for different resolutions
+    background = gaussian(image, sigma=np.prod(image.shape)/10000, truncate=4) 
+    image = image - background #This may contain some negative values
+
+    #Scale image to [0,1] in invert
+    image = image.astype(float)
+    image = image - np.min(image)
+    image = image/np.max(image)
+    image = 1 - image
+    
+    return image
+  
+
```

### Comparing `pyphe-0.981/pyphe/scan.py` & `pyphe-0.982/pyphe/scan.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-from shutil import which
-from subprocess import check_output
-from warnings import warn
-import sys
-from os import mkdir
-import numpy as np
-from datetime import datetime
-import time
-
-def find_scanner(scanner_index):
-    '''
-    This function performs a few vital checks before initialising scan sequence and selects a suitable scanner. 
-    '''
-    #Check if ImageMagick can be called from command line
-    if which('convert') is None:
-        raise ImportError("Cannot find ImageMagick's convert tool. Please make sure ImageMagick is installed and can be called from the command line.")
-    
-    #Look for scanners
-    print('Searching for scanners.')
-    scanner_list = check_output('scanimage -L', shell=True).decode('ascii')
-    if 'No scanners were identified' in scanner_list:
-        raise RuntimeError('Could not find any scanners. Please check scanners are connected and turned on, work with SANE and the TPU8x10 mode is enabled.') 
-    scanner_list = [s for s in scanner_list.split('\n') if not s.strip()=='']
-    scanner_list = [s.split()[1][1:-1] for s in scanner_list]
-    print('Scanners found: ' + str(scanner_list))
-    scanner = scanner_list[scanner_index-1]
-
-    print('Using scanner %s'%scanner)
-    return scanner
-    
-def scan_batch(n, plateStart, prefix, postfix, fixture, resolution, geometries, scanner, mode, format):
-    '''
-    High-level function for scanning a batch of plates. 
-    '''
-    
-    ppscan = len(geometries[fixture])#plates per scan
-
-    #Get geometry string and adapt to resolution
-    geometry = geometries[fixture]
-
-    print('Loaded geometry settings for fixture %s: '%fixture + str(geometry))
-    geometry_temp = []
-    for g in geometry:
-        glist = list(map(lambda x: str(int(int(x)*(resolution/600.0))), g.replace('+', 'x').split('x')))
-        geometry_temp.append(glist[0] + 'x' + glist[1] + '+' + glist[2] + '+' + glist[3])
-
-    print('Geometry settings scaled to resolution: ' + str(geometry_temp))
-    geometry = geometry_temp
-
-    wdir = '%s_%s/'%(prefix,postfix)
-    mkdir(wdir)
-    rdir = wdir + 'raw_scans/'
-    mkdir(rdir)
-    print('Successfully created directories. Please make sure the scanner is turned on.')
-
-    nscans = int(np.ceil(n/float(ppscan)))
-    labels = list(map(str, range(plateStart, plateStart+n)))
-    labels += ['empty']*(ppscan-1)#Max number of emtpy bays in last scan
-    for i in range(1, nscans+1):
-        print('Preparing for scan %i out of %i'%(i,nscans))
-        print('Please load the scanner as follows:')
-        for q in range(1,ppscan+1):
-            print('Bay %i -> Plate %s'%(q, labels[(i-1)*ppscan+(q-1)]))
-
-        ready = None
-        while not ready:
-            try:
-                inp = input('If ready, enter y to start scan > ')
-                if inp == 'y':
-                    ready = True
-                else:
-                    raise Exception
-            except Exception:
-                print('Invalid input')
-
-        source = 'TPU8x10' if mode=='Gray' else 'Flatbed'
-
-        cmdStr = 'scanimage --source %s --mode %s --resolution %i --format=tiff --device-name=%s > %s%s_rawscan%s_%s.tiff'%(source, mode, resolution, scanner, rdir, prefix, i, postfix)
-        check_output(cmdStr, shell=True)
-
-        for plate in range(ppscan):
-            plateNr = (i-1)*ppscan+plate
-            if plateNr < n:
-                cmdStr = 'convert %s%s_rawscan%s_%s.tiff -crop %s +repage -rotate 90 -flop %s%s_%i_%s.%s'%(rdir, prefix, i, postfix, geometry[plate], wdir, prefix, plateNr+plateStart, postfix, format)
-                check_output(cmdStr, shell=True)
-
-
-    print('Done')
-    
-
-def scan_timecourse(nscans, interval, prefix, postfix, fixture, resolution, geometries, scanner, mode, format):
-    '''
-    High-level function for acquiring image timeseries.
-    '''
- 
-    ppscan = len(geometries[fixture])#plates per scan
-    
-    #Get geometry string and adapt to resolution
-    geometry = geometries[fixture]
-    
-    print('Loaded geometry settings for fixture %s: '%fixture + str(geometry))
-    geometry_temp = []
-    for g in geometry:
-        glist = list(map(lambda x: str(int(int(x)*(resolution/600.0))), g.replace('+', 'x').split('x')))
-        geometry_temp.append(glist[0] + 'x' + glist[1] + '+' + glist[2] + '+' + glist[3])
-
-    print('Geometry settings scaled to resolution: ' + str(geometry_temp))
-    geometry = geometry_temp
-
-    #Create directories
-    wdir = '%s_%s/'%(prefix,postfix)
-    mkdir(wdir)
-    for q in range(1, ppscan+1):
-        mkdir(wdir+'plate_'+str(q))
-    rdir = wdir + 'raw_scans/'
-    mkdir(rdir)
-    
-    #Open log
-    log = open(wdir+'/scanlog.txt', 'w')
-    timepoints = open(wdir+'/timepoints.txt', 'w')
-    log.write(str(datetime.now()) + ' - Started scanplates-timecourse with the following parameters: ' + ' ,'.join(map(str,[nscans, interval, prefix, postfix, fixture, resolution, geometries, scanner, mode])) + '\n')
-    
-    print('Successfully created directories.')
-
-    starttime = datetime.now()
-    for i in range(1, nscans+1):
-        print('Preparing for scan %i out of %i'%(i,nscans))
-
-        source = 'TPU8x10' if mode=='Gray' else 'Flatbed'
-        
-        cmdStr = 'scanimage --source %s --mode %s --resolution %i --format=tiff --device-name=%s > %s%s_rawscan%i_%s.tiff'%(source, mode, resolution, scanner, rdir, prefix, i, postfix)
-        check_output(cmdStr, shell=True)
-
-        for plate in range(ppscan):
-            cmdStr = 'convert %s%s_rawscan%i_%s.tiff -crop %s +repage -rotate 90 -flop %s%s/%s_%i_%s_plate%i.%s'%(rdir, prefix, i, postfix, geometry[plate], wdir, 'plate_'+str(plate+1), prefix, i, postfix, plate+1, format)
-            check_output(cmdStr, shell=True)
-
-
-        log.write(str(datetime.now()) + ' - Scan %i completed sucessfully\n'%i)
-        log.flush()
-        timepoints.write(str((datetime.now() - starttime).total_seconds()/(60*60.0)) + '\n')
-        timepoints.flush()
-        time.sleep(interval*60)#Convert to seconds
-        
-    log.close()
-    timepoints.close()
+from shutil import which
+from subprocess import check_output
+from warnings import warn
+import sys
+from os import mkdir
+import numpy as np
+from datetime import datetime
+import time
+
+def find_scanner(scanner_index):
+    '''
+    This function performs a few vital checks before initialising scan sequence and selects a suitable scanner. 
+    '''
+    #Check if ImageMagick can be called from command line
+    if which('convert') is None:
+        raise ImportError("Cannot find ImageMagick's convert tool. Please make sure ImageMagick is installed and can be called from the command line.")
+    
+    #Look for scanners
+    print('Searching for scanners.')
+    scanner_list = check_output('scanimage -L', shell=True).decode('ascii')
+    if 'No scanners were identified' in scanner_list:
+        raise RuntimeError('Could not find any scanners. Please check scanners are connected and turned on, work with SANE and the TPU8x10 mode is enabled.') 
+    scanner_list = [s for s in scanner_list.split('\n') if not s.strip()=='']
+    scanner_list = [s.split()[1][1:-1] for s in scanner_list]
+    print('Scanners found: ' + str(scanner_list))
+    scanner = scanner_list[scanner_index-1]
+
+    print('Using scanner %s'%scanner)
+    return scanner
+    
+def scan_batch(n, plateStart, prefix, postfix, fixture, resolution, geometries, scanner, mode, format):
+    '''
+    High-level function for scanning a batch of plates. 
+    '''
+    
+    ppscan = len(geometries[fixture])#plates per scan
+
+    #Get geometry string and adapt to resolution
+    geometry = geometries[fixture]
+
+    print('Loaded geometry settings for fixture %s: '%fixture + str(geometry))
+    geometry_temp = []
+    for g in geometry:
+        glist = list(map(lambda x: str(int(int(x)*(resolution/600.0))), g.replace('+', 'x').split('x')))
+        geometry_temp.append(glist[0] + 'x' + glist[1] + '+' + glist[2] + '+' + glist[3])
+
+    print('Geometry settings scaled to resolution: ' + str(geometry_temp))
+    geometry = geometry_temp
+
+    wdir = '%s_%s/'%(prefix,postfix)
+    mkdir(wdir)
+    rdir = wdir + 'raw_scans/'
+    mkdir(rdir)
+    print('Successfully created directories. Please make sure the scanner is turned on.')
+
+    nscans = int(np.ceil(n/float(ppscan)))
+    labels = list(map(str, range(plateStart, plateStart+n)))
+    labels += ['empty']*(ppscan-1)#Max number of emtpy bays in last scan
+    for i in range(1, nscans+1):
+        print('Preparing for scan %i out of %i'%(i,nscans))
+        print('Please load the scanner as follows:')
+        for q in range(1,ppscan+1):
+            print('Bay %i -> Plate %s'%(q, labels[(i-1)*ppscan+(q-1)]))
+
+        ready = None
+        while not ready:
+            try:
+                inp = input('If ready, enter y to start scan > ')
+                if inp == 'y':
+                    ready = True
+                else:
+                    raise Exception
+            except Exception:
+                print('Invalid input')
+
+        source = 'TPU8x10' if mode=='Gray' else 'Flatbed'
+
+        cmdStr = 'scanimage --source %s --mode %s --resolution %i --format=tiff --device-name=%s > %s%s_rawscan%s_%s.tiff'%(source, mode, resolution, scanner, rdir, prefix, i, postfix)
+        check_output(cmdStr, shell=True)
+
+        for plate in range(ppscan):
+            plateNr = (i-1)*ppscan+plate
+            if plateNr < n:
+                cmdStr = 'convert %s%s_rawscan%s_%s.tiff -crop %s +repage -rotate 90 -flop %s%s_%i_%s.%s'%(rdir, prefix, i, postfix, geometry[plate], wdir, prefix, plateNr+plateStart, postfix, format)
+                check_output(cmdStr, shell=True)
+
+
+    print('Done')
+    
+
+def scan_timecourse(nscans, interval, prefix, postfix, fixture, resolution, geometries, scanner, mode, format):
+    '''
+    High-level function for acquiring image timeseries.
+    '''
+ 
+    ppscan = len(geometries[fixture])#plates per scan
+    
+    #Get geometry string and adapt to resolution
+    geometry = geometries[fixture]
+    
+    print('Loaded geometry settings for fixture %s: '%fixture + str(geometry))
+    geometry_temp = []
+    for g in geometry:
+        glist = list(map(lambda x: str(int(int(x)*(resolution/600.0))), g.replace('+', 'x').split('x')))
+        geometry_temp.append(glist[0] + 'x' + glist[1] + '+' + glist[2] + '+' + glist[3])
+
+    print('Geometry settings scaled to resolution: ' + str(geometry_temp))
+    geometry = geometry_temp
+
+    #Create directories
+    wdir = '%s_%s/'%(prefix,postfix)
+    mkdir(wdir)
+    for q in range(1, ppscan+1):
+        mkdir(wdir+'plate_'+str(q))
+    rdir = wdir + 'raw_scans/'
+    mkdir(rdir)
+    
+    #Open log
+    log = open(wdir+'/scanlog.txt', 'w')
+    timepoints = open(wdir+'/timepoints.txt', 'w')
+    log.write(str(datetime.now()) + ' - Started scanplates-timecourse with the following parameters: ' + ' ,'.join(map(str,[nscans, interval, prefix, postfix, fixture, resolution, geometries, scanner, mode])) + '\n')
+    
+    print('Successfully created directories.')
+
+    starttime = datetime.now()
+    for i in range(1, nscans+1):
+        print('Preparing for scan %i out of %i'%(i,nscans))
+
+        source = 'TPU8x10' if mode=='Gray' else 'Flatbed'
+        
+        cmdStr = 'scanimage --source %s --mode %s --resolution %i --format=tiff --device-name=%s > %s%s_rawscan%i_%s.tiff'%(source, mode, resolution, scanner, rdir, prefix, i, postfix)
+        check_output(cmdStr, shell=True)
+
+        for plate in range(ppscan):
+            cmdStr = 'convert %s%s_rawscan%i_%s.tiff -crop %s +repage -rotate 90 -flop %s%s/%s_%i_%s_plate%i.%s'%(rdir, prefix, i, postfix, geometry[plate], wdir, 'plate_'+str(plate+1), prefix, i, postfix, plate+1, format)
+            check_output(cmdStr, shell=True)
+
+
+        log.write(str(datetime.now()) + ' - Scan %i completed sucessfully\n'%i)
+        log.flush()
+        timepoints.write(str((datetime.now() - starttime).total_seconds()/(60*60.0)) + '\n')
+        timepoints.flush()
+        time.sleep(interval*60)#Convert to seconds
+        
+    log.close()
+    timepoints.close()
```

### Comparing `pyphe-0.981/pyphe.egg-info/PKG-INFO` & `pyphe-0.982/pyphe.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,491 +1,490 @@
-Metadata-Version: 2.1
-Name: pyphe
-Version: 0.981
-Summary: Python toolbox for phenotype analysis of arrayed microbial colonies
-Home-page: https://github.com/Bahler-Lab/pyphe
-Author: Stephan Kamrad
-Author-email: stephan.kamrad@crick.ac.uk
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![pyphe logo](https://github.com/Bahler-Lab/pyphe/blob/master/icons/toolbox-72dpi_white.png)
-
-# Welcome to the pyphe toolbox
-A python toolbox for phenotype analysis of arrayed microbial colonies written by Stephan Kamrad (stephan.kamrad at crick.ac.uk).
-
-For a quick overview, please see our [10 minute video tutorial](https://www.youtube.com/watch?v=lQ3lXIdhA1c&t=5s).
-
-For a more detailed protocol, including growth curves and viability assays, please see our [protocol preprint](https://www.researchsquare.com/article/rs-401914/v1).
-
-For more background information, please see our [_eLife_ paper](https://elifesciences.org/articles/55160).
-
-Please cite as:
-> Kamrad, S., RodrÃ­guez-LÃ³pez, M., Cotobal, C., Correia-Melo, C., Ralser M., BÃ¤hler J. (2020). Pyphe, a python toolbox for assessing microbial growth and cell viability in high-throughput colony screens. eLife 9:e55160
-
-## Installation
-1. Most tools are cross-platform compatible but scanning will only work on a Linux OS. The scanners need to be accessible by [SANE](http://www.sane-project.org/) and [ImageMagick](https://imagemagick.org/) needs to be installed and accessible from the command line.
-2. Pyphe requires Python 3 and a few common packages, available through the [anaconda distribution](https://www.anaconda.com/distribution/).
-3. Install pyphe by running 'pip install pyphe' in your terminal.
-4. Open a new terminal and try and run 'pyphe-quantify -h' which should show the help page of one of pyphe's command line tools. On Windows, make sure you are using the Anaconda Prompt, not the Anaconda Powershell Prompt.
-
-
-## Overview
-A typical fitness screen with pyphe will involve:
-1. Image acquisition with [_pyphe-scan_](#pyphe-scan), or [_pyphe-scan-timecourse_](#pyphe-scan-timecourse)
-2. Quantification of colony properties from images using [_pyphe-quantify_](#pyphe-quantify). In the case of growth curves, parameters are additionally extracted with [_pyphe-growthcurves_](#pyphe-growthcurves).
-3. Normalisation and data aggregation using [_pyphe-analyse_](#pyphe-analyse).
-4. Statistics and hit calling using [_pyphe-interpret_](#pyphe-interpret)
-Please see our paper for a detailed protocol and explanations of the algorithms.
-
-
-## Support
-Please check the manuals below carefully, they are also available in the terminal by running the command with the -h option only. If things are still not working, please email me (stephan.kamrad@crick.ac.uk) and I will try and help. If you think you have discovered a bug, or would like to request a new feature, please raise an issue on www.github.com/Bahler-Lab/pyphe.
-
-If you get an error like this, make sure you are not using the Anaconda Powershell Prompt:
-```python: can't open file 'C:\Users\user1\Anaconda3\Scripts"C:\Users\user1\Anaconda3\Scripts\pyphe-quantify.bat  -h ': [Errno 22] Invalid argument```
-
-## Manual
-
-All pyphe tools have a similar command line interface, based on the python argparse package. Generally, parameters are set using --<parameter_name> optionally followed by a value. All _pyphe_ tools can be used with relative file paths so make sure to navigate to the correct working directory before running a _pyphe_ command.
-
- 
-### Pyphe-scan
-This tools allows you to take consecutive scans of sets of plates, which are then automatically cropped, rotated and named in in a continuos filename scheme of your choice. 
-
-#### Prerequisites
-1. This tool will only run on Linux operating systems and uses the SANE library for image acquisition.
-
-2. Make sure your scanner is installed correctly and you can acquire images using the scanimage command. The Gray mode will only work on Epson V800 and V850 scanners (potentially the V700 and V750 model as well) and the TPU8x10 transmission scanning source must be enabled. This should work by default if you are using the V800/850 model and a recent Linux OS. Otherwise, there is excellent documentation available from Zackrisson et al. and the [scanomatics pipeline](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5015956/) for how to make this work using a hacked SANE driver. Please see the instructions in their [wiki](https://github.com/Scan-o-Matic/scanomatic/wiki/Installing-scanners).
-
-2. Make sure [ImageMagick](https://imagemagick.org/index.php) is installed and the 'convert' tool can be called from the command line.
-
-3. If the Pyphe toolbox has been installed correctly, you should be able to run _pyphe-scan_ in your terminal. 
-
-4. With a laser cutter, make a fixture to hold your plates in place. We provide an svg file with the cutting shape in the Documentation directory. Use tape to hold your fixture into place, it should be pushed against the back of the scanner (where the cables are) with the top of the plates facing left. Pyphe-scan and pyphe-quantify come pre-configured for using the provided fixture on an Epson V800/V850 scanner but it is easy to add your own fixture and cropping settings. If you want to use your own fixture, see below of how to add the geometry information to pyphe-scan. 
-
-#### Scanning plate batches
-
-1. Open the file manager and navigate to the folder in which you want to save your images. The script will create a sub-folder that begins with the current date to save all your images. 
-
-2. Right click and select 'Open in Terminal'
-
-3. Run scanplates with the options as detaild below. 
-
-```
-usage: pyphe-scan [-h] [--nplates NPLATES] [--start START] [--prefix PREFIX]
-                  [--postfix POSTFIX] [--fixture {som3_edge,som3}]
-                  [--resolution {150,300,600,900,1200}] [--scanner {1,2,3}]
-                  [--mode {Gray,Color}]
-
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --nplates NPLATES     Number of plates to scan. This defaults to 100 and the
-                        script can be terminated by Ctr+C when done.
-  --start START         Where to start numbering from. Defaults to 1.
-  --prefix PREFIX       Name prefix for output files. The default is the
-                        current date YYYYMMDD.
-  --postfix POSTFIX     Name postfix for output files. Defaults to empty
-                        string.
-  --fixture {som3_edge,som3,som3-color}
-                        ID of the fixture you are using.
-  --resolution {150,300,600,900,1200}
-                        Resolution for scanning in dpi. Default is 600.
-  --scanner {1,2,3}     Which scanner to use. Scanners are not uniquely
-                        identified and may switch when turned off/unplugged.
-                        This option does not need to be set when only one
-                        scanner is connected.
-  --mode {Gray,Color}   Which color mode to use for scanning. Defaults to
-                        Gray.
-```
-
-All arguments except the fixture have default values and are optional. A folder prefix_postfix will be created in your current directory and the program will abort if a folder with this name already exists. 
-
-
-
-### Pyphe-scan-timecourse
-
-This tool acquires image timeseries by scanning in fixed time intervals. For each position in the fixture, a folder is created. Image names contain number of scan. Other options for this tool are similar to [_pyphe-scan_](#pyphe-scan). More than one scanner can be connected and used at the same time. Scanner numbers are defined by the order in which they are connected to the computer. Proceed as follows: (1) disconnect all scanners, (2) prepare the first scanner with plates, connect it and turn it on. (3) start scanning with --scanner 1 option, (4) prepare the second scanner, connect it and turn it on, (5) start scanning with --scanner 2 option. Repeat step (4) and (5), each time incrementing the --scanner argument. 
-
-```
-usage: pyphe-scan-timecourse [-h] [--nscans NSCANS] [--interval INTERVAL]
-                             [--prefix PREFIX] [--postfix POSTFIX]
-                             [--fixture {som3_edge,som3}]
-                             [--resolution {150,300,600,900,1200}]
-                             [--scanner {1,2,3}] [--mode {Gray,Color}]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --nscans NSCANS       Number of time points to scan. This defaults to 100
-                        and the script can be terminated by Ctr+C when done.
-  --interval INTERVAL   Time in minutes between scans. Defaults to 20.
-  --prefix PREFIX       Name prefix for output files. The default is the
-                        current date YYYYMMDD.
-  --postfix POSTFIX     Name postfix for output files. Defaults to empty
-                        string.
-  --fixture {som3_edge,som3,som3-color}
-                        ID of the fixture you are using.
-  --resolution {150,300,600,900,1200}
-                        Resolution for scanning in dpi. Default is 600.
-  --scanner {1,2,3}     Which scanner to use. Scanners are not uniquely
-                        identified and may switch when turned off/unplugged.
-                        This option does not need to be set when only one
-                        scanner is connected.
-  --mode {Gray,Color}   Which color mode to use for scanning. Defaults to
-                        Gray.
-```
-
-
-### Pyphe-growthcurves
-This tool performs non-parametric analysis of growth curves. It was written specifically to analyse colony size timeseries data obtained with _pyphe-quantify_ _timeseries_.
-
-It is important that your csv with the growth data is in the right format. The file must contain one growth curve per column. The first column must be the timepoints and there must be a header row with unique identifiers for each curve. For example data and expected outputs, check out the files included in this Documentation folder. Sensible default parameters are set for all options but, depending on your data, you may wish to customise these, so check out the help section below. 
-
-```
-usage: pyphe-growthcurves [-h] --input INPUT [--fitrange FITRANGE]
-                          [--lag-method {abs,rel}]
-                          [--lag-threshold LAG_THRESHOLD]
-                          [--t0-fitrange T0_FITRANGE] [--plots]
-                          [--plot-ylim PLOT_YLIM]
-
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --input INPUT         Path to the growth curve file to analyse. This file
-                        contains one growth curve per column. The first column
-                        must be the timepoints and there must be a header row
-                        with unique identifiers for each curve.
-  --fitrange FITRANGE   Number of timepoint over which to fit linear
-                        regression. Defaults to 4. Please adjust this to the
-                        density of your timepoints and use higher values for
-                        more noisy data.
-  --lag-method {abs,rel}
-                        Method to use for determining lag. "abs" will measure
-                        time until the defined biomass threshold is crossed.
-                        "rel" will fist determine the inital biomass and
-                        measure the time until the biomass has passed this
-                        value times the threshold. Defaults to "rel".
-  --lag-threshold LAG_THRESHOLD
-                        Threshold to use for determining lag. With method
-                        "abs", this will measure time until the defined
-                        biomass threshold is crossed. With "rel" will fist
-                        determine the inital biomass and measure the time
-                        until the biomass has passed this value times the
-                        threshold. Defaults to 2.0, so with method "rel", this
-                        will measure the time taken for the first doubling.
-  --t0-fitrange T0_FITRANGE
-                        Specify the number of timepoint to use at the
-                        beginning of the growth curve to determine the initial
-                        biomass by averaging them. Defaults to 3.
-  --plots               Set this option (no argument required) to produce a
-                        plot of all growthcurves as pdf.
-  --plot-ylim PLOT_YLIM
-                        Specify the upper limit of the y-axis of growth curve
-                        plots. Useful if you want curves to be directly
-                        comparable. If not set, the axis of each curve is
-                        scaled to the data.
-```
-
-
-#### Interpreting results
-Pyphe-growthcurves will produce a csv file with extracted growth parameters. The maximum slope is determined by fitting all possible linear regressions in sliding windows of length n and chosing the one with the highest slope. The lag phase is determined as the first timepoint which exceeds a settable relative or absolute threshold. 
-
-| Parameter        | Explanation  |
-| ---------------- |---------------|
-|initial biomass|The average of the first n timepoints of the growth curve|
-|lag |  Lag phase |
-| max_slope| The maximum slope of the growth curve|
-| r2 | The R2 parameter of the linear regression that produced the highest maximum slope |
-|t_max | Time at which maximum growth slope is reached (center of the sliding window)|
-|y-intercept|Y-intercept of the regression which produced the maximum slope|
-|x-intercept|X-intercept of the regression which produced the maximum slope. This is interpreted as lag phase by some people|
-
-                            
-
-### Pyphe-quantify
-
-Pyphe quantify extracts colony parameters from images. In can operate in three distinct modes analysing colony sizes for each image individually (batch mode), analysing redness for each image individually (redness mode) or obtaining a growth curve from an image timeseries (timeseries mode).
-The --grid parameter is required define the position of colonies on the plate. You can either use automatic grid detection, one of our preconfigured positions if you are using the pp3 fixture or define your own (see the manual below). Images can be in any format (e.g. jpg, tiff, png). Images should be cropped closely to the colonies (this is important for good thresholding and automatic grid detection), i.e. not contain parts of the plate edges or surroundings. In batch and timecourse mode, pyphe-quantify assumes that images were acquired using transmission scanning, where colonies appear darker then the surrounding agar. If this is not the case and you took images by reflective scanning or with a camera, use --negate False. In batch and timecourse mode, images are epxected to be grayscale. If they are not, they will be converted (by simply summing all channels) and a warning will be thrown. 
-
-
-```
-usage: pyphe-quantify [-h] --grid GRID [--pattern PATTERN] [--t T] [--d D]
-                      [--s S] [--negate NEGATE] [--localThresh] [--convexhull]
-                      [--reportAll] [--reportFileNames]
-                      [--hardImageThreshold HARDIMAGETHRESHOLD]
-                      [--hardSizeThreshold HARDSIZETHRESHOLD] [--qc QC]
-                      [--calibrate CALIBRATE] [--timepoints TIMEPOINTS]
-                      [--out OUT]
-                      {batch,timecourse,redness}
-
-Welcome to pyphe-quantify, part of the pyphe toolbox. Written by
-stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
-Lab/pyphe
-
-positional arguments:
-  {batch,timecourse,redness}
-                        Pyphe-quantify can be run in three different modes. In
-                        batch mode, it quantifies colony sizes for all images
-                        matching the pattern individually. A separate results
-                        table and qc image is produced for each. Redness mode
-                        is similar except that the redness of each colony is
-                        quantified. In timecourse mode, all images matching
-                        the pattern are analysed jointly. The final image
-                        matching the pattern is used to create a mask of where
-                        the colonies are and this mask is then applied to all
-                        previous images in the timeseries. A single output
-                        table, where the timepoints are the rows and each
-                        individual colony is a row.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --grid GRID           This option is required (all others have defaults set)
-                        and specifies the grid in which the colonies are
-                        arranged. You can use automatic grid detection using
-                        one of the following parameters: auto_96, auto_384 or
-                        auto_1536. Automatic grid correction will not work if
-                        the colony grid is not aligned with the image borders.
-                        Images should contain only agar and colonies, avaoid
-                        having borders. It might fail or produce unexpected
-                        results if there are whole rows/columns missing. In
-                        those cases, it is easy to define hard-wired grid
-                        positions. If you are using the fixture provided with
-                        pyphe, we have preconfigured these for you. Depending
-                        on the pinning density, use pp3_96, pp3_384 or
-                        pp3_1536. Otherwise, the argument has to be in the
-                        form of 6 integer numbers separated by "-": <number of
-                        colony rows>-<number of colony columns>-<x-position of
-                        the top left colony>-<y-position of the top left
-                        colony>-<x-position of the bottom right
-                        colony>-<y-position of the bottom right colony>.
-                        Positions must be integers and are the distance in
-                        number of pixels from the image origin in each
-                        dimension (x is width dimension, y is height
-                        dimension). The image origin is, in line with scikit-
-                        image, in the top left corner. Pixel positions are
-                        easily determined using programs such as Microsoft
-                        Paint, by simply hovering the mouse over a position.
-  --pattern PATTERN     Pattern describing files to analyse. This follows
-                        standard unix convention and can be used to specify
-                        subfolders in which to look for images
-                        (<subfolder>/*.jpg) or the image format (*.tiff,
-                        *.png, etc.). By default, all jpg images in the
-                        working directory are analysed.
-  --t T                 By default the intensity threshold to distinguish
-                        colonies from the background is determined by the Otsu
-                        method. The determined value will be multiplied by
-                        this argument to give the final threshold. Useful for
-                        easily fine-tuning colony detection.
-  --d D                 The distance between two grid positions will be
-                        divided by this number to compute the maximum distance
-                        a putative colony can be away from its reference grid
-                        position. Decreasing this number towards 2 makes
-                        colony-to-grid-matching more permissive (might help
-                        when some of your plates are at a slight angle or out
-                        of position).
-  --s S                 Detected putative colonies will be filtered by size
-                        and small components (usually image noise) will be
-                        excluded. The default threshold is the image
-                        area*0.00005 and is therefore independent of scanning
-                        resolution. This default is then multiplied by this
-                        argument to give the final threshold. Useful for when
-                        colonies have unusual sizes.
-  --negate NEGATE       In images acquired by transmission scanning, the
-                        colonies are darker than the background. Before
-                        thresholding, the image needs to be inverted/negated.
-                        Defaults to True in timecourse and batch mode, ignored
-                        in redness mode.
-  --localThresh         Use local thresholding in batch and timecourse mode.
-                        This can help when image brightness is very uneven.
-                        Ignored in redness mode where local thresholding is
-                        always applied.
-  --convexhull          Apply convex hull transformation to identified
-                        colonies to fill holes. Useful when working with spots
-                        rather than colonies. Ignored in redness mode.
-                        WARNING: Using this options results in much longer
-                        analysis times.
-  --reportAll           Sometimes, two putative colonies are identified that
-                        are within the distance threshold of a grid position.
-                        By default, only the closest colony is reported. This
-                        can be changed by setting this option (without
-                        parameter). This option allows pyphe quantify to be
-                        used even if colonies are not arrayed in a regular
-                        grid (you still need to provide a grid parameter
-                        though that spans the colonies you are interested i).
-  --reportFileNames     Only for timecourse mode, otherwise ignored. Use
-                        filenames as index for output table instead of
-                        timepoints. Useful when the ordering of timepoints is
-                        not the same as returned by the pattern. Setting this
-                        option overrides the --timepoints argument.
-  --hardImageThreshold HARDIMAGETHRESHOLD
-                        Allows a hard (fixed) intensity threshold in the range
-                        [0,1] to be used instead of Otsu thresholding. Images
-                        intensities are re-scaled to [0,1] before
-                        thresholding. Ignored in timecourse mode.
-  --hardSizeThreshold HARDSIZETHRESHOLD
-                        Allows a hard (fixed) size threshold [number of
-                        pixels] to be used for filtering small colonies.
-  --qc QC               Directory to save qc images in. Defaults to
-                        "qc_images".
-  --calibrate CALIBRATE
-                        Transform background subtracted intensity values by
-                        this function. Function needs to be a single term with
-                        x as the variable and that is valid python code. E.g.
-                        use "2*x**2+1" to square each pixels intensity,
-                        multiply by two and add 1. Defaults to "x", i.e. use
-                        of no calibration. Used only in timecourse mode.
-  --timepoints TIMEPOINTS
-                        In timecourse mode only. Path to a file that specifies
-                        the timepoints of all images in the timeseries. This
-                        is usually the timepoints.txt file created by pyphe-
-                        scan-timecourse. It must contain one entry per line
-                        and have the same number of lines as number of images.
-  --out OUT             Directory to save output files in. Defaults to
-                        "pyphe_quant".
-```
-
-
-
-### Pyphe-analyse
-_Pyphe-analyse_ is a tool for spatial normalisation and data aggregation across many plates. It implements a grid normalisation based on the concept proposed by [Zackrisson et al. 2016](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5015956/) and row/column median normalisation. Please see our paper and the protocol in it to find out more. _Pyphe-analyse_ can be run from the command line, with options below, or using the graphical user interface by running _pyphe-analyse-gui_.
-
-
-```
-usage: pyphe-analyse.txt [-h] --edt EDT --format
-                         {gitter,pyphe-redness,pyphe-growthcurves} [--out OUT]
-                         [--load_layouts]
-                         [--gridnorm {standard384,standard1536}]
-                         [--extrapolate_corners] [--rcmedian] [--check CHECK]
-                         [--qc_plots QC_PLOTS]
-
-Welcome to pyphe-analyse, part of the pyphe toolbox. Written by
-stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
-Lab/pyphe
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --edt EDT             Path to the Experimental Design Table (EDT) listing
-                        all plates of the experiment. The table must be in csv
-                        format, the first column must contain unique plate IDs
-                        and there must be a column named 'Data_path' that
-                        contains abolute or relative file paths to each
-                        plate's data file. A 'Layout_path' column can be
-                        included, see below. Any additional columns included
-                        in this file will bestored in each plate's meta-data
-                        and included in the final data output.
-  --format {gitter,pyphe-redness,pyphe-growthcurves}
-                        Type of inout data.
-  --out OUT             Specifies the path where to save the output data
-                        result. By default, the data report is saved in the
-                        working directory as "pyphe-analyse_data_report.csv"
-                        and will overwrite the file if it exists.
-  --load_layouts        Set this option (without parameters) to load layouts
-                        (requires Layout_path column in the EDT).
-  --gridnorm {standard384,standard1536}
-                        Perform reference grid normalisation. Standard384
-                        refers to plates which are in 384 (16x24) format with
-                        the reference grid in 96 format in the top left
-                        corner. Standard1536 refers to plates in 1536 format
-                        (32x48( with two 96 reference grids in the top left
-                        and bottom right corners.
-  --extrapolate_corners
-                        If working in standard1536 format, set this option to
-                        extrapolate the reference grid in the bottom left and
-                        top right corner. A linear regression will be trained
-                        across all top left and bottom right corners on plates
-                        in the experiment to predict hypothetical grid colony
-                        sizes in the other two corners.
-  --rcmedian            Perform row/column median normalisation. If --gridnorm
-                        will be performed first if both parameters are set.
-  --check CHECK         Check colony sizes after normalisation for negative
-                        and infinite colony sizes *(normalisation artefacts),
-                        throw a warning and set to NA.
-  --qc_plots QC_PLOTS   Specify a folder in which to save qc plots for each
-                        plate.
-
-```
-
-
-### Pyphe-interpret
-
-Pyphe-interpret reports summary statistics and tests for differential fitness using t-tests. It is flexible and can in theory be used with any dataset in tidy format.
-
-```
-usage: pyphe-interpret [-h] --ld LD [--out OUT] --grouping_column
-                       GROUPING_COLUMN --axis_column AXIS_COLUMN
-                       [--values_column VALUES_COLUMN] --control CONTROL
-                       [--ld_encoding LD_ENCODING] [--circularity CIRCULARITY]
-                       [--set_missing_na]
-
-Welcome to pyphe-interpret, part of the pyphe toolbox. Written by
-stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
-Lab/pyphe. Pyphe-interpret calculates summary statistics and p-values from the
-data reports generated by pyphe-analyse. For this, specifiying your column
-names correctly is crucial. Let us assume you have measured many strains in
-many conditions. Now you would like to know for each strain in each condition
-(for each condition-strain pair) if it is "significant". There are essentially
-two ways of doing this, asking different biological questions. (1) Check for
-each condition separately (--grouping_column <condition_column>) if there is a
-significant difference in means between a mutant strain and a control strain
-(--axis_column <strain_id_column>). Or (2) Check for each strain separately
-(--grouping_column <strain_id_column>) if there is a significant difference in
-the means of the strain in the assay condition versus the control condition
-(--axis_column <condition_column>). The second option tests for condition-
-specific growth effects (i.e. is does not return significant results if a
-strain is always faster or always slower growing than the grid strain). In
-both cases you need to specify the control against which to test using
---control and this has to be a value that appears in the axis column. You
-should define the dependent variable of the t-test using --values_column. FDR
-correction with the Benjamini-Hochberg method will be applied on each level
-set of the grouping_column separately, ie for case (1) p-values will be
-corrected across each strain separately, ie more conditions means more
-stringent correction, and for case (2) p-values will be corrected for each
-condition separately, ie more strains means mpre stringent correction.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --ld LD               Path to the Data Report Table produced by pyphe-
-                        analyse.
-  --out OUT             Specifies the path where to save the output data
-                        result. By default, a table with all replicates will
-                        be saved as pyphe-interpret-report_reps.csv and the
-                        statistic table will be saved as pyphe-interpret-
-                        report_summaryStats.csv in the current working
-                        directory. Existing files will be overwritten.
-  --grouping_column GROUPING_COLUMN
-                        Name of the column in the data report to use for
-                        forming groups on which to perform independent sets of
-                        t-tests.
-  --axis_column AXIS_COLUMN
-                        Name of the column in the data report to repeat
-                        t-tests along within each group. Levels in this column
-                        will be the explanatory/independent variable used for
-                        t-tests.
-  --values_column VALUES_COLUMN
-                        Name of the column in the data report to use as
-                        fitness values. This will be the dependent variable
-                        for t-tests. Defaults to "Colony_size_corr_checked".
-  --control CONTROL     Name of the control to compare against. This must be a
-                        value found in the axis column.
-  --ld_encoding LD_ENCODING
-                        Encoding of the data report table to be passed to
-                        pandas.read_csv().
-  --circularity CIRCULARITY
-                        Exclude colonies from the analysis with a circularity
-                        below the one specified. A circularity of 1
-                        corresponds to a perfect circle. We recommend a
-                        threshold around 0.85.
-  --set_missing_na      Set 0-sized colonies to NA. This is recommended if you
-                        expect no missing colonies in your data, which means
-                        these are probably due to pinning errors.
-```
-
-
-
+Metadata-Version: 2.1
+Name: pyphe
+Version: 0.982
+Summary: Python toolbox for phenotype analysis of arrayed microbial colonies
+Home-page: https://github.com/Bahler-Lab/pyphe
+Author: Stephan Kamrad
+Author-email: stephan.kamrad@gmail.com
+License: MIT
+Description: ![pyphe logo](https://github.com/Bahler-Lab/pyphe/blob/master/icons/toolbox-72dpi_white.png)
+        
+        # Welcome to the pyphe toolbox
+        A python toolbox for phenotype analysis of arrayed microbial colonies written by Stephan Kamrad (stephan.kamrad at crick.ac.uk).
+        
+        For a quick overview, please see our [10 minute video tutorial](https://www.youtube.com/watch?v=lQ3lXIdhA1c&t=5s).
+        
+        For a more detailed protocol, including growth curves and viability assays, please see our [protocol preprint](https://www.researchsquare.com/article/rs-401914/v1).
+        
+        For more background information, please see our [_eLife_ paper](https://elifesciences.org/articles/55160).
+        
+        Please cite as:
+        > Kamrad, S., Rodríguez-López, M., Cotobal, C., Correia-Melo, C., Ralser M., Bähler J. (2020). Pyphe, a python toolbox for assessing microbial growth and cell viability in high-throughput colony screens. eLife 9:e55160
+        
+        ## Installation
+        1. Most tools are cross-platform compatible but scanning will only work on a Linux OS. The scanners need to be accessible by [SANE](http://www.sane-project.org/) and [ImageMagick](https://imagemagick.org/) needs to be installed and accessible from the command line.
+        2. Pyphe requires Python 3 and a few common packages, available through the [anaconda distribution](https://www.anaconda.com/distribution/).
+        3. Install pyphe by running 'pip install pyphe' in your terminal.
+        4. Open a new terminal and try and run 'pyphe-quantify -h' which should show the help page of one of pyphe's command line tools. On Windows, make sure you are using the Anaconda Prompt, not the Anaconda Powershell Prompt.
+        
+        
+        ## Overview
+        A typical fitness screen with pyphe will involve:
+        1. Image acquisition with [_pyphe-scan_](#pyphe-scan), or [_pyphe-scan-timecourse_](#pyphe-scan-timecourse)
+        2. Quantification of colony properties from images using [_pyphe-quantify_](#pyphe-quantify). In the case of growth curves, parameters are additionally extracted with [_pyphe-growthcurves_](#pyphe-growthcurves).
+        3. Normalisation and data aggregation using [_pyphe-analyse_](#pyphe-analyse).
+        4. Statistics and hit calling using [_pyphe-interpret_](#pyphe-interpret)
+        Please see our paper for a detailed protocol and explanations of the algorithms.
+        
+        
+        ## Support
+        Please check the manuals below carefully, they are also available in the terminal by running the command with the -h option only. If things are still not working, please email me (stephan.kamrad@gmail.com) and I will try and help. If you think you have discovered a bug, or would like to request a new feature, please raise an issue on www.github.com/Bahler-Lab/pyphe.
+        
+        If you get an error like this, make sure you are not using the Anaconda Powershell Prompt:
+        ```python: can't open file 'C:\Users\user1\Anaconda3\Scripts"C:\Users\user1\Anaconda3\Scripts\pyphe-quantify.bat  -h ': [Errno 22] Invalid argument```
+        
+        ## Manual
+        
+        All pyphe tools have a similar command line interface, based on the python argparse package. Generally, parameters are set using --<parameter_name> optionally followed by a value. All _pyphe_ tools can be used with relative file paths so make sure to navigate to the correct working directory before running a _pyphe_ command.
+        
+         
+        ### Pyphe-scan
+        This tools allows you to take consecutive scans of sets of plates, which are then automatically cropped, rotated and named in in a continuos filename scheme of your choice. 
+        
+        #### Prerequisites
+        1. This tool will only run on Linux operating systems and uses the SANE library for image acquisition.
+        
+        2. Make sure your scanner is installed correctly and you can acquire images using the scanimage command. The Gray mode will only work on Epson V800 and V850 scanners (potentially the V700 and V750 model as well) and the TPU8x10 transmission scanning source must be enabled. This should work by default if you are using the V800/850 model and a recent Linux OS. Otherwise, there is excellent documentation available from Zackrisson et al. and the [scanomatics pipeline](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5015956/) for how to make this work using a hacked SANE driver. Please see the instructions in their [wiki](https://github.com/Scan-o-Matic/scanomatic/wiki/Installing-scanners).
+        
+        2. Make sure [ImageMagick](https://imagemagick.org/index.php) is installed and the 'convert' tool can be called from the command line.
+        
+        3. If the Pyphe toolbox has been installed correctly, you should be able to run _pyphe-scan_ in your terminal. 
+        
+        4. With a laser cutter, make a fixture to hold your plates in place. We provide an svg file with the cutting shape in the Documentation directory. Use tape to hold your fixture into place, it should be pushed against the back of the scanner (where the cables are) with the top of the plates facing left. Pyphe-scan and pyphe-quantify come pre-configured for using the provided fixture on an Epson V800/V850 scanner but it is easy to add your own fixture and cropping settings. If you want to use your own fixture, see below of how to add the geometry information to pyphe-scan. 
+        
+        #### Scanning plate batches
+        
+        1. Open the file manager and navigate to the folder in which you want to save your images. The script will create a sub-folder that begins with the current date to save all your images. 
+        
+        2. Right click and select 'Open in Terminal'
+        
+        3. Run scanplates with the options as detaild below. 
+        
+        ```
+        usage: pyphe-scan [-h] [--nplates NPLATES] [--start START] [--prefix PREFIX]
+                          [--postfix POSTFIX] [--fixture {som3_edge,som3}]
+                          [--resolution {150,300,600,900,1200}] [--scanner {1,2,3}]
+                          [--mode {Gray,Color}]
+        
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --nplates NPLATES     Number of plates to scan. This defaults to 100 and the
+                                script can be terminated by Ctr+C when done.
+          --start START         Where to start numbering from. Defaults to 1.
+          --prefix PREFIX       Name prefix for output files. The default is the
+                                current date YYYYMMDD.
+          --postfix POSTFIX     Name postfix for output files. Defaults to empty
+                                string.
+          --fixture {som3_edge,som3,som3-color}
+                                ID of the fixture you are using.
+          --resolution {150,300,600,900,1200}
+                                Resolution for scanning in dpi. Default is 600.
+          --scanner {1,2,3}     Which scanner to use. Scanners are not uniquely
+                                identified and may switch when turned off/unplugged.
+                                This option does not need to be set when only one
+                                scanner is connected.
+          --mode {Gray,Color}   Which color mode to use for scanning. Defaults to
+                                Gray.
+        ```
+        
+        All arguments except the fixture have default values and are optional. A folder prefix_postfix will be created in your current directory and the program will abort if a folder with this name already exists. 
+        
+        
+        
+        ### Pyphe-scan-timecourse
+        
+        This tool acquires image timeseries by scanning in fixed time intervals. For each position in the fixture, a folder is created. Image names contain number of scan. Other options for this tool are similar to [_pyphe-scan_](#pyphe-scan). More than one scanner can be connected and used at the same time. Scanner numbers are defined by the order in which they are connected to the computer. Proceed as follows: (1) disconnect all scanners, (2) prepare the first scanner with plates, connect it and turn it on. (3) start scanning with --scanner 1 option, (4) prepare the second scanner, connect it and turn it on, (5) start scanning with --scanner 2 option. Repeat step (4) and (5), each time incrementing the --scanner argument. 
+        
+        ```
+        usage: pyphe-scan-timecourse [-h] [--nscans NSCANS] [--interval INTERVAL]
+                                     [--prefix PREFIX] [--postfix POSTFIX]
+                                     [--fixture {som3_edge,som3}]
+                                     [--resolution {150,300,600,900,1200}]
+                                     [--scanner {1,2,3}] [--mode {Gray,Color}]
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --nscans NSCANS       Number of time points to scan. This defaults to 100
+                                and the script can be terminated by Ctr+C when done.
+          --interval INTERVAL   Time in minutes between scans. Defaults to 20.
+          --prefix PREFIX       Name prefix for output files. The default is the
+                                current date YYYYMMDD.
+          --postfix POSTFIX     Name postfix for output files. Defaults to empty
+                                string.
+          --fixture {som3_edge,som3,som3-color}
+                                ID of the fixture you are using.
+          --resolution {150,300,600,900,1200}
+                                Resolution for scanning in dpi. Default is 600.
+          --scanner {1,2,3}     Which scanner to use. Scanners are not uniquely
+                                identified and may switch when turned off/unplugged.
+                                This option does not need to be set when only one
+                                scanner is connected.
+          --mode {Gray,Color}   Which color mode to use for scanning. Defaults to
+                                Gray.
+        ```
+        
+        
+        ### Pyphe-growthcurves
+        This tool performs non-parametric analysis of growth curves. It was written specifically to analyse colony size timeseries data obtained with _pyphe-quantify_ _timeseries_.
+        
+        It is important that your csv with the growth data is in the right format. The file must contain one growth curve per column. The first column must be the timepoints and there must be a header row with unique identifiers for each curve. For example data and expected outputs, check out the files included in this Documentation folder. Sensible default parameters are set for all options but, depending on your data, you may wish to customise these, so check out the help section below. 
+        
+        ```
+        usage: pyphe-growthcurves [-h] --input INPUT [--fitrange FITRANGE]
+                                  [--lag-method {abs,rel}]
+                                  [--lag-threshold LAG_THRESHOLD]
+                                  [--t0-fitrange T0_FITRANGE] [--plots]
+                                  [--plot-ylim PLOT_YLIM]
+        
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --input INPUT         Path to the growth curve file to analyse. This file
+                                contains one growth curve per column. The first column
+                                must be the timepoints and there must be a header row
+                                with unique identifiers for each curve.
+          --fitrange FITRANGE   Number of timepoint over which to fit linear
+                                regression. Defaults to 4. Please adjust this to the
+                                density of your timepoints and use higher values for
+                                more noisy data.
+          --lag-method {abs,rel}
+                                Method to use for determining lag. "abs" will measure
+                                time until the defined biomass threshold is crossed.
+                                "rel" will fist determine the inital biomass and
+                                measure the time until the biomass has passed this
+                                value times the threshold. Defaults to "rel".
+          --lag-threshold LAG_THRESHOLD
+                                Threshold to use for determining lag. With method
+                                "abs", this will measure time until the defined
+                                biomass threshold is crossed. With "rel" will fist
+                                determine the inital biomass and measure the time
+                                until the biomass has passed this value times the
+                                threshold. Defaults to 2.0, so with method "rel", this
+                                will measure the time taken for the first doubling.
+          --t0-fitrange T0_FITRANGE
+                                Specify the number of timepoint to use at the
+                                beginning of the growth curve to determine the initial
+                                biomass by averaging them. Defaults to 3.
+          --plots               Set this option (no argument required) to produce a
+                                plot of all growthcurves as pdf.
+          --plot-ylim PLOT_YLIM
+                                Specify the upper limit of the y-axis of growth curve
+                                plots. Useful if you want curves to be directly
+                                comparable. If not set, the axis of each curve is
+                                scaled to the data.
+        ```
+        
+        
+        #### Interpreting results
+        Pyphe-growthcurves will produce a csv file with extracted growth parameters. The maximum slope is determined by fitting all possible linear regressions in sliding windows of length n and chosing the one with the highest slope. The lag phase is determined as the first timepoint which exceeds a settable relative or absolute threshold. 
+        
+        | Parameter        | Explanation  |
+        | ---------------- |---------------|
+        |initial biomass|The average of the first n timepoints of the growth curve|
+        |lag |  Lag phase |
+        | max_slope| The maximum slope of the growth curve|
+        | r2 | The R2 parameter of the linear regression that produced the highest maximum slope |
+        |t_max | Time at which maximum growth slope is reached (center of the sliding window)|
+        |y-intercept|Y-intercept of the regression which produced the maximum slope|
+        |x-intercept|X-intercept of the regression which produced the maximum slope. This is interpreted as lag phase by some people|
+        
+                                    
+        
+        ### Pyphe-quantify
+        
+        Pyphe quantify extracts colony parameters from images. In can operate in three distinct modes analysing colony sizes for each image individually (batch mode), analysing redness for each image individually (redness mode) or obtaining a growth curve from an image timeseries (timeseries mode).
+        The --grid parameter is required define the position of colonies on the plate. You can either use automatic grid detection, one of our preconfigured positions if you are using the pp3 fixture or define your own (see the manual below). Images can be in any format (e.g. jpg, tiff, png). Images should be cropped closely to the colonies (this is important for good thresholding and automatic grid detection), i.e. not contain parts of the plate edges or surroundings. In batch and timecourse mode, pyphe-quantify assumes that images were acquired using transmission scanning, where colonies appear darker then the surrounding agar. If this is not the case and you took images by reflective scanning or with a camera, use --negate False. In batch and timecourse mode, images are epxected to be grayscale. If they are not, they will be converted (by simply summing all channels) and a warning will be thrown. 
+        
+        
+        ```
+        usage: pyphe-quantify [-h] --grid GRID [--pattern PATTERN] [--t T] [--d D]
+                              [--s S] [--negate NEGATE] [--localThresh] [--convexhull]
+                              [--reportAll] [--reportFileNames]
+                              [--hardImageThreshold HARDIMAGETHRESHOLD]
+                              [--hardSizeThreshold HARDSIZETHRESHOLD] [--qc QC]
+                              [--calibrate CALIBRATE] [--timepoints TIMEPOINTS]
+                              [--out OUT]
+                              {batch,timecourse,redness}
+        
+        Welcome to pyphe-quantify, part of the pyphe toolbox. Written by
+        stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
+        Lab/pyphe
+        
+        positional arguments:
+          {batch,timecourse,redness}
+                                Pyphe-quantify can be run in three different modes. In
+                                batch mode, it quantifies colony sizes for all images
+                                matching the pattern individually. A separate results
+                                table and qc image is produced for each. Redness mode
+                                is similar except that the redness of each colony is
+                                quantified. In timecourse mode, all images matching
+                                the pattern are analysed jointly. The final image
+                                matching the pattern is used to create a mask of where
+                                the colonies are and this mask is then applied to all
+                                previous images in the timeseries. A single output
+                                table, where the timepoints are the rows and each
+                                individual colony is a row.
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --grid GRID           This option is required (all others have defaults set)
+                                and specifies the grid in which the colonies are
+                                arranged. You can use automatic grid detection using
+                                one of the following parameters: auto_96, auto_384 or
+                                auto_1536. Automatic grid correction will not work if
+                                the colony grid is not aligned with the image borders.
+                                Images should contain only agar and colonies, avaoid
+                                having borders. It might fail or produce unexpected
+                                results if there are whole rows/columns missing. In
+                                those cases, it is easy to define hard-wired grid
+                                positions. If you are using the fixture provided with
+                                pyphe, we have preconfigured these for you. Depending
+                                on the pinning density, use pp3_96, pp3_384 or
+                                pp3_1536. Otherwise, the argument has to be in the
+                                form of 6 integer numbers separated by "-": <number of
+                                colony rows>-<number of colony columns>-<x-position of
+                                the top left colony>-<y-position of the top left
+                                colony>-<x-position of the bottom right
+                                colony>-<y-position of the bottom right colony>.
+                                Positions must be integers and are the distance in
+                                number of pixels from the image origin in each
+                                dimension (x is width dimension, y is height
+                                dimension). The image origin is, in line with scikit-
+                                image, in the top left corner. Pixel positions are
+                                easily determined using programs such as Microsoft
+                                Paint, by simply hovering the mouse over a position.
+          --pattern PATTERN     Pattern describing files to analyse. This follows
+                                standard unix convention and can be used to specify
+                                subfolders in which to look for images
+                                (<subfolder>/*.jpg) or the image format (*.tiff,
+                                *.png, etc.). By default, all jpg images in the
+                                working directory are analysed.
+          --t T                 By default the intensity threshold to distinguish
+                                colonies from the background is determined by the Otsu
+                                method. The determined value will be multiplied by
+                                this argument to give the final threshold. Useful for
+                                easily fine-tuning colony detection.
+          --d D                 The distance between two grid positions will be
+                                divided by this number to compute the maximum distance
+                                a putative colony can be away from its reference grid
+                                position. Decreasing this number towards 2 makes
+                                colony-to-grid-matching more permissive (might help
+                                when some of your plates are at a slight angle or out
+                                of position).
+          --s S                 Detected putative colonies will be filtered by size
+                                and small components (usually image noise) will be
+                                excluded. The default threshold is the image
+                                area*0.00005 and is therefore independent of scanning
+                                resolution. This default is then multiplied by this
+                                argument to give the final threshold. Useful for when
+                                colonies have unusual sizes.
+          --negate NEGATE       In images acquired by transmission scanning, the
+                                colonies are darker than the background. Before
+                                thresholding, the image needs to be inverted/negated.
+                                Defaults to True in timecourse and batch mode, ignored
+                                in redness mode.
+          --localThresh         Use local thresholding in batch and timecourse mode.
+                                This can help when image brightness is very uneven.
+                                Ignored in redness mode where local thresholding is
+                                always applied.
+          --convexhull          Apply convex hull transformation to identified
+                                colonies to fill holes. Useful when working with spots
+                                rather than colonies. Ignored in redness mode.
+                                WARNING: Using this options results in much longer
+                                analysis times.
+          --reportAll           Sometimes, two putative colonies are identified that
+                                are within the distance threshold of a grid position.
+                                By default, only the closest colony is reported. This
+                                can be changed by setting this option (without
+                                parameter). This option allows pyphe quantify to be
+                                used even if colonies are not arrayed in a regular
+                                grid (you still need to provide a grid parameter
+                                though that spans the colonies you are interested i).
+          --reportFileNames     Only for timecourse mode, otherwise ignored. Use
+                                filenames as index for output table instead of
+                                timepoints. Useful when the ordering of timepoints is
+                                not the same as returned by the pattern. Setting this
+                                option overrides the --timepoints argument.
+          --hardImageThreshold HARDIMAGETHRESHOLD
+                                Allows a hard (fixed) intensity threshold in the range
+                                [0,1] to be used instead of Otsu thresholding. Images
+                                intensities are re-scaled to [0,1] before
+                                thresholding. Ignored in timecourse mode.
+          --hardSizeThreshold HARDSIZETHRESHOLD
+                                Allows a hard (fixed) size threshold [number of
+                                pixels] to be used for filtering small colonies.
+          --qc QC               Directory to save qc images in. Defaults to
+                                "qc_images".
+          --calibrate CALIBRATE
+                                Transform background subtracted intensity values by
+                                this function. Function needs to be a single term with
+                                x as the variable and that is valid python code. E.g.
+                                use "2*x**2+1" to square each pixels intensity,
+                                multiply by two and add 1. Defaults to "x", i.e. use
+                                of no calibration. Used only in timecourse mode.
+          --timepoints TIMEPOINTS
+                                In timecourse mode only. Path to a file that specifies
+                                the timepoints of all images in the timeseries. This
+                                is usually the timepoints.txt file created by pyphe-
+                                scan-timecourse. It must contain one entry per line
+                                and have the same number of lines as number of images.
+          --out OUT             Directory to save output files in. Defaults to
+                                "pyphe_quant".
+        ```
+        
+        
+        
+        ### Pyphe-analyse
+        _Pyphe-analyse_ is a tool for spatial normalisation and data aggregation across many plates. It implements a grid normalisation based on the concept proposed by [Zackrisson et al. 2016](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5015956/) and row/column median normalisation. Please see our paper and the protocol in it to find out more. _Pyphe-analyse_ can be run from the command line, with options below, or using the graphical user interface by running _pyphe-analyse-gui_.
+        
+        
+        ```
+        usage: pyphe-analyse.txt [-h] --edt EDT --format
+                                 {gitter,pyphe-redness,pyphe-growthcurves} [--out OUT]
+                                 [--load_layouts]
+                                 [--gridnorm {standard384,standard1536}]
+                                 [--extrapolate_corners] [--rcmedian] [--check CHECK]
+                                 [--qc_plots QC_PLOTS]
+        
+        Welcome to pyphe-analyse, part of the pyphe toolbox. Written by
+        stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
+        Lab/pyphe
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --edt EDT             Path to the Experimental Design Table (EDT) listing
+                                all plates of the experiment. The table must be in csv
+                                format, the first column must contain unique plate IDs
+                                and there must be a column named 'Data_path' that
+                                contains abolute or relative file paths to each
+                                plate's data file. A 'Layout_path' column can be
+                                included, see below. Any additional columns included
+                                in this file will bestored in each plate's meta-data
+                                and included in the final data output.
+          --format {gitter,pyphe-redness,pyphe-growthcurves}
+                                Type of inout data.
+          --out OUT             Specifies the path where to save the output data
+                                result. By default, the data report is saved in the
+                                working directory as "pyphe-analyse_data_report.csv"
+                                and will overwrite the file if it exists.
+          --load_layouts        Set this option (without parameters) to load layouts
+                                (requires Layout_path column in the EDT).
+          --gridnorm {standard384,standard1536,1536with384grid}
+                                Perform reference grid normalisation. Standard384
+                                refers to plates which are in 384 (16x24) format with
+                                the reference grid in 96 format in the top left
+                                corner. Standard1536 refers to plates in 1536 format
+                                (32x48( with two 96 reference grids in the top left
+                                and bottom right corners. 1536with384grid refers to
+                                plates in 1536 format with a 384 reference grid in
+                                the top left position.
+          --extrapolate_corners
+                                If working in standard1536 format, set this option to
+                                extrapolate the reference grid in the bottom left and
+                                top right corner. A linear regression will be trained
+                                across all top left and bottom right corners on plates
+                                in the experiment to predict hypothetical grid colony
+                                sizes in the other two corners.
+          --rcmedian            Perform row/column median normalisation. If --gridnorm
+                                will be performed first if both parameters are set.
+          --check CHECK         Check colony sizes after normalisation for negative
+                                and infinite colony sizes *(normalisation artefacts),
+                                throw a warning and set to NA.
+          --qc_plots QC_PLOTS   Specify a folder in which to save qc plots for each
+                                plate.
+        
+        ```
+        
+        
+        ### Pyphe-interpret
+        
+        Pyphe-interpret reports summary statistics and tests for differential fitness using t-tests. It is flexible and can in theory be used with any dataset in tidy format.
+        
+        ```
+        usage: pyphe-interpret [-h] --ld LD [--out OUT] --grouping_column
+                               GROUPING_COLUMN --axis_column AXIS_COLUMN
+                               [--values_column VALUES_COLUMN] --control CONTROL
+                               [--ld_encoding LD_ENCODING] [--circularity CIRCULARITY]
+                               [--set_missing_na]
+        
+        Welcome to pyphe-interpret, part of the pyphe toolbox. Written by
+        stephan.kamrad@crick.ac.uk and maintained at https://github.com/Bahler-
+        Lab/pyphe. Pyphe-interpret calculates summary statistics and p-values from the
+        data reports generated by pyphe-analyse. For this, specifiying your column
+        names correctly is crucial. Let us assume you have measured many strains in
+        many conditions. Now you would like to know for each strain in each condition
+        (for each condition-strain pair) if it is "significant". There are essentially
+        two ways of doing this, asking different biological questions. (1) Check for
+        each condition separately (--grouping_column <condition_column>) if there is a
+        significant difference in means between a mutant strain and a control strain
+        (--axis_column <strain_id_column>). Or (2) Check for each strain separately
+        (--grouping_column <strain_id_column>) if there is a significant difference in
+        the means of the strain in the assay condition versus the control condition
+        (--axis_column <condition_column>). The second option tests for condition-
+        specific growth effects (i.e. is does not return significant results if a
+        strain is always faster or always slower growing than the grid strain). In
+        both cases you need to specify the control against which to test using
+        --control and this has to be a value that appears in the axis column. You
+        should define the dependent variable of the t-test using --values_column. FDR
+        correction with the Benjamini-Hochberg method will be applied on each level
+        set of the grouping_column separately, ie for case (1) p-values will be
+        corrected across each strain separately, ie more conditions means more
+        stringent correction, and for case (2) p-values will be corrected for each
+        condition separately, ie more strains means mpre stringent correction.
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          --ld LD               Path to the Data Report Table produced by pyphe-
+                                analyse.
+          --out OUT             Specifies the path where to save the output data
+                                result. By default, a table with all replicates will
+                                be saved as pyphe-interpret-report_reps.csv and the
+                                statistic table will be saved as pyphe-interpret-
+                                report_summaryStats.csv in the current working
+                                directory. Existing files will be overwritten.
+          --grouping_column GROUPING_COLUMN
+                                Name of the column in the data report to use for
+                                forming groups on which to perform independent sets of
+                                t-tests.
+          --axis_column AXIS_COLUMN
+                                Name of the column in the data report to repeat
+                                t-tests along within each group. Levels in this column
+                                will be the explanatory/independent variable used for
+                                t-tests.
+          --values_column VALUES_COLUMN
+                                Name of the column in the data report to use as
+                                fitness values. This will be the dependent variable
+                                for t-tests. Defaults to "Colony_size_corr_checked".
+          --control CONTROL     Name of the control to compare against. This must be a
+                                value found in the axis column.
+          --ld_encoding LD_ENCODING
+                                Encoding of the data report table to be passed to
+                                pandas.read_csv().
+          --circularity CIRCULARITY
+                                Exclude colonies from the analysis with a circularity
+                                below the one specified. A circularity of 1
+                                corresponds to a perfect circle. We recommend a
+                                threshold around 0.85.
+          --set_missing_na      Set 0-sized colonies to NA. This is recommended if you
+                                expect no missing colonies in your data, which means
+                                these are probably due to pinning errors.
+        ```
+        
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
```

### Comparing `pyphe-0.981/setup.py` & `pyphe-0.982/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from setuptools import setup
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-    
-    
-setup(name='pyphe',
-      version='0.981',
-      description='Python toolbox for phenotype analysis of arrayed microbial colonies',
-      long_description=long_description,
-      long_description_content_type="text/markdown",
-      url='https://github.com/Bahler-Lab/pyphe',
-      author='Stephan Kamrad',
-      author_email='stephan.kamrad@crick.ac.uk',
-      license='MIT',
-      packages=['pyphe'],
-      scripts=['bin/pyphe-scan', 'bin/pyphe-scan-timecourse', 'bin/pyphe-growthcurves', 'bin/pyphe-analyse', 'bin/pyphe-quantify', 'bin/pyphe-interpret',
-      'bin/pyphe-analyse-gui',
-      'bin/pyphe-growthcurves.bat', 'bin/pyphe-analyse.bat', 'bin/pyphe-quantify.bat', 'bin/pyphe-interpret.bat',],
-      install_requires=[
-          'pandas',
-          'matplotlib',
-          'numpy',
-          'seaborn',
-          'scipy',
-          'scikit-image',
-          'scikit-learn'
-      ],
-      classifiers=[
-        "Development Status :: 4 - Beta", 
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        ],
-      python_requires='>=3.7')
+from setuptools import setup
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+    
+    
+setup(name='pyphe',
+      version='0.982',
+      description='Python toolbox for phenotype analysis of arrayed microbial colonies',
+      long_description=long_description,
+      long_description_content_type="text/markdown",
+      url='https://github.com/Bahler-Lab/pyphe',
+      author='Stephan Kamrad',
+      author_email='stephan.kamrad@gmail.com',
+      license='MIT',
+      packages=['pyphe'],
+      scripts=['bin/pyphe-scan', 'bin/pyphe-scan-timecourse', 'bin/pyphe-growthcurves', 'bin/pyphe-analyse', 'bin/pyphe-quantify', 'bin/pyphe-interpret',
+      'bin/pyphe-analyse-gui',
+      'bin/pyphe-growthcurves.bat', 'bin/pyphe-analyse.bat', 'bin/pyphe-quantify.bat', 'bin/pyphe-interpret.bat',],
+      install_requires=[
+          'pandas',
+          'matplotlib',
+          'numpy',
+          'seaborn',
+          'scipy',
+          'scikit-image',
+          'scikit-learn'
+      ],
+      classifiers=[
+        "Development Status :: 4 - Beta", 
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        ],
+      python_requires='>=3.7')
```

