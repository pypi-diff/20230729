# Comparing `tmp/twitternewsbot-2.0.2.tar.gz` & `tmp/twitternewsbot-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitternewsbot-2.0.2.tar", last modified: Tue Jul 25 16:44:21 2023, max compression
+gzip compressed data, was "twitternewsbot-2.0.3.tar", last modified: Sat Jul 29 11:19:05 2023, max compression
```

## Comparing `twitternewsbot-2.0.2.tar` & `twitternewsbot-2.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 arnavmarda   (501) staff       (20)        0 2023-07-25 16:44:21.289461 twitternewsbot-2.0.2/
--rw-r--r--   0 arnavmarda   (501) staff       (20)     1068 2023-07-21 18:00:57.000000 twitternewsbot-2.0.2/LICENSE
--rw-r--r--   0 arnavmarda   (501) staff       (20)     3211 2023-07-25 16:44:21.289535 twitternewsbot-2.0.2/PKG-INFO
--rw-r--r--   0 arnavmarda   (501) staff       (20)     2459 2023-07-25 16:44:07.000000 twitternewsbot-2.0.2/README.md
--rw-r--r--   0 arnavmarda   (501) staff       (20)      131 2023-07-25 16:44:21.289721 twitternewsbot-2.0.2/setup.cfg
--rw-r--r--   0 arnavmarda   (501) staff       (20)     2049 2023-07-25 16:44:17.000000 twitternewsbot-2.0.2/setup.py
-drwxr-xr-x   0 arnavmarda   (501) staff       (20)        0 2023-07-25 16:44:21.288487 twitternewsbot-2.0.2/twitternewsbot/
--rw-r--r--   0 arnavmarda   (501) staff       (20)      148 2023-07-25 16:38:08.000000 twitternewsbot-2.0.2/twitternewsbot/__init__.py
--rw-r--r--   0 arnavmarda   (501) staff       (20)    13947 2023-07-23 21:03:02.000000 twitternewsbot-2.0.2/twitternewsbot/newsfinder.py
--rw-r--r--   0 arnavmarda   (501) staff       (20)    14626 2023-07-23 21:06:50.000000 twitternewsbot-2.0.2/twitternewsbot/tweeter.py
--rw-r--r--   0 arnavmarda   (501) staff       (20)     8096 2023-07-24 16:43:03.000000 twitternewsbot-2.0.2/twitternewsbot/twitternewsbot.py
-drwxr-xr-x   0 arnavmarda   (501) staff       (20)        0 2023-07-25 16:44:21.289341 twitternewsbot-2.0.2/twitternewsbot.egg-info/
--rw-r--r--   0 arnavmarda   (501) staff       (20)     3211 2023-07-25 16:44:21.000000 twitternewsbot-2.0.2/twitternewsbot.egg-info/PKG-INFO
--rw-r--r--   0 arnavmarda   (501) staff       (20)      340 2023-07-25 16:44:21.000000 twitternewsbot-2.0.2/twitternewsbot.egg-info/SOURCES.txt
--rw-r--r--   0 arnavmarda   (501) staff       (20)        1 2023-07-25 16:44:21.000000 twitternewsbot-2.0.2/twitternewsbot.egg-info/dependency_links.txt
--rw-r--r--   0 arnavmarda   (501) staff       (20)      143 2023-07-25 16:44:21.000000 twitternewsbot-2.0.2/twitternewsbot.egg-info/requires.txt
--rw-r--r--   0 arnavmarda   (501) staff       (20)       15 2023-07-25 16:44:21.000000 twitternewsbot-2.0.2/twitternewsbot.egg-info/top_level.txt
+drwxr-xr-x   0 arnavmarda   (501) staff       (20)        0 2023-07-29 11:19:05.239353 twitternewsbot-2.0.3/
+-rw-r--r--   0 arnavmarda   (501) staff       (20)     1068 2023-07-21 18:00:57.000000 twitternewsbot-2.0.3/LICENSE
+-rw-r--r--   0 arnavmarda   (501) staff       (20)     3623 2023-07-29 11:19:05.239416 twitternewsbot-2.0.3/PKG-INFO
+-rw-r--r--   0 arnavmarda   (501) staff       (20)     2823 2023-07-29 11:11:57.000000 twitternewsbot-2.0.3/README.md
+-rw-r--r--   0 arnavmarda   (501) staff       (20)      131 2023-07-29 11:19:05.239611 twitternewsbot-2.0.3/setup.cfg
+-rw-r--r--   0 arnavmarda   (501) staff       (20)     2112 2023-07-29 11:18:41.000000 twitternewsbot-2.0.3/setup.py
+drwxr-xr-x   0 arnavmarda   (501) staff       (20)        0 2023-07-29 11:19:05.238358 twitternewsbot-2.0.3/twitternewsbot/
+-rw-r--r--   0 arnavmarda   (501) staff       (20)      148 2023-07-25 16:38:08.000000 twitternewsbot-2.0.3/twitternewsbot/__init__.py
+-rw-r--r--   0 arnavmarda   (501) staff       (20)     2604 2023-07-28 10:58:01.000000 twitternewsbot-2.0.3/twitternewsbot/__main__.py
+-rw-r--r--   0 arnavmarda   (501) staff       (20)    16697 2023-07-29 11:01:22.000000 twitternewsbot-2.0.3/twitternewsbot/newsfinder.py
+-rw-r--r--   0 arnavmarda   (501) staff       (20)    18707 2023-07-29 10:48:33.000000 twitternewsbot-2.0.3/twitternewsbot/tweeter.py
+-rw-r--r--   0 arnavmarda   (501) staff       (20)     7418 2023-07-29 11:05:17.000000 twitternewsbot-2.0.3/twitternewsbot/twitternewsbot.py
+drwxr-xr-x   0 arnavmarda   (501) staff       (20)        0 2023-07-29 11:19:05.239234 twitternewsbot-2.0.3/twitternewsbot.egg-info/
+-rw-r--r--   0 arnavmarda   (501) staff       (20)     3623 2023-07-29 11:19:05.000000 twitternewsbot-2.0.3/twitternewsbot.egg-info/PKG-INFO
+-rw-r--r--   0 arnavmarda   (501) staff       (20)      367 2023-07-29 11:19:05.000000 twitternewsbot-2.0.3/twitternewsbot.egg-info/SOURCES.txt
+-rw-r--r--   0 arnavmarda   (501) staff       (20)        1 2023-07-29 11:19:05.000000 twitternewsbot-2.0.3/twitternewsbot.egg-info/dependency_links.txt
+-rw-r--r--   0 arnavmarda   (501) staff       (20)      143 2023-07-29 11:19:05.000000 twitternewsbot-2.0.3/twitternewsbot.egg-info/requires.txt
+-rw-r--r--   0 arnavmarda   (501) staff       (20)       15 2023-07-29 11:19:05.000000 twitternewsbot-2.0.3/twitternewsbot.egg-info/top_level.txt
```

### Comparing `twitternewsbot-2.0.2/LICENSE` & `twitternewsbot-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `twitternewsbot-2.0.2/PKG-INFO` & `twitternewsbot-2.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 Metadata-Version: 2.1
 Name: twitternewsbot
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python API allowing you to automize a personalized news delivery system.
 Home-page: https://github.com/arnavmarda/twitter-news-bot/
-Download-URL: https://github.com/arnavmarda/twitter-news-bot/archive/refs/tags/v2.0.tar.gz
+Download-URL: https://github.com/arnavmarda/twitter-news-bot/archive/refs/tags/v2.0.3.tar.gz
 Author: Arnav Marda
 Author-email: arnavmarda@gmail.com
 License: MIT
-Keywords: AI,Twitter,News,Automation
+Keywords: AI,Twitter,News,Automation,Google News,Scraping,Requests,Tweepy,Articles
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-<div align=center>
+<div align="center">
 <img alt="Logo" src="https://github.com/arnavmarda/twitter-news-bot/blob/main/docs/logo.png" width=200 />
 </div>
 
+<div align="center">
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/twitternewsbot.svg)](https://badge.fury.io/py/twitternewsbot)
+
+[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+
+</div>
+
 # twitter-news-bot
 
 A python API allowing users to:
 
 1. Scrape news articles from Google News.
 2. Extract the articles from the news sources.
 3. Create and post tweets(or now Xs) using `tweepy`.
```

