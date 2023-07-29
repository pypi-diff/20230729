# Comparing `tmp/FSRS-Optimizer-4.4.2.tar.gz` & `tmp/FSRS-Optimizer-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FSRS-Optimizer-4.4.2.tar", last modified: Fri Jul 28 18:00:40 2023, max compression
+gzip compressed data, was "FSRS-Optimizer-4.5.0.tar", last modified: Sat Jul 29 08:35:18 2023, max compression
```

## Comparing `FSRS-Optimizer-4.4.2.tar` & `FSRS-Optimizer-4.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:00:40.152486 FSRS-Optimizer-4.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-28 18:00:40.152486 FSRS-Optimizer-4.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-28 18:00:29.000000 FSRS-Optimizer-4.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-28 18:00:29.000000 FSRS-Optimizer-4.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:00:40.152486 FSRS-Optimizer-4.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 18:00:29.000000 FSRS-Optimizer-4.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:00:40.148486 FSRS-Optimizer-4.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:00:40.152486 FSRS-Optimizer-4.4.2/src/FSRS_Optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-28 18:00:40.000000 FSRS-Optimizer-4.4.2/src/FSRS_Optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-28 18:00:40.000000 FSRS-Optimizer-4.4.2/src/FSRS_Optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:00:40.000000 FSRS-Optimizer-4.4.2/src/FSRS_Optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-28 18:00:40.000000 FSRS-Optimizer-4.4.2/src/FSRS_Optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 18:00:40.000000 FSRS-Optimizer-4.4.2/src/FSRS_Optimizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:00:40.152486 FSRS-Optimizer-4.4.2/src/fsrs_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 18:00:29.000000 FSRS-Optimizer-4.4.2/src/fsrs_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-28 18:00:29.000000 FSRS-Optimizer-4.4.2/src/fsrs_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51419 2023-07-28 18:00:29.000000 FSRS-Optimizer-4.4.2/src/fsrs_optimizer/fsrs_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:35:18.833123 FSRS-Optimizer-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-29 08:35:18.833123 FSRS-Optimizer-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-29 08:35:08.000000 FSRS-Optimizer-4.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-29 08:35:08.000000 FSRS-Optimizer-4.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 08:35:18.833123 FSRS-Optimizer-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-29 08:35:08.000000 FSRS-Optimizer-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:35:18.829123 FSRS-Optimizer-4.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:35:18.829123 FSRS-Optimizer-4.5.0/src/FSRS_Optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-29 08:35:18.000000 FSRS-Optimizer-4.5.0/src/FSRS_Optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-29 08:35:18.000000 FSRS-Optimizer-4.5.0/src/FSRS_Optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 08:35:18.000000 FSRS-Optimizer-4.5.0/src/FSRS_Optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-29 08:35:18.000000 FSRS-Optimizer-4.5.0/src/FSRS_Optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 08:35:18.000000 FSRS-Optimizer-4.5.0/src/FSRS_Optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:35:18.833123 FSRS-Optimizer-4.5.0/src/fsrs_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 08:35:08.000000 FSRS-Optimizer-4.5.0/src/fsrs_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-29 08:35:08.000000 FSRS-Optimizer-4.5.0/src/fsrs_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52099 2023-07-29 08:35:08.000000 FSRS-Optimizer-4.5.0/src/fsrs_optimizer/fsrs_optimizer.py
```

### Comparing `FSRS-Optimizer-4.4.2/PKG-INFO` & `FSRS-Optimizer-4.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.4.2
+Version: 4.5.0
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # FSRS Optimizer
 
 The FSRS Optimizer is a Python library capable of utilizing personal spaced repetition review logs to refine the FSRS algorithm. Designed with the intent of delivering a standardized, universal optimizer to various FSRS implementations across numerous programming languages, this tool is set to establish a ubiquitous standard for spaced repetition review logs. By facilitating the uniformity of learning data among different spaced repetition softwares, it guarantees learners consistent review schedules across a multitude of platforms.
