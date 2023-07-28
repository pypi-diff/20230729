# Comparing `tmp/evo_prot_grad-0.1.3.tar.gz` & `tmp/evo_prot_grad-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evo_prot_grad-0.1.3.tar", last modified: Fri Jul 21 02:13:05 2023, max compression
+gzip compressed data, was "evo_prot_grad-0.1.4.tar", last modified: Fri Jul 28 23:51:08 2023, max compression
```

## Comparing `evo_prot_grad-0.1.3.tar` & `evo_prot_grad-0.1.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-21 02:13:05.215789 evo_prot_grad-0.1.3/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5109 2023-07-21 02:13:05.215480 evo_prot_grad-0.1.3/PKG-INFO
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     4380 2023-07-18 04:32:27.000000 evo_prot_grad-0.1.3/README.md
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-21 02:13:05.205463 evo_prot_grad-0.1.3/evo_prot_grad/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2343 2023-07-17 23:30:29.000000 evo_prot_grad-0.1.3/evo_prot_grad/__init__.py
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-21 02:13:05.209530 evo_prot_grad-0.1.3/evo_prot_grad/common/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-06-15 22:00:24.000000 evo_prot_grad-0.1.3/evo_prot_grad/common/__init__.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2028 2023-07-02 17:16:56.000000 evo_prot_grad-0.1.3/evo_prot_grad/common/embeddings.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    15061 2023-07-21 02:08:17.000000 evo_prot_grad-0.1.3/evo_prot_grad/common/sampler.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2751 2023-07-17 13:44:18.000000 evo_prot_grad-0.1.3/evo_prot_grad/common/tokenizers.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3029 2023-07-20 23:46:27.000000 evo_prot_grad-0.1.3/evo_prot_grad/common/utils.py
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-21 02:13:05.212284 evo_prot_grad-0.1.3/evo_prot_grad/experts/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-06-21 13:33:11.000000 evo_prot_grad-0.1.3/evo_prot_grad/experts/__init__.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    10623 2023-07-17 14:44:58.000000 evo_prot_grad-0.1.3/evo_prot_grad/experts/base_experts.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2986 2023-07-17 14:45:12.000000 evo_prot_grad-0.1.3/evo_prot_grad/experts/bert_expert.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3015 2023-07-17 13:49:07.000000 evo_prot_grad-0.1.3/evo_prot_grad/experts/causallm_expert.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2944 2023-07-17 13:48:59.000000 evo_prot_grad-0.1.3/evo_prot_grad/experts/esm_expert.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3292 2023-07-17 14:45:29.000000 evo_prot_grad-0.1.3/evo_prot_grad/experts/evcouplings_expert.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1490 2023-07-17 13:41:13.000000 evo_prot_grad-0.1.3/evo_prot_grad/experts/onehot_downstream_regression_expert.py
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-21 02:13:05.213370 evo_prot_grad-0.1.3/evo_prot_grad/models/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)      108 2023-06-21 12:05:07.000000 evo_prot_grad-0.1.3/evo_prot_grad/models/__init__.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1939 2023-07-02 21:00:15.000000 evo_prot_grad-0.1.3/evo_prot_grad/models/downstream_cnn.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    11712 2023-07-18 04:21:56.000000 evo_prot_grad-0.1.3/evo_prot_grad/models/potts.py
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-21 02:13:05.207702 evo_prot_grad-0.1.3/evo_prot_grad.egg-info/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5109 2023-07-21 02:13:05.000000 evo_prot_grad-0.1.3/evo_prot_grad.egg-info/PKG-INFO
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)      847 2023-07-21 02:13:05.000000 evo_prot_grad-0.1.3/evo_prot_grad.egg-info/SOURCES.txt
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        1 2023-07-21 02:13:05.000000 evo_prot_grad-0.1.3/evo_prot_grad.egg-info/dependency_links.txt
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       28 2023-07-21 02:13:05.000000 evo_prot_grad-0.1.3/evo_prot_grad.egg-info/requires.txt
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       14 2023-07-21 02:13:05.000000 evo_prot_grad-0.1.3/evo_prot_grad.egg-info/top_level.txt
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       38 2023-07-21 02:13:05.215929 evo_prot_grad-0.1.3/setup.cfg
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1403 2023-07-21 02:11:39.000000 evo_prot_grad-0.1.3/setup.py
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-21 02:13:05.215008 evo_prot_grad-0.1.3/test/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1611 2023-07-17 14:11:23.000000 evo_prot_grad-0.1.3/test/test_experts.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5099 2023-07-06 23:52:27.000000 evo_prot_grad-0.1.3/test/test_sampler.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3812 2023-07-17 14:14:09.000000 evo_prot_grad-0.1.3/test/test_utils.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-28 23:51:08.413679 evo_prot_grad-0.1.4/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5109 2023-07-28 23:51:08.413377 evo_prot_grad-0.1.4/PKG-INFO
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     4380 2023-07-18 04:32:27.000000 evo_prot_grad-0.1.4/README.md
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-28 23:51:08.401754 evo_prot_grad-0.1.4/evo_prot_grad/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2343 2023-07-17 23:30:29.000000 evo_prot_grad-0.1.4/evo_prot_grad/__init__.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-28 23:51:08.406640 evo_prot_grad-0.1.4/evo_prot_grad/common/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-06-15 22:00:24.000000 evo_prot_grad-0.1.4/evo_prot_grad/common/__init__.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2028 2023-07-02 17:16:56.000000 evo_prot_grad-0.1.4/evo_prot_grad/common/embeddings.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    15130 2023-07-28 23:19:54.000000 evo_prot_grad-0.1.4/evo_prot_grad/common/sampler.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2856 2023-07-28 23:20:46.000000 evo_prot_grad-0.1.4/evo_prot_grad/common/tokenizers.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3029 2023-07-20 23:46:27.000000 evo_prot_grad-0.1.4/evo_prot_grad/common/utils.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-28 23:51:08.410019 evo_prot_grad-0.1.4/evo_prot_grad/experts/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-06-21 13:33:11.000000 evo_prot_grad-0.1.4/evo_prot_grad/experts/__init__.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    10336 2023-07-28 23:38:42.000000 evo_prot_grad-0.1.4/evo_prot_grad/experts/base_experts.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3027 2023-07-28 23:33:34.000000 evo_prot_grad-0.1.4/evo_prot_grad/experts/bert_expert.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3249 2023-07-28 23:32:24.000000 evo_prot_grad-0.1.4/evo_prot_grad/experts/causallm_expert.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2992 2023-07-28 23:31:41.000000 evo_prot_grad-0.1.4/evo_prot_grad/experts/esm_expert.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3337 2023-07-28 23:33:59.000000 evo_prot_grad-0.1.4/evo_prot_grad/experts/evcouplings_expert.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1490 2023-07-17 13:41:13.000000 evo_prot_grad-0.1.4/evo_prot_grad/experts/onehot_downstream_regression_expert.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-28 23:51:08.411695 evo_prot_grad-0.1.4/evo_prot_grad/models/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)      108 2023-06-21 12:05:07.000000 evo_prot_grad-0.1.4/evo_prot_grad/models/__init__.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1939 2023-07-02 21:00:15.000000 evo_prot_grad-0.1.4/evo_prot_grad/models/downstream_cnn.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    11712 2023-07-18 04:21:56.000000 evo_prot_grad-0.1.4/evo_prot_grad/models/potts.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-28 23:51:08.404365 evo_prot_grad-0.1.4/evo_prot_grad.egg-info/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5109 2023-07-28 23:51:08.000000 evo_prot_grad-0.1.4/evo_prot_grad.egg-info/PKG-INFO
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)      847 2023-07-28 23:51:08.000000 evo_prot_grad-0.1.4/evo_prot_grad.egg-info/SOURCES.txt
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        1 2023-07-28 23:51:08.000000 evo_prot_grad-0.1.4/evo_prot_grad.egg-info/dependency_links.txt
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       28 2023-07-28 23:51:08.000000 evo_prot_grad-0.1.4/evo_prot_grad.egg-info/requires.txt
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       14 2023-07-28 23:51:08.000000 evo_prot_grad-0.1.4/evo_prot_grad.egg-info/top_level.txt
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       38 2023-07-28 23:51:08.413785 evo_prot_grad-0.1.4/setup.cfg
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1403 2023-07-28 23:47:12.000000 evo_prot_grad-0.1.4/setup.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-28 23:51:08.412918 evo_prot_grad-0.1.4/test/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1611 2023-07-17 14:11:23.000000 evo_prot_grad-0.1.4/test/test_experts.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5343 2023-07-28 22:37:41.000000 evo_prot_grad-0.1.4/test/test_sampler.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3812 2023-07-17 14:14:09.000000 evo_prot_grad-0.1.4/test/test_utils.py
```

### Comparing `evo_prot_grad-0.1.3/PKG-INFO` & `evo_prot_grad-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evo_prot_grad
-Version: 0.1.3
+Version: 0.1.4
 Summary: Directed evolution of proteins with fast gradient-based discrete MCMC.
 Home-page: https://github.nrel.gov/NREL/EvoProtGrad/
 Author: Patrick Emami
 Author-email: Patrick.Emami@nrel.gov
 License: BSD 3-Clause
 Keywords: protein engineering,directed evolution,huggingface,protein language models,mcmc
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `evo_prot_grad-0.1.3/README.md` & `evo_prot_grad-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.3/evo_prot_grad/__init__.py` & `evo_prot_grad-0.1.4/evo_prot_grad/__init__.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.3/evo_prot_grad/common/embeddings.py` & `evo_prot_grad-0.1.4/evo_prot_grad/common/embeddings.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.3/evo_prot_grad/common/sampler.py` & `evo_prot_grad-0.1.4/evo_prot_grad/common/sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 
     def reset(self):
         """Initialize the parallel chains of protein sequences.
         """
         if self.random_seed is not None:
             utils.set_seed(self.random_seed)
-
+        
         # the current state of each chain in string form
         self.chains = [self.wtseq] * self.parallel_chains
         # the current state of each chain in one-hot form
         self.chains_oh = self.canonical_chain_tokenizer(self.chains).to(self.device)
         # the WT protein in one-hot form
         self.wt_oh = self.chains_oh[0]
         # a List for storing the history of the product of experts values per chain
@@ -298,12 +298,13 @@
             for i in range(len(self.chains_oh_history)):
                 output_ += [ self.canonical_chain_tokenizer.decode(self.chains_oh_history[i]) ]
             scores_ = torch.stack(self.PoE_history).detach().cpu().numpy()
         elif self.output == 'best':
             best_idxs = torch.stack(self.PoE_history).argmax(0)
             chains_oh_history = torch.stack(self.chains_oh_history) # [n_steps, n_chains, seq_len, n_tokens]
             output_ = self.canonical_chain_tokenizer.decode(
-                torch.stack([chains_oh_history[best_idxs[i],i] for i in range(self.parallel_chains)]) )
-            scores_ = torch.stack(self.PoE_history)[best_idxs].detach().cpu().numpy()
+                torch.stack([chains_oh_history[best_idxs[i],i] for i in range(self.parallel_chains)]))
+            scores_ = torch.stack(
+                [self.PoE_history[best_idxs[i]][i] for i in range(self.parallel_chains)]).detach().cpu().numpy()
         return output_, scores_
```

