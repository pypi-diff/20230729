# Comparing `tmp/rannet-0.2.1.tar.gz` & `tmp/rannet-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rannet-0.2.1.tar", last modified: Sun Jul  9 12:52:53 2023, max compression
+gzip compressed data, was "rannet-0.3.0.tar", last modified: Sat Jul 29 10:08:11 2023, max compression
```

## Comparing `rannet-0.2.1.tar` & `rannet-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-07-09 12:52:53.699108 rannet-0.2.1/
--rw-r--r--   0 seanlee    (501) staff       (20)     1060 2023-07-03 12:41:23.000000 rannet-0.2.1/LICENSE
--rw-r--r--   0 seanlee    (501) staff       (20)     5581 2023-07-09 12:52:53.699308 rannet-0.2.1/PKG-INFO
--rw-r--r--   0 seanlee    (501) staff       (20)     4873 2023-07-09 12:48:49.000000 rannet-0.2.1/README.md
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-07-09 12:52:53.690859 rannet-0.2.1/rannet/
--rw-r--r--   0 seanlee    (501) staff       (20)      323 2023-07-09 12:52:22.000000 rannet-0.2.1/rannet/__init__.py
--rw-r--r--   0 seanlee    (501) staff       (20)     9124 2023-07-03 12:41:23.000000 rannet-0.2.1/rannet/dataloader.py
--rw-r--r--   0 seanlee    (501) staff       (20)    24517 2023-07-03 12:41:23.000000 rannet-0.2.1/rannet/layers.py
--rw-r--r--   0 seanlee    (501) staff       (20)    17145 2023-07-03 12:41:23.000000 rannet-0.2.1/rannet/optimizer.py
--rw-r--r--   0 seanlee    (501) staff       (20)    14505 2023-07-03 12:41:23.000000 rannet-0.2.1/rannet/pretrain.py
--rw-r--r--   0 seanlee    (501) staff       (20)    29604 2023-07-09 09:11:20.000000 rannet-0.2.1/rannet/ran.py
--rw-r--r--   0 seanlee    (501) staff       (20)    25469 2023-07-09 12:48:49.000000 rannet-0.2.1/rannet/rannet.py
--rw-r--r--   0 seanlee    (501) staff       (20)     6394 2023-07-03 12:41:23.000000 rannet-0.2.1/rannet/tokenizer.py
--rw-r--r--   0 seanlee    (501) staff       (20)     1808 2023-07-03 12:41:23.000000 rannet-0.2.1/rannet/utils.py
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-07-09 12:52:53.698403 rannet-0.2.1/rannet.egg-info/
--rw-r--r--   0 seanlee    (501) staff       (20)     5581 2023-07-09 12:52:53.000000 rannet-0.2.1/rannet.egg-info/PKG-INFO
--rw-r--r--   0 seanlee    (501) staff       (20)      377 2023-07-09 12:52:53.000000 rannet-0.2.1/rannet.egg-info/SOURCES.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        1 2023-07-09 12:52:53.000000 rannet-0.2.1/rannet.egg-info/dependency_links.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        1 2023-07-09 10:02:43.000000 rannet-0.2.1/rannet.egg-info/not-zip-safe
--rw-r--r--   0 seanlee    (501) staff       (20)       31 2023-07-09 12:52:53.000000 rannet-0.2.1/rannet.egg-info/requires.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        7 2023-07-09 12:52:53.000000 rannet-0.2.1/rannet.egg-info/top_level.txt
--rw-r--r--   0 seanlee    (501) staff       (20)      163 2023-07-09 12:52:53.700006 rannet-0.2.1/setup.cfg
--rw-r--r--   0 seanlee    (501) staff       (20)     1395 2023-07-09 12:52:22.000000 rannet-0.2.1/setup.py
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-07-29 10:08:11.856186 rannet-0.3.0/
+-rw-r--r--   0 seanlee    (501) staff       (20)     1060 2023-07-03 12:41:23.000000 rannet-0.3.0/LICENSE
+-rw-r--r--   0 seanlee    (501) staff       (20)     7164 2023-07-29 10:08:11.856512 rannet-0.3.0/PKG-INFO
+-rw-r--r--   0 seanlee    (501) staff       (20)     6456 2023-07-29 08:38:13.000000 rannet-0.3.0/README.md
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-07-29 10:08:11.851580 rannet-0.3.0/rannet/
+-rw-r--r--   0 seanlee    (501) staff       (20)      323 2023-07-29 10:07:41.000000 rannet-0.3.0/rannet/__init__.py
+-rw-r--r--   0 seanlee    (501) staff       (20)     9124 2023-07-03 12:41:23.000000 rannet-0.3.0/rannet/dataloader.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    24517 2023-07-03 12:41:23.000000 rannet-0.3.0/rannet/layers.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    17145 2023-07-03 12:41:23.000000 rannet-0.3.0/rannet/optimizer.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    12395 2023-07-29 08:37:53.000000 rannet-0.3.0/rannet/pretrain.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    29110 2023-07-29 08:37:53.000000 rannet-0.3.0/rannet/ran.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    25064 2023-07-29 08:37:53.000000 rannet-0.3.0/rannet/rannet.py
+-rw-r--r--   0 seanlee    (501) staff       (20)     6394 2023-07-03 12:41:23.000000 rannet-0.3.0/rannet/tokenizer.py
+-rw-r--r--   0 seanlee    (501) staff       (20)     1808 2023-07-03 12:41:23.000000 rannet-0.3.0/rannet/utils.py
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-07-29 10:08:11.855590 rannet-0.3.0/rannet.egg-info/
+-rw-r--r--   0 seanlee    (501) staff       (20)     7164 2023-07-29 10:08:11.000000 rannet-0.3.0/rannet.egg-info/PKG-INFO
+-rw-r--r--   0 seanlee    (501) staff       (20)      377 2023-07-29 10:08:11.000000 rannet-0.3.0/rannet.egg-info/SOURCES.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        1 2023-07-29 10:08:11.000000 rannet-0.3.0/rannet.egg-info/dependency_links.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        1 2023-07-09 10:02:43.000000 rannet-0.3.0/rannet.egg-info/not-zip-safe
+-rw-r--r--   0 seanlee    (501) staff       (20)       31 2023-07-29 10:08:11.000000 rannet-0.3.0/rannet.egg-info/requires.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        7 2023-07-29 10:08:11.000000 rannet-0.3.0/rannet.egg-info/top_level.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)      168 2023-07-29 10:08:11.857475 rannet-0.3.0/setup.cfg
+-rw-r--r--   0 seanlee    (501) staff       (20)     1395 2023-07-29 10:07:41.000000 rannet-0.3.0/setup.py
```

### Comparing `rannet-0.2.1/LICENSE` & `rannet-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rannet-0.2.1/PKG-INFO` & `rannet-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rannet
-Version: 0.2.1
+Version: 0.3.0
 Summary: Recurrent Attention Networks
 Author: sean lee
 Author-email: xmlee97@gmail.com
 Keywords: rannet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -37,14 +37,18 @@
    </a>
    <a href="https://arxiv.org/abs/2306.06843">
       <img src="https://img.shields.io/badge/Arxiv-2306.06843-yellow.svg?style=flat-square" alt="https://arxiv.org/abs/2306.06843" />
    </a>
 </h4>
 
 
+<p align="center">
+<img src='assets/framework.png' alt='The framework of RAN' style='width: 520px;' />
+</p>
+
 
 # ⬇️ Installation
 
 *stable*
 
 ```bash
 python -m pip install -U rannet
@@ -58,19 +62,38 @@
 
 *environment*
 - ⭐ tensorflow>2.0,<=2.10 🤗 `export TF_KERAS=1`
 - tensorflow>=1.14,<2.0 🤗 Keras==2.3.1
 
 ## 🏛️ Pretrained Models
 
+### V3 Models
+
+🎯 compatible with: `rannet>0.2.1`
+
+| Lang | Google Drive | Baidu NetDrive |
+|------|--------------|----------------|
+| EN   |    [base](https://drive.google.com/file/d/1CO1M_57U506_3mDBqtGo-5b1XXNpONln/view?usp=sharing)          |        [base](https://pan.baidu.com/s/1Z2wODILsIeZ3i8_9GEpl2g)\[code: udts\]        |
+
+Chinese Models are still pretraining...
+
+
+### V2 Models
+
+🎯 compatible with: `rannet<=0.2.1`
+
 | Lang | Google Drive | Baidu NetDrive |
 |------|--------------|----------------|
 | EN   |    [base](https://drive.google.com/file/d/1mRabw0Hy9T5_EWbZshD6Uk-bvauNzG9R/view?usp=sharing)          |        [base](https://pan.baidu.com/s/18uhAkY46aIcy4ncwzXp5mA)\[code: djkj\]        |
 | CN   |   [base](https://drive.google.com/file/d/1_gmrulSU-ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing)  \| [small](https://drive.google.com/file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/view?usp=sharing)         |        [base](https://pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\[code: e47w\]  \| [small](https://pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\[code: mdmg\]        |
 
+### V1 Models
+
+V1 models are not open.
+
 
 # 🚀 Quick Tour
 
 ## 🈶 w/ pretrained models
 
 *Extract semantic feature*
 
@@ -152,24 +175,66 @@
           apply_seq2seq_mask=False,
           apply_memory_review=True,
           dropout_rate=0.0,
           cell_initializer_type='zero')
 output, cell = ran(X)
 ```
 
