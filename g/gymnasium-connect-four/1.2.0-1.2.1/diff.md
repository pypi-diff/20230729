# Comparing `tmp/gymnasium_connect_four-1.2.0.tar.gz` & `tmp/gymnasium_connect_four-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_connect_four-1.2.0.tar", last modified: Sat Jul 29 14:21:58 2023, max compression
+gzip compressed data, was "gymnasium_connect_four-1.2.1.tar", last modified: Sat Jul 29 14:41:28 2023, max compression
```

## Comparing `gymnasium_connect_four-1.2.0.tar` & `gymnasium_connect_four-1.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 14:21:58.132609 gymnasium_connect_four-1.2.0/
--rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.0/LICENSE
--rw-rw-rw-   0        0        0      251 2023-07-29 14:21:58.128083 gymnasium_connect_four-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    10857 2023-07-29 14:18:53.000000 gymnasium_connect_four-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 14:21:58.088074 gymnasium_connect_four-1.2.0/connect_four_gymnasium/
--rw-rw-rw-   0        0        0     8934 2023-07-29 11:26:49.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/ConnectFourEnv.py
--rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:21:58.109524 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/
--rw-rw-rw-   0        0        0     4648 2023-07-29 14:16:55.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/AdultPlayer.py
--rw-rw-rw-   0        0        0     4372 2023-07-29 14:16:50.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/AdultSmarterPlayer.py
--rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/BabyPlayer.py
--rw-rw-rw-   0        0        0     1881 2023-07-29 14:17:29.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/ChildPlayer.py
--rw-rw-rw-   0        0        0     2246 2023-07-29 14:17:21.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/ChildSmarterPlayer.py
--rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/ConsolePlayer.py
--rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/ModelPlayer.py
--rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/Player.py
--rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/SimulatePlayer.py
--rw-rw-rw-   0        0        0     3159 2023-07-29 14:17:15.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/TeenagerPlayer.py
--rw-rw-rw-   0        0        0     4374 2023-07-29 14:17:06.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
--rw-rw-rw-   0        0        0      446 2023-07-29 10:59:21.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:21:58.109524 gymnasium_connect_four-1.2.0/connect_four_gymnasium/tools/
--rw-rw-rw-   0        0        0     3319 2023-07-29 14:17:42.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/tools/EloLeaderboard.py
--rw-rw-rw-   0        0        0     4744 2023-07-29 14:17:37.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/tools/Update_bot_elo.py
--rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:21:58.123066 gymnasium_connect_four-1.2.0/gymnasium_connect_four.egg-info/
--rw-rw-rw-   0        0        0      251 2023-07-29 14:21:57.000000 gymnasium_connect_four-1.2.0/gymnasium_connect_four.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2023-07-29 14:21:57.000000 gymnasium_connect_four-1.2.0/gymnasium_connect_four.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 14:21:57.000000 gymnasium_connect_four-1.2.0/gymnasium_connect_four.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-29 14:21:57.000000 gymnasium_connect_four-1.2.0/gymnasium_connect_four.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-29 14:21:57.000000 gymnasium_connect_four-1.2.0/gymnasium_connect_four.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 14:21:58.132609 gymnasium_connect_four-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-07-29 10:31:22.000000 gymnasium_connect_four-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:21:58.128083 gymnasium_connect_four-1.2.0/test/
--rw-rw-rw-   0        0        0     4688 2023-07-29 06:40:16.000000 gymnasium_connect_four-1.2.0/test/test_no_opponant.py
--rw-rw-rw-   0        0        0    21167 2023-07-25 14:09:28.000000 gymnasium_connect_four-1.2.0/test/test_power_4_logic.py
--rw-rw-rw-   0        0        0     2372 2023-07-29 10:38:54.000000 gymnasium_connect_four-1.2.0/test/test_ppo_env.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:41:28.339794 gymnasium_connect_four-1.2.1/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-07-29 14:41:28.338784 gymnasium_connect_four-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10857 2023-07-29 14:18:53.000000 gymnasium_connect_four-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 14:41:28.299186 gymnasium_connect_four-1.2.1/connect_four_gymnasium/
+-rw-rw-rw-   0        0        0     8934 2023-07-29 11:26:49.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/ConnectFourEnv.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:41:28.319731 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/
+-rw-rw-rw-   0        0        0     4648 2023-07-29 14:16:55.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/AdultPlayer.py
+-rw-rw-rw-   0        0        0     4372 2023-07-29 14:16:50.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/AdultSmarterPlayer.py
+-rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/BabyPlayer.py
+-rw-rw-rw-   0        0        0     1881 2023-07-29 14:17:29.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ChildPlayer.py
+-rw-rw-rw-   0        0        0     2246 2023-07-29 14:17:21.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ChildSmarterPlayer.py
+-rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ConsolePlayer.py
+-rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ModelPlayer.py
+-rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/Player.py
+-rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/SimulatePlayer.py
+-rw-rw-rw-   0        0        0     3159 2023-07-29 14:17:15.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/TeenagerPlayer.py
+-rw-rw-rw-   0        0        0     4374 2023-07-29 14:17:06.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
+-rw-rw-rw-   0        0        0      446 2023-07-29 10:59:21.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:41:28.324737 gymnasium_connect_four-1.2.1/connect_four_gymnasium/tools/
+-rw-rw-rw-   0        0        0     3238 2023-07-29 14:40:52.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/tools/EloLeaderboard.py
+-rw-rw-rw-   0        0        0     4744 2023-07-29 14:17:37.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/tools/Update_bot_elo.py
+-rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:41:28.332276 gymnasium_connect_four-1.2.1/gymnasium_connect_four.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-07-29 14:41:28.000000 gymnasium_connect_four-1.2.1/gymnasium_connect_four.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2023-07-29 14:41:28.000000 gymnasium_connect_four-1.2.1/gymnasium_connect_four.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 14:41:28.000000 gymnasium_connect_four-1.2.1/gymnasium_connect_four.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-29 14:41:28.000000 gymnasium_connect_four-1.2.1/gymnasium_connect_four.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-29 14:41:28.000000 gymnasium_connect_four-1.2.1/gymnasium_connect_four.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 14:41:28.339794 gymnasium_connect_four-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-07-29 14:41:05.000000 gymnasium_connect_four-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:41:28.337276 gymnasium_connect_four-1.2.1/test/
+-rw-rw-rw-   0        0        0     4688 2023-07-29 06:40:16.000000 gymnasium_connect_four-1.2.1/test/test_no_opponant.py
+-rw-rw-rw-   0        0        0    21167 2023-07-25 14:09:28.000000 gymnasium_connect_four-1.2.1/test/test_power_4_logic.py
+-rw-rw-rw-   0        0        0     2372 2023-07-29 10:38:54.000000 gymnasium_connect_four-1.2.1/test/test_ppo_env.py
```

### Comparing `gymnasium_connect_four-1.2.0/LICENSE` & `gymnasium_connect_four-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/README.md` & `gymnasium_connect_four-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/connect_four_gymnasium/ConnectFourEnv.py` & `gymnasium_connect_four-1.2.1/connect_four_gymnasium/ConnectFourEnv.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/AdultPlayer.py` & `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/AdultPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/AdultSmarterPlayer.py` & `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/AdultSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/BabyPlayer.py` & `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/BabyPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/ChildPlayer.py` & `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ChildPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/ChildSmarterPlayer.py` & `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ChildSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/ConsolePlayer.py` & `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ConsolePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/ModelPlayer.py` & `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ModelPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/SimulatePlayer.py` & `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/SimulatePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/TeenagerPlayer.py` & `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/TeenagerPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/TeenagerSmarterPlayer.py` & `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/TeenagerSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/connect_four_gymnasium/tools/EloLeaderboard.py` & `gymnasium_connect_four-1.2.1/connect_four_gymnasium/tools/EloLeaderboard.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.playersWithEloFixed = [
             BabyPlayer(),
             ChildPlayer(),
             ChildSmarterPlayer(),
             TeenagerPlayer(),
             TeenagerSmarterPlayer(),
             AdultPlayer(),
-            # AdultSmarterPlayer()
+            AdultSmarterPlayer()
         ]
 
     def update_elo(self, player_elo, opponent_elo, player_won, k_factor=32, draw=False):
         # Calculate the expected outcome based on the current Elo ratings
         expected_outcome = 1 / (1 + math.pow(10, (opponent_elo - player_elo) / 400))
         # Set the actual outcome based on whether the player won, lost, or drew
         if draw:
@@ -44,15 +44,15 @@
         all_match_opponents = [player for player in self.playersWithEloFixed for _ in range(num_matches)]
         random.shuffle(all_match_opponents)
         scores = self.get_scores(player, all_match_opponents)
         for opponent, score in zip(all_match_opponents, scores):
             player_won = score > 0
             draw = score == 0
             opponent_elo = opponent.getElo()
-            k_factor = 32 / (1 + gamePlayed / 10)
+            k_factor = 400 / (1 + (gamePlayed))
             actualElo = self.update_elo(actualElo, opponent_elo, player_won, k_factor, draw)
             gamePlayed += 1
 
         return actualElo
 
     def get_elo(self, player, num_matches=400):
         actualElo = player.getElo() if player.getElo() is not None else 1500
@@ -79,11 +79,10 @@
 
             remaining_indices = new_remaining_indices
 
         return scores
 
 
 if __name__ == "__main__":
-    from connect_four_gymnasium.players import (TeenagerSmarterPlayer)
 
     elo_leaderboard = EloLeaderboard()
-    print(elo_leaderboard.get_elo([TeenagerSmarterPlayer()], num_matches=100))
+    print(elo_leaderboard.get_elo(AdultSmarterPlayer(), num_matches=100))
```

### Comparing `gymnasium_connect_four-1.2.0/connect_four_gymnasium/tools/Update_bot_elo.py` & `gymnasium_connect_four-1.2.1/connect_four_gymnasium/tools/Update_bot_elo.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/gymnasium_connect_four.egg-info/SOURCES.txt` & `gymnasium_connect_four-1.2.1/gymnasium_connect_four.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/setup.py` & `gymnasium_connect_four-1.2.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='gymnasium_connect_four',
-    version='1.2.0',
+    version='1.2.1',
     description='A connect 4 (connect four) environment for OpenAI Gym and Gymnasium',
     author='Lucas Bertola',
     url='https://github.com/lucasBertola/Connect-4-env',  
     # author_email='your.email@example.com',
     packages=find_packages(),
     install_requires=[
         'pygame==2.1.3',
```

### Comparing `gymnasium_connect_four-1.2.0/test/test_no_opponant.py` & `gymnasium_connect_four-1.2.1/test/test_no_opponant.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/test/test_power_4_logic.py` & `gymnasium_connect_four-1.2.1/test/test_power_4_logic.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.0/test/test_ppo_env.py` & `gymnasium_connect_four-1.2.1/test/test_ppo_env.py`

 * *Files identical despite different names*

