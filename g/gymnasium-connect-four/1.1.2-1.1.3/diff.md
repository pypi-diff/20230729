# Comparing `tmp/gymnasium_connect_four-1.1.2.tar.gz` & `tmp/gymnasium_connect_four-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_connect_four-1.1.2.tar", last modified: Tue Jul 25 19:55:32 2023, max compression
+gzip compressed data, was "gymnasium_connect_four-1.1.3.tar", last modified: Sat Jul 29 07:25:06 2023, max compression
```

## Comparing `gymnasium_connect_four-1.1.2.tar` & `gymnasium_connect_four-1.1.3.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 19:55:32.993559 gymnasium_connect_four-1.1.2/
--rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      251 2023-07-25 19:55:32.992560 gymnasium_connect_four-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     9711 2023-07-25 19:44:27.000000 gymnasium_connect_four-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 19:55:32.971678 gymnasium_connect_four-1.1.2/connect_four_gymnasium/
--rw-rw-rw-   0        0        0     8754 2023-07-25 15:19:05.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/ConnectFourEnv.py
--rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:55:32.984190 gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/
--rw-rw-rw-   0        0        0     4253 2023-07-24 06:32:12.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/AdultPlayer.py
--rw-rw-rw-   0        0        0     3753 2023-07-24 17:50:51.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/AdultSmarterPlayer.py
--rw-rw-rw-   0        0        0      338 2023-07-24 06:32:47.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/BabyPlayer.py
--rw-rw-rw-   0        0        0     1596 2023-07-25 19:50:41.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/ChildPlayer.py
--rw-rw-rw-   0        0        0     1946 2023-07-24 06:32:30.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/ChildSmarterPlayer.py
--rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/ConsolePlayer.py
--rw-rw-rw-   0        0        0     4118 2023-07-24 06:02:34.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/MinMaxPlayer.py
--rw-rw-rw-   0        0        0      545 2023-07-24 21:26:20.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/ModelPlayer.py
--rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/Player.py
--rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/SimulatePlayer.py
--rw-rw-rw-   0        0        0     2609 2023-07-24 06:32:25.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/TeenagerPlayer.py
--rw-rw-rw-   0        0        0     3999 2023-07-24 06:32:20.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
--rw-rw-rw-   0        0        0      486 2023-07-25 11:49:49.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:55:32.985190 gymnasium_connect_four-1.1.2/connect_four_gymnasium/tools/
--rw-rw-rw-   0        0        0     4914 2023-07-25 19:51:32.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/tools/EloLeaderboard.py
--rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.1.2/connect_four_gymnasium/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:55:32.989555 gymnasium_connect_four-1.1.2/gymnasium_connect_four.egg-info/
--rw-rw-rw-   0        0        0      251 2023-07-25 19:55:32.000000 gymnasium_connect_four-1.1.2/gymnasium_connect_four.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1089 2023-07-25 19:55:32.000000 gymnasium_connect_four-1.1.2/gymnasium_connect_four.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 19:55:32.000000 gymnasium_connect_four-1.1.2/gymnasium_connect_four.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-25 19:55:32.000000 gymnasium_connect_four-1.1.2/gymnasium_connect_four.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-25 19:55:32.000000 gymnasium_connect_four-1.1.2/gymnasium_connect_four.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 19:55:32.993559 gymnasium_connect_four-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-07-25 19:54:31.000000 gymnasium_connect_four-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:55:32.991562 gymnasium_connect_four-1.1.2/test/
--rw-rw-rw-   0        0        0    21167 2023-07-25 14:09:28.000000 gymnasium_connect_four-1.1.2/test/test_power_4_logic.py
--rw-rw-rw-   0        0        0     2373 2023-07-23 20:26:41.000000 gymnasium_connect_four-1.1.2/test/test_ppo_env.py
+drwxrwxrwx   0        0        0        0 2023-07-29 07:25:06.970677 gymnasium_connect_four-1.1.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-07-29 07:25:06.969678 gymnasium_connect_four-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11859 2023-07-29 06:01:04.000000 gymnasium_connect_four-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 07:25:06.925670 gymnasium_connect_four-1.1.3/connect_four_gymnasium/
+-rw-rw-rw-   0        0        0     8882 2023-07-29 07:23:53.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/ConnectFourEnv.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 07:25:06.950672 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/
+-rw-rw-rw-   0        0        0     4253 2023-07-24 06:32:12.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/AdultPlayer.py
+-rw-rw-rw-   0        0        0     3753 2023-07-24 17:50:51.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/AdultSmarterPlayer.py
+-rw-rw-rw-   0        0        0      338 2023-07-24 06:32:47.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/BabyPlayer.py
+-rw-rw-rw-   0        0        0     1596 2023-07-25 19:50:41.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/ChildPlayer.py
+-rw-rw-rw-   0        0        0     1946 2023-07-24 06:32:30.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/ChildSmarterPlayer.py
+-rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/ConsolePlayer.py
+-rw-rw-rw-   0        0        0     4118 2023-07-24 06:02:34.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/MinMaxPlayer.py
+-rw-rw-rw-   0        0        0      545 2023-07-24 21:26:20.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/ModelPlayer.py
+-rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/Player.py
+-rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/SimulatePlayer.py
+-rw-rw-rw-   0        0        0     2609 2023-07-24 06:32:25.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/TeenagerPlayer.py
+-rw-rw-rw-   0        0        0     3999 2023-07-24 06:32:20.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
+-rw-rw-rw-   0        0        0      486 2023-07-25 11:49:49.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 07:25:06.953671 gymnasium_connect_four-1.1.3/connect_four_gymnasium/tools/
+-rw-rw-rw-   0        0        0     4914 2023-07-25 19:51:32.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/tools/EloLeaderboard.py
+-rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 07:25:06.962671 gymnasium_connect_four-1.1.3/gymnasium_connect_four.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-07-29 07:25:06.000000 gymnasium_connect_four-1.1.3/gymnasium_connect_four.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2023-07-29 07:25:06.000000 gymnasium_connect_four-1.1.3/gymnasium_connect_four.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 07:25:06.000000 gymnasium_connect_four-1.1.3/gymnasium_connect_four.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-29 07:25:06.000000 gymnasium_connect_four-1.1.3/gymnasium_connect_four.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-29 07:25:06.000000 gymnasium_connect_four-1.1.3/gymnasium_connect_four.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 07:25:06.971681 gymnasium_connect_four-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-07-29 07:24:51.000000 gymnasium_connect_four-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 07:25:06.967678 gymnasium_connect_four-1.1.3/test/
+-rw-rw-rw-   0        0        0     4688 2023-07-29 06:40:16.000000 gymnasium_connect_four-1.1.3/test/test_no_opponant.py
+-rw-rw-rw-   0        0        0    21167 2023-07-25 14:09:28.000000 gymnasium_connect_four-1.1.3/test/test_power_4_logic.py
+-rw-rw-rw-   0        0        0     2373 2023-07-23 20:26:41.000000 gymnasium_connect_four-1.1.3/test/test_ppo_env.py
```

### Comparing `gymnasium_connect_four-1.1.2/LICENSE` & `gymnasium_connect_four-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.2/README.md` & `gymnasium_connect_four-1.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -47,38 +47,38 @@
 000002e0: 6c6f 7069 6e67 2061 6e64 2069 6d70 726f  loping and impro
 000002f0: 7669 6e67 2079 6f75 7220 4149 2061 6c67  ving your AI alg
 00000300: 6f72 6974 686d 7320 7769 7468 6f75 7420  orithms without 
 00000310: 7370 656e 6469 6e67 2074 696d 6520 6f6e  spending time on
 00000320: 2063 7265 6174 696e 6720 616e 2065 6e76   creating an env
 00000330: 6972 6f6e 6d65 6e74 2066 726f 6d20 7363  ironment from sc
 00000340: 7261 7463 682e 0d0a 0d0a 2323 2046 6561  ratch.....## Fea
-00000350: 7475 7265 730d 0a0d 0a2d 202a 2a56 6172  tures....- **Var
-00000360: 6965 7479 206f 6620 426f 7473 2a2a 3a20  iety of Bots**: 
-00000370: 5468 6520 656e 7669 726f 6e6d 656e 7420  The environment 
-00000380: 696e 636c 7564 6573 2061 2063 6f6c 6c65  includes a colle
-00000390: 6374 696f 6e20 6f66 2043 6f6e 6e65 6374  ction of Connect
-000003a0: 2046 6f75 7220 626f 7473 2077 6974 6820   Four bots with 
-000003b0: 6469 6666 6572 656e 7420 736b 696c 6c20  different skill 
-000003c0: 6c65 7665 6c73 2074 6f20 6865 6c70 2077  levels to help w
-000003d0: 6974 6820 7468 6520 6c65 6172 6e69 6e67  ith the learning
-000003e0: 2070 726f 6365 7373 2061 6e64 2070 726f   process and pro
-000003f0: 7669 6465 2061 2064 6976 6572 7365 2072  vide a diverse r
-00000400: 616e 6765 206f 6620 6f70 706f 6e65 6e74  ange of opponent
-00000410: 732e 0d0a 2d20 2a2a 4f70 656e 4149 2047  s...- **OpenAI G
-00000420: 796d 202f 2047 796d 6e61 7369 756d 2043  ym / Gymnasium C
-00000430: 6f6d 7061 7469 626c 652a 2a3a 2043 6f6e  ompatible**: Con
-00000440: 6e65 6374 2046 6f75 7220 666f 6c6c 6f77  nect Four follow
-00000450: 7320 7468 6520 4f70 656e 4149 2047 796d  s the OpenAI Gym
-00000460: 202f 2047 796d 6e61 7369 756d 2069 6e74   / Gymnasium int
-00000470: 6572 6661 6365 2c20 6d61 6b69 6e67 2069  erface, making i
-00000480: 7420 636f 6d70 6174 6962 6c65 2077 6974  t compatible wit
-00000490: 6820 6120 7769 6465 2072 616e 6765 206f  h a wide range o
-000004a0: 6620 7265 696e 666f 7263 656d 656e 7420  f reinforcement 
-000004b0: 6c65 6172 6e69 6e67 206c 6962 7261 7269  learning librari
-000004c0: 6573 2061 6e64 2061 6c67 6f72 6974 686d  es and algorithm
+00000350: 7475 7265 730d 0a0d 0a2d 202a 2a4f 7065  tures....- **Ope
+00000360: 6e41 4920 4779 6d20 2f20 4779 6d6e 6173  nAI Gym / Gymnas
+00000370: 6975 6d20 436f 6d70 6174 6962 6c65 2a2a  ium Compatible**
+00000380: 3a20 436f 6e6e 6563 7420 466f 7572 2066  : Connect Four f
+00000390: 6f6c 6c6f 7773 2074 6865 204f 7065 6e41  ollows the OpenA
+000003a0: 4920 4779 6d20 2f20 4779 6d6e 6173 6975  I Gym / Gymnasiu
+000003b0: 6d20 696e 7465 7266 6163 652c 206d 616b  m interface, mak
+000003c0: 696e 6720 6974 2063 6f6d 7061 7469 626c  ing it compatibl
+000003d0: 6520 7769 7468 2061 2077 6964 6520 7261  e with a wide ra
+000003e0: 6e67 6520 6f66 2072 6569 6e66 6f72 6365  nge of reinforce
+000003f0: 6d65 6e74 206c 6561 726e 696e 6720 6c69  ment learning li
+00000400: 6272 6172 6965 7320 616e 6420 616c 676f  braries and algo
+00000410: 7269 7468 6d73 2e0d 0a2d 202a 2a56 6172  rithms...- **Var
+00000420: 6965 7479 206f 6620 426f 7473 2a2a 3a20  iety of Bots**: 
+00000430: 5468 6520 656e 7669 726f 6e6d 656e 7420  The environment 
+00000440: 696e 636c 7564 6573 2061 2063 6f6c 6c65  includes a colle
+00000450: 6374 696f 6e20 6f66 2043 6f6e 6e65 6374  ction of Connect
+00000460: 2046 6f75 7220 626f 7473 2077 6974 6820   Four bots with 
+00000470: 6469 6666 6572 656e 7420 736b 696c 6c20  different skill 
+00000480: 6c65 7665 6c73 2074 6f20 6865 6c70 2077  levels to help w
+00000490: 6974 6820 7468 6520 6c65 6172 6e69 6e67  ith the learning
+000004a0: 2070 726f 6365 7373 2061 6e64 2070 726f   process and pro
+000004b0: 7669 6465 2061 2064 6976 6572 7365 2072  vide a diverse r
+000004c0: 616e 6765 206f 6620 6f70 706f 6e65 6e74  ange of opponent
 000004d0: 732e 0d0a 2d20 2a2a 456c 6f20 4c65 6164  s...- **Elo Lead
 000004e0: 6572 626f 6172 6420 5379 7374 656d 2a2a  erboard System**
 000004f0: 3a20 4576 616c 7561 7465 2074 6865 2070  : Evaluate the p
 00000500: 6572 666f 726d 616e 6365 206f 6620 796f  erformance of yo
 00000510: 7572 2041 4920 6d6f 6465 6c20 6279 2061  ur AI model by a
 00000520: 7373 6967 6e69 6e67 2061 6e20 456c 6f20  ssigning an Elo 
 00000530: 7261 7469 6e67 2075 7369 6e67 2074 6865  rating using the
@@ -128,480 +128,615 @@
 000007f0: 4d6f 6465 2a2a 3a20 5472 6169 6e20 796f  Mode**: Train yo
 00000800: 7572 2061 6765 6e74 2061 6761 696e 7374  ur agent against
 00000810: 2061 6e6f 7468 6572 2041 4920 6f72 2065   another AI or e
 00000820: 7665 6e20 6120 6875 6d61 6e20 6f70 706f  ven a human oppo
 00000830: 6e65 6e74 2074 6f20 7465 7374 2069 7473  nent to test its
 00000840: 2070 6572 666f 726d 616e 6365 2069 6e20   performance in 
 00000850: 7265 616c 2d77 6f72 6c64 2073 6365 6e61  real-world scena