+## w/ history
+
+```python
+import numpy as np
+from rannet import RanNet, RanNetWordPieceTokenizer
+
+
+vocab_path = 'pretrained/vocab.txt'
+ckpt_path = 'pretrained/model.ckpt'
+config_path = 'pretrained/config.json'
+tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True)
+
+rannet, rannet_model = RanNet.load_rannet(
+    config_path=config_path,
+    checkpoint_path=ckpt_path,
+    return_sequences=False,
+    apply_cell_transform=False,
+    return_history=True,  # return history
+    cell_pooling='mean',
+    with_cell=True,  # with cell input
+)
+rannet_model.summary()
+
+text = 'sentence 1'
+tok = tokenizer.encode(text)
+init_cell = np.zeros((1, 768))  # 768 is embedding size
+vec, history = rannet_model.predict([np.array([tok.ids]), init_cell])
+
+text2 = 'sentence 2'
+tok = tokenizer.encode(text2)
+vec2, history = rannet_model.predict([np.array([tok.ids]), history])  # input history of sentence 1
+```
+
 # 📚 Citation
 
 If you use our code in your research, please cite our work:
 
 ```
-@inproceedings{li-etal-2023-ran,
+@inproceedings{li-etal-2023-recurrent,
     title = "Recurrent Attention Networks for Long-text Modeling",
-    author = "Li, Xianming and Li, Zongxi and Luo, Xiaotian and Xie, Haoran and Lee, Xing and Zhao, Yingbin and Wang, Fu Lee and Li, Qing",
+    author = "Li, Xianming  and
+      Li, Zongxi  and
+      Luo, Xiaotian  and
+      Xie, Haoran  and
+      Lee, Xing  and
+      Zhao, Yingbin  and
+      Wang, Fu Lee  and
+      Li, Qing",
     booktitle = "Findings of the Association for Computational Linguistics: ACL 2023",
+    month = jul,
     year = "2023",
-    publisher = "Association for Computational Linguistics"
+    publisher = "Association for Computational Linguistics",
+    pages = "3006--3019",
 }
 ```
 
 # 📬 Contact
 
 Please contact us at 1) for code problems, create a GitHub issue; 2) for paper problems, email xmlee97@gmail.com
```

#### html2text {}

```diff
@@ -1,46 +1,52 @@
-Metadata-Version: 2.1 Name: rannet Version: 0.2.1 Summary: Recurrent Attention
+Metadata-Version: 2.1 Name: rannet Version: 0.3.0 Summary: Recurrent Attention
 Networks Author: sean lee Author-email: xmlee97@gmail.com Keywords: rannet
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
 License-File: LICENSE
                 ****** RAN: Recurrent Attention Network ******
   *** ð¢ This project is still in the works in order to make long document
                              modeling easier. ***
  *** [RAN_is_released_under_the_MIT_license.] [PyPI_version] [PyPI_Downloads]
      [http://makeapullrequest.com] [https://arxiv.org/abs/2306.06843] ***
+                            [The framework of RAN]
 # â¬ï¸ Installation *stable* ```bash python -m pip install -U rannet ```
 *latest* ```bash python -m pip install git+https://github.com/4AI/RAN.git ```
 *environment* - â­ tensorflow>2.0,<=2.10 ð¤ `export TF_KERAS=1` -
-tensorflow>=1.14,<2.0 ð¤ Keras==2.3.1 ## ðï¸ Pretrained Models | Lang |
-Google Drive | Baidu NetDrive | |------|--------------|----------------| | EN |
-[base](https://drive.google.com/file/d/1mRabw0Hy9T5_EWbZshD6Uk-bvauNzG9R/
-view?usp=sharing) | [base](https://pan.baidu.com/s/18uhAkY46aIcy4ncwzXp5mA)\
-[code: djkj\] | | CN | [base](https://drive.google.com/file/d/1_gmrulSU-
-ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing) \| [small](https://drive.google.com/
-file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/view?usp=sharing) | [base](https://
-pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\[code: e47w\] \| [small](https://
-pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\[code: mdmg\] | # ð Quick Tour ##
-ð¶ w/ pretrained models *Extract semantic feature* set
-`return_sequences=False` to extract semantic feature. ```python import numpy as
-np from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
-'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
-'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
-lowercase=True) rannet, rannet_model = RanNet.load_rannet
-( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False,
-apply_cell_transform=False, cell_pooling='mean' ) text = 'input text' tok =
-tokenizer.encode(text) vec = rannet_model.predict(np.array([tok.ids])) ``` *For
-the classification task* ```python from rannet import RanNet,
-RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt' ckpt_path =
-'pretrained/model.ckpt' config_path = 'pretrained/config.json' tokenizer =
+tensorflow>=1.14,<2.0 ð¤ Keras==2.3.1 ## ðï¸ Pretrained Models ### V3
+Models ð¯ compatible with: `rannet>0.2.1` | Lang | Google Drive | Baidu
+NetDrive | |------|--------------|----------------| | EN | [base](https://
+drive.google.com/file/d/1CO1M_57U506_3mDBqtGo-5b1XXNpONln/view?usp=sharing) |
+[base](https://pan.baidu.com/s/1Z2wODILsIeZ3i8_9GEpl2g)\[code: udts\] | Chinese
+Models are still pretraining... ### V2 Models ð¯ compatible with:
+`rannet<=0.2.1` | Lang | Google Drive | Baidu NetDrive | |------|--------------
+|----------------| | EN | [base](https://drive.google.com/file/d/
+1mRabw0Hy9T5_EWbZshD6Uk-bvauNzG9R/view?usp=sharing) | [base](https://
+pan.baidu.com/s/18uhAkY46aIcy4ncwzXp5mA)\[code: djkj\] | | CN | [base](https://
+drive.google.com/file/d/1_gmrulSU-ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing) \|
+[small](https://drive.google.com/file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/
+view?usp=sharing) | [base](https://pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\
+[code: e47w\] \| [small](https://pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\
+[code: mdmg\] | ### V1 Models V1 models are not open. # ð Quick Tour ## ð¶
+w/ pretrained models *Extract semantic feature* set `return_sequences=False` to
+extract semantic feature. ```python import numpy as np from rannet import
+RanNet, RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt' ckpt_path
+= 'pretrained/model.ckpt' config_path = 'pretrained/config.json' tokenizer =
+RanNetWordPieceTokenizer(vocab_path, lowercase=True) rannet, rannet_model =
+RanNet.load_rannet( config_path=config_path, checkpoint_path=ckpt_path,
+return_sequences=False, apply_cell_transform=False, cell_pooling='mean' ) text
+= 'input text' tok = tokenizer.encode(text) vec = rannet_model.predict(np.array
+([tok.ids])) ``` *For the classification task* ```python from rannet import
+RanNet, RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt' ckpt_path
+= 'pretrained/model.ckpt' config_path = 'pretrained/config.json' tokenizer =
 RanNetWordPieceTokenizer(vocab_path, lowercase=True) rannet, rannet_model =
 RanNet.load_rannet( config_path=config_path, checkpoint_path=ckpt_path,
 return_sequences=False) output = rannet_model.output # (B, D) output =
 L.Dropout(0.1)(output) output = L.Dense(2, activation='softmax')(output) model
 = keras.models.Model(rannet_model.input, output) model.summary() ``` *For the
 sequence task* ```python from rannet import RanNet, RanNetWordPieceTokenizer
 vocab_path = 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt'
@@ -49,16 +55,28 @@
 ( config_path=config_path, checkpoint_path=ckpt_path, return_cell=False) output
 = rannet_model.output # (B, L, D) rannet_model.summary() ``` ## ð w/
 o pretrained models Embed the `RAN` (a Keras layer) into your network.
 ```python from rannet import RAN ran = RAN(head_num=8, head_size=256,
 window_size=256, min_window_size=16, activation='swish',
 kernel_initializer='glorot_normal', apply_lm_mask=False,
 apply_seq2seq_mask=False, apply_memory_review=True, dropout_rate=0.0,
-cell_initializer_type='zero') output, cell = ran(X) ``` # ð Citation If you
-use our code in your research, please cite our work: ``` @inproceedings{li-
-etal-2023-ran, title = "Recurrent Attention Networks for Long-text Modeling",
-author = "Li, Xianming and Li, Zongxi and Luo, Xiaotian and Xie, Haoran and
-Lee, Xing and Zhao, Yingbin and Wang, Fu Lee and Li, Qing", booktitle =
-"Findings of the Association for Computational Linguistics: ACL 2023", year =
-"2023", publisher = "Association for Computational Linguistics" } ``` # ð¬
-Contact Please contact us at 1) for code problems, create a GitHub issue; 2)
-for paper problems, email xmlee97@gmail.com
+cell_initializer_type='zero') output, cell = ran(X) ``` ## w/ history ```python
+import numpy as np from rannet import RanNet, RanNetWordPieceTokenizer
+vocab_path = 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt'
+config_path = 'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer
+(vocab_path, lowercase=True) rannet, rannet_model = RanNet.load_rannet
+( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False,
+apply_cell_transform=False, return_history=True, # return history
+cell_pooling='mean', with_cell=True, # with cell input ) rannet_model.summary()
+text = 'sentence 1' tok = tokenizer.encode(text) init_cell = np.zeros((1, 768))
+# 768 is embedding size vec, history = rannet_model.predict([np.array(
+[tok.ids]), init_cell]) text2 = 'sentence 2' tok = tokenizer.encode(text2)
+vec2, history = rannet_model.predict([np.array([tok.ids]), history]) # input
+history of sentence 1 ``` # ð Citation If you use our code in your research,
+please cite our work: ``` @inproceedings{li-etal-2023-recurrent, title =
+"Recurrent Attention Networks for Long-text Modeling", author = "Li, Xianming
+and Li, Zongxi and Luo, Xiaotian and Xie, Haoran and Lee, Xing and Zhao,
+Yingbin and Wang, Fu Lee and Li, Qing", booktitle = "Findings of the
+Association for Computational Linguistics: ACL 2023", month = jul, year =
+"2023", publisher = "Association for Computational Linguistics", pages = "3006-
+-3019", } ``` # ð¬ Contact Please contact us at 1) for code problems, create
+a GitHub issue; 2) for paper problems, email xmlee97@gmail.com
```

### Comparing `rannet-0.2.1/README.md` & `rannet-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,18 @@
    </a>
    <a href="https://arxiv.org/abs/2306.06843">
       <img src="https://img.shields.io/badge/Arxiv-2306.06843-yellow.svg?style=flat-square" alt="https://arxiv.org/abs/2306.06843" />
    </a>
 </h4>
 
 
