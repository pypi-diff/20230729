# Comparing `tmp/codedapertures-0.5.tar.gz` & `tmp/codedapertures-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedapertures-0.5.tar", last modified: Fri Jul 28 00:11:12 2023, max compression
+gzip compressed data, was "codedapertures-0.6.tar", last modified: Sat Jul 29 02:50:48 2023, max compression
```

## Comparing `codedapertures-0.5.tar` & `codedapertures-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-28 00:11:12.507591 codedapertures-0.5/
--rw-r--r--   0 bbudden    (501) staff       (20)     1062 2023-01-26 02:12:38.000000 codedapertures-0.5/LICENSE
--rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-28 00:11:12.507484 codedapertures-0.5/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)     1743 2023-07-25 00:21:35.000000 codedapertures-0.5/README.md
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-28 00:11:12.506647 codedapertures-0.5/codedapertures/
--rw-r--r--   0 bbudden    (501) staff       (20)       30 2023-01-26 02:12:38.000000 codedapertures-0.5/codedapertures/__init__.py
--rw-r--r--   0 bbudden    (501) staff       (20)    20181 2023-07-27 23:50:09.000000 codedapertures-0.5/codedapertures/codedapertures.py
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-28 00:11:12.507354 codedapertures-0.5/codedapertures.egg-info/
--rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-28 00:11:12.000000 codedapertures-0.5/codedapertures.egg-info/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)      312 2023-07-28 00:11:12.000000 codedapertures-0.5/codedapertures.egg-info/SOURCES.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-28 00:11:12.000000 codedapertures-0.5/codedapertures.egg-info/dependency_links.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-06 00:30:22.000000 codedapertures-0.5/codedapertures.egg-info/not-zip-safe
--rw-r--r--   0 bbudden    (501) staff       (20)       26 2023-07-28 00:11:12.000000 codedapertures-0.5/codedapertures.egg-info/requires.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       15 2023-07-28 00:11:12.000000 codedapertures-0.5/codedapertures.egg-info/top_level.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       38 2023-07-28 00:11:12.507624 codedapertures-0.5/setup.cfg
--rw-r--r--   0 bbudden    (501) staff       (20)      891 2023-07-28 00:08:18.000000 codedapertures-0.5/setup.py
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-29 02:50:48.012690 codedapertures-0.6/
+-rw-r--r--   0 bbudden    (501) staff       (20)     1062 2023-01-26 02:12:38.000000 codedapertures-0.6/LICENSE
+-rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-29 02:50:48.012580 codedapertures-0.6/PKG-INFO
+-rw-r--r--   0 bbudden    (501) staff       (20)     2041 2023-07-29 01:49:47.000000 codedapertures-0.6/README.md
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-29 02:50:48.011694 codedapertures-0.6/codedapertures/
+-rw-r--r--   0 bbudden    (501) staff       (20)       30 2023-01-26 02:12:38.000000 codedapertures-0.6/codedapertures/__init__.py
+-rw-r--r--   0 bbudden    (501) staff       (20)    23459 2023-07-29 02:45:59.000000 codedapertures-0.6/codedapertures/codedapertures.py
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-29 02:50:48.012432 codedapertures-0.6/codedapertures.egg-info/
+-rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-29 02:50:47.000000 codedapertures-0.6/codedapertures.egg-info/PKG-INFO
+-rw-r--r--   0 bbudden    (501) staff       (20)      312 2023-07-29 02:50:47.000000 codedapertures-0.6/codedapertures.egg-info/SOURCES.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-29 02:50:47.000000 codedapertures-0.6/codedapertures.egg-info/dependency_links.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-06 00:30:22.000000 codedapertures-0.6/codedapertures.egg-info/not-zip-safe
+-rw-r--r--   0 bbudden    (501) staff       (20)       40 2023-07-29 02:50:47.000000 codedapertures-0.6/codedapertures.egg-info/requires.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)       15 2023-07-29 02:50:47.000000 codedapertures-0.6/codedapertures.egg-info/top_level.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)       38 2023-07-29 02:50:48.012721 codedapertures-0.6/setup.cfg
+-rw-r--r--   0 bbudden    (501) staff       (20)      923 2023-07-29 02:49:32.000000 codedapertures-0.6/setup.py
```

### Comparing `codedapertures-0.5/LICENSE` & `codedapertures-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `codedapertures-0.5/PKG-INFO` & `codedapertures-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedapertures
-Version: 0.5
+Version: 0.6
 Summary: a python package for generating coded apertures
 Home-page: https://github.com/bpops/codedapertures
 Author: bpops
 License: MIT
 License-File: LICENSE
 
 CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
```

