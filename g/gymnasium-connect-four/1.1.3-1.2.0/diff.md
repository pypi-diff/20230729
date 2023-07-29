# Comparing `tmp/gymnasium_connect_four-1.1.3.tar.gz` & `tmp/gymnasium_connect_four-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_connect_four-1.1.3.tar", last modified: Sat Jul 29 07:25:06 2023, max compression
+gzip compressed data, was "gymnasium_connect_four-1.2.0.tar", last modified: Sat Jul 29 14:21:58 2023, max compression
```

## Comparing `gymnasium_connect_four-1.1.3.tar` & `gymnasium_connect_four-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 07:25:06.970677 gymnasium_connect_four-1.1.3/
--rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      251 2023-07-29 07:25:06.969678 gymnasium_connect_four-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    11859 2023-07-29 06:01:04.000000 gymnasium_connect_four-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 07:25:06.925670 gymnasium_connect_four-1.1.3/connect_four_gymnasium/
--rw-rw-rw-   0        0        0     8882 2023-07-29 07:23:53.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/ConnectFourEnv.py
--rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 07:25:06.950672 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/
--rw-rw-rw-   0        0        0     4253 2023-07-24 06:32:12.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/AdultPlayer.py
--rw-rw-rw-   0        0        0     3753 2023-07-24 17:50:51.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/AdultSmarterPlayer.py
--rw-rw-rw-   0        0        0      338 2023-07-24 06:32:47.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/BabyPlayer.py
--rw-rw-rw-   0        0        0     1596 2023-07-25 19:50:41.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/ChildPlayer.py
--rw-rw-rw-   0        0        0     1946 2023-07-24 06:32:30.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/ChildSmarterPlayer.py
--rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/ConsolePlayer.py
--rw-rw-rw-   0        0        0     4118 2023-07-24 06:02:34.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/MinMaxPlayer.py
--rw-rw-rw-   0        0        0      545 2023-07-24 21:26:20.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/ModelPlayer.py
--rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/Player.py
--rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/SimulatePlayer.py
--rw-rw-rw-   0        0        0     2609 2023-07-24 06:32:25.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/TeenagerPlayer.py
--rw-rw-rw-   0        0        0     3999 2023-07-24 06:32:20.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
--rw-rw-rw-   0        0        0      486 2023-07-25 11:49:49.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 07:25:06.953671 gymnasium_connect_four-1.1.3/connect_four_gymnasium/tools/
--rw-rw-rw-   0        0        0     4914 2023-07-25 19:51:32.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/tools/EloLeaderboard.py
--rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.1.3/connect_four_gymnasium/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 07:25:06.962671 gymnasium_connect_four-1.1.3/gymnasium_connect_four.egg-info/
--rw-rw-rw-   0        0        0      251 2023-07-29 07:25:06.000000 gymnasium_connect_four-1.1.3/gymnasium_connect_four.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2023-07-29 07:25:06.000000 gymnasium_connect_four-1.1.3/gymnasium_connect_four.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 07:25:06.000000 gymnasium_connect_four-1.1.3/gymnasium_connect_four.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-29 07:25:06.000000 gymnasium_connect_four-1.1.3/gymnasium_connect_four.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-29 07:25:06.000000 gymnasium_connect_four-1.1.3/gymnasium_connect_four.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 07:25:06.971681 gymnasium_connect_four-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-07-29 07:24:51.000000 gymnasium_connect_four-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 07:25:06.967678 gymnasium_connect_four-1.1.3/test/
--rw-rw-rw-   0        0        0     4688 2023-07-29 06:40:16.000000 gymnasium_connect_four-1.1.3/test/test_no_opponant.py
--rw-rw-rw-   0        0        0    21167 2023-07-25 14:09:28.000000 gymnasium_connect_four-1.1.3/test/test_power_4_logic.py
--rw-rw-rw-   0        0        0     2373 2023-07-23 20:26:41.000000 gymnasium_connect_four-1.1.3/test/test_ppo_env.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:21:58.132609 gymnasium_connect_four-1.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-07-29 14:21:58.128083 gymnasium_connect_four-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10857 2023-07-29 14:18:53.000000 gymnasium_connect_four-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 14:21:58.088074 gymnasium_connect_four-1.2.0/connect_four_gymnasium/
+-rw-rw-rw-   0        0        0     8934 2023-07-29 11:26:49.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/ConnectFourEnv.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:21:58.109524 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/
+-rw-rw-rw-   0        0        0     4648 2023-07-29 14:16:55.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/AdultPlayer.py
+-rw-rw-rw-   0        0        0     4372 2023-07-29 14:16:50.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/AdultSmarterPlayer.py
+-rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/BabyPlayer.py
+-rw-rw-rw-   0        0        0     1881 2023-07-29 14:17:29.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/ChildPlayer.py
+-rw-rw-rw-   0        0        0     2246 2023-07-29 14:17:21.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/ChildSmarterPlayer.py
+-rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/ConsolePlayer.py
+-rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/ModelPlayer.py
+-rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/Player.py
+-rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/SimulatePlayer.py
+-rw-rw-rw-   0        0        0     3159 2023-07-29 14:17:15.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/TeenagerPlayer.py
+-rw-rw-rw-   0        0        0     4374 2023-07-29 14:17:06.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
+-rw-rw-rw-   0        0        0      446 2023-07-29 10:59:21.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:21:58.109524 gymnasium_connect_four-1.2.0/connect_four_gymnasium/tools/
+-rw-rw-rw-   0        0        0     3319 2023-07-29 14:17:42.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/tools/EloLeaderboard.py
+-rw-rw-rw-   0        0        0     4744 2023-07-29 14:17:37.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/tools/Update_bot_elo.py
+-rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.0/connect_four_gymnasium/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:21:58.123066 gymnasium_connect_four-1.2.0/gymnasium_connect_four.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-07-29 14:21:57.000000 gymnasium_connect_four-1.2.0/gymnasium_connect_four.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2023-07-29 14:21:57.000000 gymnasium_connect_four-1.2.0/gymnasium_connect_four.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 14:21:57.000000 gymnasium_connect_four-1.2.0/gymnasium_connect_four.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-29 14:21:57.000000 gymnasium_connect_four-1.2.0/gymnasium_connect_four.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-29 14:21:57.000000 gymnasium_connect_four-1.2.0/gymnasium_connect_four.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 14:21:58.132609 gymnasium_connect_four-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-07-29 10:31:22.000000 gymnasium_connect_four-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:21:58.128083 gymnasium_connect_four-1.2.0/test/
+-rw-rw-rw-   0        0        0     4688 2023-07-29 06:40:16.000000 gymnasium_connect_four-1.2.0/test/test_no_opponant.py
+-rw-rw-rw-   0        0        0    21167 2023-07-25 14:09:28.000000 gymnasium_connect_four-1.2.0/test/test_power_4_logic.py
+-rw-rw-rw-   0        0        0     2372 2023-07-29 10:38:54.000000 gymnasium_connect_four-1.2.0/test/test_ppo_env.py
```

### Comparing `gymnasium_connect_four-1.1.3/LICENSE` & `gymnasium_connect_four-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.3/README.md` & `gymnasium_connect_four-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -60,33 +60,16 @@
 
 One powerful technique for training AI models is self-play, where the AI learns by playing against itself. This approach, famously used by AlphaGo Zero, has several advantages:
 
 - **Unbiased learning**: By playing against itself, the AI model is not influenced by human strategies or methods. This allows the model to develop its own unique strategies and potentially discover new ways of playing the game.
 - **Continuous improvement**: As the AI model improves, it continually faces a stronger opponent (itself), which helps it to learn more advanced strategies and refine its gameplay.
 - **Adaptive learning**: The AI model can adapt to its own weaknesses and exploit them, leading to a more robust and well-rounded understanding of the game.
 