@@ -16,15 +16,15 @@
 # Review Logs Schema
 
 The `review_logs` table captures the review activities performed by users. Each log records the details of a single review instance. The schema for this table is as follows:
 
 | Column Name | Data Type | Description | Constraints |
 |-------------|-----------|-------------|-------------|
 | card_id | integer or string | The unique identifier of the flashcard being reviewed | Not null |
-| review_time | timestamp  in *seconds* | The exact moment when the review took place | Not null |
+| review_time | timestamp  in *miliseconds* | The exact moment when the review took place | Not null |
 | review_rating | integer | The user's rating for the review. This rating is subjective and depends on how well the user believes they remembered the information on the card | Not null, Values: {1 (Again), 2 (Hard), 3 (Good), 4 (Easy)} |
 | review_state | integer | The state of the card at the time of review. This describes the learning phase of the card | Optional, Values: {0 (New), 1 (Learning), 2 (Review), 3 (Relearning)} |
 | review_duration | integer | The time spent on reviewing the card, typically in miliseconds | Optional, Non-negative |
 
 Extra Info:
 - `timezone`: The time zone of the user when they performed the review, which is used to identify the start of a new day.
 - `day_start`: The hour (0-23) at which the user starts a new day, which is used to separate reviews that are divided by sleep into different days.
```

### Comparing `FSRS-Optimizer-4.4.2/README.md` & `FSRS-Optimizer-4.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Review Logs Schema
 
 The `review_logs` table captures the review activities performed by users. Each log records the details of a single review instance. The schema for this table is as follows:
 
 | Column Name | Data Type | Description | Constraints |
 |-------------|-----------|-------------|-------------|
 | card_id | integer or string | The unique identifier of the flashcard being reviewed | Not null |
-| review_time | timestamp  in *seconds* | The exact moment when the review took place | Not null |
+| review_time | timestamp  in *miliseconds* | The exact moment when the review took place | Not null |
 | review_rating | integer | The user's rating for the review. This rating is subjective and depends on how well the user believes they remembered the information on the card | Not null, Values: {1 (Again), 2 (Hard), 3 (Good), 4 (Easy)} |
 | review_state | integer | The state of the card at the time of review. This describes the learning phase of the card | Optional, Values: {0 (New), 1 (Learning), 2 (Review), 3 (Relearning)} |
 | review_duration | integer | The time spent on reviewing the card, typically in miliseconds | Optional, Non-negative |
 
 Extra Info:
 - `timezone`: The time zone of the user when they performed the review, which is used to identify the start of a new day.
 - `day_start`: The hour (0-23) at which the user starts a new day, which is used to separate reviews that are divided by sleep into different days.
```

### Comparing `FSRS-Optimizer-4.4.2/src/FSRS_Optimizer.egg-info/PKG-INFO` & `FSRS-Optimizer-4.5.0/src/FSRS_Optimizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FSRS-Optimizer
-Version: 4.4.2
+Version: 4.5.0
 Project-URL: Homepage, https://github.com/open-spaced-repetition/fsrs-optimizer
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # FSRS Optimizer
 
 The FSRS Optimizer is a Python library capable of utilizing personal spaced repetition review logs to refine the FSRS algorithm. Designed with the intent of delivering a standardized, universal optimizer to various FSRS implementations across numerous programming languages, this tool is set to establish a ubiquitous standard for spaced repetition review logs. By facilitating the uniformity of learning data among different spaced repetition softwares, it guarantees learners consistent review schedules across a multitude of platforms.
@@ -16,15 +16,15 @@
 # Review Logs Schema
 
 The `review_logs` table captures the review activities performed by users. Each log records the details of a single review instance. The schema for this table is as follows:
 
 | Column Name | Data Type | Description | Constraints |
 |-------------|-----------|-------------|-------------|
 | card_id | integer or string | The unique identifier of the flashcard being reviewed | Not null |