+<p align="center">
+<img src='assets/framework.png' alt='The framework of RAN' style='width: 520px;' />
+</p>
+
 
 # ⬇️ Installation
 
 *stable*
 
 ```bash
 python -m pip install -U rannet
@@ -38,19 +42,38 @@
 
 *environment*
 - ⭐ tensorflow>2.0,<=2.10 🤗 `export TF_KERAS=1`
 - tensorflow>=1.14,<2.0 🤗 Keras==2.3.1
 
 ## 🏛️ Pretrained Models
 
+### V3 Models
+
+🎯 compatible with: `rannet>0.2.1`
+
+| Lang | Google Drive | Baidu NetDrive |
+|------|--------------|----------------|
+| EN   |    [base](https://drive.google.com/file/d/1CO1M_57U506_3mDBqtGo-5b1XXNpONln/view?usp=sharing)          |        [base](https://pan.baidu.com/s/1Z2wODILsIeZ3i8_9GEpl2g)\[code: udts\]        |
+
+Chinese Models are still pretraining...
+
+
+### V2 Models
+
+🎯 compatible with: `rannet<=0.2.1`
+
 | Lang | Google Drive | Baidu NetDrive |
 |------|--------------|----------------|
 | EN   |    [base](https://drive.google.com/file/d/1mRabw0Hy9T5_EWbZshD6Uk-bvauNzG9R/view?usp=sharing)          |        [base](https://pan.baidu.com/s/18uhAkY46aIcy4ncwzXp5mA)\[code: djkj\]        |
 | CN   |   [base](https://drive.google.com/file/d/1_gmrulSU-ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing)  \| [small](https://drive.google.com/file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/view?usp=sharing)         |        [base](https://pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\[code: e47w\]  \| [small](https://pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\[code: mdmg\]        |
 
+### V1 Models
+
+V1 models are not open.
+
 
 # 🚀 Quick Tour
 
 ## 🈶 w/ pretrained models
 
 *Extract semantic feature*
 
@@ -132,24 +155,66 @@
           apply_seq2seq_mask=False,
           apply_memory_review=True,
           dropout_rate=0.0,
           cell_initializer_type='zero')
 output, cell = ran(X)
 ```
 
+## w/ history
+
+```python
+import numpy as np
+from rannet import RanNet, RanNetWordPieceTokenizer
+
+
+vocab_path = 'pretrained/vocab.txt'
+ckpt_path = 'pretrained/model.ckpt'
+config_path = 'pretrained/config.json'
+tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True)
+
+rannet, rannet_model = RanNet.load_rannet(
+    config_path=config_path,
+    checkpoint_path=ckpt_path,
+    return_sequences=False,
+    apply_cell_transform=False,
+    return_history=True,  # return history
+    cell_pooling='mean',
+    with_cell=True,  # with cell input
+)
+rannet_model.summary()
+
+text = 'sentence 1'
+tok = tokenizer.encode(text)
+init_cell = np.zeros((1, 768))  # 768 is embedding size
+vec, history = rannet_model.predict([np.array([tok.ids]), init_cell])
+
+text2 = 'sentence 2'
+tok = tokenizer.encode(text2)
+vec2, history = rannet_model.predict([np.array([tok.ids]), history])  # input history of sentence 1
+```
+
 # 📚 Citation
 
 If you use our code in your research, please cite our work:
 
 ```
-@inproceedings{li-etal-2023-ran,
+@inproceedings{li-etal-2023-recurrent,
     title = "Recurrent Attention Networks for Long-text Modeling",
-    author = "Li, Xianming and Li, Zongxi and Luo, Xiaotian and Xie, Haoran and Lee, Xing and Zhao, Yingbin and Wang, Fu Lee and Li, Qing",
+    author = "Li, Xianming  and
+      Li, Zongxi  and
+      Luo, Xiaotian  and
+      Xie, Haoran  and
+      Lee, Xing  and
+      Zhao, Yingbin  and
+      Wang, Fu Lee  and
+      Li, Qing",
     booktitle = "Findings of the Association for Computational Linguistics: ACL 2023",
+    month = jul,
     year = "2023",
-    publisher = "Association for Computational Linguistics"
+    publisher = "Association for Computational Linguistics",
+    pages = "3006--3019",
 }
 ```
 
 # 📬 Contact
 
 Please contact us at 1) for code problems, create a GitHub issue; 2) for paper problems, email xmlee97@gmail.com
