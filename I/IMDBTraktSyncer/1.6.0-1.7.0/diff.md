# Comparing `tmp/IMDBTraktSyncer-1.6.0.tar.gz` & `tmp/IMDBTraktSyncer-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.6.0.tar", last modified: Wed Jul 26 21:56:53 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.7.0.tar", last modified: Sat Jul 29 10:47:31 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.6.0.tar` & `IMDBTraktSyncer-1.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 21:56:53.150218 IMDBTraktSyncer-1.6.0/
-drwxrwxrwx   0        0        0        0 2023-07-26 21:56:53.119219 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    39380 2023-07-26 21:50:56.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     6946 2023-06-27 06:49:08.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1669 2023-06-25 00:09:11.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0    10884 2023-06-28 04:22:19.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0    10353 2023-06-19 09:48:23.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0    12192 2023-06-19 15:47:42.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-07-26 21:56:53.148218 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    12569 2023-07-26 21:56:52.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-07-26 21:56:52.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 21:56:52.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-07-26 21:56:52.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-07-26 21:56:52.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-26 21:56:52.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.6.0/LICENSE
--rw-rw-rw-   0        0        0    12569 2023-07-26 21:56:53.150218 IMDBTraktSyncer-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0    11822 2023-07-26 21:55:34.000000 IMDBTraktSyncer-1.6.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-26 21:56:53.151209 IMDBTraktSyncer-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1377 2023-07-26 21:56:19.000000 IMDBTraktSyncer-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:47:31.735836 IMDBTraktSyncer-1.7.0/
+drwxrwxrwx   0        0        0        0 2023-07-29 10:47:31.700848 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    40858 2023-07-29 10:44:06.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     6946 2023-06-27 06:49:08.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1669 2023-06-25 00:09:11.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0    11362 2023-07-29 10:06:33.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0    10572 2023-07-29 08:41:16.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0    12192 2023-06-19 15:47:42.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-07-29 10:47:31.733846 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12719 2023-07-29 10:47:31.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-07-29 10:47:31.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 10:47:31.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-29 10:47:31.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-07-29 10:47:31.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-29 10:47:31.000000 IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0    12719 2023-07-29 10:47:31.734845 IMDBTraktSyncer-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11972 2023-07-29 10:46:05.000000 IMDBTraktSyncer-1.7.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-29 10:47:31.735836 IMDBTraktSyncer-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-07-29 10:46:25.000000 IMDBTraktSyncer-1.7.0/setup.py
```

### Comparing `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import json
 import requests
 import time
+from datetime import datetime
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import NoSuchElementException, TimeoutException, StaleElementReferenceException
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
@@ -116,30 +117,57 @@
             EL.logger.error("Error: Not signed in to IMDB")
             driver.quit()
             service.stop()
             raise SystemExit
         
         trakt_watchlist, trakt_ratings, trakt_reviews, watched_content = traktData.getTraktData()
         imdb_watchlist, imdb_ratings, imdb_reviews, errors_found_getting_imdb_reviews = imdbData.getImdbData(imdb_username, imdb_password, driver, directory, wait)
-
+        
         # Get trakt and imdb data and filter out items with missing imdb id
         trakt_ratings = [rating for rating in trakt_ratings if rating.get('IMDB_ID') is not None]
         imdb_ratings = [rating for rating in imdb_ratings if rating.get('IMDB_ID') is not None]
         trakt_reviews = [review for review in trakt_reviews if review.get('IMDB_ID') is not None]
         imdb_reviews = [review for review in imdb_reviews if review.get('IMDB_ID') is not None]
         trakt_watchlist = [item for item in trakt_watchlist if item.get('IMDB_ID') is not None]
         imdb_watchlist = [item for item in imdb_watchlist if item.get('IMDB_ID') is not None]
         # Filter out items already set
         imdb_ratings_to_set = [rating for rating in trakt_ratings if rating['IMDB_ID'] not in [imdb_rating['IMDB_ID'] for imdb_rating in imdb_ratings]]
         trakt_ratings_to_set = [rating for rating in imdb_ratings if rating['IMDB_ID'] not in [trakt_rating['IMDB_ID'] for trakt_rating in trakt_ratings]]
         imdb_reviews_to_set = [review for review in trakt_reviews if review['IMDB_ID'] not in [imdb_review['IMDB_ID'] for imdb_review in imdb_reviews]]
         trakt_reviews_to_set = [review for review in imdb_reviews if review['IMDB_ID'] not in [trakt_review['IMDB_ID'] for trakt_review in trakt_reviews]]
         imdb_watchlist_to_set = [item for item in trakt_watchlist if item['IMDB_ID'] not in [imdb_item['IMDB_ID'] for imdb_item in imdb_watchlist]]
         trakt_watchlist_to_set = [item for item in imdb_watchlist if item['IMDB_ID'] not in [trakt_item['IMDB_ID'] for trakt_item in trakt_watchlist]]
