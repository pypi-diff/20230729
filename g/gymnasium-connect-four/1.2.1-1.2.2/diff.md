# Comparing `tmp/gymnasium_connect_four-1.2.1.tar.gz` & `tmp/gymnasium_connect_four-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_connect_four-1.2.1.tar", last modified: Sat Jul 29 14:41:28 2023, max compression
+gzip compressed data, was "gymnasium_connect_four-1.2.2.tar", last modified: Sat Jul 29 17:32:22 2023, max compression
```

## Comparing `gymnasium_connect_four-1.2.1.tar` & `gymnasium_connect_four-1.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 14:41:28.339794 gymnasium_connect_four-1.2.1/
--rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.1/LICENSE
--rw-rw-rw-   0        0        0      251 2023-07-29 14:41:28.338784 gymnasium_connect_four-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    10857 2023-07-29 14:18:53.000000 gymnasium_connect_four-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 14:41:28.299186 gymnasium_connect_four-1.2.1/connect_four_gymnasium/
--rw-rw-rw-   0        0        0     8934 2023-07-29 11:26:49.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/ConnectFourEnv.py
--rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:41:28.319731 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/
--rw-rw-rw-   0        0        0     4648 2023-07-29 14:16:55.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/AdultPlayer.py
--rw-rw-rw-   0        0        0     4372 2023-07-29 14:16:50.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/AdultSmarterPlayer.py
--rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/BabyPlayer.py
--rw-rw-rw-   0        0        0     1881 2023-07-29 14:17:29.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ChildPlayer.py
--rw-rw-rw-   0        0        0     2246 2023-07-29 14:17:21.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ChildSmarterPlayer.py
--rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ConsolePlayer.py
--rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ModelPlayer.py
--rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/Player.py
--rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/SimulatePlayer.py
--rw-rw-rw-   0        0        0     3159 2023-07-29 14:17:15.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/TeenagerPlayer.py
--rw-rw-rw-   0        0        0     4374 2023-07-29 14:17:06.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
--rw-rw-rw-   0        0        0      446 2023-07-29 10:59:21.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:41:28.324737 gymnasium_connect_four-1.2.1/connect_four_gymnasium/tools/
--rw-rw-rw-   0        0        0     3238 2023-07-29 14:40:52.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/tools/EloLeaderboard.py
--rw-rw-rw-   0        0        0     4744 2023-07-29 14:17:37.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/tools/Update_bot_elo.py
--rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.1/connect_four_gymnasium/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:41:28.332276 gymnasium_connect_four-1.2.1/gymnasium_connect_four.egg-info/
--rw-rw-rw-   0        0        0      251 2023-07-29 14:41:28.000000 gymnasium_connect_four-1.2.1/gymnasium_connect_four.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2023-07-29 14:41:28.000000 gymnasium_connect_four-1.2.1/gymnasium_connect_four.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 14:41:28.000000 gymnasium_connect_four-1.2.1/gymnasium_connect_four.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-29 14:41:28.000000 gymnasium_connect_four-1.2.1/gymnasium_connect_four.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-29 14:41:28.000000 gymnasium_connect_four-1.2.1/gymnasium_connect_four.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 14:41:28.339794 gymnasium_connect_four-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-07-29 14:41:05.000000 gymnasium_connect_four-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:41:28.337276 gymnasium_connect_four-1.2.1/test/
--rw-rw-rw-   0        0        0     4688 2023-07-29 06:40:16.000000 gymnasium_connect_four-1.2.1/test/test_no_opponant.py
--rw-rw-rw-   0        0        0    21167 2023-07-25 14:09:28.000000 gymnasium_connect_four-1.2.1/test/test_power_4_logic.py
--rw-rw-rw-   0        0        0     2372 2023-07-29 10:38:54.000000 gymnasium_connect_four-1.2.1/test/test_ppo_env.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:32:22.682506 gymnasium_connect_four-1.2.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-07-29 17:32:22.682506 gymnasium_connect_four-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10858 2023-07-29 17:13:55.000000 gymnasium_connect_four-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 17:32:22.670500 gymnasium_connect_four-1.2.2/connect_four_gymnasium/
+-rw-rw-rw-   0        0        0     8813 2023-07-29 17:26:26.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/ConnectFourEnv.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:32:22.670500 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/
+-rw-rw-rw-   0        0        0     4654 2023-07-29 17:00:12.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/AdultPlayer.py
+-rw-rw-rw-   0        0        0     4378 2023-07-29 17:00:36.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/AdultSmarterPlayer.py
+-rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/BabyPlayer.py
+-rw-rw-rw-   0        0        0     1881 2023-07-29 14:17:29.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ChildPlayer.py
+-rw-rw-rw-   0        0        0     2248 2023-07-29 17:00:55.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ChildSmarterPlayer.py
+-rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ConsolePlayer.py
+-rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ModelPlayer.py
+-rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/Player.py
+-rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/SimulatePlayer.py
+-rw-rw-rw-   0        0        0     3163 2023-07-29 17:01:08.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/TeenagerPlayer.py
+-rw-rw-rw-   0        0        0     4378 2023-07-29 17:01:22.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
+-rw-rw-rw-   0        0        0      446 2023-07-29 10:59:21.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:32:22.682506 gymnasium_connect_four-1.2.2/connect_four_gymnasium/tools/
+-rw-rw-rw-   0        0        0     3238 2023-07-29 14:40:52.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/tools/EloLeaderboard.py
+-rw-rw-rw-   0        0        0     4744 2023-07-29 14:17:37.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/tools/Update_bot_elo.py
+-rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.2/connect_four_gymnasium/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:32:22.682506 gymnasium_connect_four-1.2.2/gymnasium_connect_four.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-07-29 17:32:22.000000 gymnasium_connect_four-1.2.2/gymnasium_connect_four.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2023-07-29 17:32:22.000000 gymnasium_connect_four-1.2.2/gymnasium_connect_four.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 17:32:22.000000 gymnasium_connect_four-1.2.2/gymnasium_connect_four.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-29 17:32:22.000000 gymnasium_connect_four-1.2.2/gymnasium_connect_four.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-29 17:32:22.000000 gymnasium_connect_four-1.2.2/gymnasium_connect_four.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 17:32:22.682506 gymnasium_connect_four-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-07-29 17:32:08.000000 gymnasium_connect_four-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 17:32:22.682506 gymnasium_connect_four-1.2.2/test/
+-rw-rw-rw-   0        0        0     4722 2023-07-29 17:17:01.000000 gymnasium_connect_four-1.2.2/test/test_no_opponant.py
+-rw-rw-rw-   0        0        0    21564 2023-07-29 17:15:09.000000 gymnasium_connect_four-1.2.2/test/test_power_4_logic.py
+-rw-rw-rw-   0        0        0     2372 2023-07-29 17:18:55.000000 gymnasium_connect_four-1.2.2/test/test_ppo_env.py
```

### Comparing `gymnasium_connect_four-1.2.1/LICENSE` & `gymnasium_connect_four-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.1/README.md` & `gymnasium_connect_four-1.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 ```python
 self.action_space = spaces.Discrete(self.COLUMNS_COUNT)
 ```
 
 ### Observation Space
 