### Comparing `evo_prot_grad-0.1.3/evo_prot_grad/common/tokenizers.py` & `evo_prot_grad-0.1.4/evo_prot_grad/common/tokenizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,30 +50,32 @@
         Args:
             alphabet (List[str]): A list of amino acid characters.
         """
         super().__init__(alphabet)
 
     def __call__(self, seqs: List[str]) -> torch.FloatTensor:
         """Convert seqs to one hot tensors.
-        Assumes each sequence is the same length.
+        Assumes each sequence is the same length. Handles sequences
+        with spaces between amino acids.
 
         Args:
             seqs (List[str]): A list of protein sequence strings of len [parallel_chains].
         Returns:
             ohs (torch.FloatTensor): of shape [parallel_chains, seq_len, vocab_size]
         """
         # convert seqs to ints
         seqs_ = [[self.vocab[aa] for aa in seq.upper() if aa != ' '] for seq in seqs]
         # convert to tensor using torch.nn.functional.one_hot()
         ohs = torch.nn.functional.one_hot(torch.LongTensor(seqs_), num_classes=self.vocab_size)
         return ohs.float()
 
 
     def decode(self, ohs: torch.Tensor) -> List[str]:
-        """Convert one-hot tensors back to a list of string sequences.
+        """Convert one-hot tensors back to a list of string sequences with 
+        a space between each amino acid.
 
         Args:
             ohs (torch.Tensor): shape [parallel_chains, seq_len, vocab_size]
         Returns:
             seqs (List[str]): A list of protein sequence strings of len [parallel_chains].
         """
         ohs = ohs.argmax(dim=-1)
