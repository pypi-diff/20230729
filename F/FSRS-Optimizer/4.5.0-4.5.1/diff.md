# Comparing `tmp/FSRS-Optimizer-4.5.0.tar.gz` & `tmp/FSRS-Optimizer-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FSRS-Optimizer-4.5.0.tar", last modified: Sat Jul 29 08:35:18 2023, max compression
+gzip compressed data, was "FSRS-Optimizer-4.5.1.tar", last modified: Sat Jul 29 15:58:44 2023, max compression
```

## Comparing `FSRS-Optimizer-4.5.0.tar` & `FSRS-Optimizer-4.5.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:35:18.833123 FSRS-Optimizer-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-29 08:35:18.833123 FSRS-Optimizer-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-29 08:35:08.000000 FSRS-Optimizer-4.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-29 08:35:08.000000 FSRS-Optimizer-4.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 08:35:18.833123 FSRS-Optimizer-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-29 08:35:08.000000 FSRS-Optimizer-4.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:35:18.829123 FSRS-Optimizer-4.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:35:18.829123 FSRS-Optimizer-4.5.0/src/FSRS_Optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-29 08:35:18.000000 FSRS-Optimizer-4.5.0/src/FSRS_Optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-29 08:35:18.000000 FSRS-Optimizer-4.5.0/src/FSRS_Optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 08:35:18.000000 FSRS-Optimizer-4.5.0/src/FSRS_Optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-29 08:35:18.000000 FSRS-Optimizer-4.5.0/src/FSRS_Optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 08:35:18.000000 FSRS-Optimizer-4.5.0/src/FSRS_Optimizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:35:18.833123 FSRS-Optimizer-4.5.0/src/fsrs_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 08:35:08.000000 FSRS-Optimizer-4.5.0/src/fsrs_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-29 08:35:08.000000 FSRS-Optimizer-4.5.0/src/fsrs_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52099 2023-07-29 08:35:08.000000 FSRS-Optimizer-4.5.0/src/fsrs_optimizer/fsrs_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:58:44.036138 FSRS-Optimizer-4.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-29 15:58:32.000000 FSRS-Optimizer-4.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-29 15:58:44.036138 FSRS-Optimizer-4.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-29 15:58:32.000000 FSRS-Optimizer-4.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-29 15:58:32.000000 FSRS-Optimizer-4.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 15:58:44.036138 FSRS-Optimizer-4.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-29 15:58:32.000000 FSRS-Optimizer-4.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:58:44.036138 FSRS-Optimizer-4.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:58:44.036138 FSRS-Optimizer-4.5.1/src/FSRS_Optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-29 15:58:44.000000 FSRS-Optimizer-4.5.1/src/FSRS_Optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-29 15:58:44.000000 FSRS-Optimizer-4.5.1/src/FSRS_Optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 15:58:44.000000 FSRS-Optimizer-4.5.1/src/FSRS_Optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-29 15:58:44.000000 FSRS-Optimizer-4.5.1/src/FSRS_Optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 15:58:44.000000 FSRS-Optimizer-4.5.1/src/FSRS_Optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:58:44.036138 FSRS-Optimizer-4.5.1/src/fsrs_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 15:58:32.000000 FSRS-Optimizer-4.5.1/src/fsrs_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-29 15:58:32.000000 FSRS-Optimizer-4.5.1/src/fsrs_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52297 2023-07-29 15:58:32.000000 FSRS-Optimizer-4.5.1/src/fsrs_optimizer/fsrs_optimizer.py
```

### Comparing `FSRS-Optimizer-4.5.0/PKG-INFO` & `FSRS-Optimizer-4.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.5.0
+Version: 4.5.1
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # FSRS Optimizer
 
 The FSRS Optimizer is a Python library capable of utilizing personal spaced repetition review logs to refine the FSRS algorithm. Designed with the intent of delivering a standardized, universal optimizer to various FSRS implementations across numerous programming languages, this tool is set to establish a ubiquitous standard for spaced repetition review logs. By facilitating the uniformity of learning data among different spaced repetition softwares, it guarantees learners consistent review schedules across a multitude of platforms.
 
 Delve into the underlying principles of the FSRS Optimizer's training process at: https://github.com/open-spaced-repetition/fsrs4anki/wiki/The-mechanism-of-optimization