-The observation space in the Connect Four environment is a 2D array representing the game board. Each cell in the array can have one of three possible values: 0 (empty), 1 (player's piece), or 2 (opponent's piece). The observation space is defined as follows:
+The observation space in the Connect Four environment is a 2D array representing the game board. Each cell in the array can have one of three possible values: 0 (empty), 1 (player's piece), or -1 (opponent's piece). The observation space is defined as follows:
 
 ```python
 self.observation_space = spaces.Box(low=0, high=2, shape=(self.ROWS_COUNT, self.COLUMNS_COUNT), dtype=np.int32)
 ```
 
 ### Rewards
```

#### html2text {}

```diff
@@ -66,15 +66,15 @@
 observation space, rewards, and episode termination conditions. ### Action
 Space The action space in the Connect Four environment is discrete, with a
 total of 7 possible actions. Each action corresponds to a column in the game
 board where a player can drop their piece. The action space is represented as
 follows: ```python self.action_space = spaces.Discrete(self.COLUMNS_COUNT) ```
 ### Observation Space The observation space in the Connect Four environment is
 a 2D array representing the game board. Each cell in the array can have one of
-three possible values: 0 (empty), 1 (player's piece), or 2 (opponent's piece).
+three possible values: 0 (empty), 1 (player's piece), or -1 (opponent's piece).
 The observation space is defined as follows: ```python self.observation_space =
 spaces.Box(low=0, high=2, shape=(self.ROWS_COUNT, self.COLUMNS_COUNT),
 dtype=np.int32) ``` ### Rewards The reward system in the Connect Four
 environment is designed to encourage the AI model to learn how to win the game.
 The rewards are as follows: - A reward of +1 is given when the AI model wins
 the game by connecting four of its pieces in a row, either horizontally,
 vertically, or diagonally. - A reward of -1 is given when the AI model loses
```

### Comparing `gymnasium_connect_four-1.2.1/connect_four_gymnasium/ConnectFourEnv.py` & `gymnasium_connect_four-1.2.2/connect_four_gymnasium/ConnectFourEnv.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,37 +21,37 @@
         self.opponent = opponent
 
     def __init__(self, opponent=None, render_mode=None, first_player=None):
         self.opponent = opponent  # Define the opponent
         # Define the action and observation spaces
         self.action_space = spaces.Discrete(self.COLUMNS_COUNT)
 
-        # 1 is you, 2 is the opponent
-        self.observation_space = spaces.Box(low=0, high=2, shape=(self.ROWS_COUNT, self.COLUMNS_COUNT), dtype=np.int32)
+        # 1 is you, -1 is the opponent
+        self.observation_space = spaces.Box(low=-1, high=1, shape=(self.ROWS_COUNT, self.COLUMNS_COUNT), dtype=np.int32)
 
         # Check if the render mode is valid
         assert render_mode is None or render_mode in self.metadata["render_modes"]
-        assert first_player is None or first_player in [1, 2]
+        assert first_player is None or first_player in [1, -1]
         self.render_mode = render_mode
         self.last_render_time = None
         self.window = None
         self.first_player = first_player
 
     def reset(self, seed=None, options=None):
         super().reset(seed=seed)
         self._board = np.zeros((self.ROWS_COUNT, self.COLUMNS_COUNT))
         self.render_for_human()
 
         if self.first_player is None:
-            self.next_player_to_play = np.random.choice([1, 2])
+            self.next_player_to_play = np.random.choice([1, -1])
         else:
             self.next_player_to_play = self.first_player
 
         if self.opponent is not None:
-            if self.next_player_to_play == 2:
+            if self.next_player_to_play == -1:
                 opponent_action = self.opponent.play(self._board)
                 result, isFinish = self.play_action(opponent_action, self.next_player_to_play)
                 if isFinish :
                     print('wtf')
                     print(opponent_action)
                     exit("The opponent played an invalid action in the first move!")
                 self.next_player_to_play = 1