```

### Comparing `evo_prot_grad-0.1.3/evo_prot_grad/common/utils.py` & `evo_prot_grad-0.1.4/evo_prot_grad/common/utils.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.3/evo_prot_grad/experts/base_experts.py` & `evo_prot_grad-0.1.4/evo_prot_grad/experts/base_experts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 import torch 
 import torch.nn as nn
-from typing import List, Tuple, Union, Optional, Any
+from typing import List, Tuple, Dict, Optional, Any
 from abc import ABC, abstractmethod
-from transformers import PreTrainedTokenizerBase
 import evo_prot_grad.common.utils as utils
 import evo_prot_grad.common.tokenizers as tokenizers
 
 
 class Expert(ABC):
     """Defines a common interface for any type of expert. 
     """
     def __init__(
         self,
         temperature: float,
         model: nn.Module,
-        tokenizer: Union[PreTrainedTokenizerBase, tokenizers.ExpertTokenizer],
+        vocab: Dict,
         device: str = "cpu",
         use_without_wildtype: bool = False
     ):
         """
         Args:
             temperature (float): Hyperparameter for re-scaling this expert in the Product of Experts.
             model (nn.Module): The model to use for the expert.
-            tokenizer (Union[PreTrainedTokenizerBase, tokenizers.ExpertTokenizer]):
-                The tokenizer to use for the expert.
+            vocab (Dict): The vocabulary for the expert.
             device (str): The device to use for the expert.
             use_without_wildtype (bool): Whether to use the expert without the wildtype,
                 i.e., do not subtract the wildtype score from the expert score.
         """
         self.model = model
         self.temperature = temperature
         self.device = device
         self.use_without_wildtype = use_without_wildtype
         self.model.to(self.device)
         self.model.eval()
