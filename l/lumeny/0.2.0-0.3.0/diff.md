# Comparing `tmp/lumeny-0.2.0.tar.gz` & `tmp/lumeny-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumeny-0.2.0.tar", max compression
+gzip compressed data, was "lumeny-0.3.0.tar", max compression
```

## Comparing `lumeny-0.2.0.tar` & `lumeny-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      652 2023-04-13 12:21:17.181246 lumeny-0.2.0/README.md
--rw-r--r--   0        0        0     4712 2023-04-12 16:47:14.787304 lumeny-0.2.0/lumeny/CaldavConnector.py
--rw-r--r--   0        0        0     1590 2023-04-13 12:16:45.567741 lumeny-0.2.0/lumeny/ConfigLoader.py
--rw-r--r--   0        0        0     2068 2023-03-26 21:54:13.154345 lumeny-0.2.0/lumeny/EmbeddingGenerator.py
--rw-r--r--   0        0        0     3001 2023-04-13 12:18:41.544232 lumeny-0.2.0/lumeny/MinifluxConnector.py
--rw-r--r--   0        0        0        0 2023-03-26 11:54:25.500396 lumeny-0.2.0/lumeny/QdrantConnector.py
--rw-r--r--   0        0        0        0 2023-03-26 11:44:08.561839 lumeny-0.2.0/lumeny/__init__.py
--rw-r--r--   0        0        0     1684 2023-04-20 01:43:03.801671 lumeny-0.2.0/lumeny/ai_utils.py
--rw-r--r--   0        0        0     6002 2023-04-20 02:17:32.419822 lumeny-0.2.0/lumeny/calendar.py
--rw-r--r--   0        0        0     2802 2023-04-20 02:06:59.785132 lumeny-0.2.0/lumeny/cli.py
--rw-r--r--   0        0        0     1839 2023-04-13 12:08:33.198863 lumeny-0.2.0/lumeny/tui.py
--rw-r--r--   0        0        0     1046 2023-04-20 02:04:35.099308 lumeny-0.2.0/lumeny/utils.py
--rw-r--r--   0        0        0      645 2023-04-20 02:19:05.031699 lumeny-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 lumeny-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1452 2023-07-28 19:03:12.788467 lumeny-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-26 11:44:08.561839 lumeny-0.3.0/lumeny/__init__.py
+-rw-r--r--   0        0        0     1696 2023-07-28 21:17:37.267727 lumeny-0.3.0/lumeny/ai_utils.py
+-rw-r--r--   0        0        0     4714 2023-07-28 19:08:43.301838 lumeny-0.3.0/lumeny/caldav_connector.py
+-rw-r--r--   0        0        0     3046 2023-07-28 21:15:45.791736 lumeny-0.3.0/lumeny/calendar.py
+-rw-r--r--   0        0        0     3499 2023-07-28 21:59:18.088301 lumeny-0.3.0/lumeny/cli.py
+-rw-r--r--   0        0        0     1591 2023-07-28 19:04:15.095339 lumeny-0.3.0/lumeny/config_loader.py
+-rw-r--r--   0        0        0     2068 2023-03-26 21:54:13.154345 lumeny-0.3.0/lumeny/embedding_generator.py
+-rw-r--r--   0        0        0     2978 2023-07-28 21:58:12.639666 lumeny-0.3.0/lumeny/miniflux_connector.py
+-rw-r--r--   0        0        0     3725 2023-07-28 22:05:00.534392 lumeny-0.3.0/lumeny/task_picker.py
+-rw-r--r--   0        0        0        0 2023-07-28 19:37:56.700927 lumeny-0.3.0/lumeny/testing.log
+-rw-r--r--   0        0        0     1840 2023-07-28 19:08:34.883097 lumeny-0.3.0/lumeny/tui.py
+-rw-r--r--   0        0        0      913 2023-07-28 21:17:54.079424 lumeny-0.3.0/lumeny/utils.py
+-rw-r--r--   0        0        0      666 2023-07-28 22:07:19.469667 lumeny-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2429 1970-01-01 00:00:00.000000 lumeny-0.3.0/PKG-INFO
```

### Comparing `lumeny-0.2.0/lumeny/CaldavConnector.py` & `lumeny-0.3.0/lumeny/caldav_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import caldav
 import timeit
 from typing import List