-        # Filter out items where the comment length is less than 600 characters
+        
+        # Filter ratings to update
+        imdb_ratings_to_update = []
+        trakt_ratings_to_update = []
+
+        # Dictionary to store IMDB_IDs and their corresponding ratings for IMDB and Trakt
+        imdb_ratings_dict = {rating['IMDB_ID']: rating for rating in imdb_ratings}
+        trakt_ratings_dict = {rating['IMDB_ID']: rating for rating in trakt_ratings}
+
+        # Include only items with the same IMDB_ID and different ratings and prefer the most recent rating
+        for imdb_id, imdb_rating in imdb_ratings_dict.items():
+            if imdb_id in trakt_ratings_dict:
+                trakt_rating = trakt_ratings_dict[imdb_id]
+                if imdb_rating['Rating'] != trakt_rating['Rating']:
+                    imdb_date_added = datetime.fromisoformat(imdb_rating['Date_Added'])
+                    trakt_date_added = datetime.fromisoformat(trakt_rating['Date_Added'])
+                    
+                    # If IMDB rating is more recent, add the Trakt rating to the update list, and vice versa
+                    if imdb_date_added > trakt_date_added:
+                        trakt_ratings_to_update.append(imdb_rating)
+                    else:
+                        imdb_ratings_to_update.append(trakt_rating)
+
+        # Update ratings_to_set
+        imdb_ratings_to_set.extend(imdb_ratings_to_update)
+        trakt_ratings_to_set.extend(trakt_ratings_to_update)
+        
+        # Filter out review items where the comment length is less than 600 characters
         def filter_by_comment_length(lst, min_comment_length=None):
             result = []
             for item in lst:
                 if min_comment_length is None or ('Comment' in item and len(item['Comment']) >= min_comment_length):
                     result.append(item)
             return result
         imdb_reviews_to_set = filter_by_comment_length(imdb_reviews_to_set, 600)
@@ -373,15 +401,15 @@
                             
                             # Wait until rate button is located and scroll to it
                             button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
                             driver.execute_script("arguments[0].scrollIntoView(true);", button)
 
                             # click on "Rate" button and select rating option, then submit rating
                             button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
-                            element_rating_bar = button.find_element(By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating__unrated"]')
+                            element_rating_bar = button.find_element(By.CSS_SELECTOR, '[data-testid*="hero-rating-bar__user-rating__"]')
                             if element_rating_bar:
                                 driver.execute_script("arguments[0].click();", button)
                                 rating_option_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, f'button[aria-label="Rate {item["Rating"]}"]')))
                                 driver.execute_script("arguments[0].click();", rating_option_element)
                                 submit_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button.ipc-rating-prompt__rate-button')))
                                 submit_element.click()
                                 time.sleep(1)
```

### Comparing `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/errorLogger.py` & `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/errorLogger.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/imdbData.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import time
 import csv
 import requests
+from datetime import datetime
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import NoSuchElementException, TimeoutException, StaleElementReferenceException
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
@@ -49,23 +50,26 @@
             with open(watchlist_path, 'r', encoding='utf-8') as file:
                 reader = csv.reader(file)
                 header = next(reader)  # skip the header row
                 for row in reader:
                     title = row[5]
                     year = row[10]
                     imdb_id = row[1]
+                    date_added = row[2]
+                    # Convert date format
+                    date_added = datetime.strptime(date_added, '%Y-%m-%d').strftime('%Y-%m-%dT%H:%M:%S.000Z')
                     if "tvSeries" in row[7] or "tvMiniSeries" in row[7]:
                         media_type = "show"
                     elif "tvEpisode" in row[7]:
                         media_type = "episode"
                     elif "movie" in row[7]:
                         media_type = "movie"
                     else:
                         media_type = "unknown"
-                    imdb_watchlist.append({'Title': title, 'Year': year, 'IMDB_ID': imdb_id, 'Type': media_type})
+                    imdb_watchlist.append({'Title': title, 'Year': year, 'IMDB_ID': imdb_id, 'Date_Added': date_added, 'Type': media_type})
         except FileNotFoundError:
             error_message = "Ratings file not found"
             print(f"{error_message}")
             EL.logger.error(error_message, exc_info=True)
             
         # Delete csv files
         for file in os.listdir(directory):