-
-        vocab = tokenizer.get_vocab()
+                
         # sort by vocab values
         self.alphabet = [k for k, v in sorted(vocab.items(), key=lambda item: item[1])]
-        self.tokenizer = tokenizer 
 
-        #self.alphabet = alphabet
         self.expert_to_canonical_order = utils.expert_alphabet_to_canonical(
                                          self.alphabet, self.device)
         
         # a torch scalar 
         self._wt_score = None
        
     @abstractmethod
@@ -119,26 +114,26 @@
         raise NotImplementedError()
 
  
 class HuggingFaceExpert(Expert):
     def __init__(self,
                  temperature: float, 
                  model: nn.Module,
-                 tokenizer: PreTrainedTokenizerBase,
+                 vocab: Dict,
                  device: str,
                  use_without_wildtype: bool):
         """
         Args:
             temperature (float): Hyperparameter for re-scaling this expert in the Product of Experts.
             model (nn.Module): The model to use for the expert.
-            tokenizer (PreTrainedTokenizerBase): The tokenizer to use for the expert.
+            vocab (Dict): The vocab to use for the expert.
             device (str): The device to use for the expert.
             use_without_wildtype (bool): Whether to use the expert without the wildtype.
         """
-        super().__init__(temperature, model, tokenizer, device, use_without_wildtype)
+        super().__init__(temperature, model, vocab, device, use_without_wildtype)
 
 
     def set_wt_score(self, wt_seq: str) -> None:
         """ Sets the score value for wildtype protein wt_seq.
 
         Args:
             wt_seq (str): The wildtype sequence.
@@ -206,15 +201,16 @@
             model (nn.Module): The model to use for the expert.
             tokenizer (ExpertTokenizer): The tokenizer to use for the expert.
             use_without_wildtype (bool): Whether to use the expert without the wildtype.
             device (str): The device to use for the expert.
         """
         if tokenizer is None:
             tokenizer = tokenizers.OneHotTokenizer(utils.CANONICAL_ALPHABET)
-        super().__init__(temperature, model, tokenizer, device, use_without_wildtype)
+        super().__init__(temperature, model, tokenizer.get_vocab(), device, use_without_wildtype)
+        self.tokenizer = tokenizer
 
     def set_wt_score(self, wt_seq: str) -> None:
         """Sets the score value for wildtype protein wt_seq.
         
         Args:
             wt_seq (str): The wildtype sequence.
         """
