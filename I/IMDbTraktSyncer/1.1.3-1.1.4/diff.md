# Comparing `tmp/IMDbTraktSyncer-1.1.3.tar.gz` & `tmp/IMDbTraktSyncer-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDbTraktSyncer-1.1.3.tar", last modified: Mon May 15 08:57:01 2023, max compression
+gzip compressed data, was "IMDbTraktSyncer-1.1.4.tar", last modified: Tue May 16 01:36:43 2023, max compression
```

## Comparing `IMDbTraktSyncer-1.1.3.tar` & `IMDbTraktSyncer-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 08:57:01.719166 IMDbTraktSyncer-1.1.3/
-drwxrwxrwx   0        0        0        0 2023-05-15 08:57:01.684212 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/
--rw-rw-rw-   0        0        0    10477 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/IMDbTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4079 2023-05-15 08:55:47.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     2060 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/imdbRatings.py
--rw-rw-rw-   0        0        0     1408 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     2516 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:57:01.716669 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     6624 2023-05-15 08:57:01.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-05-15 08:57:01.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 08:57:01.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-15 08:57:01.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-15 08:57:01.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-15 08:57:01.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     6624 2023-05-15 08:57:01.718667 IMDbTraktSyncer-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6004 2023-05-15 08:56:12.000000 IMDbTraktSyncer-1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-15 08:57:01.719674 IMDbTraktSyncer-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1287 2023-05-15 08:56:35.000000 IMDbTraktSyncer-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:36:43.516004 IMDbTraktSyncer-1.1.4/
+drwxrwxrwx   0        0        0        0 2023-05-16 01:36:43.483057 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/
+-rw-rw-rw-   0        0        0    10838 2023-05-16 01:11:24.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/IMDbTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-05-15 09:11:52.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4079 2023-05-15 09:11:52.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     2256 2023-05-16 00:33:22.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/imdbRatings.py
+-rw-rw-rw-   0        0        0     1876 2023-05-16 01:32:19.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     2516 2023-05-15 09:11:52.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:36:43.513507 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     6624 2023-05-16 01:36:43.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-05-16 01:36:43.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 01:36:43.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-16 01:36:43.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-16 01:36:43.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-16 01:36:43.000000 IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     6624 2023-05-16 01:36:43.515005 IMDbTraktSyncer-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6004 2023-05-15 08:56:12.000000 IMDbTraktSyncer-1.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 01:36:43.516004 IMDbTraktSyncer-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1287 2023-05-16 01:36:21.000000 IMDbTraktSyncer-1.1.4/setup.py
```

### Comparing `IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/IMDbTraktSyncer.py` & `IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/IMDbTraktSyncer.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,37 +117,32 @@
     trakt_ratings_to_set = [rating for rating in imdb_ratings if rating['ID'] not in [trakt_rating['ID'] for trakt_rating in trakt_ratings]]
 
     if imdb_ratings_to_set:
         print('Setting IMDB Ratings')
 
         # loop through each movie and TV show rating and submit rating on IMDb website
         for i, item in enumerate(imdb_ratings_to_set, 1):
-            print(f'Rating {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]} ({item["Year"]}): {item["Rating"]}/10 on IMDb')
+            year_str = f' ({item["Year"]})' if item["Year"] is not None else '' # sometimes year is None for episodes from trakt so remove it from the print string
+            print(f'Rating {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]}{year_str}: {item["Rating"]}/10 on IMDb')
             driver.get(f'https://www.imdb.com/title/{item["ID"]}/')
-            time.sleep(2)
 
             # click on "Rate" button and select rating option, then submit rating
-            buttons = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, 'button.ipc-btn span')))
-            found_rate_button = False
-            for button in buttons:
-                try:
-                    element_rating_bar = button.find_element(By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating__unrated"]')
-                    if element_rating_bar:
-                        driver.execute_script("arguments[0].click();", button)
-                        rating_option_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, f'button[aria-label="Rate {item["Rating"]}"]')))
-                        driver.execute_script("arguments[0].click();", rating_option_element)
-                        submit_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button.ipc-rating-prompt__rate-button')))
-                        submit_element.click()
-                        found_rate_button = True
-                        break
-                except:
-                    continue
-
-            if not found_rate_button:
+            button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button.ipc-btn span')))
+            try:
+                element_rating_bar = button.find_element(By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating__unrated"]')
+                if element_rating_bar:
+                    driver.execute_script("arguments[0].click();", button)
+                    rating_option_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, f'button[aria-label="Rate {item["Rating"]}"]')))
+                    driver.execute_script("arguments[0].click();", rating_option_element)
+                    submit_element = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button.ipc-rating-prompt__rate-button')))
+                    submit_element.click()
+                    time.sleep(1)
+            except:
                 continue
+
         print('Setting IMDb Ratings Complete')
     else:
         print('No IMDb Ratings To Set')
 
     if trakt_ratings_to_set:
         print('Setting Trakt Ratings')
 