-Here's an example of how to set up self-play training:
+You can directly test self-play training in the provided [Colab Notebook](https://colab.research.google.com/github/lucasBertola/Connect-4-Gym-env-Reinforcement-learning/blob/main/exemples/Self_play_training.ipynb).
 
-```python
-from connect_four_gymnasium import ConnectFourEnv, ModelPlayer
-from stable_baselines3 import PPO
-
-env = ConnectFourEnv(opponent=BabyPlayer())
-model = PPO("MlpPolicy", env, verbose=1)
-opponent = ModelPlayer(model, name="yourself")
-env.change_opponent(opponent)
-
-model.learn(total_timesteps=10000)
-```
-
-In this example, , we create a `ModelPlayer` using the model and set it as the opponent for the environment. This allows the AI model to continue learning by playing against itself.
-
-You can directly test self-play training in the provided Google Colab notebook at the following link:
-
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lucasBertola/Connect-4-Gym-env-Reinforcement-learning/blob/main/exemples/Self_play_training.ipynb)
 
 ## Environment Details
 
 In this section, we provide an overview of the Connect Four environment, including the action space, observation space, rewards, and episode termination conditions.
 
 ### Action Space
 
@@ -133,16 +116,14 @@
 
 ```python
 env = ConnectFourEnv(opponent=BabyPlayer())
 ```
 
 ### Player Descriptions
 
-- **MinMaxPlayer**: An implementation of the Minimax algorithm. Can be used with different search depths (e.g., `MinMaxPlayer(depth=3)`), but it is very slow, so it is not recommended for general use. All other algorithms are much faster.
-
 - **BabyPlayer**: Plays random moves.
 
 - **ChildPlayer**: Plays random moves, but if there is a winning move, it will play it.
 
 - **ChildSmarterPlayer**: Same as ChildPlayer, but if there is a move that would make the opponent win, it will play that move to block the opponent.
 
 - **TeenagerPlayer**: Same as ChildSmarterPlayer, but excludes moves that would allow the opponent to win if they play on top of it.
@@ -156,24 +137,21 @@
 - **ConsolePlayer**: Asks for moves to play in the console. Perfect for testing your own AI.
 
 ### Elo Ratings
 
 Here are the Elo ratings of the different algorithms:
 
 ```
-1. AdultSmarterPlayer:    1767
-2. AdultPlayer:           1712
-3. MinimaxPlayer depth 3: 1672
-4. MinimaxPlayer depth 2: 1622
-5. TeenagerSmarterPlayer: 1611
-6. TeenagerPlayer:        1604
-7. ChildSmarterPlayer:    1525
-8. MinimaxPlayer depth 1: 1220
-9. ChildPlayer:           1208
-10. BabyPlayer:            995
+1.  AdultSmarterPlayer:    1790
+2.  AdultPlayer:           1654
+5.  TeenagerSmarterPlayer: 1647
+6.  TeenagerPlayer:        1639
+7.  ChildSmarterPlayer:    1571
+9.  ChildPlayer:           1222
+10. BabyPlayer:            1000
 ```
 
 In addition to the provided players, we also offer a tool to evaluate the Elo rating of your own AI model. This is extremely useful to have an "absolute" idea of the progress of your AI. For example, if an AI learns by fighting against itself, we know that it is getting stronger as it would be able to win against its older versions, but this is not enough to evaluate if it has learned a lot. This is where our tool comes in, which allows you to give an Elo rating to the AI.
 
 Here is how to use it in Python:
 
 ```python
```

#### html2text {}