```

### Comparing `evo_prot_grad-0.1.3/evo_prot_grad/experts/bert_expert.py` & `evo_prot_grad-0.1.4/evo_prot_grad/experts/bert_expert.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,21 +31,22 @@
         Raises:
             ValueError: If either `model` or `tokenizer` is not specified.
         """
         if model is None and tokenizer is None:
             model = BertForMaskedLM.from_pretrained("Rostlab/prot_bert")
             tokenizer = BertTokenizer.from_pretrained("Rostlab/prot_bert", do_lower_case=False)
         elif model is None or tokenizer is None:
-            raise ValueError("BERTExpert requires both `model` and `tokenizer` to be specified.")        
+            raise ValueError("BERTExpert requires both `model` and `tokenizer` to be specified.")  
         super().__init__(
             temperature,
             model,
-            tokenizer,
+            tokenizer.get_vocab(),
             device,
             use_without_wildtype)
+        self.tokenizer = tokenizer
         self.model.bert.embeddings.word_embeddings = embeddings.OneHotEmbedding(model.bert.embeddings.word_embeddings)
 
     def _get_last_one_hots(self) -> torch.Tensor:
         """ Returns the one-hot tensors *most recently passed* as input.
 
         Returns:
             one_hots (torch.Tensor): of shape [parallel_chains, seq_len, vocab_size]
```

### Comparing `evo_prot_grad-0.1.3/evo_prot_grad/experts/causallm_expert.py` & `evo_prot_grad-0.1.4/evo_prot_grad/experts/causallm_expert.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,24 +27,28 @@
             device (str): The device to use for the expert. Defaults to 'cpu'.
             use_without_wildtype (bool): Whether to use the expert without the wildtype.
         Raises:
             ValueError: If either `model` or `tokenizer` is not specified.
         """
         if model is None and tokenizer is None:
             model = AutoModelForCausalLM.from_pretrained("lightonai/RITA_s", trust_remote_code=True)
-            tokenizer = AutoTokenizer.from_pretrained("lightonai/RITA_s")
+            tokenizer = AutoTokenizer.from_pretrained("lightonai/RITA_s", )
         elif model is None or tokenizer is None:
             raise ValueError("CausalLMExpert requires both `model` and `tokenizer` to be specified.")
+        vocab = tokenizer.get_vocab()
+        if '<unk>' in vocab:
+            vocab.pop('<unk>')
         super().__init__(
             temperature = temperature,
             model = model,
-            tokenizer = tokenizer,
+            vocab = vocab,
             device = device,
             use_without_wildtype = use_without_wildtype
         )
+        self.tokenizer = tokenizer
         self.model.transformer.embedding = embeddings.OneHotEmbedding(model.transformer.embedding)
 
     def _get_last_one_hots(self):
         """ Returns the one-hot tensors *most recently passed* as input.
         """
         return self.model.transformer.embedding.one_hots
     
@@ -52,12 +56,14 @@
         """Convert inputs to a format suitable for the model.
         
         Args:
             inputs (List[str]): A list of protein sequence strings of len [parallel_chains].
         Returns:
             batch_encoding (BatchEncoding): A BatchEncoding object.
         """
+        # Remove all spaces between amino acids 
+        inputs = [seq.replace(' ', '') for seq in inputs]
         return self.tokenizer(inputs, add_special_tokens=False, return_tensors="pt").to(self.device)
    
 def build(**kwargs):
     """Builds a RitaExpert."""
     return CausalLMExpert(**kwargs)
```

### Comparing `evo_prot_grad-0.1.3/evo_prot_grad/experts/esm_expert.py` & `evo_prot_grad-0.1.4/evo_prot_grad/experts/esm_expert.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,18 @@
             model = EsmForMaskedLM.from_pretrained("facebook/esm2_t6_8M_UR50D")
             tokenizer = AutoTokenizer.from_pretrained("facebook/esm2_t6_8M_UR50D")
         elif model is None or tokenizer is None:
             raise ValueError("EsmExpert requires both `model` and `tokenizer` to be specified.")
         super().__init__(
             temperature,
             model,
-            tokenizer,
+            tokenizer.get_vocab(),
             device,
             use_without_wildtype)
+        self.tokenizer = tokenizer 
         self.model.esm.embeddings.word_embeddings = embeddings.OneHotEmbedding(model.esm.embeddings.word_embeddings)
 
     def _get_last_one_hots(self) -> torch.Tensor:
         """ Returns the one-hot tensors *most recently passed* as input.
         """
         return self.model.esm.embeddings.word_embeddings.one_hots
```

### Comparing `evo_prot_grad-0.1.3/evo_prot_grad/experts/evcouplings_expert.py` & `evo_prot_grad-0.1.4/evo_prot_grad/experts/evcouplings_expert.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,20 +26,21 @@
             use_without_wildtype (bool): Whether to use the expert without the wildtype.
         """
         assert model is not None, "EVCouplingsExpert requires a potts.EVCouplings model to be provided."
         if tokenizer is None:
             tokenizer = OneHotTokenizer(utils.CANONICAL_ALPHABET)
         super().__init__(temperature,
                          model, 
-                         tokenizer=tokenizer,
+                         tokenizer.get_vocab(),
                          device=device,
                          use_without_wildtype=use_without_wildtype)
         assert model.alphabet == self.alphabet, \
             f"EVcouplings alphabet {model.alphabet} should match our canonical alphabet {self.alphabet}"