@@ -104,23 +108,26 @@
                 reader = csv.reader(file)
                 header = next(reader)  # skip the header row
                 for row in reader:
                     title = row[3]
                     year = row[8]
                     rating = row[1]
                     imdb_id = row[0]
+                    date_added = row[2]
+                    # Convert date format
+                    date_added = datetime.strptime(date_added, '%Y-%m-%d').strftime('%Y-%m-%dT%H:%M:%S.000Z')
                     if "tvSeries" in row[5] or "tvMiniSeries" in row[5]:
                         media_type = "show"
                     elif "tvEpisode" in row[5]:
                         media_type = "episode"
                     elif "movie" in row[5]:
                         media_type = "movie"
                     else:
                         media_type = "unknown"
-                    imdb_ratings.append({'Title': title, 'Year': year, 'Rating': rating, 'IMDB_ID': imdb_id, 'Type': media_type})
+                    imdb_ratings.append({'Title': title, 'Year': year, 'Rating': int(rating), 'IMDB_ID': imdb_id, 'Date_Added': date_added, 'Type': media_type})
         except FileNotFoundError:
             print('Ratings file not found')
             
         # Delete csv files
         for file in os.listdir(directory):
             if file.endswith('.csv') and 'ratings' in file:
                 os.remove(os.path.join(directory, file))
```

### Comparing `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/traktData.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,53 +26,53 @@
     trakt_watchlist = []
 
     for item in json_data:
         if item['type'] == 'movie':
             movie = item.get('movie')
             imdb_movie_id = movie.get('ids', {}).get('imdb')
             trakt_movie_id = movie.get('ids', {}).get('trakt')
-            trakt_watchlist.append({'Title': movie.get('title'), 'Year': movie.get('year'), 'IMDB_ID': imdb_movie_id, 'TraktID': trakt_movie_id, 'Type': 'movie'})
+            trakt_watchlist.append({'Title': movie.get('title'), 'Year': movie.get('year'), 'IMDB_ID': imdb_movie_id, 'TraktID': trakt_movie_id, 'Date_Added': item.get('listed_at'), 'Type': 'movie'})
         elif item['type'] == 'show':
             show = item.get('show')
             imdb_show_id = show.get('ids', {}).get('imdb')
             trakt_show_id = show.get('ids', {}).get('trakt')
-            trakt_watchlist.append({'Title': show.get('title'), 'Year': show.get('year'), 'IMDB_ID': imdb_show_id, 'TraktID': trakt_show_id, 'Type': 'show'})
+            trakt_watchlist.append({'Title': show.get('title'), 'Year': show.get('year'), 'IMDB_ID': imdb_show_id, 'TraktID': trakt_show_id, 'Date_Added': item.get('listed_at'), 'Type': 'show'})
         elif item['type'] == 'episode':
             show = item.get('show')
             show_title = show.get('title')
             episode = item.get('episode')
             imdb_episode_id = episode.get('ids', {}).get('imdb')
             trakt_episode_id = episode.get('ids', {}).get('trakt')
             episode_title = f'{show_title}: {episode.get("title")}'
-            trakt_watchlist.append({'Title': episode_title, 'Year': episode.get('year'), 'IMDB_ID': imdb_episode_id, 'TraktID': trakt_episode_id, 'Type': 'episode'})
+            trakt_watchlist.append({'Title': episode_title, 'Year': episode.get('year'), 'IMDB_ID': imdb_episode_id, 'TraktID': trakt_episode_id, 'Date_Added': item.get('listed_at'), 'Type': 'episode'})
     
     # Get Trakt Ratings
     response = EH.make_trakt_request(f'https://api.trakt.tv/users/{encoded_username}/ratings?sort=newest')
     json_data = json.loads(response.text)
 
     movie_ratings = []
     show_ratings = []
     episode_ratings = []
 
     for item in json_data:
         if item['type'] == 'movie':
             movie = item.get('movie')
             movie_id = movie.get('ids', {}).get('imdb')
-            movie_ratings.append({'Title': movie.get('title'), 'Year': movie.get('year'), 'Rating': item.get('rating'), 'IMDB_ID': movie_id, 'Type': 'movie'})
+            movie_ratings.append({'Title': movie.get('title'), 'Year': movie.get('year'), 'Rating': item.get('rating'), 'IMDB_ID': movie_id, 'Date_Added': item.get('rated_at'), 'Type': 'movie'})
         elif item['type'] == 'show':
             show = item.get('show')
             show_id = show.get('ids', {}).get('imdb')