```diff
@@ -54,96 +54,83 @@
 By playing against itself, the AI model is not influenced by human strategies
 or methods. This allows the model to develop its own unique strategies and
 potentially discover new ways of playing the game. - **Continuous
 improvement**: As the AI model improves, it continually faces a stronger
 opponent (itself), which helps it to learn more advanced strategies and refine
 its gameplay. - **Adaptive learning**: The AI model can adapt to its own
 weaknesses and exploit them, leading to a more robust and well-rounded
-understanding of the game. Here's an example of how to set up self-play
-training: ```python from connect_four_gymnasium import ConnectFourEnv,
-ModelPlayer from stable_baselines3 import PPO env = ConnectFourEnv
-(opponent=BabyPlayer()) model = PPO("MlpPolicy", env, verbose=1) opponent =
-ModelPlayer(model, name="yourself") env.change_opponent(opponent) model.learn
-(total_timesteps=10000) ``` In this example, , we create a `ModelPlayer` using
-the model and set it as the opponent for the environment. This allows the AI
-model to continue learning by playing against itself. You can directly test
-self-play training in the provided Google Colab notebook at the following link:
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
-(https://colab.research.google.com/github/lucasBertola/Connect-4-Gym-env-
-Reinforcement-learning/blob/main/exemples/Self_play_training.ipynb) ##
-Environment Details In this section, we provide an overview of the Connect Four
-environment, including the action space, observation space, rewards, and
-episode termination conditions. ### Action Space The action space in the
-Connect Four environment is discrete, with a total of 7 possible actions. Each
-action corresponds to a column in the game board where a player can drop their
-piece. The action space is represented as follows: ```python self.action_space
-= spaces.Discrete(self.COLUMNS_COUNT) ``` ### Observation Space The observation
-space in the Connect Four environment is a 2D array representing the game
-board. Each cell in the array can have one of three possible values: 0 (empty),
-1 (player's piece), or 2 (opponent's piece). The observation space is defined
-as follows: ```python self.observation_space = spaces.Box(low=0, high=2, shape=
-(self.ROWS_COUNT, self.COLUMNS_COUNT), dtype=np.int32) ``` ### Rewards The
-reward system in the Connect Four environment is designed to encourage the AI
-model to learn how to win the game. The rewards are as follows: - A reward of
-+1 is given when the AI model wins the game by connecting four of its pieces in
-a row, either horizontally, vertically, or diagonally. - A reward of -1 is
-given when the AI model loses the game or plays an invalid action. - A reward
-of 0 is given for all other actions that do not result in a win or loss. ###
-Episode Termination An episode in the Connect Four environment terminates under
-the following conditions: - The AI model wins the game by connecting four of
-its pieces in a row, either horizontally, vertically, or diagonally. - The AI
-model loses the game by allowing the opponent to connect four of their pieces
-in a row, or by playing an invalid action. - The game board is completely
-filled, resulting in a draw. When an episode terminates, the environment is
-reset, and a new episode begins. ## Available Players This library provides a
-collection of Connect Four bots with different skill levels. These bots can be
-used for various purposes, such as: - **Learning by playing against them**: You
-can improve your AI model by playing against these bots, which range from
-beginner to advanced levels. - **Comparing the level of self-learning models**:
-By playing against these bots, you can evaluate the performance of your self-
-learning model and position it in terms of skill level and elo. You can
-integrate players as opponents in your gym environment like this: ```python env
-= ConnectFourEnv(opponent=BabyPlayer()) ``` ### Player Descriptions -
-**MinMaxPlayer**: An implementation of the Minimax algorithm. Can be used with
-different search depths (e.g., `MinMaxPlayer(depth=3)`), but it is very slow,
-so it is not recommended for general use. All other algorithms are much faster.
-- **BabyPlayer**: Plays random moves. - **ChildPlayer**: Plays random moves,
-but if there is a winning move, it will play it. - **ChildSmarterPlayer**: Same
-as ChildPlayer, but if there is a move that would make the opponent win, it
-will play that move to block the opponent. - **TeenagerPlayer**: Same as
-ChildSmarterPlayer, but excludes moves that would allow the opponent to win if
-they play on top of it. - **TeenagerSmarterPlayer**: Same as TeenagerPlayer,
-but checks if a move creates a line of three tokens with available spaces on
-both sides. If so, it will play that move. - **AdultPlayer**: Same as
-TeenagerSmarterPlayer, but also checks if a move creates a line of three tokens
-with available spaces on both sides for the opponent. If so, it will play that
-move to block the opponent. - **AdultSmarterPlayer**: Same as AdultPlayer, but
-checks if a move allows to create multiple ways to win and plays that move.
-Also checks if a move allows the opponent to create multiple ways to win and
-plays that move to protect itself. - **ConsolePlayer**: Asks for moves to play
-in the console. Perfect for testing your own AI. ### Elo Ratings Here are the
-Elo ratings of the different algorithms: ``` 1. AdultSmarterPlayer: 1767 2.
-AdultPlayer: 1712 3. MinimaxPlayer depth 3: 1672 4. MinimaxPlayer depth 2: 1622
-5. TeenagerSmarterPlayer: 1611 6. TeenagerPlayer: 1604 7. ChildSmarterPlayer:
-1525 8. MinimaxPlayer depth 1: 1220 9. ChildPlayer: 1208 10. BabyPlayer: 995
-``` In addition to the provided players, we also offer a tool to evaluate the
-Elo rating of your own AI model. This is extremely useful to have an "absolute"
-idea of the progress of your AI. For example, if an AI learns by fighting
-against itself, we know that it is getting stronger as it would be able to win
-against its older versions, but this is not enough to evaluate if it has
-learned a lot. This is where our tool comes in, which allows you to give an Elo
-rating to the AI. Here is how to use it in Python: ```python env =
-ConnectFourEnv(opponent=BabyPlayer()) model = PPO("MlpPolicy", env) model.learn
-(total_timesteps=10000) myModelPlayer = ModelPlayer(model,name="Your trained
-Model") your_model_elo = EloLeaderboard().get_elo([myModelPlayer],
-num_matches=100) ``` You can find an example of how to use this tool in a
-Google Colab notebook [here](https://colab.research.google.com/github/
+understanding of the game. You can directly test self-play training in the
+provided [Colab Notebook](https://colab.research.google.com/github/
 lucasBertola/Connect-4-Gym-env-Reinforcement-learning/blob/main/exemples/
-Train_ppo_and_test.ipynb). ## Testing We believe in the importance of testing.
-That's why we have included a suite of tests in the `test` directory. To run
-the tests, simply use the command `pytest`. ## Contribute & Support We warmly
-welcome contributions from the community. If you have an idea for an
-improvement or found a bug, don't hesitate to open an issue or submit a pull
-request. Your input is greatly appreciated, and our project is made better by
-your participation! If you find this repository useful, please give it a star!
-## License This project is licensed under the MIT License. See the `LICENSE`
-file for details.
+Self_play_training.ipynb). ## Environment Details In this section, we provide
+an overview of the Connect Four environment, including the action space,
+observation space, rewards, and episode termination conditions. ### Action
+Space The action space in the Connect Four environment is discrete, with a
+total of 7 possible actions. Each action corresponds to a column in the game
+board where a player can drop their piece. The action space is represented as
+follows: ```python self.action_space = spaces.Discrete(self.COLUMNS_COUNT) ```
+### Observation Space The observation space in the Connect Four environment is
+a 2D array representing the game board. Each cell in the array can have one of
+three possible values: 0 (empty), 1 (player's piece), or 2 (opponent's piece).
+The observation space is defined as follows: ```python self.observation_space =
+spaces.Box(low=0, high=2, shape=(self.ROWS_COUNT, self.COLUMNS_COUNT),
+dtype=np.int32) ``` ### Rewards The reward system in the Connect Four
+environment is designed to encourage the AI model to learn how to win the game.
+The rewards are as follows: - A reward of +1 is given when the AI model wins
+the game by connecting four of its pieces in a row, either horizontally,
+vertically, or diagonally. - A reward of -1 is given when the AI model loses
+the game or plays an invalid action. - A reward of 0 is given for all other
+actions that do not result in a win or loss. ### Episode Termination An episode
+in the Connect Four environment terminates under the following conditions: -
+The AI model wins the game by connecting four of its pieces in a row, either
+horizontally, vertically, or diagonally. - The AI model loses the game by
+allowing the opponent to connect four of their pieces in a row, or by playing
+an invalid action. - The game board is completely filled, resulting in a draw.
+When an episode terminates, the environment is reset, and a new episode begins.
+## Available Players This library provides a collection of Connect Four bots
+with different skill levels. These bots can be used for various purposes, such
+as: - **Learning by playing against them**: You can improve your AI model by
+playing against these bots, which range from beginner to advanced levels. -
+**Comparing the level of self-learning models**: By playing against these bots,
+you can evaluate the performance of your self-learning model and position it in
+terms of skill level and elo. You can integrate players as opponents in your
+gym environment like this: ```python env = ConnectFourEnv(opponent=BabyPlayer
+()) ``` ### Player Descriptions - **BabyPlayer**: Plays random moves. -
+**ChildPlayer**: Plays random moves, but if there is a winning move, it will
+play it. - **ChildSmarterPlayer**: Same as ChildPlayer, but if there is a move
+that would make the opponent win, it will play that move to block the opponent.
+- **TeenagerPlayer**: Same as ChildSmarterPlayer, but excludes moves that would
+allow the opponent to win if they play on top of it. -
+**TeenagerSmarterPlayer**: Same as TeenagerPlayer, but checks if a move creates
+a line of three tokens with available spaces on both sides. If so, it will play
+that move. - **AdultPlayer**: Same as TeenagerSmarterPlayer, but also checks if
+a move creates a line of three tokens with available spaces on both sides for
+the opponent. If so, it will play that move to block the opponent. -
+**AdultSmarterPlayer**: Same as AdultPlayer, but checks if a move allows to
+create multiple ways to win and plays that move. Also checks if a move allows
+the opponent to create multiple ways to win and plays that move to protect
+itself. - **ConsolePlayer**: Asks for moves to play in the console. Perfect for
+testing your own AI. ### Elo Ratings Here are the Elo ratings of the different
+algorithms: ``` 1. AdultSmarterPlayer: 1790 2. AdultPlayer: 1654 5.
+TeenagerSmarterPlayer: 1647 6. TeenagerPlayer: 1639 7. ChildSmarterPlayer: 1571
+9. ChildPlayer: 1222 10. BabyPlayer: 1000 ``` In addition to the provided
+players, we also offer a tool to evaluate the Elo rating of your own AI model.
+This is extremely useful to have an "absolute" idea of the progress of your AI.
+For example, if an AI learns by fighting against itself, we know that it is
+getting stronger as it would be able to win against its older versions, but
+this is not enough to evaluate if it has learned a lot. This is where our tool
+comes in, which allows you to give an Elo rating to the AI. Here is how to use
+it in Python: ```python env = ConnectFourEnv(opponent=BabyPlayer()) model = PPO
+("MlpPolicy", env) model.learn(total_timesteps=10000) myModelPlayer =
+ModelPlayer(model,name="Your trained Model") your_model_elo = EloLeaderboard
+().get_elo([myModelPlayer], num_matches=100) ``` You can find an example of how
+to use this tool in a Google Colab notebook [here](https://
+colab.research.google.com/github/lucasBertola/Connect-4-Gym-env-Reinforcement-
+learning/blob/main/exemples/Train_ppo_and_test.ipynb). ## Testing We believe in
+the importance of testing. That's why we have included a suite of tests in the
+`test` directory. To run the tests, simply use the command `pytest`. ##
+Contribute & Support We warmly welcome contributions from the community. If you
+have an idea for an improvement or found a bug, don't hesitate to open an issue
+or submit a pull request. Your input is greatly appreciated, and our project is
+made better by your participation! If you find this repository useful, please
+give it a star! ## License This project is licensed under the MIT License. See
+the `LICENSE` file for details.
```