@@ -89,33 +89,30 @@
 
         return 0, False
 
     def board_is_full(self):
         return np.all(self._board != 0)
     
     def inverse_player_position(self):
-        new_board = np.zeros_like(self._board)
-        new_board[self._board == 1] = 2
-        new_board[self._board == 2] = 1
-        return new_board
+        return -self._board
 
     def switch_player(self):
-        self.next_player_to_play = 3 - self.next_player_to_play
+        self.next_player_to_play = -1*self.next_player_to_play
         
     def step(self, action, play_opponent=True):
         action = action.item() if isinstance(action, np.ndarray) else action
 
         result, is_finish = self.play_action(action, self.next_player_to_play)
         if is_finish:
             return self._board, result, True, False, {}
         
         self.switch_player()
 
         if  play_opponent and self.opponent is not None:
-            # because 1 is you, 2 is the opponent
+            # because 1 is you, -1 is the opponent
             # you need to see the board as the opponent sees it
             opponent_action = self.opponent.play(self.inverse_player_position())
             opponent_result = self.step(opponent_action, play_opponent=False)
             return opponent_result[0],-1* opponent_result[1], opponent_result[2], opponent_result[3], opponent_result[4]
         elif self.opponent is None:
             boardToReturn = self._board if self.next_player_to_play == 1 else self.inverse_player_position()
             return boardToReturn, 0, False, False, {}
@@ -192,15 +189,15 @@
         i_position = padding
         for i in range(self.ROWS_COUNT):
             j_position = padding
             for j in range(self.COLUMNS_COUNT):
                 color = (245, 245, 245)
                 if self._board[i, j] == 1:
                     color = self.player_1_color
-                elif self._board[i, j] == 2:
+                elif self._board[i, j] == -1:
                     color = self.player_2_color
                 pygame.draw.circle(canvas, color, (j_position + circle_radius, i_position + circle_radius), circle_radius)
                 j_position += (circle_radius * 2) + padding_center
             i_position += (circle_radius * 2) + padding_center
 
         # Display opponent's color and name
         text_position_y_first_player = end_height_board
```

### Comparing `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/AdultPlayer.py` & `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/TeenagerSmarterPlayer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from .Player import Player
 
-class AdultPlayer(Player):
-    
+class TeenagerSmarterPlayer(Player):
+
     def __init__(self, _=""):
         pass
     
     def play_single(self, observation):
         moves_to_avoid = []
 
         # Check for a winning move for the player
@@ -15,41 +15,35 @@
                 new_board, row, col = self.apply_move(observation, move, 1)
                 if self.check_win_around_last_move(new_board, 1, row, col):
                     return move
 
         # Check for a winning move for the opponent
         for move in range(7):
             if observation[0, move] == 0:
-                new_board, row, col = self.apply_move(observation, move, 2)
-                if self.check_win_around_last_move(new_board, 2, row, col):
+                new_board, row, col = self.apply_move(observation, move, -1)
+                if self.check_win_around_last_move(new_board, -1, row, col):
                     return move
 
         # Check if a move allows the opponent to win by playing the same move again
         for move in range(7):
             if observation[0, move] == 0:
                 new_board, row, col = self.apply_move(observation, move, 1)
                 if new_board[0, move] == 0:
-                    new_board, row, col = self.apply_move(new_board, move, 2)
-                    if self.check_win_around_last_move(new_board, 2, row, col):
+                    new_board, row, col = self.apply_move(new_board, move, -1)
+                    if self.check_win_around_last_move(new_board, -1, row, col):
                         moves_to_avoid.append(move)
 
         # Check if a move creates a line of three tokens with available spaces on both sides
         for move in range(7):
             if observation[0, move] == 0:
                 new_board, row, col = self.apply_move(observation, move, 1)
                 if self.check_three_in_a_row(new_board, 1, row, col) and move not in moves_to_avoid:
                     return move
-        
-        for move in range(7):
-            if observation[0, move] == 0:
-                new_board, row, col = self.apply_move(observation, move, 2)
-                if self.check_three_in_a_row(new_board, 2, row, col) and move not in moves_to_avoid:
-                    return move
 
-        # Play a random move among valid moves, excluding moves_to_avoid
+        # Play a random move among valid moves, except those in moves_to_avoid
         valid_moves = [c for c in range(7) if observation[0, c] == 0 and c not in moves_to_avoid]
 
         # If valid_moves is empty, choose a random move among all possible moves
         if not valid_moves:
             valid_moves = [c for c in range(7) if observation[0, c] == 0]
 
         if not valid_moves:
@@ -61,18 +55,18 @@
     def play(self, obs):
         if isinstance(obs, list):
             return [self.play_single(o) for o in obs]
         else:
             return self.play_single(obs)
 
     def getName(self):
-        return "AdultPlayer"
+        return "TeenagerSmarterPlayer"
 
     def getElo(self):
-        return 1654
+        return 1647
     
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
```

### Comparing `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/AdultSmarterPlayer.py` & `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/AdultSmarterPlayer.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,39 +15,39 @@
                 new_board, row, col = self.apply_move(observation, move, 1)
                 if self.check_win_around_last_move(new_board, 1, row, col):
                     return move
 
         # Check if there is a winning move for the opponent
         for move in range(7):
             if observation[0, move] == 0:
-                new_board, row, col = self.apply_move(observation, move, 2)
-                if self.check_win_around_last_move(new_board, 2, row, col):
+                new_board, row, col = self.apply_move(observation, move, -1)
+                if self.check_win_around_last_move(new_board, -1, row, col):
                     return move
 
         # Check if a move allows the opponent to win by playing the same move again
         for move in range(7):
             if observation[0, move] == 0:
                 new_board, row, col = self.apply_move(observation, move, 1)
                 if new_board[0, move] == 0:
-                    new_board, row, col = self.apply_move(new_board, move, 2)
-                    if self.check_win_around_last_move(new_board, 2, row, col):
+                    new_board, row, col = self.apply_move(new_board, move, -1)
+                    if self.check_win_around_last_move(new_board, -1, row, col):
                         moves_to_avoid.append(move)
 
         # Check if a move creates multiple ways to win for the player
         for move in range(7):
             if observation[0, move] == 0:
                 new_board, row, col = self.apply_move(observation, move, 1)
                 if self.check_multiple_ways_to_win(new_board, 1) and move not in moves_to_avoid:
                     return move
 
         # Check if a move allows the opponent to create multiple ways to win
         for move in range(7):
             if observation[0, move] == 0:
-                new_board, row, col = self.apply_move(observation, move, 2)
-                if self.check_multiple_ways_to_win(new_board, 2) and move not in moves_to_avoid:
+                new_board, row, col = self.apply_move(observation, move, -1)
+                if self.check_multiple_ways_to_win(new_board, -1) and move not in moves_to_avoid:
                     return move
 
         # Play a random move among the valid moves, except those in moves_to_avoid
         valid_moves = [c for c in range(7) if observation[0, c] == 0 and c not in moves_to_avoid]
 
         # If valid_moves is empty, choose a random move among all possible moves
         if not valid_moves:
```

### Comparing `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/BabyPlayer.py` & `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/BabyPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ChildPlayer.py` & `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ChildPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ChildSmarterPlayer.py` & `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ChildSmarterPlayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
                 new_board, row, col = self.apply_move(observation, move, 1)
                 if self.check_win_around_last_move(new_board, 1, row, col):
                     return move
 
         # Check if there is a winning move for the opponent
         for move in range(7):
             if observation[0, move] == 0:
-                new_board, row, col = self.apply_move(observation, move, 2)
-                if self.check_win_around_last_move(new_board, 2, row, col):
+                new_board, row, col = self.apply_move(observation, move, -1)
+                if self.check_win_around_last_move(new_board, -1, row, col):
                     return move
 
         # Play a random move
         valid_moves = [c for c in range(7) if observation[0, c] == 0]
         return np.random.choice(valid_moves)
 
     def play(self, observation):
```

### Comparing `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ConsolePlayer.py` & `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ConsolePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/ModelPlayer.py` & `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/ModelPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/SimulatePlayer.py` & `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/SimulatePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/TeenagerPlayer.py` & `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/TeenagerPlayer.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,25 @@
                 new_board, row, col = self.apply_move(observation, move, 1)
                 if self.check_win_around_last_move(new_board, 1, row, col):
                     return move
 
         # Check for a winning move for the opponent
         for move in range(7):
             if observation[0, move] == 0:
-                new_board, row, col = self.apply_move(observation, move, 2)
-                if self.check_win_around_last_move(new_board, 2, row, col):
+                new_board, row, col = self.apply_move(observation, move, -1)
+                if self.check_win_around_last_move(new_board, -1, row, col):
                     return move
 
         # Check if a move allows the opponent to win by playing the same move again
         for move in range(7):
             if observation[0, move] == 0:
                 new_board, row, col = self.apply_move(observation, move, 1)
                 if new_board[0, move] == 0:
-                    new_board, row, col = self.apply_move(new_board, move, 2)
-                    if self.check_win_around_last_move(new_board, 2, row, col):
+                    new_board, row, col = self.apply_move(new_board, move, -1)
+                    if self.check_win_around_last_move(new_board, -1, row, col):
                         moves_to_avoid.append(move)
 
         # Play a random move among valid moves, excluding moves_to_avoid
         valid_moves = [c for c in range(7) if observation[0, c] == 0 and c not in moves_to_avoid]
 
         # If valid_moves is empty, choose a random move among all possible moves
         if not valid_moves:
```

### Comparing `gymnasium_connect_four-1.2.1/connect_four_gymnasium/players/TeenagerSmarterPlayer.py` & `gymnasium_connect_four-1.2.2/connect_four_gymnasium/players/AdultPlayer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from .Player import Player
 
-class TeenagerSmarterPlayer(Player):
-
+class AdultPlayer(Player):
+    
     def __init__(self, _=""):
         pass
     
     def play_single(self, observation):
         moves_to_avoid = []
 
         # Check for a winning move for the player
@@ -15,35 +15,41 @@
                 new_board, row, col = self.apply_move(observation, move, 1)
                 if self.check_win_around_last_move(new_board, 1, row, col):
                     return move
 
         # Check for a winning move for the opponent
         for move in range(7):
             if observation[0, move] == 0:
-                new_board, row, col = self.apply_move(observation, move, 2)
-                if self.check_win_around_last_move(new_board, 2, row, col):
+                new_board, row, col = self.apply_move(observation, move, -1)
+                if self.check_win_around_last_move(new_board, -1, row, col):
                     return move
 
         # Check if a move allows the opponent to win by playing the same move again
         for move in range(7):
             if observation[0, move] == 0:
                 new_board, row, col = self.apply_move(observation, move, 1)
                 if new_board[0, move] == 0:
-                    new_board, row, col = self.apply_move(new_board, move, 2)
-                    if self.check_win_around_last_move(new_board, 2, row, col):
+                    new_board, row, col = self.apply_move(new_board, move, -1)
+                    if self.check_win_around_last_move(new_board, -1, row, col):
                         moves_to_avoid.append(move)
 
         # Check if a move creates a line of three tokens with available spaces on both sides
         for move in range(7):
             if observation[0, move] == 0:
                 new_board, row, col = self.apply_move(observation, move, 1)
                 if self.check_three_in_a_row(new_board, 1, row, col) and move not in moves_to_avoid:
                     return move
+        
+        for move in range(7):
+            if observation[0, move] == 0:
+                new_board, row, col = self.apply_move(observation, move, -1)
+                if self.check_three_in_a_row(new_board, -1, row, col) and move not in moves_to_avoid:
+                    return move
 
-        # Play a random move among valid moves, except those in moves_to_avoid
+        # Play a random move among valid moves, excluding moves_to_avoid
         valid_moves = [c for c in range(7) if observation[0, c] == 0 and c not in moves_to_avoid]
 
         # If valid_moves is empty, choose a random move among all possible moves
         if not valid_moves:
             valid_moves = [c for c in range(7) if observation[0, c] == 0]
 
         if not valid_moves:
@@ -55,18 +61,18 @@
     def play(self, obs):
         if isinstance(obs, list):
             return [self.play_single(o) for o in obs]
         else:
             return self.play_single(obs)
 
     def getName(self):
-        return "TeenagerSmarterPlayer"
+        return "AdultPlayer"
 
     def getElo(self):
-        return 1647
+        return 1654
     
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
```

### Comparing `gymnasium_connect_four-1.2.1/connect_four_gymnasium/tools/EloLeaderboard.py` & `gymnasium_connect_four-1.2.2/connect_four_gymnasium/tools/EloLeaderboard.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.1/connect_four_gymnasium/tools/Update_bot_elo.py` & `gymnasium_connect_four-1.2.2/connect_four_gymnasium/tools/Update_bot_elo.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.1/gymnasium_connect_four.egg-info/SOURCES.txt` & `gymnasium_connect_four-1.2.2/gymnasium_connect_four.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.1/setup.py` & `gymnasium_connect_four-1.2.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='gymnasium_connect_four',
-    version='1.2.1',
+    version='1.2.2',
     description='A connect 4 (connect four) environment for OpenAI Gym and Gymnasium',
     author='Lucas Bertola',
     url='https://github.com/lucasBertola/Connect-4-env',  
     # author_email='your.email@example.com',
     packages=find_packages(),
     install_requires=[
         'pygame==2.1.3',
```

### Comparing `gymnasium_connect_four-1.2.1/test/test_no_opponant.py` & `gymnasium_connect_four-1.2.2/test/test_no_opponant.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,105 +19,105 @@
     
     expected_model_view = np.array([
         [0, 0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 2, 0, 0, 0]
+        [0, 0, 0, -1, 0, 0, 0]
     ])
     
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 0
     board, rewards, dones, truncated, info = env.step(nextAction)
     
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [2, 0, 0, 1, 0, 0, 0]
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [-1, 0, 0, 1, 0, 0, 0]
     ])
     
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 3
     board, rewards, dones, truncated, info = env.step(nextAction)
     
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 2, 0, 0, 0],
-        [1, 0, 0, 2, 0, 0, 0]
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0, -1, 0, 0, 0],
+        [1, 0, 0, -1, 0, 0, 0]
     ])
     
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 0
     board, rewards, dones, truncated, info = env.step(nextAction)
     
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [2, 0, 0, 1, 0, 0, 0],
-        [2, 0, 0, 1, 0, 0, 0]
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [-1, 0, 0, 1, 0, 0, 0],
+        [-1, 0, 0, 1, 0, 0, 0]
     ])
     
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 3
     board, rewards, dones, truncated, info = env.step(nextAction)
     
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 2, 0, 0, 0],
-        [1, 0, 0, 2, 0, 0, 0],
-        [1, 0, 0, 2, 0, 0, 0]
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0, -1, 0, 0, 0],
+        [1, 0, 0, -1, 0, 0, 0],
+        [1, 0, 0, -1, 0, 0, 0]
     ])
     
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 0
     board, rewards, dones, truncated, info = env.step(nextAction)
     
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [2, 0, 0, 1, 0, 0, 0],
-        [2, 0, 0, 1, 0, 0, 0],
-        [2, 0, 0, 1, 0, 0, 0]
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ -1, 0, 0, 1, 0, 0, 0],
+        [ -1, 0, 0, 1, 0, 0, 0],
+        [ -1, 0, 0, 1, 0, 0, 0]
     ])
     
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 3
     board, rewards, dones, truncated, info = env.step(nextAction)
```

### Comparing `gymnasium_connect_four-1.2.1/test/test_power_4_logic.py` & `gymnasium_connect_four-1.2.2/test/test_power_4_logic.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,29 +18,29 @@
     board, rewards, dones, truncated, info = env.step(nextAction)
     
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_opponant_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 2, 0, 0, 0]
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0, -1, 0, 0, 0]
     ])
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [2, 0, 0, 1, 0, 0, 0]
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [-1, 0, 0, 1, 0, 0, 0]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
 
 def test_place_a_simple_game_horizontal_win():