-from ConfigLoader import ConfigLoader
+from config_loader import ConfigLoader
 from utils import time_usage
 import datetime
 import random
 
 # function to connect to caldav client using url and username and password
 def connect_caldav(url: str, username: str, password: str) -> caldav.DAVClient:
     return caldav.DAVClient(url, username=username, password=password)
@@ -120,8 +120,8 @@
     # get all events from today to 30 days from now
     events: List[caldav.Event] = search_events_by_day(client, today, today + datetime.timedelta(days=7))
     print(type(events[0]))
     # print events
     print_events(events)
     
 if __name__ == "__main__":
-    test_connect_caldav()
+    test_connect_caldav()
```

### Comparing `lumeny-0.2.0/lumeny/ConfigLoader.py` & `lumeny-0.3.0/lumeny/config_loader.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -41,8 +41,8 @@
         config[section][key] = value
         self.write_config(config)
     
 def main():
     config_loader = ConfigLoader()
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `lumeny-0.2.0/lumeny/EmbeddingGenerator.py` & `lumeny-0.3.0/lumeny/embedding_generator.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.2.0/lumeny/MinifluxConnector.py` & `lumeny-0.3.0/lumeny/miniflux_connector.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,87 +1,93 @@
-import miniflux
 from typing import Any, Dict, List
-from lumeny.ConfigLoader import ConfigLoader
+from config_loader import ConfigLoader
 import random
+import miniflux
+
 
 # write a function that connects to miniflux client using api key and url
 def connect_miniflux(url: str, api_key: str) -> miniflux.Client:
     return miniflux.Client(url, api_key=api_key)
 
+
 # a function that prints all the feeds' name and id
 def print_feeds(feeds: List[Dict]) -> None:
     # sort by feed id
     feeds.sort(key=lambda feed: feed["id"])
     # print number of feeds
     print(f"Number of feeds: {len(feeds)}")
     for feed in feeds:
         print(f"Feed id: {feed['id']}, Feed name: {feed['title']}")
         # print such that title ,id and site_url are aligned
 
+
 # write a function that get all the entries from a feed, optionally select by starred or unread, and return a list of entry id
 def get_entries_from_feed(
     client: miniflux.Client, feed_id: int, starred: bool = False, unread: bool = False
 ) -> List[int]:
     # get entries from feed
-    entries: Dict = client.get_entries(feed_id= feed_id, starred=starred, unread=unread)
-    
+    entries: Dict = client.get_entries(feed_id=feed_id, starred=starred, unread=unread)
+
     # since the entries are cut if the number is above 100, we need to fetch the entries again with limit from total
     total: int = entries["total"]
-    entries: List[Dict] = client.get_entries(feed_id = feed_id, starred=starred, unread=unread, limit=total)
+    entries: List[Dict] = client.get_entries(
+        feed_id=feed_id, starred=starred, unread=unread, limit=total
+    )
     # assert that the total is equal to the length of entries
     assert total == len(entries["entries"])
-    
+
     # print type of total
     print(f"Total type: {type(total)}")
-    
+
     # get only entry id
-    entry_ids: List[int] = [entry["id"] for entry in entries['entries']]
+    entry_ids: List[int] = [entry["id"] for entry in entries["entries"]]
     return entry_ids
 
+
 # write a function to find feed by its id, use map instead of for loop
 def find_feed_by_id(feed_id: int, feeds: List[Dict]) -> Dict:
     return next(filter(lambda feed: feed["id"] == feed_id, feeds))
 
+
 # TODO create embedding from feed content
 
 # TODO add feeds' embedding to "liked" category in embeddings
 
 # TODO randomly select n feeds from all unread feeds
 
 # TODO randomly select n feeds from all started feeds
 
+
 def test():
-    
     # connect
     config_loader = ConfigLoader()
     config = config_loader.get_config()
     miniflux_config = config["miniflux"]
     client: miniflux.Client = connect_miniflux(
         miniflux_config["url"], miniflux_config["api"]
     )
 
     # get feed ids
     feeds: List[Dict] = client.get_feeds()
     # get only id
     feed_ids: List[int] = [feed["id"] for feed in feeds]
-    
+
     print("feed ids are as follows: ")
     print(feed_ids)
 
     # randomly choose a feed from given feed ids
     feed_id: int = random.choice(feed_ids)
     print(f"randomly chosen feed id is: {feed_id} ")
 
     # get feed by id
     feed: Dict = find_feed_by_id(feed_id, feeds)
     print(f"feed with id {feed_id} is: {feed['title']}")
-    
+
     # get entries from feed
     entries = get_entries_from_feed(client, feed_id)
-    
+
     # print total number of entries
     print(f"Total number of entries: {len(entries)}")
-    
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `lumeny-0.2.0/lumeny/ai_utils.py` & `lumeny-0.3.0/lumeny/ai_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """The ai utilites for lumeny project"""
 
 from typing import Dict, List
 import openai