```

#### html2text {}

```diff
@@ -1,36 +1,42 @@
                 ****** RAN: Recurrent Attention Network ******
   *** ð¢ This project is still in the works in order to make long document
                              modeling easier. ***
  *** [RAN_is_released_under_the_MIT_license.] [PyPI_version] [PyPI_Downloads]
      [http://makeapullrequest.com] [https://arxiv.org/abs/2306.06843] ***
+                            [The framework of RAN]
 # â¬ï¸ Installation *stable* ```bash python -m pip install -U rannet ```
 *latest* ```bash python -m pip install git+https://github.com/4AI/RAN.git ```
 *environment* - â­ tensorflow>2.0,<=2.10 ð¤ `export TF_KERAS=1` -
-tensorflow>=1.14,<2.0 ð¤ Keras==2.3.1 ## ðï¸ Pretrained Models | Lang |
-Google Drive | Baidu NetDrive | |------|--------------|----------------| | EN |
-[base](https://drive.google.com/file/d/1mRabw0Hy9T5_EWbZshD6Uk-bvauNzG9R/
-view?usp=sharing) | [base](https://pan.baidu.com/s/18uhAkY46aIcy4ncwzXp5mA)\
-[code: djkj\] | | CN | [base](https://drive.google.com/file/d/1_gmrulSU-
-ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing) \| [small](https://drive.google.com/
-file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/view?usp=sharing) | [base](https://
-pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\[code: e47w\] \| [small](https://
-pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\[code: mdmg\] | # ð Quick Tour ##
-ð¶ w/ pretrained models *Extract semantic feature* set
-`return_sequences=False` to extract semantic feature. ```python import numpy as
-np from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
-'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
-'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
-lowercase=True) rannet, rannet_model = RanNet.load_rannet
-( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False,
-apply_cell_transform=False, cell_pooling='mean' ) text = 'input text' tok =
-tokenizer.encode(text) vec = rannet_model.predict(np.array([tok.ids])) ``` *For
-the classification task* ```python from rannet import RanNet,
-RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt' ckpt_path =
-'pretrained/model.ckpt' config_path = 'pretrained/config.json' tokenizer =
+tensorflow>=1.14,<2.0 ð¤ Keras==2.3.1 ## ðï¸ Pretrained Models ### V3
+Models ð¯ compatible with: `rannet>0.2.1` | Lang | Google Drive | Baidu
+NetDrive | |------|--------------|----------------| | EN | [base](https://
+drive.google.com/file/d/1CO1M_57U506_3mDBqtGo-5b1XXNpONln/view?usp=sharing) |
+[base](https://pan.baidu.com/s/1Z2wODILsIeZ3i8_9GEpl2g)\[code: udts\] | Chinese
+Models are still pretraining... ### V2 Models ð¯ compatible with:
+`rannet<=0.2.1` | Lang | Google Drive | Baidu NetDrive | |------|--------------
+|----------------| | EN | [base](https://drive.google.com/file/d/
+1mRabw0Hy9T5_EWbZshD6Uk-bvauNzG9R/view?usp=sharing) | [base](https://
+pan.baidu.com/s/18uhAkY46aIcy4ncwzXp5mA)\[code: djkj\] | | CN | [base](https://
+drive.google.com/file/d/1_gmrulSU-ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing) \|
+[small](https://drive.google.com/file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/
+view?usp=sharing) | [base](https://pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\
+[code: e47w\] \| [small](https://pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\
+[code: mdmg\] | ### V1 Models V1 models are not open. # ð Quick Tour ## ð¶
+w/ pretrained models *Extract semantic feature* set `return_sequences=False` to
+extract semantic feature. ```python import numpy as np from rannet import
+RanNet, RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt' ckpt_path
+= 'pretrained/model.ckpt' config_path = 'pretrained/config.json' tokenizer =
+RanNetWordPieceTokenizer(vocab_path, lowercase=True) rannet, rannet_model =
+RanNet.load_rannet( config_path=config_path, checkpoint_path=ckpt_path,
+return_sequences=False, apply_cell_transform=False, cell_pooling='mean' ) text
+= 'input text' tok = tokenizer.encode(text) vec = rannet_model.predict(np.array
+([tok.ids])) ``` *For the classification task* ```python from rannet import
+RanNet, RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt' ckpt_path
+= 'pretrained/model.ckpt' config_path = 'pretrained/config.json' tokenizer =
 RanNetWordPieceTokenizer(vocab_path, lowercase=True) rannet, rannet_model =
 RanNet.load_rannet( config_path=config_path, checkpoint_path=ckpt_path,
 return_sequences=False) output = rannet_model.output # (B, D) output =
 L.Dropout(0.1)(output) output = L.Dense(2, activation='softmax')(output) model
 = keras.models.Model(rannet_model.input, output) model.summary() ``` *For the
 sequence task* ```python from rannet import RanNet, RanNetWordPieceTokenizer
 vocab_path = 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt'
@@ -39,16 +45,28 @@
 ( config_path=config_path, checkpoint_path=ckpt_path, return_cell=False) output
 = rannet_model.output # (B, L, D) rannet_model.summary() ``` ## ð w/
 o pretrained models Embed the `RAN` (a Keras layer) into your network.
 ```python from rannet import RAN ran = RAN(head_num=8, head_size=256,
 window_size=256, min_window_size=16, activation='swish',
 kernel_initializer='glorot_normal', apply_lm_mask=False,
 apply_seq2seq_mask=False, apply_memory_review=True, dropout_rate=0.0,
-cell_initializer_type='zero') output, cell = ran(X) ``` # ð Citation If you
-use our code in your research, please cite our work: ``` @inproceedings{li-
-etal-2023-ran, title = "Recurrent Attention Networks for Long-text Modeling",
-author = "Li, Xianming and Li, Zongxi and Luo, Xiaotian and Xie, Haoran and
-Lee, Xing and Zhao, Yingbin and Wang, Fu Lee and Li, Qing", booktitle =
-"Findings of the Association for Computational Linguistics: ACL 2023", year =
-"2023", publisher = "Association for Computational Linguistics" } ``` # ð¬
-Contact Please contact us at 1) for code problems, create a GitHub issue; 2)
-for paper problems, email xmlee97@gmail.com
+cell_initializer_type='zero') output, cell = ran(X) ``` ## w/ history ```python
+import numpy as np from rannet import RanNet, RanNetWordPieceTokenizer
+vocab_path = 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt'
+config_path = 'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer
+(vocab_path, lowercase=True) rannet, rannet_model = RanNet.load_rannet
+( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False,
+apply_cell_transform=False, return_history=True, # return history
+cell_pooling='mean', with_cell=True, # with cell input ) rannet_model.summary()
+text = 'sentence 1' tok = tokenizer.encode(text) init_cell = np.zeros((1, 768))
+# 768 is embedding size vec, history = rannet_model.predict([np.array(
+[tok.ids]), init_cell]) text2 = 'sentence 2' tok = tokenizer.encode(text2)
+vec2, history = rannet_model.predict([np.array([tok.ids]), history]) # input
+history of sentence 1 ``` # ð Citation If you use our code in your research,
+please cite our work: ``` @inproceedings{li-etal-2023-recurrent, title =
+"Recurrent Attention Networks for Long-text Modeling", author = "Li, Xianming
+and Li, Zongxi and Luo, Xiaotian and Xie, Haoran and Lee, Xing and Zhao,
+Yingbin and Wang, Fu Lee and Li, Qing", booktitle = "Findings of the
+Association for Computational Linguistics: ACL 2023", month = jul, year =
+"2023", publisher = "Association for Computational Linguistics", pages = "3006-
+-3019", } ``` # ð¬ Contact Please contact us at 1) for code problems, create
+a GitHub issue; 2) for paper problems, email xmlee97@gmail.com
```

### Comparing `rannet-0.2.1/rannet/dataloader.py` & `rannet-0.3.0/rannet/dataloader.py`

 * *Files identical despite different names*

### Comparing `rannet-0.2.1/rannet/layers.py` & `rannet-0.3.0/rannet/layers.py`

 * *Files identical despite different names*

### Comparing `rannet-0.2.1/rannet/optimizer.py` & `rannet-0.3.0/rannet/optimizer.py`

 * *Files identical despite different names*

### Comparing `rannet-0.2.1/rannet/pretrain.py` & `rannet-0.3.0/rannet/pretrain.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,29 +8,22 @@
 import re
 import json
 import time
 import random
 
 import click
 import tensorflow as tf
-# import tensorflow_addons as tfa
 from langml import keras, TF_KERAS, log
 from tqdm import tqdm
 from boltons.iterutils import chunked_iter
 
 from rannet import RanNetForMLMPretrain, RanNetParams
 from rannet.dataloader import DataLoader, BertMlmDataLoader
 from rannet.tokenizer import RanNetWordPieceTokenizer
 
-from bert4keras.optimizers import Adam
-from bert4keras.optimizers import extend_with_weight_decay
-from bert4keras.optimizers import extend_with_layer_adaptation
-from bert4keras.optimizers import extend_with_piecewise_linear_lr
-from bert4keras.optimizers import extend_with_gradient_accumulation
-
 
 gpus = tf.config.experimental.list_physical_devices('GPU')
 for gpu in gpus:
     tf.config.experimental.set_memory_growth(gpu, True)
 
 
 def split_sentences(text: str, max_length: int = 512, lang: str = 'english'):