### Comparing `gymnasium_connect_four-1.1.3/connect_four_gymnasium/ConnectFourEnv.py` & `gymnasium_connect_four-1.2.0/connect_four_gymnasium/ConnectFourEnv.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,16 @@
             self.next_player_to_play = np.random.choice([1, 2])
         else:
             self.next_player_to_play = self.first_player
 
         if self.opponent is not None:
             if self.next_player_to_play == 2:
                 opponent_action = self.opponent.play(self._board)
-                result = self.play_action(opponent_action, self.next_player_to_play)
-                if result != 0:
+                result, isFinish = self.play_action(opponent_action, self.next_player_to_play)
+                if isFinish :
                     print('wtf')
                     print(opponent_action)
                     exit("The opponent played an invalid action in the first move!")
                 self.next_player_to_play = 1
 
             self.render_for_human()
 
@@ -68,30 +68,30 @@
         return self._board[0, column] != 0
 
     def is_action_valid(self, action):
         return action >= self.MIN_INDEX_TO_PLAY and action < self.COLUMNS_COUNT and not self.is_column_full(action)
 
     def play_action(self, action, player):
         if not self.is_action_valid(action):
-            return -1
+            return -1, True
 
         last_move_row = self.drop_piece(action, player)
 
         self.render_for_human()
 
         if self.check_win_around_last_move(player, last_move_row, action):
             if self.render_mode == "human":
                 print("You won!")
                 time.sleep(5)
-            return 1
+            return 1, True
         
         if self.board_is_full():
-            return 0
+            return 0, True
 
-        return 0
+        return 0, False
 
     def board_is_full(self):
         return np.all(self._board != 0)
     
     def inverse_player_position(self):
         new_board = np.zeros_like(self._board)
         new_board[self._board == 1] = 2
@@ -100,17 +100,18 @@
 
     def switch_player(self):
         self.next_player_to_play = 3 - self.next_player_to_play
         
     def step(self, action, play_opponent=True):
         action = action.item() if isinstance(action, np.ndarray) else action
 
-        result = self.play_action(action, self.next_player_to_play)
-        if result != 0:
+        result, is_finish = self.play_action(action, self.next_player_to_play)
+        if is_finish:
             return self._board, result, True, False, {}
+        
         self.switch_player()
 
         if  play_opponent and self.opponent is not None:
             # because 1 is you, 2 is the opponent
             # you need to see the board as the opponent sees it
             opponent_action = self.opponent.play(self.inverse_player_position())
             opponent_result = self.step(opponent_action, play_opponent=False)
```

### Comparing `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/AdultPlayer.py` & `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/AdultSmarterPlayer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,105 +1,116 @@
 import numpy as np
 from .Player import Player
 