-from lumeny.ConfigLoader import ConfigLoader
+# from lumeny.ConfigLoader import ConfigLoader
 
 # Set your API key from environment variables
-config = ConfigLoader().get_config()
+# config = ConfigLoader().get_config()
 
-openai.api_key = config["openai"]["api"]
+# openai.api_key = config["openai"]["api"]
 
 # Function to interact with the chatcompletion API
 
 
-def chat_with_gpt(the_conversation: List[Dict], model: str = "gpt-4", temperature: float = 0.1):
+def chat_with_gpt(
+    the_conversation: List[Dict], model: str = "gpt-4", temperature: float = 0.1
+):
     """
 
     The function to interact with the chatcompletion API
 
     :param the_conversation: conversation stored in list of dictionaries
     :param model: gpt3.5-turbo, gpt-4
     :param temperature: from 0 to 1, control the randomness of the response
```

### Comparing `lumeny-0.2.0/lumeny/cli.py` & `lumeny-0.3.0/lumeny/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # cli.py
 import os
 import questionary as q
 import click
 from prompt_toolkit.lexers import PygmentsLexer
-from lumeny.utils import InputLexer, print_green
+from lumeny.utils import InputLexer
 
 # from lumen.tui import launch_tui
-from lumeny.calendar import generate_command_with_gpt4, repeat_learn
+# from lumeny.calendar import generate_command_with_gpt4, repeat_learn
+from lumeny.task_picker import random_task_picker, available_sections
+from termcolor import colored
 
 
 @click.group()
 def cli():
     pass
 
 
@@ -41,14 +43,16 @@
         while True:
             add_one_event()
             if not q.confirm("Add another event?", qmark="").ask():
                 break
 
         return
 
+    return
+
 
 @click.command()
 @click.option("-t", "--topic", type=str, help="Specify the topic.")
 @click.option(
     "-r",
     "--repeat_days",
     type=int,
@@ -60,15 +64,14 @@
     "-s",
     "--start_date",
     type=int,
     default=0,
     help="Specify a start date as an integer.",
 )
 def repeat(topic, repeat_days, start_date):
-
     format_str = "%d-%m-%Y"
 
     command: str = repeat_learn(topic, repeat_days, start_date)
     if q.confirm(f"Execute: {command}", qmark="?").ask():
         try:
             os.system(command)
             print_green("Event Added!")
@@ -89,30 +92,59 @@
     # If input arguments are passed, concatenate them to form a single string
     input_str = " ".join(input)
     command: str = generate_command_with_gpt4(input_str)
 
     if q.confirm(f"Execute: {command}", qmark="?").ask():
         try:
             os.system(command)
-            print(f"\033[1;32mEvent Added!\033[0m")
+            print(colored("Event Added!", "green"))
         except Exception as e:
             print(e)
             print("Error executing command")
 
+    return
+
 
 @click.command()
 def show():
     """
     Launch the Text User Interface (TUI).
     """
     print("Show")
 
     # launch_tui()
 
 
+@click.command()
+@click.option(
+    "-a", "--all", is_flag=True, default=False, help="Give me a task without any pick"
+)
+def task(all):
+    """
+    Choose a random task to do.
+    """
+    section_list = available_sections()
+
+    section_list.append("All")
+
+    # choose a section
+    if not all:
+        section = q.select(
+            "Choose a section",
+            choices=section_list,
+            qmark="?",
+        ).ask()
+    else:
+        section = "All"
+
+    # choose a task
+    random_task_picker(section_code = section if section != "All" else None)
+
+
 cli.add_command(will)
 cli.add_command(show)
 cli.add_command(add)
 cli.add_command(repeat)
+cli.add_command(task)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `lumeny-0.2.0/lumeny/tui.py` & `lumeny-0.3.0/lumeny/tui.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from textual.app import App, ComposeResult
 from textual.widgets import Header, Footer, Static
-from MinifluxConnector import connect_miniflux 
+from miniflux_connector import connect_miniflux 
 
 # create a widget to display all starred feed titles
 class FeedPreview(Static):
     """A widget to display a feed 
 
     Args:
         App (_type_): _description_