### Comparing `codedapertures-0.5/README.md` & `codedapertures-0.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -22,8 +22,12 @@
 
 URA pattern: E. E. Fenimore and T. M. Cannon, "Coded aperture imaging with uniformly redundant arrays," Appl. Opt. 17, 337-347 (1978).
 
 MURA pattern:  E.E. Fenimore and S. R. Gottesman, "New family of binary arrays for coded aperture imaging" Appl. Opt. 28 (20): 4344-4352 (1989).
 
 SHURA and HURA pattern: M.H. Finger and T.A. Prince, "Hexagonal Uniformly Redundant Arrays for Coded-Aperture Imaging," Proc. 19th Int. Cosmic Ray Conf., 3: 295-298 (1985).
 
+PNP pattern: "PNP - A new class of coded aperture arrays," S. Gottesman and E. Schneid, IEEE Trans. Nucl. Sci., 33(1): 745-749 (1986).
+
+Pseudo-Random Sequences and Primitive Polynomials: F.J. MacWilliams and N.J.A. Sloane, "Pseudo-Random Sequences and Arrays", Proc. of the IEEE, 64, 1715 (1976).
+
 This package will use an axial coordinate system for the hexagonal grids. It will follow the concept outlined at https://www.redblobgames.com/grids/hexagons/#map-storage.
```

### Comparing `codedapertures-0.5/codedapertures/codedapertures.py` & `codedapertures-0.6/codedapertures/codedapertures.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 #
 #            a python package for generating coded apertures                                                                        
 #
 #                             MIT license
 #                    https://github.com/bpops/cappy
 #
 
-#import copy
+from   commpy             import pnsequence
+import copy
 import numpy              as     np
 import matplotlib.pyplot  as     plt
 from   matplotlib.patches import RegularPolygon
 import pyprimes
 import random
 
 
@@ -479,15 +480,16 @@
                 if self.l[i,j] in self.D:
                     self.mask[i,j] = 1
 
         # map to axial matrix
         for i in range(self.diam):
             for j in range(self.diam):
                 if (i+j > (self.radius-1)) and (i+j < (self.diam+self.radius)):
-                    # this next line should not work correctly. WHY does it work?
+                    # TODO: this next line should not work correctly. 
+                    # WHY does it work?
                     self.axial_matrix[i,j] = self.mask[i,j]
                 else:
                     self.axial_matrix[i,j] = np.nan
 
         if not quiet: self.report()
 
     def report(self):
@@ -553,18 +555,16 @@
 
             # add hexagon
             hex = RegularPolygon((x, y), numVertices=6, radius=hex_radius, 
                                     orientation=np.radians(60), 
                                     facecolor='w', alpha=0.2, edgecolor='k')
             ax.add_patch(hex)
 
-        plt.xlim(-self.rx,self.rx)
-        plt.ylim(-self.ry,self.ry)
-        #plt.xlim(-10,10)
-        #plt.ylim(-10,10)
+        plt.xlim(-self.rx/1.2,self.rx/1.2)
+        plt.ylim(-self.ry/2.0,self.ry/2.0)
         plt.title(f"SHURA rhombus [o:{self.v}, r:{self.r}]")
         plt.show()
 
     def show(self):
         """
         Plot the mask
         """
@@ -676,7 +676,120 @@
                 ax.add_patch(hex)
 
         # set axis limits
         plt.xlim(-self.radius*hex_vert,self.radius*hex_vert)
         plt.ylim(-self.radius,self.radius)
         plt.title(f"Random Hex Array [diam: {self.diam}, fill: {self.actual_fill:.2f}]")
         plt.show()