-class AdultPlayer(Player):
-    
+class AdultSmarterPlayer(Player):
+
     def __init__(self, _=""):
         pass
-    
-    def play(self, observation):
+
+    def play_single(self, observation):
         moves_to_avoid = []
 
-        # Check for a winning move for the player
+        # Check if there is a winning move for the player
         for move in range(7):
             if observation[0, move] == 0:
-                new_board = self.apply_move(observation, move, 1)
-                if self.check_win(new_board, 1):
+                new_board, row, col = self.apply_move(observation, move, 1)
+                if self.check_win_around_last_move(new_board, 1, row, col):
                     return move
 
-        # Check for a winning move for the opponent
+        # Check if there is a winning move for the opponent
         for move in range(7):
             if observation[0, move] == 0:
-                new_board = self.apply_move(observation, move, 2)
-                if self.check_win(new_board, 2):
+                new_board, row, col = self.apply_move(observation, move, 2)
+                if self.check_win_around_last_move(new_board, 2, row, col):
                     return move
 
         # Check if a move allows the opponent to win by playing the same move again
         for move in range(7):
             if observation[0, move] == 0:
-                new_board = self.apply_move(observation, move, 1)
-                new_board = self.apply_move(new_board, move, 2)
-                if self.check_win(new_board, 2):
-                    moves_to_avoid.append(move)
+                new_board, row, col = self.apply_move(observation, move, 1)
+                if new_board[0, move] == 0:
+                    new_board, row, col = self.apply_move(new_board, move, 2)
+                    if self.check_win_around_last_move(new_board, 2, row, col):
+                        moves_to_avoid.append(move)
 
-        # Check if a move creates a line of three tokens with available spaces on both sides
+        # Check if a move creates multiple ways to win for the player
         for move in range(7):
             if observation[0, move] == 0:
-                new_board = self.apply_move(observation, move, 1)
-                if self.check_three_in_a_row(new_board, 1) and move not in moves_to_avoid:
+                new_board, row, col = self.apply_move(observation, move, 1)
+                if self.check_multiple_ways_to_win(new_board, 1) and move not in moves_to_avoid:
                     return move
-        
+
+        # Check if a move allows the opponent to create multiple ways to win
         for move in range(7):
             if observation[0, move] == 0:
-                new_board = self.apply_move(observation, move, 2)
-                if self.check_three_in_a_row(new_board, 2) and move not in moves_to_avoid:
+                new_board, row, col = self.apply_move(observation, move, 2)
+                if self.check_multiple_ways_to_win(new_board, 2) and move not in moves_to_avoid:
                     return move
 
-        # Play a random move among valid moves, excluding moves_to_avoid
+        # Play a random move among the valid moves, except those in moves_to_avoid
         valid_moves = [c for c in range(7) if observation[0, c] == 0 and c not in moves_to_avoid]
 
         # If valid_moves is empty, choose a random move among all possible moves
         if not valid_moves:
             valid_moves = [c for c in range(7) if observation[0, c] == 0]
+        
+        if not valid_moves:
+            print('no valid_move.. i don t want to suicide myself',valid_moves,observation)
+            exit()
 
         return np.random.choice(valid_moves)
 
-    def getName(self):
-        return "AdultPlayer"
+    def play(self, obs):
+        if isinstance(obs, list):
+            return [self.play_single(o) for o in obs]
+        else:
+            return self.play_single(obs)
 
-    def getElo(self):
-        return 1712
-    
-    def isDeterministic(self):
+    def check_multiple_ways_to_win(self, board, player):
+        win_count = 0
+        for move in range(7):
+            if board[0, move] == 0:
+                new_board, row, col = self.apply_move(board, move, player)
+                if self.check_win_around_last_move(new_board, player, row, col):
+                    win_count += 1
+                    if win_count >= 2:
+                        return True
         return False
-
+    
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
             if new_board[i, move] == 0:
                 new_board[i, move] = player
-                break
-        return new_board
+                return new_board, i, move
+        print('wtf')
+        exit()
+
+    def check_win_around_last_move(self, board, player, row, col):
+        directions = [
+            (1, 0),  # horizontal
+            (0, 1),  # vertical
+            (1, 1),  # diagonal /
+            (1, -1)  # diagonal \
+        ]
+
+        for dr, dc in directions:
+            count = 0
+            for step in range(-3, 4):
+                r, c = row + step * dr, col + step * dc
+                if 0 <= r < 6 and 0 <= c < 7 and board[r, c] == player:
+                    count += 1
+                    if count == 4:
+                        return True
+                else:
+                    count = 0
 
-    def check_win(self, board, player):
-        for i in range(6):
-            for j in range(4):
-                if (board[i, j:j+4] == player).all():
-                    return True
-        for i in range(3):
-            for j in range(7):
-                if (board[i:i+4, j] == player).all():
-                    return True
-        for i in range(3):
-            for j in range(4):
-                if (board[i:i+4, j:j+4].diagonal() == player).all():
-                    return True
-                if (board[i:i+4, j:j+4][::-1].diagonal() == player).all():
-                    return True
         return False
 
-    def check_three_in_a_row(self, board, player):
-        for i in range(6):
-            for j in range(5):
-                if (board[i, j:j+3] == player).all() and (j-1 >= 0) and board[i, j-1] == 0 and (j+3 < 7) and board[i, j+3] == 0:
-                    return True
-        for i in range(4):
-            for j in range(7):
-                if (board[i:i+3, j] == player).all() and (i-1 >= 0) and board[i-1, j] == 0 and (i+3 < 6) and board[i+3, j] == 0:
-                    return True
-        for i in range(4):
-            for j in range(5):
-                if (board[i:i+3, j:j+3].diagonal() == player).all() and (i-1 >= 0) and (j-1 >= 0) and board[i-1, j-1] == 0 and (i+3 < 6) and (j+3 < 7) and board[i+3, j+3] == 0:
-                    return True
-                if (board[i:i+3, j:j+3][::-1].diagonal() == player).all() and (i-1 >= 0) and (j+2 < 7) and board[i-1, j+2] == 0 and (i+3 < 6) and (j-1 >= 0) and board[i+3, j-1] == 0:
-                    return True
+    def getName(self):
+        return "AdultSmarterPlayer"
+    
+    def getElo(self):
+        return 1790
+    
+    def isDeterministic(self):
         return False
```

### Comparing `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/AdultSmarterPlayer.py` & `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/TeenagerSmarterPlayer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,119 @@
 import numpy as np
 from .Player import Player
 