```

### Comparing `FSRS-Optimizer-4.5.0/README.md` & `FSRS-Optimizer-4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.5.0/src/FSRS_Optimizer.egg-info/PKG-INFO` & `FSRS-Optimizer-4.5.1/src/FSRS_Optimizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.5.0
+Version: 4.5.1
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # FSRS Optimizer
 
 The FSRS Optimizer is a Python library capable of utilizing personal spaced repetition review logs to refine the FSRS algorithm. Designed with the intent of delivering a standardized, universal optimizer to various FSRS implementations across numerous programming languages, this tool is set to establish a ubiquitous standard for spaced repetition review logs. By facilitating the uniformity of learning data among different spaced repetition softwares, it guarantees learners consistent review schedules across a multitude of platforms.
 
 Delve into the underlying principles of the FSRS Optimizer's training process at: https://github.com/open-spaced-repetition/fsrs4anki/wiki/The-mechanism-of-optimization
```

### Comparing `FSRS-Optimizer-4.5.0/src/fsrs_optimizer/__main__.py` & `FSRS-Optimizer-4.5.1/src/fsrs_optimizer/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,47 +44,51 @@
         if remembered_fallbacks["timezone"] not in pytz.all_timezones:
             raise Exception("Not a valid timezone, Check the list for more information")
 
         remembered_fallback_prompt("next_day", "used next day start hour")
         remembered_fallback_prompt("revlog_start_date", "the date at which before reviews will be ignored")
         remembered_fallback_prompt("filter_out_suspended_cards", "filter out suspended cards? (y/n)")
         
-        graphs_input = prompt("View graphs? (y/n)" , remembered_fallbacks["preview"])
+        graphs_input = prompt("Save graphs? (y/n)" , remembered_fallbacks["preview"])
     else:
         graphs_input = remembered_fallbacks["preview"]
 
     if graphs_input.lower() != 'y':
         remembered_fallbacks["preview"] = "n"
 
     with open(config_save, "w+") as f: # Save the settings to load next time the program is run
         json.dump(remembered_fallbacks, f)
 
-    show_graphs = graphs_input != "n"
+    save_graphs = graphs_input != "n"
 
     optimizer = fsrs_optimizer.Optimizer()
     optimizer.anki_extract(
         filename,
         remembered_fallbacks["filter_out_suspended_cards"] == "y"
     )
     analysis = optimizer.create_time_series(
         remembered_fallbacks["timezone"],
         remembered_fallbacks["revlog_start_date"],
         remembered_fallbacks["next_day"]
     )
     print(analysis)
 
     optimizer.define_model()
-    optimizer.pretrain(verbose=show_graphs)
-    optimizer.train(verbose=show_graphs)
+    figures = optimizer.pretrain(verbose=save_graphs)
+    for i, f in enumerate(figures):
+        f.savefig(f"pretrain_{i}.png")
+    figures = optimizer.train(verbose=save_graphs)
+    for i, f in enumerate(figures):
+        f.savefig(f"train_{i}.png")
 
     optimizer.predict_memory_states()
     figures = optimizer.find_optimal_retention()