+
+class pnp():
+    """
+    Pseudo-Noise Product Array
+
+    Paramters
+    ---------
+    m : int
+        degree of a_i
+    n : int
+        degree of b_i
+    mult : int
+        how many times to tile the array (default: 2)
+    """
+
+    def __init__(self, m, n, mult=2):
+
+        # generate primitive polynomials
+        self.m = m
+        self.n = n
+        a = prim_poly(m)
+        b = prim_poly(n)
+        self.r = len(a)
+        self.s = len(b)
+
+        # generate mask
+        self.mask = np.zeros((self.r,self.s))
+        for i in range(self.r):
+            for j in range(self.s):
+                self.mask[i,j] = a[i]*b[j]
+        self.mask = np.roll(self.mask,(-(m-2),-(n-2)), axis=(0,1))
+
+        # tile array
+        self.mask = np.tile(self.mask, (mult, mult))
+        self.mask = np.roll(self.mask, (-int(self.mask.shape[0]/4.0)-1,
+                                        -int(self.mask.shape[1]/4.0)-1),
+                                        axis=(0,1))
+
+        self.report()
+
+    def report(self):
+        """
+        Report the array info
+        """
+        print("Pseudo-Noise Product Array")
+        print(f"m: {self.m}")
+        print(f"n: {self.n}")
+        print(f"r (m width): {self.r}")
+        print(f"s (n width): {self.s}")
+
+    def show(self, inverse=False, size=5):
+        """
+        Plots the mask to the screen
+
+        Parameters
+        ----------
+        inverse : bool
+            if True, will invert the array before plotting
+        size : int
+            size of the plot (default 8)
+        """
+        plt.rcParams['figure.figsize'] = [size,size]
+        cmap = "binary_r" if inverse else "binary"
+        plt.imshow(self.mask, cmap="gray", origin='lower', aspect=1)
+        plt.axis('off')
+        plt.title(f"Pseudo-Noise Product Array [m: {self.m}, n: {self.n}]")
+        plt.show()
+        
+
+def prim_poly(m):
+    """
+    Primitive Polynomial
+
+    Parameters
+    ----------
+    m : int
+        degree
+
+    Returns
+    -------
+    pnsequence : ndarray
+        a pseudo-random sequence satisfying the primitive polynomial of the
+        degree specified
+    """
+
+    length = 2**m-1
+
+    # define the first 40 primitive polynomial indices here
+    h_x = {1:(0), 2:(1,0), 3:(1,0), 4:(1,0), 5:(2,0), 6:(1,0), 7:(1,0),
+           8:(6,5,1,0), 9:(4,0), 10:(3,0), 11:(2,0), 12:(7,4,3,0),
+           13:(4,3,1,0), 14:(12,11,1,0), 15:(1,0), 16:(5,3,2,0), 17:(3,0),
+           18:(7,0), 19:(6,5,1,0), 20:(3,0), 21:(2,0), 22:(1,0), 23:(5,0),
+           24:(4,3,1,0), 25:(3,0), 26:(8,7,1,0), 27:(8,7,1,0), 28:(3,0),
+           29:(2,0), 30:(16,15,1,0), 31:(3,0), 32:(28,27,1,0), 33:(13,0), 
+           34:(15,14,1,0), 35:(2,0), 36:(11,0), 37:(12,10,2,0), 38:(6,5,1,0),
+           39:(4,0), 40:(21,19,2,0)}
+    min_m = np.min(list(int(key) for key in h_x.keys()))
+    max_m = np.max(list(int(key) for key in h_x.keys()))
+
+    # check the degree exists
+    if (m < min_m) or (m > max_m):
+        raise ValueError(f"degree must be betweeen {min_m} and {max_m}")
+
+    # generate mask for this degree
+    mask = np.zeros(m)
+    for i in h_x[m]:
+        mask[m-i-1] = 1
+
+    # initialize seed to match results from [MacWilliams 1976]
+    seed = np.zeros(m)
+    seed[0] = 1
+
+    return pnsequence(m,seed,mask,2**m-1)
```

### Comparing `codedapertures-0.5/codedapertures.egg-info/PKG-INFO` & `codedapertures-0.6/codedapertures.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedapertures
-Version: 0.5
+Version: 0.6
 Summary: a python package for generating coded apertures
 Home-page: https://github.com/bpops/codedapertures
 Author: bpops
 License: MIT
 License-File: LICENSE
 
 CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
```

### Comparing `codedapertures-0.5/setup.py` & `codedapertures-0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import setuptools
 
 setuptools.setup(name='codedapertures',
-      version='0.5',
+      version='0.6',
       description='a python package for generating coded apertures',
       long_description='CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.',
       url='https://github.com/bpops/codedapertures',
       author='bpops',
       license='MIT',
       install_requires=['pyprimes',
                 'numpy',
-                'matplotlib'],
-      zip_safe=False)
+                'matplotlib',
+                'scikit-commpy'],
+      zip_safe=False)
```