-class AdultSmarterPlayer(Player):
+class TeenagerSmarterPlayer(Player):
 
     def __init__(self, _=""):
         pass
     
-    def play(self, observation):
+    def play_single(self, observation):
         moves_to_avoid = []
 
-        # Check if there is a winning move for the player
+        # Check for a winning move for the player
         for move in range(7):
             if observation[0, move] == 0:
-                new_board = self.apply_move(observation, move, 1)
-                if self.check_win(new_board, 1):
+                new_board, row, col = self.apply_move(observation, move, 1)
+                if self.check_win_around_last_move(new_board, 1, row, col):
                     return move
 
-        # Check if there is a winning move for the opponent
+        # Check for a winning move for the opponent
         for move in range(7):
             if observation[0, move] == 0:
-                new_board = self.apply_move(observation, move, 2)
-                if self.check_win(new_board, 2):
+                new_board, row, col = self.apply_move(observation, move, 2)
+                if self.check_win_around_last_move(new_board, 2, row, col):
                     return move
 
         # Check if a move allows the opponent to win by playing the same move again
         for move in range(7):
             if observation[0, move] == 0:
-                new_board = self.apply_move(observation, move, 1)
-                new_board = self.apply_move(new_board, move, 2)
-                if self.check_win(new_board, 2):
-                    moves_to_avoid.append(move)
+                new_board, row, col = self.apply_move(observation, move, 1)
+                if new_board[0, move] == 0:
+                    new_board, row, col = self.apply_move(new_board, move, 2)
+                    if self.check_win_around_last_move(new_board, 2, row, col):
+                        moves_to_avoid.append(move)
 
-        # Check if a move creates multiple ways to win for the player
+        # Check if a move creates a line of three tokens with available spaces on both sides
         for move in range(7):
             if observation[0, move] == 0:
-                new_board = self.apply_move(observation, move, 1)
-                if self.check_multiple_ways_to_win(new_board, 1) and move not in moves_to_avoid:
+                new_board, row, col = self.apply_move(observation, move, 1)
+                if self.check_three_in_a_row(new_board, 1, row, col) and move not in moves_to_avoid:
                     return move
 
-        # Check if a move allows the opponent to create multiple ways to win
-        for move in range(7):
-            if observation[0, move] == 0:
-                new_board = self.apply_move(observation, move, 2)
-                if self.check_multiple_ways_to_win(new_board, 2) and move not in moves_to_avoid:
-                    return move
-
-        # Play a random move among the valid moves, except those in moves_to_avoid
+        # Play a random move among valid moves, except those in moves_to_avoid
         valid_moves = [c for c in range(7) if observation[0, c] == 0 and c not in moves_to_avoid]
 
         # If valid_moves is empty, choose a random move among all possible moves
         if not valid_moves:
             valid_moves = [c for c in range(7) if observation[0, c] == 0]
 
+        if not valid_moves:
+            print('no valid_move.. i don t want to suicide myself',valid_moves,observation)
+            exit()
+
         return np.random.choice(valid_moves)
 
-    def check_multiple_ways_to_win(self, board, player):
-        win_count = 0
-        for move in range(7):
-            if board[0, move] == 0:
-                new_board = self.apply_move(board, move, player)
-                if self.check_win(new_board, player):
-                    win_count += 1
-                    if win_count >= 2:
-                        return True
-        return False
+    def play(self, obs):
+        if isinstance(obs, list):
+            return [self.play_single(o) for o in obs]
+        else:
+            return self.play_single(obs)
+
+    def getName(self):
+        return "TeenagerSmarterPlayer"
+
+    def getElo(self):
+        return 1647
     
+    def isDeterministic(self):
+        return False
+
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
             if new_board[i, move] == 0:
                 new_board[i, move] = player
-                break
-        return new_board
+                return new_board, i, move
+        print('wtf')
+        exit()
+
+    def check_win_around_last_move(self, board, player, row, col):
+        directions = [
+            (1, 0),  # horizontal
+            (0, 1),  # vertical
+            (1, 1),  # diagonal /
+            (1, -1)  # diagonal \
+        ]
+
+        for dr, dc in directions:
+            count = 0
+            for step in range(-3, 4):
+                r, c = row + step * dr, col + step * dc
+                if 0 <= r < 6 and 0 <= c < 7 and board[r, c] == player:
+                    count += 1
+                    if count == 4:
+                        return True
+                else:
+                    count = 0
 
-    def check_win(self, board, player):
-        for i in range(6):
-            for j in range(4):
-                if (board[i, j:j+4] == player).all():
-                    return True
-        for i in range(3):
-            for j in range(7):
-                if (board[i:i+4, j] == player).all():
-                    return True
-        for i in range(3):
-            for j in range(4):
-                if (board[i:i+4, j:j+4].diagonal() == player).all():
-                    return True
-                if (board[i:i+4, j:j+4][::-1].diagonal() == player).all():
-                    return True
         return False
 
-    def getName(self):
-        return "AdultSmarterPlayer"
-    
-    def getElo(self):
-        return 1767
-    
-    def isDeterministic(self):
+    def check_three_in_a_row(self, board, player, row, col):
+        directions = [
+            (1, 0),  # horizontal
+            (0, 1),  # vertical
+            (1, 1),  # diagonal /
+            (1, -1)  # diagonal \
+        ]
+
+        for dr, dc in directions:
+            count = 0
+            for step in range(-2, 3):
+                r, c = row + step * dr, col + step * dc
+                if 0 <= r < 6 and 0 <= c < 7 and board[r, c] == player:
+                    count += 1
+                    if count == 3 and 0 <= r - dr < 6 and 0 <= c - dc < 7 and board[r - dr, c - dc] == 0 and 0 <= r + 3 * dr < 6 and 0 <= c + 3 * dc < 7 and board[r + 3 * dr, c + 3 * dc] == 0:
+                        return True
+                else:
+                    count = 0
+
         return False
```

### Comparing `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/ChildPlayer.py` & `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/ChildSmarterPlayer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,46 @@
 import numpy as np
 from .Player import Player
 
-class ChildPlayer(Player):
+class ChildSmarterPlayer(Player):
 
     def __init__(self, _=""):
         pass
-    def play(self, observation):
-        # Check if a winning move is available for the player
+
+    def play_single(self, observation):
+        # Check if there is a winning move for the player
         for move in range(7):
             if observation[0, move] == 0:
                 new_board, row, col = self.apply_move(observation, move, 1)
                 if self.check_win_around_last_move(new_board, 1, row, col):
                     return move
 
