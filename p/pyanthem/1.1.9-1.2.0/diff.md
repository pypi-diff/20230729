# Comparing `tmp/pyanthem-1.1.9.tar.gz` & `tmp/pyanthem-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanthem-1.1.9.tar", last modified: Fri Jun 17 16:19:41 2022, max compression
+gzip compressed data, was "pyanthem-1.2.0.tar", last modified: Sat Jul 29 20:50:11 2023, max compression
```

## Comparing `pyanthem-1.1.9.tar` & `pyanthem-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nicthib    (501) staff       (20)        0 2022-06-17 16:19:41.050736 pyanthem-1.1.9/
--rw-r--r--   0 nicthib    (501) staff       (20)     1073 2022-06-17 15:48:49.000000 pyanthem-1.1.9/LICENSE
--rw-r--r--   0 nicthib    (501) staff       (20)       29 2022-06-17 15:48:49.000000 pyanthem-1.1.9/MANIFEST.in
--rw-r--r--   0 nicthib    (501) staff       (20)     9676 2022-06-17 16:19:41.050545 pyanthem-1.1.9/PKG-INFO
--rw-r--r--   0 nicthib    (501) staff       (20)     9162 2022-06-17 15:48:49.000000 pyanthem-1.1.9/README.rst
-drwxr-xr-x   0 nicthib    (501) staff       (20)        0 2022-06-17 16:19:41.049584 pyanthem-1.1.9/pyanthem/
--rw-r--r--   0 nicthib    (501) staff       (20)       68 2022-06-17 15:48:49.000000 pyanthem-1.1.9/pyanthem/__init__.py
--rw-r--r--   0 nicthib    (501) staff       (20)      767 2022-06-17 15:48:49.000000 pyanthem-1.1.9/pyanthem/decompmp4.py
--rw-r--r--   0 nicthib    (501) staff       (20)     1527 2022-06-17 15:48:49.000000 pyanthem-1.1.9/pyanthem/obsolete.py
--rw-r--r--   0 nicthib    (501) staff       (20)    35039 2022-06-17 15:56:00.000000 pyanthem-1.1.9/pyanthem/pyanthem.py
--rw-r--r--   0 nicthib    (501) staff       (20)     1521 2022-06-17 15:48:49.000000 pyanthem-1.1.9/pyanthem/pyanthem_vars.py
-drwxr-xr-x   0 nicthib    (501) staff       (20)        0 2022-06-17 16:19:41.050345 pyanthem-1.1.9/pyanthem.egg-info/
--rw-r--r--   0 nicthib    (501) staff       (20)     9676 2022-06-17 16:19:40.000000 pyanthem-1.1.9/pyanthem.egg-info/PKG-INFO
--rw-r--r--   0 nicthib    (501) staff       (20)      309 2022-06-17 16:19:41.000000 pyanthem-1.1.9/pyanthem.egg-info/SOURCES.txt
--rw-r--r--   0 nicthib    (501) staff       (20)        1 2022-06-17 16:19:40.000000 pyanthem-1.1.9/pyanthem.egg-info/dependency_links.txt
--rw-r--r--   0 nicthib    (501) staff       (20)       93 2022-06-17 16:19:40.000000 pyanthem-1.1.9/pyanthem.egg-info/requires.txt
--rw-r--r--   0 nicthib    (501) staff       (20)        9 2022-06-17 16:19:40.000000 pyanthem-1.1.9/pyanthem.egg-info/top_level.txt
--rw-r--r--   0 nicthib    (501) staff       (20)       38 2022-06-17 16:19:41.050781 pyanthem-1.1.9/setup.cfg
--rw-r--r--   0 nicthib    (501) staff       (20)      909 2022-06-17 16:19:33.000000 pyanthem-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 20:50:11.887485 pyanthem-1.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-07-29 20:49:30.000000 pyanthem-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       31 2023-07-29 20:49:30.000000 pyanthem-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9996 2023-07-29 20:50:11.885486 pyanthem-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9502 2023-07-29 20:49:30.000000 pyanthem-1.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-29 20:50:11.671527 pyanthem-1.2.0/pyanthem/
+-rw-rw-rw-   0        0        0       69 2023-07-29 20:49:30.000000 pyanthem-1.2.0/pyanthem/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-07-29 20:49:30.000000 pyanthem-1.2.0/pyanthem/decompmp4.py
+-rw-rw-rw-   0        0        0     1566 2023-07-29 20:49:30.000000 pyanthem-1.2.0/pyanthem/obsolete.py
+-rw-rw-rw-   0        0        0    35897 2023-07-29 20:49:30.000000 pyanthem-1.2.0/pyanthem/pyanthem.py
+-rw-rw-rw-   0        0        0     1631 2023-07-29 20:49:30.000000 pyanthem-1.2.0/pyanthem/pyanthem_vars.py
+drwxrwxrwx   0        0        0        0 2023-07-29 20:50:11.882491 pyanthem-1.2.0/pyanthem.egg-info/
+-rw-rw-rw-   0        0        0     9996 2023-07-29 20:50:09.000000 pyanthem-1.2.0/pyanthem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-07-29 20:50:09.000000 pyanthem-1.2.0/pyanthem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 20:50:09.000000 pyanthem-1.2.0/pyanthem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-07-29 20:50:09.000000 pyanthem-1.2.0/pyanthem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-29 20:50:09.000000 pyanthem-1.2.0/pyanthem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 20:50:11.887485 pyanthem-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      964 2023-07-29 20:49:30.000000 pyanthem-1.2.0/setup.py
```

### Comparing `pyanthem-1.1.9/LICENSE` & `pyanthem-1.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
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
+Copyright (c) 2018 The Python Packaging Authority
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
 SOFTWARE.