@@ -158,31 +151,29 @@
 @click.option('--base_ckpt_path', type=str, default=None,
               help='Specify the checkpoint path of the base RanNet model when continuing pretraining.')
 @click.option('--save_dir', type=str, required=True, help='Specify dir to save model')
 @click.option('--record_info_path', type=str, required=True, help='Specify record info path.')
 @click.option('--batch_size', type=int, default=32, help='Specify batch size. Defaults to 32')
 @click.option('--learning_rate', type=float, default=1e-3, help='Specify learning rate. Defaults to 1e-3')
 @click.option('--weight_decay', type=float, default=0.01, help='Specify weight decay. Defaults to 1e-2')
-@click.option('--global_clipnorm', type=float, default=1.0, help='Specify global_clipnorm. Defaults to 1.0')
 @click.option('--sequence_length', type=int, default=512, help='Specify sequence length. Defaults to 512')
 @click.option('--num_warmup_steps', type=int, default=3000, help='Specify warmup steps. Defaults to 3000')
 @click.option('--num_train_steps', type=int, default=125000, help='Specify training steps. Defaults to 125000')
 @click.option('--ckpt_save_freq', type=int, default=125000, help='Specify ckpt save freq. Defaults to 125000')
 @click.option('--gradient_accumulation_steps', type=int, default=1,
               help='Specify gradient accumulation steps. Defaults to 1, if value > 1, then use gradient accumulation.')
 @click.option('--distributed', is_flag=True, default=False, help='Specify distributed training with `--distributed`.')
 @click.option('--distributed_strategy', type=str, default='MirroredStrategy',
               help='Specify distributed training strategy. Defaults to MirroredStrategy')
 @click.option('--verbose', type=int, default=1,
               help='0 = silent, 1 = progress bar, 2 = one line per epoch.')
 def pretrain(corpus_path: str, config_path: str, log_path: str, base_ckpt_path: str, save_dir: str,
              record_info_path: str, batch_size: int, learning_rate: float, weight_decay: float,
-             global_clipnorm: float, sequence_length: int, num_warmup_steps: int, num_train_steps: int,
-             ckpt_save_freq: int, gradient_accumulation_steps: int, distributed: bool,
-             distributed_strategy: str, verbose: int):
+             sequence_length: int, num_warmup_steps: int, num_train_steps: int, ckpt_save_freq: int,
+             gradient_accumulation_steps: int, distributed: bool, distributed_strategy: str, verbose: int):
     # create save dir
     os.makedirs(save_dir, exist_ok=True)
 
     # environment check
     assert TF_KERAS, 'To pretrain rannet, please `export TF_KERAS=1` first'
 
     # load hyperparameters
@@ -192,62 +183,27 @@
     log.info(f'config: {config}')
 
     # load model
     def build_model():
         rannet = RanNetForMLMPretrain(params)
         model = rannet()
 
-        '''
         lr_schedule = None if gradient_accumulation_steps < 2 else {
             num_warmup_steps * gradient_accumulation_steps: 1.0,
             num_train_steps * gradient_accumulation_steps: 0.0,
         }
         grad_accum_steps = None if gradient_accumulation_steps < 2 else gradient_accumulation_steps
         RanNetForMLMPretrain.compile(model,
                                      learning_rate=learning_rate,
                                      weight_decay=weight_decay,
                                      loss=None,
                                      lr_schedule=lr_schedule,
                                      gradient_accumulation_steps=grad_accum_steps,
                                      metrics=['sparse_categorical_accuracy'])
-        '''
 
-        lr_schedule = None if gradient_accumulation_steps < 2 else {
-            num_warmup_steps * gradient_accumulation_steps: 1.0,
-            num_train_steps * gradient_accumulation_steps: 0.0,
-        }
-        grad_accum_steps = None if gradient_accumulation_steps < 2 else gradient_accumulation_steps
-        optimizer = extend_with_weight_decay(Adam)
-        optimizer = extend_with_layer_adaptation(optimizer)  # lambda
-        optimizer = extend_with_piecewise_linear_lr(optimizer)
-        optimizer_params = {
-            'learning_rate': learning_rate,
-            'weight_decay_rate': weight_decay,
-            'exclude_from_weight_decay': ['Norm', 'bias'],
-            'exclude_from_layer_adaptation': ['Norm', 'bias'],
-            'bias_correction': False,
-        }
-        if lr_schedule is not None:
-            optimizer_params['lr_schedule'] = lr_schedule
-        if grad_accum_steps is not None:
-            optimizer = extend_with_gradient_accumulation(optimizer)
-            optimizer_params['grad_accum_steps'] = grad_accum_steps
-        optimizer = optimizer(**optimizer_params)
-
-        '''
-        optimizer = tfa.optimizers.LAMB(
-            learning_rate=learning_rate,
-            weight_decay=weight_decay,
-            exclude_from_weight_decay=['LayerNorm', 'Norm', 'bias'],
-            exclude_from_layer_adaptation=['LayerNorm', 'Norm', 'bias'],
-            global_clipnorm=global_clipnorm,
-        )
-        '''
-        model.compile(optimizer=optimizer, loss=None, metrics=['sparse_categorical_accuracy'])
-        model.summary()
         if base_ckpt_path is not None:
             # restore the pre-trained model
             log.info(f'restore weights from {base_ckpt_path}')
             try:
                 model.load_weights(base_ckpt_path)
             except NotImplementedError:
                 log.warn('failed to restore weights via `model.load_weights`, '
```

### Comparing `rannet-0.2.1/rannet/ran.py` & `rannet-0.3.0/rannet/ran.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Dict, Optional, Tuple, List, Callable, Union
 
 import tensorflow as tf
 from langml import keras, L, K
 from langml.layers import SineCosinePositionEmbedding, LayerNorm
 from langml.tensor_typing import Tensors, Initializer, Activation
 
-from rannet.utils import triangular_causal_mask, prefix_causal_mask, standard_normalize, mean
+from rannet.utils import triangular_causal_mask, prefix_causal_mask, standard_normalize
 
 
 def align(tensor: Tensors, axes: int, ndim: Optional[int] = None) -> Tensors:
     assert len(axes) == K.ndim(tensor)
     assert ndim or min(axes) >= 0
     ndim = ndim or max(axes) + 1
     indices = [None] * ndim
@@ -417,15 +417,14 @@
         return {'PosMultiHeadAttention': PosMultiHeadAttention}
 
 
 def ran(inputs: Tensors,
         encode_attn: PosMultiHeadAttention,
         cell: Optional[Tensors] = None,
         segments: Optional[Tensors] = None,
-        cell_initializer_type: str = 'zero',
         cell_initializer: Optional[Callable] = None,
         cell_glu: Optional[Callable] = None,
         cell_residual_layernorm: Optional[Callable] = None,
         mask: Optional[Tensors] = None,
         apply_lm_mask: bool = False,
         apply_seq2seq_mask: bool = False,
         window_size: int = 128,
@@ -484,31 +483,29 @@
                 0,
                 K.shape(inputs)[1] + 1, K.shape(inputs)[1],
                 dtype='int32'),  # [0, K.shape(inputs)[1]], time_steps < window_size
         )
 
         # init cell
         if cell is None:
-            if cell_initializer_type == 'mean':
-                # initialize cell with mean pooling
-                cell = mean(inputs, mask, axis=1, keepdims=True)
-            elif cell_initializer_type == 'zero':
-                # initialize cell with zeros
-                cell = K.zeros_like(inputs[:, 0])
-                cell = K.expand_dims(cell, axis=1)
-            else:
-                raise ValueError(f'invalid assignment {cell_initializer_type}, '
-                                 'please specify cell_initializer_type from [`mean`, `zero`]')
+            # initialize cell with zeros
+            cell = K.zeros_like(inputs[:, 0])
+            cell = K.expand_dims(cell, axis=1)
         else:
             if K.ndim(cell) == 2:
                 cell = K.expand_dims(cell, axis=1)
-        # with weight
-        cell = cell_initializer(cell)
+
+        cell_t = cell_initializer(cell)
         if dropout_rate > 0:
-            cell = L.Dropout(dropout_rate)(cell)
+            cell_t = L.Dropout(dropout_rate)(cell_t)
+        cell = tf.cond(
+            tf.equal(tf.math.count_nonzero(cell), 0),
+            lambda: cell_t,  # apply dense layer
+            lambda: cell
+        )
 
         # slice window input
         current_input = inputs[:, ind[0]: ind[1]]  # (B, W, D)
         current_mask = mask[:, ind[0]: ind[1]] if mask is not None else None
         current_segment = segments[:, ind[0]: ind[1]] if segments is not None else None
 
         # encode