-        return np.random.choice(range(7))
+        # Check if there is a winning move for the opponent
+        for move in range(7):
+            if observation[0, move] == 0:
+                new_board, row, col = self.apply_move(observation, move, 2)
+                if self.check_win_around_last_move(new_board, 2, row, col):
+                    return move
+
+        # Play a random move
+        valid_moves = [c for c in range(7) if observation[0, c] == 0]
+        return np.random.choice(valid_moves)
+
+    def play(self, observation):
+        if isinstance(observation, list):
+            return [self.play_single(obs) for obs in observation]
+        else:
+            return self.play_single(observation)
 
     def getName(self):
-        return "ChildPlayer"
-    
+        return "ChildSmarterPlayer"
+
     def getElo(self):
-        return 1208
-    
+        return 1571
+
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
             if new_board[i, move] == 0:
```

### Comparing `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/ConsolePlayer.py` & `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/ConsolePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/ModelPlayer.py` & `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/ModelPlayer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .Player import Player
 
 class ModelPlayer(Player):
     def __init__(self, model,name="Model",deteministic=True):
         self.model = model
         self.name = name
         self.deteministic = deteministic
-    def play(self, observation):
-        action, _states = self.model.predict(observation,deterministic=self.deteministic)
-        return action
+    def play(self, observations): #todo other bot : make able to takes multiples observations
+        actions, _states = self.model.predict(observations,deterministic=self.deteministic)
+        return actions
         
     def getName(self):
         return self.name
     
     def isDeterministic(self):
         return self.deteministic
```

### Comparing `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/SimulatePlayer.py` & `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/SimulatePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.3/connect_four_gymnasium/players/TeenagerPlayer.py` & `gymnasium_connect_four-1.2.0/connect_four_gymnasium/players/TeenagerPlayer.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,75 +2,91 @@
 from .Player import Player
 
 
 class TeenagerPlayer(Player):
 
     def __init__(self, _=""):
         pass
-    
-    def play(self, observation):
+
+    def play_single(self, observation):
         moves_to_avoid = []
 
         # Check for a winning move for the player
         for move in range(7):
             if observation[0, move] == 0:
-                new_board = self.apply_move(observation, move, 1)
-                if self.check_win(new_board, 1):
+                new_board, row, col = self.apply_move(observation, move, 1)
+                if self.check_win_around_last_move(new_board, 1, row, col):
                     return move
 
         # Check for a winning move for the opponent
         for move in range(7):
             if observation[0, move] == 0:
-                new_board = self.apply_move(observation, move, 2)
-                if self.check_win(new_board, 2):
+                new_board, row, col = self.apply_move(observation, move, 2)
+                if self.check_win_around_last_move(new_board, 2, row, col):
                     return move
 
         # Check if a move allows the opponent to win by playing the same move again
         for move in range(7):
             if observation[0, move] == 0:
-                new_board = self.apply_move(observation, move, 1)
-                new_board = self.apply_move(new_board, move, 2)
-                if self.check_win(new_board, 2):
-                    moves_to_avoid.append(move)
+                new_board, row, col = self.apply_move(observation, move, 1)
+                if new_board[0, move] == 0:
+                    new_board, row, col = self.apply_move(new_board, move, 2)
+                    if self.check_win_around_last_move(new_board, 2, row, col):
+                        moves_to_avoid.append(move)
 
         # Play a random move among valid moves, excluding moves_to_avoid
         valid_moves = [c for c in range(7) if observation[0, c] == 0 and c not in moves_to_avoid]
 
         # If valid_moves is empty, choose a random move among all possible moves
         if not valid_moves:
             valid_moves = [c for c in range(7) if observation[0, c] == 0]
 
+        if not valid_moves:
+            print('no valid_move.. i don t want to suicide myself',valid_moves,observation)
+            exit()
+
         return np.random.choice(valid_moves)
 
+    def play(self, obs):
+        if isinstance(obs, list):
+            return [self.play_single(o) for o in obs]
+        else:
+            return self.play_single(obs)
+
     def getName(self):
         return "TeenagerPlayer"
 
     def getElo(self):
-        return 1604
-    
+        return 1639
+
     def isDeterministic(self):
         return False
 
     def apply_move(self, board, move, player):
         new_board = board.copy()
         for i in range(5, -1, -1):
             if new_board[i, move] == 0:
                 new_board[i, move] = player
-                break
-        return new_board
+                return new_board, i, move
+        print('wtf')
+        exit()
+
+    def check_win_around_last_move(self, board, player, row, col):
+        directions = [
+            (1, 0),  # horizontal
+            (0, 1),  # vertical
+            (1, 1),  # diagonal /
+            (1, -1)  # diagonal \
+        ]
+
+        for dr, dc in directions:
+            count = 0
+            for step in range(-3, 4):
+                r, c = row + step * dr, col + step * dc
+                if 0 <= r < 6 and 0 <= c < 7 and board[r, c] == player:
+                    count += 1
+                    if count == 4:
+                        return True
+                else:
+                    count = 0
 
-    def check_win(self, board, player):
-        for i in range(6):
-            for j in range(4):
-                if (board[i, j:j+4] == player).all():
-                    return True
-        for i in range(3):
-            for j in range(7):
-                if (board[i:i+4, j] == player).all():
-                    return True
-        for i in range(3):
-            for j in range(4):
-                if (board[i:i+4, j:j+4].diagonal() == player).all():
-                    return True
-                if (board[i:i+4, j:j+4][::-1].diagonal() == player).all():
-                    return True
         return False
```

### Comparing `gymnasium_connect_four-1.1.3/connect_four_gymnasium/tools/EloLeaderboard.py` & `gymnasium_connect_four-1.2.0/connect_four_gymnasium/tools/Update_bot_elo.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,51 +25,56 @@
             TeenagerSmarterPlayer(),
             AdultPlayer(),
             AdultSmarterPlayer()
         ]
         # Initialize the Elo rankings for each player
         self.elo_rankings = {player.getName(): player.getElo() if player.getElo() is not None else 1500 for player in self.players}
 
-    def update_elo(self, player_elo, opponent_elo, player_won, k_factor=32):
+    def update_elo(self, player_elo, opponent_elo, player_won, k_factor=32, draw=False):
         # Calculate the expected outcome based on the current Elo ratings
         expected_outcome = 1 / (1 + math.pow(10, (opponent_elo - player_elo) / 400))