### Comparing `twitternewsbot-2.0.2/README.md` & `twitternewsbot-2.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 
-<div align=center>
+<div align="center">
 <img alt="Logo" src="https://github.com/arnavmarda/twitter-news-bot/blob/main/docs/logo.png" width=200 />
 </div>
 
+<div align="center">
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/twitternewsbot.svg)](https://badge.fury.io/py/twitternewsbot)
+
+[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+
+</div>
+
 # twitter-news-bot
 
 A python API allowing users to:
 
 1. Scrape news articles from Google News.
 2. Extract the articles from the news sources.
 3. Create and post tweets(or now Xs) using `tweepy`.
```

### Comparing `twitternewsbot-2.0.2/setup.py` & `twitternewsbot-2.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'twitternewsbot',         # How you named your package folder (MyLib)
   packages = ['twitternewsbot'],   # Chose the same as "name"
-  version = '2.0.2',      # Start with a small number and increase it with every change you make
+  version = '2.0.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Python API allowing you to automize a personalized news delivery system.',   # Give a short description about your library
   author = 'Arnav Marda',                   # Type in your name
   author_email = 'arnavmarda@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/arnavmarda/twitter-news-bot/',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/arnavmarda/twitter-news-bot/archive/refs/tags/v2.0.tar.gz',    # I explain this later on
-  keywords = ['AI', 'Twitter', 'News', 'Automation'],   # Keywords that define your package best
+  download_url = 'https://github.com/arnavmarda/twitter-news-bot/archive/refs/tags/v2.0.3.tar.gz',    # I explain this later on
+  keywords = ['AI', 'Twitter', 'News', 'Automation', 'Google News', 'Scraping', 'Requests', 'Tweepy', 'Articles'],   # Keywords that define your package best
   long_description = long_description,
   long_description_content_type="text/markdown",
   install_requires=[            # I get to this in a second
           'requests==2.31.0',
           'requests-html==0.10.0',
           'tweepy==4.14.0',
           'google-generativeai==0.1.0',
```

### Comparing `twitternewsbot-2.0.2/twitternewsbot/tweeter.py` & `twitternewsbot-2.0.3/twitternewsbot/tweeter.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,45 +4,110 @@
 from dotenv import load_dotenv
 
 class Tweeter():
 
     """
     API Object allowing users to tweet articles, summaries and other text to Twitter. 
     It leverages PaLM to summarize articles and then tweets them in chunks of 280 characters.
-    Requires having the Twitter API API_KEY, API_SECRET_KEY, ACCESS_TOKEN and ACCESS_TOKEN_SECRET set as environment variables.
+    The API keys required for the Twitter API must be provided as environment variables or as arguments to the constructor.
+    The API key required for the Google API can be provided as environment variables or as an argument to the constructor. 
+    The Google API key is optional. If not provided, the API will not be able to summarize articles.
+
+    Attributes
+    ----------
+    __API_KEY : str
+        The API key for the Twitter API
+    __API_SECRET_KEY : str
+        The API secret key for the Twitter API
+    __ACCESS_TOKEN : str
+        The access token for the Twitter API
+    __ACCESS_TOKEN_SECRET : str
+        The access token secret for the Twitter API
+    __GOOGLE_API_KEY : str
+        The API key for the Google API
+    __client : Client
+        The tweepy client object
     """
 
   #####################################
   # Initialization
   #####################################
     
-    def __init__(self):
-        """Initialize the class with tokens and tweepy client"""
+    def __init__(self, api_key: str|None = None, api_secret_key: str|None = None, access_token: str|None = None, access_token_secret: str|None = None, google_api_key: str|None = None):
+        """Initialize the class with tokens and tweepy client
+        
+        Parameters
+        ----------
+        api_key : str, optional
+            The API key for the Twitter API, by default None
+        api_secret_key : str, optional
+            The API secret key for the Twitter API, by default None
+        access_token : str, optional
+            The access token for the Twitter API, by default None
+        access_token_secret : str, optional
+            The access token secret for the Twitter API, by default None
+        google_api_key : str, optional
+            The API key for the Google API, by default None
+
+        Raises
+        ------
+        Exception
+            If API_KEY is not found in environment variables and not provided as an argument
+        Exception
+            If API_SECRET_KEY is not found in environment variables and not provided as an argument
+        Exception
+            If ACCESS_TOKEN is not found in environment variables and not provided as an argument
+        Exception
+            If ACCESS_TOKEN_SECRET is not found in environment variables and not provided as an argument
+        Exception
+            Twitter API Authentication Failed. Invalid Twitter API Credentials
+        """
 
         # Load environment variables
         load_dotenv()
-        try:
-            self.__API_KEY = os.getenv("API_KEY")
-        except:
-            raise Exception("API_KEY not found in environment variables")
-        
-        try:
-            self.__API_SECRET_KEY = os.getenv("API_SECRET_KEY")
-        except:
-            raise Exception("API_SECRET_KEY not found in environment variables")
-        
-        try:
-            self.__ACCESS_TOKEN = os.getenv("ACCESS_TOKEN")
-        except:
-            raise Exception("ACCESS_TOKEN not found in environment variables")
-        
-        try:
-            self.__ACCESS_TOKEN_SECRET = os.getenv("ACCESS_TOKEN_SECRET")
-        except:
-            raise Exception("ACCESS_TOKEN_SECRET not found in environment variables")
+
+        if api_key is None:
+            try:
+                self.__API_KEY = os.getenv("API_KEY")
+            except:
+                raise Exception("API_KEY not found in environment variables and not provided as an argument")
+        else:
+            self.__API_KEY = api_key
+        
+        if api_secret_key is None:
+            try:
+                self.__API_SECRET_KEY = os.getenv("API_SECRET_KEY")
+            except:
+                raise Exception("API_SECRET_KEY not found in environment variables and not provided as an argument")
+        else:
+            self.__API_SECRET_KEY = api_secret_key
+        
+        if access_token is None:
+            try:
+                self.__ACCESS_TOKEN = os.getenv("ACCESS_TOKEN")
+            except:
+                raise Exception("ACCESS_TOKEN not found in environment variables and not provided as an argument")
+        else:
+            self.__ACCESS_TOKEN = access_token
+        
+        if access_token_secret is None:
+            try:
+                self.__ACCESS_TOKEN_SECRET = os.getenv("ACCESS_TOKEN_SECRET")
+            except:
+                raise Exception("ACCESS_TOKEN_SECRET not found in environment variables and not provided as an argument")
+        else:
+            self.__ACCESS_TOKEN_SECRET = access_token_secret
+        
+        if google_api_key is None:
+            try:
+                self.__GOOGLE_API_KEY = os.getenv("GOOGLE_API_KEY")
+            except:
+                pass
+        else:
+            self.__GOOGLE_API_KEY = google_api_key
 
         try:
             self.__client = Client(consumer_key=self.__API_KEY, 
                                    consumer_secret=self.__API_SECRET_KEY, 
                                    access_token=self.__ACCESS_TOKEN, 
                                    access_token_secret=self.__ACCESS_TOKEN_SECRET)
         except:
@@ -157,22 +222,20 @@
         Returns
         -------
         summary : str
             The summary of the article created using GOOGLE PaLM
         """
 
         # Get the API key
-        try:
-            GOOGLE_API_KEY = os.getenv('GOOGLE_API_KEY')
-        except:
+        if self.__GOOGLE_API_KEY is None:
             raise Exception("GOOGLE_API_KEY not found in environment variables")
 
         # Initialize PaLM
         try:
-            palm.configure(api_key=GOOGLE_API_KEY)
+            palm.configure(api_key=self.__GOOGLE_API_KEY)
         except:
             raise Exception("Authentication Failed. Invalid Google API Credentials")
 
         # Default Settings
         defaults = {
                         'model': 'models/text-bison-001',
                         'temperature': 0.1,
@@ -320,14 +383,21 @@
     def get_client(self) -> Client:
         """Get the tweepy client object
 
         Returns
         -------
         client : Client
             The tweepy client object
+
+        Examples
+        --------
+        >>> from twitternewsbot.tweeter import Tweeter
+        >>> tweeter = Tweeter()
+        >>> client = tweeter.get_client() # Retrieve your tweety client object
+        >>> client.create_tweet(text="Hello World!") # Tweet Hello World using your account's client
         """
         return self.__client
 
     def tweet(self, title: str|None = None, tweet: str|None = None, articles_list: list|None = None, use_palm: bool = False, prompt: str|None = None) -> dict:
         """Tweet the given articles list
 
         Parameters
@@ -363,14 +433,38 @@
             If use_palm is True and tweet or articles_list is not None
         ValueError
             If use_palm is True and prompt is None
         ValueError
             If tweet and articles_list are both not None
         TypeError
             If prompt is not a string
+
+        Examples
+        --------
+
+        Provide a title and tweet to be posted:
+
+        >>> from twitternewsbot.tweeter import Tweeter
+        >>> tweeter = Tweeter()
+        >>> tweeter.tweet(title="Hello World", tweet="Hello World!")
+
+        Provide a title and articles list to be posted:
+
+        >>> from twitternewsbot.tweeter import Tweeter
+        >>> from twitternewsbot.newsfinder import NewsFinder
+        >>> tweeter = Tweeter()
+        >>> newsfinder = NewsFinder()
+        >>> articles_list = newsfinder.get_news_articles(topic="Bitcoin", num_articles=5, article_text=True) # Article Text must be True if summarizing articles
+        >>> tweeter.tweet(title="Bitcoin News", articles_list=articles_list)
+
+        Provide a prompt to be used with PaLM to generate a tweet:
+
+        >>> from twitternewsbot.tweeter import Tweeter
+        >>> tweeter = Tweeter()
+        >>> tweeter.tweet(title="AI", use_palm=True, prompt="Create a 50 word description of what Artificial Intelligence is.")
         """
 
         # Check if title is valid
         if title is not None and not isinstance(title, str):
             raise TypeError("title must be a string")
         
         # Check if tweet is valid
```

### Comparing `twitternewsbot-2.0.2/twitternewsbot.egg-info/PKG-INFO` & `twitternewsbot-2.0.3/twitternewsbot.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 Metadata-Version: 2.1
 Name: twitternewsbot
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python API allowing you to automize a personalized news delivery system.
 Home-page: https://github.com/arnavmarda/twitter-news-bot/
-Download-URL: https://github.com/arnavmarda/twitter-news-bot/archive/refs/tags/v2.0.tar.gz
+Download-URL: https://github.com/arnavmarda/twitter-news-bot/archive/refs/tags/v2.0.3.tar.gz
 Author: Arnav Marda
 Author-email: arnavmarda@gmail.com
 License: MIT
-Keywords: AI,Twitter,News,Automation
+Keywords: AI,Twitter,News,Automation,Google News,Scraping,Requests,Tweepy,Articles
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-<div align=center>
+<div align="center">
 <img alt="Logo" src="https://github.com/arnavmarda/twitter-news-bot/blob/main/docs/logo.png" width=200 />
 </div>
 
+<div align="center">
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/twitternewsbot.svg)](https://badge.fury.io/py/twitternewsbot)
+
+[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+
+</div>
+
 # twitter-news-bot
 
 A python API allowing users to:
 
 1. Scrape news articles from Google News.
 2. Extract the articles from the news sources.
 3. Create and post tweets(or now Xs) using `tweepy`.
```

