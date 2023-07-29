# Comparing `tmp/firefox_bookmarks-1.0.0.tar.gz` & `tmp/firefox_bookmarks-1.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefox_bookmarks-1.0.0.tar", max compression
+gzip compressed data, was "firefox_bookmarks-1.0.0.post1.tar", max compression
```

## Comparing `firefox_bookmarks-1.0.0.tar` & `firefox_bookmarks-1.0.0.post1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    19028 2023-07-29 20:13:57.122984 firefox_bookmarks-1.0.0/firefox_bookmarks/__init__.py
--rw-r--r--   0        0        0     4451 2023-07-29 20:13:57.138108 firefox_bookmarks-1.0.0/firefox_bookmarks/bookmark.py
--rw-r--r--   0        0        0     1268 2023-07-25 08:53:37.841063 firefox_bookmarks-1.0.0/firefox_bookmarks/connect.py
--rw-r--r--   0        0        0      437 2023-07-29 20:50:08.340724 firefox_bookmarks-1.0.0/firefox_bookmarks/constants.py
--rw-r--r--   0        0        0     2391 2023-07-24 14:39:36.813164 firefox_bookmarks-1.0.0/firefox_bookmarks/locate.py
--rw-r--r--   0        0        0     3974 2023-07-29 20:13:57.164801 firefox_bookmarks-1.0.0/firefox_bookmarks/models.py
--rw-r--r--   0        0        0    35184 2023-07-21 16:18:12.325494 firefox_bookmarks-1.0.0/LICENSE
--rw-r--r--   0        0        0     1417 2023-07-29 20:48:57.651905 firefox_bookmarks-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2503 2023-07-29 20:39:23.972578 firefox_bookmarks-1.0.0/README.md
--rw-r--r--   0        0        0     3921 1970-01-01 00:00:00.000000 firefox_bookmarks-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    19028 2023-07-29 20:13:57.122984 firefox_bookmarks-1.0.0.post1/firefox_bookmarks/__init__.py
+-rw-r--r--   0        0        0     4451 2023-07-29 20:13:57.138108 firefox_bookmarks-1.0.0.post1/firefox_bookmarks/bookmark.py
+-rw-r--r--   0        0        0     1268 2023-07-25 08:53:37.841063 firefox_bookmarks-1.0.0.post1/firefox_bookmarks/connect.py
+-rw-r--r--   0        0        0      437 2023-07-29 21:08:46.723557 firefox_bookmarks-1.0.0.post1/firefox_bookmarks/constants.py
+-rw-r--r--   0        0        0     2391 2023-07-24 14:39:36.813164 firefox_bookmarks-1.0.0.post1/firefox_bookmarks/locate.py
+-rw-r--r--   0        0        0     3974 2023-07-29 20:13:57.164801 firefox_bookmarks-1.0.0.post1/firefox_bookmarks/models.py
+-rw-r--r--   0        0        0    35184 2023-07-21 16:18:12.325494 firefox_bookmarks-1.0.0.post1/LICENSE
+-rw-r--r--   0        0        0     1423 2023-07-29 21:03:36.778493 firefox_bookmarks-1.0.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     2059 2023-07-29 21:08:19.526471 firefox_bookmarks-1.0.0.post1/README.md
+-rw-r--r--   0        0        0     3496 1970-01-01 00:00:00.000000 firefox_bookmarks-1.0.0.post1/PKG-INFO
```

### Comparing `firefox_bookmarks-1.0.0/firefox_bookmarks/__init__.py` & `firefox_bookmarks-1.0.0.post1/firefox_bookmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `firefox_bookmarks-1.0.0/firefox_bookmarks/bookmark.py` & `firefox_bookmarks-1.0.0.post1/firefox_bookmarks/bookmark.py`

 * *Files identical despite different names*

### Comparing `firefox_bookmarks-1.0.0/firefox_bookmarks/connect.py` & `firefox_bookmarks-1.0.0.post1/firefox_bookmarks/connect.py`

 * *Files identical despite different names*

### Comparing `firefox_bookmarks-1.0.0/firefox_bookmarks/locate.py` & `firefox_bookmarks-1.0.0.post1/firefox_bookmarks/locate.py`

 * *Files identical despite different names*