@@ -54,116 +54,116 @@
     board, rewards, dones, truncated, info = env.step(nextAction)
     
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_opponant_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [2, 0, 0, 0, 0, 0, 0]
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [-1, 0, 0, 0, 0, 0, 0]
     ])
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [2, 0, 0, 0, 0, 0, 0],
-        [1, 0, 0, 0, 0, 0, 0]
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [-1, 0, 0, 0, 0, 0, 0],
+        [ 1, 0, 0, 0, 0, 0, 0]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 1
     simulatePlayer.set_next_move(1)
     board, rewards, dones, truncated, info = env.step(nextAction)
     
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_opponant_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [1, 0, 0, 0, 0, 0, 0],
-        [2, 2, 0, 0, 0, 0, 0]
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 1,  0, 0, 0, 0, 0, 0],
+        [-1, -1, 0, 0, 0, 0, 0]
     ])
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [2, 2, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0]
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [-1, -1, 0, 0, 0, 0, 0],
+        [ 1,  1, 0, 0, 0, 0, 0]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 2
     simulatePlayer.set_next_move(1)
     board, rewards, dones, truncated, info = env.step(nextAction)
     
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_opponant_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [2, 2, 2, 0, 0, 0, 0]
+        [ 0,  0,  0, 0, 0, 0, 0],
+        [ 0,  0,  0, 0, 0, 0, 0],
+        [ 0,  0,  0, 0, 0, 0, 0],
+        [ 0,  0,  0, 0, 0, 0, 0],
+        [ 1,  1,  0, 0, 0, 0, 0],
+        [-1, -1, -1, 0, 0, 0, 0]
     ])
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 2, 0, 0, 0, 0, 0],
-        [2, 2, 0, 0, 0, 0, 0],
-        [1, 1, 1, 0, 0, 0, 0]
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0, -1, 0, 0, 0, 0, 0],
+        [-1, -1, 0, 0, 0, 0, 0],
+        [ 1,  1, 1, 0, 0, 0, 0]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 3
     simulatePlayer.set_next_move(1)
     board, rewards, dones, truncated, info = env.step(nextAction)
     
     assert rewards == 1, f"Expected reward: 1 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == True, f"Expected dones: True but got {dones}"
     
     expected_opponant_view = np.array([ # he doesn't view your move because you win before
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [1, 1, 0, 0, 0, 0, 0],
-        [2, 2, 2, 0, 0, 0, 0]
+        [ 0,  0,  0, 0, 0, 0, 0],
+        [ 0,  0,  0, 0, 0, 0, 0],
+        [ 0,  0,  0, 0, 0, 0, 0],
+        [ 0,  0,  0, 0, 0, 0, 0],
+        [ 1,  1,  0, 0, 0, 0, 0],
+        [-1, -1, -1, 0, 0, 0, 0]
     ])
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 2, 0, 0, 0, 0, 0],
-        [2, 2, 0, 0, 0, 0, 0],
-        [1, 1, 1, 1, 0, 0, 0]
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0, -1, 0, 0, 0, 0, 0],
+        [-1, -1, 0, 0, 0, 0, 0],
+        [ 1,  1, 1, 1, 0, 0, 0]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
 def test_place_a_simple_game_vertical_win():
     simulatePlayer = SimulatePlayer()
@@ -175,107 +175,107 @@
     board, rewards, dones, truncated, info = env.step(nextAction)
     
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_opponant_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 2, 0, 0, 0, 0, 0]
+        [0,  0, 0, 0, 0, 0, 0],
+        [0,  0, 0, 0, 0, 0, 0],
+        [0,  0, 0, 0, 0, 0, 0],
+        [0,  0, 0, 0, 0, 0, 0],
+        [0,  0, 0, 0, 0, 0, 0],
+        [0, -1, 0, 0, 0, 0, 0]
     ])
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 1, 0, 2, 0, 0, 0]
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 1, 0, -1, 0, 0, 0]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 1
     simulatePlayer.set_next_move(6)
     board, rewards, dones, truncated, info = env.step(nextAction)
 
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_opponant_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 2, 0, 0, 0, 0, 0],
-        [0, 2, 0, 1, 0, 0, 0]
+        [0,  0, 0, 0, 0, 0, 0],
+        [0,  0, 0, 0, 0, 0, 0],
+        [0,  0, 0, 0, 0, 0, 0],
+        [0,  0, 0, 0, 0, 0, 0],
+        [0, -1, 0, 0, 0, 0, 0],
+        [0, -1, 0, 1, 0, 0, 0]
     ])
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 1, 0, 0, 0, 0, 0],
-        [0, 1, 0, 2, 0, 0, 2]
+        [0, 0, 0,  0, 0, 0,  0],
+        [0, 0, 0,  0, 0, 0,  0],
+        [0, 0, 0,  0, 0, 0,  0],
+        [0, 0, 0,  0, 0, 0,  0],
+        [0, 1, 0,  0, 0, 0,  0],
+        [0, 1, 0, -1, 0, 0, -1]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 1
     simulatePlayer.set_next_move(5)
     board, rewards, dones, truncated, info = env.step(nextAction)
 
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_opponant_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 2, 0, 0, 0, 0, 0],
-        [0, 2, 0, 0, 0, 0, 0],
-        [0, 2, 0, 1, 0, 0, 1]
+        [0,  0, 0, 0, 0, 0, 0],
+        [0,  0, 0, 0, 0, 0, 0],
+        [0,  0, 0, 0, 0, 0, 0],
+        [0, -1, 0, 0, 0, 0, 0],
+        [0, -1, 0, 0, 0, 0, 0],
+        [0, -1, 0, 1, 0, 0, 1]
     ])
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 1, 0, 0, 0, 0, 0],
-        [0, 1, 0, 0, 0, 0, 0],
-        [0, 1, 0, 2, 0, 2, 2]
+        [0, 0, 0,  0, 0,  0,  0],
+        [0, 0, 0,  0, 0,  0,  0],
+        [0, 0, 0,  0, 0,  0,  0],
+        [0, 1, 0,  0, 0,  0,  0],
+        [0, 1, 0,  0, 0,  0,  0],
+        [0, 1, 0, -1, 0, -1, -1]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 1
     simulatePlayer.set_next_move(4)
     board, rewards, dones, truncated, info = env.step(nextAction)
 
     assert rewards == 1, f"Expected reward: 1 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == True, f"Expected dones: True but got {dones}"
         
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 1, 0, 0, 0, 0, 0],
-        [0, 1, 0, 0, 0, 0, 0],
-        [0, 1, 0, 0, 0, 0, 0],
-        [0, 1, 0, 2, 0, 2, 2]
+        [0, 0, 0,  0, 0,  0,  0],
+        [0, 0, 0,  0, 0,  0,  0],
+        [0, 1, 0,  0, 0,  0,  0],
+        [0, 1, 0,  0, 0,  0,  0],
+        [0, 1, 0,  0, 0,  0,  0],
+        [0, 1, 0, -1, 0, -1, -1]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
 
 def test_place_a_simple_game_updiagonal_win():