-| review_time | timestamp  in *seconds* | The exact moment when the review took place | Not null |
+| review_time | timestamp  in *miliseconds* | The exact moment when the review took place | Not null |
 | review_rating | integer | The user's rating for the review. This rating is subjective and depends on how well the user believes they remembered the information on the card | Not null, Values: {1 (Again), 2 (Hard), 3 (Good), 4 (Easy)} |
 | review_state | integer | The state of the card at the time of review. This describes the learning phase of the card | Optional, Values: {0 (New), 1 (Learning), 2 (Review), 3 (Relearning)} |
 | review_duration | integer | The time spent on reviewing the card, typically in miliseconds | Optional, Non-negative |
 
 Extra Info:
 - `timezone`: The time zone of the user when they performed the review, which is used to identify the start of a new day.
 - `day_start`: The hour (0-23) at which the user starts a new day, which is used to separate reviews that are divided by sleep into different days.
```

### Comparing `FSRS-Optimizer-4.4.2/src/fsrs_optimizer/__main__.py` & `FSRS-Optimizer-4.5.0/src/fsrs_optimizer/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,20 +57,22 @@
 
     with open(config_save, "w+") as f: # Save the settings to load next time the program is run
         json.dump(remembered_fallbacks, f)
 
     show_graphs = graphs_input != "n"
 
     optimizer = fsrs_optimizer.Optimizer()
-    optimizer.anki_extract(filename)
+    optimizer.anki_extract(
+        filename,
+        remembered_fallbacks["filter_out_suspended_cards"] == "y"
+    )
     analysis = optimizer.create_time_series(
         remembered_fallbacks["timezone"],
         remembered_fallbacks["revlog_start_date"],
-        remembered_fallbacks["next_day"],
-        remembered_fallbacks["filter_out_suspended_cards"] == "y"
+        remembered_fallbacks["next_day"]
     )
     print(analysis)
 
     optimizer.define_model()
     optimizer.pretrain(verbose=show_graphs)
     optimizer.train(verbose=show_graphs)
```

### Comparing `FSRS-Optimizer-4.4.2/src/fsrs_optimizer/fsrs_optimizer.py` & `FSRS-Optimizer-4.5.0/src/fsrs_optimizer/fsrs_optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,19 @@
 from sklearn.metrics import mean_squared_error, mean_absolute_error, r2_score
 from scipy.optimize import curve_fit
 from itertools import accumulate
 from tqdm.auto import tqdm
 import warnings
 warnings.filterwarnings("ignore", category=UserWarning)
 
+New = 0
+Learning = 1
+Review = 2
+Relearning = 3
+
 def power_forgetting_curve(t, s):
     return (1 + t / (9 * s)) ** -1
 
 def next_interval(s, r):
     return np.maximum(1, np.round(9 * s * (1/r - 1)))
 
 class FSRS(nn.Module):
@@ -306,24 +311,21 @@
             return stabilities.tolist(), difficulties.tolist()
 
 """Used to store all the results from FSRS related functions"""
 class Optimizer:
     def __init__(self) -> None:
         tqdm.pandas()
 
-    @staticmethod
-    def anki_extract(filename: str):
+    def anki_extract(self, filename: str, filter_out_suspended_cards: bool = False):
         """Step 1"""
         # Extract the collection file or deck file to get the .anki21 database.
         with zipfile.ZipFile(f'{filename}', 'r') as zip_ref:
             zip_ref.extractall('./')
             tqdm.write("Deck file extracted successfully!")
 
-    def create_time_series(self, timezone: str, revlog_start_date: str, next_day_starts_at: int, filter_out_suspended_cards: bool = False):
-        """Step 2"""
         if os.path.isfile("collection.anki21b"):
             os.remove("collection.anki21b")
             raise Exception(
                 "Please export the file with `support older Anki versions` if you use the latest version of Anki.")
         elif os.path.isfile("collection.anki21"):
             con = sqlite3.connect("collection.anki21")
         elif os.path.isfile("collection.anki2"):