-
+        self.tokenizer = tokenizer
+        
     def set_wt_score(self, wt_seq: str) -> None:
         """Sets the wildtype score value for protein wt_seq
         """
         encoded_inputs = self._tokenize([wt_seq])
         self._wt_score = self.model(encoded_inputs)
```

### Comparing `evo_prot_grad-0.1.3/evo_prot_grad/experts/onehot_downstream_regression_expert.py` & `evo_prot_grad-0.1.4/evo_prot_grad/experts/onehot_downstream_regression_expert.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.3/evo_prot_grad/models/downstream_cnn.py` & `evo_prot_grad-0.1.4/evo_prot_grad/models/downstream_cnn.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.3/evo_prot_grad/models/potts.py` & `evo_prot_grad-0.1.4/evo_prot_grad/models/potts.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.3/evo_prot_grad.egg-info/PKG-INFO` & `evo_prot_grad-0.1.4/evo_prot_grad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evo-prot-grad
-Version: 0.1.3
+Version: 0.1.4
 Summary: Directed evolution of proteins with fast gradient-based discrete MCMC.
 Home-page: https://github.nrel.gov/NREL/EvoProtGrad/
 Author: Patrick Emami
 Author-email: Patrick.Emami@nrel.gov
 License: BSD 3-Clause
 Keywords: protein engineering,directed evolution,huggingface,protein language models,mcmc
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `evo_prot_grad-0.1.3/evo_prot_grad.egg-info/SOURCES.txt` & `evo_prot_grad-0.1.4/evo_prot_grad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.3/setup.py` & `evo_prot_grad-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(name='evo_prot_grad',
-      version='0.1.3',
+      version='0.1.4',
       description='Directed evolution of proteins with fast gradient-based discrete MCMC.',
       author='Patrick Emami',
       author_email='Patrick.Emami@nrel.gov',
       url='https://github.nrel.gov/NREL/EvoProtGrad/',
       python_requires='>=3.8',
       install_requires=requirements,
       long_description=readme,
```

### Comparing `evo_prot_grad-0.1.3/test/test_experts.py` & `evo_prot_grad-0.1.4/test/test_experts.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.3/test/test_sampler.py` & `evo_prot_grad-0.1.4/test/test_sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest 
 from transformers import AutoModel
 from evo_prot_grad import get_expert
 from evo_prot_grad.common.sampler import DirectedEvolution
-
+import numpy as np
 
 class TestSampler(unittest.TestCase):
     
     def setUp(self):
         self.gfp_expert = get_expert(
             'onehot_downstream_regression',
             1.0,
@@ -127,14 +127,18 @@
             parallel_chains=2,
             n_steps=1,
             max_mutations=-1,
             output = 'best',
             wt_fasta='test/gfp.fasta'
         )()
         self.assertEqual(len(epg), 2)
+        variants, scores = epg
+        self.assertEqual(len(variants), 2)
+        self.assertEqual(len(scores), 2)
+        self.assertTrue(isinstance(scores[0], np.float32), "Score is not a float, {}".format(type(scores[0])))
 
         # Test 'last'
         epg = DirectedEvolution(
             experts=[self.gfp_expert],
             parallel_chains=2,
             n_steps=1,
             max_mutations=-1,
```

### Comparing `evo_prot_grad-0.1.3/test/test_utils.py` & `evo_prot_grad-0.1.4/test/test_utils.py`

 * *Files identical despite different names*