@@ -288,165 +288,165 @@
     board, rewards, dones, truncated, info = env.step(nextAction)
     
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_opponant_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [2, 0, 0, 0, 0, 0, 0]
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [-1, 0, 0, 0, 0, 0, 0]
     ])
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [1, 2, 0, 0, 0, 0, 0]
+        [0,  0, 0, 0, 0, 0, 0],
+        [0,  0, 0, 0, 0, 0, 0],
+        [0,  0, 0, 0, 0, 0, 0],
+        [0,  0, 0, 0, 0, 0, 0],
+        [0,  0, 0, 0, 0, 0, 0],
+        [1, -1, 0, 0, 0, 0, 0]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 1
     simulatePlayer.set_next_move(2)
     board, rewards, dones, truncated, info = env.step(nextAction)
 
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_opponant_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 2, 0, 0, 0, 0, 0],
-        [2, 1, 0, 0, 0, 0, 0]
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0,  0, 0, 0, 0, 0, 0],
+        [ 0, -1, 0, 0, 0, 0, 0],
+        [-1,  1, 0, 0, 0, 0, 0]
     ])
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 1, 0, 0, 0, 0, 0],
-        [1, 2, 2, 0, 0, 0, 0]
+        [0,  0,  0, 0, 0, 0, 0],
+        [0,  0,  0, 0, 0, 0, 0],
+        [0,  0,  0, 0, 0, 0, 0],
+        [0,  0,  0, 0, 0, 0, 0],
+        [0,  1,  0, 0, 0, 0, 0],
+        [1, -1, -1, 0, 0, 0, 0]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 3
     simulatePlayer.set_next_move(2)
     board, rewards, dones, truncated, info = env.step(nextAction)
 
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_opponant_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 2, 0, 0, 0, 0, 0],
-        [2, 1, 1, 2, 0, 0, 0]
+        [ 0,  0, 0,  0, 0, 0, 0],
+        [ 0,  0, 0,  0, 0, 0, 0],
+        [ 0,  0, 0,  0, 0, 0, 0],
+        [ 0,  0, 0,  0, 0, 0, 0],
+        [ 0, -1, 0,  0, 0, 0, 0],
+        [-1,  1, 1, -1, 0, 0, 0]
     ])
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 1, 2, 0, 0, 0, 0],
-        [1, 2, 2, 1, 0, 0, 0]
+        [0,  0,  0, 0, 0, 0, 0],
+        [0,  0,  0, 0, 0, 0, 0],
+        [0,  0,  0, 0, 0, 0, 0],
+        [0,  0,  0, 0, 0, 0, 0],
+        [0,  1, -1, 0, 0, 0, 0],
+        [1, -1, -1, 1, 0, 0, 0]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 2
     simulatePlayer.set_next_move(3)
     board, rewards, dones, truncated, info = env.step(nextAction)
 
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_opponant_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 2, 0, 0, 0, 0],
-        [0, 2, 1, 0, 0, 0, 0],
-        [2, 1, 1, 2, 0, 0, 0]
+        [ 0,  0,  0,  0, 0, 0, 0],
+        [ 0,  0,  0,  0, 0, 0, 0],
+        [ 0,  0,  0,  0, 0, 0, 0],
+        [ 0,  0, -1,  0, 0, 0, 0],
+        [ 0, -1,  1,  0, 0, 0, 0],
+        [-1,  1,  1, -1, 0, 0, 0]
     ])
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 1, 0, 0, 0, 0],
-        [0, 1, 2, 2, 0, 0, 0],
-        [1, 2, 2, 1, 0, 0, 0]
+        [0,  0,  0,  0, 0, 0, 0],
+        [0,  0,  0,  0, 0, 0, 0],
+        [0,  0,  0,  0, 0, 0, 0],
+        [0,  0,  1,  0, 0, 0, 0],
+        [0,  1, -1, -1, 0, 0, 0],
+        [1, -1, -1,  1, 0, 0, 0]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"  
 
     nextAction = 2
     simulatePlayer.set_next_move(3)
     board, rewards, dones, truncated, info = env.step(nextAction)
 
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
     
     expected_opponant_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 2, 0, 0, 0, 0],
