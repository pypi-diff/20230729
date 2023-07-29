# Comparing `tmp/physicsLab-1.3.0.tar.gz` & `tmp/physicsLab-1.3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\physicsLab-1.3.0.tar", last modified: Sat Jul  1 04:17:24 2023, max compression
+gzip compressed data, was "dist\physicsLab-1.3.0.1.tar", last modified: Sat Jul 29 08:55:00 2023, max compression
```

## Comparing `physicsLab-1.3.0.tar` & `physicsLab-1.3.0.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 04:17:24.000000 physicsLab-1.3.0/
--rw-rw-rw-   0        0        0     1086 2023-06-30 14:48:23.000000 physicsLab-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     4719 2023-07-01 04:17:24.000000 physicsLab-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4163 2023-06-30 14:48:23.000000 physicsLab-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab/
--rw-rw-rw-   0        0        0     2685 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/__init__.py
--rw-rw-rw-   0        0        0      966 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/_colorUtils.py
--rw-rw-rw-   0        0        0     7004 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/_fileGlobals.py
--rw-rw-rw-   0        0        0     1110 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/_tools.py
-drwxrwxrwx   0        0        0        0 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab/astrophysics/
--rw-rw-rw-   0        0        0       13 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/astrophysics/__init__.py
--rw-rw-rw-   0        0        0       62 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/astrophysics/elementsClass.py
-drwxrwxrwx   0        0        0        0 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab/electricity/
--rw-rw-rw-   0        0        0      687 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/__init__.py
--rw-rw-rw-   0        0        0      567 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementPin.py
--rw-rw-rw-   0        0        0     3277 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementXYZ.py
-drwxrwxrwx   0        0        0        0 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementsClass/
--rw-rw-rw-   0        0        0      517 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementsClass/__init__.py
--rw-rw-rw-   0        0        0     5157 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementsClass/_elementClassHead.py
--rw-rw-rw-   0        0        0     9060 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementsClass/artificialCircuit.py
--rw-rw-rw-   0        0        0     8423 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementsClass/basicCircuit.py
--rw-rw-rw-   0        0        0    17465 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementsClass/logicCircuit.py
--rw-rw-rw-   0        0        0     7106 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementsClass/otherCircuit.py
-drwxrwxrwx   0        0        0        0 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab/electricity/unionElements/
--rw-rw-rw-   0        0        0      314 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/unionElements/__init__.py
--rw-rw-rw-   0        0        0     2395 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/unionElements/_unionClassHead.py
--rw-rw-rw-   0        0        0    22879 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/unionElements/unionLogic.py
--rw-rw-rw-   0        0        0     8896 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/unionElements/unionMusic.py
--rw-rw-rw-   0        0        0      769 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/unionElements/unionPin.py
--rw-rw-rw-   0        0        0     2095 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/unionElements/wires.py
--rw-rw-rw-   0        0        0     2476 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/wire.py
-drwxrwxrwx   0        0        0        0 2023-07-01 04:17:24.000000 physicsLab-1.3.0/physicsLab/electromagnetism/
--rw-rw-rw-   0        0        0       70 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electromagnetism/__init__.py
--rw-rw-rw-   0        0        0     4483 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electromagnetism/elementsClass.py
--rw-rw-rw-   0        0        0     4607 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/element.py
--rw-rw-rw-   0        0        0     1619 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/errors.py
--rw-rw-rw-   0        0        0    11010 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/experiment.py
-drwxrwxrwx   0        0        0        0 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab.egg-info/
--rw-rw-rw-   0        0        0     4719 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 04:17:24.000000 physicsLab-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1153 2023-07-01 04:16:00.000000 physicsLab-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:55:00.000000 physicsLab-1.3.0.1/
+-rw-rw-rw-   0        0        0     6457 2023-07-29 08:55:00.000000 physicsLab-1.3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5050 2023-07-29 05:19:04.000000 physicsLab-1.3.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 08:54:59.000000 physicsLab-1.3.0.1/physicsLab/
+-rw-rw-rw-   0        0        0     2883 2023-07-29 05:19:04.000000 physicsLab-1.3.0.1/physicsLab/__init__.py
+-rw-rw-rw-   0        0        0     1145 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/_colorUtils.py
+-rw-rw-rw-   0        0        0     7085 2023-07-29 05:19:04.000000 physicsLab-1.3.0.1/physicsLab/_fileGlobals.py
+-rw-rw-rw-   0        0        0     1110 2023-07-29 05:08:11.000000 physicsLab-1.3.0.1/physicsLab/_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:55:00.000000 physicsLab-1.3.0.1/physicsLab/astrophysics/
+-rw-rw-rw-   0        0        0       13 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/astrophysics/__init__.py
+-rw-rw-rw-   0        0        0       62 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/astrophysics/elementsClass.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:55:00.000000 physicsLab-1.3.0.1/physicsLab/electricity/
+-rw-rw-rw-   0        0        0      344 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/electricity/__init__.py
+-rw-rw-rw-   0        0        0      567 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/electricity/elementPin.py
+-rw-rw-rw-   0        0        0     2770 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/electricity/elementXYZ.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:55:00.000000 physicsLab-1.3.0.1/physicsLab/electricity/elementsClass/
+-rw-rw-rw-   0        0        0      517 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/electricity/elementsClass/__init__.py
+-rw-rw-rw-   0        0        0     4913 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/electricity/elementsClass/_elementClassHead.py
+-rw-rw-rw-   0        0        0     9467 2023-07-29 07:34:25.000000 physicsLab-1.3.0.1/physicsLab/electricity/elementsClass/artificialCircuit.py
+-rw-rw-rw-   0        0        0     7996 2023-07-29 07:34:25.000000 physicsLab-1.3.0.1/physicsLab/electricity/elementsClass/basicCircuit.py
+-rw-rw-rw-   0        0        0    16304 2023-07-29 07:34:25.000000 physicsLab-1.3.0.1/physicsLab/electricity/elementsClass/logicCircuit.py
+-rw-rw-rw-   0        0        0     7000 2023-07-29 07:34:25.000000 physicsLab-1.3.0.1/physicsLab/electricity/elementsClass/otherCircuit.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:55:00.000000 physicsLab-1.3.0.1/physicsLab/electricity/unionElements/
+-rw-rw-rw-   0        0        0      278 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/electricity/unionElements/__init__.py
+-rw-rw-rw-   0        0        0     2395 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/electricity/unionElements/_unionClassHead.py
+-rw-rw-rw-   0        0        0    23377 2023-07-29 07:46:15.000000 physicsLab-1.3.0.1/physicsLab/electricity/unionElements/unionLogic.py
+-rw-rw-rw-   0        0        0     9362 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/electricity/unionElements/unionMusic.py
+-rw-rw-rw-   0        0        0      769 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/electricity/unionElements/unionPin.py
+-rw-rw-rw-   0        0        0     2095 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/electricity/unionElements/wires.py
+-rw-rw-rw-   0        0        0     2709 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/electricity/wire.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:55:00.000000 physicsLab-1.3.0.1/physicsLab/electromagnetism/
+-rw-rw-rw-   0        0        0       70 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/electromagnetism/__init__.py
+-rw-rw-rw-   0        0        0     4483 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/electromagnetism/elementsClass.py
+-rw-rw-rw-   0        0        0     4741 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/element.py
+-rw-rw-rw-   0        0        0     1625 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/errors.py
+-rw-rw-rw-   0        0        0    10980 2023-07-29 05:19:04.000000 physicsLab-1.3.0.1/physicsLab/experiment.py
+-rw-rw-rw-   0        0        0       40 2023-07-28 16:04:37.000000 physicsLab-1.3.0.1/physicsLab/union.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:55:00.000000 physicsLab-1.3.0.1/physicsLab.egg-info/
+-rw-rw-rw-   0        0        0     6457 2023-07-29 08:54:59.000000 physicsLab-1.3.0.1/physicsLab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1300 2023-07-29 08:54:59.000000 physicsLab-1.3.0.1/physicsLab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 08:54:59.000000 physicsLab-1.3.0.1/physicsLab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-29 08:54:59.000000 physicsLab-1.3.0.1/physicsLab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-29 08:54:59.000000 physicsLab-1.3.0.1/physicsLab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 08:55:00.000000 physicsLab-1.3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1207 2023-07-29 08:54:50.000000 physicsLab-1.3.0.1/setup.py
```

### Comparing `physicsLab-1.3.0/PKG-INFO` & `physicsLab-1.3.0.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,101 +1,103 @@
-Metadata-Version: 2.1
-Name: physicsLab
-Version: 1.3.0
-Summary: Doing experiments in the physics lab AR by python
-Home-page: https://gitee.com/script2000/physicsLab
-Author: Goodenough
-Author-email: 2381642961@qq.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ﻿# physicsLab 物实程序化
 
-![输入图片说明](cover.png)
+[English](./README.en.md)
+
+![输入图片说明](./cover.png)
 
 ## 介绍
-在物理实验室做实验的时候，我们可能会苦恼于元件不够整齐且无法浮空等等问题。这些都可以通过改存档来轻易实现！然而，手动改存档局限性很大，于是我封装了一些常用功能，让你用Python也能够轻易地做实验，**你甚至不需用知道存档在电脑的哪里**！
+在物理实验室做实验的时候，我们可能会苦恼于元件不够整齐，需要重复的搭建某些电路且重复地做测，或元件无法浮空等问题。这些问题都可以通过改存档来轻易解决！然而，手动改存档操作麻烦且出错率高。于是我写了```PhysicsLab```，并在其中封装了一些常用功能，让你用```Python```也能够轻易地在物实做实验，而且***你甚至不需用知道存档在电脑的哪里！***
 
 ## 安装教程
 