-            show_ratings.append({'Title': show.get('title'), 'Year': show.get('year'), 'Rating': item.get('rating'), 'IMDB_ID': show_id, 'Type': 'show'})
+            show_ratings.append({'Title': show.get('title'), 'Year': show.get('year'), 'Rating': item.get('rating'), 'IMDB_ID': show_id, 'Date_Added': item.get('rated_at'), 'Type': 'show'})
         elif item['type'] == 'episode':
             show = item.get('show')
             show_title = show.get('title')
             episode = item.get('episode')
             episode_id = episode.get('ids', {}).get('imdb')
             episode_title = f'{show_title}: {episode.get("title")}'
-            episode_ratings.append({'Title': episode_title, 'Year': episode.get('year'), 'Rating': item.get('rating'), 'IMDB_ID': episode_id, 'Type': 'episode'})
+            episode_ratings.append({'Title': episode_title, 'Year': episode.get('year'), 'Rating': item.get('rating'), 'IMDB_ID': episode_id, 'Date_Added': item.get('rated_at'), 'Type': 'episode'})
 
     trakt_ratings = movie_ratings + show_ratings + episode_ratings
 
     # Get Trakt Comments
     response = EH.make_trakt_request(f'https://api.trakt.tv/users/{encoded_username}/comments?sort=newest')
     json_data = json.loads(response.text)
     total_pages = response.headers.get('X-Pagination-Page-Count')
```

### Comparing `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.6.0
+Version: 1.7.0
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 
 # IMDB-Trakt-Syncer
 This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Existing items will not be overwritten. Ratings, watchlist and comment/review sync are all optional. The user will be prompted to enter their settings and credentials on first run.
 
 The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux and Mac). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/IMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During installation, tick the box for adding Python to your PATH variable. _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## Installing the Script:
@@ -51,15 +51,15 @@
 ## Installing a Specific Version:
 ```
 python -m pip install IMDBTraktSyncer==VERSION_NUMBER
 ```
 _Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) (e.g. 1.1.6) and run in your operating system's native command line._
 
 ## Alternative Manual Installation Method (without pip install)
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/).  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During installation, tick the box for adding Python to your PATH variable.  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run `IMDBTraktSyncer.py` or open the terminal and navigate to the folder where `IMDBTraktSyncer.py` is located. Run `IMDBTraktSyncer.py` in the terminal.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## For Setting Up Automation See the Following Wiki Pages:
```

### Comparing `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.7.0/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.6.0/LICENSE` & `IMDBTraktSyncer-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.6.0/PKG-INFO` & `IMDBTraktSyncer-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.6.0
+Version: 1.7.0
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 
 # IMDB-Trakt-Syncer
 This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Existing items will not be overwritten. Ratings, watchlist and comment/review sync are all optional. The user will be prompted to enter their settings and credentials on first run.
 
 The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux and Mac). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/IMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During installation, tick the box for adding Python to your PATH variable. _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## Installing the Script:
@@ -51,15 +51,15 @@
 ## Installing a Specific Version:
 ```
 python -m pip install IMDBTraktSyncer==VERSION_NUMBER
 ```
 _Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) (e.g. 1.1.6) and run in your operating system's native command line._
 
 ## Alternative Manual Installation Method (without pip install)
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/).  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During installation, tick the box for adding Python to your PATH variable.  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run `IMDBTraktSyncer.py` or open the terminal and navigate to the folder where `IMDBTraktSyncer.py` is located. Run `IMDBTraktSyncer.py` in the terminal.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## For Setting Up Automation See the Following Wiki Pages:
```

### Comparing `IMDBTraktSyncer-1.6.0/README.md` & `IMDBTraktSyncer-1.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # IMDB-Trakt-Syncer
 This Python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Existing items will not be overwritten. Ratings, watchlist and comment/review sync are all optional. The user will be prompted to enter their settings and credentials on first run.
 
 The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux and Mac). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/IMDB-Trakt-Syncer#other-recommended-projects).
 
 ## Installation Instructions
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During installation, tick the box for adding Python to your PATH variable. _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## Installing the Script:
@@ -35,15 +35,15 @@
 ## Installing a Specific Version:
 ```
 python -m pip install IMDBTraktSyncer==VERSION_NUMBER
 ```
 _Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) (e.g. 1.1.6) and run in your operating system's native command line._
 
 ## Alternative Manual Installation Method (without pip install)
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/).  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). During installation, tick the box for adding Python to your PATH variable.  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run `IMDBTraktSyncer.py` or open the terminal and navigate to the folder where `IMDBTraktSyncer.py` is located. Run `IMDBTraktSyncer.py` in the terminal.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
 6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## For Setting Up Automation See the Following Wiki Pages:
```

### Comparing `IMDBTraktSyncer-1.6.0/setup.py` & `IMDBTraktSyncer-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.6.0'
+VERSION = '1.7.0'
 DESCRIPTION = 'A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