-        [0, 0, 2, 0, 0, 0, 0],
-        [0, 2, 1, 1, 0, 0, 0],
-        [2, 1, 1, 2, 0, 0, 0]
+        [ 0,  0,  0,  0, 0, 0, 0],
+        [ 0,  0,  0,  0, 0, 0, 0],
+        [ 0,  0, -1,  0, 0, 0, 0],
+        [ 0,  0, -1,  0, 0, 0, 0],
+        [ 0, -1,  1,  1, 0, 0, 0],
+        [-1,  1,  1, -1, 0, 0, 0]
     ])
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 1, 0, 0, 0, 0],
-        [0, 0, 1, 2, 0, 0, 0],
-        [0, 1, 2, 2, 0, 0, 0],
-        [1, 2, 2, 1, 0, 0, 0]
+        [0,  0,  0,  0, 0, 0, 0],
+        [0,  0,  0,  0, 0, 0, 0],
+        [0,  0,  1,  0, 0, 0, 0],
+        [0,  0,  1, -1, 0, 0, 0],
+        [0,  1, -1, -1, 0, 0, 0],
+        [1, -1, -1,  1, 0, 0, 0]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"   
 
     nextAction = 3
     simulatePlayer.set_next_move(3)
     board, rewards, dones, truncated, info = env.step(nextAction)
 
     assert rewards == 1, f"Expected reward: 1 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == True, f"Expected dones: True but got {dones}"
     
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 1, 1, 0, 0, 0],
-        [0, 0, 1, 2, 0, 0, 0],
-        [0, 1, 2, 2, 0, 0, 0],
-        [1, 2, 2, 1, 0, 0, 0]
+        [0,  0,  0,  0, 0, 0, 0],
+        [0,  0,  0,  0, 0, 0, 0],
+        [0,  0,  1,  1, 0, 0, 0],
+        [0,  0,  1, -1, 0, 0, 0],
+        [0,  1, -1, -1, 0, 0, 0],
+        [1, -1, -1,  1, 0, 0, 0]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"   
 
 def test_place_a_simple_game_downdiagonal_win():
     simulatePlayer = SimulatePlayer()
@@ -473,81 +473,81 @@
     simulatePlayer.set_next_move(1)
     board, rewards, dones, truncated, info = env.step(nextAction)
 
     nextAction = 2
     board, rewards, dones, truncated, info = env.step(nextAction)
 
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 1, 0, 0, 0, 0],
-        [0, 0, 1, 1, 0, 0, 0],
-        [0, 0, 2, 2, 1, 0, 0],
-        [0, 2, 1, 2, 2, 1, 0]
+        [0,  0,  0,  0,  0, 0, 0],
+        [0,  0,  0,  0,  0, 0, 0],
+        [0,  0,  1,  0,  0, 0, 0],
+        [0,  0,  1,  1,  0, 0, 0],
+        [0,  0, -1, -1,  1, 0, 0],
+        [0, -1,  1, -1, -1, 1, 0]
     ])
 
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     assert rewards == 1, f"Expected reward: 1 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == True, f"Expected dones: True but got {dones}"
 
 def test_second_player_can_begin():
     simulatePlayer = SimulatePlayer()
 
 
-    env = ConnectFourEnv(opponent=simulatePlayer,first_player=2)
+    env = ConnectFourEnv(opponent=simulatePlayer,first_player=-1)
     simulatePlayer.set_next_move(0)
     board, _ = env.reset(seed=0)
     
     expected_opponant_view = np.array([
         [0, 0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0, 0],
         [0, 0, 0, 0, 0, 0, 0]
     ])
 
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [2, 0, 0, 0, 0, 0, 0]
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [ 0, 0, 0, 0, 0, 0, 0],
+        [-1, 0, 0, 0, 0, 0, 0]
     ])
 
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     nextAction = 3
     simulatePlayer.set_next_move(4)
     board, rewards, dones, truncated, info = env.step(nextAction)
     
     assert rewards == 0, f"Expected reward: 0 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == False, f"Expected dones: False but got {dones}"
 
     expected_opponant_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [1, 0, 0, 2, 0, 0, 0]
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [0, 0, 0,  0, 0, 0, 0],
+        [1, 0, 0, -1, 0, 0, 0]
     ])
 
     expected_model_view = np.array([
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [0, 0, 0, 0, 0, 0, 0],
-        [2, 0, 0, 1, 2, 0, 0]
+        [ 0, 0, 0, 0,  0, 0, 0],
+        [ 0, 0, 0, 0,  0, 0, 0],
+        [ 0, 0, 0, 0,  0, 0, 0],
+        [ 0, 0, 0, 0,  0, 0, 0],
+        [ 0, 0, 0, 0,  0, 0, 0],
+        [-1, 0, 0, 1, -1, 0, 0]
     ])
 
     
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
```

### Comparing `gymnasium_connect_four-1.2.1/test/test_ppo_env.py` & `gymnasium_connect_four-1.2.2/test/test_ppo_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,21 +24,21 @@
         obs, rewards, dones, truncated, info = env.step(action)
 
         if truncated or dones:
             allrewards.append(rewards)
             obs, _ = env.reset()
 
     # Check if the model is deterministic
-    assert np.sum(allrewards) == 8, "The model is not determinist"
+    assert np.sum(allrewards) == 7, "The model is not determinist"
 
 
 def test_is_working_with_ppo():
     # Initialize the environment and the PPO model
     env = ConnectFourEnv(opponent=BabyPlayer())
-    model = PPO("MlpPolicy", env, verbose=0, seed=0)
+    model = PPO("MlpPolicy", env, verbose=0, seed=1)
 
     # Train the model
     model.learn(total_timesteps=10000)
 
     # Test the model's performance
     obs, _ = env.reset(seed=0)
     allrewards = []
```