```

### Comparing `pyanthem-1.1.9/PKG-INFO` & `pyanthem-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,220 +1,218 @@
-Metadata-Version: 2.1
-Name: pyanthem
-Version: 1.1.9
-Summary: pyanthem - an audiovisualization tool to make your data more interesting
-Home-page: https://github.com/nicthib/pyanthem
-Author: Nic Thibodeaux
-Author-email: dnt2111@columbia.edu
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7,!= 3.8.*
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-********************************************************************
-pyanthem: Transforming your datasets into a colorful, audible format
-********************************************************************
-
-Features:
-=========
-
-1) Converts three-dimensional datasets to visually pleasing, audible representations
-2) A variety of video and audio parameters
-3) In-place video and audio merge
-4) GUI and Command-line interface for maximum flexibility
-5) Example datasets to get you started
-6) Headache-free installation with an Anaconda environment
-
-Usage
-=====
-
-pyanthem was primarily developed to interpret matrix-decomposed functional imaging datasets - for example, a dataset **V** with shape :code:`[height,width,time]`, is decomposed into two matrixes: **W** with shape :code:`[height*width,n]`, and **H** with shape :code:`[n,time]` such that :code:`H x W = V`. Here, n represents the number of variables represented by the decomposition. There are various techniques used to decompose matrixes - two popular techniques include Non-negative Matrix Factorization (NMF), and Singular Value Decomposition (SVD).
-
-Here's a visual illustration of matrix decomposition - note that in this example, :code:`n=2`:
-
-.. image:: https://upload.wikimedia.org/wikipedia/commons/f/f9/NMF.png
-
-If you would prefer to keep things simple, you can skip matrix decomposition altogether and focus solely on converting raw data to audio - only working with the **H** matrix, where each row represents a variable and each column represents a time point.
-
-If this is too much information to digest, don't worry! Try the example below to get more familiar with what the data looks like, and how pyanthem transforms it.
-
-Requirements
-============
-
-*See installation guide below before proceeding!*
-
-`Python 3.7`_:
-   Currently, pyanthem is tested to work on Python 3.7. This will be updated as more versions are tested.
-
-FFmpeg_:
-   ffmpeg enables video creation and merging.
-
-FluidSynth_:
-   FluidSynth enables conversion of MIDI files to crisp, high quality sound files.
-   
-If you do have the above requirements installed, you can install pyanthem using pip: :code:`pip install pyanthem`
-
-Conda (optional, but highly recommended):
-   Conda enables simple and reliable package installation. Use Miniconda_ for a minimal installation, or Anaconda_ otherwise.
-
-.. _`Python 3.7`: https://www.python.org/downloads/release/python-378/
-.. _FFmpeg: https://ffmpeg.org/
-.. _FluidSynth: http://www.fluidsynth.org/
-.. _Miniconda: https://docs.conda.io/en/latest/miniconda.html
-.. _Anaconda: https://www.anaconda.com/products/individual
-
-Installation
-============
-Note: If you do not have working installations of the listed requirements (Python 3.7 + fluidsynth + ffmpeg), it is **strongly recommended** that you use Miniconda_/Anaconda_ for a straightforward installation process. If you do not have either, Miniconda is preferred as it is a faster install and takes up much less space than Anaconda.
-
-Using Miniconda/Anaconda:
--------------------------
-
-Create an environment and install the required packages::
-   
-   conda create -n pyanthem python=3.7 pip ffmpeg fluidsynth --channel conda-forge --channel nicthib
-
-Next, activate the environment::
-   
-   conda activate pyanthem
-
-Finally, install the pyanthem Python package using pip::
-   
-   pip install pyanthem
-
-Example datasets and Scripts
-----------------------------
-
-If you want to get familiar with the datasets that pyanthem uses and try some applications of pyanthem, clone this repository or download `here.`
-
-.. _`here`: https://github.com/nicthib/pyanthem/archive/master.zip
-
-Using pyanthem in a Jupyter Notebook
------------------------------------------------
-
-To access the pyanthem environment in a Jupyter notebook, first install ipykernel in your environment::
-   
-   conda install -c anaconda ipykernel
-
-After this, create the kernel::
-   
-   python -m ipykernel install --user --name=pyanthem
-
-Once in a notebook, switch to the pyanthem kernel by selecting :code:`Kernel > Change kernel > pyanthem`
-
-*Note: While the pyanthem kernel will now be available in any Jupyter notebook session, pyanthem will not function properly unless the Jupyter notebook is launched inside the pyanthem environment*.
-
-Example
-=======
-
-Using pyanthem in GUI mode
---------------------------
-
-First, import pyanthem and begin a pyanthem session:
-
-.. code-block:: python
-   
-   import pyanthem
-   pyanthem.run()
-
-The first time you run pyanthem, it will download a necessary soundfont file - this will take a minute or two.
-
-.. code-block::
-   
-   ♫ Initializing soundfont library...
-   ♫ Downloading 17QuXRbApe0JTlYfBs7iSMCMu3xRWMHOV into...
-   ♫ 238.3 MiB Done.
-
-Once completed, the pyanthem GUI will initialize:
-
-.. image:: https://github.com/nicthib/pyanthem/blob/media/GUI1.png
-
-Next, load a dataset by clicking :code:`File > Load from .mat`. For this section, we will load the dataset :code:`demo1.mat`. Currently, you can import any .mat or hdf5 file that contains the following variables:
-
-1) Temporal variable (**H, required**): A 2D matrix of shape :code:`[n,t]`, where each row is a component and each column is a time-point. This variable is referred to as **"H"** in the pyanthem environment.
-
-2) Spatial variable (**W, optional**): A 3D matrix of shape :code:`[h,w,n]`, where h and w represent the spatial height and width of your dataset. If this variable is not given, no video output is possible.
-
-3) Framerate (**fr, optional**): A single float value, representing the frame rate of your dataset in Hz. If a framerate is not given, pyanthem will provide a default.
-
-*Note: Make sure to only include these variables in your file to avoid any errors. You can name them however you like, but make sure there are only one of each variable.* 
-
-Once loading is complete, the GUI should update with default options, and plots of **H** and **W**:
-
-.. image:: https://github.com/nicthib/pyanthem/blob/media/GUI2.png
-
-The bottom left plots show two representations of the dataset: A preview of the output movie (left), and a visualization of what components are included and the colormap selection. The right two plots show raw representations of **H** (top), and a visualization of the audio output file (right). Lighter colors indicate loud notes, and darker colors indicate quiet notes, with black indicating silence.
-
-From here, you can adjust parameters, preview the output, and finally save video and audio files. If you want to check how your parameter adjustments impact your audivisualization, click the **Update** button, and your changes will be reflected. Any issues with your selected parameters will be indicated in the white status box. Try adjusting a few parameters and observing how the plots change.
-
-Finally, render output files with the :code:`Save --> Write A/V then merge` menu command.
-
-Congratulations - you've created your first audiovisualization!
-
-Using pyanthem in CLI (command-line interface) mode
----------------------------------------------------
-
-pyanthem's CLI mode is useful for running batch conversions of large amounts of data once you are happy with your audiovisualization parameters, or creating more complex audiovisualizions that use multiple datasets and instruments. CLI mode is not recommended to use until you have used the GUI and are comfortable with the parameters and usage.
-
-To run pyanthem in CLI mode, pass the argument :code:`display=False`, and assign the :code:`.run()` method to a variable:
-
-.. code-block:: python
-   
-   import pyanthem
-   g=pyanthem.run(display=False)
-
-Next, load a dataset and config file using the :code:`.load_data()` and :code:`.load_config()` methods. You can pass an explicit file name to the :code:`file_in` argument, or pass none to recieve a file select prompt (note the use of the leading :code:`r` when naming a file location):
-
-.. code-block:: python
-   
-   g.load_data(file_in=r'path/to/your/file.mat')
-   g.load_config(file_in=r'path/to/your/config.p')
-
-Finally, render the audio and video file, then merge the files using the :code:`.write_audio()`, :code:`.write_video()` and :code:`.merge()` methods:
-
-.. code-block:: python
-   
-   g.write_audio()
-   g.write_video()
-   g.merge()
-
-Once you're comfortable with this syntax, you can combine all of these steps into a single line, write a merged video with the :code:`.write_AV()` method, and even remove the intermediate files using the :code:`.cleanup()` method:
-
-.. code-block:: python
-   
-   data_file = r'path/to/your/file.mat'
-   config_file = r'path/to/your/config.p'
-   g.load_data(file_in=data_file).load_config(file_in=config_file).write_AV().cleanup()
-
-Congratulations - you've created your first audiovisualization in CLI mode!
-
-Team
-====
-
-.. |niclogo| image:: https://avatars1.githubusercontent.com/u/34455769?v=3&s=200
-
-+---------------------------+
-| Nic Thibodeaux            |
-+===========================+
-| |niclogo|                 |
-+---------------------------+
-| http://github.com/nicthib |
-+---------------------------+
-
-FAQ
-===
-
-Under construction!
--------------------
-
-Support
-=======
-
-- Twitter: `@nicthibs`_
-
-.. _`@nicthibs`: http://twitter.com/nicthibs
-
-
+Metadata-Version: 2.1
+Name: pyanthem
+Version: 1.2.0
+Summary: pyanthem - an audiovisualization tool to make your data more interesting
+Home-page: https://github.com/nicthib/pyanthem
+Author: Nic Thibodeaux
+Author-email: dnt2111@columbia.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+********************************************************************
+pyanthem: Transforming your datasets into a colorful, audible format
+********************************************************************
+
+Features:
+=========
+
+1) Converts three-dimensional datasets to visually pleasing, audible representations
+2) A variety of video and audio parameters
+3) In-place video and audio merge
+4) GUI and Command-line interface for maximum flexibility
+5) Example datasets to get you started
+6) Headache-free installation with an Anaconda environment
+
+Usage
+=====
+
+pyanthem was primarily developed to interpret matrix-decomposed functional imaging datasets - for example, a dataset **V** with shape :code:`[height,width,time]`, is decomposed into two matrixes: **W** with shape :code:`[height*width,n]`, and **H** with shape :code:`[n,time]` such that :code:`H x W = V`. Here, n represents the number of variables represented by the decomposition. There are various techniques used to decompose matrixes - two popular techniques include Non-negative Matrix Factorization (NMF), and Singular Value Decomposition (SVD).
+
+Here's a visual illustration of matrix decomposition - note that in this example, :code:`n=2`:
+
+.. image:: https://upload.wikimedia.org/wikipedia/commons/f/f9/NMF.png
+
+If you would prefer to keep things simple, you can skip matrix decomposition altogether and focus solely on converting raw data to audio - only working with the **H** matrix, where each row represents a variable and each column represents a time point.
+
+If this is too much information to digest, don't worry! Try the example below to get more familiar with what the data looks like, and how pyanthem transforms it.
+
+Requirements
+============
+
+*See installation guide below before proceeding!*
+
+`Python 3.7`_:
+   Currently, pyanthem is tested to work on Python 3.7. This will be updated as more versions are tested.
+
+FFmpeg_:
+   ffmpeg enables video creation and merging.
+
+FluidSynth_:
+   FluidSynth enables conversion of MIDI files to crisp, high quality sound files.
+   
+If you do have the above requirements installed, you can install pyanthem using pip: :code:`pip install pyanthem`
+
+Conda (optional, but highly recommended):
+   Conda enables simple and reliable package installation. Use Miniconda_ for a minimal installation, or Anaconda_ otherwise.
+
+.. _`Python 3.7`: https://www.python.org/downloads/release/python-378/
+.. _FFmpeg: https://ffmpeg.org/
+.. _FluidSynth: http://www.fluidsynth.org/
+.. _Miniconda: https://docs.conda.io/en/latest/miniconda.html
+.. _Anaconda: https://www.anaconda.com/products/individual
+
+Installation
+============
+Note: If you do not have working installations of the listed requirements (Python 3.7 + fluidsynth + ffmpeg), it is **strongly recommended** that you use Miniconda_/Anaconda_ for a straightforward installation process. If you do not have either, Miniconda is preferred as it is a faster install and takes up much less space than Anaconda.
+
+Using Miniconda/Anaconda:
+-------------------------
+
+Create an environment and install the required packages::
+   
+   conda create -n pyanthem python=3.7 pip ffmpeg fluidsynth --channel conda-forge --channel nicthib
+
+Next, activate the environment::
+   
+   conda activate pyanthem
+
+Finally, install the pyanthem Python package using pip::
+   
+   pip install pyanthem
+
+Example datasets and Scripts
+----------------------------
+
+If you want to get familiar with the datasets that pyanthem uses and try some applications of pyanthem, clone this repository or download `here.`
+
+.. _`here`: https://github.com/nicthib/pyanthem/archive/master.zip
+
+Using pyanthem in a Jupyter Notebook
+-----------------------------------------------
+
+To access the pyanthem environment in a Jupyter notebook, first install ipykernel in your environment::
+   
+   conda install -c anaconda ipykernel
+
+After this, create the kernel::
+   
+   python -m ipykernel install --user --name=pyanthem
+
+Once in a notebook, switch to the pyanthem kernel by selecting :code:`Kernel > Change kernel > pyanthem`
+
+*Note: While the pyanthem kernel will now be available in any Jupyter notebook session, pyanthem will not function properly unless the Jupyter notebook is launched inside the pyanthem environment*.
+
+Example
+=======
+
+Using pyanthem in GUI mode
+--------------------------
+
+First, import pyanthem and begin a pyanthem session:
+
+.. code-block:: python
+   
+   import pyanthem
+   pyanthem.run()
+
+*Note: You may run into an error here where some packages are missing. Simply install them using pip, and try running pyanthem again.*
+
+The first time you run pyanthem, it will download a necessary soundfont file - this will take a minute or two.
+
+.. code-block::
+   
+   â™« Initializing soundfont library...
+   â™« Downloading 17QuXRbApe0JTlYfBs7iSMCMu3xRWMHOV into...
+   â™« 238.3 MiB Done.
+
+Once completed, the pyanthem GUI will initialize:
+
+.. image:: https://github.com/nicthib/pyanthem/blob/media/GUI1.png
+
+Next, load a dataset by clicking :code:`File > Load from .mat`. For this section, we will load the dataset :code:`demo1.mat`. Currently, you can import any .mat or hdf5 file that contains the following variables:
+
+1) Temporal variable (**H, required**): A 2D matrix of shape :code:`[n,t]`, where each row is a component and each column is a time-point. This variable is referred to as **"H"** in the pyanthem environment.
+
+2) Spatial variable (**W, optional**): A 3D matrix of shape :code:`[h,w,n]`, where h and w represent the spatial height and width of your dataset. If this variable is not given, no video output is possible.
+
+3) Framerate (**fr, optional**): A single float value, representing the frame rate of your dataset in Hz. If a framerate is not given, pyanthem will provide a default.
+
+*Note: Make sure to only include these variables in your file to avoid any errors. You can name them however you like, but make sure there are only one of each variable.* 
+
+Once loading is complete, the GUI should update with default options, and plots of **H** and **W**:
+
+.. image:: https://github.com/nicthib/pyanthem/blob/media/GUI2.png
+
+The bottom left plots show two representations of the dataset: A preview of the output movie (left), and a visualization of what components are included and the colormap selection. The right two plots show raw representations of **H** (top), and a visualization of the audio output file (right). Lighter colors indicate loud notes, and darker colors indicate quiet notes, with black indicating silence.
+
+From here, you can adjust parameters, preview the output, and finally save video and audio files. If you want to check how your parameter adjustments impact your audivisualization, click the **Update** button, and your changes will be reflected. Any issues with your selected parameters will be indicated in the white status box. Try adjusting a few parameters and observing how the plots change.
+
+Finally, render output files with the :code:`Save --> Write A/V then merge` menu command.
+
+Congratulations - you've created your first audiovisualization!
+
+Using pyanthem in CLI (command-line interface) mode
+---------------------------------------------------
+
+pyanthem's CLI mode is useful for running batch conversions of large amounts of data once you are happy with your audiovisualization parameters, or creating more complex audiovisualizions that use multiple datasets and instruments. CLI mode is not recommended to use until you have used the GUI and are comfortable with the parameters and usage.
+
+To run pyanthem in CLI mode, pass the argument :code:`display=False`, and assign the :code:`.run()` method to a variable:
+
+.. code-block:: python
+   
+   import pyanthem
+   g=pyanthem.run(display=False)
+
+Next, load a dataset and config file using the :code:`.load_data()` and :code:`.load_config()` methods. You can pass an explicit file name to the :code:`file_in` argument, or pass none to recieve a file select prompt (note the use of the leading :code:`r` when naming a file location):
+
+.. code-block:: python
+   
+   g.load_data(file_in=r'path/to/your/file.mat')
+   g.load_config(file_in=r'path/to/your/config.p')
+
+Finally, render the audio and video file, then merge the files using the :code:`.write_audio()`, :code:`.write_video()` and :code:`.merge()` methods:
+
+.. code-block:: python
+   
+   g.write_audio()
+   g.write_video()
+   g.merge()
+
+Once you're comfortable with this syntax, you can combine all of these steps into a single line, write a merged video with the :code:`.write_AV()` method, and even remove the intermediate files using the :code:`.cleanup()` method:
+
+.. code-block:: python
+   
+   data_file = r'path/to/your/file.mat'
+   config_file = r'path/to/your/config.p'
+   g.load_data(file_in=data_file).load_config(file_in=config_file).write_AV().cleanup()
+
+Congratulations - you've created your first audiovisualization in CLI mode!
+
+Team
+====
+
+.. |niclogo| image:: https://avatars1.githubusercontent.com/u/34455769?v=3&s=200
+
++---------------------------+
+| Nic Thibodeaux            |
++===========================+
+| |niclogo|                 |
++---------------------------+
+| http://github.com/nicthib |
++---------------------------+
+
+FAQ
+===
+
+Under construction!
+-------------------
+
+Support
+=======
+
+- Twitter: `@nicthibs`_
+
+.. _`@nicthibs`: http://twitter.com/nicthibs
```

### Comparing `pyanthem-1.1.9/README.rst` & `pyanthem-1.2.0/pyanthem.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,202 +1,218 @@
-********************************************************************
-pyanthem: Transforming your datasets into a colorful, audible format
-********************************************************************
-
-Features:
-=========
-
-1) Converts three-dimensional datasets to visually pleasing, audible representations
-2) A variety of video and audio parameters
-3) In-place video and audio merge
-4) GUI and Command-line interface for maximum flexibility
-5) Example datasets to get you started
-6) Headache-free installation with an Anaconda environment
-
-Usage
-=====
-
-pyanthem was primarily developed to interpret matrix-decomposed functional imaging datasets - for example, a dataset **V** with shape :code:`[height,width,time]`, is decomposed into two matrixes: **W** with shape :code:`[height*width,n]`, and **H** with shape :code:`[n,time]` such that :code:`H x W = V`. Here, n represents the number of variables represented by the decomposition. There are various techniques used to decompose matrixes - two popular techniques include Non-negative Matrix Factorization (NMF), and Singular Value Decomposition (SVD).
-
-Here's a visual illustration of matrix decomposition - note that in this example, :code:`n=2`:
-
-.. image:: https://upload.wikimedia.org/wikipedia/commons/f/f9/NMF.png
-
-If you would prefer to keep things simple, you can skip matrix decomposition altogether and focus solely on converting raw data to audio - only working with the **H** matrix, where each row represents a variable and each column represents a time point.
-
-If this is too much information to digest, don't worry! Try the example below to get more familiar with what the data looks like, and how pyanthem transforms it.
-
-Requirements
-============
-
-*See installation guide below before proceeding!*
-
-`Python 3.7`_:
-   Currently, pyanthem is tested to work on Python 3.7. This will be updated as more versions are tested.
-
-FFmpeg_:
-   ffmpeg enables video creation and merging.
-
-FluidSynth_:
-   FluidSynth enables conversion of MIDI files to crisp, high quality sound files.
-   
-If you do have the above requirements installed, you can install pyanthem using pip: :code:`pip install pyanthem`
-
-Conda (optional, but highly recommended):
-   Conda enables simple and reliable package installation. Use Miniconda_ for a minimal installation, or Anaconda_ otherwise.
-
-.. _`Python 3.7`: https://www.python.org/downloads/release/python-378/
-.. _FFmpeg: https://ffmpeg.org/
-.. _FluidSynth: http://www.fluidsynth.org/
-.. _Miniconda: https://docs.conda.io/en/latest/miniconda.html
-.. _Anaconda: https://www.anaconda.com/products/individual
-
-Installation
-============
-Note: If you do not have working installations of the listed requirements (Python 3.7 + fluidsynth + ffmpeg), it is **strongly recommended** that you use Miniconda_/Anaconda_ for a straightforward installation process. If you do not have either, Miniconda is preferred as it is a faster install and takes up much less space than Anaconda.
-
-Using Miniconda/Anaconda:
--------------------------
-
-Create an environment and install the required packages::
-   
-   conda create -n pyanthem python=3.7 pip ffmpeg fluidsynth --channel conda-forge --channel nicthib
-
-Next, activate the environment::
-   
-   conda activate pyanthem
-
-Finally, install the pyanthem Python package using pip::
-   
-   pip install pyanthem
-
-Example datasets and Scripts
-----------------------------
-
-If you want to get familiar with the datasets that pyanthem uses and try some applications of pyanthem, clone this repository or download `here.`
-
-.. _`here`: https://github.com/nicthib/pyanthem/archive/master.zip
-
-Using pyanthem in a Jupyter Notebook
------------------------------------------------
-
-To access the pyanthem environment in a Jupyter notebook, first install ipykernel in your environment::
-   
-   conda install -c anaconda ipykernel
-
-After this, create the kernel::
-   
-   python -m ipykernel install --user --name=pyanthem
-
-Once in a notebook, switch to the pyanthem kernel by selecting :code:`Kernel > Change kernel > pyanthem`
-
-*Note: While the pyanthem kernel will now be available in any Jupyter notebook session, pyanthem will not function properly unless the Jupyter notebook is launched inside the pyanthem environment*.
-
-Example
-=======
-
-Using pyanthem in GUI mode
---------------------------
-
-First, import pyanthem and begin a pyanthem session:
-
-.. code-block:: python
-   
-   import pyanthem
-   pyanthem.run()
-
-The first time you run pyanthem, it will download a necessary soundfont file - this will take a minute or two.
-
-.. code-block::
-   
-   ♫ Initializing soundfont library...
-   ♫ Downloading 17QuXRbApe0JTlYfBs7iSMCMu3xRWMHOV into...
-   ♫ 238.3 MiB Done.
-
-Once completed, the pyanthem GUI will initialize:
-
-.. image:: https://github.com/nicthib/pyanthem/blob/media/GUI1.png
-
-Next, load a dataset by clicking :code:`File > Load from .mat`. For this section, we will load the dataset :code:`demo1.mat`. Currently, you can import any .mat or hdf5 file that contains the following variables:
-
-1) Temporal variable (**H, required**): A 2D matrix of shape :code:`[n,t]`, where each row is a component and each column is a time-point. This variable is referred to as **"H"** in the pyanthem environment.
-
-2) Spatial variable (**W, optional**): A 3D matrix of shape :code:`[h,w,n]`, where h and w represent the spatial height and width of your dataset. If this variable is not given, no video output is possible.
-
-3) Framerate (**fr, optional**): A single float value, representing the frame rate of your dataset in Hz. If a framerate is not given, pyanthem will provide a default.
-
-*Note: Make sure to only include these variables in your file to avoid any errors. You can name them however you like, but make sure there are only one of each variable.* 
-
-Once loading is complete, the GUI should update with default options, and plots of **H** and **W**:
-
-.. image:: https://github.com/nicthib/pyanthem/blob/media/GUI2.png
-
-The bottom left plots show two representations of the dataset: A preview of the output movie (left), and a visualization of what components are included and the colormap selection. The right two plots show raw representations of **H** (top), and a visualization of the audio output file (right). Lighter colors indicate loud notes, and darker colors indicate quiet notes, with black indicating silence.
-
-From here, you can adjust parameters, preview the output, and finally save video and audio files. If you want to check how your parameter adjustments impact your audivisualization, click the **Update** button, and your changes will be reflected. Any issues with your selected parameters will be indicated in the white status box. Try adjusting a few parameters and observing how the plots change.
-
-Finally, render output files with the :code:`Save --> Write A/V then merge` menu command.
-
-Congratulations - you've created your first audiovisualization!
-
-Using pyanthem in CLI (command-line interface) mode
----------------------------------------------------
-
-pyanthem's CLI mode is useful for running batch conversions of large amounts of data once you are happy with your audiovisualization parameters, or creating more complex audiovisualizions that use multiple datasets and instruments. CLI mode is not recommended to use until you have used the GUI and are comfortable with the parameters and usage.
-
-To run pyanthem in CLI mode, pass the argument :code:`display=False`, and assign the :code:`.run()` method to a variable:
-
-.. code-block:: python
-   
-   import pyanthem
-   g=pyanthem.run(display=False)
-
-Next, load a dataset and config file using the :code:`.load_data()` and :code:`.load_config()` methods. You can pass an explicit file name to the :code:`file_in` argument, or pass none to recieve a file select prompt (note the use of the leading :code:`r` when naming a file location):
-
-.. code-block:: python
-   
-   g.load_data(file_in=r'path/to/your/file.mat')
-   g.load_config(file_in=r'path/to/your/config.p')
-
-Finally, render the audio and video file, then merge the files using the :code:`.write_audio()`, :code:`.write_video()` and :code:`.merge()` methods:
-
-.. code-block:: python
-   
-   g.write_audio()
-   g.write_video()
-   g.merge()
-
-Once you're comfortable with this syntax, you can combine all of these steps into a single line, write a merged video with the :code:`.write_AV()` method, and even remove the intermediate files using the :code:`.cleanup()` method:
-
-.. code-block:: python
-   
-   data_file = r'path/to/your/file.mat'
-   config_file = r'path/to/your/config.p'
-   g.load_data(file_in=data_file).load_config(file_in=config_file).write_AV().cleanup()
-
-Congratulations - you've created your first audiovisualization in CLI mode!
-
-Team
-====
-
-.. |niclogo| image:: https://avatars1.githubusercontent.com/u/34455769?v=3&s=200
-
-+---------------------------+
-| Nic Thibodeaux            |
-+===========================+
-| |niclogo|                 |
-+---------------------------+
-| http://github.com/nicthib |
-+---------------------------+
-
-FAQ
-===
-
-Under construction!
--------------------
-
-Support
-=======
-
-- Twitter: `@nicthibs`_
-
-.. _`@nicthibs`: http://twitter.com/nicthibs
+Metadata-Version: 2.1
+Name: pyanthem
+Version: 1.2.0
+Summary: pyanthem - an audiovisualization tool to make your data more interesting
+Home-page: https://github.com/nicthib/pyanthem
+Author: Nic Thibodeaux
+Author-email: dnt2111@columbia.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+********************************************************************
+pyanthem: Transforming your datasets into a colorful, audible format
+********************************************************************
+
+Features:
+=========
+
+1) Converts three-dimensional datasets to visually pleasing, audible representations
+2) A variety of video and audio parameters
+3) In-place video and audio merge
+4) GUI and Command-line interface for maximum flexibility
+5) Example datasets to get you started
+6) Headache-free installation with an Anaconda environment
+
+Usage
+=====
+
+pyanthem was primarily developed to interpret matrix-decomposed functional imaging datasets - for example, a dataset **V** with shape :code:`[height,width,time]`, is decomposed into two matrixes: **W** with shape :code:`[height*width,n]`, and **H** with shape :code:`[n,time]` such that :code:`H x W = V`. Here, n represents the number of variables represented by the decomposition. There are various techniques used to decompose matrixes - two popular techniques include Non-negative Matrix Factorization (NMF), and Singular Value Decomposition (SVD).
+
+Here's a visual illustration of matrix decomposition - note that in this example, :code:`n=2`:
+
+.. image:: https://upload.wikimedia.org/wikipedia/commons/f/f9/NMF.png
+
+If you would prefer to keep things simple, you can skip matrix decomposition altogether and focus solely on converting raw data to audio - only working with the **H** matrix, where each row represents a variable and each column represents a time point.
+
+If this is too much information to digest, don't worry! Try the example below to get more familiar with what the data looks like, and how pyanthem transforms it.
+
+Requirements
+============
+
+*See installation guide below before proceeding!*
+
+`Python 3.7`_:
+   Currently, pyanthem is tested to work on Python 3.7. This will be updated as more versions are tested.
+
+FFmpeg_:
+   ffmpeg enables video creation and merging.
+
+FluidSynth_:
+   FluidSynth enables conversion of MIDI files to crisp, high quality sound files.
+   
+If you do have the above requirements installed, you can install pyanthem using pip: :code:`pip install pyanthem`
+
+Conda (optional, but highly recommended):
+   Conda enables simple and reliable package installation. Use Miniconda_ for a minimal installation, or Anaconda_ otherwise.
+
+.. _`Python 3.7`: https://www.python.org/downloads/release/python-378/
+.. _FFmpeg: https://ffmpeg.org/
+.. _FluidSynth: http://www.fluidsynth.org/
+.. _Miniconda: https://docs.conda.io/en/latest/miniconda.html
+.. _Anaconda: https://www.anaconda.com/products/individual
+
+Installation
+============
+Note: If you do not have working installations of the listed requirements (Python 3.7 + fluidsynth + ffmpeg), it is **strongly recommended** that you use Miniconda_/Anaconda_ for a straightforward installation process. If you do not have either, Miniconda is preferred as it is a faster install and takes up much less space than Anaconda.
+
+Using Miniconda/Anaconda:
+-------------------------
+
+Create an environment and install the required packages::
+   
+   conda create -n pyanthem python=3.7 pip ffmpeg fluidsynth --channel conda-forge --channel nicthib
+
+Next, activate the environment::
+   
+   conda activate pyanthem
+
+Finally, install the pyanthem Python package using pip::
+   
+   pip install pyanthem
+
+Example datasets and Scripts
+----------------------------
+
+If you want to get familiar with the datasets that pyanthem uses and try some applications of pyanthem, clone this repository or download `here.`
+
+.. _`here`: https://github.com/nicthib/pyanthem/archive/master.zip
+
+Using pyanthem in a Jupyter Notebook
+-----------------------------------------------
+
+To access the pyanthem environment in a Jupyter notebook, first install ipykernel in your environment::
+   
+   conda install -c anaconda ipykernel
+
+After this, create the kernel::
+   
+   python -m ipykernel install --user --name=pyanthem
+
+Once in a notebook, switch to the pyanthem kernel by selecting :code:`Kernel > Change kernel > pyanthem`
+
+*Note: While the pyanthem kernel will now be available in any Jupyter notebook session, pyanthem will not function properly unless the Jupyter notebook is launched inside the pyanthem environment*.
+
+Example
+=======
+
+Using pyanthem in GUI mode
+--------------------------
+
+First, import pyanthem and begin a pyanthem session:
+
+.. code-block:: python
+   
+   import pyanthem
+   pyanthem.run()
+
+*Note: You may run into an error here where some packages are missing. Simply install them using pip, and try running pyanthem again.*
+
+The first time you run pyanthem, it will download a necessary soundfont file - this will take a minute or two.
+
+.. code-block::
+   
+   â™« Initializing soundfont library...
+   â™« Downloading 17QuXRbApe0JTlYfBs7iSMCMu3xRWMHOV into...
+   â™« 238.3 MiB Done.
+
+Once completed, the pyanthem GUI will initialize:
+
+.. image:: https://github.com/nicthib/pyanthem/blob/media/GUI1.png
+
+Next, load a dataset by clicking :code:`File > Load from .mat`. For this section, we will load the dataset :code:`demo1.mat`. Currently, you can import any .mat or hdf5 file that contains the following variables:
+
+1) Temporal variable (**H, required**): A 2D matrix of shape :code:`[n,t]`, where each row is a component and each column is a time-point. This variable is referred to as **"H"** in the pyanthem environment.
+
+2) Spatial variable (**W, optional**): A 3D matrix of shape :code:`[h,w,n]`, where h and w represent the spatial height and width of your dataset. If this variable is not given, no video output is possible.
+
+3) Framerate (**fr, optional**): A single float value, representing the frame rate of your dataset in Hz. If a framerate is not given, pyanthem will provide a default.
+
+*Note: Make sure to only include these variables in your file to avoid any errors. You can name them however you like, but make sure there are only one of each variable.* 
+
+Once loading is complete, the GUI should update with default options, and plots of **H** and **W**:
+
+.. image:: https://github.com/nicthib/pyanthem/blob/media/GUI2.png
+
+The bottom left plots show two representations of the dataset: A preview of the output movie (left), and a visualization of what components are included and the colormap selection. The right two plots show raw representations of **H** (top), and a visualization of the audio output file (right). Lighter colors indicate loud notes, and darker colors indicate quiet notes, with black indicating silence.
+
+From here, you can adjust parameters, preview the output, and finally save video and audio files. If you want to check how your parameter adjustments impact your audivisualization, click the **Update** button, and your changes will be reflected. Any issues with your selected parameters will be indicated in the white status box. Try adjusting a few parameters and observing how the plots change.
+
+Finally, render output files with the :code:`Save --> Write A/V then merge` menu command.
+
+Congratulations - you've created your first audiovisualization!
+
+Using pyanthem in CLI (command-line interface) mode
+---------------------------------------------------
+
+pyanthem's CLI mode is useful for running batch conversions of large amounts of data once you are happy with your audiovisualization parameters, or creating more complex audiovisualizions that use multiple datasets and instruments. CLI mode is not recommended to use until you have used the GUI and are comfortable with the parameters and usage.
+
+To run pyanthem in CLI mode, pass the argument :code:`display=False`, and assign the :code:`.run()` method to a variable:
+
+.. code-block:: python
+   
+   import pyanthem
+   g=pyanthem.run(display=False)
+
+Next, load a dataset and config file using the :code:`.load_data()` and :code:`.load_config()` methods. You can pass an explicit file name to the :code:`file_in` argument, or pass none to recieve a file select prompt (note the use of the leading :code:`r` when naming a file location):
+
+.. code-block:: python
+   
+   g.load_data(file_in=r'path/to/your/file.mat')
+   g.load_config(file_in=r'path/to/your/config.p')
+
+Finally, render the audio and video file, then merge the files using the :code:`.write_audio()`, :code:`.write_video()` and :code:`.merge()` methods:
+
+.. code-block:: python
+   
+   g.write_audio()
+   g.write_video()
+   g.merge()
+
+Once you're comfortable with this syntax, you can combine all of these steps into a single line, write a merged video with the :code:`.write_AV()` method, and even remove the intermediate files using the :code:`.cleanup()` method:
+
+.. code-block:: python
+   
+   data_file = r'path/to/your/file.mat'
+   config_file = r'path/to/your/config.p'
+   g.load_data(file_in=data_file).load_config(file_in=config_file).write_AV().cleanup()
+
+Congratulations - you've created your first audiovisualization in CLI mode!
+
+Team
+====
+
+.. |niclogo| image:: https://avatars1.githubusercontent.com/u/34455769?v=3&s=200
+
++---------------------------+
+| Nic Thibodeaux            |
++===========================+
+| |niclogo|                 |
++---------------------------+
+| http://github.com/nicthib |
++---------------------------+
+
+FAQ
+===
+
+Under construction!
+-------------------
+
+Support
+=======
+
+- Twitter: `@nicthibs`_
+
+.. _`@nicthibs`: http://twitter.com/nicthibs
```

### Comparing `pyanthem-1.1.9/pyanthem/decompmp4.py` & `pyanthem-1.2.0/pyanthem/decompmp4.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import pyanthem
-from numpy.matlib import repmat
-g=pyanthem.GUI(display=False)
-import subprocess as sp
-import numpy as np
-file = r'C:\Users\dnt21\Downloads\stars.mp4'
-command = [ 'ffmpeg','-i', file,'-f', 'image2pipe','-pix_fmt', 'rgb24','-vcodec', 'rawvideo', '-']
-pipe = sp.Popen(command, stdout = sp.PIPE, bufsize=10**8)
-vid = []
-while True:
-    try:
-        raw_image = pipe.stdout.read(640*360*3)
-        image =  np.fromstring(raw_image, dtype='uint8')
-        vid.append(np.mean(image.reshape((360,640,3)),axis=2))
-        pipe.stdout.flush()
-    except:
-        break
-vid = np.moveaxis(np.asarray(vid),0,-1)
-bl = np.mean(vid,axis=2)
-vid = vid - np.repeat(bl[:, :, np.newaxis], vid.shape[2], axis=2)
+import pyanthem
+from numpy.matlib import repmat
+g=pyanthem.GUI(display=False)
+import subprocess as sp
+import numpy as np
+file = r'C:\Users\dnt21\Downloads\stars.mp4'
+command = [ 'ffmpeg','-i', file,'-f', 'image2pipe','-pix_fmt', 'rgb24','-vcodec', 'rawvideo', '-']
+pipe = sp.Popen(command, stdout = sp.PIPE, bufsize=10**8)
+vid = []
+while True:
+    try:
+        raw_image = pipe.stdout.read(640*360*3)
+        image =  np.fromstring(raw_image, dtype='uint8')
+        vid.append(np.mean(image.reshape((360,640,3)),axis=2))
+        pipe.stdout.flush()
+    except:
+        break
+vid = np.moveaxis(np.asarray(vid),0,-1)
+bl = np.mean(vid,axis=2)
+vid = vid - np.repeat(bl[:, :, np.newaxis], vid.shape[2], axis=2)
 g.process_raw(data=vid,frame_rate=25,save=True,n_clusters=30)