@@ -342,68 +344,69 @@
         )
         """
         )
         revlog = res.fetchall()
         if len(revlog) == 0:
             raise Exception("No review log found!")
         df = pd.DataFrame(revlog)
-        df.columns = ['id', 'cid', 'usn', 'r', 'ivl', 'last_ivl', 'factor', 'time', 'type']
-        df = df[(df['cid'] <= time.time() * 1000) &
-                (df['id'] <= time.time() * 1000)].copy()
-        
-        df_set_due_date = df[(df['type'] == 4) & (df['ivl'] > 0)]
+        df.columns = ['review_time', 'card_id', 'usn', 'review_rating', 'ivl', 'last_ivl', 'factor', 'review_duration', 'review_state']
+        df = df[(df['card_id'] <= time.time() * 1000) &
+                (df['review_time'] <= time.time() * 1000)].copy()
+        df_set_due_date = df[(df['review_state'] == 4) & (df['ivl'] > 0)]
         df.drop(df_set_due_date.index, inplace=True)
+        df.sort_values(by=['card_id', 'review_time'], inplace=True, ignore_index=True)
 
-        df['create_date'] = pd.to_datetime(df['cid'] // 1000, unit='s')
-        df['create_date'] = df['create_date'].dt.tz_localize('UTC').dt.tz_convert(timezone)
-        df['review_date'] = pd.to_datetime(df['id'] // 1000, unit='s')
-        df['review_date'] = df['review_date'].dt.tz_localize('UTC').dt.tz_convert(timezone)
-        df.drop(df[df['review_date'].dt.year < 2006].index, inplace=True)
-        df.sort_values(by=['cid', 'id'], inplace=True, ignore_index=True)
-
-        df['is_learn_start'] = (df['type'] == 0) & (df['type'].shift() != 0)
+        df['is_learn_start'] = (df['review_state'] == 0) & (df['review_state'].shift() != 0)
         df['sequence_group'] = df['is_learn_start'].cumsum()
-        last_learn_start = df[df['is_learn_start']].groupby('cid')['sequence_group'].last()
-        df['last_learn_start'] = df['cid'].map(last_learn_start).fillna(0).astype(int)
+        last_learn_start = df[df['is_learn_start']].groupby('card_id')['sequence_group'].last()
+        df['last_learn_start'] = df['card_id'].map(last_learn_start).fillna(0).astype(int)
         df['mask'] = df['last_learn_start'] <= df['sequence_group']
         df = df[df['mask'] == True].copy()
-        df.drop(columns=['is_learn_start', 'sequence_group', 'last_learn_start', 'mask'], inplace=True)
-        df = df[(df['type'] != 4)].copy()
-
-        self.type_sequence = np.array(df['type'])
-        self.time_sequence = np.array(df['time'])
+        df = df[(df['review_state'] != 4)].copy()
+        df = df[(df['review_state'] != 3) | (df['factor'] != 0)].copy()
+        df['review_state'] = df['review_state'] + 1
+        df.loc[df['is_learn_start'], 'review_state'] = New
+        df.drop(columns=['is_learn_start', 'sequence_group', 'last_learn_start', 'mask', 'usn', 'ivl', 'last_ivl', 'factor'], inplace=True)
         df.to_csv("revlog.csv", index=False)
         tqdm.write("revlog.csv saved.")
 
-        df = df[(df['type'] != 3) | (df['factor'] != 0)].copy()
+    def create_time_series(self, timezone: str, revlog_start_date: str, next_day_starts_at: int):
+        """Step 2"""
+        df = pd.read_csv("./revlog.csv")
+        df['review_state'] = df['review_state'].map(lambda x: x if x != New else Learning)
+        self.state_sequence = np.array(df['review_state'])
+        self.duration_sequence = np.array(df['review_duration'])
+        df['review_date'] = pd.to_datetime(df['review_time'] // 1000, unit='s')
+        df['review_date'] = df['review_date'].dt.tz_localize('UTC').dt.tz_convert(timezone)
+        df.drop(df[df['review_date'].dt.year < 2006].index, inplace=True)
         df['real_days'] = df['review_date'] - timedelta(hours=int(next_day_starts_at))
         df['real_days'] = pd.DatetimeIndex(df['real_days'].dt.floor('D', ambiguous='infer', nonexistent='shift_forward')).to_julian_date()
-        df.drop_duplicates(['cid', 'real_days'], keep='first', inplace=True)
+        df.drop_duplicates(['card_id', 'real_days'], keep='first', inplace=True)
         df['delta_t'] = df.real_days.diff()
         df.dropna(inplace=True)
-        df['i'] = df.groupby('cid').cumcount() + 1
+        df['i'] = df.groupby('card_id').cumcount() + 1
         df.loc[df['i'] == 1, 'delta_t'] = 0
-        df = df.groupby('cid').filter(lambda group: group['type'].iloc[0] == 0)
-        df['prev_type'] = df.groupby('cid')['type'].shift(1).fillna(0).astype(int)
-        df['helper'] = ((df['type'] == 0) & ((df['prev_type'] == 1) | (df['prev_type'] == 2)) & (df['i'] > 1)).astype(int)
-        df['helper'] = df.groupby('cid')['helper'].cumsum()
+        df = df.groupby('card_id').filter(lambda group: group['review_state'].iloc[0] == Learning)
+        df['prev_review_state'] = df.groupby('card_id')['review_state'].shift(1).fillna(Learning).astype(int)
+        df['helper'] = ((df['review_state'] == Learning) & ((df['prev_review_state'] == Review) | (df['prev_review_state'] == Relearning)) & (df['i'] > 1)).astype(int)
+        df['helper'] = df.groupby('card_id')['helper'].cumsum()
         df = df[df['helper'] == 0]
-        del df['prev_type']
+        del df['prev_review_state']
         del df['helper']
 
         def cum_concat(x):
             return list(accumulate(x))
 
-        t_history = df.groupby('cid', group_keys=False)['delta_t'].apply(lambda x: cum_concat([[int(i)] for i in x]))
+        t_history = df.groupby('card_id', group_keys=False)['delta_t'].apply(lambda x: cum_concat([[int(i)] for i in x]))
         df['t_history']=[','.join(map(str, item[:-1])) for sublist in t_history for item in sublist]
-        r_history = df.groupby('cid', group_keys=False)['r'].apply(lambda x: cum_concat([[i] for i in x]))
+        r_history = df.groupby('card_id', group_keys=False)['review_rating'].apply(lambda x: cum_concat([[i] for i in x]))
         df['r_history']=[','.join(map(str, item[:-1])) for sublist in r_history for item in sublist]
-        df = df.groupby('cid').filter(lambda group: group['id'].min() > time.mktime(datetime.strptime(revlog_start_date, "%Y-%m-%d").timetuple()) * 1000)
-        df = df[df['r'] != 0].copy()
-        df['y'] = df['r'].map(lambda x: {1: 0, 2: 1, 3: 1, 4: 1}[x])
+        df = df.groupby('card_id').filter(lambda group: group['review_time'].min() > time.mktime(datetime.strptime(revlog_start_date, "%Y-%m-%d").timetuple()) * 1000)
+        df = df[df['review_rating'] != 0].copy()
+        df['y'] = df['review_rating'].map(lambda x: {1: 0, 2: 1, 3: 1, 4: 1}[x])
 
         def remove_outliers(group: pd.DataFrame) -> pd.DataFrame:
             # threshold = np.mean(group['delta_t']) * 1.5
             # threshold = group['delta_t'].quantile(0.95)
             Q1 = group['delta_t'].quantile(0.25)
             Q3 = group['delta_t'].quantile(0.75)
             IQR = Q3 - Q1
@@ -417,28 +420,28 @@
             discontinuity = group['i'].diff().fillna(1).ne(1)
             if not discontinuity.any():
                 return group
             else:
                 first_non_continuous_index = discontinuity.idxmax()
                 return group.loc[:first_non_continuous_index-1]
 
-        df = df.groupby('cid', as_index=False, group_keys=False).progress_apply(remove_non_continuous_rows)
+        df = df.groupby('card_id', as_index=False, group_keys=False).progress_apply(remove_non_continuous_rows)
 
         df.to_csv('revlog_history.tsv', sep="\t", index=False)
         tqdm.write("Trainset saved.")
 
         S0_dataset = df[df['i'] == 2]
         self.S0_dataset_group = S0_dataset.groupby(by=['r_history', 'delta_t'], group_keys=False).agg({'y': ['mean', 'count']}).reset_index()
         self.S0_dataset_group.to_csv('stability_for_pretrain.tsv', sep='\t', index=None)
 
         df['retention'] = df.groupby(by=['r_history', 'delta_t'], group_keys=False)['y'].transform('mean')
-        df['total_cnt'] = df.groupby(by=['r_history', 'delta_t'], group_keys=False)['id'].transform('count')
+        df['total_cnt'] = df.groupby(by=['r_history', 'delta_t'], group_keys=False)['review_time'].transform('count')
         tqdm.write("Retention calculated.")
 
-        df = df.drop(columns=['id', 'cid', 'usn', 'ivl', 'last_ivl', 'factor', 'time', 'type', 'create_date', 'review_date', 'real_days', 'r', 't_history', 'y'])
+        df.drop(columns=['review_time', 'card_id', 'review_duration', 'review_state', 'review_date', 'real_days', 'review_rating', 't_history', 'y'], inplace=True)
         df.drop_duplicates(inplace=True)
         df['retention'] = df['retention'].map(lambda x: max(min(0.99, x), 0.01))
 
         def cal_stability(group: pd.DataFrame) -> pd.DataFrame:
             group_cnt = sum(group['total_cnt'])
             if group_cnt < 10:
                 return pd.DataFrame()
@@ -612,27 +615,27 @@
         w = np.array(w)
         avg_w = np.round(np.mean(w, axis=0), 4)
         self.w = avg_w.tolist()
 
         tqdm.write("\nTraining finished!")
         return plots
 
-    def preview(self, requestRetention: float):
+    def preview(self, requestRetention: float, verbose=False):
         my_collection = Collection(self.w)
         preview_text = "1:again, 2:hard, 3:good, 4:easy\n"
         for first_rating in (1,2,3,4):
             preview_text += f'\nfirst rating: {first_rating}\n'
             t_history = "0"
             d_history = "0"
             r_history = f"{first_rating}"  # the first rating of the new card
             # print("stability, difficulty, lapses")
             for i in range(10):
                 states = my_collection.predict(t_history, r_history)
-                # print('{0:9.2f} {1:11.2f} {2:7.0f}'.format(
-                    # *list(map(lambda x: round(float(x), 4), states))))
+                if verbose:
+                    print('{0:9.2f} {1:11.2f} {2:7.0f}'.format(*list(map(lambda x: round(float(x), 4), states))))
                 next_t = next_interval(states[0], requestRetention)                
                 difficulty = round(float(states[1]), 1)
                 t_history += f',{int(next_t)}'
                 d_history += f',{difficulty}'
                 r_history += f",3"
             preview_text += f"rating history: {r_history}\n"
             preview_text += "interval history: " + ",".join([f"{ivl}d" if ivl < 30 else f"{ivl / 30:.1f}m" if ivl < 365 else f"{ivl / 365:.1f}y" for ivl in map(int, t_history.split(','))]) + "\n"
@@ -660,18 +663,18 @@
         my_collection = Collection(self.w)
 
         stabilities, difficulties = my_collection.batch_predict(self.dataset)
         stabilities = map(lambda x: round(x, 2), stabilities)
         difficulties = map(lambda x: round(x, 2), difficulties)
         self.dataset['stability'] = list(stabilities)
         self.dataset['difficulty'] = list(difficulties)
-        prediction = self.dataset.groupby(by=['t_history', 'r_history']).agg({"stability": "mean", "difficulty": "mean", "id": "count"})
+        prediction = self.dataset.groupby(by=['t_history', 'r_history']).agg({"stability": "mean", "difficulty": "mean", "review_time": "count"})
         prediction.reset_index(inplace=True)
         prediction.sort_values(by=['r_history'], inplace=True)
-        prediction.rename(columns={"id": "count"}, inplace=True)
+        prediction.rename(columns={"review_time": "count"}, inplace=True)
         prediction.to_csv("./prediction.tsv", sep='\t', index=None)
         tqdm.write("prediction.tsv saved.")
         prediction['difficulty'] = prediction['difficulty'].map(lambda x: int(round(x)))
         self.difficulty_distribution = prediction.groupby(by=['difficulty'])['count'].sum() / prediction['count'].sum()
         self.difficulty_distribution_padding = np.zeros(10)
         for i in range(10):
             if i+1 in self.difficulty_distribution.index:
@@ -686,32 +689,32 @@
         index_offset = -(np.log(minimum_stability) / np.log(base)).round().astype(int)
         d_range = 10
         d_offset = 1
         r_time = 8
         f_time = 25
         max_time = 1e10
 
-        type_block = dict()
-        type_count = dict()
-        type_time = dict()
-        last_t = self.type_sequence[0]
-        type_block[last_t] = 1
-        type_count[last_t] = 1
-        type_time[last_t] = self.time_sequence[0]
-        for i,t in enumerate(self.type_sequence[1:]):
-            type_count[t] = type_count.setdefault(t, 0) + 1
-            type_time[t] = type_time.setdefault(t, 0) + self.time_sequence[i]
-            if t != last_t:
-                type_block[t] = type_block.setdefault(t, 0) + 1
-            last_t = t
+        state_block = dict()
+        state_count = dict()
+        state_duration = dict()
+        last_state = self.state_sequence[0]
+        state_block[last_state] = 1
+        state_count[last_state] = 1
+        state_duration[last_state] = self.duration_sequence[0]
+        for i, state in enumerate(self.state_sequence[1:]):
+            state_count[state] = state_count.setdefault(state, 0) + 1
+            state_duration[state] = state_duration.setdefault(state, 0) + self.duration_sequence[i]
+            if state != last_state:
+                state_block[state] = state_block.setdefault(state, 0) + 1
+            last_state = state
 
-        r_time = round(type_time[1]/type_count[1]/1000, 1)
+        r_time = round(state_duration[Review]/state_count[Review]/1000, 1)
 
-        if 2 in type_count and 2 in type_block:
-            f_time = round(type_time[2]/type_block[2]/1000 + r_time, 1)
+        if Relearning in state_count and Relearning in state_block:
+            f_time = round(state_duration[Relearning]/state_block[Relearning]/1000 + r_time, 1)
 
         tqdm.write(f"average time for failed cards: {f_time}s")
         tqdm.write(f"average time for recalled cards: {r_time}s")
 
         def stability2index(stability):
             return (np.log(stability) / np.log(base)).round().astype(int) + index_offset
 
@@ -802,16 +805,16 @@
         loss_after = self.dataset['log_loss'].mean()
 
         tmp = self.dataset.copy()
         tmp['stability'] = tmp['stability'].map(lambda x: round(x, 2))
         tmp['difficulty'] = tmp['difficulty'].map(lambda x: round(x, 2))
         tmp['p'] = tmp['p'].map(lambda x: round(x, 2))
         tmp['log_loss'] = tmp['log_loss'].map(lambda x: round(x, 2))
-        tmp.rename(columns={"r": "grade", "p": "retrievability"}, inplace=True)
-        tmp[['id', 'cid', 'review_date', 'r_history', 't_history', 'delta_t', 'grade', 'stability', 'difficulty', 'retrievability', 'log_loss']].to_csv("./evaluation.tsv", sep='\t', index=False)
+        tmp.rename(columns={"p": "retrievability"}, inplace=True)
+        tmp[['review_time', 'card_id', 'review_date', 'r_history', 't_history', 'delta_t', 'review_rating', 'stability', 'difficulty', 'retrievability', 'log_loss']].to_csv("./evaluation.tsv", sep='\t', index=False)
         del tmp
         return loss_before, loss_after
 
     def calibration_graph(self):
         fig1 = plt.figure()
         plot_brier(self.dataset['p'], self.dataset['y'], bins=40, ax=fig1.add_subplot(111))
         fig2 = plt.figure(figsize=(16, 12))
```