@@ -176,26 +171,37 @@
                     "shows": [{
                         "ids": {
                             "imdb": item["ID"]
                         },
                         "rating": item["Rating"]
                     }]
                 }
-                print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}) with rating {item['Rating']}/10 on Trakt")
+                print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
             elif item["Type"] == "movie":
                 # This is a movie
                 data = {
                     "movies": [{
                         "ids": {
                             "imdb": item["ID"]
                         },
                         "rating": item["Rating"]
                     }]
                 }
-                print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}) with rating {item['Rating']}/10 on Trakt")
+                print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
+            elif item["Type"] == "episode":
+                # This is an episode
+                data = {
+                    "episodes": [{
+                        "ids": {
+                            "imdb": item["ID"]
+                        },
+                        "rating": item["Rating"]
+                    }]
+                }
+                print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
 
             # Make the API call to rate the item
             response = requests.post(rate_url, headers=headers, json=data)
             time.sleep(1)
             while response.status_code == 429:
                 print("Rate limit exceeded. Waiting for 1 second...")
                 time.sleep(1)
```

### Comparing `IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/authTrakt.py` & `IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/checkChromedriver.py` & `IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/imdbRatings.py` & `IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/imdbRatings.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,18 +35,22 @@
             reader = csv.reader(file)
             header = next(reader)  # skip the header row
             for row in reader:
                 title = row[3]
                 year = row[8]
                 rating = row[1]
                 imdb_id = row[0]
-                if "tv" in row[5]:
+                if "tvSeries" in row[5] or "tvMiniSeries" in row[5]:
                     type = "show"
-                else:
+                elif "tvEpisode" in row[5]:
+                    type = "episode"
+                elif "movie" in row[5]:
                     type = "movie"
+                else:
+                    type = "unknown"
                 imdb_ratings.append({'Title': title, 'Year': year, 'Rating': rating, 'ID': imdb_id, 'Type': type})
     except FileNotFoundError:
         print('Ratings file not found')
         
     # Delete csv files
     for file in os.listdir(directory):
         if file.endswith('.csv') and 'ratings' in file:
```

### Comparing `IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/traktRatings.py` & `IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/traktRatings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import json
 import subprocess
 import requests
 
 def getTraktRatings(trakt_client_id, trakt_access_token):
-    #Get Trakt Ratings
+    # Get Trakt Ratings
     print('Getting Trakt Ratings')
 
     headers = {
         'Content-Type': 'application/json',
         'trakt-api-version': '2',
         'trakt-api-key': trakt_client_id,
         'Authorization': f'Bearer {trakt_access_token}'
@@ -18,23 +18,31 @@
     json_data = json.loads(response.text)
     username = json_data['username']
     response = requests.get(f'https://api.trakt.tv/users/{username}/ratings', headers=headers)
     json_data = json.loads(response.text)
 
     movie_ratings = []
     show_ratings = []
+    episode_ratings = []
 
     for item in json_data:
         if item['type'] == 'movie':
             movie = item['movie']
             movie_id = movie['ids']['imdb']
             movie_ratings.append({'Title': movie['title'], 'Year': movie['year'], 'Rating': item['rating'], 'ID': movie_id, 'Type': 'movie'})
         elif item['type'] == 'show':
             show = item['show']
             show_id = show['ids']['imdb']
             show_ratings.append({'Title': show['title'], 'Year': show['year'], 'Rating': item['rating'], 'ID': show_id, 'Type': 'show'})
+        elif item['type'] == 'episode':
+            show = item['show']
+            show_title = show['title']
+            episode = item['episode']
+            episode_id = episode['ids']['imdb']
+            episode_title = f'{show_title}: {episode["title"]}'
+            episode_ratings.append({'Title': episode_title, 'Year': episode.get('year'), 'Rating': item['rating'], 'ID': episode_id, 'Type': 'episode'})
 
-    trakt_ratings = movie_ratings + show_ratings
+    trakt_ratings = movie_ratings + show_ratings + episode_ratings
 
     print('Getting Trakt Ratings Complete')
     
-    return trakt_ratings
+    return trakt_ratings
```

### Comparing `IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/verifyCredentials.py` & `IMDbTraktSyncer-1.1.4/IMDbTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/PKG-INFO` & `IMDbTraktSyncer-1.1.4/IMDbTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.1.3
+Version: 1.1.4
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDbTraktSyncer-1.1.3/LICENSE` & `IMDbTraktSyncer-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.3/PKG-INFO` & `IMDbTraktSyncer-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.1.3
+Version: 1.1.4
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDbTraktSyncer-1.1.3/README.md` & `IMDbTraktSyncer-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.3/setup.py` & `IMDbTraktSyncer-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.3'
+VERSION = '1.1.4'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.'
 
 # Setting up
 setup(
     name="IMDbTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