### Comparing `firefox_bookmarks-1.0.0/firefox_bookmarks/models.py` & `firefox_bookmarks-1.0.0.post1/firefox_bookmarks/models.py`

 * *Files identical despite different names*

### Comparing `firefox_bookmarks-1.0.0/LICENSE` & `firefox_bookmarks-1.0.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `firefox_bookmarks-1.0.0/pyproject.toml` & `firefox_bookmarks-1.0.0.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firefox-bookmarks"
-version = "1.0.0"
+version = "1.0.0.post1"
 description = "Manage your Firefox bookmarks with ease"
 authors = ["Aditya Rajput <adiraj20072002@gmail.com>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [{ include = "firefox_bookmarks" }]
 repository = "https://github.com/BURG3R5/firefox-bookmarks"
 documentation = "https://github.com/BURG3R5/firefox-bookmarks"
```

### Comparing `firefox_bookmarks-1.0.0/README.md` & `firefox_bookmarks-1.0.0.post1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,157 +1,129 @@
-00000000: 2320 6669 7265 666f 782d 626f 6f6b 6d61  # firefox-bookma
-00000010: 726b 730d 0a0d 0a3c 7020 616c 6967 6e3d  rks....<p align=
-00000020: 2263 656e 7465 7222 3e0d 0a20 2020 203c  "center">..    <
-00000030: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000040: 6769 7468 7562 2e63 6f6d 2f42 5552 4733  github.com/BURG3
-00000050: 5235 2f66 6972 6566 6f78 2d62 6f6f 6b6d  R5/firefox-bookm
-00000060: 6172 6b73 2f61 6374 696f 6e73 2f77 6f72  arks/actions/wor
-00000070: 6b66 6c6f 7773 2f63 692e 796d 6c22 3e0d  kflows/ci.yml">.
-00000080: 0a20 2020 2020 2020 203c 696d 6720 616c  .        <img al
-00000090: 743d 2243 4920 5374 6174 7573 2220 7372  t="CI Status" sr
-000000a0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-000000b0: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-000000c0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-000000d0: 772f 7374 6174 7573 2f42 5552 4733 5235  w/status/BURG3R5
-000000e0: 2f66 6972 6566 6f78 2d62 6f6f 6b6d 6172  /firefox-bookmar
-000000f0: 6b73 2f63 692e 796d 6c3f 6272 616e 6368  ks/ci.yml?branch
-00000100: 3d6d 6169 6e26 7374 796c 653d 666c 6174  =main&style=flat
-00000110: 2d73 7175 6172 6522 3e0d 0a20 2020 203c  -square">..    <
-00000120: 2f61 3e0d 0a20 2020 203c 6120 6872 6566  /a>..    <a href
-00000130: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00000140: 2e63 6f6d 2f42 5552 4733 5235 2f66 6972  .com/BURG3R5/fir
-00000150: 6566 6f78 2d62 6f6f 6b6d 6172 6b73 2f62  efox-bookmarks/b
-00000160: 6c6f 622f 6d61 696e 2f4c 4943 454e 5345  lob/main/LICENSE
-00000170: 223e 0d0a 2020 2020 2020 2020 3c69 6d67  ">..        <img
-00000180: 2061 6c74 3d22 4c69 6365 6e73 6520 2d20   alt="License - 
-00000190: 4147 504c 2076 3320 6f72 206c 6174 6572  AGPL v3 or later
-000001a0: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-000001b0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000001c0: 7069 2f6c 2f66 6972 6566 6f78 2d62 6f6f  pi/l/firefox-boo
-000001d0: 6b6d 6172 6b73 3f73 7479 6c65 3d66 6c61  kmarks?style=fla
-000001e0: 742d 7371 7561 7265 223e 0d0a 2020 2020  t-square">..    
-000001f0: 3c2f 613e 0d0a 2020 2020 3c61 2068 7265  </a>..    <a hre
-00000200: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
-00000210: 6f72 672f 7072 6f6a 6563 742f 6669 7265  org/project/fire
-00000220: 666f 782d 626f 6f6b 6d61 726b 732f 223e  fox-bookmarks/">
-00000230: 0d0a 2020 2020 2020 2020 3c69 6d67 2061  ..        <img a
-00000240: 6c74 3d22 5079 5049 2220 7372 633d 2268  lt="PyPI" src="h
-00000250: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000260: 6473 2e69 6f2f 7079 7069 2f76 2f66 6972  ds.io/pypi/v/fir
-00000270: 6566 6f78 2d62 6f6f 6b6d 6172 6b73 3f73  efox-bookmarks?s
-00000280: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
-00000290: 223e 0d0a 2020 2020 3c2f 613e 0d0a 2020  ">..    </a>..  
-000002a0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-000002b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 676f  ://github.com/go
-000002c0: 6f67 6c65 2f79 6170 6622 3e0d 0a20 2020  ogle/yapf">..   
-000002d0: 2020 2020 203c 696d 6720 616c 743d 2243       <img alt="C
-000002e0: 6f64 6520 7374 796c 653a 2059 4150 4622  ode style: YAPF"
-000002f0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00000300: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000310: 6765 2f63 6f64 6525 3230 7374 796c 652d  ge/code%20style-
-00000320: 7961 7066 2d62 6c75 653f 7374 796c 653d  yapf-blue?style=
-00000330: 666c 6174 2d73 7175 6172 6522 3e0d 0a20  flat-square">.. 
-00000340: 2020 203c 2f61 3e0d 0a20 2020 203c 2f61     </a>..    </a
-00000350: 3e0d 0a20 2020 203c 6120 6872 6566 3d22  >..    <a href="
-00000360: 6874 7470 733a 2f2f 7079 6371 612e 6769  https://pycqa.gi
-00000370: 7468 7562 2e69 6f2f 6973 6f72 7422 3e0d  thub.io/isort">.
-00000380: 0a20 2020 2020 2020 203c 696d 6720 616c  .        <img al
-00000390: 743d 2243 6f64 6520 7374 796c 653a 2069  t="Code style: i
-000003a0: 736f 7274 2220 7372 633d 2268 7474 7073  sort" src="https
-000003b0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-000003c0: 6f2f 6261 6467 652f 2532 3069 6d70 6f72  o/badge/%20impor
-000003d0: 7473 2d69 736f 7274 2d25 3233 3136 3734  ts-isort-%231674
-000003e0: 6231 3f73 7479 6c65 3d66 6c61 742d 7371  b1?style=flat-sq
-000003f0: 7561 7265 223e 0d0a 2020 2020 3c2f 613e  uare">..    </a>
-00000400: 0d0a 3c2f 703e 0d0a 0d0a 4d61 6e61 6765  ..</p>....Manage
-00000410: 2079 6f75 7220 4669 7265 666f 7820 626f   your Firefox bo
-00000420: 6f6b 6d61 726b 7320 7769 7468 2065 6173  okmarks with eas
-00000430: 650d 0a0d 0a23 2320 696e 7374 616c 6c61  e....## installa
-00000440: 7469 6f6e 0d0a 0d0a 6060 6073 6865 6c6c  tion....```shell
-00000450: 0d0a 7069 7020 696e 7374 616c 6c20 6669  ..pip install fi
-00000460: 7265 666f 782d 626f 6f6b 6d61 726b 730d  refox-bookmarks.
-00000470: 0a60 6060 0d0a 0d0a 2323 2075 7361 6765  .```....## usage
-00000480: 0d0a 0d0a 496d 706f 7274 2061 6e64 2069  ....Import and i
-00000490: 6e69 7469 616c 697a 653a 0d0a 0d0a 6060  nitialize:....``
-000004a0: 6070 7974 686f 6e0d 0a66 726f 6d20 6669  `python..from fi
-000004b0: 7265 666f 785f 626f 6f6b 6d61 726b 7320  refox_bookmarks 
-000004c0: 696d 706f 7274 202a 0d0a 0d0a 6662 203d  import *....fb =
-000004d0: 2046 6972 6566 6f78 426f 6f6b 6d61 726b   FirefoxBookmark
-000004e0: 7328 290d 0a0d 0a23 2059 6f75 2063 616e  s()....# You can
-000004f0: 2070 6173 7320 6120 6050 726f 6669 6c65   pass a `Profile
-00000500: 4372 6974 6572 696f 6e60 2074 6f20 6368  Criterion` to ch
-00000510: 6f6f 7365 2066 726f 6d20 6d75 6c74 6970  oose from multip
-00000520: 6c65 2070 726f 6669 6c65 730d 0a66 622e  le profiles..fb.
-00000530: 636f 6e6e 6563 7428 6372 6974 6572 696f  connect(criterio
-00000540: 6e3d 5072 6f66 696c 6543 7269 7465 7269  n=ProfileCriteri
-00000550: 6f6e 2e4c 4152 4745 5354 290d 0a60 6060  on.LARGEST)..```
-00000560: 0d0a 0d0a 5175 6572 7920 6173 2079 6f75  ....Query as you
-00000570: 2077 6f75 6c64 2069 6e20 7065 6577 6565   would in peewee
-00000580: 2028 6f72 2044 6a61 6e67 6f20 6f72 2053   (or Django or S
-00000590: 514c 416c 6368 656d 7929 0d0a 0d0a 6060  QLAlchemy)....``
-000005a0: 6070 7974 686f 6e0d 0a67 6974 6875 625f  `python..github_
-000005b0: 626f 6f6b 6d61 726b 7320 3d20 6662 2e62  bookmarks = fb.b
-000005c0: 6f6f 6b6d 6172 6b73 280d 0a20 2020 2077  ookmarks(..    w
-000005d0: 6865 7265 3d42 6f6f 6b6d 6172 6b2e 7572  here=Bookmark.ur
-000005e0: 6c2e 636f 6e74 6169 6e73 2822 6874 7470  l.contains("http
-000005f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2229  s://github.com")
-00000600: 2c0d 0a29 0d0a 0d0a 666f 7220 626f 6f6b  ,..)....for book
-00000610: 6d61 726b 2069 6e20 6769 7468 7562 5f62  mark in github_b
-00000620: 6f6f 6b6d 6172 6b73 3a0d 0a20 2020 2070  ookmarks:..    p
-00000630: 7269 6e74 2866 2254 6974 6c65 3a20 7b62  rint(f"Title: {b
-00000640: 6f6f 6b6d 6172 6b2e 7469 746c 657d 5c6e  ookmark.title}\n
-00000650: 5552 4c3a 207b 626f 6f6b 6d61 726b 2e75  URL: {bookmark.u
-00000660: 726c 7d5c 6e22 290d 0a60 6060 0d0a 0d0a  rl}\n")..```....
-00000670: 2323 2065 7861 6d70 6c65 730d 0a0d 0a53  ## examples....S
-00000680: 6565 205b 7468 6520 6578 616d 706c 6573  ee [the examples
-00000690: 2064 6972 6563 746f 7279 5d28 6874 7470   directory](http
-000006a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f42  s://github.com/B
-000006b0: 5552 4733 5235 2f66 6972 6566 6f78 2d62  URG3R5/firefox-b
-000006c0: 6f6f 6b6d 6172 6b73 2f74 7265 652f 6d61  ookmarks/tree/ma
-000006d0: 696e 2f65 7861 6d70 6c65 7329 0d0a 0d0a  in/examples)....
-000006e0: 2323 2063 6f6e 7472 6962 7574 696e 670d  ## contributing.
-000006f0: 0a0d 0a57 616e 7420 746f 2066 6978 2061  ...Want to fix a
-00000700: 2062 7567 2c20 6164 6420 6120 6665 6174   bug, add a feat
-00000710: 7572 652c 206f 7220 696d 7072 6f76 6520  ure, or improve 
-00000720: 646f 6375 6d65 6e74 6174 696f 6e3f 2041  documentation? A
-00000730: 7765 736f 6d65 2120 5265 6164 2075 7020  wesome! Read up 
-00000740: 6f6e 206f 7572 205b 6775 6964 656c 696e  on our [guidelin
-00000750: 6573 2066 6f72 2063 6f6e 7472 6962 7574  es for contribut
-00000760: 696e 675d 2868 7474 7073 3a2f 2f67 6974  ing](https://git
-00000770: 6875 622e 636f 6d2f 4255 5247 3352 352f  hub.com/BURG3R5/
-00000780: 6669 7265 666f 782d 626f 6f6b 6d61 726b  firefox-bookmark
-00000790: 732f 626c 6f62 2f6d 6169 6e2f 2e67 6974  s/blob/main/.git
-000007a0: 6875 622f 434f 4e54 5249 4255 5449 4e47  hub/CONTRIBUTING
-000007b0: 2e6d 6429 2061 6e64 2074 6865 6e20 7669  .md) and then vi
-000007c0: 7369 7420 6f75 7220 5b2f 636f 6e74 7269  sit our [/contri
-000007d0: 6275 7465 2070 6167 655d 2868 7474 7073  bute page](https
-000007e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4255  ://github.com/BU
-000007f0: 5247 3352 352f 6669 7265 666f 782d 626f  RG3R5/firefox-bo
-00000800: 6f6b 6d61 726b 732f 636f 6e74 7269 6275  okmarks/contribu
-00000810: 7465 2920 746f 2066 696e 6420 676f 6f64  te) to find good
-00000820: 2066 6972 7374 2069 7373 7565 7321 2050   first issues! P
-00000830: 756c 6c20 7265 7175 6573 7473 2061 7265  ull requests are
-00000840: 2061 6c77 6179 7320 7765 6c63 6f6d 6521   always welcome!
-00000850: 0d0a 0d0a 2323 206c 6963 656e 7365 0d0a  ....## license..
-00000860: 0d0a 436f 7079 7269 6768 7420 2843 2920  ..Copyright (C) 
-00000870: 3230 3233 2041 6469 7479 6120 5261 6a70  2023 Aditya Rajp
-00000880: 7574 2026 206f 7468 6572 2063 6f6e 7472  ut & other contr
-00000890: 6962 7574 6f72 730d 0a0d 0a54 6869 7320  ibutors....This 
-000008a0: 736f 6674 7761 7265 2069 7320 6c69 6365  software is lice
-000008b0: 6e73 6564 2075 6e64 6572 2074 6865 202a  nsed under the *
-000008c0: 2a41 6666 6572 6f20 4750 4c20 7633 2a2a  *Affero GPL v3**
-000008d0: 2e20 596f 7520 7368 6f75 6c64 2068 6176  . You should hav
-000008e0: 6520 7265 6365 6976 6564 205b 6120 636f  e received [a co
-000008f0: 7079 5d28 6874 7470 733a 2f2f 6769 7468  py](https://gith
-00000900: 7562 2e63 6f6d 2f42 5552 4733 5235 2f66  ub.com/BURG3R5/f
-00000910: 6972 6566 6f78 2d62 6f6f 6b6d 6172 6b73  irefox-bookmarks
-00000920: 2f62 6c6f 622f 6d61 696e 2f4c 4943 454e  /blob/main/LICEN
-00000930: 5345 2920 6f66 2074 6865 2041 6666 6572  SE) of the Affer
-00000940: 6f20 4750 4c20 7633 2061 6c6f 6e67 2077  o GPL v3 along w
-00000950: 6974 6820 7468 6973 2070 726f 6772 616d  ith this program
-00000960: 2e20 4966 206e 6f74 2c20 796f 7520 6361  . If not, you ca
-00000970: 6e20 7669 7369 7420 7468 6520 6f72 6967  n visit the orig
-00000980: 696e 616c 205b 6865 7265 5d28 6874 7470  inal [here](http
-00000990: 733a 2f2f 7777 772e 676e 752e 6f72 672f  s://www.gnu.org/
-000009a0: 6c69 6365 6e73 6573 2f61 6770 6c2d 332e  licenses/agpl-3.
-000009b0: 302e 6874 6d6c 236c 6963 656e 7365 2d74  0.html#license-t
-000009c0: 6578 7429 2e0d 0a                        ext)...
+00000000: 3c69 6d67 2061 6c74 3d22 4349 2053 7461  <img alt="CI Sta
+00000010: 7475 7322 2073 7263 3d22 6874 7470 733a  tus" src="https:
+00000020: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000030: 2f67 6974 6875 622f 6163 7469 6f6e 732f  /github/actions/
+00000040: 776f 726b 666c 6f77 2f73 7461 7475 732f  workflow/status/
+00000050: 4255 5247 3352 352f 6669 7265 666f 782d  BURG3R5/firefox-
+00000060: 626f 6f6b 6d61 726b 732f 6369 2e79 6d6c  bookmarks/ci.yml
+00000070: 3f62 7261 6e63 683d 6d61 696e 2673 7479  ?branch=main&sty
+00000080: 6c65 3d66 6c61 742d 7371 7561 7265 223e  le=flat-square">
+00000090: 0d0a 3c69 6d67 2061 6c74 3d22 5079 5049  ..<img alt="PyPI
+000000a0: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+000000b0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+000000c0: 7069 2f76 2f66 6972 6566 6f78 2d62 6f6f  pi/v/firefox-boo
+000000d0: 6b6d 6172 6b73 3f73 7479 6c65 3d66 6c61  kmarks?style=fla
+000000e0: 742d 7371 7561 7265 223e 0d0a 3c69 6d67  t-square">..<img
+000000f0: 2061 6c74 3d22 4c69 6365 6e73 6520 2d20   alt="License - 
+00000100: 4147 504c 2076 3320 6f72 206c 6174 6572  AGPL v3 or later
+00000110: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+00000120: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000130: 7069 2f6c 2f66 6972 6566 6f78 2d62 6f6f  pi/l/firefox-boo
+00000140: 6b6d 6172 6b73 3f73 7479 6c65 3d66 6c61  kmarks?style=fla
+00000150: 742d 7371 7561 7265 223e 0d0a 3c69 6d67  t-square">..<img
+00000160: 2061 6c74 3d22 436f 6465 2073 7479 6c65   alt="Code style
+00000170: 3a20 5941 5046 2220 7372 633d 2268 7474  : YAPF" src="htt
+00000180: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000190: 2e69 6f2f 6261 6467 652f 636f 6465 2532  .io/badge/code%2
+000001a0: 3073 7479 6c65 2d79 6170 662d 626c 7565  0style-yapf-blue
+000001b0: 3f73 7479 6c65 3d66 6c61 742d 7371 7561  ?style=flat-squa
+000001c0: 7265 223e 0d0a 3c69 6d67 2061 6c74 3d22  re">..<img alt="
+000001d0: 436f 6465 2073 7479 6c65 3a20 6973 6f72  Code style: isor
+000001e0: 7422 2073 7263 3d22 6874 7470 733a 2f2f  t" src="https://
+000001f0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000200: 6164 6765 2f25 3230 696d 706f 7274 732d  adge/%20imports-
+00000210: 6973 6f72 742d 2532 3331 3637 3462 313f  isort-%231674b1?
+00000220: 7374 796c 653d 666c 6174 2d73 7175 6172  style=flat-squar
+00000230: 6522 3e0d 0a0d 0a23 2066 6972 6566 6f78  e">....# firefox
+00000240: 2d62 6f6f 6b6d 6172 6b73 0d0a 0d0a 4d61  -bookmarks....Ma
+00000250: 6e61 6765 2079 6f75 7220 4669 7265 666f  nage your Firefo
+00000260: 7820 626f 6f6b 6d61 726b 7320 7769 7468  x bookmarks with
+00000270: 2065 6173 650d 0a0d 0a23 2320 696e 7374   ease....## inst
+00000280: 616c 6c61 7469 6f6e 0d0a 0d0a 6060 6073  allation....```s
+00000290: 6865 6c6c 0d0a 7069 7020 696e 7374 616c  hell..pip instal
+000002a0: 6c20 6669 7265 666f 782d 626f 6f6b 6d61  l firefox-bookma
+000002b0: 726b 730d 0a60 6060 0d0a 0d0a 2323 2075  rks..```....## u
+000002c0: 7361 6765 0d0a 0d0a 496d 706f 7274 2061  sage....Import a
+000002d0: 6e64 2069 6e69 7469 616c 697a 653a 0d0a  nd initialize:..
+000002e0: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
+000002f0: 6d20 6669 7265 666f 785f 626f 6f6b 6d61  m firefox_bookma
+00000300: 726b 7320 696d 706f 7274 202a 0d0a 0d0a  rks import *....
+00000310: 6662 203d 2046 6972 6566 6f78 426f 6f6b  fb = FirefoxBook
+00000320: 6d61 726b 7328 290d 0a0d 0a23 2059 6f75  marks()....# You
+00000330: 2063 616e 2070 6173 7320 6120 6050 726f   can pass a `Pro
+00000340: 6669 6c65 4372 6974 6572 696f 6e60 2074  fileCriterion` t
+00000350: 6f20 6368 6f6f 7365 2066 726f 6d20 6d75  o choose from mu
+00000360: 6c74 6970 6c65 2070 726f 6669 6c65 730d  ltiple profiles.
+00000370: 0a66 622e 636f 6e6e 6563 7428 6372 6974  .fb.connect(crit
+00000380: 6572 696f 6e3d 5072 6f66 696c 6543 7269  erion=ProfileCri
+00000390: 7465 7269 6f6e 2e4c 4152 4745 5354 290d  terion.LARGEST).
+000003a0: 0a60 6060 0d0a 0d0a 5175 6572 7920 6173  .```....Query as
+000003b0: 2079 6f75 2077 6f75 6c64 2069 6e20 7065   you would in pe
+000003c0: 6577 6565 2028 6f72 2044 6a61 6e67 6f20  ewee (or Django 
+000003d0: 6f72 2053 514c 416c 6368 656d 7929 0d0a  or SQLAlchemy)..
+000003e0: 0d0a 6060 6070 7974 686f 6e0d 0a67 6974  ..```python..git
+000003f0: 6875 625f 626f 6f6b 6d61 726b 7320 3d20  hub_bookmarks = 
+00000400: 6662 2e62 6f6f 6b6d 6172 6b73 280d 0a20  fb.bookmarks(.. 
+00000410: 2020 2077 6865 7265 3d42 6f6f 6b6d 6172     where=Bookmar
+00000420: 6b2e 7572 6c2e 636f 6e74 6169 6e73 2822  k.url.contains("
+00000430: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000440: 6f6d 2229 2c0d 0a29 0d0a 0d0a 666f 7220  om"),..)....for 
+00000450: 626f 6f6b 6d61 726b 2069 6e20 6769 7468  bookmark in gith
+00000460: 7562 5f62 6f6f 6b6d 6172 6b73 3a0d 0a20  ub_bookmarks:.. 
+00000470: 2020 2070 7269 6e74 2866 2254 6974 6c65     print(f"Title
+00000480: 3a20 7b62 6f6f 6b6d 6172 6b2e 7469 746c  : {bookmark.titl
+00000490: 657d 5c6e 5552 4c3a 207b 626f 6f6b 6d61  e}\nURL: {bookma
+000004a0: 726b 2e75 726c 7d5c 6e22 290d 0a60 6060  rk.url}\n")..```
+000004b0: 0d0a 0d0a 2323 2065 7861 6d70 6c65 730d  ....## examples.
+000004c0: 0a0d 0a53 6565 205b 7468 6520 6578 616d  ...See [the exam
+000004d0: 706c 6573 2064 6972 6563 746f 7279 5d28  ples directory](
+000004e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000004f0: 6f6d 2f42 5552 4733 5235 2f66 6972 6566  om/BURG3R5/firef
+00000500: 6f78 2d62 6f6f 6b6d 6172 6b73 2f74 7265  ox-bookmarks/tre
+00000510: 652f 6d61 696e 2f65 7861 6d70 6c65 7329  e/main/examples)
+00000520: 0d0a 0d0a 2323 2063 6f6e 7472 6962 7574  ....## contribut
+00000530: 696e 670d 0a0d 0a57 616e 7420 746f 2066  ing....Want to f
+00000540: 6978 2061 2062 7567 2c20 6164 6420 6120  ix a bug, add a 
+00000550: 6665 6174 7572 652c 206f 7220 696d 7072  feature, or impr
+00000560: 6f76 6520 646f 6375 6d65 6e74 6174 696f  ove documentatio
+00000570: 6e3f 2041 7765 736f 6d65 2120 5265 6164  n? Awesome! Read
+00000580: 2075 7020 6f6e 206f 7572 205b 6775 6964   up on our [guid
+00000590: 656c 696e 6573 2066 6f72 2063 6f6e 7472  elines for contr
+000005a0: 6962 7574 696e 675d 2868 7474 7073 3a2f  ibuting](https:/
+000005b0: 2f67 6974 6875 622e 636f 6d2f 4255 5247  /github.com/BURG
+000005c0: 3352 352f 6669 7265 666f 782d 626f 6f6b  3R5/firefox-book
+000005d0: 6d61 726b 732f 626c 6f62 2f6d 6169 6e2f  marks/blob/main/
+000005e0: 2e67 6974 6875 622f 434f 4e54 5249 4255  .github/CONTRIBU
+000005f0: 5449 4e47 2e6d 6429 2061 6e64 2074 6865  TING.md) and the
+00000600: 6e20 7669 7369 7420 6f75 7220 5b2f 636f  n visit our [/co
+00000610: 6e74 7269 6275 7465 2070 6167 655d 2868  ntribute page](h
+00000620: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000630: 6d2f 4255 5247 3352 352f 6669 7265 666f  m/BURG3R5/firefo
+00000640: 782d 626f 6f6b 6d61 726b 732f 636f 6e74  x-bookmarks/cont
+00000650: 7269 6275 7465 2920 746f 2066 696e 6420  ribute) to find 
+00000660: 676f 6f64 2066 6972 7374 2069 7373 7565  good first issue
+00000670: 7321 2050 756c 6c20 7265 7175 6573 7473  s! Pull requests
+00000680: 2061 7265 2061 6c77 6179 7320 7765 6c63   are always welc
+00000690: 6f6d 6521 0d0a 0d0a 2323 206c 6963 656e  ome!....## licen
+000006a0: 7365 0d0a 0d0a 436f 7079 7269 6768 7420  se....Copyright 
+000006b0: 2843 2920 3230 3233 2041 6469 7479 6120  (C) 2023 Aditya 
+000006c0: 5261 6a70 7574 2026 206f 7468 6572 2063  Rajput & other c
+000006d0: 6f6e 7472 6962 7574 6f72 730d 0a0d 0a54  ontributors....T
+000006e0: 6869 7320 736f 6674 7761 7265 2069 7320  his software is 
+000006f0: 6c69 6365 6e73 6564 2075 6e64 6572 2074  licensed under t
+00000700: 6865 202a 2a41 6666 6572 6f20 4750 4c20  he **Affero GPL 
+00000710: 7633 2a2a 2e20 596f 7520 7368 6f75 6c64  v3**. You should
+00000720: 2068 6176 6520 7265 6365 6976 6564 205b   have received [
+00000730: 6120 636f 7079 5d28 6874 7470 733a 2f2f  a copy](https://
+00000740: 6769 7468 7562 2e63 6f6d 2f42 5552 4733  github.com/BURG3
+00000750: 5235 2f66 6972 6566 6f78 2d62 6f6f 6b6d  R5/firefox-bookm
+00000760: 6172 6b73 2f62 6c6f 622f 6d61 696e 2f4c  arks/blob/main/L
+00000770: 4943 454e 5345 2920 6f66 2074 6865 2041  ICENSE) of the A
+00000780: 6666 6572 6f20 4750 4c20 7633 2061 6c6f  ffero GPL v3 alo
+00000790: 6e67 2077 6974 6820 7468 6973 2070 726f  ng with this pro
+000007a0: 6772 616d 2e20 4966 206e 6f74 2c20 796f  gram. If not, yo
+000007b0: 7520 6361 6e20 7669 7369 7420 7468 6520  u can visit the 
+000007c0: 6f72 6967 696e 616c 205b 6865 7265 5d28  original [here](
+000007d0: 6874 7470 733a 2f2f 7777 772e 676e 752e  https://www.gnu.
+000007e0: 6f72 672f 6c69 6365 6e73 6573 2f61 6770  org/licenses/agp
+000007f0: 6c2d 332e 302e 6874 6d6c 236c 6963 656e  l-3.0.html#licen
+00000800: 7365 2d74 6578 7429 2e0d 0a              se-text)...
```

