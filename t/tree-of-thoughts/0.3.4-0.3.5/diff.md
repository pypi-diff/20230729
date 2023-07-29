# Comparing `tmp/tree-of-thoughts-0.3.4.tar.gz` & `tmp/tree-of-thoughts-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.3.4.tar", last modified: Mon Jun  5 20:28:19 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.3.5.tar", last modified: Sat Jul 29 19:03:42 2023, max compression
```

## Comparing `tree-of-thoughts-0.3.4.tar` & `tree-of-thoughts-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:28:19.755589 tree-of-thoughts-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-05 20:28:19.755589 tree-of-thoughts-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15227 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 20:28:19.755589 tree-of-thoughts-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:28:19.755589 tree-of-thoughts-0.3.4/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/tree_of_thoughts/abstractLanguageModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/tree_of_thoughts/guidanceModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/tree_of_thoughts/huggingModels.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/tree_of_thoughts/openaiModels.py
--rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-06-05 20:28:10.000000 tree-of-thoughts-0.3.4/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:28:19.755589 tree-of-thoughts-0.3.4/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-05 20:28:19.000000 tree-of-thoughts-0.3.4/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-05 20:28:19.000000 tree-of-thoughts-0.3.4/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:28:19.000000 tree-of-thoughts-0.3.4/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 20:28:19.000000 tree-of-thoughts-0.3.4/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-05 20:28:19.000000 tree-of-thoughts-0.3.4/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:42.836820 tree-of-thoughts-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-29 19:03:42.836820 tree-of-thoughts-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19219 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 19:03:42.836820 tree-of-thoughts-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:42.832820 tree-of-thoughts-0.3.5/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/abstract_language_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/guidance_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/huggingface_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/langchain_tot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/openai_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/text_generation_web_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23217 2023-07-29 19:03:30.000000 tree-of-thoughts-0.3.5/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:42.836820 tree-of-thoughts-0.3.5/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-29 19:03:42.000000 tree-of-thoughts-0.3.5/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-29 19:03:42.000000 tree-of-thoughts-0.3.5/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 19:03:42.000000 tree-of-thoughts-0.3.5/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 19:03:42.000000 tree-of-thoughts-0.3.5/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 19:03:42.000000 tree-of-thoughts-0.3.5/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.3.4/LICENSE` & `tree-of-thoughts-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.3.4/PKG-INFO` & `tree-of-thoughts-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.3.4
+Version: 0.3.5
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.3.4/README.md` & `tree-of-thoughts-0.3.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,161 +1,144 @@
-# Agora
-This implementation of Tree of Thoughts is brought to you by Agora, Agora advances Humanity with open source SOTA Multi-Modality AI research!
-
-
-![Agora banner](agora-banner.png)
-
-[Join our Discord and contribute to this project](https://discord.gg/qUtxnK2NMf)
-
 # Tree of Thoughts 🌳🌲🌴🌿🍃
 
-![tree of thoughts banner](tree-of-thoughts.png)
+![Discord](https://img.shields.io/discord/999382051935506503)
+[![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20project%20on%20improving%20AI%20reasoning%20-%20Tree%20of%20Thoughts!%20https://github.com/kyegomez/tree-of-thoughts)
+[![LinkedIn](https://img.shields.io/badge/Share-LinkedIn-blue?style=social&logo=linkedin)](https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)
+[![Facebook](https://img.shields.io/badge/Share-Facebook-blue?style=social&logo=facebook)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)
+[![Reddit](https://img.shields.io/badge/Share-Reddit-orange?style=social&logo=reddit)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts&title=Check%20out%20this%20amazing%20project%20on%20improving%20AI%20reasoning%20-%20Tree%20of%20Thoughts%21)
+[![Hacker News](https://img.shields.io/badge/Share-Hacker%20News-orange?style=social&logo=y-combinator)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts&t=Check%20out%20this%20amazing%20project%20on%20improving%20AI%20reasoning%20-%20Tree%20of%20Thoughts%21)
+[![Pinterest](https://img.shields.io/badge/Share-Pinterest-red?style=social&logo=pinterest)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts&media=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts%2Fraw%2Fmain%2Ftree-of-thoughts.jpeg&description=Check%20out%20this%20amazing%20project%20on%20improving%20AI%20reasoning%20-%20Tree%20of%20Thoughts%21)
+[![WhatsApp](https://img.shields.io/badge/Share-WhatsApp-green?style=social&logo=whatsapp)](https://api.whatsapp.com/send?text=Check%20out%20this%20amazing%20project%20on%20improving%20AI%20reasoning%20-%20Tree%20of%20Thoughts%21%20https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)
 
-[Paper link](https://arxiv.org/pdf/2305.10601.pdf)
+![Tree of Thoughts Banner](tree-of-thoughts.png)
 
-Tree of Thoughts (ToT) is an all-new powerful and flexible algorithm that advances model reasoning by a whopping 70%. This is an plug in and play verision, connect your own models and enjoy superintelligence!
+[Paper link](https://arxiv.org/pdf/2305.10601.pdf)
 
-## 🔥 All-New Search Algorithms
+## Introduction
 
-* MonteCarlo
+Tree of Thoughts (ToT) is a powerful and flexible algorithm that significantly advances model reasoning by up to 70%. This plug-and-play version allows you to connect your own models and experience superintelligence!
 
-* A* Search 
+## 🔥 Updates
 
-* Best First Search
+- Langchain TOT
+- MonteCarlo
+- A* Search
+- Best First Search
 
 #### Coming soon!
-* Iterative Depth Search 
-
-* Any search algorithms you like?? Open an issue 😊 
 
+- Iterative Depth Search
+- Any search algorithms you like? Open an issue 😊
 
-Help cultivate this repository to democratize superintelligence! Share this repository by clicking on the following buttons 😊 
+## Basic Prompts
 
-[![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20project%20on%20improving%20AI%20reasoning%20-%20Tree%20of%20Thoughts!%20https://github.com/kyegomez/tree-of-thoughts)
-[![LinkedIn](https://img.shields.io/badge/Share-LinkedIn-blue?style=social&logo=linkedin)](https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)
+No complex implementations, just pass in one of these prompts to your model. Head over to `prompts.txt`.
 
+"Three experts with exceptional logical thinking skills are collaboratively answering a question using the tree of thoughts method. Each expert will share their thought process in detail, taking into account the previous thoughts of others and admitting any errors. They will iteratively refine and expand upon each other's ideas, giving credit where it's due. The process continues until a conclusive answer is found. Organize the entire response in a markdown table format. The question is..."
 
+## Getting Started
 
-# Basic Prompts:
-No complex implementations, just pass in one of these prompts to your model: head over to `prompts.txt`
+### Method 1
 
-'Three experts with exceptional logical thinking skills are collaboratively answering a question using a tree of thoughts method. Each expert will share their thought process in detail, taking into account the previous thoughts of others and admitting any errors. They will iteratively refine and expand upon each other's ideas, giving credit where it's due. The process continues until a conclusive answer is found. Organize the entire response in a markdown table format. The question is...'
+Clone this repository:
 
-## Getting started
-Set Openai key in an environment file,
-
-first create an file called: `.env` 
-
-Then get your openai key and input it inside the '' as `OPENAI_API_KEY='SK-YOUR KEY'`
-
-
-## Method1
-Clone this repository with 
-
-```git clone https://github.com/kyegomez/tree-of-thoughts```
-
-``` 
+```bash
+git clone https://github.com/kyegomez/tree-of-thoughts
 cd tree-of-thoughts
 python3 -m pip install -r requirements.txt
 cd tree_of_thoughts
 ```
-Then go to `montecarlo_example.py` and fill in your api key! 
 
-# 🔥 For much improved performance provide custom few prompt shots in the generate thoughts and generate states 🔥 
+Set OpenAI key in an environment file:
+
+1. Create a file called `.env`.
+2. Get your OpenAI key and input it inside the `.env` file as `OPENAI_API_KEY='SK-YOUR KEY'`.
+
+Then go to `montecarlo_example.py` and fill in your API key!
+
+#### For much improved performance, provide custom prompt shots in the generate thoughts and generate states.
 
-And in the `examples` folder we have other examples for huggingface transformers + hugginggface pipelines
+In the `examples` folder, we have other examples for Hugging Face Transformers + Hugging Face Pipelines.
 
-## Method2
-or:
+### Method 2
 
-```pip install tree-of-thoughts ```
+Alternatively, you can use pip to install Tree of Thoughts:
 
+```bash
+pip install tree-of-thoughts
+```
 
 Create a Python script (e.g., example.py) and import the necessary classes:
 
-``` python
+```python
 import os
 from tree_of_thoughts import OpenAILanguageModel
 from tree_of_thoughts import MonteCarloTreeofThoughts
 
-
-api_model= "gpt-3.5-turbo"
-
-
+api_model = "gpt-3.5-turbo"
 model = OpenAILanguageModel(api_key='api key', api_model=api_model)
 
-
 # Initialize the MonteCarloTreeofThoughts class with the model
 tree_of_thoughts = MonteCarloTreeofThoughts(model)
 
-# Note to reproduce the same results from the tree of thoughts paper if not better, 
-# craft an 1 shot chain of thought prompt for your task below
+# To reproduce the same results from the Tree of Thoughts paper, or even better,
+# craft a one-shot chain of thought prompt for your task below:
 
 initial_prompt =  """
-
-
 Input: 2 8 8 14
 Possible next steps:
 2 + 8 = 10 (left: 8 10 14)
 8 / 2 = 4 (left: 4 8 14)
 14 + 2 = 16 (left: 8 8 16)
 2 * 8 = 16 (left: 8 14 16)
 8 - 2 = 6 (left: 6 8 14)
 14 - 8 = 6 (left: 2 6 8)
 14 /  2 = 7 (left: 7 8 8)
 14 - 2 = 12 (left: 8 8 12)
 Input: use 4 numbers and basic arithmetic operations (+-*/) to obtain 24 in 1 equation
-Possible next steps:
-
 
 
+Possible next steps:
 """
 num_thoughts = 1
 max_steps = 3
 max_states = 4
 pruning_threshold = 0.5
 
-
-
-
 solution = tree_of_thoughts.solve(
     initial_prompt=initial_prompt,
     num_thoughts=num_thoughts, 
     max_steps=max_steps, 
     max_states=max_states, 
     pruning_threshold=pruning_threshold,
-    # sleep_time=sleep_time
 )
 
 print(f"Solution: {solution}")
-
 ```
 
-Or Integrate your own custom language model:
+Or integrate your own custom language model:
 
 ```python
-
 class CustomLanguageModel(AbstractLanguageModel):
     def __init__(self, model):
         self.model = model
 
     def generate_thoughts(self, state, k):
-        #implement the thought generation logic using self.model
+        # implement the thought generation logic using self.model
         pass
 
     def evaluate_states(self, states):
-        #implement state evaluation logic using self.model
+        # implement state evaluation logic using self.model
         pass
-
 ```
 
-
-Run the example script
+Run the example script.
 
 ## 🌟 Features:
+
 - General problem-solving framework for language models
 - Supports both breadth-first search (BFS) and depth-first search (DFS) algorithms
 - Easy integration with popular language models like OpenAI and Hugging Face
 - Extensible and adaptable to different problem properties and resource constraints
 
 ## Algorithmic Pseudocode
 
@@ -166,41 +149,39 @@
 3. Create a state evaluator function V(pθ, S) with two strategies:
    a. Value each state independently.
    b. Vote across states.
 4. Choose a search algorithm (BFS or DFS) based on the tree structure.
 5. Implement the chosen search algorithm.
 6. Execute the chosen search algorithm with the input problem, thought generator, state evaluator, and other required parameters.
 
-
 ## Usage Examples
 
 ### OpenAI API
 
 To use Tree of Thoughts with OpenAI's API, create a custom model class that inherits from `AbstractLanguageModel` and implements the required methods using OpenAI's API. Then, create an instance of the `TreeOfThoughts` class with the custom model and the desired search algorithm ('BFS' or 'DFS').
 
 ### Hugging Face Transformers
-To run huggingface transformers with Tree of Thoughts
 
-``` 
+To run Hugging Face Transformers with Tree of Thoughts:
+
+```bash
 git clone https://github.com/kyegomez/tree-of-thoughts
 cd tree-of-thoughts
 python3 huggingfaceExample.py
 ```
 
 ```python
 from tree_of_thoughts import HuggingLanguageModel
 
-model_name="gpt2"
-model_tokenizer="your tokenizer"
+model_name = "gpt2"
+model_tokenizer = "your tokenizer"
 
 huggingface_model = HuggingLanguageModel(model_name, model_tokenizer)
 ```
 
-
-
 ```python
 class HuggingLanguageModel(AbstractLanguageModel):
     def __init__(self, model_name):
         self.model = AutoModelForCausalLM.from_pretrained(model_name)
         self.tokenizer = AutoTokenizer.from_pretrained(model_name)
 
     def generate_thoughts(self, state, k):
@@ -213,15 +194,15 @@
 
         return thoughts
 
     def evaluate_states(self, states, initial_prompt):
         state_values = {}
         for state in states:
             state_text = ' '.join(state)
-            prompt = f"Given the current state of reasoning: '{state_text}', pessimitically evaluate its value as a float between 0 and 1 based on it's potential to achieve {initial_prompt}"
+            prompt = f"Given the current state of reasoning: '{state_text}', pessimistically evaluate its value as a float between 0 and 1 based on its potential to achieve {initial_prompt}"
 
             inputs = self.tokenizer(prompt, return_tensors="pt")
             outputs = self.model.generate(**inputs, num_return_sequences=1)
             value_text = self.tokenizer.decode(outputs[0], skip_special_tokens=True)
 
             try:
                 value = float(value_text)
@@ -231,50 +212,44 @@
             state_values[state] = value
 
         return state_values
 
 
 ```
 
+## Contributing
 
-# Contributing
-This algorithm is still infant yet it's potential remains unimaginable, let's advance the reasoning of AI's together under this banner.
+This algorithm is still in its infancy, but its potential remains unimaginable. Let's advance the reasoning of AI together under this banner.
 
 # Share With Your Network
 
 You can easily share this repository by clicking on the following buttons:
 
 [![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20project%20on%20improving%20AI%20reasoning%20-%20Tree%20of%20Thoughts!%20https://github.com/kyegomez/tree-of-thoughts)
 [![LinkedIn](https://img.shields.io/badge/Share-LinkedIn-blue?style=social&logo=linkedin)](https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)
 
-For Instagram, while it doesn't directly support sharing of web links, you can share the screenshot of our project and the link in your caption or bio. You can download the project screenshot by clicking the image below:
+For Instagram, while it doesn't directly support sharing web links, you can share the screenshot of our project and the link in your caption or bio. You can download the project screenshot by clicking the image below:
 
 [![Tree of Thoughts](https://github.com/kyegomez/tree-of-thoughts/raw/main/tree-of-thoughts.jpeg)](https://github.com/kyegomez/tree-of-thoughts/raw/main/tree-of-thoughts.jpeg)
 
 We greatly appreciate any help in spreading the word about our project. Thank you for your support!
 
-# Roadmap:
-
-* Resilient Prompting: Teach model how to think rather than what to think.
-
-* Add pruning treshold management for precise bad state cutoff
-
-* Evaluating each thought as soon as thought generated then evaluating an chain of thoughts or the state of thoughts by averaging out the values of each thought evaluation.
-
-* Add Traversal method, which "will incapsulate the run of either dfs or bfs under the hood so that the issue of different args is solved from @ivanzhovannik
+# Roadmap
 
-* Add Delay between generate solutions and generate values
+- Resilient Prompting: Teach model how to think rather than what to think.
+- Add pruning threshold management for precise bad state cutoff.
+- Evaluating each thought as soon as it's generated, then evaluating a chain of thoughts or the state of thoughts by averaging out the values of each thought evaluation.
+- Add Traversal method, which will encapsulate the run of either DFS or BFS under the hood so that the issue of different args is solved (from @ivanzhovannik).
+- Add Delay between generating solutions and generating values.
+- Dynamic and adaptive parameters like max steps, num_thoughts, max_states, and value threshold that shift depending on the complexity of the user objective.
+- Add Rejected reasoning metadata (thought, state, reasoning_on_state) into generate solutions.
+- And more! Feel free to suggest any other ideas. This algorithm is very young, and its potential is limitless.
+- Chain of Thought Hub Evaluation tests!
 
-* Dynamic and adaptive parameters, like max steps, num_thoughts, max_states and value threshold that shift depending on the complexity of the user objective.
-
-* Add Rejected reasoning metadata (thought, state, reasoning_on_state) into  generate solutions
-
-* any other ideas? Please pr request this algorithm is very infant and it's potential is limitless
-
-* Chain of Thought Hub Evaluation tests!
+----
 
 # Documentation:
 # Search Algorithms in Tree of Thoughts 
 
 The Tree of Thoughts library supports a variety of search algorithms that can be employed for different problem-solving contexts. Here's a brief overview of each search algorithm along with their primary benefits and use-cases.
 
 ## 1. Breadth-First Search (BFS)
@@ -353,12 +328,77 @@
 The branching factor of the search tree, which determines the maximum number of child nodes for each parent node.
 A higher value of b allows the algorithm to explore more states, potentially leading to better solutions. However, increasing b may also increase the computational complexity and time required to find a solution.
 
 ## value_threshold (float, default=0.5): 
 The value threshold for pruning states. 
 States with a value below this threshold will be discarded, reducing the search space. A higher value of vth will result in a more aggressive pruning strategy, potentially speeding up the search process. However, setting vth too high may cause the algorithm to discard promising states, leading to suboptimal solutions.
 
+
+## LangchainTOT class
+
+`LangchainTOT` is the main class you'll interact with. It acts as a wrapper for the Large Language Model and allows you to set a problem description, add thoughts, and check the validity of these thoughts using a specified checker.
+
+### Initialization
+
+You initialize a `LangchainTOT` object with an optional problem description and a checker class:
+
+```python
+problem_description = """
+3,*,*,2|1,*,3,*|*,1,*,3|4,*,*,1
+- This is a 4x4 Sudoku puzzle.
+- The * represents a cell to be filled.
+- The | character separates rows.
+- At each step, replace one or more * with digits 1-4.
+- There must be no duplicate digits in any row, column or 2x2 subgrid.
+- Keep the known digits from previous valid thoughts in place.
+- Each thought can be a partial or the final solution.
+""".strip()
+
+langchain_tot = LangchainTOT(problem_description=problem_description, checker_class=lambda: my_checker)
+```
+
+If you want to change the problem description or checker class later, you can use the `set_problem_description` and `set_checker_class` methods.
+
+### Adding thoughts
+
+Once you have your `LangchainTOT` object, you can add thoughts to it. A thought is a string representing a possible solution or step towards a solution. You can add thoughts using the `add_thought` method:
+
+```python
+langchain_tot.add_thought("3,*,*,2|1,*,3,*|*,1,*,3|4,*,*,1")
+```
+
+### Checking thoughts
+
+Once you've added one or more thoughts, you can check their validity using the `check_thoughts` method:
+
+```python
+print(langchain_tot.check_thoughts())
+```
+
+This method will return a `ThoughtValidity` value representing whether the latest thought is a final valid solution (`VALID_FINAL`), an intermediate valid step (`VALID_INTERMEDIATE`), or invalid (`INVALID`).
+
+## MyChecker class
+
+`MyChecker` is a class for creating custom checkers. It inherits from `ToTChecker` and must implement the `evaluate` method.
+
+### Initialization
+
+You initialize a `MyChecker` object with a validation function:
+
+```python
+my_checker = MyChecker(validate_fn=lambda p, t: validate_sudoku(p, t, sudoku_solution))
+```
+
+## Custom validation function
+
+The validation function is a callable that takes a problem description and a tuple of thoughts and returns a `ThoughtValidity` value. It defines how to check the validity of thoughts for a specific problem.
+
+In this code, we're using the `validate_sudoku` function as our validation function. This function takes a problem description, a tuple of thoughts, and a solution string, and returns the validity of the last thought based on whether it matches the solution and whether it's a possible step towards the solution.
+
+The `validate_sudoku` function is specific to 4x4 Sudoku puzzles and you'll need to create your own validation function for different types of problems.
+
+
 # Acknowledgements
 
 Thanks to: Shunyu Yao Princeton University, Dian Yu Google DeepMind, Jeffrey Zhao, Google DeepMind, Izhak Shafran Google DeepMind, Thomas L. Griffiths, Princeton University, Yuan Cao Google DeepMind, Karthik Narasimha, Princeton University for sharing this amazing work with the world!
 
 And, thanks to Phil Wang or Lucidrains for inspiring me to devote myself to open source AI Research
```

### Comparing `tree-of-thoughts-0.3.4/setup.py` & `tree-of-thoughts-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.3.4',
+  version = '0.3.5',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
```

### Comparing `tree-of-thoughts-0.3.4/tree_of_thoughts/guidanceModels.py` & `tree-of-thoughts-0.3.5/tree_of_thoughts/guidance_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import guidance
-from tree_of_thoughts.abstractLanguageModel import AbstractLanguageModel
+from tree_of_thoughts.abstract_language_model import AbstractLanguageModel
 import time
 import os
 import openai
 
 
 class GuidanceLanguageModel(AbstractLanguageModel):
     def __init__(self, model, strategy="cot", evaluation_strategy="value", enable_ReAct_prompting=False):
@@ -120,29 +120,29 @@
         else:
             raise ValueError("Invalid evaluation strategy. Choose 'value' or 'vote'.")
         
 
 
 class GuidanceOpenAILanguageModel(GuidanceLanguageModel):
     def __init__(self, api_key, strategy="cot", evaluation_strategy="value", api_base="", api_model="", enable_ReAct_prompting=False):
-        if api_key == "" or api_key == None:
+        if api_key == "" or api_key is None:
             api_key = os.environ.get("OPENAI_API_KEY", "")
         if api_key != "":
             openai.api_key = api_key
         else:
             raise Exception("Please provide OpenAI API key")
 
-        if api_base == ""or api_base == None:
+        if api_base == ""or api_base is None:
             api_base = os.environ.get("OPENAI_API_BASE", "")  # if not set, use the default base path of "https://api.openai.com/v1"
         if api_base != "":
             # e.g. https://api.openai.com/v1/ or your custom url
             openai.api_base = api_base
             print(f'Using custom api_base {api_base}')
             
-        if api_model == "" or api_model == None:
+        if api_model == "" or api_model is None:
             api_model = os.environ.get("OPENAI_API_MODEL", "")
         if api_model != "":
             self.api_model = api_model
         else:
             self.api_model = "text-davinci-003"
         print(f'Using api_model {self.api_model}')
```

### Comparing `tree-of-thoughts-0.3.4/tree_of_thoughts/huggingModels.py` & `tree-of-thoughts-0.3.5/tree_of_thoughts/huggingface_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from transformers import AutoModelForCausalLM, AutoTokenizer
 from transformers import pipeline
-from tree_of_thoughts.abstractLanguageModel import AbstractLanguageModel
+from tree_of_thoughts.abstract_language_model import AbstractLanguageModel
 
 
 class HuggingLanguageModel(AbstractLanguageModel):
     def __init__(self, model_name, model_tokenizer=None, verbose=False):
         self.model = AutoModelForCausalLM.from_pretrained(model_name)
         self.tokenizer = AutoTokenizer.from_pretrained(model_tokenizer or model_name)
         self.verbose = verbose
```

### Comparing `tree-of-thoughts-0.3.4/tree_of_thoughts/openaiModels.py` & `tree-of-thoughts-0.3.5/tree_of_thoughts/openai_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import os
 import openai
 import time
-from  tree_of_thoughts.abstractLanguageModel import AbstractLanguageModel
+from  tree_of_thoughts.abstract_language_model import AbstractLanguageModel
 import concurrent.futures
 import logging 
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
 
 
 class OpenAILanguageModel(AbstractLanguageModel):
     def __init__(self, api_key, strategy="cot", evaluation_strategy="value", api_base="", api_model="", enable_ReAct_prompting=True):
-        if api_key == "" or api_key == None:
+        if api_key == "" or api_key is None:
             api_key = os.environ.get("OPENAI_API_KEY", "")
         if api_key != "":
             openai.api_key = api_key
         else:
             raise Exception("Please provide OpenAI API key")
 
-        if api_base == ""or api_base == None:
+        if api_base == ""or api_base is None:
             api_base = os.environ.get("OPENAI_API_BASE", "")  # if not set, use the default base path of "https://api.openai.com/v1"
         if api_base != "":
             # e.g. https://api.openai.com/v1/ or your custom url
             openai.api_base = api_base
             print(f'Using custom api_base {api_base}')
             
-        if api_model == "" or api_model == None:
+        if api_model == "" or api_model is None:
             api_model = os.environ.get("OPENAI_API_MODEL", "")
         if api_model != "":
             self.api_model = api_model
         else:
             self.api_model = "text-davinci-003"
         print(f'Using api_model {self.api_model}')
```

### Comparing `tree-of-thoughts-0.3.4/tree_of_thoughts/treeofthoughts.py` & `tree-of-thoughts-0.3.5/tree_of_thoughts/treeofthoughts.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 #thought -> evaluated value (0.4, This solution is invalid because x) -> thought prompt + this solution is invalid because + better eval
 
+import json
 import os
 import time
-import json
+
 DATA_PATH = './data'
-import logging 
-import argparse
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
-logger = logging.getLogger(__name__)
-from typing import Any, Dict, Union
-import re
-import numpy as np
+import logging
+
+
 import concurrent.futures
 from queue import PriorityQueue
+from typing import Any, Dict, Union
 
+import numpy as np
+from abstractLanguageModel import AbstractLanguageModel
 
+from tree_of_thoughts.text_generation_web_ui import (
+    build_text_generation_web_ui_client_llm,
+    ui_default_parameters,
+)
 
 
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+logger = logging.getLogger(__name__)
+
 
 class TreeofThoughts:
     def __init__(self, model):
         self.model = model
         self.tree: Dict[str, Dict[str, Union[float, Dict[str, Any]]]] = {
             "nodes": {},
         }
@@ -260,15 +267,15 @@
     def reconstruct_path(self, came_from, current_state, initial_prompt):
         path = [current_state]
         while current_state in came_from:
             current_state = came_from[current_state]
             path.append(current_state)
         path.reverse()
 
-        path = self.reconstruct_path(came_from, current_state)
+        path = self.reconstruct_path(came_from, current_state, initial_prompt)
         solution = self.model.generate_solution(initial_prompt, path)
         print(f"Path: {path} solution: {solution}")
         return solution if solution else path
 
 
 class MonteCarloTreeofThoughts(TreeofThoughts):
     def __init__(self, model, objective="balance"):
@@ -306,15 +313,15 @@
               initial_prompt: str,
               num_thoughts: int,
               max_steps: int,
               max_states: int,
               pruning_threshold: float,
             #   sleep_time: float,
               ):
-        self.file_name = f"logs/tree_of_thoughts_output_montecarlo.json"
+        self.file_name = "logs/tree_of_thoughts_output_montecarlo.json"
         return self.monte_carlo_search(
             initial_prompt,
             num_thoughts,
             max_steps,
             max_states,
             pruning_threshold,
             # sleep_time,
@@ -336,15 +343,15 @@
         best_value = float('-inf')
 
         for step in range(1, max_steps + 1):
             selected_states = []
 
             for state in current_states:
                 if state in transposition_table:
-                    state_value = transposition_table[state]
+                    transposition_table[state]
                 else:
                     time.sleep(1)
                     thoughts = self.model.generate_thoughts(state, num_thoughts, initial_prompt)
                     time.sleep(1)
                     evaluated_thoughts = self.model.evaluate_states(thoughts, initial_prompt)
 
                     for thought, value in evaluated_thoughts.items():
@@ -381,27 +388,123 @@
         # else:
         #     solution = None
 
         # return None
         solution = self.model.generate_solution(initial_prompt, best_state)
         return solution if solution else best_state
 
-#does not output state after each thought --- idk why -- needs work
-class OptimizedTreeofThoughts(TreeofThoughts):
-    def solve(self, x, k=None, T=None, b=None, vth=None, timeout=None, confidence_threshold=None, max_iterations=None, convergence_threshold=None, convergence_count=None):
-        start_time = time.time()
-        print(f'Start time {start_time}')
-        if self.search_algorithm == 'BFS':
-            while timeout is None or time.time() - start_time < timeout:
-                result = self.tot_bfs(x, k, T, b, pruning_threshold=0.5)
-                print(f'result in optimized tree of thoughts: {result}')
-                if result:
-                    return result
-        elif self.search_algorithm == 'DFS':
-            while timeout is None or time.time() - start_time < timeout:
-                result = self.tot_dfs(x, k, T, vth, confidence_threshold=confidence_threshold, max_iterations=max_iterations, convergence_threshold=convergence_threshold, convergence_count=convergence_count)
-                if result:
-                    return result
-        else:
-            raise ValueError("Invalid search algorithm. Choose 'BFS' or 'DFS'.")
+# #does not output state after each thought --- idk why -- needs work
+# class OptimizedTreeofThoughts(TreeofThoughts):
+#     def solve(self, x, k=None, T=None, b=None, vth=None, timeout=None, confidence_threshold=None, max_iterations=None, convergence_threshold=None, convergence_count=None):
+#         start_time = time.time()
+#         print(f'Start time {start_time}')
+#         if self.search_algorithm == 'BFS':
+#             while timeout is None or time.time() - start_time < timeout:
+#                 result = self.tot_bfs(x, k, T, b, pruning_threshold=0.5)
+#                 print(f'result in optimized tree of thoughts: {result}')
+#                 if result:
+#                     return result
+#         elif self.search_algorithm == 'DFS':
+#             while timeout is None or time.time() - start_time < timeout:
+#                 result = self.tot_dfs(x, k, T, vth, confidence_threshold=confidence_threshold, max_iterations=max_iterations, convergence_threshold=convergence_threshold, convergence_count=convergence_count)
+#                 if result:
+#                     return result
+#         else:
+#             raise ValueError("Invalid search algorithm. Choose 'BFS' or 'DFS'.")
+
+
+class TextGenerationWebUILanguageModel(AbstractLanguageModel):
+    def __init__(self, strategy="cot", evaluation_strategy="value"):
+        thought_generator_params = ui_default_parameters()
+        thought_generator_params["max_new_tokens"] = 50
+        thought_generator_params["temperature"] = 0.5
+        self.thought_generator = build_text_generation_web_ui_client_llm(parameters=thought_generator_params)
+
+        state_voter_params = ui_default_parameters()
+        state_voter_params["max_new_tokens"] = 10
+        state_voter_params["temperature"] = 0.2
+        self.state_voter = build_text_generation_web_ui_client_llm(parameters=state_voter_params)  
+
+        value_evaluator_params = ui_default_parameters()
+        value_evaluator_params["max_new_tokens"] = 10
+        value_evaluator_params["temperature"] = 0.2
+        self.value_evaluator = build_text_generation_web_ui_client_llm(parameters=value_evaluator_params)
+
+
+        self.strategy = strategy
+        self.evaluation_strategy = evaluation_strategy
+
+    def generate_thoughts(self, state, k, initial_prompt, rejected_solutions=None):
+        if self.strategy == "cot":
+            if (type(state) == str):
+                state_text = state
+            else:
+                state_text = '\n'.join(state)
+            print("New state generating thought:", state, "\n\n")
+            # prompt = f"Considering the thoughts you've had until now:\n\n{state_text}\n\nDevise the next coherent thought that will aid in advancing the reasoning process and achieving a solution to {initial_prompt}. Assess various scenarios, think unconventionally, anticipate potential challenges, and resolve any outstanding queries. Tap into your mind's full potential and make certain no open questions remain."
+            prompt = f"""You're an TreeofThoughts, an superintelligent AI model devoted to helping Humans by any means necessary. You're purpose is to generate a series of solutions to comply with the user's instructions, you must generate solutions on the basis of determining the most reliable solution in the shortest amount of time, while taking rejected solutions into account and learning from them. 
+            Considering the reasoning provided:\n\n
+            ###'{state_text}'\n\n###
+            Devise the best possible solution for the task: {initial_prompt}, Here are evaluated solutions that were rejected: 
+            ###{rejected_solutions}###, 
+            complete the {initial_prompt} without making the same mistakes you did with the evaluated rejected solutions. Be simple. Be direct. Provide intuitive solutions as soon as you think of them."""
+            
+            prompt += self.ReAct_prompt
+            # print(prompt)
+            thoughts = self.generate_text(prompt, k)
+            # print(thoughts)
+            # print(f"Generated thoughts: {thoughts}")
+            return thoughts
+
+    def evaluate_states(self, states, initial_prompt):
+        if not states:
+            return {}
+
+        if self.evaluation_strategy == 'value':
+            state_values = {}
+            for state in states:
+                if (type(state) == str):
+                    state_text = state
+                else:
+                    state_text = '\n'.join(state)
+                print("We receive a state of type", type(state), "For state: ", state, "\n\n")
+                # prompt = f"Given the current state of reasoning: '{state_text}', evaluate its value as a float between 0 and 1, become very pessimistic think of potential adverse risks on the probability of this state of reasoning achieveing {initial_prompt} and DO NOT RESPOND WITH ANYTHING ELSE: OTHER THAN AN FLOAT"
+                prompt = f""" To achieve the following goal: '{initial_prompt}', pessimistically value the context of the past solutions and more importantly the latest generated solution you had AS A FLOAT BETWEEN 0 AND 1\n
+                    Past solutions:\n\n
+                    {state_text}\n       
+                    If the solutions is not directly concretely making fast progress in achieving the goal, give it a lower score.
+                    Evaluate all solutions AS A FLOAT BETWEEN 0 and 1:\n,  DO NOT RETURN ANYTHING ELSE
+                """
+                # and then inside backticks provide an simple and direct bulletpoint list as to why you evaluated this thought the way you did. Provide simple yet intuitive feedback.
+                
+                response = self.openai_api_call_handler(prompt, 10, 1)
+                try:
+                    value_text = self.openai_choice2text_handler(response.choices[0])
+                    # print(f'state: {value_text}')
+                    value = float(value_text)
+                    print(f"Evaluated Thought Value: {value}")
+                except ValueError:
+                    value = 0  # Assign a default value if the conversion fails
+                state_values[state] = value
+            return state_values
+
+        elif self.evaluation_strategy == 'vote':
+            states_text = '\n'.join([' '.join(state) for state in states])
+
+            prompt = f"Given the following states of reasoning, vote for the best state utilizing an scalar value 1-10:\n{states_text}\n\nVote, on the probability of this state of reasoning achieveing {initial_prompt} and become very pessimistic very NOTHING ELSE"
+
+            response = self.openai_api_call_handler(prompt, 50, 1)
+
+            print(f'state response: {response}')
+
+            best_state_text = self.openai_choice2text_handler(response.choices[0])
+
+            print(f"Best state text: {best_state_text}")
+
+            best_state = tuple(best_state_text.split())
 
+            print(f'best_state: {best_state}')
 
+            return {state: 1 if state == best_state else 0 for state in states}
+
+        else:
+            raise ValueError("Invalid evaluation strategy. Choose 'value' or 'vote'.")
```

### Comparing `tree-of-thoughts-0.3.4/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.3.5/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.3.4
+Version: 0.3.5
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