-        # Set the actual outcome based on whether the player won or lost
-        actual_outcome = 1 if player_won else 0
+        # Set the actual outcome based on whether the player won, lost, or drew
+        if draw:
+            actual_outcome = 0.5
+        else:
+            actual_outcome = 1 if player_won else 0
         # Update the player's Elo rating
         new_elo = player_elo + k_factor * (actual_outcome - expected_outcome)
         return new_elo
 
     def play_round(self, k_factor=32, move_elo_already_known=False):
         # Iterate through all possible player-opponent pairs
         for player in self.players:
             for opponent in self.players:
                 if player != opponent:
                     # Skip the match if both players have known Elo ratings and we don't want to update them
                     if not move_elo_already_known and player.getElo() is not None and opponent.getElo() is not None:
                         continue
                     player_score = self.get_score(player, opponent)
                     player_won = player_score > 0.5
+                    draw = player_score == 0.5
                     player_elo = self.elo_rankings[player.getName()]
                     opponent_elo = self.elo_rankings[opponent.getName()]
-                    new_player_elo = self.update_elo(player_elo, opponent_elo, player_won, k_factor)
-                    new_opponent_elo = self.update_elo(opponent_elo, player_elo, not player_won, k_factor)
+                    new_player_elo = self.update_elo(player_elo, opponent_elo, player_won, k_factor,draw)
+                    new_opponent_elo = self.update_elo(opponent_elo, player_elo, not player_won, k_factor,draw)
                     if player.getElo() is None or move_elo_already_known:
                         self.elo_rankings[player.getName()] = new_player_elo
-                    if opponent.getElo() is None or move_elo_already_known:
+                    if opponent.getElo() is None or move_elo_already_known :
                         self.elo_rankings[opponent.getName()] = new_opponent_elo
+                    self.elo_rankings["BabyPlayer"] = 1000
 
     def get_elo(self, new_players, num_matches=100, move_elo_already_known=False, display_log=True):
         # Add new players to the leaderboard
         self.players.extend(new_players)
         for player in new_players:
             self.elo_rankings[player.getName()] = player.getElo() if player.getElo() is not None else 1500
 
         # Play the specified number of matches
         for i in range(num_matches):
-            k_factor = 32 / (1 + i / 10)
+            k_factor = 2 / (1 + i / 10)
             self.play_round(k_factor, move_elo_already_known)
             if display_log:
                 print(f"Elo rankings after {i+1} matches:")
                 self.display_rankings()
                 print("\n")
 
         # Return the updated Elo ratings for the new players
@@ -93,22 +98,10 @@
             obs, rewards, dones, truncated, _ = env.step(action)
             if truncated or dones:
                 obs, _ = env.reset()
                 return rewards
 
 
 if __name__ == "__main__":
-    from connect_four_gymnasium.players import (MinMaxPlayer)
 
     elo_leaderboard = EloLeaderboard()
-    print(elo_leaderboard.get_elo([MinMaxPlayer(depth=1)], num_matches=100))
-
-# 1. AdultSmarterPlayer:    1767
-# 2. AdultPlayer:           1712
-# 3. MinimaxPlayer depth 3: 1672
-# 4. MinimaxPlayer depth 2: 1622
-# 5. TeenagerSmarterPlayer: 1611
-# 6. TeenagerPlayer:        1604
-# 7. ChildSmarterPlayer:    1525
-# 8. MinimaxPlayer depth 1: 1220
-# 9. ChildPlayer:           1208
-# 10. BabyPlayer:            995
+    print(elo_leaderboard.get_elo([], num_matches=100000,display_log=True,move_elo_already_known=True))
```

### Comparing `gymnasium_connect_four-1.1.3/gymnasium_connect_four.egg-info/SOURCES.txt` & `gymnasium_connect_four-1.2.0/gymnasium_connect_four.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 connect_four_gymnasium/__init__.py
 connect_four_gymnasium/players/AdultPlayer.py
 connect_four_gymnasium/players/AdultSmarterPlayer.py
 connect_four_gymnasium/players/BabyPlayer.py
 connect_four_gymnasium/players/ChildPlayer.py
 connect_four_gymnasium/players/ChildSmarterPlayer.py
 connect_four_gymnasium/players/ConsolePlayer.py
-connect_four_gymnasium/players/MinMaxPlayer.py
 connect_four_gymnasium/players/ModelPlayer.py
 connect_four_gymnasium/players/Player.py
 connect_four_gymnasium/players/SimulatePlayer.py
 connect_four_gymnasium/players/TeenagerPlayer.py
 connect_four_gymnasium/players/TeenagerSmarterPlayer.py
 connect_four_gymnasium/players/__init__.py
 connect_four_gymnasium/tools/EloLeaderboard.py
+connect_four_gymnasium/tools/Update_bot_elo.py
 connect_four_gymnasium/tools/__init__.py
 gymnasium_connect_four.egg-info/PKG-INFO
 gymnasium_connect_four.egg-info/SOURCES.txt
 gymnasium_connect_four.egg-info/dependency_links.txt
 gymnasium_connect_four.egg-info/requires.txt
 gymnasium_connect_four.egg-info/top_level.txt
 test/test_no_opponant.py
```

### Comparing `gymnasium_connect_four-1.1.3/setup.py` & `gymnasium_connect_four-1.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='gymnasium_connect_four',
-    version='1.1.3',
+    version='1.2.0',
     description='A connect 4 (connect four) environment for OpenAI Gym and Gymnasium',
     author='Lucas Bertola',
     url='https://github.com/lucasBertola/Connect-4-env',  
     # author_email='your.email@example.com',
     packages=find_packages(),
     install_requires=[
         'pygame==2.1.3',
```

### Comparing `gymnasium_connect_four-1.1.3/test/test_no_opponant.py` & `gymnasium_connect_four-1.2.0/test/test_no_opponant.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.3/test/test_power_4_logic.py` & `gymnasium_connect_four-1.2.0/test/test_power_4_logic.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.1.3/test/test_ppo_env.py` & `gymnasium_connect_four-1.2.0/test/test_ppo_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         obs, rewards, dones, truncated, info = env.step(action)
 
         if truncated or dones:
             allrewards.append(rewards)
             obs, _ = env.reset()
 
     # Check if the model is deterministic
-    assert np.sum(allrewards) == -9, "The model is not determinist"
+    assert np.sum(allrewards) == 8, "The model is not determinist"
 
 
 def test_is_working_with_ppo():
     # Initialize the environment and the PPO model
     env = ConnectFourEnv(opponent=BabyPlayer())
     model = PPO("MlpPolicy", env, verbose=0, seed=0)
```