```

### Comparing `lumeny-0.2.0/lumeny/utils.py` & `lumeny-0.3.0/lumeny/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import os
 import timeit
 from pygments.lexer import RegexLexer
 from pygments.token import Text, Comment
 
 
-def print_green(text):
-    green_escape = "\033[32m"
-    reset_escape = "\033[0m"
-    print(f"{green_escape}{text}{reset_escape}")
-
-
 def notify(title: str, notification: str, icon: str = "arch") -> None:
     cmd = f"notify-send '{title}' '{notification}' --icon={icon}"
     os.system(cmd)
 
 
 # write a decorator to time functions
 def time_usage(func):
```

### Comparing `lumeny-0.2.0/pyproject.toml` & `lumeny-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lumeny"
-version = "0.2.0"
+version = "0.3.0"
 description = "A cli and tui based personal management app for Lumen Young"
 authors = ["Lumen Young <pip@lumeny.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 caldav = "^1.2.1"
@@ -16,14 +16,15 @@
 openai = "^0.27.2"
 docker = "^6.0.1"
 nltk = "^3.8.1"
 pyyaml = "^6.0"
 questionary = "^1.10.0"
 prompt-toolkit = "^3.0.38"
 dateparser = "^1.1.8"
+termcolor = "^2.3.0"
 
 [tool.poetry.scripts]
 lumen = "lumeny.cli:cli"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `lumeny-0.2.0/PKG-INFO` & `lumeny-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumeny
-Version: 0.2.0
+Version: 0.3.0
 Summary: A cli and tui based personal management app for Lumen Young
 Author: Lumen Young
 Author-email: pip@lumeny.io
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -16,21 +16,38 @@
 Requires-Dist: miniflux (>=0.0.15,<0.0.16)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (>=0.27.2,<0.28.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: qdrant-client (>=1.1.0,<2.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
+Requires-Dist: termcolor (>=2.3.0,<3.0.0)
 Requires-Dist: textual (>=0.16.0,<0.17.0)
 Description-Content-Type: text/markdown
 
 # Lumeny
 
 This is lumeny, a cli project that I used for my own daily usage.
 
 There are several aspects that I want my cli app grows:
 
 1. Connect to caldav so that it can reminds me of my events, or add new events in cli convinently. Pushing notification to the KDE desktop is also a important part to remind me of the events.
 2. Connect to my RSS reader miniflux and filter the most important feeds using ChatGPT (A small recommendation system).
 3. A TUI based on textual to help me manage several aspects of point 1 and 2, like inspect upcoming events or get general statistic of my feeds, and help me gradually improve the recommandation algorithm.
 
+## Functions
+
+This is a amalgamation of interesting feature for my personal use, they are not necessarily corelated.
+
+### Caldav integrator
+
+Connect to caldav so that it can reminds me of my events, or add new events in cli convinently. Pushing notification to the KDE desktop is also a important part to remind me of the events.
+
+### Miniflux filter
+
+There are several thousands of feeds in my miniflux, which I sometimes not able to process them all. I would like to make it more automated by using LLM to find the interesting feeds for me.
+
+### Random tasks picker
+
+Through times I accumulated a list of interesting project/subject. I would like to have a command to help me randomly select a project exists in my task page and make it a bonus to my day after finishing the main goal of the day.
+
```