-    if show_graphs:
-        for f in figures:
-            f.show()
+    if save_graphs:
+        for i, f in enumerate(figures):
+            f.savefig(f"find_optimal_retention_{i}.png")
 
     optimizer.preview(optimizer.optimal_retention)
 
     profile = \
     f"""{{
     // Generated, Optimized anki deck settings
     "deckName": "{os.path.splitext(os.path.basename(filename))[0]}",// PLEASE CHANGE THIS TO THE DECKS PROPER NAME
@@ -98,19 +102,19 @@
     print(profile)
 
     if args.out:
         with open(args.out, "a+") as f:
             f.write(profile)
 
     optimizer.evaluate()
-    if show_graphs:
-        for f in optimizer.calibration_graph():
-            f.show()
-        for f in optimizer.compare_with_sm2():
-            f.show()
+    if save_graphs:
+        for i, f in enumerate(optimizer.calibration_graph()):
+            f.savefig(f"calibration_{i}.png")
+        for i, f in enumerate(optimizer.compare_with_sm2()):
+            f.savefig(f"compare_with_sm2_{i}.png")
 
 if __name__ == "__main__":
 
     config_save = os.path.expanduser(".fsrs_optimizer")
 
     parser = argparse.ArgumentParser()
     parser.add_argument("filenames", nargs='+')
```

### Comparing `FSRS-Optimizer-4.5.0/src/fsrs_optimizer/fsrs_optimizer.py` & `FSRS-Optimizer-4.5.1/src/fsrs_optimizer/fsrs_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -492,14 +492,15 @@
         self.dataset = pd.read_csv("./revlog_history.tsv", sep='\t', index_col=None, dtype={'r_history': str ,'t_history': str} )
         self.dataset = self.dataset[(self.dataset['i'] > 1) & (self.dataset['delta_t'] > 0) & (self.dataset['t_history'].str.count(',0') == 0)]
         if self.dataset.empty:
             raise ValueError('Training data is inadequate.')
         rating_stability = {}
         rating_count = {}
         average_recall = self.dataset['y'].mean()
+        plots = []
 
         for first_rating in ("1", "2", "3", "4"):
             group = self.S0_dataset_group[self.S0_dataset_group['r_history'] == first_rating]
             if group.empty:
                 tqdm.write(f'Not enough data for first rating {first_rating}. Expected at least 100, got 0.')
                 continue
             delta_t = group['delta_t']
@@ -513,59 +514,63 @@
             stability = params[0]
             rating_stability[int(first_rating)] = stability
             rating_count[int(first_rating)] = total_count
             predict_recall = power_forgetting_curve(delta_t, *params)
             rmse = mean_squared_error(recall, predict_recall, sample_weight=count, squared=False)
 
             if verbose:
-                plt.plot(delta_t, recall, label='Exact')
-                plt.plot(np.linspace(0, 30), power_forgetting_curve(np.linspace(0, 30), *params), label=f'Weighted fit (RMSE: {rmse:.4f})')
+                fig = plt.figure()
+                ax = fig.gca()
+                ax.plot(delta_t, recall, label='Exact')
+                ax.plot(np.linspace(0, 30), power_forgetting_curve(np.linspace(0, 30), *params), label=f'Weighted fit (RMSE: {rmse:.4f})')
                 count_percent = np.array([x/total_count for x in count])
-                plt.scatter(delta_t, recall, s=count_percent * 1000, alpha=0.5)
-                plt.legend(loc='upper right', fancybox=True, shadow=False)
-                plt.grid(True)
-                plt.ylim(0, 1)
-                plt.xlim(0, 30)
-                plt.xlabel('Interval')
-                plt.ylabel('Recall')
-                plt.title(f'Forgetting curve for first rating {first_rating} (n={total_count}, s={stability:.2f})')
-                plt.show()
+                ax.scatter(delta_t, recall, s=count_percent * 1000, alpha=0.5)
+                ax.legend(loc='upper right', fancybox=True, shadow=False)
+                ax.grid(True)
+                ax.set_ylim(0, 1)
+                ax.set_xlim(0, 30)
+                ax.set_xlabel('Interval')
+                ax.set_ylabel('Recall')
+                ax.set_title(f'Forgetting curve for first rating {first_rating} (n={total_count}, s={stability:.2f})')
+                plots.append(fig)
                 tqdm.write(str(rating_stability))
 
         if len(rating_stability) == 0:
             raise Exception("Not enough data for pretraining!")
         elif len(rating_stability) == 1:
             init_stability = round(list(rating_stability.values())[0], 2)
             for i in (0, 1, 2, 3):
                 self.init_w[i] = init_stability
         elif len(rating_stability) == 4:
             for rating, stability in rating_stability.items():
                 self.init_w[rating-1] = round(stability, 2)
             tqdm.write(f"Pretrain finished!")
-            return
+            return plots
 
         def S0_rating_curve(rating, a, b, c):
             return np.exp(a + b * rating) + c
 
         params, covs = curve_fit(S0_rating_curve, list(rating_stability.keys()), list(rating_stability.values()), sigma=1/np.sqrt(list(rating_count.values())), method='dogbox', bounds=((-15, 0.03, -5), (15, 7, 30)))
         if verbose:
             tqdm.write(f'Weighted fit parameters: {params}')
             predict_stability = S0_rating_curve(np.array(list(rating_stability.keys())), *params)
             tqdm.write(f"Fit stability: {predict_stability}")
             tqdm.write(f'RMSE: {mean_squared_error(list(rating_stability.values()), predict_stability, sample_weight=list(rating_count.values()), squared=False):.4f}')
-            plt.plot(list(rating_stability.keys()), list(rating_stability.values()), label='Exact')
-            plt.plot(np.linspace(1, 4), S0_rating_curve(np.linspace(1, 4), *params), label='Weighted fit')
+            fig = plt.figure()
+            ax = fig.gca()
+            ax.plot(list(rating_stability.keys()), list(rating_stability.values()), label='Exact')
+            ax.plot(np.linspace(1, 4), S0_rating_curve(np.linspace(1, 4), *params), label='Weighted fit')
             scatter_size = np.array([x/sum(rating_count.values()) for x in rating_count.values()]) * 1000
-            plt.scatter(list(rating_stability.keys()), list(rating_stability.values()), scatter_size, label='Exact', alpha=0.5)
-            plt.legend(loc='upper right', fancybox=True, shadow=False)
-            plt.grid(True)
-            plt.xlabel('First rating')
-            plt.ylabel('Stability')
-            plt.title('Stability for first rating')
-            plt.show()
+            ax.scatter(list(rating_stability.keys()), list(rating_stability.values()), scatter_size, label='Exact', alpha=0.5)
+            ax.legend(loc='upper right', fancybox=True, shadow=False)
+            ax.grid(True)
+            ax.set_xlabel('First rating')
+            ax.set_ylabel('Stability')
+            ax.set_title('Stability for first rating')
+            plots.append(fig)
 
         for rating in (1, 2, 3, 4):
             again_extrap = max(min(S0_rating_curve(1, *params), 30), 0.1)
             # if there isn't enough data to calculate the value for "Again" exactly
             if 1 not in rating_stability:
                 # then check if there exists an exact value for "Hard"
                 if 2 in rating_stability:
@@ -583,14 +588,15 @@
             elif rating not in rating_stability:
                 rating_stability[rating] = max(min(S0_rating_curve(rating, *params), 30), 0.1)
 
         rating_stability = {k: round(v, 2) for k, v in sorted(rating_stability.items(), key=lambda item: item[0])}
         for rating, stability in rating_stability.items():
             self.init_w[rating-1] = stability
         tqdm.write(f"Pretrain finished!")
+        return plots
 
     def train(self, lr: float = 4e-2, n_epoch: int = 5, n_splits: int = 5, batch_size: int = 512, verbose: bool = True):
         """Step 4"""
         self.dataset['tensor'] = self.dataset.progress_apply(lambda x: lineToTensor(list(zip([x['t_history']], [x['r_history']]))[0]), axis=1)
         self.dataset['group'] = self.dataset['r_history'] + self.dataset['t_history']
         tqdm.write("Tensorized!")
```