@@ -606,53 +603,52 @@
         name='final-step'
     )
 
     if isinstance(memory_review, SelfAttention):
         outputs = memory_review([outputs, cells, cells], mask=mask)
     else:
         outputs = memory_review(outputs)
+    last_cell = K.squeeze(cell, axis=1)  # (B, D)
     if cell_pooling == 'last':
-        cell = K.squeeze(cell, axis=1)  # (B, D)
+        cell = last_cell
     elif cell_pooling == 'mean':
         cell = K.mean(cells, axis=1)
     elif cell_pooling == 'max':
         cell = K.max(cells, axis=1)
     else:
         raise ValueError('Please specify `cell_pooling` from [`last`, `mean`, `max`]')
-    return outputs, cell
+    return last_cell, outputs, cell
 
 
 class RAN(L.Layer):
     def __init__(self,
                  head_num: int,
                  head_size: int = 256,
                  window_size: int = 128,
                  min_window_size: int = 16,
                  activation: Activation = 'swish',
                  kernel_initializer: Initializer = 'glorot_normal',
                  apply_lm_mask: bool = False,
                  apply_seq2seq_mask: bool = False,
                  apply_memory_review: bool = True,
                  dropout_rate: float = 0.0,
-                 cell_initializer_type: str = 'zero',
                  cell_pooling: str = 'last',
                  **kwargs):
         super(RAN, self).__init__(**kwargs)
         assert window_size > min_window_size, "window_size must be greater than min_window_size"
         self.head_num = head_num
         self.head_size = head_size
         self.window_size = window_size
         self.min_window_size = min_window_size
         self.activation = keras.activations.get(activation)
         self.kernel_initializer = kernel_initializer
         self.apply_lm_mask = apply_lm_mask
         self.apply_seq2seq_mask = apply_seq2seq_mask
         self.apply_memory_review = apply_memory_review
         self.dropout_rate = dropout_rate
-        self.cell_initializer_type = cell_initializer_type
         self.cell_pooling = cell_pooling
         self.supports_masking = True
 
     def get_config(self):
         config = {
             "head_num": self.head_num,
             "head_size": self.head_size,
@@ -660,15 +656,14 @@
             "min_window_size": self.min_window_size,
             "activation": keras.activations.serialize(self.activation),
             "kernel_initializer": keras.initializers.serialize(self.kernel_initializer),
             "apply_lm_mask": self.apply_lm_mask,
             "apply_seq2seq_mask": self.apply_seq2seq_mask,
             "apply_memory_review": self.apply_memory_review,
             "dropout_rate": self.dropout_rate,
-            "cell_initializer_type": self.cell_initializer_type,
             "cell_pooling": self.cell_pooling
         }
         base_config = super(RAN, self).get_config()
         return dict(base_config, **config)
 
     def build(self, input_shape: Union[Tensors, List[Tensors]]):
         super(RAN, self).build(input_shape)
@@ -727,41 +722,40 @@
         if isinstance(inputs, list):
             inputs, mask = inputs[0], inputs[1]
 
         # text mask
         mask = mask[0] if isinstance(mask, list) else mask
         assert mask is not None, "mask should not be None!"
 