-1.  请确保你的电脑有[Python](https://www.python.org)与[物理实验室PC版](https://www.turtlesim.com/)（也可以联系[开发者Jone-Chen](https://gitee.com/civitasjohn)）
+1.  请确保你的电脑有[Python](https://www.python.org)（大于等于3.6）与[物理实验室PC版](https://www.turtlesim.com/)（也可以联系[开发者Jone-Chen](https://gitee.com/civitasjohn)）
 2.  在cmd或shell输入：
 ```diff
 pip install physicsLab
 ```
+3.  如果你等不及使用一些新功能的话，测试版通常在gitee可以找到
 
 ## 开发环境
 python 3.7.8, win7  
-目测对其他版本支持应该也很好
-3.6及以上应该没问题
+目测对其他版本支持应该也很好  
+python3.6及以上应该没问题
 
 ## 使用说明
+*目前```physicsLab```在```windows```上的支持最好，在```Android```上仅支持手动导入/导出存档（默认在```physicsLabSav```文件夹中）。**暂不支持其他操作系统***  
 
+下面给出一个简单的例子：
 ```Python
 from physicsLab import *
- # 打开存档  
-open_Experiment("在物实保存的存档的名字")
- # 例：open_Experiment('测逝')  
- # 也支持输入存档的文件名（也就是xxx.sav）
- # 如果你希望程序不覆盖掉存档中已有的实验状态，需要这样写  
-read_Experiment()  
- # 创建一个逻辑输入，坐标为(0, 0, 0.1)  
-Logic_Input(0, 0, 0.1)   
- # 你也可以不写坐标，默认是(0,0,0)，请注意2原件的坐标不允许重叠！  
-o = Or_Gate() # 此时o存储的是orGate的self  
- # crt_wire输入格式：  
- #    crt_wire(SourcePin, TargetPin, color = "蓝")  
-crt_Wire(o.i_up, o.i_low)  
- # 将程序中生成的原件，导线等等写入存档  
-write_Experiment()  
- # 然后用物实打开存档见证奇迹  
+
+  # 打开存档
+open_Experiment("在物实保存的本地存档的名字")
+  # 例：open_Experiment('测逝')
+  # 也支持输入存档的文件名（也就是xxx.sav）
+  # 如果你希望程序不覆盖掉存档中已有的实验状态，需要这样写
+read_Experiment()
+  # 创建一个逻辑输入，坐标为(0, 0, 0.1)
+Logic_Input(0, 0, 0.1)
+  # 你也可以不写坐标，默认是(0,0,0)，请注意2原件的坐标不允许重叠！
+o = Or_Gate()
+  # 此时o存储的是orGate的self
+  # 元件含有引脚属性，是对物实原始的引脚表示方法的封装
+  # 比如或门（Or_Gate），含有 i_up, i_low, o三个引脚属性
+  # 通过引脚属性，就可以更方便的连接导线了
+
+  # crt_Wire()函数用来连接导线，有三个参数：SourcePin, TargetPin, color
+  # SourcePin与TargetPin必须传入元件的引脚
+  # color可有可无，默认为蓝色
+crt_Wire(o.i_up, o.i_low)
+  # 将程序中生成的原件，导线等等写入存档
+write_Experiment()
+  # 然后用物实打开存档见证奇迹
 ```
-如今有了更优雅的方式：
+
+```physicsLab```还支持功能相同但更优雅的方式：
 ```python
 from physicsLab import *
 
-with experiment('测逝', read=True, elementXYZ=True):
-    Logic_Input(0, 0, 1)
+with experiment('测逝', read=True):
+    Logic_Input(0, 0, 0.1)
     o = Or_Gate()
     o.i_up - o.i_low # 连接导线
 ```
 上面两段代码产生的结果是一样的  
   
-更详细的内容请在[wiki](https://gitee.com/script2000/physicsLab/wikis/functions)中查看  
-请注意：Python采用GBK编码，而物实用的是utf-8，尽管尽量确保编码格式正确，但中文仍有可能出现问题，因此建议多用英文。  
+更详细的内容请在[Doc](./Doc)中查看  
+请注意：Python采用```GBK```编码，而物实用的是```utf-8```，在极少数情况下会出现乱码。
+此时你可以在```Python```代码的第一行添加如下注释：
+```Python
+#coding=utf-8
+
+# to do something...
+```  
+此时整个Python文件会被编码为utf-8  
+注：```physicsLab```有相关机制在你运行代码的时候自动加上该行注释，但并不总是工作。
 
 ## 优点
-1. 通过read_Experiment()，你无须把所有工作交给代码。因为用代码写并不总是意味着方便（比如连接导线）。  
-你现在可以手动连接部分导线或者添加原件，并通过保存的形式，让程序在下次也可以轻松读取。  
-这也意味着你不用一口气把控制整个电路的脚本写出来，而是每次写一部分，并把更适合代码的工作交给代码完成。  
-也就是说，写这个脚本的感觉更像在控制台上操作，非常灵活。
-2. 封装了物实里的大量原件，即使是**未解锁的原件**也可以轻易用脚本生成，甚至一些常用的电路也被封装好了！
-3. 物理实验室存档的位置有点隐蔽，但用该脚本生成实验时，你无须亲自寻找这个文件在哪里。
-4. 所有调用的库皆为Python的内置库。
-5. 最重要的一点：改存档做出来的实验往往有十分惊艳的效果！
-6. 相比于手动做实验，代码复用率更高
-7. 程序有利于实验的大型化
+1.  ```physicsLab```拥有优秀的与物实存档交互的能力，你甚至可以使用程序完成部分工作之后你再继续完成或者让程序在你已完成的实验的基础上继续完成。  
+  如此灵活的功能使得physicsLab即使是在python shell上也能出色的完成工作！
+2.  封装了物实里的大量原件，即使是***未解锁的原件***也可以轻易用脚本生成，甚至一些常用的电路也被封装好了！
+3.  物理实验室存档的位置有点隐蔽，但用该脚本生成实验时，你无须亲自寻找这个文件在哪里。
+4.  所有调用的库皆为Python的内置库，不存在第三方依赖。
+5.  相比于手动做实验，代码复用率更高，许多逻辑电路已经被封装，只需简单的一行调用即可生成。
+6.  程序有利于大型实验的创作
+7.  最重要的一点：改存档做出来的实验往往有十分惊艳的效果！
 
 ## 不足
 1. 对逻辑电路元件的支持是最好的，其余电路的部分原件还没有时间封装。但随着时间的推移，这一问题会逐渐消失。
-2. 在物理实验室连接导线只需要点击两下，但用程序连接导线需要指定什么原件的什么引脚，相对麻烦。
-3. 在物理实验室选择原件只需要点击一下，但用程序选择原件需要确定它的位置。（如果有更好的索引原件的方式，欢迎提出）
-4. 作者在接下来很长一段时间内将因为学业没有精力继续维护该仓库，但这并不代表弃坑。
+2. 在物理实验室连接导线只需要点击两下，但用程序连接导线相对麻烦一些。
+3. 在物理实验室选择原件只需要点击一下，但用程序选择原件相对麻烦一些。
+4. 作者在接下来一段时间内将因为学业难以维护该仓库，但这并不代表弃坑。
 
 ## 其他
-1. 更多内容请在[other physicsLab](https://gitee.com/script2000/temporary-warehouse/tree/master/other%20physicsLab)查看
+1. 更多内容请在 [other physicsLab](https://gitee.com/script2000/temporary-warehouse/tree/master/other%20physicsLab) 中查看
 2. github: https://github.com/GoodenoughPhysicsLab/physicsLab
 3. gitee: https://gitee.com/script2000/physicsLab
 
 ## 参与贡献
 1.  Fork 本仓库
-2.  新建分支
-3.  提交代码
-4.  新建 Pull Request
-
+2.  新建```yourName_xxx```分支
+3.  新建 Pull Request(PR)
+4.  完善文档
+5.  提issue或帮忙回答问题
```

### Comparing `physicsLab-1.3.0/physicsLab/__init__.py` & `physicsLab-1.3.0.1/physicsLab/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,32 +14,36 @@
 # 电学实验
 from physicsLab.electricity import *
 # 天体物理实验
 from physicsLab.astrophysics import *
 # 电与磁实验
 from physicsLab.electromagnetism.elementsClass import *
 # 操作元件
-from physicsLab.element import crt_Element, get_Element, del_Element, count_Elements, clear_Elements, print_Elements
+from physicsLab.element import *
 # 自定义异常类
 from physicsLab.errors import *
 # 获取存档类型与整个存档文件
-from physicsLab._fileGlobals import get_experimentType, get_Sav
+import physicsLab._fileGlobals as _fileGlobals
+from physicsLab._fileGlobals import get_Sav, get_experimentType
+# 模块化电路
+import physicsLab.electricity.unionElements.unionLogic as union
+import physicsLab.electricity.unionElements.unionMusic as music
 
 
 __all__ = [
     # _fileGlobals.py
-    "get_Sav", "get_experimentType",
+    "_fileGlobals", "get_Sav", "get_experimentType",
 
     # errors.py
     "openExperimentError", "wireColorError", "wireNotFoundError", "bitLengthError",
     "experimentExistError", "experimentTypeError", "getElementError", "crtExperimentFailError",
 
     # experiment.py
     "experiment", "open_Experiment", "crt_Experiment", "read_Experiment", "write_Experiment",
-    "rename_Experiment", "show_Experiment", "del_Experiment", "yield_Experiment",
+    "rename_Experiment", "show_Experiment", "del_Experiment", "yield_Experiment", "exist_Experiment",
 
     # element.py
     "crt_Element", "del_Element", "count_Elements", "get_Element", "clear_Elements", "print_Elements",
 
     # wire.py
     "crt_Wire", "del_Wire", "count_Wires", "clear_Wires", "print_Wires",
 
@@ -47,20 +51,21 @@
     "NE555", "Basic_Capacitor", 'Ground_Component', "Operational_Amplifier", "Relay_Component",
     "N_MOSFET", "Sinewave_Source", "Square_Source", "Triangle_Source", "Sawtooth_Source", "Pulse_Source",
     "Simple_Switch", "SPDT_Switch", "DPDT_Switch", "Push_Switch", "Battery_Source", "Student_Source",
     "Resistor", "Fuse_Component", "Slide_Rheostat", "Logic_Input", "Logic_Output", "Yes_Gate", "No_Gate",
     "Or_Gate", "And_Gate", "Nor_Gate", "Nand_Gate", "Xor_Gate", "Xnor_Gate", "Imp_Gate", "Nimp_Gate",
     "Half_Adder", "Full_Adder", "Multiplier", "D_Flipflop", "T_Flipflop", "JK_Flipflop", "Counter",
     "Random_Generator", "eight_bit_Input", "eight_bit_Display", "Electric_Fan", "Simple_Instrument",
+    "P_MOSFET",
 
     # unionElements
     "union", "music",
 
     # wires.py
     "crt_Wires", "del_Wires",
 
     # elementXYZ.py
-    "set_elementXYZ", "is_elementXYZ", "set_O", "get_OriginPosition", "get_xyzUnit",
+    "set_elementXYZ", "is_elementXYZ", "xyzTranslate", "translateXYZ", "set_O", "get_OriginPosition", "get_xyzUnit",
 
     # electromagnetism
     "Negative_Charge", "Positive_Charge"
 ]
```

### Comparing `physicsLab-1.3.0/physicsLab/_colorUtils.py` & `physicsLab-1.3.0.1/physicsLab/_colorUtils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 #coding=utf-8
 import sys
+from enum import Enum, unique
 
-BLACK = '\033[30m'
-RED = '\033[31m'
-GREEN = '\033[32m'
-YELLOW = '\033[33m'
-BLUE = '\033[34m'
-MAGENTA = '\033[35m'
-CYAN = '\033[36m'
-WHITE = '\033[37m'
-DEFAULT = '\033[39m'
+@unique
+class COLOR(Enum):
+    BLACK = '\033[30m'
+    RED = '\033[31m'
+    GREEN = '\033[32m'
+    YELLOW = '\033[33m'
+    BLUE = '\033[34m'
+    MAGENTA = '\033[35m'
+    CYAN = '\033[36m'
+    WHITE = '\033[37m'
+    DEFAULT = '\033[39m'
 
 # 打印write_Experiment的信息时是否使用彩色字
 colorSupport = True
 
 # 打印颜色字
 def printf(msg: str, color) -> None:
     global colorSupport
 
+    if not isinstance(color, COLOR):
+        raise TypeError
+
     if sys.platform == "win32":
         try:
             # https://stackoverflow.com/questions/36760127/...
             # how-to-use-the-new-support-for-ansi-escape-sequences-in-the-windows-10-console
             from ctypes import windll
             kernel32 = windll.kernel32
             kernel32.SetConsoleMode(kernel32.GetStdHandle(-11), 7)
         except Exception:  # pragma: no cover
             colorSupport = False
 
     if not isinstance(msg, str):
         raise TypeError
     if colorSupport:
-        print(f"{color}{msg}{DEFAULT}")
+        print(f"{color.value}{msg}{COLOR.DEFAULT.value}")
     else:
         print(msg)
```

### Comparing `physicsLab-1.3.0/physicsLab/_fileGlobals.py` & `physicsLab-1.3.0.1/physicsLab/_fileGlobals.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,22 +174,23 @@
 FILE_HEAD = os.path.abspath(os.sep) # 获取根目录
 if platform == "win32":
     from getpass import getuser
     FILE_HEAD = f"C:/Users/{getuser()}/AppData/LocalLow/CIVITAS/Quantum Physics/Circuit"
 elif platform == "linux": # Android
     FILE_HEAD = "/storage/emulated/0/physicsLabSav"
 
-savName: str = ""  # sav的文件名
+SavPath: str = "" # 存档的完整路径，为 f"{FILE_HEAD}/{SavName}"
+SavName: str = ""  # sav的文件名
 StatusSave: dict = {} # 存放实验元件，导线（如果是电学实验的话）
 Elements: list = []  # 装原件的_arguments
 Wires: list = []
-sav: dict = {}
+PlSav: dict = {}
 
 # 通过坐标索引元件
-elements_Position: dict = {}  # key: self._position，value: dict([self], ...)
+elements_Position: dict = {}  # key: self._position, value: List[self...]
 # 通过index（元件生成顺序）索引元件
 elements_Index: list = [] # List[self]
 
 # 初始化_fileGlobals的变量
 def fileGlobals_init(experimentType: Union[int, str]) -> None:
     if isinstance(experimentType, str):
         experimentType.strip()
@@ -200,25 +201,25 @@
                 experimentType == 3 or # 天体物理实验
                 experimentType == 4    # 电与磁实验
             )
         ) or experimentType is None
     ):
         raise TypeError
 
-    global sav, savName, StatusSave, Elements, Wires, elements_Index, elements_Position
-    savName = ""  # sav的文件名
+    global PlSav, SavName, StatusSave, Elements, Wires, elements_Index, elements_Position
+    SavName = ""  # sav的文件名
     Elements = []  # 装原件的_arguments
     Wires = []
     # 电学实验
     if experimentType == 0 or experimentType is None:
-        sav = _electricity
+        PlSav = _electricity
         StatusSave = {"SimulationSpeed": 1.0, "Elements": [], "Wires": []}
     # 电与磁实验
     elif experimentType == 4 or experimentType == "电与磁实验":
-        sav = _electromagnetism
+        PlSav = _electromagnetism
         StatusSave = {"SimulationSpeed": 1.0, "Elements": []}
 
     elements_Position = {}
     elements_Index = []
 
 # 检查实验类型
 def check_ExperimentType(targetType: int, error: bool = True):
@@ -229,15 +230,15 @@
         raise errors.experimentTypeError
     else:
         return targetType == get_experimentType()
 
 # 获取sav
 def get_Sav() -> dict:
     import copy
-    return copy.deepcopy(sav)
+    return copy.deepcopy(PlSav)
 
 # 获取实验类型
 def get_experimentType() -> int:
     try:
-        return sav["Type"]
+        return PlSav["Type"]
     except KeyError:
         raise errors.openExperimentError
```

### Comparing `physicsLab-1.3.0/physicsLab/_tools.py` & `physicsLab-1.3.0.1/physicsLab/_tools.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.3.0/physicsLab/electricity/elementPin.py` & `physicsLab-1.3.0.1/physicsLab/electricity/elementPin.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.3.0/physicsLab/electricity/elementXYZ.py` & `physicsLab-1.3.0.1/physicsLab/electricity/elementXYZ.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,24 @@
 #coding=utf-8
 # 元件坐标系
-# 一个非门的长为0.16，宽为0.08
-# 一个非门的长宽会成为元件坐标系的x, y的单位长度
-# z轴的单位长度是原坐标系的0.1
-#
-# 像二位乘法器这种元件的位置必须经过修正才能使元件整齐排列
-# x, z轴不用修正
-# y轴的修正为 +0.04
-# 坐标修正部分的代码在对应的类的文件中
-# 如big_Elements的坐标修正在logicCircuit.py
-
-# _elementClassHead里的element_Init_HEAD有部分处理元件坐标系的代码，并调用了该文件
+# 元件坐标系的单位x为一个是门的长
+# 单位y是一个是门的宽
+# 单位z为物实默认坐标系的0.1
 
 import physicsLab._tools as _tools
 import physicsLab._fileGlobals as _fileGlobals
 from typing import Callable as _Callable
 
 ### define ###
 
 _elementXYZ: bool = False
 
-# 所有元件坐标系的函数都会有的操作：
-def _dec_EelementXYZ(func: _Callable) -> _Callable:
-    def result(*args, **kwargs):
-        _fileGlobals.check_ExperimentType(0)
-        func(*args, **kwargs)
-    return result
-
 # 是否将全局设置为元件坐标系
 def set_elementXYZ(boolen: bool) -> None:
+    _fileGlobals.check_ExperimentType(0)
     if not isinstance(boolen, bool):
         raise TypeError
     global _elementXYZ
     _elementXYZ = boolen
 
 # 获取是否为元件坐标系
 def is_elementXYZ() -> bool:
@@ -48,25 +34,27 @@
 # 元件坐标系原点
 _xOrigin, _yOrigin, _zOrigin = 0, 0, 0
 
 ### end define ###
 
 # 将元件坐标系转换为物实支持的坐标系
 def xyzTranslate(x: _tools.numType, y: _tools.numType, z: _tools.numType):
+    _fileGlobals.check_ExperimentType(0)
     x *= _xUnit
     y *= _yUnit
     z *= _zUnit
     # 修改元件坐标系原点
     x += _xOrigin
     y += _yOrigin
     z += _zOrigin
     return x, y, z
 
 # 将物实支持的坐标系转换为元件坐标系
 def translateXYZ(x: _tools.numType, y: _tools.numType, z: _tools.numType, bigElement: bool = False):
+    _fileGlobals.check_ExperimentType(0)
     x /= _xUnit
     y /= _yUnit
     z /= _zUnit
     # 修改元件坐标系原点
     x -= _xOrigin
     y -= _yOrigin
     z -= _zOrigin
```

### Comparing `physicsLab-1.3.0/physicsLab/electricity/elementsClass/__init__.py` & `physicsLab-1.3.0.1/physicsLab/electricity/elementsClass/__init__.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.3.0/physicsLab/electricity/elementsClass/_elementClassHead.py` & `physicsLab-1.3.0.1/physicsLab/electricity/elementsClass/_elementClassHead.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # coding=utf-8
+from typing import *
 import physicsLab._tools as _tools
 import physicsLab.errors as errors
 import physicsLab._fileGlobals as _fileGlobals
 import physicsLab.electricity.elementPin as _elementPin
 import physicsLab.electricity.elementXYZ as _elementXYZ
 
 # electricity class's metaClass
@@ -23,39 +24,39 @@
                 isinstance(x, (float, int)) and
                 isinstance(y, (float, int)) and
                 isinstance(z, (float, int))
         ):
             raise TypeError('illegal argument')
         _fileGlobals.check_ExperimentType(0)
 
+        self.is_elementXYZ: bool = False # 元件坐标系
+        self.is_bigElement: bool = False # 2体积元件
+
         x, y, z = _tools.roundData(x, y, z)
         self._position = (x, y, z)
         # 元件坐标系
         if elementXYZ == True or (_elementXYZ.is_elementXYZ() == True and elementXYZ is None):
             x, y, z = _elementXYZ.xyzTranslate(x, y, z)
-        self.__init__(x, y, z, *args, **kwargs)
+            self.is_elementXYZ = True
+
+        self.__init__(x, y, z, elementXYZ, *args, **kwargs)
         # 若是big_Element，则修正坐标
-        if isinstance(self, is_big_element):
+        if self.is_bigElement:
             x, y, z = _elementXYZ.amend_big_Element(x, y, z)
 
         self._arguments["Identifier"] = _tools.randString(32)
         # x, z, y 物实采用欧拉坐标系
         self._arguments["Position"] = f"{x},{z},{y}"
         _fileGlobals.Elements.append(self._arguments)
 
         # 该坐标是否已存在，则存入列表
         if self._position in _fileGlobals.elements_Position.keys():
-            _fileGlobals.elements_Position[self._position]['self'].append(self)
+            _fileGlobals.elements_Position[self._position].append(self)
         else:
-            elementDict: dict = {
-                'self': [self],
-                'elementXYZ': _elementXYZ.is_elementXYZ,  # 是否为元件坐标系
-                'originPosition': tuple(_elementXYZ.get_OriginPosition())  # 坐标原点
-            }
-            _fileGlobals.elements_Position[self._position] = elementDict
+            _fileGlobals.elements_Position[self._position] = [self]
         self.set_Rotation()
         # 通过元件生成顺序来索引元件
         self._index = eletricityMeta.__index
         _fileGlobals.elements_Index.append(self)
         # 元件index索引加1
         eletricityMeta.__index += 1
         return self
@@ -99,24 +100,21 @@
         self._position = _tools.roundData(self._position[0], self._position[1], self._position[2])
         return self._position
 
     # 获取原件的坐标
     def get_Position(self) -> tuple:
         return self._position
 
-    # 获取父类的类型
-    def father_type(self) -> str:
-        return 'element'
-
     # 获取元件的index（每创建一个元件，index就加1）
     def get_Index(self) -> int:
         return self._index
 
     # 获取子类的类型（也就是ModelID）
-    def type(self) -> str:
+    @property
+    def modelID(self) -> str:
         return self._arguments['ModelID']
 
     # 打印参数
     def print_arguments(self) -> None:
         print(self._arguments)
 
 # 双引脚模拟电路原件的引脚
@@ -129,12 +127,8 @@
 
     @property
     def black(self):
         return _elementPin.element_Pin(self, 1)
 
     cls.black, cls.r = black, black
 
-    return cls
-
-# 仅用于判断是否为2体积元件
-class is_big_element:
-    pass
+    return cls
```

### Comparing `physicsLab-1.3.0/physicsLab/electricity/elementsClass/artificialCircuit.py` & `physicsLab-1.3.0.1/physicsLab/electricity/elementsClass/artificialCircuit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 #coding=utf-8
+from ..elementPin import element_Pin
 from physicsLab._tools import numType
-import physicsLab.electricity.elementPin as _elementPin
-from ._elementClassHead import electricityBase, is_big_element, two_pin_ArtificialCircuit_Pin
+from ._elementClassHead import electricityBase, two_pin_ArtificialCircuit_Pin
 
 
 # 555定时器
-class NE555(electricityBase, is_big_element):
+class NE555(electricityBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '555 Timer', 'Identifier': '', 'IsBroken': False,
                            'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '锁定': 1.0},
                            'Statistics': {'供电': 10, '放电': 0.0, '阈值': 4,
                                           '控制': 6.6666666666666666, '触发': 4,
                                           '输出': 0, '重设': 10, '接地': 0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
+        self.is_bigElement = True
 
     @property
-    def VCC(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def VCC(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def Dis(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def Dis(self) -> element_Pin:
+        return element_Pin(self, 1)
 
     @property
-    def Thr(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def Thr(self) -> element_Pin:
+        return element_Pin(self, 2)
 
     @property
-    def Ctrl(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def Ctrl(self) -> element_Pin:
+        return element_Pin(self, 3)
 
     @property
-    def Trig(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 4)
+    def Trig(self) -> element_Pin:
+        return element_Pin(self, 4)
 
     @property
-    def Out(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 5)
+    def Out(self) -> element_Pin:
+        return element_Pin(self, 5)
 
     @property
-    def Reset(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 6)
+    def Reset(self) -> element_Pin:
+        return element_Pin(self, 6)
 
     @property
-    def Ground(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 7)
+    def Ground(self) -> element_Pin:
+        return element_Pin(self, 7)
 
 # 电容
 @two_pin_ArtificialCircuit_Pin
 class Basic_Capacitor(electricityBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Basic Capacitor', 'Identifier': '',
                            'IsBroken': False, 'IsLocked': False, 'Properties': {'耐压': 16.0, '电容': 1e-06, '内阻': 5.0, '锁定': 1.0},
@@ -63,110 +64,131 @@
         self._arguments = {'ModelID': 'Ground Component', 'Identifier': '',
                            'IsBroken': False, 'IsLocked': False, 'Properties': {'锁定': 1.0},
                            'Statistics': {'电流': 0}, 'Position': '',
                            'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def i(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def i(self) -> element_Pin:
+        return element_Pin(self, 0)
 
 # 运算放大器
 class Operational_Amplifier(electricityBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Operational Amplifier', 'Identifier': '',
                            'IsBroken': False, 'IsLocked': False,
                            'Properties': {'增益系数': 100_0000.0, '最大电压': 15.0, '最小电压': -15.0, '锁定': 1.0},
                            'Statistics': {'电压-': 0, '电压+': 0, '输出电压': 0,
                                           '输出电流': 0, '输出功率': 0},
                            'Position': '',
                            'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def i_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def i_up(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def i_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def i_low(self) -> element_Pin:
+        return element_Pin(self, 1)
 
     @property
-    def o(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def o(self) -> element_Pin:
+        return element_Pin(self, 2)
 
 # 继电器
 class Relay_Component(electricityBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Relay Component', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
                            'Properties': {'开关': 0.0, '线圈电感': 0.2, '线圈电阻': 20.0,
                                           '接通电流': 0.02, '额定电流': 1.0, '锁定': 1.0}, 'Statistics': {},
                            'Position': '', 'Rotation': '',
                            'DiagramCached': False, 'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0},
                            'DiagramRotation': 0}
 
     @property
-    def l_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def l_up(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def l_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def l_low(self) -> element_Pin:
+        return element_Pin(self, 2)
 
     @property
-    def mid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def mid(self) -> element_Pin:
+        return element_Pin(self, 1)
 
     @property
-    def r_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 4)
+    def r_up(self) -> element_Pin:
+        return element_Pin(self, 4)
 
     @property
-    def r_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 5)
+    def r_low(self) -> element_Pin:
+        return element_Pin(self, 5)
 
 # n mos
 class N_MOSFET(electricityBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'N-MOSFET', 'Identifier': '', 'IsBroken': False,
                            'IsLocked': False, 'Properties': {'PNP': 1.0, '放大系数': 0.027, '阈值电压': 1.5, '最大功率': 100.0, '锁定': 1.0},
                            'Statistics': {'电压GS': 0.0, '电压': 0.0, '电流': 0.0, '功率': 0.0, '状态': 0.0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def D(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def D(self) -> element_Pin:
+        return element_Pin(self, 2)
 
     @property
-    def S(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def S(self) -> element_Pin:
+        return element_Pin(self, 1)
 
     @property
-    def G(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def G(self) -> element_Pin:
+        return element_Pin(self, 0)
+
+# p mos
+class P_MOSFET(electricityBase):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ=None):
+        self._arguments = {'ModelID': 'P-MOSFET', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
+                           'Properties': {'PNP': 1.0, '放大系数': 0.027, '阈值电压': 1.5, '最大功率': 100.0, '锁定': 1.0},
+                           'Statistics': {'电压GS': 0.0, '电压': 0.0, '电流': 0.0, '功率': 0.0, '状态': 1.0},
+                           'Position': '', 'Rotation': '', 'DiagramCached': False,
+                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
+
+    @property
+    def G(self) -> element_Pin:
+        return element_Pin(self, 0)
+
+    @property
+    def S(self) -> element_Pin:
+        return element_Pin(self, 2)
+
+    @property
+    def D(self) -> element_Pin:
+        return element_Pin(self, 1)
 
 # 波形发生器基类
 class _source_electricity(electricityBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '', 'Identifier': '',
                            'IsBroken': False, 'IsLocked': False,
                            'Properties': {'电压': 3.0, '内阻': 0.5, '频率': 20000.0, '偏移': 0.0, '占空比': 0.5, '锁定': 1.0},
                            'Statistics': {'电流': 0.0, '功率': 0.0, '电压': -3.0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def l(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def l(self) -> element_Pin:
+        return element_Pin(self, 0)
     i = l
 
     @property
-    def r(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def r(self) -> element_Pin:
+        return element_Pin(self, 1)
     o = r
 
 # 正弦波发生器
 class Sinewave_Source(_source_electricity):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Sinewave_Source, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Sinewave Source'
```

### Comparing `physicsLab-1.3.0/physicsLab/electricity/elementsClass/basicCircuit.py` & `physicsLab-1.3.0.1/physicsLab/electricity/elementsClass/basicCircuit.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #coding=utf-8
+from ..elementPin import element_Pin
 from physicsLab._tools import numType
-import physicsLab.electricity.elementPin as _elementPin
 from ._elementClassHead import electricityBase, two_pin_ArtificialCircuit_Pin
 
 # 开关基类
 
 class _switch_electricity(electricityBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {"ModelID": "", "Identifier": "", "IsBroken": False,
@@ -23,54 +23,54 @@
 # 单刀双掷开关
 class SPDT_Switch(_switch_electricity):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(SPDT_Switch, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'SPDT Switch'
 
     @property
-    def l(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def l(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def mid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def mid(self) -> element_Pin:
+        return element_Pin(self, 1)
 
     @property
-    def r(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def r(self) -> element_Pin:
+        return element_Pin(self, 2)
 
 # 双刀双掷开关
 class DPDT_Switch(_switch_electricity):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(DPDT_Switch, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'DPDT Switch'
 
     @property
-    def l_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def l_up(self) -> element_Pin:
+        return element_Pin(self, 3)
 
     @property
-    def mid_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 4)
+    def mid_up(self) -> element_Pin:
+        return element_Pin(self, 4)
 
     @property
-    def r_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 5)
+    def r_up(self) -> element_Pin:
+        return element_Pin(self, 5)
 
     @property
-    def l_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def l_low(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def mid_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def mid_low(self) -> element_Pin:
+        return element_Pin(self, 1)
 
     @property
-    def r_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def r_low(self) -> element_Pin:
+        return element_Pin(self, 2)
 
 # 按钮开关
 @two_pin_ArtificialCircuit_Pin
 class Push_Switch(electricityBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {
             'ModelID': 'Push Switch', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
@@ -102,28 +102,28 @@
                                           '功率1': 0.0, '电阻1': 0.0, '电流1': 0.0},
                            'Position': '',
                            'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0},
                            'DiagramRotation': 0}
 
     @property
-    def l(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def l(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def l_mid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def l_mid(self) -> element_Pin:
+        return element_Pin(self, 1)
 
     @property
-    def r_mid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def r_mid(self) -> element_Pin:
+        return element_Pin(self, 2)
 
     @property
-    def r(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def r(self) -> element_Pin:
+        return element_Pin(self, 3)
 
 # 电阻
 @two_pin_ArtificialCircuit_Pin
 class Resistor(electricityBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Resistor', 'Identifier': '', 'IsBroken': False,
                            'IsLocked': False,
@@ -151,21 +151,21 @@
                            'Properties': {'额定电阻': 10.0, '滑块位置': 0.0, '电阻1': 10, '电阻2': 10.0, '锁定': 1.0},
                            'Statistics': {'瞬间功率': 0.0, '瞬间电流': 0.0, '瞬间电压': 0.0, '功率': 0.0, '电压': 0.0, '电流': 0.0,
                                           '瞬间功率1': 0.0, '瞬间电流1': 0.0, '瞬间电压1': 0.0, '功率1': 0.0, '电压1': 0.0, '电流1': 0.0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def l_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def l_low(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def r_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def r_low(self) -> element_Pin:
+        return element_Pin(self, 1)
 
     @property
-    def l_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def l_up(self) -> element_Pin:
+        return element_Pin(self, 2)
 
     @property
-    def r_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def r_up(self) -> element_Pin:
+        return element_Pin(self, 3)
```

### Comparing `physicsLab-1.3.0/physicsLab/electricity/elementsClass/logicCircuit.py` & `physicsLab-1.3.0.1/physicsLab/electricity/elementsClass/logicCircuit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 #coding=utf-8
+from ..elementPin import element_Pin
 from physicsLab._tools import numType
-import physicsLab.electricity.elementPin as _elementPin
-from ._elementClassHead import electricityBase, is_big_element
+from ._elementClassHead import electricityBase
 
 class _logicBase(electricityBase):
     # 设置高电平的值
     def set_HighLeaveValue(self, num: numType) -> None:
         if not isinstance(num, (int, float)):
-            raise RuntimeError('illegal argument')
+            raise TypeError('illegal argument')
+        if num < self.get_LowLeaveValue():
+            raise TypeError("illegal range")
         self._arguments['Properties']['高电平'] = num
 
+    def get_HighLeaveValue(self) -> numType:
+        return self._arguments['Properties']['高电平']
+
     # 设置低电平的值
     def set_LowLeaveValue(self, num: numType) -> None:
         if not isinstance(num, (int, float)):
-            raise RuntimeError('illegal argument')
+            raise TypeError('illegal argument')
+        if num > self.get_HighLeaveValue():
+            raise TypeError("illegal range")
         self._arguments['Properties']['低电平'] = num
 
+    def get_LowLeaveValue(self):
+        return self._arguments['Properties']['低电平']
+
 
 # _arguments是参数的意思
 
 # 逻辑输入
 class Logic_Input(_logicBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {"ModelID": "Logic Input", "Identifier": "",
@@ -31,46 +41,46 @@
                           "DiagramRotation": 0}
 
     def set_highLevel(self) -> "Logic_Input":
         self._arguments['Properties']['开关'] = 1.0
         return self
 
     @property
-    def o(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def o(self) -> element_Pin:
+        return element_Pin(self, 0)
 
 # 逻辑输出
 class Logic_Output(_logicBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Logic Output', 'Identifier': "",
                           'IsBroken': False, 'IsLocked': False,
                           'Properties': {'状态': 0.0, '高电平': 3.0, '低电平': 0.0, '锁定': 1.0}, 'Statistics': {},
                           'Position': "",
                           'Rotation': '0,180,0', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def i(self) -> _elementPin.element_Pin:
-            return _elementPin.element_Pin(self, 0)
+    def i(self) -> element_Pin:
+            return element_Pin(self, 0)
 
 # 2引脚门电路
 class _2_pin_Gate(_logicBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '', 'Identifier': "", 'IsBroken': False,
                           'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '最大电流': 0.1, '锁定': 1.0},
                           'Statistics': {}, 'Position': "", 'Rotation': '', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def i(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def i(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def o(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def o(self) -> element_Pin:
+        return element_Pin(self, 1)
 
 # 是门
 class Yes_Gate(_2_pin_Gate):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Yes_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Yes Gate'
 
@@ -85,24 +95,24 @@
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '', 'Identifier': '', 'IsBroken': False,
                           'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '最大电流': 0.1, '锁定': 1.0},
                           'Statistics': {}, 'Position': "", 'Rotation': "", 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def i_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def i_up(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def i_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def i_low(self) -> element_Pin:
+        return element_Pin(self, 1)
 
     @property
-    def o(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def o(self) -> element_Pin:
+        return element_Pin(self, 2)
 
 # 或门
 class Or_Gate(_3_pin_Gate):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Or_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Or Gate'
 
@@ -145,318 +155,321 @@
 # 蕴含非门
 class Nimp_Gate(_3_pin_Gate):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Nimp_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Nimp Gate'
 
 # 2体积元件父类
-class _big_element(_logicBase, is_big_element):
+class _big_element(_logicBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '', 'Identifier': '', 'IsBroken': False,
                           'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '锁定': 1.0}, 'Statistics': {},
                           'Position': '', 'Rotation': '', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
+        self.is_bigElement = True
 
 # 半加器
 class Half_Adder(_big_element):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Half_Adder, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Half Adder'
 
     @property
-    def i_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def i_up(self) -> element_Pin:
+        return element_Pin(self, 2)
 
     @property
-    def i_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def i_low(self) -> element_Pin:
+        return element_Pin(self, 3)
 
     @property
-    def o_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def o_up(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def o_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def o_low(self) -> element_Pin:
+        return element_Pin(self, 1)
 
 # 全加器
 class Full_Adder(_big_element):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Full_Adder, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Full Adder'
 
     @property
-    def i_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def i_up(self) -> element_Pin:
+        return element_Pin(self, 2)
 
     @property
-    def i_mid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def i_mid(self) -> element_Pin:
+        return element_Pin(self, 3)
 
     @property
-    def i_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 4)
+    def i_low(self) -> element_Pin:
+        return element_Pin(self, 4)
 
     @property
-    def o_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def o_up(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def o_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def o_low(self) -> element_Pin:
+        return element_Pin(self, 1)
 
 # 二位乘法器
 class Multiplier(_big_element):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Multiplier, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Multiplier'
 
     @property
-    def i_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 4)
+    def i_up(self) -> element_Pin:
+        return element_Pin(self, 4)
 
     @property
-    def i_upmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 5)
+    def i_upmid(self) -> element_Pin:
+        return element_Pin(self, 5)
 
     @property
-    def i_lowmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 6)
+    def i_lowmid(self) -> element_Pin:
+        return element_Pin(self, 6)
 
     @property
-    def i_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 7)
+    def i_low(self) -> element_Pin:
+        return element_Pin(self, 7)
 
     @property
-    def o_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def o_up(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def o_upmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def o_upmid(self) -> element_Pin:
+        return element_Pin(self, 1)
 
     @property
-    def o_lowmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def o_lowmid(self) -> element_Pin:
+        return element_Pin(self, 2)
 
     @property
-    def o_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def o_low(self) -> element_Pin:
+        return element_Pin(self, 3)
 
 # D触发器
 class D_Flipflop(_big_element):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(D_Flipflop, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'D Flipflop'
 
     @property
-    def i_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def i_up(self) -> element_Pin:
+        return element_Pin(self, 2)
 
     @property
-    def i_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def i_low(self) -> element_Pin:
+        return element_Pin(self, 3)
 
     @property
-    def o_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def o_up(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def o_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def o_low(self) -> element_Pin:
+        return element_Pin(self, 1)
 
 # T触发器
 class T_Flipflop(_big_element):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(T_Flipflop, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'T Flipflop'
 
     @property
-    def i_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def i_up(self) -> element_Pin:
+        return element_Pin(self, 2)
 
     @property
-    def i_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def i_low(self) -> element_Pin:
+        return element_Pin(self, 3)
 
     @property
-    def o_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def o_up(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def o_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def o_low(self) -> element_Pin:
+        return element_Pin(self, 1)
 
 # JK触发器
 class JK_Flipflop(_big_element):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(JK_Flipflop, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'JK Flipflop'
 
     @property
-    def i_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def i_up(self) -> element_Pin:
+        return element_Pin(self, 2)
 
     @property
-    def i_mid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def i_mid(self) -> element_Pin:
+        return element_Pin(self, 3)
 
     @property
-    def i_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 4)
+    def i_low(self) -> element_Pin:
+        return element_Pin(self, 4)
 
     @property
-    def o_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def o_up(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def o_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def o_low(self) -> element_Pin:
+        return element_Pin(self, 1)
 
 # 计数器
 class Counter(_big_element):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Counter, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Counter'
 
     @property
-    def i_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 4)
+    def i_up(self) -> element_Pin:
+        return element_Pin(self, 4)
 
     @property
-    def i_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 5)
+    def i_low(self) -> element_Pin:
+        return element_Pin(self, 5)
 
     @property
-    def o_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def o_up(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def o_upmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def o_upmid(self) -> element_Pin:
+        return element_Pin(self, 1)
 
     @property
-    def o_lowmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def o_lowmid(self) -> element_Pin:
+        return element_Pin(self, 2)
 
     @property
-    def o_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def o_low(self) -> element_Pin:
+        return element_Pin(self, 3)
 
 # 随机数发生器
 class Random_Generator(_big_element):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Random_Generator, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Random Generator'
 
     @property
-    def i_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 4)
+    def i_up(self) -> element_Pin:
+        return element_Pin(self, 4)
 
     @property
-    def i_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 5)
+    def i_low(self) -> element_Pin:
+        return element_Pin(self, 5)
 
     @property
-    def o_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def o_up(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def o_upmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def o_upmid(self) -> element_Pin:
+        return element_Pin(self, 1)
 
     @property
-    def o_lowmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def o_lowmid(self) -> element_Pin:
+        return element_Pin(self, 2)
 
     @property
-    def o_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def o_low(self) -> element_Pin:
+        return element_Pin(self, 3)
 
 # 8位输入器
-class eight_bit_Input(_logicBase, is_big_element):
+class eight_bit_Input(_logicBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '8bit Input', 'Identifier': '', 'IsBroken': False,
                            'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '十进制': 0.0, '锁定': 1.0},
                            'Statistics': {}, 'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
+        self.is_bigElement = True
 
     def set_num(self, num : int):
         if 0 <= num <= 255:
             self._arguments['Properties']['十进制'] = num
         else:
             raise RuntimeError('The number range entered is incorrect')
 
     @property
-    def i_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def i_up(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def i_upmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def i_upmid(self) -> element_Pin:
+        return element_Pin(self, 1)
 
     @property
-    def i_lowmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def i_lowmid(self) -> element_Pin:
+        return element_Pin(self, 2)
 
     @property
-    def i_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def i_low(self) -> element_Pin:
+        return element_Pin(self, 3)
 
     @property
-    def o_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 4)
+    def o_up(self) -> element_Pin:
+        return element_Pin(self, 4)
 
     @property
-    def o_upmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 5)
+    def o_upmid(self) -> element_Pin:
+        return element_Pin(self, 5)
 
     @property
-    def o_lowmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 6)
+    def o_lowmid(self) -> element_Pin:
+        return element_Pin(self, 6)
 
     @property
-    def o_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 7)
+    def o_low(self) -> element_Pin:
+        return element_Pin(self, 7)
 
 # 8位显示器
-class eight_bit_Display(_logicBase, is_big_element):
+class eight_bit_Display(_logicBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '8bit Display', 'Identifier': '',
                           'IsBroken': False, 'IsLocked': False,
                           'Properties': {'高电平': 3.0, '低电平': 0.0, '状态': 0.0, '锁定': 1.0},
                           'Statistics': {'7': 0.0, '6': 0.0, '5': 0.0, '4': 0.0, '3': 0.0, '2': 0.0, '1': 0.0, '0': 0.0,
                                          '十进制': 0.0}, 'Position': '',
                           'Rotation': '', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
+        self.is_bigElement = True
 
     @property
-    def i_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def i_up(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def i_upmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def i_upmid(self) -> element_Pin:
+        return element_Pin(self, 1)
 
     @property
-    def i_lowmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def i_lowmid(self) -> element_Pin:
+        return element_Pin(self, 2)
 
     @property
-    def i_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def i_low(self) -> element_Pin:
+        return element_Pin(self, 3)
 
     @property
-    def o_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 4)
+    def o_up(self) -> element_Pin:
+        return element_Pin(self, 4)
 
     @property
-    def o_upmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 5)
+    def o_upmid(self) -> element_Pin:
+        return element_Pin(self, 5)
 
     @property
-    def o_lowmid(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 6)
+    def o_lowmid(self) -> element_Pin:
+        return element_Pin(self, 6)
 
     @property
-    def o_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 7)
+    def o_low(self) -> element_Pin:
+        return element_Pin(self, 7)
```

### Comparing `physicsLab-1.3.0/physicsLab/electricity/elementsClass/otherCircuit.py` & `physicsLab-1.3.0.1/physicsLab/electricity/elementsClass/otherCircuit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #coding=utf-8
 from typing import Union
-#from string import digits as _digits
+from ..elementPin import element_Pin
 from physicsLab._tools import numType
-import physicsLab.electricity.elementPin as _elementPin
 from ._elementClassHead import electricityBase, two_pin_ArtificialCircuit_Pin
 
 # 小电扇
 @two_pin_ArtificialCircuit_Pin
 class Electric_Fan(electricityBase):
     def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Electric Fan', 'Identifier': '',
@@ -45,20 +44,20 @@
                            'Statistics': {'瞬间功率': 0, '瞬间电流': 0, '瞬间电压': 0, '功率': 0, '电压': 0, '电流': 0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
         self.set_Tonality(pitch)
 
     @property
-    def i(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def i(self) -> element_Pin:
+        return element_Pin(self, 0)
 
     @property
-    def o(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def o(self) -> element_Pin:
+        return element_Pin(self, 1)
 
     # 设置音高
     def set_Tonality(self, *inputs) -> "Simple_Instrument":
         '''
         输入格式：
             中音区：
                 (funcInput -> 音调)
```

### Comparing `physicsLab-1.3.0/physicsLab/electricity/unionElements/_unionClassHead.py` & `physicsLab-1.3.0.1/physicsLab/electricity/unionElements/_unionClassHead.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.3.0/physicsLab/electricity/unionElements/unionLogic.py` & `physicsLab-1.3.0.1/physicsLab/electricity/unionElements/unionLogic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #coding=utf-8
 # 模块化电路
 import typing as _typing
-import physicsLab._tools as _tools
+from physicsLab._tools import numType
 import physicsLab.errors as _errors
 import physicsLab.electricity as electricity
 import physicsLab.electricity.elementsClass as _elementsClass
 from physicsLab.electricity.unionElements.unionPin import union_Pin
 import physicsLab.electricity.unionElements._unionClassHead as _unionClassHead
 
 # unionHeading与fold的判断的代码
@@ -31,36 +31,35 @@
 # 用metaClass检查是否有self._elements
 class _union_LogicMeta(type):
     pass
 
 # 模块化电路逻辑电路基类
 class Union_LogicBase(_unionClassHead.UnionBase):
     # 设置高电平的值
-    def set_HighLeaveValue(self, num: _tools.numType) -> "Union_LogicBase":
+    def set_HighLeaveValue(self, num: numType) -> "Union_LogicBase":
         for element in self._elements:
             element.set_HighLeaveValue(num)
         return self
 
-    def set_LowLeaveValue(self, num: _tools.numType) -> "Union_LogicBase":
+    def set_LowLeaveValue(self, num: numType) -> "Union_LogicBase":
         for element in self._elements:
             element.set_LowLeaveValue(num)
         return self
 
 # 任意引脚加法电路
 class Sum(Union_LogicBase):
-    def __init__(
-            self,
-            x: _tools.numType = 0,
-            y: _tools.numType = 0,
-            z: _tools.numType = 0,
-            bitLength: int = None,
-            elementXYZ: bool = None,  # x, y, z是否为元件坐标系
-            unionHeading: bool = False,  # False: 生成的元件为竖直方向，否则为横方向
-            fold: bool = False,  # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
-            foldMaxNum: int = 4  # 达到foldMaxNum个元件数时即在z轴自动折叠
+    def __init__(self,
+                 x: numType = 0,
+                 y: numType = 0,
+                 z: numType = 0,
+                 bitLength: int = 4,
+                 elementXYZ: bool = None,  # x, y, z是否为元件坐标系
+                 unionHeading: bool = False,  # False: 生成的元件为竖直方向，否则为横方向
+                 fold: bool = False,  # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
+                 foldMaxNum: int = 4  # 达到foldMaxNum个元件数时即在z轴自动折叠
     ) -> None:
         def link_union_Sum(elements: _typing.List[_elementsClass.Full_Adder]) -> None:
             for i in range(elements.__len__() - 1):
                 elements[i].o_low - elements[i + 1].i_low
 
         def func1():
             zcor = z
@@ -89,16 +88,14 @@
         def func4():
             for increase in range(bitLength):
                 self._elements.append(
                     electricity.Full_Adder(x, y + increase * 2, z, True)
                 )
 
         # main
-        # if bitLength < 2:
-        #     raise errors.bitLengthError
 
         x, y, z = _unionClassHead.union_Init_HEAD(
             x, y, z,
             bitLength,
             elementXYZ,
             unionHeading,
             fold,
@@ -129,26 +126,41 @@
     def data_Output(self) -> union_Pin:
         return union_Pin(
             self,
             *(element.o_up for element in self._elements),
             self._elements[-1].o_low
         )
 
+# 只读非门，若没有则创建一个只读非门，若已存在则不会创建新的元件
+class Const_NoGate:
+    __singleton_NoGate: electricity.No_Gate = None
+    def __init__(self,
+                 x: numType = 0,
+                 y: numType = 0,
+                 z: numType = 0,
+                 elementXYZ: bool = None
+    ) -> None:
+        if Const_NoGate.__singleton_NoGate is None:
+            Const_NoGate.__singleton_NoGate = electricity.No_Gate(x, y, z, elementXYZ)
+
+    @property
+    def o(self):
+        return Const_NoGate.__singleton_NoGate.o
+
 # 任意引脚减法电路
 class Sub(Union_LogicBase):
-    def __init__(
-            self,
-            x: _tools.numType = 0,
-            y: _tools.numType = 0,
-            z: _tools.numType = 0,
-            bitLength: int = None,
-            elementXYZ: bool = None,  # x, y, z是否为元件坐标系
-            unionHeading: bool = False,  # False: 生成的元件为竖直方向，否则为横方向
-            fold: bool = False,  # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
-            foldMaxNum: int = 4  # 达到foldMaxNum个元件数时即在z轴自动折叠
+    def __init__(self,
+                 x: numType = 0,
+                 y: numType = 0,
+                 z: numType = 0,
+                 bitLength: int = 4, # 减法器的最大计算比特数
+                 elementXYZ: bool = None,  # x, y, z是否为元件坐标系
+                 unionHeading: bool = False,  # False: 生成的元件为竖直方向，否则为横方向
+                 fold: bool = False,  # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
+                 foldMaxNum: int = 4  # 达到foldMaxNum个元件数时即在z轴自动折叠
     ) -> None:
         def link_union_Sub(
                 fullAdders: _typing.List[_elementsClass.Full_Adder],
                 noGates: _typing.List[_elementsClass.No_Gate]
         ) -> None:
             self._elements[0].o - fullAdders[0].i_low
             for i in range(fullAdders.__len__() - 1):
@@ -204,15 +216,15 @@
             elementXYZ,
             unionHeading,
             fold,
             foldMaxNum
         )
 
         self._elements: _typing.List[_typing.Union[_elementsClass.Full_Adder, _elementsClass.No_Gate]] = [
-            _elementsClass.No_Gate(x, y, z, True)
+            Const_NoGate(x, y, z, True)
         ]
 
         self._noGates: _typing.List[_elementsClass.No_Gate] = []
         self._fullAdders: _typing.List[_elementsClass.Full_Adder] = []
 
         _unionHeading_fold(
             func1, func2, func3, func4, unionHeading, fold
@@ -242,15 +254,15 @@
             self,
             *(e.o_up for e in self._fullAdders),
             self._fullAdders[-1].o_low
         )
 
 # 2-4译码器
 class _two_four_Decoder:
-    def __init__(self, x : _tools.numType = 0, y : _tools.numType = 0, z : _tools.numType = 0):
+    def __init__(self, x : numType = 0, y : numType = 0, z : numType = 0):
         if not (isinstance(x, (int, float)) and isinstance(y, (int, float)) and isinstance(z, (int, float))):
             raise RuntimeError('illegal argument')
         self.x = x
         self.y = y
         self.z = z
         obj1 = electricity.Nor_Gate(x, y, z)
         obj2 = electricity.Nimp_Gate(x, y + 0.1, z)
@@ -265,15 +277,15 @@
 
     @property
     def i_low(self):
         return electricity.element_Pin(electricity.get_Element(self.x, self.y + 0.3, self.z), 1)
 
 # 4-16译码器
 class _four_sixteen_Decoder:
-    def __init__(self, x : _tools.numType = 0, y : _tools.numType = 0, z : _tools.numType = 0):
+    def __init__(self, x : numType = 0, y : numType = 0, z : numType = 0):
         if not (isinstance(x, (int, float)) and isinstance(y, (int, float)) and isinstance(z, (int, float))):
             raise RuntimeError('illegal argument')
         self.x = x
         self.y = y
         self.z = z
         obj1 = electricity.Nor_Gate(x, y, z); obj2 = electricity.Nimp_Gate(x, y + 0.1, z)
         obj3 = electricity.Nimp_Gate(x, y + 0.2, z); obj4 = electricity.And_Gate(x, y + 0.3, z)
@@ -387,24 +399,23 @@
 
     @property
     def o15(self):
         return electricity.get_Element(self.x + 0.3, self.y + 0.25, self.z).o_upmid
 
 # 多个逻辑输入（暂不支持m * n矩阵排列元件的方式）
 class Inputs(Union_LogicBase):
-    def __init__(
-            self,
-            x: _tools.numType = 0,
-            y: _tools.numType = 0,
-            z: _tools.numType = 0,
-            bitLength: int = None,
-            elementXYZ: bool = None,  # x, y, z是否为元件坐标系
-            unionHeading: bool = False,  # False: 生成的元件为竖直方向，否则为横方向
-            fold: bool = False,  # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
-            foldMaxNum: int = 8  # 达到foldMaxNum个元件数时即在z轴自动折叠
+    def __init__(self,
+                 x: numType = 0,
+                 y: numType = 0,
+                 z: numType = 0,
+                 bitLength: int = 4,
+                 elementXYZ: bool = None,  # x, y, z是否为元件坐标系
+                 unionHeading: bool = False,  # False: 生成的元件为竖直方向，否则为横方向
+                 fold: bool = False,  # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
+                 foldMaxNum: int = 8  # 达到foldMaxNum个元件数时即在z轴自动折叠
     ) -> None:
         # 搭配_unionHeading_fold使用
         def func1():
             zcor = z
             for i in range(bitLength):
                 self._elements.append(
                     electricity.Logic_Input(x + i % foldMaxNum, y, zcor, True)
@@ -453,24 +464,23 @@
         return union_Pin(
             self,
             *(element.o for element in self._elements)
         )
 
 # 多个逻辑输入（暂不支持m * n矩阵排列元件的方式）
 class Outputs(Union_LogicBase):
-    def __init__(
-            self,
-            x: _tools.numType = 0,
-            y: _tools.numType = 0,
-            z: _tools.numType = 0,
-            bitLength: int = None,
-            elementXYZ: bool = None,  # x, y, z是否为元件坐标系
-            unionHeading: bool = False,  # False: 生成的元件为竖直方向，否则为横方向
-            fold: bool = False,  # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
-            foldMaxNum: int = 8  # 达到foldMaxNum个元件数时即在z轴自动折叠
+    def __init__(self,
+                 x: numType = 0,
+                 y: numType = 0,
+                 z: numType = 0,
+                 bitLength: int = 4,
+                 elementXYZ: bool = None,  # x, y, z是否为元件坐标系
+                 unionHeading: bool = False,  # False: 生成的元件为竖直方向，否则为横方向
+                 fold: bool = False,  # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
+                 foldMaxNum: int = 8  # 达到foldMaxNum个元件数时即在z轴自动折叠
     ) -> None:
         # 搭配_unionHeading_fold使用
         def func1():
             zcor = z
             for i in range(bitLength):
                 self._elements.append(
                     electricity.Logic_Output(x + i % foldMaxNum, y, zcor, True)
@@ -519,25 +529,24 @@
         return union_Pin(
             self,
             *(element.i for element in self._elements)
         )
 
 # D触发器流水灯
 class D_WaterLamp(Union_LogicBase):
-    def __init__(
-            self,
-            x: _tools.numType = 0,
-            y: _tools.numType = 0,
-            z: _tools.numType = 0,
-            bitLength: int = None,
-            elementXYZ: bool = None, # x, y, z是否为元件坐标系
-            unionHeading: bool = False, # False: 生成的元件为竖直方向，否则为横方向
-            fold: bool = False, # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
-            foldMaxNum: int = 4, # 达到foldMaxNum个元件数时即在z轴自动折叠
-            is_loop: bool = True # 是否使流水灯循环
+    def __init__(self,
+                 x: numType = 0,
+                 y: numType = 0,
+                 z: numType = 0,
+                 bitLength: int = 4,
+                 elementXYZ: bool = None, # x, y, z是否为元件坐标系
+                 unionHeading: bool = False, # False: 生成的元件为竖直方向，否则为横方向
+                 fold: bool = False, # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
+                 foldMaxNum: int = 4, # 达到foldMaxNum个元件数时即在z轴自动折叠
+                 is_loop: bool = True # 是否使流水灯循环
     ) -> None:
         # D触流水灯导线连接方式
         def link_D_Flipflop(elements: _typing.List[_elementsClass.D_Flipflop]) -> None:
             # 连接clk
             for i in range(len(elements) - 1):
                 elements[i].i_low - elements[i + 1].i_low
             # 连接数据传输导线
```

### Comparing `physicsLab-1.3.0/physicsLab/electricity/unionElements/unionMusic.py` & `physicsLab-1.3.0.1/physicsLab/electricity/unionElements/unionMusic.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,27 @@
 import physicsLab.electricity.elementsClass as _elementsClass
 from physicsLab.electricity.unionElements.unionLogic import D_WaterLamp
 import physicsLab.electricity.unionElements._unionClassHead as _unionClassHead
 
 noteType = List[Union[None, "Note"]] # 音符类型
 chordType = Union[Tuple["Note"], List["Note"]] # 和弦类型
 
+# midi类，用于提供physicsLab与midi文件之间的桥梁
+class Midi:
+    def __init__(self) -> None:
+        pass
+
+    # 播放midi类存储的信息
+    def sound(self):
+        pass
+
+    # 转换为physicsLab的piece类
+    def translate_to_piece(self) -> "Piece":
+        pass
+
 # 音符类
 class Note:
     def __init__(self,
                  time: int, # 在音轨中播放的时间
                  playTime: int = 1,  # 音符发出声音的时长 暂时不支持相关机制
                  instrument: Union[int, str] = 0, # 演奏的乐器，暂时只支持传入数字
                  pitch: Union[int, str] = 60, # 音高/音调
@@ -108,20 +121,16 @@
 
 # 乐曲类
 class Piece:
     def __init__(self, *tracks: Track):
         if not all(isinstance(a_track, Track) for a_track in tracks):
             raise TypeError
 
-        self.notes: noteType = []
-
-        if len(tracks) > 1:
-            raise RuntimeError("Sorry, multiple tracks are not supported for the moment")
-
-        self.notes: noteType = tracks[0].notes
+        self.tracks: Track = tracks
+        self.mergeTrack()
 
     def __len__(self):
         return len(self.notes)
 
     def __getitem__(self, item):
         return self.notes[item]
 
@@ -129,23 +138,31 @@
     def __iter__(self):
         self.__iter = iter(self.notes)
         return self.__iter
 
     def __next__(self):
         for a_note in self.__iter:
             yield a_note
+    
+    # 将多个音轨合并为一个音轨（方便物实生成）
+    def mergeTrack(self) -> "Piece":
+        if len(self.tracks) > 1:
+            raise RuntimeError("Sorry, multiple tracks are not supported for the moment")
+        
+        self.notes = self.tracks[0].notes
+        
+        return self
 
     # 在物实生成对应的电路
     def play(self, x:numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None) -> None:
         Player(self, x, y, z, elementXYZ)
 
-    # 在电脑上自动播放改midi
-    def sound(self) -> "Piece":
+    # 转换为Midi类
+    def translate_to_midi(self) -> Midi:
         pass
-        return self
 
 # 将piece的数据生成为物实的电路
 class Player(_unionClassHead.UnionBase):
     def __init__(self,
                  musicArray: Union[Piece, List[Piece], Tuple[Piece]],
                  x: numType = 0, y: numType = 0, z: numType = 0,
                  elementXYZ = None
@@ -210,24 +227,24 @@
                         yesGate.o - ins.o
                     else:
                         ins.o - xPlayer.data_Output[xcor]
                     # 连接y轴的d触的导线
                     ins.i - yPlayer.neg_data_Output[ycor // 2]
 
                 i = 1
-                exit = None
+                exit_sign = None
                 while True:
                     if a_note_item + i >= len(musicArray):
-                        exit = True
+                        exit_sign = True
                         break
                     if musicArray[a_note_item+i] is None:
                         i += 1
                     else:
                         break
-                if exit:
+                if exit_sign:
                     break
                 next_note = musicArray[a_note_item+i]
                 if a_note_item+1 < len(musicArray) and next_note is not None and next_note.time != 0:
                     zcor = 0
                 else:
                     zcor += 1
                     continue
```

### Comparing `physicsLab-1.3.0/physicsLab/electricity/unionElements/unionPin.py` & `physicsLab-1.3.0.1/physicsLab/electricity/unionElements/unionPin.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.3.0/physicsLab/electricity/unionElements/wires.py` & `physicsLab-1.3.0.1/physicsLab/electricity/unionElements/wires.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.3.0/physicsLab/electricity/wire.py` & `physicsLab-1.3.0.1/physicsLab/electricity/wire.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,21 @@
 # 检查函数参数是否是导线
 def _check_typeWire(func):
     def result(SourcePin: "_elementPin.element_Pin", TargetPin: "_elementPin.element_Pin", color: str = '蓝') -> None:
         if (
                 isinstance(SourcePin, _elementPin.element_Pin) and
                 isinstance(TargetPin, _elementPin.element_Pin)
         ):
-            if (color not in ["黑", "蓝", "红", "绿", "黄"]):
+            # 将英文的color转换为中文
+            if color in ("black", "blue", "red", "green", "yellow"):
+                color = {"black": "黑", "blue": "蓝", "red": "红", "green": "绿", "yellow": "黄"}[color]
+
+            if (color not in ("黑", "蓝", "红", "绿", "黄")):
                 raise errors.wireColorError
+
             _fileGlobals.check_ExperimentType(0)
 
             func(SourcePin, TargetPin, color)
 
     return result
 
 # 新版连接导线
```

### Comparing `physicsLab-1.3.0/physicsLab/electromagnetism/elementsClass.py` & `physicsLab-1.3.0.1/physicsLab/electromagnetism/elementsClass.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.3.0/physicsLab/element.py` & `physicsLab-1.3.0.1/physicsLab/element.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     # 通过坐标索引元件
     def position_Element(x: _tools.numType, y: _tools.numType, z: _tools.numType):
         if not (isinstance(x, (int, float)) and isinstance(y, (int, float)) and isinstance(z, (int, float))):
             raise TypeError('illegal argument')
         position = _tools.roundData(x, y, z)
         if position not in _fileGlobals.elements_Position.keys():
             raise RuntimeError(f"{position} do not exist")
-        result: list = _fileGlobals.elements_Position[position]['self']
+        result: list = _fileGlobals.elements_Position[position]
         return result[0] if len(result) == 1 else result
     # 通过index（元件生成顺序）索引元件
     def index_Element(index: int):
         if 0 < index <= len(_fileGlobals.elements_Index):
             return _fileGlobals.elements_Index[index - 1]
         else:
             raise errors.getElementError
@@ -77,45 +77,55 @@
         else:
             raise TypeError
     else:
         raise TypeError
 
 # 删除原件
 def del_Element(self) -> None:
-#    _fileGlobals.check_ExperimentType(0)
+#    self是物实三大实验支持的所有元件
+
+    if not isinstance(self, _elementsClass.electricityBase):
+        raise TypeError
+
+    identifier = self._arguments["Identifier"]
+
+    # 删除Elements中的引用
+    for element in _fileGlobals.Elements:
+        if element["Identifier"] == identifier:
+            _fileGlobals.Elements.remove(element)
+            break
 
-    try:
-        identifier = self._arguments['Identifier']
-        if isinstance(self, _elementsClass.electricityBase):
-            for element in _fileGlobals.Elements:
-                if identifier == element['Identifier']:
-                    # 删除原件
-                    _fileGlobals.Elements.remove(element)
-                    # 删除导线
-                    i = 0
-                    while i < _fileGlobals.Wires.__len__():
-                        wire = _fileGlobals.Wires[i]
-                        if wire['Source'] == identifier or wire['Target'] == identifier:
-                            _fileGlobals.Wires.pop(i)
-                        else:
-                            i += 1
-                    return
-    except:
-        raise RuntimeError('Unable to delete a nonexistent element')
+
+    i = 0
+    while i < _fileGlobals.Wires.__len__():
+        wire = _fileGlobals.Wires[i]
+        if wire['Source'] == identifier or wire['Target'] == identifier:
+            _fileGlobals.Wires.pop(i)
+        else:
+            i += 1
+
+    # 删除elements_Position中的引用
+    for elements in _fileGlobals.elements_Position.values():
+        if self in elements:
+            elements.remove(self)
+            break
+
+    # 删除elements_Index中的引用
+    for element in _fileGlobals.elements_Index:
+        if element is self:
+            _fileGlobals.elements_Index.remove(self)
+            break
 
 # 原件的数量
 def count_Elements() -> int:
     return len(_fileGlobals.Elements)
 
 # 清空原件
 def clear_Elements() -> None:
     _fileGlobals.Elements.clear()
     _fileGlobals.Wires.clear()
     _fileGlobals.elements_Index.clear()
     _fileGlobals.elements_Position.clear()
 
+# 打印物实存档格式的所有元件
 def print_Elements() -> None:
-    print(_fileGlobals.Elements)
-
-# 元件基类
-class elementBase:
-    pass
+    print(_fileGlobals.Elements)
```

### Comparing `physicsLab-1.3.0/physicsLab/errors.py` & `physicsLab-1.3.0.1/physicsLab/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #coding=utf-8
 # 用于存放自定义错误类
 # 由于有时在package外需要异常处理，故不为文件私有变量
 import physicsLab._colorUtils as _colorUtils
 
 def warning(msg: str) -> None:
-    _colorUtils.printf("Warning: " + msg, _colorUtils.YELLOW)
+    _colorUtils.printf("Warning: " + msg, _colorUtils.COLOR.YELLOW)
 
 # 打开实验异常
 class openExperimentError(Exception):
     def __str__(self):
         return "open a experiment but find nothing(must open a experiment)."
 
 # 导线颜色类型异常
```

### Comparing `physicsLab-1.3.0/physicsLab/experiment.py` & `physicsLab-1.3.0.1/physicsLab/experiment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #coding=utf-8
 import os
 import json
 from typing import Union
 
 import physicsLab._tools as _tools
 import physicsLab.errors as errors
+import physicsLab.electricity as electricity
 import physicsLab._colorUtils as _colorUtils
 import physicsLab._fileGlobals as _fileGlobals
 
 # 实验（存档）类，主要与'with'关键字搭配使用
 class experiment:
     def __init__(
             self,
@@ -57,29 +58,14 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self.write:
             write_Experiment()
         if self.delete:
             del_Experiment()
 
-# 输入sav文件名并读取（旧函数，不建议使用）
-def old_open_Experiment(file: str) -> None:
-    file = file.strip()
-    if (not file.endswith('.sav')):
-        raise RuntimeError("The input parameters are incorrect")
-
-    _fileGlobals.savName = f"{_fileGlobals.FILE_HEAD}/{file}"
-    with open(_fileGlobals.savName, encoding="UTF-8") as f:
-        InternalName = (json.loads(f.read().replace('\n', '')))["InternalName"]
-        _fileGlobals.sav["InternalName"] = InternalName
-        try: # 当Summary为None时触发TypeError
-            _fileGlobals.sav["Summary"]["Subject"] = InternalName
-        except TypeError:
-            pass
-
 # 将import了physicsLab的文件的第一行添加上 #coding=utf-8
 def _utf8_coding(func):
     def result(*args, **kwargs) -> None:
         try: # 在cmd或者shell上无法执行该功能
             import sys
             s = ''
             with open(sys.argv[0], encoding='utf-8') as f:
@@ -92,97 +78,109 @@
                         f.write(f'#coding=utf-8\n{s}')
         except FileNotFoundError:
             # 在cmd或IDLE上运行时会关闭打印彩字功能
             _colorUtils.printColor = False
         func(*args, **kwargs)
     return result
 
+# 检测实验是否存在，输入为存档名，若存在则返回存档对应的文件名，若不存在则返回None
+def exist_Experiment(savName: str) -> Union[str, None]:
+    savs = _tools.getAllSav()
+    for aSav in savs:
+        with open(f"{_fileGlobals.FILE_HEAD}/{aSav}", encoding='utf-8') as f:
+            try:
+                f = json.loads(f.read().replace('\n', ''))
+            except json.decoder.JSONDecodeError: # 文件不是物实存档
+                continue
+            else:
+                if f["InternalName"]== savName:
+                    return aSav
+    return None
+
 # 打开一个指定的sav文件（支持输入本地实验的名字或sav文件名）
 @_utf8_coding
 def open_Experiment(fileName : str) -> None:
+    # 输入sav（存档）的文件名并读取部分实验内容
+    def _open_Experiment(file: str) -> None:        
+        _fileGlobals.SavPath = f"{_fileGlobals.FILE_HEAD}/{file}"
+        with open(_fileGlobals.SavPath, encoding="UTF-8") as f:
+            f = json.loads(f.read().replace('\n', ''))
+            # 初始化package全局变量
+            _fileGlobals.fileGlobals_init(f["Type"])
+
+            _fileGlobals.PlSav["InternalName"] = f["InternalName"]
+            try: # 当Summary为None时触发TypeError
+                _fileGlobals.PlSav["Summary"]["Subject"] = f["InternalName"]
+            except TypeError:
+                pass
+
     fileName = fileName.strip()
     if fileName.endswith('.sav'):
-        old_open_Experiment(fileName)
-    else:
-        savs = _tools.getAllSav()
-        for aSav in savs:
-            with open(f"{_fileGlobals.FILE_HEAD}/{aSav}", encoding='utf-8') as f:
-                try:
-                    f = json.loads(f.read().replace('\n', ''))
-                except json.decoder.JSONDecodeError: # 文件不是物实存档
-                    pass
-                else:
-                    if f["InternalName"]== fileName:
-                        # 初始化package全局变量
-                        _fileGlobals.fileGlobals_init(f["Type"])
+        _open_Experiment(fileName)
+        return
 
-                        old_open_Experiment(aSav)
-                        return
+    _fileGlobals.SavName = exist_Experiment(fileName)
+    if _fileGlobals.SavName is None:
         raise errors.openExperimentError(f'No such experiment "{fileName}"')
 
-# 创建存档
+    _open_Experiment(_fileGlobals.SavName)
+
+# 创建存档，输入为存档名
 @_utf8_coding
-def crt_Experiment(fileName : str, experimentType: str = None) -> None:
+def crt_Experiment(savName : str, experimentType: str = None) -> None:
     _fileGlobals.fileGlobals_init(experimentType)
-    savs = _tools.getAllSav()
-    for aSav in savs:
-        with open(f"{_fileGlobals.FILE_HEAD}/{aSav}", 'r', encoding='utf-8') as f:
-            try:
-                f = json.loads(f.read().replace('\n', ''))
-            except json.decoder.JSONDecodeError:
-                continue
-            else:
-                if f['InternalName'] == fileName:
-                    raise errors.crtExperimentFailError
+    if exist_Experiment(savName) is not None:
+        raise errors.crtExperimentFailError
+    
     # 创建存档
-    if not isinstance(fileName, str):
-        fileName = str(fileName)
-    _fileGlobals.savName = _tools.randString(34)
-    _fileGlobals.savName = f'{_fileGlobals.FILE_HEAD}/{_fileGlobals.savName}.sav'
-    rename_Experiment(fileName)
+    if not isinstance(savName, str):
+        savName = str(savName)
+    _fileGlobals.SavName = _tools.randString(34)
+    _fileGlobals.SavPath = f'{_fileGlobals.FILE_HEAD}/{_fileGlobals.SavName}.sav'
+    rename_Experiment(savName)
 
 # 将编译完成的json写入sav
 def write_Experiment() -> None:
     def _format_StatusSave(stringJson: str) -> str:
         stringJson = stringJson.replace('{\\\"ModelID', '\n      {\\\"ModelID') # format element json
         stringJson = stringJson.replace('DiagramRotation\\\": 0}]', 'DiagramRotation\\\": 0}\n    ]') # format end element json
         stringJson = stringJson.replace('{\\\"Source', '\n      {\\\"Source')
         stringJson = stringJson.replace("色导线\\\"}]}", "色导线\\\"}\n    ]}")
         return stringJson
 
     _fileGlobals.StatusSave["Elements"] = _fileGlobals.Elements
     _fileGlobals.StatusSave["Wires"] = _fileGlobals.Wires
-    _fileGlobals.sav["Experiment"]["StatusSave"] = \
+    _fileGlobals.PlSav["Experiment"]["StatusSave"] = \
         json.dumps(_fileGlobals.StatusSave, ensure_ascii=False, separators=(',', ': '))
-    with open(_fileGlobals.savName, "w", encoding="UTF-8") as f:
+    with open(_fileGlobals.SavPath, "w", encoding="UTF-8") as f:
         f.write(
-                _format_StatusSave(json.dumps(_fileGlobals.sav, indent=2, ensure_ascii=False, separators=(',', ': ')))
+                _format_StatusSave(json.dumps(_fileGlobals.PlSav, indent=2, ensure_ascii=False, separators=(',', ': ')))
         )
     # 编译成功，打印信息
     if _fileGlobals.get_experimentType() == 0:
         _colorUtils.printf(
             f"Successfully compiled! {_fileGlobals.Elements.__len__()} elements, {_fileGlobals.Wires.__len__()} wires.",
-            _colorUtils.GREEN
+            _colorUtils.COLOR.GREEN
         )
     else:
         _colorUtils.printf(
             f"Successfully compiled! {_fileGlobals.Elements.__len__()} elements.",
-            _colorUtils.GREEN
+            _colorUtils.COLOR.GREEN
         )
 
 # 读取sav文件已有的原件与导线
 def read_Experiment() -> None:
-    with open(_fileGlobals.savName, encoding='UTF-8') as f:
+    with open(_fileGlobals.SavPath, encoding='UTF-8') as f:
         readmem = json.loads(f.read().replace('\n', ''))
         # 元件
         _local_Elements = json.loads(readmem["Experiment"]["StatusSave"])["Elements"]
         # 导线
         _fileGlobals.Wires = json.loads(readmem['Experiment']['StatusSave'])['Wires']
         # 实验介绍
-        _fileGlobals.sav['Summary']["Description"] = readmem["Summary"]["Description"]
+        _fileGlobals.PlSav['Summary']["Description"] = readmem["Summary"]["Description"]
 
         for element in _local_Elements:
             # 坐标标准化（消除浮点误差）
             sign1 = element['Position'].find(',')
             sign2 = element['Position'].find(',', sign1 + 1)
             num1 = _tools.roundData(float(element['Position'][:sign1:]))
             num2 = _tools.roundData(float(element['Position'][sign1 + 1: sign2:]))
@@ -203,18 +201,18 @@
             sign2 = element['Rotation'].find(',', sign1 + 1)
             x = float(element['Rotation'][:sign1:])
             z = float(element['Rotation'][sign1 + 1: sign2:])
             y = float(element['Rotation'][sign2 + 1::])
             obj.set_Rotation(x, y, z)
             obj._arguments['Identifier'] = element['Identifier']
             # 如果obj是逻辑输入
-            if obj.type() == 'Logic Input' and element['Properties'].get('开关') == 1:
+            if isinstance(obj, electricity.Logic_Input) and element['Properties'].get('开关') == 1:
                 obj.set_highLevel()
             # 如果obj是8位输入器
-            elif obj.type() == '8bit Input':
+            elif isinstance(obj, electricity.eight_bit_Input):
                 obj._arguments['Statistics'] = element['Statistics']
                 obj._arguments['Properties']['十进制'] = element['Properties']['十进制']
 
 # 重命名sav
 def rename_Experiment(name: str) -> None:
     # 检查是否重名
     savs = [i for i in os.walk(_fileGlobals.FILE_HEAD)][0]
@@ -227,42 +225,42 @@
             except:
                 pass
             else:
                 if f['InternalName'] == name:
                     raise RuntimeError('Duplicate name archives are forbidden')
     # 重命名存档
     name = str(name)
-    _fileGlobals.sav["Summary"]["Subject"] = name
-    _fileGlobals.sav["InternalName"] = name
+    _fileGlobals.PlSav["Summary"]["Subject"] = name
+    _fileGlobals.PlSav["InternalName"] = name
 
 # 打开一个存档的窗口
 def show_Experiment() -> None:
-    os.popen(f'notepad {_fileGlobals.savName}')
-os_Experiment = show_Experiment
+    # os.system() 在文件夹有空格的时候会出现错误
+    os.popen(f'notepad {_fileGlobals.SavPath}')
 
 # 删除存档
 def del_Experiment() -> None:
-    os.remove(_fileGlobals.savName)
+    os.remove(_fileGlobals.SavPath)
     try: # 用存档生成的实验无图片，因此可能删除失败
-        os.remove(_fileGlobals.savName.replace('.sav', '.jpg'))
+        os.remove(_fileGlobals.SavPath.replace('.sav', '.jpg'))
     except FileNotFoundError:
         pass
-    _colorUtils.printf("Successfully delete experiment!", _colorUtils.BLUE)
+    _colorUtils.printf("Successfully delete experiment!", _colorUtils.COLOR.BLUE)
 
 # 发布实验
 def yield_Experiment(title: str = None, introduction: str = None) -> None:
     # 发布实验时输入实验介绍
     def introduce_Experiment(introduction: str) -> None:
         if introduction is not None:
-            _fileGlobals.sav['Summary']['Description'] = introduction.split('\n')
+            _fileGlobals.PlSav['Summary']['Description'] = introduction.split('\n')
 
     # 发布实验时输入实验标题
     def title_Experiment(title: str) -> None:
         if title is not None:
-            _fileGlobals.sav['Summary']['Subject'] = title
+            _fileGlobals.PlSav['Summary']['Subject'] = title
 
     if (not isinstance(title, str) and title is not None) or \
             (not isinstance(introduction, str) and introduction is not None):
         raise TypeError
 
     introduce_Experiment(introduction)
     title_Experiment(title)
```

### Comparing `physicsLab-1.3.0/physicsLab.egg-info/SOURCES.txt` & `physicsLab-1.3.0.1/physicsLab.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-LICENSE
 README.md
 setup.py
 physicsLab/__init__.py
 physicsLab/_colorUtils.py
 physicsLab/_fileGlobals.py
 physicsLab/_tools.py
 physicsLab/element.py
 physicsLab/errors.py
 physicsLab/experiment.py
+physicsLab/union.py
 physicsLab.egg-info/PKG-INFO
 physicsLab.egg-info/SOURCES.txt
 physicsLab.egg-info/dependency_links.txt
+physicsLab.egg-info/requires.txt
 physicsLab.egg-info/top_level.txt
 physicsLab/astrophysics/__init__.py
 physicsLab/astrophysics/elementsClass.py
 physicsLab/electricity/__init__.py
 physicsLab/electricity/elementPin.py
 physicsLab/electricity/elementXYZ.py
 physicsLab/electricity/wire.py
```

### Comparing `physicsLab-1.3.0/setup.py` & `physicsLab-1.3.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("D:/program_physicsLab/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="physicsLab",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.3.0",  # 包版本号，便于维护版本
+    version="1.3.0.1",  # 包版本号，便于维护版本
+    license="MIT",
     author="Goodenough",  # 作者，可以写自己的姓名
     author_email="2381642961@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="Doing experiments in the physics lab AR by python",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://gitee.com/script2000/physicsLab",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
+    install_requires=["mido"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: Chinese (Simplified)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',  # 对python的最低版本要求
```