```

### Comparing `pyanthem-1.1.9/pyanthem/obsolete.py` & `pyanthem-1.2.0/pyanthem/obsolete.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-def synth(self):
-		'''
-		
-		'''
-		fs = 44100
-		r = .5 # release for note
-		#r_mat = np.linspace(1, 0, num=int(fs*r))
-		#r_mat = np.vstack((r_mat,r_mat)).T
-		currnote = -1
-		ext = 11
-		note = [[0] * 8 for i in range(3)]
-		raws = np.zeros((int(fs*(np.max(self.nd['st'])+ext)),2))
-		nnotes = len(self.nd['st'])
-		for i in range(len(self.nd['st'])):
-			if currnote != self.nd['note'][i]:
-				currnote = self.nd['note'][i]
-				for mag in range(8): # Load up new notes
-					for length in range(3):
-						fn = str(currnote+1)+'_'+str(mag)+'_'+str(length+1)+'.ogg';
-						note[length][mag],notused = read(os.path.join(self.package_path,'AE',fn))
-			L = self.nd['en'][i]-self.nd['st'][i]
-			L = min(L,10-r)
-			if L > 1:
-				raw = note[2][int(np.ceil(self.nd['mag'][i]/16-1))]#[0:int(L*fs)] # Truncate to note length plus release
-			elif 1 > L > .25:
-				raw = note[1][int(np.ceil(self.nd['mag'][i]/16-1))]#[0:int(L*fs)] # Truncate to note length plus release
-			elif L < .25:
-				raw = note[0][int(np.ceil(self.nd['mag'][i]/16-1))]#[0:int(L*fs)] # Truncate to note length plus release
-			#raw[-int(fs*r):] *= r_mat
-			inds = range(int(self.nd['st'][i][0]*fs),int(self.nd['st'][i][0]*fs)+len(raw))
-			raws[inds,:] += raw
-			if self.display:
-				self.status['text'] = f'Status: writing audio file, {i+1} out of {nnotes} notes written'
-				self.update()
-		raws = raws[:-fs*(ext-1),:] # Crop wav
-		raws = np.int16(raws/np.max(np.abs(raws)) * 32767)
-		wavwrite(os.path.join(self.cfg['save_path'],self.cfg['file_out'])+'.wav',fs,raws)
-		
-	
+def synth(self):
+		'''
+		
+		'''
+		fs = 44100
+		r = .5 # release for note
+		#r_mat = np.linspace(1, 0, num=int(fs*r))
+		#r_mat = np.vstack((r_mat,r_mat)).T
+		currnote = -1
+		ext = 11
+		note = [[0] * 8 for i in range(3)]
+		raws = np.zeros((int(fs*(np.max(self.nd['st'])+ext)),2))
+		nnotes = len(self.nd['st'])
+		for i in range(len(self.nd['st'])):
+			if currnote != self.nd['note'][i]:
+				currnote = self.nd['note'][i]
+				for mag in range(8): # Load up new notes
+					for length in range(3):
+						fn = str(currnote+1)+'_'+str(mag)+'_'+str(length+1)+'.ogg';
+						note[length][mag],notused = read(os.path.join(self.package_path,'AE',fn))
+			L = self.nd['en'][i]-self.nd['st'][i]
+			L = min(L,10-r)
+			if L > 1:
+				raw = note[2][int(np.ceil(self.nd['mag'][i]/16-1))]#[0:int(L*fs)] # Truncate to note length plus release
+			elif 1 > L > .25:
+				raw = note[1][int(np.ceil(self.nd['mag'][i]/16-1))]#[0:int(L*fs)] # Truncate to note length plus release
+			elif L < .25:
+				raw = note[0][int(np.ceil(self.nd['mag'][i]/16-1))]#[0:int(L*fs)] # Truncate to note length plus release
+			#raw[-int(fs*r):] *= r_mat
+			inds = range(int(self.nd['st'][i][0]*fs),int(self.nd['st'][i][0]*fs)+len(raw))
+			raws[inds,:] += raw
+			if self.display:
+				self.status['text'] = f'Status: writing audio file, {i+1} out of {nnotes} notes written'
+				self.update()
+		raws = raws[:-fs*(ext-1),:] # Crop wav
+		raws = np.int16(raws/np.max(np.abs(raws)) * 32767)
+		wavwrite(os.path.join(self.cfg['save_path'],self.cfg['file_out'])+'.wav',fs,raws)
+		
+
```

### Comparing `pyanthem-1.1.9/pyanthem/pyanthem.py` & `pyanthem-1.2.0/pyanthem/pyanthem.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,907 +1,907 @@
-import os, random, sys, time, csv, pickle, re, pkg_resources, mido, h5py
-os.environ['PYGAME_HIDE_SUPPORT_PROMPT']="hide"
-from tkinter import *
-from tkinter.ttk import *
-from tkinter import filedialog as fd 
-from tkinter import simpledialog as sd 
-from ttkthemes import ThemedTk
-from scipy.io import loadmat, savemat, whosmat
-from scipy.optimize import nnls
-from scipy.interpolate import interp1d
-from scipy.io.wavfile import write as wavwrite
-from sklearn.cluster import KMeans
-from pygame.mixer import init, quit, get_init, set_num_channels, pre_init, music
-import matplotlib.pyplot as plt
-from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
-import matplotlib.ticker as tkr
-import matplotlib.cm as cmaps # https://matplotlib.org/gallery/color/colormap_reference.html
-import numpy as np
-from numpy.matlib import repmat
-try:
-	from pyanthem.pyanthem_vars import *
-except:
-	from pyanthem_vars import *
-from google_drive_downloader import GoogleDriveDownloader as gdd
-import subprocess as sp
-import PIL.Image as Image
-
-def init_entry(fn):
-	'''
-	Generalized version of StringVar/DoubleVar followed by set()
-	'''
-	if isinstance(fn, str) or fn is None:
-		entry=StringVar()
-	else:
-		entry=DoubleVar()
-	entry.set(fn)
-	return entry
-
-def stack_files(files,fmts,fn):
-	'''
-	Stacks .mp4 videos horizontally, and merges wav files
-	the fmts argument is a list of three possible formats: 'a', 'v', or 'av'
-	Videos must match in height.
-	'''
-	nv=len([fmt for fmt in fmts if 'v' in fmt])
-	na=len([fmt for fmt in fmts if 'a' in fmt])
-	vf=[i for i,fmt in enumerate(fmts) if 'v' in fmt]
-	af=[i for i,fmt in enumerate(fmts) if 'a' in fmt]
-
-	# 3 cases: 1) Videos and audio, 2) Only videos, 3) Only audio
-	filter_command='"'
-	map_command=''
-
-	if nv > 1:
-		for v in vf:
-			filter_command+='[{}:v]'.format(v)
-		filter_command+='hstack=inputs={}[v]'.format(nv)
-		map_command+=' -map "[v]" '
-	elif nv == 1:
-		map_command += '-c:v copy -map {}:v:0'.format(vf[0])
-	
-	if na > 1:
-		# Seperate complex filters if video is being merged
-		if nv > 1:
-			filter_command+=';'
-		for a in af:
-			filter_command+='[{}:a]'.format(a)
-		filter_command+='amerge=inputs={}[a]'.format(na)
-		map_command+=' -map "[a]" '
-	elif na == 1:
-		map_command += ' -c:a aac -map {}:a:0 '.format(af[0])
-		
-	filter_command+='"'
-	in_command=''
-	for i in range(len(files)):
-		in_command += ' -i '+files[i]
-	full_command = 'ffmpeg -y '+in_command+' -filter_complex '+filter_command+' '+map_command+' -ac 2 -vsync 0 '+fn
-	print(full_command)
-	os.system(full_command)
-
-def uiopen(title,filetypes):
-	'''
-	Simple uiopen GUI instance.
-	'''
-	root=Tk()
-	root.withdraw()
-	file_in=os.path.normpath(fd.askopenfilename(title=title,filetypes=filetypes))
-	root.update()
-	root.destroy()
-	return file_in
-
-def run(display=True):
-	'''
-	Main command to run GUI or CLI
-	'''
-	root=GUI(display=display)
-	sys.ps1='♫ '
-	if display:
-		root.mainloop()
-	else:
-		print('Welcome to pyanthem v{}!'.format(pkg_resources.require('pyanthem')[0].version))
-		return root
-
-class GUI(ThemedTk):
-	def __init__(self,display=True):
-		'''
-		Initializes the GUI instance. display=True runs the Tk.__init__(self)
-		command, while display=False skips that and visual initialization, keeping
-		the GUI 'hidden'
-		'''
-		self.display=display
-		self.sf_path=os.path.join(os.path.dirname(os.path.abspath(__file__)),'anthem_soundfonts')
-		if not os.path.isdir(self.sf_path):
-			print('Initializing soundfont library...')
-			os.mkdir(self.sf_path)
-			gdd.download_file_from_google_drive(file_id=sound_font,dest_path=\
-				os.path.join(os.path.join(os.path.dirname(os.path.abspath(__file__)),'anthem_soundfonts'),'font.sf2'),showsize=True)
-		if self.display:
-			ThemedTk.__init__(self)
-			self.set_theme('clearlooks')
-			self.initGUI()
-	
-	def quit(self,event=None):
-		'''
-		Quits the GUI instance. Currently, jupyter instances are kinda buggy
-		'''
-		try:
-			# This raises a NameError exception in a notebook env, since 
-			# sys.exit() is not an appropriate method
-			get_ipython().__class__.__name__ 
-			self.destroy()
-		except NameError:
-			sys.exit()
-
-	def message(self,msg):
-		'''
-		Sends message through print if no GUI, through self.status if GUI is running
-		'''
-		if self.display:
-			self.status['text']=msg
-		else:
-			print(msg)
-
-	def check_data(self):
-		'''
-		Checks to make sure data is loaded.
-		'''
-		if hasattr(self,'data') and self.cfg['save_path'] is not None:
-			return True
-		else:
-			self.message('Error: No dataset has been loaded or save_path is empty.')
-			return False
-	
-	def self_to_cfg(self):
-		'''
-		This function is necessary to allow command-line access of the GUI functions. 
-		StringVar() and IntVar() allow for dynamic, quick field updating and access, 
-		but cannot be used outside of a mainloop or be pickled. for this reason, I convert 
-		all StringVars and IntVars to a new dict called 'self.cfg', that can be accessed 
-		oustide the GUI and dumped to a pickle file, which essentially "saves" the GUI.
-		'''
-		self.cfg={k: getattr(self,k).get() if self_fns[k] is 'entry' else getattr(self,k) for k in self_fns}
-
-	def dump_cfg(self):
-		'''
-		Saves config file.
-		'''
-		file_out=os.path.join(self.cfg['save_path'],self.cfg['file_out'])+'_cfg.p'
-		pickle.dump(self.cfg,open(file_out, "wb"))
-		self.message(f'cfg file saved to {file_out}')
-	
-	def load_data(self,filein=None):
-		'''
-		Loads dataset from filein. At the time, only supports .mat files.
-		'''
-		if filein is None:
-			filein=uiopen(title='Select mat or hdf5 file for import',filetypes=[('.mat files','*.mat'),('hdf5 files','*.h5'),('hdf5 files','*.hdf5')])
-		if filein=='.':
-			return
-		if filein.endswith('.mat'):
-			data_unk,var=loadmat(filein),whosmat(filein)
-			var = [v[0] for v in var]
-		elif filein.endswith('.hdf5') or filein.endswith('.h5'):
-			data_unk=h5py.File(filein, 'r')
-			var = data_unk.keys
-		data = {}
-		for k in var:
-			print()
-			tmp_var = np.asarray(data_unk[k])
-			if k in ('__header__', '__version__', '__globals__'):
-				continue
-			elif len(tmp_var.flatten())==1:
-				data['fr']=float(tmp_var)
-			elif tmp_var.ndim==2:
-				data['H']=tmp_var
-			elif tmp_var.ndim==3:
-				data['W']=tmp_var
-		# Checks inner dimension match if both H and W present in file.
-		if ('H' in data and 'W' in data) and data['H'].shape[0] != data['W'].shape[-1]:
-			# try flipping dims
-			if ('H' in data and 'W' in data) and data['H'].T.shape[0] == data['W'].T.shape[-1]:
-				data['H'] = data['H'].T
-				data['W'] = data['W'].T
-			else:
-				self.message('Error: Inner or outer dimensions of W [shape={}] and H [shape={}] do not match!'.format(data['H'].shape, data['W'].shape))
-				return
-		if 'H' in data:
-			if 'W' in data:
-				data['W_shape']=data['W'].shape
-				data['W']=data['W'].reshape(data['W'].shape[0]*data['W'].shape[1],data['W'].shape[2])
-			if 'fr' not in data:
-				data['fr']=data['H'].shape[1]/60 # Forces length to be 1 minute!
-			self.data=data
-			if not self.display:
-				return self
-		else:
-			self.message('Error: .mat file incompatible. Please select a .mat file with three variables: W (3D), H (2D), and fr (1-element float)')
-
-	def load_GUI(self):
-		'''
-		GUI-addons for load_data. Prompts user with filedialog, assigns defaults and sets GUI fields. 
-		'''
-		filein=uiopen(title='Select mat or hdf5 file for import',filetypes=[('.mat files','*.mat'),('hdf5 files','*.h5'),('hdf5 files','*.hdf5')])
-		if filein=='.':
-			return
-		self.load_data(filein)
-		if not hasattr(self,'data'):
-			return
-		self.data['H_pp']=self.data['H']
-		self.data['H_fp']=self.data['H']
-		self.fr.set(self.data['fr'])
-		if 'W' in self.data:
-			self.data['W_pp']=self.data['W']
-		self.file_in.set(os.path.splitext(os.path.split(filein)[1])[0])
-
-		# Set some defaults
-		self.file_out.set(self.file_in.get())
-		self.save_path.set(os.path.split(filein)[0])
-		Hstr='H' # for whatever reason, can't double nest quotations in an f-string :/
-		self.brightness.set(f'{float(f"{np.mean(self.data[Hstr])+np.std(self.data[Hstr]):.3g}"):g}')
-		self.threshold.set(f'{float(f"{np.mean(self.data[Hstr])+np.std(self.data[Hstr]):.3g}"):g}')
-		self.comps_to_show_arr=list(range(len(self.data['H'])))
-		self.init_plots()
-		self.process_H_W()
-	
-	def load_config(self,filein=None):
-		'''
-		Loads .p file containing dict of parameters needed to create outputs. If display=True, sets GUI fields.
-		'''
-		if filein is None:
-			filein=uiopen(title='Select pickle file for import',filetypes=[('pickle file','*.p'),('pickle file','*.pkl'),('pickle file','*.pickle')])
-		if filein=='.':
-			return
-		with open(filein, "rb") as f:
-			self.cfg=pickle.load(f)
-			if self.display:
-				for key,value in self.cfg.items():
-					if self_fns[key] is 'entry':
-						getattr(self,key).set(value)
-					else:
-						setattr(self,key,value)
-				self.refresh_GUI()
-			else:
-				return self
-
-	def refresh_GUI(self,event=None):
-		#self.init_plots()
-		if 'W_pp' in self.data:
-			if self.frameslider.get() > len(self.data['H_pp'].T): # This (usually) occurs when the user crops the dataset
-				self.frameslider.set(1)
-			self.frameslider['to']=int(len(self.data['H_pp'].T)-1)
-			self.imWH=self.Wax1.imshow((self.data['W_pp']@np.diag(self.data['H_pp'][:,int(self.frameslider.get())])@\
-				self.cmap[:,:-1]*(255/self.cfg['brightness'])).reshape(self.data['W_shape'][0],self.data['W_shape'][1],3)\
-				.clip(min=0,max=255).astype('uint8'))
-			self.imW=self.Wax2.imshow((self.data['W_pp']@self.cmap[:,:-1]*255/np.max(self.data['W_pp'])).\
-				reshape(self.data['W_shape'][0],self.data['W_shape'][1],3).clip(min=0,max=255).astype('uint8'))
-			self.imW.axes.set_aspect('equal')
-			self.imWH.axes.set_aspect('equal')
-			self.canvas_W.draw()
-			self.refresh_slider([])
-
-		if 'H_pp' in self.data:
-			Hstd=self.data['H_pp'].std()*3
-			if self.offsetH.get():
-				tmpH=self.data['H_pp'].T - repmat([w*Hstd for w in list(range(len(self.comps_to_show_arr)))],len(self.data['H_pp'].T),1)
-			else:
-				tmpH=self.data['H_pp'].T
-
-			self.Hax1.cla()
-			self.Hax1.set_title('Temporal Data (H)')
-			self.Hax1.plot(tmpH,linewidth=.5)
-			for i,j in enumerate(self.Hax1.lines):
-				j.set_color(self.cmap[i])
-			if not self.offsetH.get():
-				thresh_line=self.Hax1.plot(np.ones((len(self.data['H_pp'].T,)))*self.cfg['threshold'],linestyle='dashed',color='0',linewidth=1)
-				zero_line=self.Hax1.plot(np.zeros((len(self.data['H_pp'].T,))),linestyle='dashed',color='.5',linewidth=1)
-				self.legend=self.Hax1.legend((thresh_line[0],), ('Threshold',))
-			self.Hax1.set_xlim(0, len(self.data['H_pp'].T))
-			self.Hax1.set_ylim(np.min(tmpH), np.max(tmpH))
-			if self.offsetH.get():
-				self.Hax1.set(ylabel='Component #')
-			else:
-				self.Hax1.set(ylabel='Magnitude')
-
-			if self.audio_analog.get():
-				if len(self.data['H_pp'])>16:
-					self.audio_analog.set(0)
-					self.Hax2.imshow(self.data['H_fp'],interpolation='none',cmap=plt.get_cmap('gray'))
-					self.message('Error: Analog audio is currently limited to 16 components.')
-				else:
-					# I do not understand why I have to do it this way
-					tmp=self.Hax2.imshow(self.data['H_pp'],interpolation='none',cmap=plt.get_cmap('gray'))
-					tmp.set_clim(0, np.max(self.data['H_pp']))
-			else:
-				self.Hax2.imshow(self.data['H_fp'],interpolation='none',cmap=plt.get_cmap('gray'))
-
-			self.Hax2.xaxis.set_major_formatter(tkr.FuncFormatter(lambda x, pos: '{:.2g}'.format(x/self.cfg['fr'])))
-
-			if len(self.comps_to_show_arr) > 12:
-				yticks=np.arange(4,len(self.data['H_pp']),5)
-				yticklabels=np.arange(4,len(self.data['H_pp']),5)
-			else:
-				yticks=np.arange(0,len(self.data['H_pp']),1)
-				yticklabels=np.arange(0,len(self.data['H_pp']),1)
-
-			if self.offsetH.get():
-				self.Hax1.set(yticks=-yticks*Hstd,yticklabels=yticklabels)
-			self.Hax2.set(yticks=yticks,yticklabels=yticklabels)
-			self.Hax2.axes.set_aspect('auto')
-			self.canvas_H.draw()
-
-	def process_H_W(self):
-		'''
-		Core function of pyanthem. Applies all cfg settings to dataset, and 
-		creates the note dict used for synthesis. Automatically calls 
-		refresh_GUI() if display=True
-		'''
-		if self.display:
-			self.self_to_cfg()
-			self.message('Updating...')
-			self.update()
-		if self.cfg['comps_to_show']=='all':
-			self.comps_to_show_arr=list(range(len(self.data['H'])))
-		# regex expression which lazily checks for a bracketed expression containing numbers, colons and commas.
-		elif re.match('^\[[0-9,: ]*\]$',self.cfg['comps_to_show']) is not None:
-			# This is a magic function which transforms bracketed string arrays to actual numpy arrays.
-			# Example: '[1,3,5:8]' --> array([1,3,5,6,7])
-			self.comps_to_show_arr=eval('np.r_'+self.cfg['comps_to_show']) 
-		else:
-			self.message('For \'components to show\', please input indices with commas and colons enclosed by square brackets, or \'all\' for all components.')
-			return
-		
-		self.data['H_pp']=self.data['H'][self.comps_to_show_arr,int(len(self.data['H'].T)*self.cfg['start_percent']/100):int(len(self.data['H'].T)*self.cfg['end_percent']/100)]
-		self.data['H_pp']=self.data['H_pp']+self.cfg['baseline']
-		if 'W' in self.data:
-			self.data['W_pp']=self.data['W'][:,self.comps_to_show_arr]
-		
-		# make_keys()
-		self.keys,i=[],0
-		while len(self.keys) < len(self.data['H_pp']):
-			self.keys.extend([k+i+key_opts[self.cfg['key']]+octave_add_opts[self.cfg['octave_add']] for k in scale_keys[self.cfg['scale_type']]])
-			i+=12
-		self.keys=self.keys[:len(self.data['H_pp'])]
-		self.keys=[min(k,127) for k in self.keys] # Notes cannot be higher than 127
-
-		# Making note dict
-		true_fr=self.cfg['fr']*self.cfg['speed']/100
-		upsample=1000
-		ns=int(len(self.data['H_pp'].T)*upsample/true_fr)
-		t1=np.linspace(0,len(self.data['H_pp'].T)/self.cfg['fr'],len(self.data['H_pp'].T))
-		t2=np.linspace(0,len(self.data['H_pp'].T)/self.cfg['fr'],ns)
-		nchan=len(self.data['H_pp'])
-		Hmax=np.max(self.data['H_pp'])
-		self.data['H_fp']=np.zeros(np.shape(self.data['H_pp']))
-		self.data['H_pp'][self.data['H_pp'] < 0]=0
-		self.data['H_pp'][:,-1]=0
-		self.data['H_pp'][:,0]=0
-		self.nd=[]
-		for i in range(nchan):
-			H_rs=interp1d(t1,self.data['H_pp'][i,:])(t2)
-			H_b=H_rs.copy()
-			H_b[H_b<self.cfg['threshold']]=0
-			H_b[H_b>=self.cfg['threshold']]=1
-			TC=np.diff(H_b)
-			st=np.argwhere(TC==1)
-			en=np.argwhere(TC==-1)
-			st=np.ndarray.flatten(st).tolist()
-			en=np.ndarray.flatten(en).tolist()
-			for j in range(len(st)):
-				mag=np.max(H_rs[st[j]:en[j]])
-				self.data['H_fp'][i,int(st[j]*true_fr/upsample):int(en[j]*true_fr/upsample)]=mag
-				# Type, time, note, velocity
-				self.nd.append(['note_on',st[j],self.keys[i],int(mag * 127 / Hmax)])
-				self.nd.append(['note_off',en[j],self.keys[i],int(mag * 127 / Hmax)])
-			self.nd=sorted(self.nd, key=lambda x: x[1])
-		# Colormap
-		cmap=getattr(cmaps,self.cfg['cmapchoice'])
-		self.cmap=cmap(np.linspace(0,1,len(self.data['H_pp'])))
-		if self.display:
-			self.refresh_GUI()
-
-	def refresh_slider(self,event):
-		'''
-		Updates bottom left W plot with slider movement
-		'''
-		self.imWH.set_data((self.data['W_pp']@np.diag(self.data['H_pp'][:,int(self.frameslider.get())])@self.cmap[:,:-1]*(255/self.cfg['brightness'])).reshape(self.data['W_shape'][0],self.data['W_shape'][1],3).clip(min=0,max=255).astype('uint8'))
-		self.canvas_W.draw()
-
-	def preview_notes(self):
-		'''
-		Previews the self.keys list audibly and visually simultaneously.
-		'''
-		self.process_H_W()
-		self.message('Previewing notes...')
-		fn_font=os.path.join(os.path.dirname(os.path.abspath(__file__)),'anthem_soundfonts','font.sf2')
-		fn_midi=os.path.join(os.path.dirname(os.path.abspath(__file__)),'preview.mid')
-		fn_wav=os.path.join(os.path.dirname(os.path.abspath(__file__)),'preview.wav')
-		if get_init() is None: # Checks if pygame has initialized audio engine. Only needs to be run once per instance
-			pre_init(fs, -16, 2, 1024)
-			init()
-			set_num_channels(128) # We will never need more than 128...
-		mid=mido.MidiFile()
-		track=mido.MidiTrack()
-		mid.tracks.append(track)
-		mid.ticks_per_beat=1000
-		track.append(mido.MetaMessage('set_tempo', tempo=int(1e6)))
-		track.append(mido.Message('program_change', program=sound_presets[self.cfg['sound_preset']], time=0))
-		for i in range(len(self.keys)):
-			track.append(mido.Message('note_on', note=self.keys[i], velocity=100, time=250))
-			track.append(mido.Message('note_off', note=self.keys[i], time=250))
-		track.append(mido.Message('note_off', note=self.keys[i], time=500))
-		mid.save(fn_midi)
-		cmd='fluidsynth -ni {} -F {} -r {} {} {} '.format(self.cfg['fluidsynthextracommand'],fn_wav,fs,fn_font,fn_midi)
-		os.system(cmd)
-		music.load(fn_wav)
-		for i in range(len(self.keys)):
-			t=time.time()
-			if 'W' in self.data:
-				self.imW.remove()
-				Wtmp=self.data['W_pp'][:,i]
-				cmaptmp=self.cmap[i,:-1]
-				self.imW=self.Wax2.imshow((Wtmp[:,None]@cmaptmp[None,:]*255/np.max(self.data['W_pp'])).reshape(self.data['W_shape'][0],self.data['W_shape'][1],3).clip(min=0,max=255).astype('uint8'))
-				self.canvas_W.draw()
-				self.update()
-			if i==0:
-				music.play(0)
-			time.sleep(.5-np.min(((time.time()-t),.5)))
-		time.sleep(.5)
-		music.unload()
-		try:
-			os.remove(fn_midi)
-			os.remove(fn_wav)
-		except OSError as e:
-			print("Failed with:", e.strerror)
-		self.refresh_GUI()
-		
-	def write_audio(self):
-		'''
-		Writes audio either from .sf2 using fluidsynth or into raw file.
-		'''
-		if not self.check_data():
-			return
-		self.process_H_W()
-		fn_midi=os.path.join(self.cfg['save_path'],self.cfg['file_out'])+'.mid'
-		fn_wav=os.path.join(self.cfg['save_path'],self.cfg['file_out'])+'.wav'
-		fn_font=os.path.join(os.path.dirname(os.path.abspath(__file__)),'anthem_soundfonts','font.sf2')
-		mid=mido.MidiFile()
-		track=mido.MidiTrack()
-		mid.tracks.append(track)
-		mid.ticks_per_beat=1000
-		track.append(mido.MetaMessage('set_tempo', tempo=int(1e6)))
-		if not self.cfg['audio_analog']:
-			track.append(mido.Message('program_change', program=sound_presets[self.cfg['sound_preset']], time=0))
-			current_time=0
-			for i in range(len(self.nd)):
-				track.append(mido.Message(self.nd[i][0], time=int(self.nd[i][1]-current_time), note=self.nd[i][2], velocity=self.nd[i][3]))
-				current_time=self.nd[i][1]
-			mid.save(fn_midi)
-		else:
-			true_fr=self.cfg['fr']*self.cfg['speed']/100
-			upsample=100
-			ns=int(len(self.data['H_pp'].T)*upsample/true_fr)
-			t1=np.linspace(0,len(self.data['H_pp'].T)/self.cfg['fr'],len(self.data['H_pp'].T))
-			t2=np.linspace(0,len(self.data['H_pp'].T)/self.cfg['fr'],ns)
-			nchan=len(self.data['H_pp'])
-			Hmax=np.max(self.data['H_pp'])
-			H_rs=np.zeros((nchan,ns))
-			ticks=int(mid.ticks_per_beat/upsample)
-			for i in range(nchan):
-				H_rs[i,:]=interp1d(t1,self.data['H_pp'][i,:])(t2)
-			for chan in range(nchan):
-				track.append(mido.Message('program_change', channel=chan, program=sound_presets[self.cfg['sound_preset']], time=0))
-				track.append(mido.Message('note_on', channel=chan, note=self.keys[chan], time=0, velocity=127))
-				track.append(mido.Message('control_change', channel=chan, control=7, value=0, time=0))
-			for i in range(ns):
-				for chan in range(nchan):
-					if chan==0:
-						realticks=ticks
-					else:
-						realticks=0
-					track.append(mido.Message('control_change', channel=chan, control=7, value=int(H_rs[chan,i]*127/Hmax), time=realticks))
-			for chan in range(nchan):
-				track.append(mido.Message('note_off', channel=chan, note=self.keys[chan], time=0))
-			mid.save(fn_midi)
-		os.system('fluidsynth -ni {} -F {} -r {} {} {}'.format(self.cfg['fluidsynthextracommand'],fn_wav,fs,fn_font,fn_midi))
-		self.message(f'Audio file written to {self.cfg["save_path"]}')
-		return self
-
-	def write_video(self):
-		'''
-		Writes video file using self.data['H_pp'] and self.data['W_pp'] using ffmpeg. 
-		We avoid using opencv because it is very slow in a conda environment
-		http://zulko.github.io/blog/2013/09/27/read-and-write-video-frames-in-python-using-ffmpeg/
-		'''
-		if not self.check_data():
-			return
-		self.process_H_W()
-		fn_vid=os.path.join(self.cfg['save_path'],self.cfg['file_out'])+'.mp4'
-		v_shape=self.data['W_shape'][::-1][1:] # Reverse because ffmpeg does hxw
-		command=['ffmpeg',
-			'-loglevel', 'warning', # Prevents excessive messages
-			'-hide_banner',
-			'-y', # Auto overwrite
-			'-f', 'image2pipe',
-			'-vcodec','png',
-			'-s', '{}x{}'.format(v_shape[0],v_shape[1]),
-			'-r', str(self.cfg['fr']*self.cfg['speed']/100),
-			'-i', '-', # The input comes from a pipe
-			'-an', # Tells FFMPEG not to expect any audio
-			'-q:v','2', # Quality
-			'-vcodec', 'mpeg4',
-			'-preset', 'ultrafast',
-			fn_vid]
-		pipe=sp.Popen(command, stdin=sp.PIPE)
-		nframes=len(self.data['H_pp'].T)
-		t0 = time.time()
-		for i in range(nframes):
-			frame=(self.data['W_pp']@np.diag(self.data['H_pp'][:,i])@self.cmap[:,:-1]*(255/self.cfg['brightness'])).reshape(self.data['W_shape'][0],self.data['W_shape'][1],3).clip(min=0,max=255).astype('uint8')
-			im=Image.fromarray(frame)
-			im.save(pipe.stdin, 'PNG')
-			if self.display and i%20==1:
-				self.status['text']=f'Writing video file, {i} out of {nframes} frames written, avg fps: {i/(time.time()-t0)}'
-				self.update()
-			elif not self.display and i%20==1:
-				print(f'Writing video file, {i} out of {nframes} frames written, avg fps: {i/(time.time()-t0)}',end='\r')
-		pipe.stdin.close()
-		pipe.wait()
-		self.message(f'Video file written to {self.cfg["save_path"]}')
-		return self
-	
-	def merge(self):
-		'''
-		Merges video and audio with ffmpeg
-		'''
-		fn=os.path.join(self.cfg['save_path'],self.cfg['file_out'])
-		cmd='ffmpeg -hide_banner -loglevel warning -y -i {} -i {} -c:a aac -map 0:v:0 -map 1:a:0 {}'.format(fn+'.mp4',fn+'.wav',fn+'_AV.mp4')
-		os.system(cmd)
-		self.message(f'A/V file written to {self.cfg["save_path"]}')
-		return self
-	
-	def write_AV(self):
-		'''
-		Runs full write and merge
-		'''
-		self.write_video()
-		self.write_audio()
-		self.merge()
-		if not self.display:
-			return self
-
-	def cleanup(self):
-		'''
-		Tries to remove any files that are video or audio only.	
-		'''
-		fn=os.path.join(self.cfg['save_path'],self.cfg['file_out'])
-		try: 
-			os.remove(fn+'.mp4')
-		except OSError: 
-			pass
-		try: 
-			os.remove(fn+'.wav')
-		except OSError: 
-			pass
-		try: 
-			os.remove(fn+'.mid')
-		except OSError: 
-			pass
-		self.message(f'A/V only videos removed')
-		return self
-
-	def edit_save_path(self):
-		self.save_path.set(fd.askdirectory(title='Select a directory to save output files',initialdir=self.cfg['save_path']))
-
-	def initGUI(self):
-		'''
-		Initialize GUI fields, labels, dropdowns, etc.
-		'''
-		self.winfo_toplevel().title('pyanthem v{}'.format(pkg_resources.require("pyanthem")[0].version))
-		#photo = PhotoImage(file = os.path.join(os.path.dirname(os.path.abspath(__file__)),'logo.png'))
-		#self.iconphoto(False, photo)
-		self.protocol('WM_DELETE_WINDOW', self.quit)
-
-		# StringVars
-		self.file_in=init_entry(None)
-		self.file_out=init_entry(None)
-		self.save_path=init_entry(None)
-		self.speed=init_entry(100)
-		self.fr=init_entry(0)
-		self.start_percent=init_entry(0)
-		self.end_percent=init_entry(100)
-		self.baseline=init_entry(0)
-		self.brightness=init_entry(0)
-		self.threshold=init_entry(0)
-		self.octave_add=init_entry('2')
-		self.scale_type=init_entry('Maj. 7 (4/oct)')
-		self.key=init_entry('C')
-		self.sound_preset=init_entry('Piano')
-		self.comps_to_show=init_entry('all')
-		self.cmapchoice=init_entry('jet')
-		
-		self.fluidsynthextracommand = ''
-		#self.ffmpegextracommand = ''
-
-		# Labels
-		Label(text='',font='Helvetica 1 bold').grid(row=0,column=0) # Just to give a border around Seperators
-		Label(text='File Parameters',font='Helvetica 14 bold').grid(row=1,column=1,columnspan=2,sticky='WE')
-		Label(text='Movie Parameters',font='Helvetica 14 bold').grid(row=1,column=3,columnspan=2,sticky='WE')
-		Label(text='Audio Parameters',font='Helvetica 14 bold').grid(row=1,column=5,columnspan=2,sticky='WE')
-		Label(text='Input Filename').grid(row=2, column=1,columnspan=2,sticky='W')
-		Label(text='Output Filename').grid(row=4, column=1,columnspan=2,sticky='W')
-		Label(text='Save Path').grid(row=6, column=1,columnspan=1,sticky='W')
-		Label(text='Speed (%)').grid(row=2, column=3, sticky='E')
-		Label(text='Start (%)').grid(row=3, column=3, sticky='E')
-		Label(text='End (%)').grid(row=4, column=3, sticky='E')
-		Label(text='Baseline').grid(row=5, column=3, sticky='E')
-		Label(text='Max brightness').grid(row=6, column=3, sticky='E')
-		Label(text='Colormap').grid(row=7, column=3, sticky='E')
-		Label(text='Threshold').grid(row=2, column=5, sticky='E')
-		Label(text='Octave').grid(row=3, column=5, sticky='E')
-		Label(text='Scale Type').grid(row=4, column=5, sticky='E')
-		Label(text='Key').grid(row=5, column=5, sticky='E')
-		Label(text='Audio format').grid(row=6, column=5, sticky='E')
-
-		# Messages
-		self.status=Message(text='Welcome to pyanthem v{}!'.\
-			format(pkg_resources.require("pyanthem")[0].version),bg='white',fg='black',width=450)
-		self.status.grid(row=9, column=2, columnspan=5, sticky='NESW')
-		self.status['anchor']='nw'
-
-		# Entries
-		Entry(textvariable=self.file_in).grid(row=3, column=1,columnspan=2,sticky='W')
-		Entry(textvariable=self.file_out).grid(row=5, column=1,columnspan=2,sticky='W')
-		Entry(textvariable=self.save_path,width=17).grid(row=7, column=1,columnspan=2,sticky='EW')
-		Entry(textvariable=self.speed,width=7).grid(row=2, column=4, sticky='W')
-		Entry(textvariable=self.start_percent,width=7).grid(row=3, column=4, sticky='W')
-		Entry(textvariable=self.end_percent,width=7).grid(row=4, column=4, sticky='W')
-		Entry(textvariable=self.baseline,width=7).grid(row=5, column=4, sticky='W')
-		Entry(textvariable=self.brightness,width=7).grid(row=6, column=4, sticky='W')
-		self.threshold_entry=Entry(textvariable=self.threshold,width=7)
-		self.threshold_entry.grid(row=2, column=6, sticky='W')
-
-		# Styles
-		s = Style()
-		s.configure('my.TButton', font=('Helvetica', 14))
-
-		# Buttons
-		Button(text='Edit',command=self.edit_save_path,width=5).grid(row=6, column=2)
-		Button(text='Preview',width=11,command=self.preview_notes).grid(row=7, column=5,columnspan=1)
-		
-		self.update_button=Button(text='Update',width=7,command=self.process_H_W,style='my.TButton')
-		self.update_button.grid(row=9,column=1,columnspan=1)
-		
-		# Combo box
-		self.cmapchooser=Combobox(self,textvariable=self.cmapchoice,width=5)
-		self.cmapchooser['values']=cmaps_opts
-		self.cmapchooser['state']='readonly'
-		self.cmapchooser.grid(row=7, column=4, sticky='W')
-		self.cmapchooser.current()
-		self.cmap=[]
-
-		self.octave_add_menu=Combobox(self,textvariable=self.octave_add,width=7)
-		self.octave_add_menu['values']=tuple(octave_add_opts.keys())
-		self.octave_add_menu['state']='readonly'
-		self.octave_add_menu.grid(row=3, column=6, sticky='W')
-		self.octave_add_menu.current()
-
-		self.scale_type_menu=Combobox(self,textvariable=self.scale_type,width=11)
-		self.scale_type_menu['values']=tuple(scale_keys.keys())
-		self.scale_type_menu['state']='readonly'
-		self.scale_type_menu.grid(row=4, column=6, sticky='W')
-		self.scale_type_menu.current()
-
-		self.key_menu=Combobox(self,textvariable=self.key,width=7)
-		self.key_menu['values']=tuple(key_opts.keys())
-		self.key_menu['state']='readonly'
-		self.key_menu.grid(row=5, column=6, sticky='W')
-		self.key_menu.current()
-
-		self.sound_preset_menu=Combobox(self,textvariable=self.sound_preset,width=7)
-		self.sound_preset_menu['values']=tuple(sound_presets.keys())
-		self.sound_preset_menu['state']='readonly'
-		self.sound_preset_menu.grid(row=6, column=6, sticky='W')
-		self.sound_preset_menu.current()
-
-		# Checkbox
-		self.audio_analog=IntVar()
-		self.audio_analog.set(0)
-		Checkbutton(self, text="Analog",command=self.process_H_W,variable=self.audio_analog).grid(row=7, column=6,columnspan=1)
-
-		# Menu bar
-		menubar=Menu(self)
-		filemenu=Menu(menubar, tearoff=0)
-		filemenu.add_command(label="Load data...", command=self.load_GUI)
-		filemenu.add_command(label="Load config...", command=self.load_config)
-		filemenu.add_command(label="Quit",command=self.quit,accelerator="Ctrl+Q")
-
-		savemenu=Menu(menubar, tearoff=0)
-		savemenu.add_command(label="Audio", command=self.write_audio)
-		savemenu.add_command(label="Video", command=self.write_video)
-		savemenu.add_command(label="Config", command=self.dump_cfg)
-		savemenu.add_command(label="Merge A/V", command=self.merge)
-		savemenu.add_command(label="Write A/V then merge", command=self.write_AV)
-		savemenu.add_command(label="Cleanup", command=self.cleanup)
-
-		advancedmenu=Menu(menubar, tearoff=0)
-		advancedmenu.add_command(label="Custom fluidsynth params", command=self.fluidsynthextra)
-		#advancedmenu.add_command(label="Custom ffmpeg params", command=self.ffmpegextra)
-		advancedmenu.add_command(label="View config", command=self.view_cfg)
-
-		menubar.add_cascade(label="File", menu=filemenu)
-		menubar.add_cascade(label="Save", menu=savemenu)
-		menubar.add_cascade(label="Advanced", menu=advancedmenu)
-		self.config(menu=menubar)
-
-		# Seperators
-		s_v=[[0,1,9],[2,1,8],[4,1,8],[6,1,9]]
-		s_h=[[1,1,6],[1,2,6],[1,9,6],[1,10,6],[1,4,2],[1,6,2]]
-		for sv in s_v:
-			Separator(self, orient='vertical').grid(column=sv[0], row=sv[1], rowspan=sv[2], sticky='nse')
-		for sh in s_h:
-			Separator(self, orient='horizontal').grid(column=sh[0], row=sh[1], columnspan=sh[2], sticky='nwe')
-
-		# Offset
-		self.offsetH=IntVar()
-		self.offsetH.set(1)
-
-		# Bind shortcuts
-		self.bind_all("<Control-q>", self.quit)
-		self.bind_all("<Control-a>", lambda:[self.process_H_W(),self.refresh_GUI()])
-
-	def init_plots(self):
-		'''
-		Initializes the plot areas. Is called every time update_GUI() is called.
-		'''
-		# H
-		if 'H_pp' in self.data:
-			self.figH=plt.Figure(figsize=(7,6), dpi=100, tight_layout=True)
-			self.Hax1=self.figH.add_subplot(211)
-			self.Hax2=self.figH.add_subplot(212)
-			self.Hax2.set_title('Audio Preview')
-			self.canvas_H=FigureCanvasTkAgg(self.figH, master=self)
-			self.canvas_H.get_tk_widget().grid(row=1,column=7,rowspan=30,columnspan=10)
-			bg=self.status.winfo_rgb(self['bg'])
-			self.figH.set_facecolor([(x>>8)/255 for x in bg])
-			self.Hax1.spines['left'].set_visible(False)
-			self.Hax1.spines['top'].set_visible(False)
-			self.Hax1.spines['bottom'].set_visible(False)
-			self.Hax1.spines['right'].set_visible(False)
-			self.Hax1.yaxis.tick_right()
-			self.Hax1.yaxis.set_label_position('right')
-			self.Hax1.tick_params(axis='x',which='both',bottom=False, top=False, labelbottom=False, right=False)
-			self.Hax2.set(xlabel='time (sec)',ylabel='Component #')
-			self.Hax2.spines['left'].set_visible(False)
-			self.Hax2.spines['top'].set_visible(False)
-			self.Hax2.spines['bottom'].set_visible(False)
-			self.Hax2.spines['right'].set_visible(False)
-			self.Hax2.yaxis.tick_right()
-			self.Hax2.yaxis.set_label_position('right')
-			# Checkbox
-			Checkbutton(self, text="Offset H",command=self.refresh_GUI,variable=self.offsetH).grid(row=1,rowspan=1,column=16)
-		
-		try: 
-			# If user previously loaded dataset with W, clear those 
-			# plots and remove associated GUI elements.
-			self.figW.clear()
-			self.canvas_W.draw()
-			self.frameslider.grid_forget()
-			self.comps_to_show_label.grid_forget()
-			self.comps_to_show_entry.grid_forget()
-		except:
-			pass
-
-		if 'W_pp' in self.data:
-			self.figW=plt.Figure(figsize=(6,3), dpi=100, constrained_layout=True)
-			self.Wax1=self.figW.add_subplot(121)
-			self.Wax2=self.figW.add_subplot(122)
-			self.Wax1.set_title('Video Preview')
-			self.Wax2.set_title('Spatial Data (W)')
-			self.Wax1.axis('off')
-			self.Wax2.axis('off')
-			self.canvas_W=FigureCanvasTkAgg(self.figW, master=self)
-			self.canvas_W.get_tk_widget().grid(row=11,column=1,rowspan=19,columnspan=6)
-			self.figW.set_facecolor([(x>>8)/255 for x in bg])
-			
-			# Frameslider
-			# frameslider
-			self.frameslider=Scale(self, from_=1, to=2, orient=HORIZONTAL)
-			self.frameslider.set(1)
-			self.frameslider['command']=self.refresh_slider
-			self.frameslider.grid(row=30, column=1, columnspan=3,sticky='EW')
-			
-		# comps_to_show
-		self.comps_to_show_label=Label(text='Components:')
-		self.comps_to_show_label.grid(row=30, column=5, columnspan=1, sticky='E')
-		self.comps_to_show_entry=Entry(textvariable=self.comps_to_show,width=15,justify='center')
-		self.comps_to_show_entry.grid(row=30, column=6, columnspan=1,sticky='W')
-		
-	def process_raw(self,data=None,n_clusters=None,frame_rate=None,save=False,file_in=None):
-		'''
-		Decomposes raw dataset. Can be used in two ways: as a part of the 
-		GUI class for immediate processing (e.g. process_raw().write_AV()),
-		or as a method to save a new dataset. 
-		'''
-		sh=data.shape
-		if len(sh) != 3:
-			self.message('ERROR: input dataset is not 3D.')
-			return
-		data=data.reshape(sh[0]*sh[1],sh[2])
-		# Ignore rows with any nans
-		nanidx=np.any(np.isnan(data), axis=1)
-		data_nn=data[~nanidx] # nn=non-nan
-		# k-means
-		print('Performing k-means...',end='')
-		if n_clusters is None:
-			# Default k is the 4th root of the number of samples per frame (for 256x256, this would be 16)
-			n_clusters=int(len(data)**.25) 
-			print(f'No num_clusters given. Defaulting to {n_clusters}...',end='')
-		idx_nn=KMeans(n_clusters=n_clusters, random_state=0).fit(data_nn).labels_
-		idx=np.zeros((len(data),))
-		idx[nanidx==False]=idx_nn
-		# TCs
-		H=np.zeros((n_clusters,len(data.T)))
-		for i in range(n_clusters):
-			H[i,:]=np.nanmean(data[idx==i,:],axis=0)
-		print('done.')
-		# NNLS
-		nnidx=np.where(~nanidx)[0]
-		W=np.zeros((len(data),n_clusters))
-		print('Performing NNLS...',end='')
-		for i in range(len(nnidx)):
-			W[nnidx[i],:]=nnls(H.T,data_nn[i,:])[0]
-		# Sort bottom to top
-		xc,yc=[],[]
-		(X,Y)=np.meshgrid(range(sh[1]),range(sh[0]))
-		for i in range(len(W.T)):
-			Wtmp=W[:,i].reshape(sh[0],sh[1])
-			xc.append((X*Wtmp).sum() / Wtmp.sum().astype("float"))
-			yc.append((Y*Wtmp).sum() / Wtmp.sum().astype("float"))
-		I=np.argsort(yc[::-1]) # Reverse orders from bottom to top
-		W,H=W[:,I],H[I,:]
-		print('done.')
-		
-		# Assign variables and save
-		self.data={}
-		self.data['H']=H
-		self.data['W']=W.reshape(sh[0],sh[1],n_clusters)
-		#self.data['W_shape']=self.data['W'].shape.flatten()
-		if frame_rate==[]:
-			self.data['fr']=10
-			print('No fr given. Defaulting to 10')
-		else:
-			self.data['fr']=frame_rate
-		if save:
-			if file_in is None:
-				file_in='data.mat'
-			fn=file_in.replace('.mat','_decomp.mat')
-			savemat(fn,self.data)
-			self.message(f'Decomposed data file saved to {fn}')
-		
-		# Reshape W here, since any use of self from here would require a flattened W
-		self.data['W']=self.data['W'].reshape(self.data['W'].shape[0]*self.data['W'].shape[1],self.data['W'].shape[2])
-		return self
-
-	def fluidsynthextra(self):
-		self.fluidsynthextracommand=sd.askstring('Input custom fluidsynth parameters here','',initialvalue=self.fluidsynthextracommand,parent=self)
-
-	#def ffmpegextra(self):
-#		self.ffmpegextracommand=sd.askstring('Input custom ffmpeg parameters here','',initialvalue=self.ffmpegextracommand,parent=self)
-
-	def view_cfg(self):
-		'''
-		Prints cfg info to command line
-		'''
-		try:
-			for key in self.cfg:
-				print(str(key)+': '+str(self.cfg[key]))
-		except:
-			pass
-		
-	def help(self):
-		print('To load a dataset:\npyanthem.load_data()\n\nTo load a cfg file:\npyanthem.load_config()\n\nTo write video:\npyanthem.write_video()\n\nTo write audio:\npyanthem.write_audio()')
-
-if __name__=="__main__":
-	run()
-
-# self\.([a-z_]{1,14})\.get\(\)
-# self\.cfg\[$1\]
+import os, random, sys, time, csv, pickle, re, pkg_resources, mido, h5py
+os.environ['PYGAME_HIDE_SUPPORT_PROMPT']="hide"
+from tkinter import *
+from tkinter.ttk import *
+from tkinter import filedialog as fd 
+from tkinter import simpledialog as sd 
+from ttkthemes import ThemedTk
+from scipy.io import loadmat, savemat, whosmat
+from scipy.optimize import nnls
+from scipy.interpolate import interp1d
+from scipy.io.wavfile import write as wavwrite
+from sklearn.cluster import KMeans
+from pygame.mixer import init, quit, get_init, set_num_channels, pre_init, music
+import matplotlib.pyplot as plt
+from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
+import matplotlib.ticker as tkr
+import matplotlib.cm as cmaps # https://matplotlib.org/gallery/color/colormap_reference.html
+import numpy as np
+from numpy.matlib import repmat
+try:
+	from pyanthem.pyanthem_vars import *
+except:
+	from pyanthem_vars import *
+import gdown
+import subprocess as sp
+import PIL.Image as Image
+
+def init_entry(fn):
+	'''
+	Generalized version of StringVar/DoubleVar followed by set()
+	'''
+	if isinstance(fn, str) or fn is None:
+		entry=StringVar()
+	else:
+		entry=DoubleVar()
+	entry.set(fn)
+	return entry
+
+def stack_files(files,fmts,fn):
+	'''
+	Stacks .mp4 videos horizontally, and merges wav files
+	the fmts argument is a list of three possible formats: 'a', 'v', or 'av'
+	Videos must match in height.
+	'''
+	nv=len([fmt for fmt in fmts if 'v' in fmt])
+	na=len([fmt for fmt in fmts if 'a' in fmt])
+	vf=[i for i,fmt in enumerate(fmts) if 'v' in fmt]
+	af=[i for i,fmt in enumerate(fmts) if 'a' in fmt]
+
+	# 3 cases: 1) Videos and audio, 2) Only videos, 3) Only audio
+	filter_command='"'
+	map_command=''
+
+	if nv > 1:
+		for v in vf:
+			filter_command+='[{}:v]'.format(v)
+		filter_command+='hstack=inputs={}[v]'.format(nv)
+		map_command+=' -map "[v]" '
+	elif nv == 1:
+		map_command += '-c:v copy -map {}:v:0'.format(vf[0])
+	
+	if na > 1:
+		# Seperate complex filters if video is being merged
+		if nv > 1:
+			filter_command+=';'
+		for a in af:
+			filter_command+='[{}:a]'.format(a)
+		filter_command+='amerge=inputs={}[a]'.format(na)
+		map_command+=' -map "[a]" '
+	elif na == 1:
+		map_command += ' -c:a aac -map {}:a:0 '.format(af[0])
+		
+	filter_command+='"'
+	in_command=''
+	for i in range(len(files)):
+		in_command += ' -i '+files[i]
+	full_command = 'ffmpeg -y '+in_command+' -filter_complex '+filter_command+' '+map_command+' -ac 2 -vsync 0 '+fn
+	print(full_command)
+	os.system(full_command)
+
+def uiopen(title,filetypes):
+	'''
+	Simple uiopen GUI instance.
+	'''
+	root=Tk()
+	root.withdraw()
+	file_in=os.path.normpath(fd.askopenfilename(title=title,filetypes=filetypes))
+	root.update()
+	root.destroy()
+	return file_in
+
+def run(display=True):
+	'''
+	Main command to run GUI or CLI
+	'''
+	root=GUI(display=display)
+	sys.ps1='♫ '
+	if display:
+		root.mainloop()
+	else:
+		print('Welcome to pyanthem v{}!'.format(pkg_resources.require('pyanthem')[0].version))
+		return root
+
+class GUI(ThemedTk):
+	def __init__(self,display=True):
+		'''
+		Initializes the GUI instance. display=True runs the Tk.__init__(self)
+		command, while display=False skips that and visual initialization, keeping
+		the GUI 'hidden'
+		'''
+		self.display=display
+		self.sf_path=os.path.join(os.path.dirname(os.path.abspath(__file__)),'anthem_soundfonts')
+		if not os.path.isdir(self.sf_path):
+			print('Initializing soundfont library...')
+			os.mkdir(self.sf_path)
+			gdown.download('https://drive.google.com/uc?id={}'.format(sound_font),
+				os.path.join(os.path.join(os.path.dirname(os.path.abspath(__file__)),'anthem_soundfonts'),'font.sf2'),quiet=False)
+		if self.display:
+			ThemedTk.__init__(self)
+			self.set_theme('clearlooks')
+			self.initGUI()
+	
+	def quit(self,event=None):
+		'''
+		Quits the GUI instance. Currently, jupyter instances are kinda buggy
+		'''
+		try:
+			# This raises a NameError exception in a notebook env, since 
+			# sys.exit() is not an appropriate method
+			get_ipython().__class__.__name__ 
+			self.destroy()
+		except NameError:
+			sys.exit()
+
+	def message(self,msg):
+		'''
+		Sends message through print if no GUI, through self.status if GUI is running
+		'''
+		if self.display:
+			self.status['text']=msg
+		else:
+			print(msg)
+
+	def check_data(self):
+		'''
+		Checks to make sure data is loaded.
+		'''
+		if hasattr(self,'data') and self.cfg['save_path'] is not None:
+			return True
+		else:
+			self.message('Error: No dataset has been loaded or save_path is empty.')
+			return False
+	
+	def self_to_cfg(self):
+		'''
+		This function is necessary to allow command-line access of the GUI functions. 
+		StringVar() and IntVar() allow for dynamic, quick field updating and access, 
+		but cannot be used outside of a mainloop or be pickled. for this reason, I convert 
+		all StringVars and IntVars to a new dict called 'self.cfg', that can be accessed 
+		oustide the GUI and dumped to a pickle file, which essentially "saves" the GUI.
+		'''
+		self.cfg={k: getattr(self,k).get() if self_fns[k] is 'entry' else getattr(self,k) for k in self_fns}
+
+	def dump_cfg(self):
+		'''
+		Saves config file.
+		'''
+		file_out=os.path.join(self.cfg['save_path'],self.cfg['file_out'])+'_cfg.p'
+		pickle.dump(self.cfg,open(file_out, "wb"))
+		self.message(f'cfg file saved to {file_out}')
+	
+	def load_data(self,filein=None):
+		'''
+		Loads dataset from filein. At the time, only supports .mat files.
+		'''
+		if filein is None:
+			filein=uiopen(title='Select mat or hdf5 file for import',filetypes=[('.mat files','*.mat'),('hdf5 files','*.h5'),('hdf5 files','*.hdf5')])
+		if filein=='.':
+			return
+		if filein.endswith('.mat'):
+			data_unk,var=loadmat(filein),whosmat(filein)
+			var = [v[0] for v in var]
+		elif filein.endswith('.hdf5') or filein.endswith('.h5'):
+			data_unk=h5py.File(filein, 'r')
+			var = data_unk.keys
+		data = {}
+		for k in var:
+			print()
+			tmp_var = np.asarray(data_unk[k])
+			if k in ('__header__', '__version__', '__globals__'):
+				continue
+			elif len(tmp_var.flatten())==1:
+				data['fr']=float(tmp_var)
+			elif tmp_var.ndim==2:
+				data['H']=tmp_var
+			elif tmp_var.ndim==3:
+				data['W']=tmp_var
+		# Checks inner dimension match if both H and W present in file.
+		if ('H' in data and 'W' in data) and data['H'].shape[0] != data['W'].shape[-1]:
+			# try flipping dims
+			if ('H' in data and 'W' in data) and data['H'].T.shape[0] == data['W'].T.shape[-1]:
+				data['H'] = data['H'].T
+				data['W'] = data['W'].T
+			else:
+				self.message('Error: Inner or outer dimensions of W [shape={}] and H [shape={}] do not match!'.format(data['H'].shape, data['W'].shape))
+				return
+		if 'H' in data:
+			if 'W' in data:
+				data['W_shape']=data['W'].shape
+				data['W']=data['W'].reshape(data['W'].shape[0]*data['W'].shape[1],data['W'].shape[2])
+			if 'fr' not in data:
+				data['fr']=data['H'].shape[1]/60 # Forces length to be 1 minute!
+			self.data=data
+			if not self.display:
+				return self
+		else:
+			self.message('Error: .mat file incompatible. Please select a .mat file with three variables: W (3D), H (2D), and fr (1-element float)')
+
+	def load_GUI(self):
+		'''
+		GUI-addons for load_data. Prompts user with filedialog, assigns defaults and sets GUI fields. 
+		'''
+		filein=uiopen(title='Select mat or hdf5 file for import',filetypes=[('.mat files','*.mat'),('hdf5 files','*.h5'),('hdf5 files','*.hdf5')])
+		if filein=='.':
+			return
+		self.load_data(filein)
+		if not hasattr(self,'data'):
+			return
+		self.data['H_pp']=self.data['H']
+		self.data['H_fp']=self.data['H']
+		self.fr.set(self.data['fr'])
+		if 'W' in self.data:
+			self.data['W_pp']=self.data['W']
+		self.file_in.set(os.path.splitext(os.path.split(filein)[1])[0])
+
+		# Set some defaults
+		self.file_out.set(self.file_in.get())
+		self.save_path.set(os.path.split(filein)[0])
+		Hstr='H' # for whatever reason, can't double nest quotations in an f-string :/
+		self.brightness.set(f'{float(f"{np.mean(self.data[Hstr])+np.std(self.data[Hstr]):.3g}"):g}')
+		self.threshold.set(f'{float(f"{np.mean(self.data[Hstr])+np.std(self.data[Hstr]):.3g}"):g}')
+		self.comps_to_show_arr=list(range(len(self.data['H'])))
+		self.init_plots()
+		self.process_H_W()
+	
+	def load_config(self,filein=None):
+		'''
+		Loads .p file containing dict of parameters needed to create outputs. If display=True, sets GUI fields.
+		'''
+		if filein is None:
+			filein=uiopen(title='Select pickle file for import',filetypes=[('pickle file','*.p'),('pickle file','*.pkl'),('pickle file','*.pickle')])
+		if filein=='.':
+			return
+		with open(filein, "rb") as f:
+			self.cfg=pickle.load(f)
+			if self.display:
+				for key,value in self.cfg.items():
+					if self_fns[key] is 'entry':
+						getattr(self,key).set(value)
+					else:
+						setattr(self,key,value)
+				self.refresh_GUI()
+			else:
+				return self
+
+	def refresh_GUI(self,event=None):
+		#self.init_plots()
+		if 'W_pp' in self.data:
+			if self.frameslider.get() > len(self.data['H_pp'].T): # This (usually) occurs when the user crops the dataset
+				self.frameslider.set(1)
+			self.frameslider['to']=int(len(self.data['H_pp'].T)-1)
+			self.imWH=self.Wax1.imshow((self.data['W_pp']@np.diag(self.data['H_pp'][:,int(self.frameslider.get())])@\
+				self.cmap[:,:-1]*(255/self.cfg['brightness'])).reshape(self.data['W_shape'][0],self.data['W_shape'][1],3)\
+				.clip(min=0,max=255).astype('uint8'))
+			self.imW=self.Wax2.imshow((self.data['W_pp']@self.cmap[:,:-1]*255/np.max(self.data['W_pp'])).\
+				reshape(self.data['W_shape'][0],self.data['W_shape'][1],3).clip(min=0,max=255).astype('uint8'))
+			self.imW.axes.set_aspect('equal')
+			self.imWH.axes.set_aspect('equal')
+			self.canvas_W.draw()
+			self.refresh_slider([])
+
+		if 'H_pp' in self.data:
+			Hstd=self.data['H_pp'].std()*3
+			if self.offsetH.get():
+				tmpH=self.data['H_pp'].T - repmat([w*Hstd for w in list(range(len(self.comps_to_show_arr)))],len(self.data['H_pp'].T),1)
+			else:
+				tmpH=self.data['H_pp'].T
+
+			self.Hax1.cla()
+			self.Hax1.set_title('Temporal Data (H)')
+			self.Hax1.plot(tmpH,linewidth=.5)
+			for i,j in enumerate(self.Hax1.lines):
+				j.set_color(self.cmap[i])
+			if not self.offsetH.get():
+				thresh_line=self.Hax1.plot(np.ones((len(self.data['H_pp'].T,)))*self.cfg['threshold'],linestyle='dashed',color='0',linewidth=1)
+				zero_line=self.Hax1.plot(np.zeros((len(self.data['H_pp'].T,))),linestyle='dashed',color='.5',linewidth=1)
+				self.legend=self.Hax1.legend((thresh_line[0],), ('Threshold',))
+			self.Hax1.set_xlim(0, len(self.data['H_pp'].T))
+			self.Hax1.set_ylim(np.min(tmpH), np.max(tmpH))
+			if self.offsetH.get():
+				self.Hax1.set(ylabel='Component #')
+			else:
+				self.Hax1.set(ylabel='Magnitude')
+
+			if self.audio_analog.get():
+				if len(self.data['H_pp'])>16:
+					self.audio_analog.set(0)
+					self.Hax2.imshow(self.data['H_fp'],interpolation='none',cmap=plt.get_cmap('gray'))
+					self.message('Error: Analog audio is currently limited to 16 components.')
+				else:
+					# I do not understand why I have to do it this way
+					tmp=self.Hax2.imshow(self.data['H_pp'],interpolation='none',cmap=plt.get_cmap('gray'))
+					tmp.set_clim(0, np.max(self.data['H_pp']))
+			else:
+				self.Hax2.imshow(self.data['H_fp'],interpolation='none',cmap=plt.get_cmap('gray'))
+
+			self.Hax2.xaxis.set_major_formatter(tkr.FuncFormatter(lambda x, pos: '{:.2g}'.format(x/self.cfg['fr'])))
+
+			if len(self.comps_to_show_arr) > 12:
+				yticks=np.arange(4,len(self.data['H_pp']),5)
+				yticklabels=np.arange(4,len(self.data['H_pp']),5)
+			else:
+				yticks=np.arange(0,len(self.data['H_pp']),1)
+				yticklabels=np.arange(0,len(self.data['H_pp']),1)
+
+			if self.offsetH.get():
+				self.Hax1.set(yticks=-yticks*Hstd,yticklabels=yticklabels)
+			self.Hax2.set(yticks=yticks,yticklabels=yticklabels)
+			self.Hax2.axes.set_aspect('auto')
+			self.canvas_H.draw()
+
+	def process_H_W(self):
+		'''
+		Core function of pyanthem. Applies all cfg settings to dataset, and 
+		creates the note dict used for synthesis. Automatically calls 
+		refresh_GUI() if display=True
+		'''
+		if self.display:
+			self.self_to_cfg()
+			self.message('Updating...')
+			self.update()
+		if self.cfg['comps_to_show']=='all':
+			self.comps_to_show_arr=list(range(len(self.data['H'])))
+		# regex expression which lazily checks for a bracketed expression containing numbers, colons and commas.
+		elif re.match('^\[[0-9,: ]*\]$',self.cfg['comps_to_show']) is not None:
+			# This is a magic function which transforms bracketed string arrays to actual numpy arrays.
+			# Example: '[1,3,5:8]' --> array([1,3,5,6,7])
+			self.comps_to_show_arr=eval('np.r_'+self.cfg['comps_to_show']) 
+		else:
+			self.message('For \'components to show\', please input indices with commas and colons enclosed by square brackets, or \'all\' for all components.')
+			return
+		
+		self.data['H_pp']=self.data['H'][self.comps_to_show_arr,int(len(self.data['H'].T)*self.cfg['start_percent']/100):int(len(self.data['H'].T)*self.cfg['end_percent']/100)]
+		self.data['H_pp']=self.data['H_pp']+self.cfg['baseline']
+		if 'W' in self.data:
+			self.data['W_pp']=self.data['W'][:,self.comps_to_show_arr]
+		
+		# make_keys()
+		self.keys,i=[],0
+		while len(self.keys) < len(self.data['H_pp']):
+			self.keys.extend([k+i+key_opts[self.cfg['key']]+octave_add_opts[self.cfg['octave_add']] for k in scale_keys[self.cfg['scale_type']]])
+			i+=12
+		self.keys=self.keys[:len(self.data['H_pp'])]
+		self.keys=[min(k,127) for k in self.keys] # Notes cannot be higher than 127
+
+		# Making note dict
+		true_fr=self.cfg['fr']*self.cfg['speed']/100
+		upsample=1000
+		ns=int(len(self.data['H_pp'].T)*upsample/true_fr)
+		t1=np.linspace(0,len(self.data['H_pp'].T)/self.cfg['fr'],len(self.data['H_pp'].T))
+		t2=np.linspace(0,len(self.data['H_pp'].T)/self.cfg['fr'],ns)
+		nchan=len(self.data['H_pp'])
+		Hmax=np.max(self.data['H_pp'])
+		self.data['H_fp']=np.zeros(np.shape(self.data['H_pp']))
+		self.data['H_pp'][self.data['H_pp'] < 0]=0
+		self.data['H_pp'][:,-1]=0
+		self.data['H_pp'][:,0]=0
+		self.nd=[]
+		for i in range(nchan):
+			H_rs=interp1d(t1,self.data['H_pp'][i,:])(t2)
+			H_b=H_rs.copy()
+			H_b[H_b<self.cfg['threshold']]=0
+			H_b[H_b>=self.cfg['threshold']]=1
+			TC=np.diff(H_b)
+			st=np.argwhere(TC==1)
+			en=np.argwhere(TC==-1)
+			st=np.ndarray.flatten(st).tolist()
+			en=np.ndarray.flatten(en).tolist()
+			for j in range(len(st)):
+				mag=np.max(H_rs[st[j]:en[j]])
+				self.data['H_fp'][i,int(st[j]*true_fr/upsample):int(en[j]*true_fr/upsample)]=mag
+				# Type, time, note, velocity
+				self.nd.append(['note_on',st[j],self.keys[i],int(mag * 127 / Hmax)])
+				self.nd.append(['note_off',en[j],self.keys[i],int(mag * 127 / Hmax)])
+			self.nd=sorted(self.nd, key=lambda x: x[1])
+		# Colormap
+		cmap=getattr(cmaps,self.cfg['cmapchoice'])
+		self.cmap=cmap(np.linspace(0,1,len(self.data['H_pp'])))
+		if self.display:
+			self.refresh_GUI()
+
+	def refresh_slider(self,event):
+		'''
+		Updates bottom left W plot with slider movement
+		'''
+		self.imWH.set_data((self.data['W_pp']@np.diag(self.data['H_pp'][:,int(self.frameslider.get())])@self.cmap[:,:-1]*(255/self.cfg['brightness'])).reshape(self.data['W_shape'][0],self.data['W_shape'][1],3).clip(min=0,max=255).astype('uint8'))
+		self.canvas_W.draw()
+
+	def preview_notes(self):
+		'''
+		Previews the self.keys list audibly and visually simultaneously.
+		'''
+		self.process_H_W()
+		self.message('Previewing notes...')
+		fn_font=os.path.join(os.path.dirname(os.path.abspath(__file__)),'anthem_soundfonts','font.sf2')
+		fn_midi=os.path.join(os.path.dirname(os.path.abspath(__file__)),'preview.mid')
+		fn_wav=os.path.join(os.path.dirname(os.path.abspath(__file__)),'preview.wav')
+		if get_init() is None: # Checks if pygame has initialized audio engine. Only needs to be run once per instance
+			pre_init(fs, -16, 2, 1024)
+			init()
+			set_num_channels(128) # We will never need more than 128...
+		mid=mido.MidiFile()
+		track=mido.MidiTrack()
+		mid.tracks.append(track)
+		mid.ticks_per_beat=1000
+		track.append(mido.MetaMessage('set_tempo', tempo=int(1e6)))
+		track.append(mido.Message('program_change', program=sound_presets[self.cfg['sound_preset']], time=0))
+		for i in range(len(self.keys)):
+			track.append(mido.Message('note_on', note=self.keys[i], velocity=100, time=250))
+			track.append(mido.Message('note_off', note=self.keys[i], time=250))
+		track.append(mido.Message('note_off', note=self.keys[i], time=500))
+		mid.save(fn_midi)
+		cmd='fluidsynth -ni {} -F {} -r {} {} {} '.format(self.cfg['fluidsynthextracommand'],fn_wav,fs,fn_font,fn_midi)
+		os.system(cmd)
+		music.load(fn_wav)
+		for i in range(len(self.keys)):
+			t=time.time()
+			if 'W' in self.data:
+				self.imW.remove()
+				Wtmp=self.data['W_pp'][:,i]
+				cmaptmp=self.cmap[i,:-1]
+				self.imW=self.Wax2.imshow((Wtmp[:,None]@cmaptmp[None,:]*255/np.max(self.data['W_pp'])).reshape(self.data['W_shape'][0],self.data['W_shape'][1],3).clip(min=0,max=255).astype('uint8'))
+				self.canvas_W.draw()
+				self.update()
+			if i==0:
+				music.play(0)
+			time.sleep(.5-np.min(((time.time()-t),.5)))
+		time.sleep(.5)
+		music.unload()
+		try:
+			os.remove(fn_midi)
+			os.remove(fn_wav)
+		except OSError as e:
+			print("Failed with:", e.strerror)
+		self.refresh_GUI()
+		
+	def write_audio(self):
+		'''
+		Writes audio either from .sf2 using fluidsynth or into raw file.
+		'''
+		if not self.check_data():
+			return
+		self.process_H_W()
+		fn_midi=os.path.join(self.cfg['save_path'],self.cfg['file_out'])+'.mid'
+		fn_wav=os.path.join(self.cfg['save_path'],self.cfg['file_out'])+'.wav'
+		fn_font=os.path.join(os.path.dirname(os.path.abspath(__file__)),'anthem_soundfonts','font.sf2')
+		mid=mido.MidiFile()
+		track=mido.MidiTrack()
+		mid.tracks.append(track)
+		mid.ticks_per_beat=1000
+		track.append(mido.MetaMessage('set_tempo', tempo=int(1e6)))
+		if not self.cfg['audio_analog']:
+			track.append(mido.Message('program_change', program=sound_presets[self.cfg['sound_preset']], time=0))
+			current_time=0
+			for i in range(len(self.nd)):
+				track.append(mido.Message(self.nd[i][0], time=int(self.nd[i][1]-current_time), note=self.nd[i][2], velocity=self.nd[i][3]))
+				current_time=self.nd[i][1]
+			mid.save(fn_midi)
+		else:
+			true_fr=self.cfg['fr']*self.cfg['speed']/100
+			upsample=100
+			ns=int(len(self.data['H_pp'].T)*upsample/true_fr)
+			t1=np.linspace(0,len(self.data['H_pp'].T)/self.cfg['fr'],len(self.data['H_pp'].T))
+			t2=np.linspace(0,len(self.data['H_pp'].T)/self.cfg['fr'],ns)
+			nchan=len(self.data['H_pp'])
+			Hmax=np.max(self.data['H_pp'])
+			H_rs=np.zeros((nchan,ns))
+			ticks=int(mid.ticks_per_beat/upsample)
+			for i in range(nchan):
+				H_rs[i,:]=interp1d(t1,self.data['H_pp'][i,:])(t2)
+			for chan in range(nchan):
+				track.append(mido.Message('program_change', channel=chan, program=sound_presets[self.cfg['sound_preset']], time=0))
+				track.append(mido.Message('note_on', channel=chan, note=self.keys[chan], time=0, velocity=127))
+				track.append(mido.Message('control_change', channel=chan, control=7, value=0, time=0))
+			for i in range(ns):
+				for chan in range(nchan):
+					if chan==0:
+						realticks=ticks
+					else:
+						realticks=0
+					track.append(mido.Message('control_change', channel=chan, control=7, value=int(H_rs[chan,i]*127/Hmax), time=realticks))
+			for chan in range(nchan):
+				track.append(mido.Message('note_off', channel=chan, note=self.keys[chan], time=0))
+			mid.save(fn_midi)
+		os.system('fluidsynth -ni {} -F {} -r {} {} {}'.format(self.cfg['fluidsynthextracommand'],fn_wav,fs,fn_font,fn_midi))
+		self.message(f'Audio file written to {self.cfg["save_path"]}')
+		return self
+
+	def write_video(self):
+		'''
+		Writes video file using self.data['H_pp'] and self.data['W_pp'] using ffmpeg. 
+		We avoid using opencv because it is very slow in a conda environment
+		http://zulko.github.io/blog/2013/09/27/read-and-write-video-frames-in-python-using-ffmpeg/
+		'''
+		if not self.check_data():
+			return
+		self.process_H_W()
+		fn_vid=os.path.join(self.cfg['save_path'],self.cfg['file_out'])+'.mp4'
+		v_shape=self.data['W_shape'][::-1][1:] # Reverse because ffmpeg does hxw
+		command=['ffmpeg',
+			'-loglevel', 'warning', # Prevents excessive messages
+			'-hide_banner',
+			'-y', # Auto overwrite
+			'-f', 'image2pipe',
+			'-vcodec','png',
+			'-s', '{}x{}'.format(v_shape[0],v_shape[1]),
+			'-r', str(self.cfg['fr']*self.cfg['speed']/100),
+			'-i', '-', # The input comes from a pipe
+			'-an', # Tells FFMPEG not to expect any audio
+			'-q:v','2', # Quality
+			'-vcodec', 'mpeg4',
+			'-preset', 'ultrafast',
+			fn_vid]
+		pipe=sp.Popen(command, stdin=sp.PIPE)
+		nframes=len(self.data['H_pp'].T)
+		t0 = time.time()
+		for i in range(nframes):
+			frame=(self.data['W_pp']@np.diag(self.data['H_pp'][:,i])@self.cmap[:,:-1]*(255/self.cfg['brightness'])).reshape(self.data['W_shape'][0],self.data['W_shape'][1],3).clip(min=0,max=255).astype('uint8')
+			im=Image.fromarray(frame)
+			im.save(pipe.stdin, 'PNG')
+			if self.display and i%20==1:
+				self.status['text']=f'Writing video file, {i} out of {nframes} frames written, avg fps: {i/(time.time()-t0)}'
+				self.update()
+			elif not self.display and i%20==1:
+				print(f'Writing video file, {i} out of {nframes} frames written, avg fps: {i/(time.time()-t0)}',end='\r')
+		pipe.stdin.close()
+		pipe.wait()
+		self.message(f'Video file written to {self.cfg["save_path"]}')
+		return self
+	
+	def merge(self):
+		'''
+		Merges video and audio with ffmpeg
+		'''
+		fn=os.path.join(self.cfg['save_path'],self.cfg['file_out'])
+		cmd='ffmpeg -hide_banner -loglevel warning -y -i {} -i {} -c:a aac -map 0:v:0 -map 1:a:0 {}'.format(fn+'.mp4',fn+'.wav',fn+'_AV.mp4')
+		os.system(cmd)
+		self.message(f'A/V file written to {self.cfg["save_path"]}')
+		return self
+	
+	def write_AV(self):
+		'''
+		Runs full write and merge
+		'''
+		self.write_video()
+		self.write_audio()
+		self.merge()
+		if not self.display:
+			return self
+
+	def cleanup(self):
+		'''
+		Tries to remove any files that are video or audio only.	
+		'''
+		fn=os.path.join(self.cfg['save_path'],self.cfg['file_out'])
+		try: 
+			os.remove(fn+'.mp4')
+		except OSError: 
+			pass
+		try: 
+			os.remove(fn+'.wav')
+		except OSError: 
+			pass
+		try: 
+			os.remove(fn+'.mid')
+		except OSError: 
+			pass
+		self.message(f'A/V only videos removed')
+		return self
+
+	def edit_save_path(self):
+		self.save_path.set(fd.askdirectory(title='Select a directory to save output files',initialdir=self.cfg['save_path']))
+
+	def initGUI(self):
+		'''
+		Initialize GUI fields, labels, dropdowns, etc.
+		'''
+		self.winfo_toplevel().title('pyanthem v{}'.format(pkg_resources.require("pyanthem")[0].version))
+		#photo = PhotoImage(file = os.path.join(os.path.dirname(os.path.abspath(__file__)),'logo.png'))
+		#self.iconphoto(False, photo)
+		self.protocol('WM_DELETE_WINDOW', self.quit)
+
+		# StringVars
+		self.file_in=init_entry(None)
+		self.file_out=init_entry(None)
+		self.save_path=init_entry(None)
+		self.speed=init_entry(100)
+		self.fr=init_entry(0)
+		self.start_percent=init_entry(0)
+		self.end_percent=init_entry(100)
+		self.baseline=init_entry(0)
+		self.brightness=init_entry(0)
+		self.threshold=init_entry(0)
+		self.octave_add=init_entry('2')
+		self.scale_type=init_entry('Maj. 7 (4/oct)')
+		self.key=init_entry('C')
+		self.sound_preset=init_entry('Piano')
+		self.comps_to_show=init_entry('all')
+		self.cmapchoice=init_entry('jet')
+		
+		self.fluidsynthextracommand = ''
+		#self.ffmpegextracommand = ''
+
+		# Labels
+		Label(text='',font='Helvetica 1 bold').grid(row=0,column=0) # Just to give a border around Seperators
+		Label(text='File Parameters',font='Helvetica 14 bold').grid(row=1,column=1,columnspan=2,sticky='WE')
+		Label(text='Movie Parameters',font='Helvetica 14 bold').grid(row=1,column=3,columnspan=2,sticky='WE')
+		Label(text='Audio Parameters',font='Helvetica 14 bold').grid(row=1,column=5,columnspan=2,sticky='WE')
+		Label(text='Input Filename').grid(row=2, column=1,columnspan=2,sticky='W')
+		Label(text='Output Filename').grid(row=4, column=1,columnspan=2,sticky='W')
+		Label(text='Save Path').grid(row=6, column=1,columnspan=1,sticky='W')
+		Label(text='Speed (%)').grid(row=2, column=3, sticky='E')
+		Label(text='Start (%)').grid(row=3, column=3, sticky='E')
+		Label(text='End (%)').grid(row=4, column=3, sticky='E')
+		Label(text='Baseline').grid(row=5, column=3, sticky='E')
+		Label(text='Max brightness').grid(row=6, column=3, sticky='E')
+		Label(text='Colormap').grid(row=7, column=3, sticky='E')
+		Label(text='Threshold').grid(row=2, column=5, sticky='E')
+		Label(text='Octave').grid(row=3, column=5, sticky='E')
+		Label(text='Scale Type').grid(row=4, column=5, sticky='E')
+		Label(text='Key').grid(row=5, column=5, sticky='E')
+		Label(text='Audio format').grid(row=6, column=5, sticky='E')
+
+		# Messages
+		self.status=Message(text='Welcome to pyanthem v{}!'.\
+			format(pkg_resources.require("pyanthem")[0].version),bg='white',fg='black',width=450)
+		self.status.grid(row=9, column=2, columnspan=5, sticky='NESW')
+		self.status['anchor']='nw'
+
+		# Entries
+		Entry(textvariable=self.file_in).grid(row=3, column=1,columnspan=2,sticky='W')
+		Entry(textvariable=self.file_out).grid(row=5, column=1,columnspan=2,sticky='W')
+		Entry(textvariable=self.save_path,width=17).grid(row=7, column=1,columnspan=2,sticky='EW')
+		Entry(textvariable=self.speed,width=7).grid(row=2, column=4, sticky='W')
+		Entry(textvariable=self.start_percent,width=7).grid(row=3, column=4, sticky='W')
+		Entry(textvariable=self.end_percent,width=7).grid(row=4, column=4, sticky='W')
+		Entry(textvariable=self.baseline,width=7).grid(row=5, column=4, sticky='W')
+		Entry(textvariable=self.brightness,width=7).grid(row=6, column=4, sticky='W')
+		self.threshold_entry=Entry(textvariable=self.threshold,width=7)
+		self.threshold_entry.grid(row=2, column=6, sticky='W')
+
+		# Styles
+		s = Style()
+		s.configure('my.TButton', font=('Helvetica', 14))
+
+		# Buttons
+		Button(text='Edit',command=self.edit_save_path,width=5).grid(row=6, column=2)
+		Button(text='Preview',width=11,command=self.preview_notes).grid(row=7, column=5,columnspan=1)
+		
+		self.update_button=Button(text='Update',width=7,command=self.process_H_W,style='my.TButton')
+		self.update_button.grid(row=9,column=1,columnspan=1)
+		
+		# Combo box
+		self.cmapchooser=Combobox(self,textvariable=self.cmapchoice,width=5)
+		self.cmapchooser['values']=cmaps_opts
+		self.cmapchooser['state']='readonly'
+		self.cmapchooser.grid(row=7, column=4, sticky='W')
+		self.cmapchooser.current()
+		self.cmap=[]
+
+		self.octave_add_menu=Combobox(self,textvariable=self.octave_add,width=7)
+		self.octave_add_menu['values']=tuple(octave_add_opts.keys())
+		self.octave_add_menu['state']='readonly'
+		self.octave_add_menu.grid(row=3, column=6, sticky='W')
+		self.octave_add_menu.current()
+
+		self.scale_type_menu=Combobox(self,textvariable=self.scale_type,width=11)
+		self.scale_type_menu['values']=tuple(scale_keys.keys())
+		self.scale_type_menu['state']='readonly'
+		self.scale_type_menu.grid(row=4, column=6, sticky='W')
+		self.scale_type_menu.current()
+
+		self.key_menu=Combobox(self,textvariable=self.key,width=7)
+		self.key_menu['values']=tuple(key_opts.keys())
+		self.key_menu['state']='readonly'
+		self.key_menu.grid(row=5, column=6, sticky='W')
+		self.key_menu.current()
+
+		self.sound_preset_menu=Combobox(self,textvariable=self.sound_preset,width=7)
+		self.sound_preset_menu['values']=tuple(sound_presets.keys())
+		self.sound_preset_menu['state']='readonly'
+		self.sound_preset_menu.grid(row=6, column=6, sticky='W')
+		self.sound_preset_menu.current()
+
+		# Checkbox
+		self.audio_analog=IntVar()
+		self.audio_analog.set(0)
+		Checkbutton(self, text="Analog",command=self.process_H_W,variable=self.audio_analog).grid(row=7, column=6,columnspan=1)
+
+		# Menu bar
+		menubar=Menu(self)
+		filemenu=Menu(menubar, tearoff=0)
+		filemenu.add_command(label="Load data...", command=self.load_GUI)
+		filemenu.add_command(label="Load config...", command=self.load_config)
+		filemenu.add_command(label="Quit",command=self.quit,accelerator="Ctrl+Q")
+
+		savemenu=Menu(menubar, tearoff=0)
+		savemenu.add_command(label="Audio", command=self.write_audio)
+		savemenu.add_command(label="Video", command=self.write_video)
+		savemenu.add_command(label="Config", command=self.dump_cfg)
+		savemenu.add_command(label="Merge A/V", command=self.merge)
+		savemenu.add_command(label="Write A/V then merge", command=self.write_AV)
+		savemenu.add_command(label="Cleanup", command=self.cleanup)
+
+		advancedmenu=Menu(menubar, tearoff=0)
+		advancedmenu.add_command(label="Custom fluidsynth params", command=self.fluidsynthextra)
+		#advancedmenu.add_command(label="Custom ffmpeg params", command=self.ffmpegextra)
+		advancedmenu.add_command(label="View config", command=self.view_cfg)
+
+		menubar.add_cascade(label="File", menu=filemenu)
+		menubar.add_cascade(label="Save", menu=savemenu)
+		menubar.add_cascade(label="Advanced", menu=advancedmenu)
+		self.config(menu=menubar)
+
+		# Seperators
+		s_v=[[0,1,9],[2,1,8],[4,1,8],[6,1,9]]
+		s_h=[[1,1,6],[1,2,6],[1,9,6],[1,10,6],[1,4,2],[1,6,2]]
+		for sv in s_v:
+			Separator(self, orient='vertical').grid(column=sv[0], row=sv[1], rowspan=sv[2], sticky='nse')
+		for sh in s_h:
+			Separator(self, orient='horizontal').grid(column=sh[0], row=sh[1], columnspan=sh[2], sticky='nwe')
+
+		# Offset
+		self.offsetH=IntVar()
+		self.offsetH.set(1)
+
+		# Bind shortcuts
+		self.bind_all("<Control-q>", self.quit)
+		self.bind_all("<Control-a>", lambda:[self.process_H_W(),self.refresh_GUI()])
+
+	def init_plots(self):
+		'''
+		Initializes the plot areas. Is called every time update_GUI() is called.
+		'''
+		# H
+		if 'H_pp' in self.data:
+			self.figH=plt.Figure(figsize=(7,6), dpi=100, tight_layout=True)
+			self.Hax1=self.figH.add_subplot(211)
+			self.Hax2=self.figH.add_subplot(212)
+			self.Hax2.set_title('Audio Preview')
+			self.canvas_H=FigureCanvasTkAgg(self.figH, master=self)
+			self.canvas_H.get_tk_widget().grid(row=1,column=7,rowspan=30,columnspan=10)
+			bg=self.status.winfo_rgb(self['bg'])
+			self.figH.set_facecolor([(x>>8)/255 for x in bg])
+			self.Hax1.spines['left'].set_visible(False)
+			self.Hax1.spines['top'].set_visible(False)
+			self.Hax1.spines['bottom'].set_visible(False)
+			self.Hax1.spines['right'].set_visible(False)
+			self.Hax1.yaxis.tick_right()
+			self.Hax1.yaxis.set_label_position('right')
+			self.Hax1.tick_params(axis='x',which='both',bottom=False, top=False, labelbottom=False, right=False)
+			self.Hax2.set(xlabel='time (sec)',ylabel='Component #')
+			self.Hax2.spines['left'].set_visible(False)
+			self.Hax2.spines['top'].set_visible(False)
+			self.Hax2.spines['bottom'].set_visible(False)
+			self.Hax2.spines['right'].set_visible(False)
+			self.Hax2.yaxis.tick_right()
+			self.Hax2.yaxis.set_label_position('right')
+			# Checkbox
+			Checkbutton(self, text="Offset H",command=self.refresh_GUI,variable=self.offsetH).grid(row=1,rowspan=1,column=16)
+		
+		try: 
+			# If user previously loaded dataset with W, clear those 
+			# plots and remove associated GUI elements.
+			self.figW.clear()
+			self.canvas_W.draw()
+			self.frameslider.grid_forget()
+			self.comps_to_show_label.grid_forget()
+			self.comps_to_show_entry.grid_forget()
+		except:
+			pass
+
+		if 'W_pp' in self.data:
+			self.figW=plt.Figure(figsize=(6,3), dpi=100, constrained_layout=True)
+			self.Wax1=self.figW.add_subplot(121)
+			self.Wax2=self.figW.add_subplot(122)
+			self.Wax1.set_title('Video Preview')
+			self.Wax2.set_title('Spatial Data (W)')
+			self.Wax1.axis('off')
+			self.Wax2.axis('off')
+			self.canvas_W=FigureCanvasTkAgg(self.figW, master=self)
+			self.canvas_W.get_tk_widget().grid(row=11,column=1,rowspan=19,columnspan=6)
+			self.figW.set_facecolor([(x>>8)/255 for x in bg])
+			
+			# Frameslider
+			# frameslider
+			self.frameslider=Scale(self, from_=1, to=2, orient=HORIZONTAL)
+			self.frameslider.set(1)
+			self.frameslider['command']=self.refresh_slider
+			self.frameslider.grid(row=30, column=1, columnspan=3,sticky='EW')
+			
+		# comps_to_show
+		self.comps_to_show_label=Label(text='Components:')
+		self.comps_to_show_label.grid(row=30, column=5, columnspan=1, sticky='E')
+		self.comps_to_show_entry=Entry(textvariable=self.comps_to_show,width=15,justify='center')
+		self.comps_to_show_entry.grid(row=30, column=6, columnspan=1,sticky='W')
+		
+	def process_raw(self,data=None,n_clusters=None,frame_rate=None,save=False,file_in=None):
+		'''
+		Decomposes raw dataset. Can be used in two ways: as a part of the 
+		GUI class for immediate processing (e.g. process_raw().write_AV()),
+		or as a method to save a new dataset. 
+		'''
+		sh=data.shape
+		if len(sh) != 3:
+			self.message('ERROR: input dataset is not 3D.')
+			return
+		data=data.reshape(sh[0]*sh[1],sh[2])
+		# Ignore rows with any nans
+		nanidx=np.any(np.isnan(data), axis=1)
+		data_nn=data[~nanidx] # nn=non-nan
+		# k-means
+		print('Performing k-means...',end='')
+		if n_clusters is None:
+			# Default k is the 4th root of the number of samples per frame (for 256x256, this would be 16)
+			n_clusters=int(len(data)**.25) 
+			print(f'No num_clusters given. Defaulting to {n_clusters}...',end='')
+		idx_nn=KMeans(n_clusters=n_clusters, random_state=0).fit(data_nn).labels_
+		idx=np.zeros((len(data),))
+		idx[nanidx==False]=idx_nn
+		# TCs
+		H=np.zeros((n_clusters,len(data.T)))
+		for i in range(n_clusters):
+			H[i,:]=np.nanmean(data[idx==i,:],axis=0)
+		print('done.')
+		# NNLS
+		nnidx=np.where(~nanidx)[0]
+		W=np.zeros((len(data),n_clusters))
+		print('Performing NNLS...',end='')
+		for i in range(len(nnidx)):
+			W[nnidx[i],:]=nnls(H.T,data_nn[i,:])[0]
+		# Sort bottom to top
+		xc,yc=[],[]
+		(X,Y)=np.meshgrid(range(sh[1]),range(sh[0]))
+		for i in range(len(W.T)):
+			Wtmp=W[:,i].reshape(sh[0],sh[1])
+			xc.append((X*Wtmp).sum() / Wtmp.sum().astype("float"))
+			yc.append((Y*Wtmp).sum() / Wtmp.sum().astype("float"))
+		I=np.argsort(yc[::-1]) # Reverse orders from bottom to top
+		W,H=W[:,I],H[I,:]
+		print('done.')
+		
+		# Assign variables and save
+		self.data={}
+		self.data['H']=H
+		self.data['W']=W.reshape(sh[0],sh[1],n_clusters)
+		#self.data['W_shape']=self.data['W'].shape.flatten()
+		if frame_rate==[]:
+			self.data['fr']=10
+			print('No fr given. Defaulting to 10')
+		else:
+			self.data['fr']=frame_rate
+		if save:
+			if file_in is None:
+				file_in='data.mat'
+			fn=file_in.replace('.mat','_decomp.mat')
+			savemat(fn,self.data)
+			self.message(f'Decomposed data file saved to {fn}')
+		
+		# Reshape W here, since any use of self from here would require a flattened W
+		self.data['W']=self.data['W'].reshape(self.data['W'].shape[0]*self.data['W'].shape[1],self.data['W'].shape[2])
+		return self
+
+	def fluidsynthextra(self):
+		self.fluidsynthextracommand=sd.askstring('Input custom fluidsynth parameters here','',initialvalue=self.fluidsynthextracommand,parent=self)
+
+	#def ffmpegextra(self):
+#		self.ffmpegextracommand=sd.askstring('Input custom ffmpeg parameters here','',initialvalue=self.ffmpegextracommand,parent=self)
+
+	def view_cfg(self):
+		'''
+		Prints cfg info to command line
+		'''
+		try:
+			for key in self.cfg:
+				print(str(key)+': '+str(self.cfg[key]))
+		except:
+			pass
+		
+	def help(self):
+		print('To load a dataset:\npyanthem.load_data()\n\nTo load a cfg file:\npyanthem.load_config()\n\nTo write video:\npyanthem.write_video()\n\nTo write audio:\npyanthem.write_audio()')
+
+if __name__=="__main__":
+	run()
+
+# self\.([a-z_]{1,14})\.get\(\)
+# self\.cfg\[$1\]
```

### Comparing `pyanthem-1.1.9/pyanthem/pyanthem_vars.py` & `pyanthem-1.2.0/pyanthem/pyanthem_vars.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,87 @@
-from os.path import realpath, join, split
-self_fns={
-'fr':'entry',
-'start_percent':'entry',
-'end_percent':'entry',
-'baseline':'entry',
-'brightness':'entry',
-'threshold':'entry',
-'octave_add':'entry',
-'scale_type':'entry',
-'key':'entry',
-'sound_preset':'entry',
-'comps_to_show':'entry',
-'cmapchoice':'entry', 
-'speed':'entry',
-'file_in':'entry',
-'file_out':'entry',
-'save_path':'entry',
-'audio_analog':'entry',
-'comps_to_show_arr':'value',
-'fluidsynthextracommand':'value'
-}
-
-octave_add_opts={
-'0':0,
-'1':12,
-'2':24,
-'3':36,
-'4':48,
-'5':60,
-'6':60
-}
-
-scale_keys={
-'Chromatic (12/oct)':[0,1,2,3,4,5,6,7,8,9,10,11],
-'Major scale (7/oct)':[0,2,4,5,7,9,11],
-'Minor scale (7/oct)':[0,2,3,5,7,9,11],
-'Maj. chord (3/oct)':[0,4,7],
-'Min. chord (3/oct)':[0,3,7],
-'Maj. 7 (4/oct)':[0,4,7,11],
-'Min. 7 (4/oct)':[0,3,7,11],
-'Maj. 2/9 (5/oct)':[0,2,4,7,11],
-'Min. 2/9 (5/oct)':[0,2,3,7,11]
-}
-
-key_opts={
-'C' :0, 
-'C#':1,
-'D' :2,
-'D#':3,
-'E' :4,
-'F' :5,
-'F#':6,
-'G' :7,
-'G#':8,
-'A' :9,
-'A#':10,
-'B' :11
-}
-
-cmaps_opts=tuple(sorted(['viridis', 'plasma', 'inferno', 'magma', 'cividis', 
-'bone', 'pink','spring', 'summer', 'autumn', 'winter', 'cool','hot','copper', 
-'coolwarm', 'bwr', 'seismic','twilight', 'hsv', 'prism', 'ocean', 
-'terrain','brg', 'rainbow', 'jet'],key=lambda s: s.lower()))
-
-'''
-Google drive id for .sf2 files from https://sites.google.com/site/soundfonts4u/
-'''
-sound_font='142L-FgN7ToWmiB2y7PzmcnGOvzGNnZX4'
-sound_presets={
-'Piano':0,
-'Piano w/ Reverb':1,
-'Strings':2,
-'Rhodes':3
-}
-
-'''
-static variables
-'''
-fs=44100
+from os.path import realpath, join, split
+self_fns={
+'fr':'entry',
+'start_percent':'entry',
+'end_percent':'entry',
+'baseline':'entry',
+'brightness':'entry',
+'threshold':'entry',
+'octave_add':'entry',
+'scale_type':'entry',
+'key':'entry',
+'sound_preset':'entry',
+'comps_to_show':'entry',
+'cmapchoice':'entry', 
+'speed':'entry',
+'file_in':'entry',
+'file_out':'entry',
+'save_path':'entry',
+'audio_analog':'entry',
+'comps_to_show_arr':'value',
+'fluidsynthextracommand':'value'
+}
+
+octave_add_opts={
+'0':0,
+'1':12,
+'2':24,
+'3':36,
+'4':48,
+'5':60,
+'6':60
+}
+
+scale_keys={
+'Chromatic (12/oct)':[0,1,2,3,4,5,6,7,8,9,10,11],
+'Major scale (7/oct)':[0,2,4,5,7,9,11],
+'Minor scale (7/oct)':[0,2,3,5,7,9,11],
+'Maj. chord (3/oct)':[0,4,7],
+'Min. chord (3/oct)':[0,3,7],
+'Maj. 7 (4/oct)':[0,4,7,11],
+'Min. 7 (4/oct)':[0,3,7,11],
+'Maj. 2/9 (5/oct)':[0,2,4,7,11],
+'Min. 2/9 (5/oct)':[0,2,3,7,11]
+}
+
+key_opts={
+'C' :0, 
+'C#':1,
+'D' :2,
+'D#':3,
+'E' :4,
+'F' :5,
+'F#':6,
+'G' :7,
+'G#':8,
+'A' :9,
+'A#':10,
+'B' :11
+}
+
+cmaps_opts=tuple(sorted(['viridis', 'plasma', 'inferno', 'magma', 'cividis', 
+'bone', 'pink','spring', 'summer', 'autumn', 'winter', 'cool','hot','copper', 
+'coolwarm', 'bwr', 'seismic','twilight', 'hsv', 'prism', 'ocean', 
+'terrain','brg', 'rainbow', 'jet'],key=lambda s: s.lower()))
+
+'''
+Google drive id for .sf2 files from https://sites.google.com/site/soundfonts4u/
+'''
+sound_font='1TvjLlgKqZxcrZvefciJGX1Q_3e8Cy4dP'
+sound_presets={
+'0':0,
+'1':1,
+'2':2,
+'3':3,
+'4':4,
+'5':5,
+'6':6,
+'7':7,
+'8':8,
+'9':9,
+'10':10,
+}
+
+'''
+static variables
+'''
+fs=44100
```

### Comparing `pyanthem-1.1.9/pyanthem.egg-info/PKG-INFO` & `pyanthem-1.2.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,220 +1,204 @@
-Metadata-Version: 2.1
-Name: pyanthem
-Version: 1.1.9
-Summary: pyanthem - an audiovisualization tool to make your data more interesting
-Home-page: https://github.com/nicthib/pyanthem
-Author: Nic Thibodeaux
-Author-email: dnt2111@columbia.edu
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7,!= 3.8.*
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-********************************************************************
-pyanthem: Transforming your datasets into a colorful, audible format
-********************************************************************
-
-Features:
-=========
-
-1) Converts three-dimensional datasets to visually pleasing, audible representations
-2) A variety of video and audio parameters
-3) In-place video and audio merge
-4) GUI and Command-line interface for maximum flexibility
-5) Example datasets to get you started
-6) Headache-free installation with an Anaconda environment
-
-Usage
-=====
-
-pyanthem was primarily developed to interpret matrix-decomposed functional imaging datasets - for example, a dataset **V** with shape :code:`[height,width,time]`, is decomposed into two matrixes: **W** with shape :code:`[height*width,n]`, and **H** with shape :code:`[n,time]` such that :code:`H x W = V`. Here, n represents the number of variables represented by the decomposition. There are various techniques used to decompose matrixes - two popular techniques include Non-negative Matrix Factorization (NMF), and Singular Value Decomposition (SVD).
-
-Here's a visual illustration of matrix decomposition - note that in this example, :code:`n=2`:
-
-.. image:: https://upload.wikimedia.org/wikipedia/commons/f/f9/NMF.png
-
-If you would prefer to keep things simple, you can skip matrix decomposition altogether and focus solely on converting raw data to audio - only working with the **H** matrix, where each row represents a variable and each column represents a time point.
-
-If this is too much information to digest, don't worry! Try the example below to get more familiar with what the data looks like, and how pyanthem transforms it.
-
-Requirements
-============
-
-*See installation guide below before proceeding!*
-
-`Python 3.7`_:
-   Currently, pyanthem is tested to work on Python 3.7. This will be updated as more versions are tested.
-
-FFmpeg_:
-   ffmpeg enables video creation and merging.
-
-FluidSynth_:
-   FluidSynth enables conversion of MIDI files to crisp, high quality sound files.
-   
-If you do have the above requirements installed, you can install pyanthem using pip: :code:`pip install pyanthem`
-
-Conda (optional, but highly recommended):
-   Conda enables simple and reliable package installation. Use Miniconda_ for a minimal installation, or Anaconda_ otherwise.
-
-.. _`Python 3.7`: https://www.python.org/downloads/release/python-378/
-.. _FFmpeg: https://ffmpeg.org/
-.. _FluidSynth: http://www.fluidsynth.org/
-.. _Miniconda: https://docs.conda.io/en/latest/miniconda.html
-.. _Anaconda: https://www.anaconda.com/products/individual
-
-Installation
-============
-Note: If you do not have working installations of the listed requirements (Python 3.7 + fluidsynth + ffmpeg), it is **strongly recommended** that you use Miniconda_/Anaconda_ for a straightforward installation process. If you do not have either, Miniconda is preferred as it is a faster install and takes up much less space than Anaconda.
-
-Using Miniconda/Anaconda:
--------------------------
-
-Create an environment and install the required packages::
-   
-   conda create -n pyanthem python=3.7 pip ffmpeg fluidsynth --channel conda-forge --channel nicthib
-
-Next, activate the environment::
-   
-   conda activate pyanthem
-
-Finally, install the pyanthem Python package using pip::
-   
-   pip install pyanthem
-
-Example datasets and Scripts
-----------------------------
-
-If you want to get familiar with the datasets that pyanthem uses and try some applications of pyanthem, clone this repository or download `here.`
-
-.. _`here`: https://github.com/nicthib/pyanthem/archive/master.zip
-
-Using pyanthem in a Jupyter Notebook
------------------------------------------------
-
-To access the pyanthem environment in a Jupyter notebook, first install ipykernel in your environment::
-   
-   conda install -c anaconda ipykernel
-
-After this, create the kernel::
-   
-   python -m ipykernel install --user --name=pyanthem
-
-Once in a notebook, switch to the pyanthem kernel by selecting :code:`Kernel > Change kernel > pyanthem`
-
-*Note: While the pyanthem kernel will now be available in any Jupyter notebook session, pyanthem will not function properly unless the Jupyter notebook is launched inside the pyanthem environment*.
-
-Example
-=======
-
-Using pyanthem in GUI mode
---------------------------
-
-First, import pyanthem and begin a pyanthem session:
-
-.. code-block:: python
-   
-   import pyanthem
-   pyanthem.run()
-
-The first time you run pyanthem, it will download a necessary soundfont file - this will take a minute or two.
-
-.. code-block::
-   
-   ♫ Initializing soundfont library...
-   ♫ Downloading 17QuXRbApe0JTlYfBs7iSMCMu3xRWMHOV into...
-   ♫ 238.3 MiB Done.
-
-Once completed, the pyanthem GUI will initialize:
-
-.. image:: https://github.com/nicthib/pyanthem/blob/media/GUI1.png
-
-Next, load a dataset by clicking :code:`File > Load from .mat`. For this section, we will load the dataset :code:`demo1.mat`. Currently, you can import any .mat or hdf5 file that contains the following variables:
-
-1) Temporal variable (**H, required**): A 2D matrix of shape :code:`[n,t]`, where each row is a component and each column is a time-point. This variable is referred to as **"H"** in the pyanthem environment.
-
-2) Spatial variable (**W, optional**): A 3D matrix of shape :code:`[h,w,n]`, where h and w represent the spatial height and width of your dataset. If this variable is not given, no video output is possible.
-
-3) Framerate (**fr, optional**): A single float value, representing the frame rate of your dataset in Hz. If a framerate is not given, pyanthem will provide a default.
-
-*Note: Make sure to only include these variables in your file to avoid any errors. You can name them however you like, but make sure there are only one of each variable.* 
-
-Once loading is complete, the GUI should update with default options, and plots of **H** and **W**:
-
-.. image:: https://github.com/nicthib/pyanthem/blob/media/GUI2.png
-
-The bottom left plots show two representations of the dataset: A preview of the output movie (left), and a visualization of what components are included and the colormap selection. The right two plots show raw representations of **H** (top), and a visualization of the audio output file (right). Lighter colors indicate loud notes, and darker colors indicate quiet notes, with black indicating silence.
-
-From here, you can adjust parameters, preview the output, and finally save video and audio files. If you want to check how your parameter adjustments impact your audivisualization, click the **Update** button, and your changes will be reflected. Any issues with your selected parameters will be indicated in the white status box. Try adjusting a few parameters and observing how the plots change.
-
-Finally, render output files with the :code:`Save --> Write A/V then merge` menu command.
-
-Congratulations - you've created your first audiovisualization!
-
-Using pyanthem in CLI (command-line interface) mode
----------------------------------------------------
-
-pyanthem's CLI mode is useful for running batch conversions of large amounts of data once you are happy with your audiovisualization parameters, or creating more complex audiovisualizions that use multiple datasets and instruments. CLI mode is not recommended to use until you have used the GUI and are comfortable with the parameters and usage.
-
-To run pyanthem in CLI mode, pass the argument :code:`display=False`, and assign the :code:`.run()` method to a variable:
-
-.. code-block:: python
-   
-   import pyanthem
-   g=pyanthem.run(display=False)
-
-Next, load a dataset and config file using the :code:`.load_data()` and :code:`.load_config()` methods. You can pass an explicit file name to the :code:`file_in` argument, or pass none to recieve a file select prompt (note the use of the leading :code:`r` when naming a file location):
-
-.. code-block:: python
-   
-   g.load_data(file_in=r'path/to/your/file.mat')
-   g.load_config(file_in=r'path/to/your/config.p')
-
-Finally, render the audio and video file, then merge the files using the :code:`.write_audio()`, :code:`.write_video()` and :code:`.merge()` methods:
-
-.. code-block:: python
-   
-   g.write_audio()
-   g.write_video()
-   g.merge()
-
-Once you're comfortable with this syntax, you can combine all of these steps into a single line, write a merged video with the :code:`.write_AV()` method, and even remove the intermediate files using the :code:`.cleanup()` method:
-
-.. code-block:: python
-   
-   data_file = r'path/to/your/file.mat'
-   config_file = r'path/to/your/config.p'
-   g.load_data(file_in=data_file).load_config(file_in=config_file).write_AV().cleanup()
-
-Congratulations - you've created your first audiovisualization in CLI mode!
-
-Team
-====
-
-.. |niclogo| image:: https://avatars1.githubusercontent.com/u/34455769?v=3&s=200
-
-+---------------------------+
-| Nic Thibodeaux            |
-+===========================+
-| |niclogo|                 |
-+---------------------------+
-| http://github.com/nicthib |
-+---------------------------+
-
-FAQ
-===
-
-Under construction!
--------------------
-
-Support
-=======
-
-- Twitter: `@nicthibs`_
-
-.. _`@nicthibs`: http://twitter.com/nicthibs
-
-
+********************************************************************
+pyanthem: Transforming your datasets into a colorful, audible format
+********************************************************************
+
+Features:
+=========
+
+1) Converts three-dimensional datasets to visually pleasing, audible representations
+2) A variety of video and audio parameters
+3) In-place video and audio merge
+4) GUI and Command-line interface for maximum flexibility
+5) Example datasets to get you started
+6) Headache-free installation with an Anaconda environment
+
+Usage
+=====
+
+pyanthem was primarily developed to interpret matrix-decomposed functional imaging datasets - for example, a dataset **V** with shape :code:`[height,width,time]`, is decomposed into two matrixes: **W** with shape :code:`[height*width,n]`, and **H** with shape :code:`[n,time]` such that :code:`H x W = V`. Here, n represents the number of variables represented by the decomposition. There are various techniques used to decompose matrixes - two popular techniques include Non-negative Matrix Factorization (NMF), and Singular Value Decomposition (SVD).
+
+Here's a visual illustration of matrix decomposition - note that in this example, :code:`n=2`:
+
+.. image:: https://upload.wikimedia.org/wikipedia/commons/f/f9/NMF.png
+
+If you would prefer to keep things simple, you can skip matrix decomposition altogether and focus solely on converting raw data to audio - only working with the **H** matrix, where each row represents a variable and each column represents a time point.
+
+If this is too much information to digest, don't worry! Try the example below to get more familiar with what the data looks like, and how pyanthem transforms it.
+
+Requirements
+============
+
+*See installation guide below before proceeding!*
+
+`Python 3.7`_:
+   Currently, pyanthem is tested to work on Python 3.7. This will be updated as more versions are tested.
+
+FFmpeg_:
+   ffmpeg enables video creation and merging.
+
+FluidSynth_:
+   FluidSynth enables conversion of MIDI files to crisp, high quality sound files.
+   
+If you do have the above requirements installed, you can install pyanthem using pip: :code:`pip install pyanthem`
+
+Conda (optional, but highly recommended):
+   Conda enables simple and reliable package installation. Use Miniconda_ for a minimal installation, or Anaconda_ otherwise.
+
+.. _`Python 3.7`: https://www.python.org/downloads/release/python-378/
+.. _FFmpeg: https://ffmpeg.org/
+.. _FluidSynth: http://www.fluidsynth.org/
+.. _Miniconda: https://docs.conda.io/en/latest/miniconda.html
+.. _Anaconda: https://www.anaconda.com/products/individual
+
+Installation
+============
+Note: If you do not have working installations of the listed requirements (Python 3.7 + fluidsynth + ffmpeg), it is **strongly recommended** that you use Miniconda_/Anaconda_ for a straightforward installation process. If you do not have either, Miniconda is preferred as it is a faster install and takes up much less space than Anaconda.
+
+Using Miniconda/Anaconda:
+-------------------------
+
+Create an environment and install the required packages::
+   
+   conda create -n pyanthem python=3.7 pip ffmpeg fluidsynth --channel conda-forge --channel nicthib
+
+Next, activate the environment::
+   
+   conda activate pyanthem
+
+Finally, install the pyanthem Python package using pip::
+   
+   pip install pyanthem
+
+Example datasets and Scripts
+----------------------------
+
+If you want to get familiar with the datasets that pyanthem uses and try some applications of pyanthem, clone this repository or download `here.`
+
+.. _`here`: https://github.com/nicthib/pyanthem/archive/master.zip
+
+Using pyanthem in a Jupyter Notebook
+-----------------------------------------------
+
+To access the pyanthem environment in a Jupyter notebook, first install ipykernel in your environment::
+   
+   conda install -c anaconda ipykernel
+
+After this, create the kernel::
+   
+   python -m ipykernel install --user --name=pyanthem
+
+Once in a notebook, switch to the pyanthem kernel by selecting :code:`Kernel > Change kernel > pyanthem`
+
+*Note: While the pyanthem kernel will now be available in any Jupyter notebook session, pyanthem will not function properly unless the Jupyter notebook is launched inside the pyanthem environment*.
+
+Example
+=======
+
+Using pyanthem in GUI mode
+--------------------------
+
+First, import pyanthem and begin a pyanthem session:
+
+.. code-block:: python
+   
+   import pyanthem
+   pyanthem.run()
+
+*Note: You may run into an error here where some packages are missing. Simply install them using pip, and try running pyanthem again.*
+
+The first time you run pyanthem, it will download a necessary soundfont file - this will take a minute or two.
+
+.. code-block::
+   
+   ♫ Initializing soundfont library...
+   ♫ Downloading 17QuXRbApe0JTlYfBs7iSMCMu3xRWMHOV into...
+   ♫ 238.3 MiB Done.
+
+Once completed, the pyanthem GUI will initialize:
+
+.. image:: https://github.com/nicthib/pyanthem/blob/media/GUI1.png
+
+Next, load a dataset by clicking :code:`File > Load from .mat`. For this section, we will load the dataset :code:`demo1.mat`. Currently, you can import any .mat or hdf5 file that contains the following variables:
+
+1) Temporal variable (**H, required**): A 2D matrix of shape :code:`[n,t]`, where each row is a component and each column is a time-point. This variable is referred to as **"H"** in the pyanthem environment.
+
+2) Spatial variable (**W, optional**): A 3D matrix of shape :code:`[h,w,n]`, where h and w represent the spatial height and width of your dataset. If this variable is not given, no video output is possible.
+
+3) Framerate (**fr, optional**): A single float value, representing the frame rate of your dataset in Hz. If a framerate is not given, pyanthem will provide a default.
+
+*Note: Make sure to only include these variables in your file to avoid any errors. You can name them however you like, but make sure there are only one of each variable.* 
+
+Once loading is complete, the GUI should update with default options, and plots of **H** and **W**:
+
+.. image:: https://github.com/nicthib/pyanthem/blob/media/GUI2.png
+
+The bottom left plots show two representations of the dataset: A preview of the output movie (left), and a visualization of what components are included and the colormap selection. The right two plots show raw representations of **H** (top), and a visualization of the audio output file (right). Lighter colors indicate loud notes, and darker colors indicate quiet notes, with black indicating silence.
+
+From here, you can adjust parameters, preview the output, and finally save video and audio files. If you want to check how your parameter adjustments impact your audivisualization, click the **Update** button, and your changes will be reflected. Any issues with your selected parameters will be indicated in the white status box. Try adjusting a few parameters and observing how the plots change.
+
+Finally, render output files with the :code:`Save --> Write A/V then merge` menu command.
+
+Congratulations - you've created your first audiovisualization!
+
+Using pyanthem in CLI (command-line interface) mode
+---------------------------------------------------
+
+pyanthem's CLI mode is useful for running batch conversions of large amounts of data once you are happy with your audiovisualization parameters, or creating more complex audiovisualizions that use multiple datasets and instruments. CLI mode is not recommended to use until you have used the GUI and are comfortable with the parameters and usage.
+
+To run pyanthem in CLI mode, pass the argument :code:`display=False`, and assign the :code:`.run()` method to a variable:
+
+.. code-block:: python
+   
+   import pyanthem
+   g=pyanthem.run(display=False)
+
+Next, load a dataset and config file using the :code:`.load_data()` and :code:`.load_config()` methods. You can pass an explicit file name to the :code:`file_in` argument, or pass none to recieve a file select prompt (note the use of the leading :code:`r` when naming a file location):
+
+.. code-block:: python
+   
+   g.load_data(file_in=r'path/to/your/file.mat')
+   g.load_config(file_in=r'path/to/your/config.p')
+
+Finally, render the audio and video file, then merge the files using the :code:`.write_audio()`, :code:`.write_video()` and :code:`.merge()` methods:
+
+.. code-block:: python
+   
+   g.write_audio()
+   g.write_video()
+   g.merge()
+
+Once you're comfortable with this syntax, you can combine all of these steps into a single line, write a merged video with the :code:`.write_AV()` method, and even remove the intermediate files using the :code:`.cleanup()` method:
+
+.. code-block:: python
+   
+   data_file = r'path/to/your/file.mat'
+   config_file = r'path/to/your/config.p'
+   g.load_data(file_in=data_file).load_config(file_in=config_file).write_AV().cleanup()
+
+Congratulations - you've created your first audiovisualization in CLI mode!
+
+Team
+====
+
+.. |niclogo| image:: https://avatars1.githubusercontent.com/u/34455769?v=3&s=200
+
++---------------------------+
+| Nic Thibodeaux            |
++===========================+
+| |niclogo|                 |
++---------------------------+
+| http://github.com/nicthib |
++---------------------------+
+
+FAQ
+===
+
+Under construction!
+-------------------
+
+Support
+=======
+
+- Twitter: `@nicthibs`_
+
+.. _`@nicthibs`: http://twitter.com/nicthibs
```

### Comparing `pyanthem-1.1.9/setup.py` & `pyanthem-1.2.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-# conda remove --name pyanthem --all
-import setuptools
-with open('README.rst', 'r') as fh:
-	long_description = fh.read()
-setuptools.setup(
-	name='pyanthem',
-	version='1.1.9',
-	author='Nic Thibodeaux',
-	author_email='dnt2111@columbia.edu',
-	description='pyanthem - an audiovisualization tool to make your data more interesting',
-	long_description=long_description,
-	long_description_content_type='text/x-rst',
-	url='https://github.com/nicthib/pyanthem',
-	packages=setuptools.find_packages(),
-	setup_requires=[
-		'numpy',
-		'scipy'],
-	install_requires=[
-		'midiutil',
-		'matplotlib',
-		'pygame',
-		'sklearn',
-		'requests',
-		'googledrivedownloader',
-		'pillow',
-		'mido',
-		'ttkthemes',
-		'h5py'
-	  ],
-	include_package_data=True,
-	classifiers=[
-		'Programming Language :: Python :: 3',
-		'License :: OSI Approved :: MIT License',
-		'Operating System :: OS Independent',
-	],
-	python_requires='>=3.7,!= 3.8.*',
-)
+# conda remove --name pyanthem --all
+import setuptools
+with open('README.rst', 'r') as fh:
+	long_description = fh.read()
+setuptools.setup(
+	name='pyanthem',
+	version='1.2.0',
+	author='Nic Thibodeaux',
+	author_email='dnt2111@columbia.edu',
+	description='pyanthem - an audiovisualization tool to make your data more interesting',
+	long_description=long_description,
+	long_description_content_type='text/x-rst',
+	url='https://github.com/nicthib/pyanthem',
+	packages=setuptools.find_packages(),
+	setup_requires=[
+		'numpy',
+		'scipy'],
+	install_requires=[
+		'midiutil',
+		'matplotlib',
+		'pygame',
+		'sklearn',
+		'requests',
+		'gdown',
+		'pillow',
+		'mido',
+		'ttkthemes',
+		'h5py',
+		'scipy',
+		'scikit-learn',
+		'numpy'
+	  ],
+	include_package_data=True,
+	classifiers=[
+		'Programming Language :: Python :: 3',
+		'License :: OSI Approved :: MIT License',
+		'Operating System :: OS Independent',
+	],
+	python_requires='>=3.7',
+)
```