-        outputs, cell = ran(
+        last_cell, outputs, cell = ran(
             inputs,
             self.encode_attn,
             cell=cell,
             segments=segments,
-            cell_initializer_type=self.cell_initializer_type,
             cell_initializer=self.cell_initializer,
             cell_glu=self.cell_glu,
             cell_residual_layernorm=self.cell_residual_layernorm,
             mask=mask,
             apply_lm_mask=self.apply_lm_mask,
             apply_seq2seq_mask=self.apply_seq2seq_mask,
             window_size=self.window_size,
             concat_layernorm=self.concat_layernorm,
             memory_review=self.memory_review,
             dropout_rate=self.dropout_rate,
             min_window_size=self.min_window_size,
             cell_pooling=self.cell_pooling
         )
-        return [outputs, cell]
+        return [last_cell, outputs, cell]
 
     def compute_output_shape(self,
                              input_shape: Union[Tensors, List[Tensors]]) -> Union[Tensors, Tuple[Tensors, Tensors]]:
         if not isinstance(input_shape, list):
             input_shape = [input_shape]
         cell_shape = (input_shape[0][0], input_shape[0][-1])
-        return [input_shape[0], cell_shape]
+        return [cell_shape, input_shape[0], cell_shape]
 
     @staticmethod
     def get_custom_objects() -> Dict:
         return {'RAN': RAN}
 
 
 custom_objects = {}
```

### Comparing `rannet-0.2.1/rannet/rannet.py` & `rannet-0.3.0/rannet/rannet.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         self.embedding_size = config.get('embedding_size', 512)
         self.dropout_rate = config.get('dropout_rate', 0.1)
         self.ran_layers = config.get('ran_layers', 2)
         self.head_size = config.get('head_size', 128)
         self.head_num = config.get('head_num', 8)
         self.window_size = config.get('window_size', 256)
         self.min_window_size = config.get('min_window_size', 16)
-        self.cell_initializer_type = config.get('cell_initializer_type', 'zero')  # zero | mean
         self.cell_pooling = config.get('cell_pooling', 'last')  # last | mean | max
         self.embedding_initializer = config.get('embedding_initializer', 'truncated_normal')
         self.kernel_initializer = config.get('kernel_initializer', 'truncated_normal')
         self.kernel_initializer_range = config.get('kernel_initializer_range', 0.02)
 
     @staticmethod
     def from_file(config_path: str):
@@ -51,31 +50,29 @@
 
 
 class RanNet:
     def __init__(self,
                  params: RanNetParams,
                  return_sequences: bool = True,
                  return_cell: bool = True,
-                 return_history: bool = True,
+                 return_history: bool = False,
                  mlm_softmax: bool = False,
                  apply_cell_transform: bool = True,
                  apply_lm_mask: bool = False,
                  apply_seq2seq_mask: bool = False,
                  apply_memory_review: bool = True,
-                 cell_initializer_type: str = 'zero',
                  cell_pooling: str = 'last',
                  min_window_size: Optional[int] = None,
                  window_size: Optional[int] = None,
                  prefix: str = ''):
         self.params = params
         self.return_sequences = return_sequences
         self.return_cell = return_cell
         self.return_history = return_history
         self.apply_cell_transform = apply_cell_transform
-        self.cell_initializer_type = cell_initializer_type
         self.cell_pooling = cell_pooling
         self.min_window_size = min_window_size
         self.window_size = window_size
         self.prefix = prefix
         self.inputs = None
         self.__var_status = {}
 
@@ -108,15 +105,14 @@
                 min_window_size=self.min_window_size or self.params.min_window_size,
                 activation='swish',
                 kernel_initializer=self.initializer,
                 apply_lm_mask=apply_lm_mask,
                 apply_seq2seq_mask=apply_seq2seq_mask,
                 apply_memory_review=apply_memory_review,
                 dropout_rate=self.params.dropout_rate,
-                cell_initializer_type=self.cell_initializer_type or self.params.cell_initializer_type,
                 cell_pooling=self.cell_pooling or self.params.cell_pooling,
                 name=self.get_weight_name(f'RAN-{i}')
             )
             for i in range(self.params.ran_layers)
         ]
         self.mlm_hidden = keras.Sequential([
             L.Dropout(self.params.dropout_rate, name='Dropout'),
@@ -165,16 +161,17 @@
                x_mask: Tensors,
                cell: Optional[Tensors] = None,
                segments: Optional[Tensors] = None) -> Union[Tensors, List[Tensors]]:
         x = self.embedding_layernorm(x)
         x = self.embedding_dropout(x)
 
         outputs = x
+        last_cell = cell
         for kernel in self.rans:
-            outputs, cell = kernel([outputs, x_mask], cell=cell, segments=segments)
+            last_cell, outputs, cell = kernel([outputs, x_mask], cell=last_cell, segments=segments)
 
         if self.return_cell and self.apply_cell_transform:
             cell = L.Lambda(lambda x: K.expand_dims(x, axis=1))(cell)
             cell = L.Dense(self.params.embedding_size,
                            kernel_initializer=self.initializer,
                            activation='swish',
                            name='Output-Cell-Dense')(cell)
@@ -186,19 +183,23 @@
             max_pooling = L.Lambda(lambda x: K.max(x, axis=1, keepdims=True))(outputs)
             max_pooling = L.Dense(self.params.embedding_size,
                                   kernel_initializer=self.initializer,
                                   name='Output-Pooling-Dense')(max_pooling)
             # ct = p + g(c), use maxpooling to enhance semantic feature
             cell = L.Lambda(lambda x: x[0] + x[1], name='Output-Cell-Fuse')([cell, max_pooling])
             cell = L.Lambda(lambda x: K.squeeze(x, axis=1), name='Output-Cell-Squeeze')(cell)
+
+        ret = []
         if self.return_sequences:
-            if self.return_cell:
-                return [outputs, cell]
-            return outputs
-        return cell
+            ret.append(outputs)
+        if self.return_cell:
+            ret.append(cell)
+        if self.return_history:
+            ret.append(last_cell)
+        return ret
 
     def __call__(self,
                  with_cell: bool = False,
                  with_mlm: bool = False,
                  return_model: bool = True,
                  seq2seq: bool = False) -> Union[Models, Tensors]:
         """ build model
@@ -227,15 +228,15 @@
         outputs = self.encode(x, x_mask, cell, segments=segments)
 
         if not with_mlm:
             if return_model:
                 return keras.Model(self.inputs, outputs)
             return outputs
 
-        output = outputs[0] if self.return_cell else outputs
+        output = outputs[0]
         mlm = self.mlm_hidden(output)
         mlm = self.mlm_matching([mlm, embedding_weights])
 
         if return_model:
             return keras.Model(self.inputs, mlm)
         return mlm
 
@@ -385,15 +386,14 @@
                     raise ValueError(f'failed load layer {layer_name}, error: {error}')
         return model
 
     @staticmethod
     def load_rannet(config_path: str,
                     checkpoint_path: str,
                     window_size: Optional[int] = None,
-                    cell_initializer_type: Optional[str] = None,
                     with_mlm: bool = False,
                     with_cell: bool = False,
                     **kwargs) -> Tuple[object, Models]:
         """ Load pretrained RanNet model
         Args:
             config_path: str. Path to config
             checkpoint_path: str. Path to checkpoint
@@ -402,16 +402,14 @@
         Return:
             RanNet: RanNet object
             model: RanNet keras model
         """
         params = RanNetParams.from_file(config_path)
         if window_size is not None:
             params.window_size = window_size
-        if cell_initializer_type is not None:
-            params.cell_initializer_type = cell_initializer_type
         rannet = RanNet(params, **kwargs)
         model = rannet(with_mlm=with_mlm, with_cell=with_cell)
         model = rannet.restore_weights_from_checkpoint(model, checkpoint_path, ran_layers=params.ran_layers)
         return rannet, model
 
     @staticmethod
     def compile(model: Models,
```

### Comparing `rannet-0.2.1/rannet/tokenizer.py` & `rannet-0.3.0/rannet/tokenizer.py`

 * *Files identical despite different names*

### Comparing `rannet-0.2.1/rannet/utils.py` & `rannet-0.3.0/rannet/utils.py`

 * *Files identical despite different names*

### Comparing `rannet-0.2.1/rannet.egg-info/PKG-INFO` & `rannet-0.3.0/rannet.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rannet
-Version: 0.2.1
+Version: 0.3.0
 Summary: Recurrent Attention Networks
 Author: sean lee
 Author-email: xmlee97@gmail.com
 Keywords: rannet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -37,14 +37,18 @@
    </a>
    <a href="https://arxiv.org/abs/2306.06843">
       <img src="https://img.shields.io/badge/Arxiv-2306.06843-yellow.svg?style=flat-square" alt="https://arxiv.org/abs/2306.06843" />
    </a>
 </h4>
 
 
+<p align="center">
+<img src='assets/framework.png' alt='The framework of RAN' style='width: 520px;' />
+</p>
+
 
 # ⬇️ Installation
 
 *stable*
 
 ```bash
 python -m pip install -U rannet
@@ -58,19 +62,38 @@
 
 *environment*
 - ⭐ tensorflow>2.0,<=2.10 🤗 `export TF_KERAS=1`
 - tensorflow>=1.14,<2.0 🤗 Keras==2.3.1
 
 ## 🏛️ Pretrained Models
 
+### V3 Models
+
+🎯 compatible with: `rannet>0.2.1`
+
+| Lang | Google Drive | Baidu NetDrive |
+|------|--------------|----------------|
+| EN   |    [base](https://drive.google.com/file/d/1CO1M_57U506_3mDBqtGo-5b1XXNpONln/view?usp=sharing)          |        [base](https://pan.baidu.com/s/1Z2wODILsIeZ3i8_9GEpl2g)\[code: udts\]        |
+
+Chinese Models are still pretraining...
+
+
+### V2 Models
+
+🎯 compatible with: `rannet<=0.2.1`
+
 | Lang | Google Drive | Baidu NetDrive |
 |------|--------------|----------------|
 | EN   |    [base](https://drive.google.com/file/d/1mRabw0Hy9T5_EWbZshD6Uk-bvauNzG9R/view?usp=sharing)          |        [base](https://pan.baidu.com/s/18uhAkY46aIcy4ncwzXp5mA)\[code: djkj\]        |
 | CN   |   [base](https://drive.google.com/file/d/1_gmrulSU-ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing)  \| [small](https://drive.google.com/file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/view?usp=sharing)         |        [base](https://pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\[code: e47w\]  \| [small](https://pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\[code: mdmg\]        |
 
+### V1 Models
+
+V1 models are not open.
+
 
 # 🚀 Quick Tour
 
 ## 🈶 w/ pretrained models
 
 *Extract semantic feature*
 
@@ -152,24 +175,66 @@
           apply_seq2seq_mask=False,
           apply_memory_review=True,
           dropout_rate=0.0,
           cell_initializer_type='zero')
 output, cell = ran(X)
 ```
 
+## w/ history
+
+```python
+import numpy as np
+from rannet import RanNet, RanNetWordPieceTokenizer
+
+
+vocab_path = 'pretrained/vocab.txt'
+ckpt_path = 'pretrained/model.ckpt'
+config_path = 'pretrained/config.json'
+tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True)
+
+rannet, rannet_model = RanNet.load_rannet(
+    config_path=config_path,
+    checkpoint_path=ckpt_path,
+    return_sequences=False,
+    apply_cell_transform=False,
+    return_history=True,  # return history
+    cell_pooling='mean',
+    with_cell=True,  # with cell input
+)
+rannet_model.summary()
+
+text = 'sentence 1'
+tok = tokenizer.encode(text)
+init_cell = np.zeros((1, 768))  # 768 is embedding size
+vec, history = rannet_model.predict([np.array([tok.ids]), init_cell])
+
+text2 = 'sentence 2'
+tok = tokenizer.encode(text2)
+vec2, history = rannet_model.predict([np.array([tok.ids]), history])  # input history of sentence 1
+```
+
 # 📚 Citation
 
 If you use our code in your research, please cite our work:
 
 ```
-@inproceedings{li-etal-2023-ran,
+@inproceedings{li-etal-2023-recurrent,
     title = "Recurrent Attention Networks for Long-text Modeling",
-    author = "Li, Xianming and Li, Zongxi and Luo, Xiaotian and Xie, Haoran and Lee, Xing and Zhao, Yingbin and Wang, Fu Lee and Li, Qing",
+    author = "Li, Xianming  and
+      Li, Zongxi  and
+      Luo, Xiaotian  and
+      Xie, Haoran  and
+      Lee, Xing  and
+      Zhao, Yingbin  and
+      Wang, Fu Lee  and
+      Li, Qing",
     booktitle = "Findings of the Association for Computational Linguistics: ACL 2023",
+    month = jul,
     year = "2023",
-    publisher = "Association for Computational Linguistics"
+    publisher = "Association for Computational Linguistics",
+    pages = "3006--3019",
 }
 ```
 
 # 📬 Contact
 
 Please contact us at 1) for code problems, create a GitHub issue; 2) for paper problems, email xmlee97@gmail.com
```

#### html2text {}

```diff
@@ -1,46 +1,52 @@
-Metadata-Version: 2.1 Name: rannet Version: 0.2.1 Summary: Recurrent Attention
+Metadata-Version: 2.1 Name: rannet Version: 0.3.0 Summary: Recurrent Attention
 Networks Author: sean lee Author-email: xmlee97@gmail.com Keywords: rannet
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
 License-File: LICENSE
                 ****** RAN: Recurrent Attention Network ******
   *** ð¢ This project is still in the works in order to make long document
                              modeling easier. ***
  *** [RAN_is_released_under_the_MIT_license.] [PyPI_version] [PyPI_Downloads]
      [http://makeapullrequest.com] [https://arxiv.org/abs/2306.06843] ***
+                            [The framework of RAN]
 # â¬ï¸ Installation *stable* ```bash python -m pip install -U rannet ```
 *latest* ```bash python -m pip install git+https://github.com/4AI/RAN.git ```
 *environment* - â­ tensorflow>2.0,<=2.10 ð¤ `export TF_KERAS=1` -
-tensorflow>=1.14,<2.0 ð¤ Keras==2.3.1 ## ðï¸ Pretrained Models | Lang |
-Google Drive | Baidu NetDrive | |------|--------------|----------------| | EN |
-[base](https://drive.google.com/file/d/1mRabw0Hy9T5_EWbZshD6Uk-bvauNzG9R/
-view?usp=sharing) | [base](https://pan.baidu.com/s/18uhAkY46aIcy4ncwzXp5mA)\
-[code: djkj\] | | CN | [base](https://drive.google.com/file/d/1_gmrulSU-
-ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing) \| [small](https://drive.google.com/
-file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/view?usp=sharing) | [base](https://
-pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\[code: e47w\] \| [small](https://
-pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\[code: mdmg\] | # ð Quick Tour ##
-ð¶ w/ pretrained models *Extract semantic feature* set
-`return_sequences=False` to extract semantic feature. ```python import numpy as
-np from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
-'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
-'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
-lowercase=True) rannet, rannet_model = RanNet.load_rannet
-( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False,
-apply_cell_transform=False, cell_pooling='mean' ) text = 'input text' tok =
-tokenizer.encode(text) vec = rannet_model.predict(np.array([tok.ids])) ``` *For
-the classification task* ```python from rannet import RanNet,
-RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt' ckpt_path =
-'pretrained/model.ckpt' config_path = 'pretrained/config.json' tokenizer =
+tensorflow>=1.14,<2.0 ð¤ Keras==2.3.1 ## ðï¸ Pretrained Models ### V3
+Models ð¯ compatible with: `rannet>0.2.1` | Lang | Google Drive | Baidu
+NetDrive | |------|--------------|----------------| | EN | [base](https://
+drive.google.com/file/d/1CO1M_57U506_3mDBqtGo-5b1XXNpONln/view?usp=sharing) |
+[base](https://pan.baidu.com/s/1Z2wODILsIeZ3i8_9GEpl2g)\[code: udts\] | Chinese
+Models are still pretraining... ### V2 Models ð¯ compatible with:
+`rannet<=0.2.1` | Lang | Google Drive | Baidu NetDrive | |------|--------------
+|----------------| | EN | [base](https://drive.google.com/file/d/
+1mRabw0Hy9T5_EWbZshD6Uk-bvauNzG9R/view?usp=sharing) | [base](https://
+pan.baidu.com/s/18uhAkY46aIcy4ncwzXp5mA)\[code: djkj\] | | CN | [base](https://
+drive.google.com/file/d/1_gmrulSU-ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing) \|
+[small](https://drive.google.com/file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/
+view?usp=sharing) | [base](https://pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\
+[code: e47w\] \| [small](https://pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\
+[code: mdmg\] | ### V1 Models V1 models are not open. # ð Quick Tour ## ð¶
+w/ pretrained models *Extract semantic feature* set `return_sequences=False` to
+extract semantic feature. ```python import numpy as np from rannet import
+RanNet, RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt' ckpt_path
+= 'pretrained/model.ckpt' config_path = 'pretrained/config.json' tokenizer =
+RanNetWordPieceTokenizer(vocab_path, lowercase=True) rannet, rannet_model =
+RanNet.load_rannet( config_path=config_path, checkpoint_path=ckpt_path,
+return_sequences=False, apply_cell_transform=False, cell_pooling='mean' ) text
+= 'input text' tok = tokenizer.encode(text) vec = rannet_model.predict(np.array
+([tok.ids])) ``` *For the classification task* ```python from rannet import
+RanNet, RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt' ckpt_path
+= 'pretrained/model.ckpt' config_path = 'pretrained/config.json' tokenizer =
 RanNetWordPieceTokenizer(vocab_path, lowercase=True) rannet, rannet_model =
 RanNet.load_rannet( config_path=config_path, checkpoint_path=ckpt_path,
 return_sequences=False) output = rannet_model.output # (B, D) output =
 L.Dropout(0.1)(output) output = L.Dense(2, activation='softmax')(output) model
 = keras.models.Model(rannet_model.input, output) model.summary() ``` *For the
 sequence task* ```python from rannet import RanNet, RanNetWordPieceTokenizer
 vocab_path = 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt'
@@ -49,16 +55,28 @@
 ( config_path=config_path, checkpoint_path=ckpt_path, return_cell=False) output
 = rannet_model.output # (B, L, D) rannet_model.summary() ``` ## ð w/
 o pretrained models Embed the `RAN` (a Keras layer) into your network.
 ```python from rannet import RAN ran = RAN(head_num=8, head_size=256,
 window_size=256, min_window_size=16, activation='swish',
 kernel_initializer='glorot_normal', apply_lm_mask=False,
 apply_seq2seq_mask=False, apply_memory_review=True, dropout_rate=0.0,
-cell_initializer_type='zero') output, cell = ran(X) ``` # ð Citation If you
-use our code in your research, please cite our work: ``` @inproceedings{li-
-etal-2023-ran, title = "Recurrent Attention Networks for Long-text Modeling",
-author = "Li, Xianming and Li, Zongxi and Luo, Xiaotian and Xie, Haoran and
-Lee, Xing and Zhao, Yingbin and Wang, Fu Lee and Li, Qing", booktitle =
-"Findings of the Association for Computational Linguistics: ACL 2023", year =
-"2023", publisher = "Association for Computational Linguistics" } ``` # ð¬
-Contact Please contact us at 1) for code problems, create a GitHub issue; 2)
-for paper problems, email xmlee97@gmail.com
+cell_initializer_type='zero') output, cell = ran(X) ``` ## w/ history ```python
+import numpy as np from rannet import RanNet, RanNetWordPieceTokenizer
+vocab_path = 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt'
+config_path = 'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer
+(vocab_path, lowercase=True) rannet, rannet_model = RanNet.load_rannet
+( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False,
+apply_cell_transform=False, return_history=True, # return history
+cell_pooling='mean', with_cell=True, # with cell input ) rannet_model.summary()
+text = 'sentence 1' tok = tokenizer.encode(text) init_cell = np.zeros((1, 768))
+# 768 is embedding size vec, history = rannet_model.predict([np.array(
+[tok.ids]), init_cell]) text2 = 'sentence 2' tok = tokenizer.encode(text2)
+vec2, history = rannet_model.predict([np.array([tok.ids]), history]) # input
+history of sentence 1 ``` # ð Citation If you use our code in your research,
+please cite our work: ``` @inproceedings{li-etal-2023-recurrent, title =
+"Recurrent Attention Networks for Long-text Modeling", author = "Li, Xianming
+and Li, Zongxi and Luo, Xiaotian and Xie, Haoran and Lee, Xing and Zhao,
+Yingbin and Wang, Fu Lee and Li, Qing", booktitle = "Findings of the
+Association for Computational Linguistics: ACL 2023", month = jul, year =
+"2023", publisher = "Association for Computational Linguistics", pages = "3006-
+-3019", } ``` # ð¬ Contact Please contact us at 1) for code problems, create
+a GitHub issue; 2) for paper problems, email xmlee97@gmail.com
```

### Comparing `rannet-0.2.1/setup.py` & `rannet-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     requirements = [l for l in f.read().splitlines() if l]
 
 with open('dev-requirements.txt', encoding='utf-8') as f:
     test_requirements = [l for l in f.read().splitlines() if l][1:]
 
 setup(
     name='rannet',
-    version='0.2.1',
+    version='0.3.0',
     description='Recurrent Attention Networks',
     long_description=readme,
     long_description_content_type="text/markdown",
     author='sean lee',
     author_email='xmlee97@gmail.com',
     packages=find_packages(exclude=("tests", "tests.*", "examples", "examples.*")),
     install_requires=requirements,
```