-00000860: 7269 6f73 2e0d 0a0d 0a23 2320 496e 7374  rios.....## Inst
-00000870: 616c 6c61 7469 6f6e 0d0a 0d0a 546f 2075  allation....To u
-00000880: 7365 2074 6865 204d 696e 6947 7269 6420  se the MiniGrid 
-00000890: 656e 7669 726f 6e6d 656e 742c 2079 6f75  environment, you
-000008a0: 2063 616e 2069 6e73 7461 6c6c 2069 7420   can install it 
-000008b0: 6469 7265 6374 6c79 2069 6e74 6f20 796f  directly into yo
-000008c0: 7572 2070 726f 6a65 6374 2075 7369 6e67  ur project using
-000008d0: 2070 6970 3a0d 0a0d 0a60 6060 6261 7368   pip:....```bash
-000008e0: 0d0a 7069 7020 696e 7374 616c 6c20 6779  ..pip install gy
-000008f0: 6d6e 6173 6975 6d2d 636f 6e6e 6563 742d  mnasium-connect-
-00000900: 666f 7572 0d0a 6060 600d 0a0d 0a23 2320  four..```....## 
-00000910: 5573 6167 650d 0a0d 0a49 6d70 6f72 7420  Usage....Import 
-00000920: 7468 6520 6043 6f6e 6e65 6374 466f 7572  the `ConnectFour
-00000930: 456e 7660 2063 6c61 7373 2c20 616e 6420  Env` class, and 
-00000940: 6869 7320 6f70 706f 6e61 6e74 2028 666f  his opponant (fo
-00000950: 7220 6578 656d 706c 6520 7468 6520 7665  r exemple the ve
-00000960: 7279 2065 6173 7920 706c 6179 6572 2060  ry easy player `
-00000970: 4261 6279 506c 6179 6572 6020 290d 0a0d  BabyPlayer` )...
-00000980: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
-00000990: 2063 6f6e 6e65 6374 5f66 6f75 725f 6779   connect_four_gy
-000009a0: 6d6e 6173 6975 6d20 696d 706f 7274 2043  mnasium import C
-000009b0: 6f6e 6e65 6374 466f 7572 456e 760d 0a66  onnectFourEnv..f
-000009c0: 726f 6d20 636f 6e6e 6563 745f 666f 7572  rom connect_four
-000009d0: 5f67 796d 6e61 7369 756d 2e70 6c61 7965  _gymnasium.playe
-000009e0: 7273 2069 6d70 6f72 7420 4261 6279 506c  rs import BabyPl
-000009f0: 6179 6572 0d0a 6060 600d 0a0d 0a48 6572  ayer..```....Her
-00000a00: 6520 6973 2061 2073 696d 706c 6520 6578  e is a simple ex
-00000a10: 616d 706c 6520 6f66 2068 6f77 2074 6f20  ample of how to 
-00000a20: 7573 6520 7468 6520 656e 7669 726f 6e6d  use the environm
-00000a30: 656e 7420 7769 7468 2050 504f 3a0d 0a0d  ent with PPO:...
-00000a40: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
-00000a50: 2063 6f6e 6e65 6374 5f66 6f75 725f 6779   connect_four_gy
-00000a60: 6d6e 6173 6975 6d20 696d 706f 7274 2043  mnasium import C
-00000a70: 6f6e 6e65 6374 466f 7572 456e 760d 0a66  onnectFourEnv..f
-00000a80: 726f 6d20 636f 6e6e 6563 745f 666f 7572  rom connect_four
-00000a90: 5f67 796d 6e61 7369 756d 2e70 6c61 7965  _gymnasium.playe
-00000aa0: 7273 2069 6d70 6f72 7420 4261 6279 506c  rs import BabyPl
-00000ab0: 6179 6572 0d0a 6672 6f6d 2073 7461 626c  ayer..from stabl
-00000ac0: 655f 6261 7365 6c69 6e65 7333 2069 6d70  e_baselines3 imp
-00000ad0: 6f72 7420 5050 4f0d 0a20 2020 2020 2020  ort PPO..       
-00000ae0: 200d 0a65 6e76 203d 2043 6f6e 6e65 6374   ..env = Connect
-00000af0: 466f 7572 456e 7628 6f70 706f 6e65 6e74  FourEnv(opponent
-00000b00: 3d42 6162 7950 6c61 7965 7228 2929 0d0a  =BabyPlayer())..
-00000b10: 6d6f 6465 6c20 3d20 5050 4f28 224d 6c70  model = PPO("Mlp
-00000b20: 506f 6c69 6379 222c 2065 6e76 2c20 7665  Policy", env, ve
-00000b30: 7262 6f73 653d 3129 0d0a 0d0a 6d6f 6465  rbose=1)....mode
-00000b40: 6c2e 6c65 6172 6e28 746f 7461 6c5f 7469  l.learn(total_ti
-00000b50: 6d65 7374 6570 733d 2831 3030 3030 3029  mesteps=(100000)
-00000b60: 290d 0a60 6060 0d0a 0d0a 466f 7220 6465  )..```....For de
-00000b70: 7461 696c 6564 2075 7361 6765 2069 6e73  tailed usage ins
-00000b80: 7472 7563 7469 6f6e 7320 616e 6420 6578  tructions and ex
-00000b90: 616d 706c 6573 2c20 706c 6561 7365 2072  amples, please r
-00000ba0: 6566 6572 2074 6f20 7468 6520 5b65 7861  efer to the [exa
-00000bb0: 6d70 6c65 735d 2868 7474 7073 3a2f 2f67  mples](https://g
-00000bc0: 6974 6875 622e 636f 6d2f 6c75 6361 7342  ithub.com/lucasB
-00000bd0: 6572 746f 6c61 2f43 6f6e 6e65 6374 2d34  ertola/Connect-4
-00000be0: 2d47 796d 2d65 6e76 2d52 6569 6e66 6f72  -Gym-env-Reinfor
-00000bf0: 6365 6d65 6e74 2d6c 6561 726e 696e 672f  cement-learning/
-00000c00: 7472 6565 2f6d 6169 6e2f 6578 656d 706c  tree/main/exempl
-00000c10: 6573 2920 6469 7265 6374 6f72 7920 6f72  es) directory or
-00000c20: 2063 6865 636b 206f 7574 206f 7572 205b   check out our [
-00000c30: 436f 6c61 6220 4e6f 7465 626f 6f6b 5d28  Colab Notebook](
-00000c40: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-00000c50: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-00000c60: 6d2f 6769 7468 7562 2f6c 7563 6173 4265  m/github/lucasBe
-00000c70: 7274 6f6c 612f 436f 6e6e 6563 742d 342d  rtola/Connect-4-
-00000c80: 4779 6d2d 656e 762d 5265 696e 666f 7263  Gym-env-Reinforc
-00000c90: 656d 656e 742d 6c65 6172 6e69 6e67 2f62  ement-learning/b
-00000ca0: 6c6f 622f 6d61 696e 2f65 7865 6d70 6c65  lob/main/exemple
-00000cb0: 732f 5050 4f5f 4d6c 7050 6f6c 6963 792e  s/PPO_MlpPolicy.
-00000cc0: 6970 796e 6229 2e0d 0a0d 0a5b 215b 4f70  ipynb).....[![Op
-00000cd0: 656e 2049 6e20 436f 6c61 625d 2868 7474  en In Colab](htt
-00000ce0: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
-00000cf0: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f61  rch.google.com/a
-00000d00: 7373 6574 732f 636f 6c61 622d 6261 6467  ssets/colab-badg
-00000d10: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
-00000d20: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
-00000d30: 6f6f 676c 652e 636f 6d2f 6769 7468 7562  oogle.com/github
-00000d40: 2f6c 7563 6173 4265 7274 6f6c 612f 436f  /lucasBertola/Co
-00000d50: 6e6e 6563 742d 342d 4779 6d2d 656e 762d  nnect-4-Gym-env-
-00000d60: 5265 696e 666f 7263 656d 656e 742d 6c65  Reinforcement-le
-00000d70: 6172 6e69 6e67 2f62 6c6f 622f 6d61 696e  arning/blob/main
-00000d80: 2f65 7865 6d70 6c65 732f 5050 4f5f 4d6c  /exemples/PPO_Ml
-00000d90: 7050 6f6c 6963 792e 6970 796e 6229 0d0a  pPolicy.ipynb)..
-00000da0: 0d0a 2323 2045 6e76 6972 6f6e 6d65 6e74  ..## Environment
-00000db0: 2044 6574 6169 6c73 0d0a 0d0a 496e 2074   Details....In t
-00000dc0: 6869 7320 7365 6374 696f 6e2c 2077 6520  his section, we 
-00000dd0: 7072 6f76 6964 6520 616e 206f 7665 7276  provide an overv
-00000de0: 6965 7720 6f66 2074 6865 2043 6f6e 6e65  iew of the Conne
-00000df0: 6374 2046 6f75 7220 656e 7669 726f 6e6d  ct Four environm
-00000e00: 656e 742c 2069 6e63 6c75 6469 6e67 2074  ent, including t
-00000e10: 6865 2061 6374 696f 6e20 7370 6163 652c  he action space,
-00000e20: 206f 6273 6572 7661 7469 6f6e 2073 7061   observation spa
-00000e30: 6365 2c20 7265 7761 7264 732c 2061 6e64  ce, rewards, and
-00000e40: 2065 7069 736f 6465 2074 6572 6d69 6e61   episode termina
-00000e50: 7469 6f6e 2063 6f6e 6469 7469 6f6e 732e  tion conditions.
-00000e60: 0d0a 0d0a 2323 2320 4163 7469 6f6e 2053  ....### Action S
-00000e70: 7061 6365 0d0a 0d0a 5468 6520 6163 7469  pace....The acti
-00000e80: 6f6e 2073 7061 6365 2069 6e20 7468 6520  on space in the 
-00000e90: 436f 6e6e 6563 7420 466f 7572 2065 6e76  Connect Four env
-00000ea0: 6972 6f6e 6d65 6e74 2069 7320 6469 7363  ironment is disc
-00000eb0: 7265 7465 2c20 7769 7468 2061 2074 6f74  rete, with a tot
-00000ec0: 616c 206f 6620 3720 706f 7373 6962 6c65  al of 7 possible
-00000ed0: 2061 6374 696f 6e73 2e20 4561 6368 2061   actions. Each a
-00000ee0: 6374 696f 6e20 636f 7272 6573 706f 6e64  ction correspond
-00000ef0: 7320 746f 2061 2063 6f6c 756d 6e20 696e  s to a column in
-00000f00: 2074 6865 2067 616d 6520 626f 6172 6420   the game board 
-00000f10: 7768 6572 6520 6120 706c 6179 6572 2063  where a player c
-00000f20: 616e 2064 726f 7020 7468 6569 7220 7069  an drop their pi
-00000f30: 6563 652e 2054 6865 2061 6374 696f 6e20  ece. The action 
-00000f40: 7370 6163 6520 6973 2072 6570 7265 7365  space is represe
-00000f50: 6e74 6564 2061 7320 666f 6c6c 6f77 733a  nted as follows:
-00000f60: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a73  ....```python..s
-00000f70: 656c 662e 6163 7469 6f6e 5f73 7061 6365  elf.action_space
-00000f80: 203d 2073 7061 6365 732e 4469 7363 7265   = spaces.Discre
-00000f90: 7465 2873 656c 662e 434f 4c55 4d4e 535f  te(self.COLUMNS_
-00000fa0: 434f 554e 5429 0d0a 6060 600d 0a0d 0a23  COUNT)..```....#
-00000fb0: 2323 204f 6273 6572 7661 7469 6f6e 2053  ## Observation S
-00000fc0: 7061 6365 0d0a 0d0a 5468 6520 6f62 7365  pace....The obse
-00000fd0: 7276 6174 696f 6e20 7370 6163 6520 696e  rvation space in
-00000fe0: 2074 6865 2043 6f6e 6e65 6374 2046 6f75   the Connect Fou
-00000ff0: 7220 656e 7669 726f 6e6d 656e 7420 6973  r environment is
-00001000: 2061 2032 4420 6172 7261 7920 7265 7072   a 2D array repr
-00001010: 6573 656e 7469 6e67 2074 6865 2067 616d  esenting the gam
-00001020: 6520 626f 6172 642e 2045 6163 6820 6365  e board. Each ce
-00001030: 6c6c 2069 6e20 7468 6520 6172 7261 7920  ll in the array 
-00001040: 6361 6e20 6861 7665 206f 6e65 206f 6620  can have one of 
-00001050: 7468 7265 6520 706f 7373 6962 6c65 2076  three possible v
-00001060: 616c 7565 733a 2030 2028 656d 7074 7929  alues: 0 (empty)
-00001070: 2c20 3120 2870 6c61 7965 7227 7320 7069  , 1 (player's pi
-00001080: 6563 6529 2c20 6f72 2032 2028 6f70 706f  ece), or 2 (oppo
-00001090: 6e65 6e74 2773 2070 6965 6365 292e 2054  nent's piece). T
-000010a0: 6865 206f 6273 6572 7661 7469 6f6e 2073  he observation s
-000010b0: 7061 6365 2069 7320 6465 6669 6e65 6420  pace is defined 
-000010c0: 6173 2066 6f6c 6c6f 7773 3a0d 0a0d 0a60  as follows:....`
-000010d0: 6060 7079 7468 6f6e 0d0a 7365 6c66 2e6f  ``python..self.o
-000010e0: 6273 6572 7661 7469 6f6e 5f73 7061 6365  bservation_space
-000010f0: 203d 2073 7061 6365 732e 426f 7828 6c6f   = spaces.Box(lo
-00001100: 773d 302c 2068 6967 683d 322c 2073 6861  w=0, high=2, sha
-00001110: 7065 3d28 7365 6c66 2e52 4f57 535f 434f  pe=(self.ROWS_CO
-00001120: 554e 542c 2073 656c 662e 434f 4c55 4d4e  UNT, self.COLUMN
-00001130: 535f 434f 554e 5429 2c20 6474 7970 653d  S_COUNT), dtype=
-00001140: 6e70 2e69 6e74 3332 290d 0a60 6060 0d0a  np.int32)..```..
-00001150: 0d0a 2323 2320 5265 7761 7264 730d 0a0d  ..### Rewards...
-00001160: 0a54 6865 2072 6577 6172 6420 7379 7374  .The reward syst
-00001170: 656d 2069 6e20 7468 6520 436f 6e6e 6563  em in the Connec
-00001180: 7420 466f 7572 2065 6e76 6972 6f6e 6d65  t Four environme
-00001190: 6e74 2069 7320 6465 7369 676e 6564 2074  nt is designed t
-000011a0: 6f20 656e 636f 7572 6167 6520 7468 6520  o encourage the 
-000011b0: 4149 206d 6f64 656c 2074 6f20 6c65 6172  AI model to lear
-000011c0: 6e20 686f 7720 746f 2077 696e 2074 6865  n how to win the
-000011d0: 2067 616d 652e 2054 6865 2072 6577 6172   game. The rewar
-000011e0: 6473 2061 7265 2061 7320 666f 6c6c 6f77  ds are as follow
-000011f0: 733a 0d0a 0d0a 2d20 4120 7265 7761 7264  s:....- A reward
-00001200: 206f 6620 2b31 2069 7320 6769 7665 6e20   of +1 is given 
-00001210: 7768 656e 2074 6865 2041 4920 6d6f 6465  when the AI mode
-00001220: 6c20 7769 6e73 2074 6865 2067 616d 6520  l wins the game 
-00001230: 6279 2063 6f6e 6e65 6374 696e 6720 666f  by connecting fo
-00001240: 7572 206f 6620 6974 7320 7069 6563 6573  ur of its pieces
-00001250: 2069 6e20 6120 726f 772c 2065 6974 6865   in a row, eithe
-00001260: 7220 686f 7269 7a6f 6e74 616c 6c79 2c20  r horizontally, 
-00001270: 7665 7274 6963 616c 6c79 2c20 6f72 2064  vertically, or d
-00001280: 6961 676f 6e61 6c6c 792e 0d0a 2d20 4120  iagonally...- A 
-00001290: 7265 7761 7264 206f 6620 2d31 2069 7320  reward of -1 is 
-000012a0: 6769 7665 6e20 7768 656e 2074 6865 2041  given when the A
-000012b0: 4920 6d6f 6465 6c20 6c6f 7365 7320 7468  I model loses th
-000012c0: 6520 6761 6d65 206f 7220 706c 6179 7320  e game or plays 
-000012d0: 616e 2069 6e76 616c 6964 2061 6374 696f  an invalid actio
-000012e0: 6e2e 0d0a 2d20 4120 7265 7761 7264 206f  n...- A reward o
-000012f0: 6620 3020 6973 2067 6976 656e 2066 6f72  f 0 is given for
-00001300: 2061 6c6c 206f 7468 6572 2061 6374 696f   all other actio
-00001310: 6e73 2074 6861 7420 646f 206e 6f74 2072  ns that do not r
-00001320: 6573 756c 7420 696e 2061 2077 696e 206f  esult in a win o
-00001330: 7220 6c6f 7373 2e0d 0a0d 0a23 2323 2045  r loss.....### E
-00001340: 7069 736f 6465 2054 6572 6d69 6e61 7469  pisode Terminati
-00001350: 6f6e 0d0a 0d0a 416e 2065 7069 736f 6465  on....An episode
-00001360: 2069 6e20 7468 6520 436f 6e6e 6563 7420   in the Connect 
-00001370: 466f 7572 2065 6e76 6972 6f6e 6d65 6e74  Four environment
-00001380: 2074 6572 6d69 6e61 7465 7320 756e 6465   terminates unde
-00001390: 7220 7468 6520 666f 6c6c 6f77 696e 6720  r the following 
-000013a0: 636f 6e64 6974 696f 6e73 3a0d 0a0d 0a2d  conditions:....-
-000013b0: 2054 6865 2041 4920 6d6f 6465 6c20 7769   The AI model wi
-000013c0: 6e73 2074 6865 2067 616d 6520 6279 2063  ns the game by c
-000013d0: 6f6e 6e65 6374 696e 6720 666f 7572 206f  onnecting four o
-000013e0: 6620 6974 7320 7069 6563 6573 2069 6e20  f its pieces in 
-000013f0: 6120 726f 772c 2065 6974 6865 7220 686f  a row, either ho
-00001400: 7269 7a6f 6e74 616c 6c79 2c20 7665 7274  rizontally, vert
-00001410: 6963 616c 6c79 2c20 6f72 2064 6961 676f  ically, or diago
-00001420: 6e61 6c6c 792e 0d0a 2d20 5468 6520 4149  nally...- The AI
-00001430: 206d 6f64 656c 206c 6f73 6573 2074 6865   model loses the
-00001440: 2067 616d 6520 6279 2061 6c6c 6f77 696e   game by allowin
-00001450: 6720 7468 6520 6f70 706f 6e65 6e74 2074  g the opponent t
-00001460: 6f20 636f 6e6e 6563 7420 666f 7572 206f  o connect four o
-00001470: 6620 7468 6569 7220 7069 6563 6573 2069  f their pieces i
-00001480: 6e20 6120 726f 772c 206f 7220 6279 2070  n a row, or by p
-00001490: 6c61 7969 6e67 2061 6e20 696e 7661 6c69  laying an invali
-000014a0: 6420 6163 7469 6f6e 2e0d 0a2d 2054 6865  d action...- The
-000014b0: 2067 616d 6520 626f 6172 6420 6973 2063   game board is c
-000014c0: 6f6d 706c 6574 656c 7920 6669 6c6c 6564  ompletely filled
-000014d0: 2c20 7265 7375 6c74 696e 6720 696e 2061  , resulting in a
-000014e0: 2064 7261 772e 0d0a 0d0a 5768 656e 2061   draw.....When a
-000014f0: 6e20 6570 6973 6f64 6520 7465 726d 696e  n episode termin
-00001500: 6174 6573 2c20 7468 6520 656e 7669 726f  ates, the enviro
-00001510: 6e6d 656e 7420 6973 2072 6573 6574 2c20  nment is reset, 
-00001520: 616e 6420 6120 6e65 7720 6570 6973 6f64  and a new episod
-00001530: 6520 6265 6769 6e73 2e0d 0a0d 0a23 2320  e begins.....## 
-00001540: 4176 6169 6c61 626c 6520 506c 6179 6572  Available Player
-00001550: 730d 0a0d 0a54 6869 7320 6c69 6272 6172  s....This librar
-00001560: 7920 7072 6f76 6964 6573 2061 2063 6f6c  y provides a col
-00001570: 6c65 6374 696f 6e20 6f66 2043 6f6e 6e65  lection of Conne
-00001580: 6374 2046 6f75 7220 626f 7473 2077 6974  ct Four bots wit
-00001590: 6820 6469 6666 6572 656e 7420 736b 696c  h different skil
-000015a0: 6c20 6c65 7665 6c73 2e20 5468 6573 6520  l levels. These 
-000015b0: 626f 7473 2063 616e 2062 6520 7573 6564  bots can be used
-000015c0: 2066 6f72 2076 6172 696f 7573 2070 7572   for various pur
-000015d0: 706f 7365 732c 2073 7563 6820 6173 3a0d  poses, such as:.
-000015e0: 0a0d 0a2d 202a 2a4c 6561 726e 696e 6720  ...- **Learning 
-000015f0: 6279 2070 6c61 7969 6e67 2061 6761 696e  by playing again
-00001600: 7374 2074 6865 6d2a 2a3a 2059 6f75 2063  st them**: You c
-00001610: 616e 2069 6d70 726f 7665 2079 6f75 7220  an improve your 
-00001620: 4149 206d 6f64 656c 2062 7920 706c 6179  AI model by play
-00001630: 696e 6720 6167 6169 6e73 7420 7468 6573  ing against thes
-00001640: 6520 626f 7473 2c20 7768 6963 6820 7261  e bots, which ra
-00001650: 6e67 6520 6672 6f6d 2062 6567 696e 6e65  nge from beginne
-00001660: 7220 746f 2061 6476 616e 6365 6420 6c65  r to advanced le
-00001670: 7665 6c73 2e0d 0a2d 202a 2a43 6f6d 7061  vels...- **Compa
-00001680: 7269 6e67 2074 6865 206c 6576 656c 206f  ring the level o
-00001690: 6620 7365 6c66 2d6c 6561 726e 696e 6720  f self-learning 
-000016a0: 6d6f 6465 6c73 2a2a 3a20 4279 2070 6c61  models**: By pla
-000016b0: 7969 6e67 2061 6761 696e 7374 2074 6865  ying against the
-000016c0: 7365 2062 6f74 732c 2079 6f75 2063 616e  se bots, you can
-000016d0: 2065 7661 6c75 6174 6520 7468 6520 7065   evaluate the pe
-000016e0: 7266 6f72 6d61 6e63 6520 6f66 2079 6f75  rformance of you
-000016f0: 7220 7365 6c66 2d6c 6561 726e 696e 6720  r self-learning 
-00001700: 6d6f 6465 6c20 616e 6420 706f 7369 7469  model and positi
-00001710: 6f6e 2069 7420 696e 2074 6572 6d73 206f  on it in terms o
-00001720: 6620 736b 696c 6c20 6c65 7665 6c20 616e  f skill level an
-00001730: 6420 656c 6f2e 0d0a 0d0a 596f 7520 6361  d elo.....You ca
-00001740: 6e20 696e 7465 6772 6174 6520 706c 6179  n integrate play
-00001750: 6572 7320 6173 206f 7070 6f6e 656e 7473  ers as opponents
-00001760: 2069 6e20 796f 7572 2067 796d 2065 6e76   in your gym env
-00001770: 6972 6f6e 6d65 6e74 206c 696b 6520 7468  ironment like th
-00001780: 6973 3a0d 0a0d 0a60 6060 7079 7468 6f6e  is:....```python
-00001790: 0d0a 656e 7620 3d20 436f 6e6e 6563 7446  ..env = ConnectF
-000017a0: 6f75 7245 6e76 286f 7070 6f6e 656e 743d  ourEnv(opponent=
-000017b0: 4261 6279 506c 6179 6572 2829 290d 0a60  BabyPlayer())..`
-000017c0: 6060 0d0a 0d0a 2323 2320 506c 6179 6572  ``....### Player
-000017d0: 2044 6573 6372 6970 7469 6f6e 730d 0a0d   Descriptions...
-000017e0: 0a2d 202a 2a4d 696e 4d61 7850 6c61 7965  .- **MinMaxPlaye
-000017f0: 722a 2a3a 2041 6e20 696d 706c 656d 656e  r**: An implemen
-00001800: 7461 7469 6f6e 206f 6620 7468 6520 4d69  tation of the Mi
-00001810: 6e69 6d61 7820 616c 676f 7269 7468 6d2e  nimax algorithm.
-00001820: 2043 616e 2062 6520 7573 6564 2077 6974   Can be used wit
-00001830: 6820 6469 6666 6572 656e 7420 7365 6172  h different sear
-00001840: 6368 2064 6570 7468 7320 2865 2e67 2e2c  ch depths (e.g.,
-00001850: 2060 4d69 6e4d 6178 506c 6179 6572 2864   `MinMaxPlayer(d
-00001860: 6570 7468 3d33 2960 292c 2062 7574 2069  epth=3)`), but i
-00001870: 7420 6973 2076 6572 7920 736c 6f77 2c20  t is very slow, 
-00001880: 736f 2069 7420 6973 206e 6f74 2072 6563  so it is not rec
-00001890: 6f6d 6d65 6e64 6564 2066 6f72 2067 656e  ommended for gen
-000018a0: 6572 616c 2075 7365 2e20 416c 6c20 6f74  eral use. All ot
-000018b0: 6865 7220 616c 676f 7269 7468 6d73 2061  her algorithms a
-000018c0: 7265 206d 7563 6820 6661 7374 6572 2e0d  re much faster..
-000018d0: 0a0d 0a2d 202a 2a42 6162 7950 6c61 7965  ...- **BabyPlaye
-000018e0: 722a 2a3a 2050 6c61 7973 2072 616e 646f  r**: Plays rando
-000018f0: 6d20 6d6f 7665 732e 0d0a 0d0a 2d20 2a2a  m moves.....- **
-00001900: 4368 696c 6450 6c61 7965 722a 2a3a 2050  ChildPlayer**: P
-00001910: 6c61 7973 2072 616e 646f 6d20 6d6f 7665  lays random move
-00001920: 732c 2062 7574 2069 6620 7468 6572 6520  s, but if there 
-00001930: 6973 2061 2077 696e 6e69 6e67 206d 6f76  is a winning mov
-00001940: 652c 2069 7420 7769 6c6c 2070 6c61 7920  e, it will play 
-00001950: 6974 2e0d 0a0d 0a2d 202a 2a43 6869 6c64  it.....- **Child
-00001960: 536d 6172 7465 7250 6c61 7965 722a 2a3a  SmarterPlayer**:
-00001970: 2053 616d 6520 6173 2043 6869 6c64 506c   Same as ChildPl
-00001980: 6179 6572 2c20 6275 7420 6966 2074 6865  ayer, but if the
-00001990: 7265 2069 7320 6120 6d6f 7665 2074 6861  re is a move tha
-000019a0: 7420 776f 756c 6420 6d61 6b65 2074 6865  t would make the
-000019b0: 206f 7070 6f6e 656e 7420 7769 6e2c 2069   opponent win, i
-000019c0: 7420 7769 6c6c 2070 6c61 7920 7468 6174  t will play that
-000019d0: 206d 6f76 6520 746f 2062 6c6f 636b 2074   move to block t
-000019e0: 6865 206f 7070 6f6e 656e 742e 0d0a 0d0a  he opponent.....
-000019f0: 2d20 2a2a 5465 656e 6167 6572 506c 6179  - **TeenagerPlay
-00001a00: 6572 2a2a 3a20 5361 6d65 2061 7320 4368  er**: Same as Ch
-00001a10: 696c 6453 6d61 7274 6572 506c 6179 6572  ildSmarterPlayer
-00001a20: 2c20 6275 7420 6578 636c 7564 6573 206d  , but excludes m
-00001a30: 6f76 6573 2074 6861 7420 776f 756c 6420  oves that would 
-00001a40: 616c 6c6f 7720 7468 6520 6f70 706f 6e65  allow the oppone
-00001a50: 6e74 2074 6f20 7769 6e20 6966 2074 6865  nt to win if the
-00001a60: 7920 706c 6179 206f 6e20 746f 7020 6f66  y play on top of
-00001a70: 2069 742e 0d0a 0d0a 2d20 2a2a 5465 656e   it.....- **Teen
-00001a80: 6167 6572 536d 6172 7465 7250 6c61 7965  agerSmarterPlaye
-00001a90: 722a 2a3a 2053 616d 6520 6173 2054 6565  r**: Same as Tee
-00001aa0: 6e61 6765 7250 6c61 7965 722c 2062 7574  nagerPlayer, but
-00001ab0: 2063 6865 636b 7320 6966 2061 206d 6f76   checks if a mov
-00001ac0: 6520 6372 6561 7465 7320 6120 6c69 6e65  e creates a line
-00001ad0: 206f 6620 7468 7265 6520 746f 6b65 6e73   of three tokens
-00001ae0: 2077 6974 6820 6176 6169 6c61 626c 6520   with available 
-00001af0: 7370 6163 6573 206f 6e20 626f 7468 2073  spaces on both s
-00001b00: 6964 6573 2e20 4966 2073 6f2c 2069 7420  ides. If so, it 
-00001b10: 7769 6c6c 2070 6c61 7920 7468 6174 206d  will play that m
-00001b20: 6f76 652e 0d0a 0d0a 2d20 2a2a 4164 756c  ove.....- **Adul
-00001b30: 7450 6c61 7965 722a 2a3a 2053 616d 6520  tPlayer**: Same 
-00001b40: 6173 2054 6565 6e61 6765 7253 6d61 7274  as TeenagerSmart
-00001b50: 6572 506c 6179 6572 2c20 6275 7420 616c  erPlayer, but al
-00001b60: 736f 2063 6865 636b 7320 6966 2061 206d  so checks if a m
-00001b70: 6f76 6520 6372 6561 7465 7320 6120 6c69  ove creates a li
-00001b80: 6e65 206f 6620 7468 7265 6520 746f 6b65  ne of three toke
-00001b90: 6e73 2077 6974 6820 6176 6169 6c61 626c  ns with availabl
-00001ba0: 6520 7370 6163 6573 206f 6e20 626f 7468  e spaces on both
-00001bb0: 2073 6964 6573 2066 6f72 2074 6865 206f   sides for the o
-00001bc0: 7070 6f6e 656e 742e 2049 6620 736f 2c20  pponent. If so, 
-00001bd0: 6974 2077 696c 6c20 706c 6179 2074 6861  it will play tha
-00001be0: 7420 6d6f 7665 2074 6f20 626c 6f63 6b20  t move to block 
-00001bf0: 7468 6520 6f70 706f 6e65 6e74 2e0d 0a0d  the opponent....
-00001c00: 0a2d 202a 2a41 6475 6c74 536d 6172 7465  .- **AdultSmarte
-00001c10: 7250 6c61 7965 722a 2a3a 2053 616d 6520  rPlayer**: Same 
-00001c20: 6173 2041 6475 6c74 506c 6179 6572 2c20  as AdultPlayer, 
-00001c30: 6275 7420 6368 6563 6b73 2069 6620 6120  but checks if a 
-00001c40: 6d6f 7665 2061 6c6c 6f77 7320 746f 2063  move allows to c
-00001c50: 7265 6174 6520 6d75 6c74 6970 6c65 2077  reate multiple w
-00001c60: 6179 7320 746f 2077 696e 2061 6e64 2070  ays to win and p
-00001c70: 6c61 7973 2074 6861 7420 6d6f 7665 2e20  lays that move. 
-00001c80: 416c 736f 2063 6865 636b 7320 6966 2061  Also checks if a
-00001c90: 206d 6f76 6520 616c 6c6f 7773 2074 6865   move allows the
-00001ca0: 206f 7070 6f6e 656e 7420 746f 2063 7265   opponent to cre
-00001cb0: 6174 6520 6d75 6c74 6970 6c65 2077 6179  ate multiple way
-00001cc0: 7320 746f 2077 696e 2061 6e64 2070 6c61  s to win and pla
-00001cd0: 7973 2074 6861 7420 6d6f 7665 2074 6f20  ys that move to 
-00001ce0: 7072 6f74 6563 7420 6974 7365 6c66 2e0d  protect itself..
-00001cf0: 0a0d 0a2d 202a 2a43 6f6e 736f 6c65 506c  ...- **ConsolePl
-00001d00: 6179 6572 2a2a 3a20 4173 6b73 2066 6f72  ayer**: Asks for
-00001d10: 206d 6f76 6573 2074 6f20 706c 6179 2069   moves to play i
-00001d20: 6e20 7468 6520 636f 6e73 6f6c 652e 2050  n the console. P
-00001d30: 6572 6665 6374 2066 6f72 2074 6573 7469  erfect for testi
-00001d40: 6e67 2079 6f75 7220 6f77 6e20 4149 2e0d  ng your own AI..
-00001d50: 0a0d 0a23 2323 2045 6c6f 2052 6174 696e  ...### Elo Ratin
-00001d60: 6773 0d0a 0d0a 4865 7265 2061 7265 2074  gs....Here are t
-00001d70: 6865 2045 6c6f 2072 6174 696e 6773 206f  he Elo ratings o
-00001d80: 6620 7468 6520 6469 6666 6572 656e 7420  f the different 
-00001d90: 616c 676f 7269 7468 6d73 3a0d 0a0d 0a60  algorithms:....`
-00001da0: 6060 0d0a 312e 2041 6475 6c74 536d 6172  ``..1. AdultSmar
-00001db0: 7465 7250 6c61 7965 723a 2020 2020 3137  terPlayer:    17
-00001dc0: 3637 0d0a 322e 2041 6475 6c74 506c 6179  67..2. AdultPlay
-00001dd0: 6572 3a20 2020 2020 2020 2020 2020 3137  er:           17
-00001de0: 3132 0d0a 332e 204d 696e 696d 6178 506c  12..3. MinimaxPl
-00001df0: 6179 6572 2064 6570 7468 2033 3a20 3136  ayer depth 3: 16
-00001e00: 3732 0d0a 342e 204d 696e 696d 6178 506c  72..4. MinimaxPl
-00001e10: 6179 6572 2064 6570 7468 2032 3a20 3136  ayer depth 2: 16
-00001e20: 3232 0d0a 352e 2054 6565 6e61 6765 7253  22..5. TeenagerS
-00001e30: 6d61 7274 6572 506c 6179 6572 3a20 3136  marterPlayer: 16
-00001e40: 3131 0d0a 362e 2054 6565 6e61 6765 7250  11..6. TeenagerP
-00001e50: 6c61 7965 723a 2020 2020 2020 2020 3136  layer:        16
-00001e60: 3034 0d0a 372e 2043 6869 6c64 536d 6172  04..7. ChildSmar
-00001e70: 7465 7250 6c61 7965 723a 2020 2020 3135  terPlayer:    15
-00001e80: 3235 0d0a 382e 204d 696e 696d 6178 506c  25..8. MinimaxPl
-00001e90: 6179 6572 2064 6570 7468 2031 3a20 3132  ayer depth 1: 12
-00001ea0: 3230 0d0a 392e 2043 6869 6c64 506c 6179  20..9. ChildPlay
-00001eb0: 6572 3a20 2020 2020 2020 2020 2020 3132  er:           12
-00001ec0: 3038 0d0a 3130 2e20 4261 6279 506c 6179  08..10. BabyPlay
-00001ed0: 6572 3a20 2020 2020 2020 2020 2020 2039  er:            9
-00001ee0: 3935 0d0a 6060 600d 0a0d 0a49 6e20 6164  95..```....In ad
-00001ef0: 6469 7469 6f6e 2074 6f20 7468 6520 7072  dition to the pr
-00001f00: 6f76 6964 6564 2070 6c61 7965 7273 2c20  ovided players, 
-00001f10: 7765 2061 6c73 6f20 6f66 6665 7220 6120  we also offer a 
-00001f20: 746f 6f6c 2074 6f20 6576 616c 7561 7465  tool to evaluate
-00001f30: 2074 6865 2045 6c6f 2072 6174 696e 6720   the Elo rating 
-00001f40: 6f66 2079 6f75 7220 6f77 6e20 4149 206d  of your own AI m
-00001f50: 6f64 656c 2e20 5468 6973 2069 7320 6578  odel. This is ex
-00001f60: 7472 656d 656c 7920 7573 6566 756c 2074  tremely useful t
-00001f70: 6f20 6861 7665 2061 6e20 2261 6273 6f6c  o have an "absol
-00001f80: 7574 6522 2069 6465 6120 6f66 2074 6865  ute" idea of the
-00001f90: 2070 726f 6772 6573 7320 6f66 2079 6f75   progress of you
-00001fa0: 7220 4149 2e20 466f 7220 6578 616d 706c  r AI. For exampl
-00001fb0: 652c 2069 6620 616e 2041 4920 6c65 6172  e, if an AI lear
-00001fc0: 6e73 2062 7920 6669 6768 7469 6e67 2061  ns by fighting a
-00001fd0: 6761 696e 7374 2069 7473 656c 662c 2077  gainst itself, w
-00001fe0: 6520 6b6e 6f77 2074 6861 7420 6974 2069  e know that it i
-00001ff0: 7320 6765 7474 696e 6720 7374 726f 6e67  s getting strong
-00002000: 6572 2061 7320 6974 2077 6f75 6c64 2062  er as it would b
-00002010: 6520 6162 6c65 2074 6f20 7769 6e20 6167  e able to win ag
-00002020: 6169 6e73 7420 6974 7320 6f6c 6465 7220  ainst its older 
-00002030: 7665 7273 696f 6e73 2c20 6275 7420 7468  versions, but th
-00002040: 6973 2069 7320 6e6f 7420 656e 6f75 6768  is is not enough
-00002050: 2074 6f20 6576 616c 7561 7465 2069 6620   to evaluate if 
-00002060: 6974 2068 6173 206c 6561 726e 6564 2061  it has learned a
-00002070: 206c 6f74 2e20 5468 6973 2069 7320 7768   lot. This is wh
-00002080: 6572 6520 6f75 7220 746f 6f6c 2063 6f6d  ere our tool com
-00002090: 6573 2069 6e2c 2077 6869 6368 2061 6c6c  es in, which all
-000020a0: 6f77 7320 796f 7520 746f 2067 6976 6520  ows you to give 
-000020b0: 616e 2045 6c6f 2072 6174 696e 6720 746f  an Elo rating to
-000020c0: 2074 6865 2041 492e 0d0a 0d0a 4865 7265   the AI.....Here
-000020d0: 2069 7320 686f 7720 746f 2075 7365 2069   is how to use i
-000020e0: 7420 696e 2050 7974 686f 6e3a 0d0a 0d0a  t in Python:....
-000020f0: 6060 6070 7974 686f 6e0d 0a65 6e76 203d  ```python..env =
-00002100: 2043 6f6e 6e65 6374 466f 7572 456e 7628   ConnectFourEnv(
-00002110: 6f70 706f 6e65 6e74 3d42 6162 7950 6c61  opponent=BabyPla
-00002120: 7965 7228 2929 0d0a 6d6f 6465 6c20 3d20  yer())..model = 
-00002130: 5050 4f28 224d 6c70 506f 6c69 6379 222c  PPO("MlpPolicy",
-00002140: 2065 6e76 290d 0a6d 6f64 656c 2e6c 6561   env)..model.lea
-00002150: 726e 2874 6f74 616c 5f74 696d 6573 7465  rn(total_timeste
-00002160: 7073 3d31 3030 3030 290d 0a0d 0a6d 794d  ps=10000)....myM
-00002170: 6f64 656c 506c 6179 6572 203d 204d 6f64  odelPlayer = Mod
-00002180: 656c 506c 6179 6572 286d 6f64 656c 2c6e  elPlayer(model,n
-00002190: 616d 653d 2259 6f75 7220 7472 6169 6e65  ame="Your traine
-000021a0: 6420 4d6f 6465 6c22 290d 0a0d 0a79 6f75  d Model")....you
-000021b0: 725f 6d6f 6465 6c5f 656c 6f20 3d20 456c  r_model_elo = El
-000021c0: 6f4c 6561 6465 7262 6f61 7264 2829 2e67  oLeaderboard().g
-000021d0: 6574 5f65 6c6f 285b 6d79 4d6f 6465 6c50  et_elo([myModelP
-000021e0: 6c61 7965 725d 2c20 6e75 6d5f 6d61 7463  layer], num_matc
-000021f0: 6865 733d 3130 3029 0d0a 6060 600d 0a0d  hes=100)..```...
-00002200: 0a59 6f75 2063 616e 2066 696e 6420 616e  .You can find an
-00002210: 2065 7861 6d70 6c65 206f 6620 686f 7720   example of how 
-00002220: 746f 2075 7365 2074 6869 7320 746f 6f6c  to use this tool
-00002230: 2069 6e20 6120 476f 6f67 6c65 2043 6f6c   in a Google Col
-00002240: 6162 206e 6f74 6562 6f6f 6b20 5b68 6572  ab notebook [her
-00002250: 655d 2868 7474 7073 3a2f 2f63 6f6c 6162  e](https://colab
-00002260: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
-00002270: 2e63 6f6d 2f67 6974 6875 622f 6c75 6361  .com/github/luca
-00002280: 7342 6572 746f 6c61 2f43 6f6e 6e65 6374  sBertola/Connect
-00002290: 2d34 2d65 6e76 2f62 6c6f 622f 6d61 696e  -4-env/blob/main
-000022a0: 2f65 7865 6d70 6c65 732f 5050 4f5f 4d6c  /exemples/PPO_Ml
-000022b0: 7050 6f6c 6963 792e 6970 796e 6229 2e0d  pPolicy.ipynb)..
-000022c0: 0a0d 0a5b 215b 4f70 656e 2049 6e20 436f  ...[![Open In Co
-000022d0: 6c61 625d 2868 7474 7073 3a2f 2f63 6f6c  lab](https://col
-000022e0: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
-000022f0: 6c65 2e63 6f6d 2f61 7373 6574 732f 636f  le.com/assets/co
-00002300: 6c61 622d 6261 6467 652e 7376 6729 5d28  lab-badge.svg)](
-00002310: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-00002320: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-00002330: 6d2f 6769 7468 7562 2f6c 7563 6173 4265  m/github/lucasBe
-00002340: 7274 6f6c 612f 436f 6e6e 6563 742d 342d  rtola/Connect-4-
-00002350: 656e 762f 626c 6f62 2f6d 6169 6e2f 6578  env/blob/main/ex
-00002360: 656d 706c 6573 2f50 504f 5f4d 6c70 506f  emples/PPO_MlpPo
-00002370: 6c69 6379 2e69 7079 6e62 290d 0a0d 0a23  licy.ipynb)....#
-00002380: 2320 5465 7374 696e 670d 0a0d 0a57 6520  # Testing....We 
-00002390: 6265 6c69 6576 6520 696e 2074 6865 2069  believe in the i
-000023a0: 6d70 6f72 7461 6e63 6520 6f66 2074 6573  mportance of tes
-000023b0: 7469 6e67 2e20 5468 6174 2773 2077 6879  ting. That's why
-000023c0: 2077 6520 6861 7665 2069 6e63 6c75 6465   we have include
-000023d0: 6420 6120 7375 6974 6520 6f66 2074 6573  d a suite of tes
-000023e0: 7473 2069 6e20 7468 6520 6074 6573 7460  ts in the `test`
-000023f0: 2064 6972 6563 746f 7279 2e20 546f 2072   directory. To r
-00002400: 756e 2074 6865 2074 6573 7473 2c20 7369  un the tests, si
-00002410: 6d70 6c79 2075 7365 2074 6865 2063 6f6d  mply use the com
-00002420: 6d61 6e64 2060 7079 7465 7374 602e 0d0a  mand `pytest`...
-00002430: 0d0a 2323 2043 6f6e 7472 6962 7574 6520  ..## Contribute 
-00002440: 2620 5375 7070 6f72 740d 0a0d 0a57 6520  & Support....We 
-00002450: 7761 726d 6c79 2077 656c 636f 6d65 2063  warmly welcome c
-00002460: 6f6e 7472 6962 7574 696f 6e73 2066 726f  ontributions fro
-00002470: 6d20 7468 6520 636f 6d6d 756e 6974 792e  m the community.
-00002480: 2049 6620 796f 7520 6861 7665 2061 6e20   If you have an 
-00002490: 6964 6561 2066 6f72 2061 6e20 696d 7072  idea for an impr
-000024a0: 6f76 656d 656e 7420 6f72 2066 6f75 6e64  ovement or found
-000024b0: 2061 2062 7567 2c20 646f 6e27 7420 6865   a bug, don't he
-000024c0: 7369 7461 7465 2074 6f20 6f70 656e 2061  sitate to open a
-000024d0: 6e20 6973 7375 6520 6f72 2073 7562 6d69  n issue or submi
-000024e0: 7420 6120 7075 6c6c 2072 6571 7565 7374  t a pull request
-000024f0: 2e20 596f 7572 2069 6e70 7574 2069 7320  . Your input is 
-00002500: 6772 6561 746c 7920 6170 7072 6563 6961  greatly apprecia
-00002510: 7465 642c 2061 6e64 206f 7572 2070 726f  ted, and our pro
-00002520: 6a65 6374 2069 7320 6d61 6465 2062 6574  ject is made bet
-00002530: 7465 7220 6279 2079 6f75 7220 7061 7274  ter by your part
-00002540: 6963 6970 6174 696f 6e21 0d0a 0d0a 4966  icipation!....If
-00002550: 2079 6f75 2066 696e 6420 7468 6973 2072   you find this r
-00002560: 6570 6f73 6974 6f72 7920 7573 6566 756c  epository useful
-00002570: 2c20 706c 6561 7365 2067 6976 6520 6974  , please give it
-00002580: 2061 2073 7461 7221 0d0a 0d0a 2323 204c   a star!....## L
-00002590: 6963 656e 7365 0d0a 0d0a 5468 6973 2070  icense....This p
-000025a0: 726f 6a65 6374 2069 7320 6c69 6365 6e73  roject is licens
-000025b0: 6564 2075 6e64 6572 2074 6865 204d 4954  ed under the MIT
-000025c0: 204c 6963 656e 7365 2e20 5365 6520 7468   License. See th
-000025d0: 6520 604c 4943 454e 5345 6020 6669 6c65  e `LICENSE` file
-000025e0: 2066 6f72 2064 6574 6169 6c73 2e0d 0a     for details...
+00000860: 7269 6f73 2e0d 0a2d 202a 2a53 656c 662d  rios...- **Self-
+00000870: 506c 6179 2054 7261 696e 696e 672a 2a3a  Play Training**:
+00000880: 2054 6865 2065 6e76 6972 6f6e 6d65 6e74   The environment
+00000890: 2073 7570 706f 7274 7320 7365 6c66 2d70   supports self-p
+000008a0: 6c61 7920 7472 6169 6e69 6e67 2c20 616c  lay training, al
+000008b0: 6c6f 7769 6e67 2079 6f75 7220 4149 206d  lowing your AI m
+000008c0: 6f64 656c 2074 6f20 6c65 6172 6e20 6279  odel to learn by
+000008d0: 2070 6c61 7969 6e67 2061 6761 696e 7374   playing against
+000008e0: 2069 7473 656c 662c 2073 696d 696c 6172   itself, similar
+000008f0: 2074 6f20 7468 6520 6170 7072 6f61 6368   to the approach
+00000900: 2075 7365 6420 6279 2041 6c70 6861 476f   used by AlphaGo
+00000910: 205a 6572 6f2e 2054 6869 7320 6361 6e20   Zero. This can 
+00000920: 6c65 6164 2074 6f20 6d6f 7265 2061 6476  lead to more adv
+00000930: 616e 6365 6420 7374 7261 7465 6769 6573  anced strategies
+00000940: 2061 6e64 2061 2064 6565 7065 7220 756e   and a deeper un
+00000950: 6465 7273 7461 6e64 696e 6720 6f66 2074  derstanding of t
+00000960: 6865 2067 616d 6520 6173 2074 6865 206d  he game as the m
+00000970: 6f64 656c 2063 6f6e 7469 6e75 6f75 736c  odel continuousl
+00000980: 7920 696d 7072 6f76 6573 2074 6872 6f75  y improves throu
+00000990: 6768 2073 656c 662d 706c 6179 2e0d 0a2d  gh self-play...-
+000009a0: 202a 2a4f 7074 696d 697a 6564 2050 6572   **Optimized Per
+000009b0: 666f 726d 616e 6365 2a2a 3a20 5468 6520  formance**: The 
+000009c0: 656e 7669 726f 6e6d 656e 7420 6861 7320  environment has 
+000009d0: 6265 656e 2073 7065 6369 6669 6361 6c6c  been specificall
+000009e0: 7920 6465 7369 676e 6564 2077 6974 6820  y designed with 
+000009f0: 7065 7266 6f72 6d61 6e63 6520 696e 206d  performance in m
+00000a00: 696e 642c 2065 6e73 7572 696e 6720 7468  ind, ensuring th
+00000a10: 6174 2079 6f75 7220 6d6f 6465 6c73 2073  at your models s
+00000a20: 7065 6e64 2074 6865 6972 2074 696d 6520  pend their time 
+00000a30: 6c65 6172 6e69 6e67 2072 6174 6865 7220  learning rather 
+00000a40: 7468 616e 2070 6c61 7969 6e67 2074 6865  than playing the
+00000a50: 2067 616d 652e 2054 6869 7320 616c 6c6f   game. This allo
+00000a60: 7773 2066 6f72 2066 6173 7465 7220 7472  ws for faster tr
+00000a70: 6169 6e69 6e67 2061 6e64 206d 6f72 6520  aining and more 
+00000a80: 6566 6669 6369 656e 7420 7573 6520 6f66  efficient use of
+00000a90: 2063 6f6d 7075 7461 7469 6f6e 616c 2072   computational r
+00000aa0: 6573 6f75 7263 6573 2e0d 0a0d 0a0d 0a23  esources.......#
+00000ab0: 2320 496e 7374 616c 6c61 7469 6f6e 0d0a  # Installation..
+00000ac0: 0d0a 546f 2075 7365 2074 6865 204d 696e  ..To use the Min
+00000ad0: 6947 7269 6420 656e 7669 726f 6e6d 656e  iGrid environmen
+00000ae0: 742c 2079 6f75 2063 616e 2069 6e73 7461  t, you can insta
+00000af0: 6c6c 2069 7420 6469 7265 6374 6c79 2069  ll it directly i
+00000b00: 6e74 6f20 796f 7572 2070 726f 6a65 6374  nto your project
+00000b10: 2075 7369 6e67 2070 6970 3a0d 0a0d 0a60   using pip:....`
+00000b20: 6060 6261 7368 0d0a 7069 7020 696e 7374  ``bash..pip inst
+00000b30: 616c 6c20 6779 6d6e 6173 6975 6d2d 636f  all gymnasium-co
+00000b40: 6e6e 6563 742d 666f 7572 0d0a 6060 600d  nnect-four..```.
+00000b50: 0a0d 0a23 2320 5573 6167 650d 0a0d 0a49  ...## Usage....I
+00000b60: 6d70 6f72 7420 7468 6520 6043 6f6e 6e65  mport the `Conne
+00000b70: 6374 466f 7572 456e 7660 2063 6c61 7373  ctFourEnv` class
+00000b80: 2c20 616e 6420 6869 7320 6f70 706f 6e61  , and his oppona
+00000b90: 6e74 2028 666f 7220 6578 656d 706c 6520  nt (for exemple 
+00000ba0: 7468 6520 7665 7279 2065 6173 7920 706c  the very easy pl
+00000bb0: 6179 6572 2060 4261 6279 506c 6179 6572  ayer `BabyPlayer
+00000bc0: 6020 290d 0a0d 0a60 6060 7079 7468 6f6e  ` )....```python
+00000bd0: 0d0a 6672 6f6d 2063 6f6e 6e65 6374 5f66  ..from connect_f
+00000be0: 6f75 725f 6779 6d6e 6173 6975 6d20 696d  our_gymnasium im
+00000bf0: 706f 7274 2043 6f6e 6e65 6374 466f 7572  port ConnectFour
+00000c00: 456e 760d 0a66 726f 6d20 636f 6e6e 6563  Env..from connec
+00000c10: 745f 666f 7572 5f67 796d 6e61 7369 756d  t_four_gymnasium
+00000c20: 2e70 6c61 7965 7273 2069 6d70 6f72 7420  .players import 
+00000c30: 4261 6279 506c 6179 6572 0d0a 6060 600d  BabyPlayer..```.
+00000c40: 0a0d 0a48 6572 6520 6973 2061 2073 696d  ...Here is a sim
+00000c50: 706c 6520 6578 616d 706c 6520 6f66 2068  ple example of h
+00000c60: 6f77 2074 6f20 7573 6520 7468 6520 656e  ow to use the en
+00000c70: 7669 726f 6e6d 656e 7420 7769 7468 2050  vironment with P
+00000c80: 504f 3a0d 0a0d 0a60 6060 7079 7468 6f6e  PO:....```python
+00000c90: 0d0a 6672 6f6d 2063 6f6e 6e65 6374 5f66  ..from connect_f
+00000ca0: 6f75 725f 6779 6d6e 6173 6975 6d20 696d  our_gymnasium im
+00000cb0: 706f 7274 2043 6f6e 6e65 6374 466f 7572  port ConnectFour
+00000cc0: 456e 760d 0a66 726f 6d20 636f 6e6e 6563  Env..from connec
+00000cd0: 745f 666f 7572 5f67 796d 6e61 7369 756d  t_four_gymnasium
+00000ce0: 2e70 6c61 7965 7273 2069 6d70 6f72 7420  .players import 
+00000cf0: 4261 6279 506c 6179 6572 0d0a 6672 6f6d  BabyPlayer..from
+00000d00: 2073 7461 626c 655f 6261 7365 6c69 6e65   stable_baseline
+00000d10: 7333 2069 6d70 6f72 7420 5050 4f0d 0a20  s3 import PPO.. 
+00000d20: 2020 2020 2020 200d 0a65 6e76 203d 2043         ..env = C
+00000d30: 6f6e 6e65 6374 466f 7572 456e 7628 6f70  onnectFourEnv(op
+00000d40: 706f 6e65 6e74 3d42 6162 7950 6c61 7965  ponent=BabyPlaye
+00000d50: 7228 2929 0d0a 6d6f 6465 6c20 3d20 5050  r())..model = PP
+00000d60: 4f28 224d 6c70 506f 6c69 6379 222c 2065  O("MlpPolicy", e
+00000d70: 6e76 2c20 7665 7262 6f73 653d 3129 0d0a  nv, verbose=1)..
+00000d80: 0d0a 6d6f 6465 6c2e 6c65 6172 6e28 746f  ..model.learn(to
+00000d90: 7461 6c5f 7469 6d65 7374 6570 733d 2831  tal_timesteps=(1
+00000da0: 3030 3030 3029 290d 0a60 6060 0d0a 0d0a  00000))..```....
+00000db0: 466f 7220 6465 7461 696c 6564 2075 7361  For detailed usa
+00000dc0: 6765 2069 6e73 7472 7563 7469 6f6e 7320  ge instructions 
+00000dd0: 616e 6420 6578 616d 706c 6573 2c20 706c  and examples, pl
+00000de0: 6561 7365 2072 6566 6572 2074 6f20 7468  ease refer to th
+00000df0: 6520 5b65 7861 6d70 6c65 735d 2868 7474  e [examples](htt
+00000e00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000e10: 6c75 6361 7342 6572 746f 6c61 2f43 6f6e  lucasBertola/Con
+00000e20: 6e65 6374 2d34 2d47 796d 2d65 6e76 2d52  nect-4-Gym-env-R
+00000e30: 6569 6e66 6f72 6365 6d65 6e74 2d6c 6561  einforcement-lea
+00000e40: 726e 696e 672f 7472 6565 2f6d 6169 6e2f  rning/tree/main/
+00000e50: 6578 656d 706c 6573 2920 6469 7265 6374  exemples) direct
+00000e60: 6f72 7920 6f72 2063 6865 636b 206f 7574  ory or check out
+00000e70: 206f 7572 205b 436f 6c61 6220 4e6f 7465   our [Colab Note
+00000e80: 626f 6f6b 5d28 6874 7470 733a 2f2f 636f  book](https://co
+00000e90: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
+00000ea0: 676c 652e 636f 6d2f 6769 7468 7562 2f6c  gle.com/github/l
+00000eb0: 7563 6173 4265 7274 6f6c 612f 436f 6e6e  ucasBertola/Conn
+00000ec0: 6563 742d 342d 4779 6d2d 656e 762d 5265  ect-4-Gym-env-Re
+00000ed0: 696e 666f 7263 656d 656e 742d 6c65 6172  inforcement-lear
+00000ee0: 6e69 6e67 2f62 6c6f 622f 6d61 696e 2f65  ning/blob/main/e
+00000ef0: 7865 6d70 6c65 732f 5472 6169 6e5f 7070  xemples/Train_pp
+00000f00: 6f5f 616e 645f 7465 7374 2e69 7079 6e62  o_and_test.ipynb
+00000f10: 292e 0d0a 0d0a 0d0a 3c61 2068 7265 663d  ).......<a href=
+00000f20: 2268 7474 7073 3a2f 2f63 6f6c 6162 2e72  "https://colab.r
+00000f30: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
+00000f40: 6f6d 2f67 6974 6875 622f 6c75 6361 7342  om/github/lucasB
+00000f50: 6572 746f 6c61 2f43 6f6e 6e65 6374 2d34  ertola/Connect-4
+00000f60: 2d47 796d 2d65 6e76 2d52 6569 6e66 6f72  -Gym-env-Reinfor
+00000f70: 6365 6d65 6e74 2d6c 6561 726e 696e 672f  cement-learning/
+00000f80: 626c 6f62 2f6d 6169 6e2f 6578 656d 706c  blob/main/exempl
+00000f90: 6573 2f54 7261 696e 5f70 706f 5f61 6e64  es/Train_ppo_and
+00000fa0: 5f74 6573 742e 6970 796e 6222 2074 6172  _test.ipynb" tar
+00000fb0: 6765 743d 225f 626c 616e 6b22 3e3c 696d  get="_blank"><im
+00000fc0: 6720 7372 633d 2268 7474 7073 3a2f 2f63  g src="https://c
+00000fd0: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00000fe0: 6f67 6c65 2e63 6f6d 2f61 7373 6574 732f  ogle.com/assets/
+00000ff0: 636f 6c61 622d 6261 6467 652e 7376 6722  colab-badge.svg"
+00001000: 2061 6c74 3d22 4f70 656e 2049 6e20 436f   alt="Open In Co
+00001010: 6c61 6222 3e3c 2f61 3e0d 0a0d 0a23 2323  lab"></a>....###
+00001020: 2053 656c 662d 506c 6179 2054 7261 696e   Self-Play Train
+00001030: 696e 670d 0a0d 0a4f 6e65 2070 6f77 6572  ing....One power
+00001040: 6675 6c20 7465 6368 6e69 7175 6520 666f  ful technique fo
+00001050: 7220 7472 6169 6e69 6e67 2041 4920 6d6f  r training AI mo
+00001060: 6465 6c73 2069 7320 7365 6c66 2d70 6c61  dels is self-pla
+00001070: 792c 2077 6865 7265 2074 6865 2041 4920  y, where the AI 
+00001080: 6c65 6172 6e73 2062 7920 706c 6179 696e  learns by playin
+00001090: 6720 6167 6169 6e73 7420 6974 7365 6c66  g against itself
+000010a0: 2e20 5468 6973 2061 7070 726f 6163 682c  . This approach,
+000010b0: 2066 616d 6f75 736c 7920 7573 6564 2062   famously used b
+000010c0: 7920 416c 7068 6147 6f20 5a65 726f 2c20  y AlphaGo Zero, 
+000010d0: 6861 7320 7365 7665 7261 6c20 6164 7661  has several adva
+000010e0: 6e74 6167 6573 3a0d 0a0d 0a2d 202a 2a55  ntages:....- **U
+000010f0: 6e62 6961 7365 6420 6c65 6172 6e69 6e67  nbiased learning
+00001100: 2a2a 3a20 4279 2070 6c61 7969 6e67 2061  **: By playing a
+00001110: 6761 696e 7374 2069 7473 656c 662c 2074  gainst itself, t
+00001120: 6865 2041 4920 6d6f 6465 6c20 6973 206e  he AI model is n
+00001130: 6f74 2069 6e66 6c75 656e 6365 6420 6279  ot influenced by
+00001140: 2068 756d 616e 2073 7472 6174 6567 6965   human strategie
+00001150: 7320 6f72 206d 6574 686f 6473 2e20 5468  s or methods. Th
+00001160: 6973 2061 6c6c 6f77 7320 7468 6520 6d6f  is allows the mo
+00001170: 6465 6c20 746f 2064 6576 656c 6f70 2069  del to develop i
+00001180: 7473 206f 776e 2075 6e69 7175 6520 7374  ts own unique st
+00001190: 7261 7465 6769 6573 2061 6e64 2070 6f74  rategies and pot
+000011a0: 656e 7469 616c 6c79 2064 6973 636f 7665  entially discove
+000011b0: 7220 6e65 7720 7761 7973 206f 6620 706c  r new ways of pl
+000011c0: 6179 696e 6720 7468 6520 6761 6d65 2e0d  aying the game..
+000011d0: 0a2d 202a 2a43 6f6e 7469 6e75 6f75 7320  .- **Continuous 
+000011e0: 696d 7072 6f76 656d 656e 742a 2a3a 2041  improvement**: A
+000011f0: 7320 7468 6520 4149 206d 6f64 656c 2069  s the AI model i
+00001200: 6d70 726f 7665 732c 2069 7420 636f 6e74  mproves, it cont
+00001210: 696e 7561 6c6c 7920 6661 6365 7320 6120  inually faces a 
+00001220: 7374 726f 6e67 6572 206f 7070 6f6e 656e  stronger opponen
+00001230: 7420 2869 7473 656c 6629 2c20 7768 6963  t (itself), whic
+00001240: 6820 6865 6c70 7320 6974 2074 6f20 6c65  h helps it to le
+00001250: 6172 6e20 6d6f 7265 2061 6476 616e 6365  arn more advance
+00001260: 6420 7374 7261 7465 6769 6573 2061 6e64  d strategies and
+00001270: 2072 6566 696e 6520 6974 7320 6761 6d65   refine its game
+00001280: 706c 6179 2e0d 0a2d 202a 2a41 6461 7074  play...- **Adapt
+00001290: 6976 6520 6c65 6172 6e69 6e67 2a2a 3a20  ive learning**: 
+000012a0: 5468 6520 4149 206d 6f64 656c 2063 616e  The AI model can
+000012b0: 2061 6461 7074 2074 6f20 6974 7320 6f77   adapt to its ow
+000012c0: 6e20 7765 616b 6e65 7373 6573 2061 6e64  n weaknesses and
+000012d0: 2065 7870 6c6f 6974 2074 6865 6d2c 206c   exploit them, l
+000012e0: 6561 6469 6e67 2074 6f20 6120 6d6f 7265  eading to a more
+000012f0: 2072 6f62 7573 7420 616e 6420 7765 6c6c   robust and well
+00001300: 2d72 6f75 6e64 6564 2075 6e64 6572 7374  -rounded underst
+00001310: 616e 6469 6e67 206f 6620 7468 6520 6761  anding of the ga
+00001320: 6d65 2e0d 0a0d 0a48 6572 6527 7320 616e  me.....Here's an
+00001330: 2065 7861 6d70 6c65 206f 6620 686f 7720   example of how 
+00001340: 746f 2073 6574 2075 7020 7365 6c66 2d70  to set up self-p
+00001350: 6c61 7920 7472 6169 6e69 6e67 3a0d 0a0d  lay training:...
+00001360: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
+00001370: 2063 6f6e 6e65 6374 5f66 6f75 725f 6779   connect_four_gy
+00001380: 6d6e 6173 6975 6d20 696d 706f 7274 2043  mnasium import C
+00001390: 6f6e 6e65 6374 466f 7572 456e 762c 204d  onnectFourEnv, M
+000013a0: 6f64 656c 506c 6179 6572 0d0a 6672 6f6d  odelPlayer..from
+000013b0: 2073 7461 626c 655f 6261 7365 6c69 6e65   stable_baseline
+000013c0: 7333 2069 6d70 6f72 7420 5050 4f0d 0a0d  s3 import PPO...
+000013d0: 0a65 6e76 203d 2043 6f6e 6e65 6374 466f  .env = ConnectFo
+000013e0: 7572 456e 7628 6f70 706f 6e65 6e74 3d42  urEnv(opponent=B
+000013f0: 6162 7950 6c61 7965 7228 2929 0d0a 6d6f  abyPlayer())..mo
+00001400: 6465 6c20 3d20 5050 4f28 224d 6c70 506f  del = PPO("MlpPo
+00001410: 6c69 6379 222c 2065 6e76 2c20 7665 7262  licy", env, verb
+00001420: 6f73 653d 3129 0d0a 6f70 706f 6e65 6e74  ose=1)..opponent
+00001430: 203d 204d 6f64 656c 506c 6179 6572 286d   = ModelPlayer(m
+00001440: 6f64 656c 2c20 6e61 6d65 3d22 796f 7572  odel, name="your
+00001450: 7365 6c66 2229 0d0a 656e 762e 6368 616e  self")..env.chan
+00001460: 6765 5f6f 7070 6f6e 656e 7428 6f70 706f  ge_opponent(oppo
+00001470: 6e65 6e74 290d 0a0d 0a6d 6f64 656c 2e6c  nent)....model.l
+00001480: 6561 726e 2874 6f74 616c 5f74 696d 6573  earn(total_times
+00001490: 7465 7073 3d31 3030 3030 290d 0a60 6060  teps=10000)..```
+000014a0: 0d0a 0d0a 496e 2074 6869 7320 6578 616d  ....In this exam
+000014b0: 706c 652c 202c 2077 6520 6372 6561 7465  ple, , we create
+000014c0: 2061 2060 4d6f 6465 6c50 6c61 7965 7260   a `ModelPlayer`
+000014d0: 2075 7369 6e67 2074 6865 206d 6f64 656c   using the model
+000014e0: 2061 6e64 2073 6574 2069 7420 6173 2074   and set it as t
+000014f0: 6865 206f 7070 6f6e 656e 7420 666f 7220  he opponent for 
+00001500: 7468 6520 656e 7669 726f 6e6d 656e 742e  the environment.
+00001510: 2054 6869 7320 616c 6c6f 7773 2074 6865   This allows the
+00001520: 2041 4920 6d6f 6465 6c20 746f 2063 6f6e   AI model to con
+00001530: 7469 6e75 6520 6c65 6172 6e69 6e67 2062  tinue learning b
+00001540: 7920 706c 6179 696e 6720 6167 6169 6e73  y playing agains
+00001550: 7420 6974 7365 6c66 2e0d 0a0d 0a59 6f75  t itself.....You
+00001560: 2063 616e 2064 6972 6563 746c 7920 7465   can directly te
+00001570: 7374 2073 656c 662d 706c 6179 2074 7261  st self-play tra
+00001580: 696e 696e 6720 696e 2074 6865 2070 726f  ining in the pro
+00001590: 7669 6465 6420 476f 6f67 6c65 2043 6f6c  vided Google Col
+000015a0: 6162 206e 6f74 6562 6f6f 6b20 6174 2074  ab notebook at t
+000015b0: 6865 2066 6f6c 6c6f 7769 6e67 206c 696e  he following lin
+000015c0: 6b3a 0d0a 0d0a 5b21 5b4f 7065 6e20 496e  k:....[![Open In
+000015d0: 2043 6f6c 6162 5d28 6874 7470 733a 2f2f   Colab](https://
+000015e0: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+000015f0: 6f6f 676c 652e 636f 6d2f 6173 7365 7473  oogle.com/assets
+00001600: 2f63 6f6c 6162 2d62 6164 6765 2e73 7667  /colab-badge.svg
+00001610: 295d 2868 7474 7073 3a2f 2f63 6f6c 6162  )](https://colab
+00001620: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
+00001630: 2e63 6f6d 2f67 6974 6875 622f 6c75 6361  .com/github/luca
+00001640: 7342 6572 746f 6c61 2f43 6f6e 6e65 6374  sBertola/Connect
+00001650: 2d34 2d47 796d 2d65 6e76 2d52 6569 6e66  -4-Gym-env-Reinf
+00001660: 6f72 6365 6d65 6e74 2d6c 6561 726e 696e  orcement-learnin
+00001670: 672f 626c 6f62 2f6d 6169 6e2f 6578 656d  g/blob/main/exem
+00001680: 706c 6573 2f53 656c 665f 706c 6179 5f74  ples/Self_play_t
+00001690: 7261 696e 696e 672e 6970 796e 6229 0d0a  raining.ipynb)..
+000016a0: 0d0a 2323 2045 6e76 6972 6f6e 6d65 6e74  ..## Environment
+000016b0: 2044 6574 6169 6c73 0d0a 0d0a 496e 2074   Details....In t
+000016c0: 6869 7320 7365 6374 696f 6e2c 2077 6520  his section, we 
+000016d0: 7072 6f76 6964 6520 616e 206f 7665 7276  provide an overv
+000016e0: 6965 7720 6f66 2074 6865 2043 6f6e 6e65  iew of the Conne
+000016f0: 6374 2046 6f75 7220 656e 7669 726f 6e6d  ct Four environm
+00001700: 656e 742c 2069 6e63 6c75 6469 6e67 2074  ent, including t
+00001710: 6865 2061 6374 696f 6e20 7370 6163 652c  he action space,
+00001720: 206f 6273 6572 7661 7469 6f6e 2073 7061   observation spa
+00001730: 6365 2c20 7265 7761 7264 732c 2061 6e64  ce, rewards, and
+00001740: 2065 7069 736f 6465 2074 6572 6d69 6e61   episode termina
+00001750: 7469 6f6e 2063 6f6e 6469 7469 6f6e 732e  tion conditions.
+00001760: 0d0a 0d0a 2323 2320 4163 7469 6f6e 2053  ....### Action S
+00001770: 7061 6365 0d0a 0d0a 5468 6520 6163 7469  pace....The acti
+00001780: 6f6e 2073 7061 6365 2069 6e20 7468 6520  on space in the 
+00001790: 436f 6e6e 6563 7420 466f 7572 2065 6e76  Connect Four env
+000017a0: 6972 6f6e 6d65 6e74 2069 7320 6469 7363  ironment is disc
+000017b0: 7265 7465 2c20 7769 7468 2061 2074 6f74  rete, with a tot
+000017c0: 616c 206f 6620 3720 706f 7373 6962 6c65  al of 7 possible
+000017d0: 2061 6374 696f 6e73 2e20 4561 6368 2061   actions. Each a
+000017e0: 6374 696f 6e20 636f 7272 6573 706f 6e64  ction correspond
+000017f0: 7320 746f 2061 2063 6f6c 756d 6e20 696e  s to a column in
+00001800: 2074 6865 2067 616d 6520 626f 6172 6420   the game board 
+00001810: 7768 6572 6520 6120 706c 6179 6572 2063  where a player c
+00001820: 616e 2064 726f 7020 7468 6569 7220 7069  an drop their pi
+00001830: 6563 652e 2054 6865 2061 6374 696f 6e20  ece. The action 
+00001840: 7370 6163 6520 6973 2072 6570 7265 7365  space is represe
+00001850: 6e74 6564 2061 7320 666f 6c6c 6f77 733a  nted as follows:
+00001860: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a73  ....```python..s
+00001870: 656c 662e 6163 7469 6f6e 5f73 7061 6365  elf.action_space
+00001880: 203d 2073 7061 6365 732e 4469 7363 7265   = spaces.Discre
+00001890: 7465 2873 656c 662e 434f 4c55 4d4e 535f  te(self.COLUMNS_
+000018a0: 434f 554e 5429 0d0a 6060 600d 0a0d 0a23  COUNT)..```....#
+000018b0: 2323 204f 6273 6572 7661 7469 6f6e 2053  ## Observation S
+000018c0: 7061 6365 0d0a 0d0a 5468 6520 6f62 7365  pace....The obse
+000018d0: 7276 6174 696f 6e20 7370 6163 6520 696e  rvation space in
+000018e0: 2074 6865 2043 6f6e 6e65 6374 2046 6f75   the Connect Fou
+000018f0: 7220 656e 7669 726f 6e6d 656e 7420 6973  r environment is
+00001900: 2061 2032 4420 6172 7261 7920 7265 7072   a 2D array repr
+00001910: 6573 656e 7469 6e67 2074 6865 2067 616d  esenting the gam
+00001920: 6520 626f 6172 642e 2045 6163 6820 6365  e board. Each ce
+00001930: 6c6c 2069 6e20 7468 6520 6172 7261 7920  ll in the array 
+00001940: 6361 6e20 6861 7665 206f 6e65 206f 6620  can have one of 
+00001950: 7468 7265 6520 706f 7373 6962 6c65 2076  three possible v
+00001960: 616c 7565 733a 2030 2028 656d 7074 7929  alues: 0 (empty)
+00001970: 2c20 3120 2870 6c61 7965 7227 7320 7069  , 1 (player's pi
+00001980: 6563 6529 2c20 6f72 2032 2028 6f70 706f  ece), or 2 (oppo
+00001990: 6e65 6e74 2773 2070 6965 6365 292e 2054  nent's piece). T
+000019a0: 6865 206f 6273 6572 7661 7469 6f6e 2073  he observation s
+000019b0: 7061 6365 2069 7320 6465 6669 6e65 6420  pace is defined 
+000019c0: 6173 2066 6f6c 6c6f 7773 3a0d 0a0d 0a60  as follows:....`
+000019d0: 6060 7079 7468 6f6e 0d0a 7365 6c66 2e6f  ``python..self.o
+000019e0: 6273 6572 7661 7469 6f6e 5f73 7061 6365  bservation_space
+000019f0: 203d 2073 7061 6365 732e 426f 7828 6c6f   = spaces.Box(lo
+00001a00: 773d 302c 2068 6967 683d 322c 2073 6861  w=0, high=2, sha
+00001a10: 7065 3d28 7365 6c66 2e52 4f57 535f 434f  pe=(self.ROWS_CO
+00001a20: 554e 542c 2073 656c 662e 434f 4c55 4d4e  UNT, self.COLUMN
+00001a30: 535f 434f 554e 5429 2c20 6474 7970 653d  S_COUNT), dtype=
+00001a40: 6e70 2e69 6e74 3332 290d 0a60 6060 0d0a  np.int32)..```..
+00001a50: 0d0a 2323 2320 5265 7761 7264 730d 0a0d  ..### Rewards...
+00001a60: 0a54 6865 2072 6577 6172 6420 7379 7374  .The reward syst
+00001a70: 656d 2069 6e20 7468 6520 436f 6e6e 6563  em in the Connec
+00001a80: 7420 466f 7572 2065 6e76 6972 6f6e 6d65  t Four environme
+00001a90: 6e74 2069 7320 6465 7369 676e 6564 2074  nt is designed t
+00001aa0: 6f20 656e 636f 7572 6167 6520 7468 6520  o encourage the 
+00001ab0: 4149 206d 6f64 656c 2074 6f20 6c65 6172  AI model to lear
+00001ac0: 6e20 686f 7720 746f 2077 696e 2074 6865  n how to win the
+00001ad0: 2067 616d 652e 2054 6865 2072 6577 6172   game. The rewar
+00001ae0: 6473 2061 7265 2061 7320 666f 6c6c 6f77  ds are as follow
+00001af0: 733a 0d0a 0d0a 2d20 4120 7265 7761 7264  s:....- A reward
+00001b00: 206f 6620 2b31 2069 7320 6769 7665 6e20   of +1 is given 
+00001b10: 7768 656e 2074 6865 2041 4920 6d6f 6465  when the AI mode
+00001b20: 6c20 7769 6e73 2074 6865 2067 616d 6520  l wins the game 
+00001b30: 6279 2063 6f6e 6e65 6374 696e 6720 666f  by connecting fo
+00001b40: 7572 206f 6620 6974 7320 7069 6563 6573  ur of its pieces
+00001b50: 2069 6e20 6120 726f 772c 2065 6974 6865   in a row, eithe
+00001b60: 7220 686f 7269 7a6f 6e74 616c 6c79 2c20  r horizontally, 
+00001b70: 7665 7274 6963 616c 6c79 2c20 6f72 2064  vertically, or d
+00001b80: 6961 676f 6e61 6c6c 792e 0d0a 2d20 4120  iagonally...- A 
+00001b90: 7265 7761 7264 206f 6620 2d31 2069 7320  reward of -1 is 
+00001ba0: 6769 7665 6e20 7768 656e 2074 6865 2041  given when the A
+00001bb0: 4920 6d6f 6465 6c20 6c6f 7365 7320 7468  I model loses th
+00001bc0: 6520 6761 6d65 206f 7220 706c 6179 7320  e game or plays 
+00001bd0: 616e 2069 6e76 616c 6964 2061 6374 696f  an invalid actio
+00001be0: 6e2e 0d0a 2d20 4120 7265 7761 7264 206f  n...- A reward o
+00001bf0: 6620 3020 6973 2067 6976 656e 2066 6f72  f 0 is given for
+00001c00: 2061 6c6c 206f 7468 6572 2061 6374 696f   all other actio
+00001c10: 6e73 2074 6861 7420 646f 206e 6f74 2072  ns that do not r
+00001c20: 6573 756c 7420 696e 2061 2077 696e 206f  esult in a win o
+00001c30: 7220 6c6f 7373 2e0d 0a0d 0a23 2323 2045  r loss.....### E
+00001c40: 7069 736f 6465 2054 6572 6d69 6e61 7469  pisode Terminati
+00001c50: 6f6e 0d0a 0d0a 416e 2065 7069 736f 6465  on....An episode
+00001c60: 2069 6e20 7468 6520 436f 6e6e 6563 7420   in the Connect 
+00001c70: 466f 7572 2065 6e76 6972 6f6e 6d65 6e74  Four environment
+00001c80: 2074 6572 6d69 6e61 7465 7320 756e 6465   terminates unde
+00001c90: 7220 7468 6520 666f 6c6c 6f77 696e 6720  r the following 
+00001ca0: 636f 6e64 6974 696f 6e73 3a0d 0a0d 0a2d  conditions:....-
+00001cb0: 2054 6865 2041 4920 6d6f 6465 6c20 7769   The AI model wi
+00001cc0: 6e73 2074 6865 2067 616d 6520 6279 2063  ns the game by c
+00001cd0: 6f6e 6e65 6374 696e 6720 666f 7572 206f  onnecting four o
+00001ce0: 6620 6974 7320 7069 6563 6573 2069 6e20  f its pieces in 
+00001cf0: 6120 726f 772c 2065 6974 6865 7220 686f  a row, either ho
+00001d00: 7269 7a6f 6e74 616c 6c79 2c20 7665 7274  rizontally, vert
+00001d10: 6963 616c 6c79 2c20 6f72 2064 6961 676f  ically, or diago
+00001d20: 6e61 6c6c 792e 0d0a 2d20 5468 6520 4149  nally...- The AI
+00001d30: 206d 6f64 656c 206c 6f73 6573 2074 6865   model loses the
+00001d40: 2067 616d 6520 6279 2061 6c6c 6f77 696e   game by allowin
+00001d50: 6720 7468 6520 6f70 706f 6e65 6e74 2074  g the opponent t
+00001d60: 6f20 636f 6e6e 6563 7420 666f 7572 206f  o connect four o
+00001d70: 6620 7468 6569 7220 7069 6563 6573 2069  f their pieces i
+00001d80: 6e20 6120 726f 772c 206f 7220 6279 2070  n a row, or by p
+00001d90: 6c61 7969 6e67 2061 6e20 696e 7661 6c69  laying an invali
+00001da0: 6420 6163 7469 6f6e 2e0d 0a2d 2054 6865  d action...- The
+00001db0: 2067 616d 6520 626f 6172 6420 6973 2063   game board is c
+00001dc0: 6f6d 706c 6574 656c 7920 6669 6c6c 6564  ompletely filled
+00001dd0: 2c20 7265 7375 6c74 696e 6720 696e 2061  , resulting in a
+00001de0: 2064 7261 772e 0d0a 0d0a 5768 656e 2061   draw.....When a
+00001df0: 6e20 6570 6973 6f64 6520 7465 726d 696e  n episode termin
+00001e00: 6174 6573 2c20 7468 6520 656e 7669 726f  ates, the enviro
+00001e10: 6e6d 656e 7420 6973 2072 6573 6574 2c20  nment is reset, 
+00001e20: 616e 6420 6120 6e65 7720 6570 6973 6f64  and a new episod
+00001e30: 6520 6265 6769 6e73 2e0d 0a0d 0a23 2320  e begins.....## 
+00001e40: 4176 6169 6c61 626c 6520 506c 6179 6572  Available Player
+00001e50: 730d 0a0d 0a54 6869 7320 6c69 6272 6172  s....This librar
+00001e60: 7920 7072 6f76 6964 6573 2061 2063 6f6c  y provides a col
+00001e70: 6c65 6374 696f 6e20 6f66 2043 6f6e 6e65  lection of Conne
+00001e80: 6374 2046 6f75 7220 626f 7473 2077 6974  ct Four bots wit
+00001e90: 6820 6469 6666 6572 656e 7420 736b 696c  h different skil
+00001ea0: 6c20 6c65 7665 6c73 2e20 5468 6573 6520  l levels. These 
+00001eb0: 626f 7473 2063 616e 2062 6520 7573 6564  bots can be used
+00001ec0: 2066 6f72 2076 6172 696f 7573 2070 7572   for various pur
+00001ed0: 706f 7365 732c 2073 7563 6820 6173 3a0d  poses, such as:.
+00001ee0: 0a0d 0a2d 202a 2a4c 6561 726e 696e 6720  ...- **Learning 
+00001ef0: 6279 2070 6c61 7969 6e67 2061 6761 696e  by playing again
+00001f00: 7374 2074 6865 6d2a 2a3a 2059 6f75 2063  st them**: You c
+00001f10: 616e 2069 6d70 726f 7665 2079 6f75 7220  an improve your 
+00001f20: 4149 206d 6f64 656c 2062 7920 706c 6179  AI model by play
+00001f30: 696e 6720 6167 6169 6e73 7420 7468 6573  ing against thes
+00001f40: 6520 626f 7473 2c20 7768 6963 6820 7261  e bots, which ra
+00001f50: 6e67 6520 6672 6f6d 2062 6567 696e 6e65  nge from beginne
+00001f60: 7220 746f 2061 6476 616e 6365 6420 6c65  r to advanced le
+00001f70: 7665 6c73 2e0d 0a2d 202a 2a43 6f6d 7061  vels...- **Compa
+00001f80: 7269 6e67 2074 6865 206c 6576 656c 206f  ring the level o
+00001f90: 6620 7365 6c66 2d6c 6561 726e 696e 6720  f self-learning 
+00001fa0: 6d6f 6465 6c73 2a2a 3a20 4279 2070 6c61  models**: By pla
+00001fb0: 7969 6e67 2061 6761 696e 7374 2074 6865  ying against the
+00001fc0: 7365 2062 6f74 732c 2079 6f75 2063 616e  se bots, you can
+00001fd0: 2065 7661 6c75 6174 6520 7468 6520 7065   evaluate the pe
+00001fe0: 7266 6f72 6d61 6e63 6520 6f66 2079 6f75  rformance of you
+00001ff0: 7220 7365 6c66 2d6c 6561 726e 696e 6720  r self-learning 
+00002000: 6d6f 6465 6c20 616e 6420 706f 7369 7469  model and positi
+00002010: 6f6e 2069 7420 696e 2074 6572 6d73 206f  on it in terms o
+00002020: 6620 736b 696c 6c20 6c65 7665 6c20 616e  f skill level an
+00002030: 6420 656c 6f2e 0d0a 0d0a 596f 7520 6361  d elo.....You ca
+00002040: 6e20 696e 7465 6772 6174 6520 706c 6179  n integrate play
+00002050: 6572 7320 6173 206f 7070 6f6e 656e 7473  ers as opponents
+00002060: 2069 6e20 796f 7572 2067 796d 2065 6e76   in your gym env
+00002070: 6972 6f6e 6d65 6e74 206c 696b 6520 7468  ironment like th
+00002080: 6973 3a0d 0a0d 0a60 6060 7079 7468 6f6e  is:....```python
+00002090: 0d0a 656e 7620 3d20 436f 6e6e 6563 7446  ..env = ConnectF
+000020a0: 6f75 7245 6e76 286f 7070 6f6e 656e 743d  ourEnv(opponent=
+000020b0: 4261 6279 506c 6179 6572 2829 290d 0a60  BabyPlayer())..`
+000020c0: 6060 0d0a 0d0a 2323 2320 506c 6179 6572  ``....### Player
+000020d0: 2044 6573 6372 6970 7469 6f6e 730d 0a0d   Descriptions...
+000020e0: 0a2d 202a 2a4d 696e 4d61 7850 6c61 7965  .- **MinMaxPlaye
+000020f0: 722a 2a3a 2041 6e20 696d 706c 656d 656e  r**: An implemen
+00002100: 7461 7469 6f6e 206f 6620 7468 6520 4d69  tation of the Mi
+00002110: 6e69 6d61 7820 616c 676f 7269 7468 6d2e  nimax algorithm.
+00002120: 2043 616e 2062 6520 7573 6564 2077 6974   Can be used wit
+00002130: 6820 6469 6666 6572 656e 7420 7365 6172  h different sear
+00002140: 6368 2064 6570 7468 7320 2865 2e67 2e2c  ch depths (e.g.,
+00002150: 2060 4d69 6e4d 6178 506c 6179 6572 2864   `MinMaxPlayer(d
+00002160: 6570 7468 3d33 2960 292c 2062 7574 2069  epth=3)`), but i
+00002170: 7420 6973 2076 6572 7920 736c 6f77 2c20  t is very slow, 
+00002180: 736f 2069 7420 6973 206e 6f74 2072 6563  so it is not rec
+00002190: 6f6d 6d65 6e64 6564 2066 6f72 2067 656e  ommended for gen
+000021a0: 6572 616c 2075 7365 2e20 416c 6c20 6f74  eral use. All ot
+000021b0: 6865 7220 616c 676f 7269 7468 6d73 2061  her algorithms a
+000021c0: 7265 206d 7563 6820 6661 7374 6572 2e0d  re much faster..
+000021d0: 0a0d 0a2d 202a 2a42 6162 7950 6c61 7965  ...- **BabyPlaye
+000021e0: 722a 2a3a 2050 6c61 7973 2072 616e 646f  r**: Plays rando
+000021f0: 6d20 6d6f 7665 732e 0d0a 0d0a 2d20 2a2a  m moves.....- **
+00002200: 4368 696c 6450 6c61 7965 722a 2a3a 2050  ChildPlayer**: P
+00002210: 6c61 7973 2072 616e 646f 6d20 6d6f 7665  lays random move
+00002220: 732c 2062 7574 2069 6620 7468 6572 6520  s, but if there 
+00002230: 6973 2061 2077 696e 6e69 6e67 206d 6f76  is a winning mov
+00002240: 652c 2069 7420 7769 6c6c 2070 6c61 7920  e, it will play 
+00002250: 6974 2e0d 0a0d 0a2d 202a 2a43 6869 6c64  it.....- **Child
+00002260: 536d 6172 7465 7250 6c61 7965 722a 2a3a  SmarterPlayer**:
+00002270: 2053 616d 6520 6173 2043 6869 6c64 506c   Same as ChildPl
+00002280: 6179 6572 2c20 6275 7420 6966 2074 6865  ayer, but if the
+00002290: 7265 2069 7320 6120 6d6f 7665 2074 6861  re is a move tha
+000022a0: 7420 776f 756c 6420 6d61 6b65 2074 6865  t would make the
+000022b0: 206f 7070 6f6e 656e 7420 7769 6e2c 2069   opponent win, i
+000022c0: 7420 7769 6c6c 2070 6c61 7920 7468 6174  t will play that
+000022d0: 206d 6f76 6520 746f 2062 6c6f 636b 2074   move to block t
+000022e0: 6865 206f 7070 6f6e 656e 742e 0d0a 0d0a  he opponent.....
+000022f0: 2d20 2a2a 5465 656e 6167 6572 506c 6179  - **TeenagerPlay
+00002300: 6572 2a2a 3a20 5361 6d65 2061 7320 4368  er**: Same as Ch
+00002310: 696c 6453 6d61 7274 6572 506c 6179 6572  ildSmarterPlayer
+00002320: 2c20 6275 7420 6578 636c 7564 6573 206d  , but excludes m
+00002330: 6f76 6573 2074 6861 7420 776f 756c 6420  oves that would 
+00002340: 616c 6c6f 7720 7468 6520 6f70 706f 6e65  allow the oppone
+00002350: 6e74 2074 6f20 7769 6e20 6966 2074 6865  nt to win if the
+00002360: 7920 706c 6179 206f 6e20 746f 7020 6f66  y play on top of
+00002370: 2069 742e 0d0a 0d0a 2d20 2a2a 5465 656e   it.....- **Teen
+00002380: 6167 6572 536d 6172 7465 7250 6c61 7965  agerSmarterPlaye
+00002390: 722a 2a3a 2053 616d 6520 6173 2054 6565  r**: Same as Tee
+000023a0: 6e61 6765 7250 6c61 7965 722c 2062 7574  nagerPlayer, but
+000023b0: 2063 6865 636b 7320 6966 2061 206d 6f76   checks if a mov
+000023c0: 6520 6372 6561 7465 7320 6120 6c69 6e65  e creates a line
+000023d0: 206f 6620 7468 7265 6520 746f 6b65 6e73   of three tokens
+000023e0: 2077 6974 6820 6176 6169 6c61 626c 6520   with available 
+000023f0: 7370 6163 6573 206f 6e20 626f 7468 2073  spaces on both s
+00002400: 6964 6573 2e20 4966 2073 6f2c 2069 7420  ides. If so, it 
+00002410: 7769 6c6c 2070 6c61 7920 7468 6174 206d  will play that m
+00002420: 6f76 652e 0d0a 0d0a 2d20 2a2a 4164 756c  ove.....- **Adul
+00002430: 7450 6c61 7965 722a 2a3a 2053 616d 6520  tPlayer**: Same 
+00002440: 6173 2054 6565 6e61 6765 7253 6d61 7274  as TeenagerSmart
+00002450: 6572 506c 6179 6572 2c20 6275 7420 616c  erPlayer, but al
+00002460: 736f 2063 6865 636b 7320 6966 2061 206d  so checks if a m
+00002470: 6f76 6520 6372 6561 7465 7320 6120 6c69  ove creates a li
+00002480: 6e65 206f 6620 7468 7265 6520 746f 6b65  ne of three toke
+00002490: 6e73 2077 6974 6820 6176 6169 6c61 626c  ns with availabl
+000024a0: 6520 7370 6163 6573 206f 6e20 626f 7468  e spaces on both
+000024b0: 2073 6964 6573 2066 6f72 2074 6865 206f   sides for the o
+000024c0: 7070 6f6e 656e 742e 2049 6620 736f 2c20  pponent. If so, 
+000024d0: 6974 2077 696c 6c20 706c 6179 2074 6861  it will play tha
+000024e0: 7420 6d6f 7665 2074 6f20 626c 6f63 6b20  t move to block 
+000024f0: 7468 6520 6f70 706f 6e65 6e74 2e0d 0a0d  the opponent....
+00002500: 0a2d 202a 2a41 6475 6c74 536d 6172 7465  .- **AdultSmarte
+00002510: 7250 6c61 7965 722a 2a3a 2053 616d 6520  rPlayer**: Same 
+00002520: 6173 2041 6475 6c74 506c 6179 6572 2c20  as AdultPlayer, 
+00002530: 6275 7420 6368 6563 6b73 2069 6620 6120  but checks if a 
+00002540: 6d6f 7665 2061 6c6c 6f77 7320 746f 2063  move allows to c
+00002550: 7265 6174 6520 6d75 6c74 6970 6c65 2077  reate multiple w
+00002560: 6179 7320 746f 2077 696e 2061 6e64 2070  ays to win and p
+00002570: 6c61 7973 2074 6861 7420 6d6f 7665 2e20  lays that move. 
+00002580: 416c 736f 2063 6865 636b 7320 6966 2061  Also checks if a
+00002590: 206d 6f76 6520 616c 6c6f 7773 2074 6865   move allows the
+000025a0: 206f 7070 6f6e 656e 7420 746f 2063 7265   opponent to cre
+000025b0: 6174 6520 6d75 6c74 6970 6c65 2077 6179  ate multiple way
+000025c0: 7320 746f 2077 696e 2061 6e64 2070 6c61  s to win and pla
+000025d0: 7973 2074 6861 7420 6d6f 7665 2074 6f20  ys that move to 
+000025e0: 7072 6f74 6563 7420 6974 7365 6c66 2e0d  protect itself..
+000025f0: 0a0d 0a2d 202a 2a43 6f6e 736f 6c65 506c  ...- **ConsolePl
+00002600: 6179 6572 2a2a 3a20 4173 6b73 2066 6f72  ayer**: Asks for
+00002610: 206d 6f76 6573 2074 6f20 706c 6179 2069   moves to play i
+00002620: 6e20 7468 6520 636f 6e73 6f6c 652e 2050  n the console. P
+00002630: 6572 6665 6374 2066 6f72 2074 6573 7469  erfect for testi
+00002640: 6e67 2079 6f75 7220 6f77 6e20 4149 2e0d  ng your own AI..
+00002650: 0a0d 0a23 2323 2045 6c6f 2052 6174 696e  ...### Elo Ratin
+00002660: 6773 0d0a 0d0a 4865 7265 2061 7265 2074  gs....Here are t
+00002670: 6865 2045 6c6f 2072 6174 696e 6773 206f  he Elo ratings o
+00002680: 6620 7468 6520 6469 6666 6572 656e 7420  f the different 
+00002690: 616c 676f 7269 7468 6d73 3a0d 0a0d 0a60  algorithms:....`
+000026a0: 6060 0d0a 312e 2041 6475 6c74 536d 6172  ``..1. AdultSmar
+000026b0: 7465 7250 6c61 7965 723a 2020 2020 3137  terPlayer:    17
+000026c0: 3637 0d0a 322e 2041 6475 6c74 506c 6179  67..2. AdultPlay
+000026d0: 6572 3a20 2020 2020 2020 2020 2020 3137  er:           17
+000026e0: 3132 0d0a 332e 204d 696e 696d 6178 506c  12..3. MinimaxPl
+000026f0: 6179 6572 2064 6570 7468 2033 3a20 3136  ayer depth 3: 16
+00002700: 3732 0d0a 342e 204d 696e 696d 6178 506c  72..4. MinimaxPl
+00002710: 6179 6572 2064 6570 7468 2032 3a20 3136  ayer depth 2: 16
+00002720: 3232 0d0a 352e 2054 6565 6e61 6765 7253  22..5. TeenagerS
+00002730: 6d61 7274 6572 506c 6179 6572 3a20 3136  marterPlayer: 16
+00002740: 3131 0d0a 362e 2054 6565 6e61 6765 7250  11..6. TeenagerP
+00002750: 6c61 7965 723a 2020 2020 2020 2020 3136  layer:        16
+00002760: 3034 0d0a 372e 2043 6869 6c64 536d 6172  04..7. ChildSmar
+00002770: 7465 7250 6c61 7965 723a 2020 2020 3135  terPlayer:    15
+00002780: 3235 0d0a 382e 204d 696e 696d 6178 506c  25..8. MinimaxPl
+00002790: 6179 6572 2064 6570 7468 2031 3a20 3132  ayer depth 1: 12
+000027a0: 3230 0d0a 392e 2043 6869 6c64 506c 6179  20..9. ChildPlay
+000027b0: 6572 3a20 2020 2020 2020 2020 2020 3132  er:           12
+000027c0: 3038 0d0a 3130 2e20 4261 6279 506c 6179  08..10. BabyPlay
+000027d0: 6572 3a20 2020 2020 2020 2020 2020 2039  er:            9
+000027e0: 3935 0d0a 6060 600d 0a0d 0a49 6e20 6164  95..```....In ad
+000027f0: 6469 7469 6f6e 2074 6f20 7468 6520 7072  dition to the pr
+00002800: 6f76 6964 6564 2070 6c61 7965 7273 2c20  ovided players, 
+00002810: 7765 2061 6c73 6f20 6f66 6665 7220 6120  we also offer a 
+00002820: 746f 6f6c 2074 6f20 6576 616c 7561 7465  tool to evaluate
+00002830: 2074 6865 2045 6c6f 2072 6174 696e 6720   the Elo rating 
+00002840: 6f66 2079 6f75 7220 6f77 6e20 4149 206d  of your own AI m
+00002850: 6f64 656c 2e20 5468 6973 2069 7320 6578  odel. This is ex
+00002860: 7472 656d 656c 7920 7573 6566 756c 2074  tremely useful t
+00002870: 6f20 6861 7665 2061 6e20 2261 6273 6f6c  o have an "absol
+00002880: 7574 6522 2069 6465 6120 6f66 2074 6865  ute" idea of the
+00002890: 2070 726f 6772 6573 7320 6f66 2079 6f75   progress of you
+000028a0: 7220 4149 2e20 466f 7220 6578 616d 706c  r AI. For exampl
+000028b0: 652c 2069 6620 616e 2041 4920 6c65 6172  e, if an AI lear
+000028c0: 6e73 2062 7920 6669 6768 7469 6e67 2061  ns by fighting a
+000028d0: 6761 696e 7374 2069 7473 656c 662c 2077  gainst itself, w
+000028e0: 6520 6b6e 6f77 2074 6861 7420 6974 2069  e know that it i
+000028f0: 7320 6765 7474 696e 6720 7374 726f 6e67  s getting strong
+00002900: 6572 2061 7320 6974 2077 6f75 6c64 2062  er as it would b
+00002910: 6520 6162 6c65 2074 6f20 7769 6e20 6167  e able to win ag
+00002920: 6169 6e73 7420 6974 7320 6f6c 6465 7220  ainst its older 
+00002930: 7665 7273 696f 6e73 2c20 6275 7420 7468  versions, but th
+00002940: 6973 2069 7320 6e6f 7420 656e 6f75 6768  is is not enough
+00002950: 2074 6f20 6576 616c 7561 7465 2069 6620   to evaluate if 
+00002960: 6974 2068 6173 206c 6561 726e 6564 2061  it has learned a
+00002970: 206c 6f74 2e20 5468 6973 2069 7320 7768   lot. This is wh
+00002980: 6572 6520 6f75 7220 746f 6f6c 2063 6f6d  ere our tool com
+00002990: 6573 2069 6e2c 2077 6869 6368 2061 6c6c  es in, which all
+000029a0: 6f77 7320 796f 7520 746f 2067 6976 6520  ows you to give 
+000029b0: 616e 2045 6c6f 2072 6174 696e 6720 746f  an Elo rating to
+000029c0: 2074 6865 2041 492e 0d0a 0d0a 4865 7265   the AI.....Here
+000029d0: 2069 7320 686f 7720 746f 2075 7365 2069   is how to use i
+000029e0: 7420 696e 2050 7974 686f 6e3a 0d0a 0d0a  t in Python:....
+000029f0: 6060 6070 7974 686f 6e0d 0a65 6e76 203d  ```python..env =
+00002a00: 2043 6f6e 6e65 6374 466f 7572 456e 7628   ConnectFourEnv(
+00002a10: 6f70 706f 6e65 6e74 3d42 6162 7950 6c61  opponent=BabyPla
+00002a20: 7965 7228 2929 0d0a 6d6f 6465 6c20 3d20  yer())..model = 
+00002a30: 5050 4f28 224d 6c70 506f 6c69 6379 222c  PPO("MlpPolicy",
+00002a40: 2065 6e76 290d 0a6d 6f64 656c 2e6c 6561   env)..model.lea
+00002a50: 726e 2874 6f74 616c 5f74 696d 6573 7465  rn(total_timeste
+00002a60: 7073 3d31 3030 3030 290d 0a0d 0a6d 794d  ps=10000)....myM
+00002a70: 6f64 656c 506c 6179 6572 203d 204d 6f64  odelPlayer = Mod
+00002a80: 656c 506c 6179 6572 286d 6f64 656c 2c6e  elPlayer(model,n
+00002a90: 616d 653d 2259 6f75 7220 7472 6169 6e65  ame="Your traine
+00002aa0: 6420 4d6f 6465 6c22 290d 0a0d 0a79 6f75  d Model")....you
+00002ab0: 725f 6d6f 6465 6c5f 656c 6f20 3d20 456c  r_model_elo = El
+00002ac0: 6f4c 6561 6465 7262 6f61 7264 2829 2e67  oLeaderboard().g
+00002ad0: 6574 5f65 6c6f 285b 6d79 4d6f 6465 6c50  et_elo([myModelP
+00002ae0: 6c61 7965 725d 2c20 6e75 6d5f 6d61 7463  layer], num_matc
+00002af0: 6865 733d 3130 3029 0d0a 6060 600d 0a0d  hes=100)..```...
+00002b00: 0a59 6f75 2063 616e 2066 696e 6420 616e  .You can find an
+00002b10: 2065 7861 6d70 6c65 206f 6620 686f 7720   example of how 
+00002b20: 746f 2075 7365 2074 6869 7320 746f 6f6c  to use this tool
+00002b30: 2069 6e20 6120 476f 6f67 6c65 2043 6f6c   in a Google Col
+00002b40: 6162 206e 6f74 6562 6f6f 6b20 5b68 6572  ab notebook [her
+00002b50: 655d 2868 7474 7073 3a2f 2f63 6f6c 6162  e](https://colab
+00002b60: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
+00002b70: 2e63 6f6d 2f67 6974 6875 622f 6c75 6361  .com/github/luca
+00002b80: 7342 6572 746f 6c61 2f43 6f6e 6e65 6374  sBertola/Connect
+00002b90: 2d34 2d47 796d 2d65 6e76 2d52 6569 6e66  -4-Gym-env-Reinf
+00002ba0: 6f72 6365 6d65 6e74 2d6c 6561 726e 696e  orcement-learnin
+00002bb0: 672f 626c 6f62 2f6d 6169 6e2f 6578 656d  g/blob/main/exem
+00002bc0: 706c 6573 2f54 7261 696e 5f70 706f 5f61  ples/Train_ppo_a
+00002bd0: 6e64 5f74 6573 742e 6970 796e 6229 2e0d  nd_test.ipynb)..
+00002be0: 0a0d 0a23 2320 5465 7374 696e 670d 0a0d  ...## Testing...
+00002bf0: 0a57 6520 6265 6c69 6576 6520 696e 2074  .We believe in t
+00002c00: 6865 2069 6d70 6f72 7461 6e63 6520 6f66  he importance of
+00002c10: 2074 6573 7469 6e67 2e20 5468 6174 2773   testing. That's
+00002c20: 2077 6879 2077 6520 6861 7665 2069 6e63   why we have inc
+00002c30: 6c75 6465 6420 6120 7375 6974 6520 6f66  luded a suite of
+00002c40: 2074 6573 7473 2069 6e20 7468 6520 6074   tests in the `t
+00002c50: 6573 7460 2064 6972 6563 746f 7279 2e20  est` directory. 
+00002c60: 546f 2072 756e 2074 6865 2074 6573 7473  To run the tests
+00002c70: 2c20 7369 6d70 6c79 2075 7365 2074 6865  , simply use the
+00002c80: 2063 6f6d 6d61 6e64 2060 7079 7465 7374   command `pytest
+00002c90: 602e 0d0a 0d0a 2323 2043 6f6e 7472 6962  `.....## Contrib
+00002ca0: 7574 6520 2620 5375 7070 6f72 740d 0a0d  ute & Support...
+00002cb0: 0a57 6520 7761 726d 6c79 2077 656c 636f  .We warmly welco
+00002cc0: 6d65 2063 6f6e 7472 6962 7574 696f 6e73  me contributions
+00002cd0: 2066 726f 6d20 7468 6520 636f 6d6d 756e   from the commun
+00002ce0: 6974 792e 2049 6620 796f 7520 6861 7665  ity. If you have
+00002cf0: 2061 6e20 6964 6561 2066 6f72 2061 6e20   an idea for an 
+00002d00: 696d 7072 6f76 656d 656e 7420 6f72 2066  improvement or f
+00002d10: 6f75 6e64 2061 2062 7567 2c20 646f 6e27  ound a bug, don'
+00002d20: 7420 6865 7369 7461 7465 2074 6f20 6f70  t hesitate to op
+00002d30: 656e 2061 6e20 6973 7375 6520 6f72 2073  en an issue or s
+00002d40: 7562 6d69 7420 6120 7075 6c6c 2072 6571  ubmit a pull req
+00002d50: 7565 7374 2e20 596f 7572 2069 6e70 7574  uest. Your input
+00002d60: 2069 7320 6772 6561 746c 7920 6170 7072   is greatly appr
+00002d70: 6563 6961 7465 642c 2061 6e64 206f 7572  eciated, and our
+00002d80: 2070 726f 6a65 6374 2069 7320 6d61 6465   project is made
+00002d90: 2062 6574 7465 7220 6279 2079 6f75 7220   better by your 
+00002da0: 7061 7274 6963 6970 6174 696f 6e21 0d0a  participation!..
+00002db0: 0d0a 4966 2079 6f75 2066 696e 6420 7468  ..If you find th
+00002dc0: 6973 2072 6570 6f73 6974 6f72 7920 7573  is repository us
+00002dd0: 6566 756c 2c20 706c 6561 7365 2067 6976  eful, please giv
+00002de0: 6520 6974 2061 2073 7461 7221 0d0a 0d0a  e it a star!....
+00002df0: 2323 204c 6963 656e 7365 0d0a 0d0a 5468  ## License....Th
+00002e00: 6973 2070 726f 6a65 6374 2069 7320 6c69  is project is li
+00002e10: 6365 6e73 6564 2075 6e64 6572 2074 6865  censed under the
+00002e20: 204d 4954 204c 6963 656e 7365 2e20 5365   MIT License. Se
+00002e30: 6520 7468 6520 604c 4943 454e 5345 6020  e the `LICENSE` 
+00002e40: 6669 6c65 2066 6f72 2064 6574 6169 6c73  file for details
+00002e50: 2e0d 0a                                  ...
```

### Comparing `gymnasium_connect_four-1.1.2/connect_four_gymnasium/ConnectFourEnv.py` & `gymnasium_connect_four-1.1.3/connect_four_gymnasium/ConnectFourEnv.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     MIN_INDEX_TO_PLAY = 0
     INVALID_player = 0
     INVALID_opponent = 0
 
     def change_opponent(self, opponent):
         self.opponent = opponent
 
-    def __init__(self, opponent, render_mode=None, first_player=None):
+    def __init__(self, opponent=None, render_mode=None, first_player=None):
         self.opponent = opponent  # Define the opponent
         # Define the action and observation spaces
         self.action_space = spaces.Discrete(self.COLUMNS_COUNT)
 
         # 1 is you, 2 is the opponent
         self.observation_space = spaces.Box(low=0, high=2, shape=(self.ROWS_COUNT, self.COLUMNS_COUNT), dtype=np.int32)
 
@@ -41,25 +41,26 @@
         self._board = np.zeros((self.ROWS_COUNT, self.COLUMNS_COUNT))
         self.render_for_human()
 
         if self.first_player is None:
             self.next_player_to_play = np.random.choice([1, 2])
         else:
             self.next_player_to_play = self.first_player
-        # If it's the opponent's turn, make the opponent play
-        if self.next_player_to_play == 2:
-            opponent_action = self.opponent.play(self._board)
-            result = self.play_action(opponent_action, self.next_player_to_play)
-            if result != 0:
-                print('wtf')
-                print(opponent_action)
-                exit("The opponent played an invalid action in the first move!")
-            self.next_player_to_play = 1
 
-        self.render_for_human()
+        if self.opponent is not None:
+            if self.next_player_to_play == 2:
+                opponent_action = self.opponent.play(self._board)
+                result = self.play_action(opponent_action, self.next_player_to_play)
+                if result != 0:
+                    print('wtf')
+                    print(opponent_action)
+                    exit("The opponent played an invalid action in the first move!")
+                self.next_player_to_play = 1
+
+            self.render_for_human()
 
         return self._board, {}
 
     def render_for_human(self):
         if self.render_mode == "human":
             self._render_frame()
 
@@ -78,56 +79,50 @@
         self.render_for_human()
 
         if self.check_win_around_last_move(player, last_move_row, action):
             if self.render_mode == "human":
                 print("You won!")
                 time.sleep(5)
             return 1
+        
+        if self.board_is_full():
+            return 0
 
         return 0
 
+    def board_is_full(self):
+        return np.all(self._board != 0)
+    
     def inverse_player_position(self):
         new_board = np.zeros_like(self._board)
         new_board[self._board == 1] = 2
         new_board[self._board == 2] = 1
         return new_board
 
-    def step(self, action):
-        if self.next_player_to_play == 2:
-            exit("It's not your turn!")
-
+    def switch_player(self):
+        self.next_player_to_play = 3 - self.next_player_to_play
+        
+    def step(self, action, play_opponent=True):
         action = action.item() if isinstance(action, np.ndarray) else action
 
         result = self.play_action(action, self.next_player_to_play)
-        if result == 1:
-            return self._board, 1, True, False, {}
-        elif result == -1:
-            return self._board, -1, True, False, {}
-
-        if np.all(self._board != 0):
-            return self._board, 0, True, False, {}
-
-        self.next_player_to_play = 2
-
-        # because 1 is you, 2 is the opponent
-        # you need to see the board as the opponent sees it
-        opponent_action = self.opponent.play(self.inverse_player_position())
-
-        result = self.play_action(opponent_action, self.next_player_to_play)
-
-        if result == 1:
-            return self._board, -1, True, False, {}
-        elif result == -1:
-            return self._board, 1, True, False, {}
-
-        if np.all(self._board != 0):
-            return self._board, 0, True, False, {}
-
-        self.next_player_to_play = 1
-
+        if result != 0:
+            return self._board, result, True, False, {}
+        self.switch_player()
+
+        if  play_opponent and self.opponent is not None:
+            # because 1 is you, 2 is the opponent
+            # you need to see the board as the opponent sees it
+            opponent_action = self.opponent.play(self.inverse_player_position())
+            opponent_result = self.step(opponent_action, play_opponent=False)
+            return opponent_result[0],-1* opponent_result[1], opponent_result[2], opponent_result[3], opponent_result[4]
+        elif self.opponent is None:
+            boardToReturn = self._board if self.next_player_to_play == 1 else self.inverse_player_position()
+            return boardToReturn, 0, False, False, {}
+            
         return self._board, 0, False, False, {}
 
     def drop_piece(self, action, player):
         for i in range(self.ROWS_COUNT - 1, -1, -1):
             if self._board[i, action] == 0:
                 self._board[i, action] = player
                 return i
@@ -151,16 +146,14 @@
                     if count == 4:
                         return True
                 else:
                     count = 0
 
         return False
     
-    
-
     def render(self):
         if self.render_mode == "rgb_array":
             return self._render_frame()
 
     def wait_for_render(self):
         current_time = time.time()
         time_to_wait = 1 / self.FPS
```

### Comparing `gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/AdultPlayer.py` & `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/AdultPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/AdultSmarterPlayer.py` & `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/AdultSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/ChildPlayer.py` & `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/ChildPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/ChildSmarterPlayer.py` & `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/ChildSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/ConsolePlayer.py` & `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/ConsolePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/MinMaxPlayer.py` & `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/MinMaxPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/ModelPlayer.py` & `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/ModelPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/SimulatePlayer.py` & `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/SimulatePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/TeenagerPlayer.py` & `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/TeenagerPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.2/connect_four_gymnasium/players/TeenagerSmarterPlayer.py` & `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/TeenagerSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.2/connect_four_gymnasium/tools/EloLeaderboard.py` & `gymnasium_connect_four-1.1.3/connect_four_gymnasium/tools/EloLeaderboard.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.2/gymnasium_connect_four.egg-info/SOURCES.txt` & `gymnasium_connect_four-1.1.3/gymnasium_connect_four.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -19,9 +19,10 @@
 connect_four_gymnasium/tools/EloLeaderboard.py
 connect_four_gymnasium/tools/__init__.py
 gymnasium_connect_four.egg-info/PKG-INFO
 gymnasium_connect_four.egg-info/SOURCES.txt
 gymnasium_connect_four.egg-info/dependency_links.txt
 gymnasium_connect_four.egg-info/requires.txt
 gymnasium_connect_four.egg-info/top_level.txt
+test/test_no_opponant.py
 test/test_power_4_logic.py
 test/test_ppo_env.py
```

### Comparing `gymnasium_connect_four-1.1.2/setup.py` & `gymnasium_connect_four-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='gymnasium_connect_four',
-    version='1.1.2',
+    version='1.1.3',
     description='A connect 4 (connect four) environment for OpenAI Gym and Gymnasium',
     author='Lucas Bertola',
     url='https://github.com/lucasBertola/Connect-4-env',  
     # author_email='your.email@example.com',
     packages=find_packages(),
     install_requires=[
         'pygame==2.1.3',
```

### Comparing `gymnasium_connect_four-1.1.2/test/test_power_4_logic.py` & `gymnasium_connect_four-1.1.3/test/test_power_4_logic.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.2/test/test_ppo_env.py` & `gymnasium_connect_four-1.1.3/test/test_ppo_env.py`

 * *Files identical despite different names*

