# Comparing `tmp/rottentomatoes-python-0.5.17.tar.gz` & `tmp/rottentomatoes-python-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rottentomatoes-python-0.5.17.tar", last modified: Tue May 16 19:34:45 2023, max compression
+gzip compressed data, was "rottentomatoes-python-0.5.2.tar", last modified: Mon Feb 13 00:20:25 2023, max compression
```

## Comparing `rottentomatoes-python-0.5.17.tar` & `rottentomatoes-python-0.5.2.tar`

### file list

```diff
@@ -1,26 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:34:45.666593 rottentomatoes-python-0.5.17/
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-05-16 19:34:45.666593 rottentomatoes-python-0.5.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-05-16 19:34:18.000000 rottentomatoes-python-0.5.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:34:45.662593 rottentomatoes-python-0.5.17/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-16 19:34:18.000000 rottentomatoes-python-0.5.17/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-16 19:34:18.000000 rottentomatoes-python-0.5.17/api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:34:45.666593 rottentomatoes-python-0.5.17/rottentomatoes/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 19:34:18.000000 rottentomatoes-python-0.5.17/rottentomatoes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-16 19:34:18.000000 rottentomatoes-python-0.5.17/rottentomatoes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-16 19:34:18.000000 rottentomatoes-python-0.5.17/rottentomatoes/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-16 19:34:18.000000 rottentomatoes-python-0.5.17/rottentomatoes/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-05-16 19:34:18.000000 rottentomatoes-python-0.5.17/rottentomatoes/standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-16 19:34:18.000000 rottentomatoes-python-0.5.17/rottentomatoes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:34:45.666593 rottentomatoes-python-0.5.17/rottentomatoes_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-05-16 19:34:45.000000 rottentomatoes-python-0.5.17/rottentomatoes_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-16 19:34:45.000000 rottentomatoes-python-0.5.17/rottentomatoes_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:34:45.000000 rottentomatoes-python-0.5.17/rottentomatoes_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 19:34:45.000000 rottentomatoes-python-0.5.17/rottentomatoes_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 19:34:45.000000 rottentomatoes-python-0.5.17/rottentomatoes_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 19:34:45.666593 rottentomatoes-python-0.5.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-16 19:34:18.000000 rottentomatoes-python-0.5.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:34:45.666593 rottentomatoes-python-0.5.17/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:34:18.000000 rottentomatoes-python-0.5.17/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-16 19:34:18.000000 rottentomatoes-python-0.5.17/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-16 19:34:18.000000 rottentomatoes-python-0.5.17/tests/test_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-16 19:34:18.000000 rottentomatoes-python-0.5.17/tests/test_standalone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 00:20:25.695365 rottentomatoes-python-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-02-13 00:20:25.695365 rottentomatoes-python-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-02-13 00:20:05.000000 rottentomatoes-python-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 00:20:25.691365 rottentomatoes-python-0.5.2/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-02-13 00:20:05.000000 rottentomatoes-python-0.5.2/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 00:20:25.695365 rottentomatoes-python-0.5.2/rottentomatoes/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-13 00:20:05.000000 rottentomatoes-python-0.5.2/rottentomatoes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-13 00:20:05.000000 rottentomatoes-python-0.5.2/rottentomatoes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-02-13 00:20:05.000000 rottentomatoes-python-0.5.2/rottentomatoes/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-02-13 00:20:05.000000 rottentomatoes-python-0.5.2/rottentomatoes/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-02-13 00:20:05.000000 rottentomatoes-python-0.5.2/rottentomatoes/standalone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 00:20:25.695365 rottentomatoes-python-0.5.2/rottentomatoes_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-02-13 00:20:25.000000 rottentomatoes-python-0.5.2/rottentomatoes_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-13 00:20:25.000000 rottentomatoes-python-0.5.2/rottentomatoes_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 00:20:25.000000 rottentomatoes-python-0.5.2/rottentomatoes_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-13 00:20:25.000000 rottentomatoes-python-0.5.2/rottentomatoes_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-13 00:20:25.000000 rottentomatoes-python-0.5.2/rottentomatoes_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 00:20:25.695365 rottentomatoes-python-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-02-13 00:20:05.000000 rottentomatoes-python-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 00:20:25.695365 rottentomatoes-python-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-02-13 00:20:05.000000 rottentomatoes-python-0.5.2/tests/test_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-02-13 00:20:05.000000 rottentomatoes-python-0.5.2/tests/test_standalone.py
```

### Comparing `rottentomatoes-python-0.5.17/PKG-INFO` & `rottentomatoes-python-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rottentomatoes-python
-Version: 0.5.17
+Version: 0.5.2
 Summary: Scrape Rotten Tomatoes's website for basic information on movies, without the use of their hard-to-attain official REST API.
 Author: Prerit Das
 Author-email: <preritdas@gmail.com>
 Keywords: python,movies,rottentomatoes
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
@@ -13,24 +13,21 @@
 
 ![tests](https://github.com/preritdas/rottentomatoes-python/actions/workflows/pytest.yml/badge.svg)
 ![pypi](https://github.com/preritdas/rottentomatoes-python/actions/workflows/python-publish.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/rottentomatoes-python.svg)](https://badge.fury.io/py/rottentomatoes-python)
 ![versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)
 
 
-# :movie_camera: Rotten Tomatoes in Python (and API) :clapper:
+# Rotten Tomatoes in Python
 
 This package allows you to easily fetch Rotten Tomatoes scores and other movie data such as genres, without the use of the official Rotten Tomatoes API. The package scrapes their website for the data. I built this because unfortunately, to get access to their API, you have to submit a special request which takes an inordinate amount of time to process, or doesn't go through at all. 
 
 The package now, by default, scrapes the Rotten Tomatoes search page to find the true url of the first valid movie response (is a movie and has a tomatometer). This means queries that previously didn't work because their urls had a unique identifier or a year-released prefix, now work. The limitation of this new mechanism is that you only get the top response, and when searching for specific movies (sequels, by year, etc.) Rotten Tomatoes seems to return the same results as the original query. So, it's difficult to use specific queries to try and get the desired result movie as the top response. See #4 for more info on this.
 
-There is now an API deployed to make querying multiple movies and getting several responses easier. The endpoint is https://rotten-tomatoes-api.ue.r.appspot.com and it's open and free to use. Visit `/docs` or `/redoc` in the browser to view the endpoints. Both endpoints live right now are browser accessible meaning you don't need an HTTP client to use the API. 
-
-- https://rotten-tomatoes-api.ue.r.appspot.com/movie/bad_boys for JSON response of the top result
-- https://rotten-tomatoes-api.ue.r.appspot.com/search/bad_boys for a JSON response of all valid results
+There is now an API structure in place to make querying multiple movies and getting several responses easier. See the API section at the bottom for more.
 
 
 ## Usage
 
 You can either call the standalone functions `tomatometer`, `audience_score`, `genres`, etc., or use the `Movie` class to only pass the name and have each attribute be fetched automatically. If you use the `Movie` class, you can print all attributes by printing the object itself, or by accessing each attribute individually. 
 
 The weighted score is calculated using the formula $\frac{2}{3}(tomatometer) + \frac{1}{3}(audience)$. The result is then rounded to the nearest integer.
@@ -139,15 +136,15 @@
 Prominent actors: Tom Cruise, Miles Teller, Jennifer Connelly, Jon Hamm, Glen Powell.
 
 That took 0.3400420409961953 seconds.
 ```
 
 ## API
 
-The API is deployed at https://rotten-tomatoes-api.ue.r.appspot.com/. It has two endpoints currently, `/movie/{movie_name}` and `/search/{movie_name}`. The first will pull one movie, the top result. The second will pull a list of _all_ valid movie results.
+The API isn't deployed anywhere (for now) but you can run it locally. It has two endpoints, `/movie/{movie_name}` and `/search/{movie_name}`. The first will pull one movie, the top result. The second will pull a list of _all_ valid movie results.
 
 The first, with `movie_name="bad boys"`:
 
 ```json
 {
   "name": "Bad Boys for Life",
   "tomatometer": 76,
@@ -270,7 +267,11 @@
       "directors": [
         "Rick Rosenthal 2"
       ]
     }
   ]
 }
 ```
+
+When deployed you can do this in the browser too...
+
+`http(s)://localhostordeployment/movie/bad_boys` for JSON response of the top result, or `http(s)://localhostordeployment/search/bad_boys` for a JSON response of all valid results.
```

### Comparing `rottentomatoes-python-0.5.17/README.md` & `rottentomatoes-python-0.5.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 ![tests](https://github.com/preritdas/rottentomatoes-python/actions/workflows/pytest.yml/badge.svg)
 ![pypi](https://github.com/preritdas/rottentomatoes-python/actions/workflows/python-publish.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/rottentomatoes-python.svg)](https://badge.fury.io/py/rottentomatoes-python)
 ![versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)
 
 
-# :movie_camera: Rotten Tomatoes in Python (and API) :clapper:
+# Rotten Tomatoes in Python
 
 This package allows you to easily fetch Rotten Tomatoes scores and other movie data such as genres, without the use of the official Rotten Tomatoes API. The package scrapes their website for the data. I built this because unfortunately, to get access to their API, you have to submit a special request which takes an inordinate amount of time to process, or doesn't go through at all. 
 
 The package now, by default, scrapes the Rotten Tomatoes search page to find the true url of the first valid movie response (is a movie and has a tomatometer). This means queries that previously didn't work because their urls had a unique identifier or a year-released prefix, now work. The limitation of this new mechanism is that you only get the top response, and when searching for specific movies (sequels, by year, etc.) Rotten Tomatoes seems to return the same results as the original query. So, it's difficult to use specific queries to try and get the desired result movie as the top response. See #4 for more info on this.
 
-There is now an API deployed to make querying multiple movies and getting several responses easier. The endpoint is https://rotten-tomatoes-api.ue.r.appspot.com and it's open and free to use. Visit `/docs` or `/redoc` in the browser to view the endpoints. Both endpoints live right now are browser accessible meaning you don't need an HTTP client to use the API. 
-
-- https://rotten-tomatoes-api.ue.r.appspot.com/movie/bad_boys for JSON response of the top result
-- https://rotten-tomatoes-api.ue.r.appspot.com/search/bad_boys for a JSON response of all valid results
+There is now an API structure in place to make querying multiple movies and getting several responses easier. See the API section at the bottom for more.
 
 
 ## Usage
 
 You can either call the standalone functions `tomatometer`, `audience_score`, `genres`, etc., or use the `Movie` class to only pass the name and have each attribute be fetched automatically. If you use the `Movie` class, you can print all attributes by printing the object itself, or by accessing each attribute individually. 
 
 The weighted score is calculated using the formula $\frac{2}{3}(tomatometer) + \frac{1}{3}(audience)$. The result is then rounded to the nearest integer.
@@ -126,15 +123,15 @@
 Prominent actors: Tom Cruise, Miles Teller, Jennifer Connelly, Jon Hamm, Glen Powell.
 
 That took 0.3400420409961953 seconds.
 ```
 
 ## API
 
-The API is deployed at https://rotten-tomatoes-api.ue.r.appspot.com/. It has two endpoints currently, `/movie/{movie_name}` and `/search/{movie_name}`. The first will pull one movie, the top result. The second will pull a list of _all_ valid movie results.
+The API isn't deployed anywhere (for now) but you can run it locally. It has two endpoints, `/movie/{movie_name}` and `/search/{movie_name}`. The first will pull one movie, the top result. The second will pull a list of _all_ valid movie results.
 
 The first, with `movie_name="bad boys"`:
 
 ```json
 {
   "name": "Bad Boys for Life",
   "tomatometer": 76,
@@ -257,7 +254,11 @@
       "directors": [
         "Rick Rosenthal 2"
       ]
     }
   ]
 }
 ```
+
+When deployed you can do this in the browser too...
+
+`http(s)://localhostordeployment/movie/bad_boys` for JSON response of the top result, or `http(s)://localhostordeployment/search/bad_boys` for a JSON response of all valid results.
```

### Comparing `rottentomatoes-python-0.5.17/rottentomatoes/movie.py` & `rottentomatoes-python-0.5.2/rottentomatoes/movie.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.tomatometer = standalone.tomatometer(self.movie_title, content=content)
         self.audience_score = standalone.audience_score(self.movie_title, content=content)
         self.weighted_score = standalone.weighted_score(self.movie_title, content=content)
         self.genres = standalone.genres(self.movie_title, content=content)
         self.rating = standalone.rating(self.movie_title, content=content)
         self.duration = standalone.duration(self.movie_title, content=content)
         self.year_released = standalone.year_released(self.movie_title, content=content)
-        self.actors = standalone.actors(self.movie_title, content=content)
+        self.actors = standalone.actors(self.movie_title, max_actors=5, content=content)
         self.directors = standalone.directors(self.movie_title, max_directors=5, content=content)
 
     def __str__(self) -> str:
         return f"{self.movie_title.title()}, {self.rating}, {self.duration}.\n" \
             f"Released in {self.year_released}.\n" \
             f"Directed by {', '.join(self.actors)}.\n" \
             f"Tomatometer: {self.tomatometer}\n" \
```

### Comparing `rottentomatoes-python-0.5.17/rottentomatoes/search.py` & `rottentomatoes-python-0.5.2/rottentomatoes/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Search for movies. Use search page results to find absolute link. Write more/better docs later."""
 import requests
 
 import re
 from typing import List
 
-from . import utils
 from .exceptions import LookupError
 
 
 class SearchListing:
     """A search listing from the Rotten Tomatoes search page."""
     def __init__(self, has_tomatometer: bool, is_movie: bool, url: str) -> None:
         self.has_tomatometer = has_tomatometer
@@ -45,15 +44,15 @@
         return f"Tomatometer: {self.has_tomatometer}. URL: {self.url}. Is movie: {self.is_movie}."
 
 
 def _movie_search_content(name: str) -> str:
     """Raw HTML content from searching for a movie."""
     url_name = "%20".join(name.split())
     url = f"https://www.rottentomatoes.com/search?search={url_name}"
-    content = str(requests.get(url, headers=utils.REQUEST_HEADERS).content)
+    content = str(requests.get(url).content)
     
     # Remove misc quotes from conversion
     content = content[2:-1]
     return content
 
 
 def search_results(name: str) -> List[SearchListing]:
```

### Comparing `rottentomatoes-python-0.5.17/rottentomatoes/standalone.py` & `rottentomatoes-python-0.5.2/rottentomatoes/standalone.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """Standalone functions to fetch attributes about a movie."""
-from bs4 import BeautifulSoup
 
 # Non-local imports
 import json
 import requests  # interact with RT website
 from typing import List
 
 # Project modules
 from .exceptions import *
 from . import search
-from . import utils
 
 
 def _movie_url(movie_name: str) -> str:
     """Generates a target url on the Rotten Tomatoes website given
     the name of a movie.
 
     Args:
@@ -78,15 +76,15 @@
 
     Returns:
         object: The scoreboard data for the movie.
     """
     return json.loads(
         _extract(
             content,
-            '<script id="scoreDetails" type="application/json">',
+            '<script id="score-details-json" type="application/json">',
             '</script>'
         )
     )
 
 
 def _request(movie_name: str, raw_url: bool = False, force_url: str = "") -> str:
     """Scrapes Rotten Tomatoes for the raw website data, to be
@@ -107,15 +105,15 @@
     """
     if raw_url or force_url:
         rt_url = _movie_url(movie_name) if movie_name else force_url
     else:
         search_result = search.top_movie_result(movie_name)
         rt_url = search_result.url
     
-    response = requests.get(rt_url, headers=utils.REQUEST_HEADERS)
+    response = requests.get(rt_url)
 
     if response.status_code == 404:
         raise LookupError(
             "Unable to find that movie on Rotten Tomatoes.",
             f"Try this link to source the movie manually: {rt_url}"
         )
 
@@ -123,19 +121,19 @@
 
 
 def movie_title(movie_name: str, content: str = None) -> str:
     """Search for the movie and return the queried title."""
     if content is None:
         content = _request(movie_name)
 
-    find_str = '<meta property="og:title" content='
-    loc = content.find(find_str) + len(find_str)
+    find_str = "score-panel-movie-title"
+    loc = content.find(find_str) + len(find_str) + 2
     substring = content[loc:loc+100]  # enough breathing room
-    subs = substring.split('>')
-    return subs[0][1:-1]
+    subs = substring.split("<")
+    return subs[0]
 
 
 def tomatometer(movie_name: str, content: str = None) -> int:
     """Returns an integer of the Rotten Tomatoes tomatometer
     of `movie_name`. 
 
     Args:
@@ -148,15 +146,15 @@
 
     Returns:
         int: Tomatometer of `movie_name`.
     """
     if content is None:
         content = _request(movie_name)
 
-    return _get_score_details(content)['scoreboard']['tomatometerScore']["value"]
+    return _get_score_details(content)['scoreboard']['tomatometerScore']
 
 
 def audience_score(movie_name: str, content: str = None) -> int:
     """Returns an integer of the Rotten Tomatoes tomatometer
     of `movie_name`. 
 
     Args:
@@ -169,15 +167,15 @@
 
     Returns:
         int: Tomatometer of `movie_name`.
     """
     if content is None:
         content = _request(movie_name)
 
-    return _get_score_details(content)['scoreboard']['audienceScore']["value"]
+    return _get_score_details(content)['scoreboard']['audienceScore']
 
 
 def genres(movie_name: str, content: str = None) -> List[str]:
     """Returns an integer of the Rotten Tomatoes tomatometer
     of `movie_name`. Copies the movie url to clipboard.
 
     Args:
@@ -230,38 +228,34 @@
         content = _request(movie_name)
 
     release_year = _get_score_details(
         content)['scoreboard']['info'].split(',')[0]
     return release_year
 
 
-def actors(movie_name: str, content: str = None) -> List[str]:
-    """
-    Returns a list of the top 5 actors listed by Rotten Tomatoes.
-    """
+def actors(movie_name: str, max_actors: int = 100, content: str = None) -> List[str]:
+    """Returns a list of all the actors listed
+    by Rotten Tomatoes. Specify `max_actors` to only receive
+    a certain number of the most prominent actors in the film."""
     if content is None:
         content = _request(movie_name)
 
-    def _get_top_n_actors(html, n):
-        soup = BeautifulSoup(html, 'html.parser')
-        cast_items = soup.find_all('div', {'data-qa': 'cast-crew-item'})
-        
-        top_actors = []
-        
-        for i, cast_item in enumerate(cast_items):
-            if i == n:
-                break
-            
-            actor_name = cast_item.find('p').text.strip()
-            top_actors.append(actor_name)
-        
-        return top_actors
-
-    return _get_top_n_actors(content, 5)
+    # Find all instances
+    actors = []
+    start_string = '<span class="characters subtle smaller" title="'
+    while len(actors) < max_actors:
+        actor = _extract(content, start_string, '">')
+        # If no other actors can be extracted
+        if actor is None:
+            break
+        actors.append(actor)
+        # Continue traversing content for more actors
+        content = content[content.find(start_string)+len(start_string):]
 
+    return actors[:max_actors]
 
 def directors(movie_name: str, max_directors: int = 10, content: str = None) -> List[str]:
     """Returns a list of all the directors listed
     by Rotten Tomatoes. Specify `max_directors` to only receive
     a certain number."""
     get_name = lambda x: x.split("/")[-1].replace("_", " ").title()
     if content is None:
```

### Comparing `rottentomatoes-python-0.5.17/rottentomatoes_python.egg-info/PKG-INFO` & `rottentomatoes-python-0.5.2/rottentomatoes_python.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rottentomatoes-python
-Version: 0.5.17
+Version: 0.5.2
 Summary: Scrape Rotten Tomatoes's website for basic information on movies, without the use of their hard-to-attain official REST API.
 Author: Prerit Das
 Author-email: <preritdas@gmail.com>
 Keywords: python,movies,rottentomatoes
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
@@ -13,24 +13,21 @@
 
 ![tests](https://github.com/preritdas/rottentomatoes-python/actions/workflows/pytest.yml/badge.svg)
 ![pypi](https://github.com/preritdas/rottentomatoes-python/actions/workflows/python-publish.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/rottentomatoes-python.svg)](https://badge.fury.io/py/rottentomatoes-python)
 ![versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)
 
 
-# :movie_camera: Rotten Tomatoes in Python (and API) :clapper:
+# Rotten Tomatoes in Python
 
 This package allows you to easily fetch Rotten Tomatoes scores and other movie data such as genres, without the use of the official Rotten Tomatoes API. The package scrapes their website for the data. I built this because unfortunately, to get access to their API, you have to submit a special request which takes an inordinate amount of time to process, or doesn't go through at all. 
 
 The package now, by default, scrapes the Rotten Tomatoes search page to find the true url of the first valid movie response (is a movie and has a tomatometer). This means queries that previously didn't work because their urls had a unique identifier or a year-released prefix, now work. The limitation of this new mechanism is that you only get the top response, and when searching for specific movies (sequels, by year, etc.) Rotten Tomatoes seems to return the same results as the original query. So, it's difficult to use specific queries to try and get the desired result movie as the top response. See #4 for more info on this.
 
-There is now an API deployed to make querying multiple movies and getting several responses easier. The endpoint is https://rotten-tomatoes-api.ue.r.appspot.com and it's open and free to use. Visit `/docs` or `/redoc` in the browser to view the endpoints. Both endpoints live right now are browser accessible meaning you don't need an HTTP client to use the API. 
-
-- https://rotten-tomatoes-api.ue.r.appspot.com/movie/bad_boys for JSON response of the top result
-- https://rotten-tomatoes-api.ue.r.appspot.com/search/bad_boys for a JSON response of all valid results
+There is now an API structure in place to make querying multiple movies and getting several responses easier. See the API section at the bottom for more.
 
 
 ## Usage
 
 You can either call the standalone functions `tomatometer`, `audience_score`, `genres`, etc., or use the `Movie` class to only pass the name and have each attribute be fetched automatically. If you use the `Movie` class, you can print all attributes by printing the object itself, or by accessing each attribute individually. 
 
 The weighted score is calculated using the formula $\frac{2}{3}(tomatometer) + \frac{1}{3}(audience)$. The result is then rounded to the nearest integer.
@@ -139,15 +136,15 @@
 Prominent actors: Tom Cruise, Miles Teller, Jennifer Connelly, Jon Hamm, Glen Powell.
 
 That took 0.3400420409961953 seconds.
 ```
 
 ## API
 
-The API is deployed at https://rotten-tomatoes-api.ue.r.appspot.com/. It has two endpoints currently, `/movie/{movie_name}` and `/search/{movie_name}`. The first will pull one movie, the top result. The second will pull a list of _all_ valid movie results.
+The API isn't deployed anywhere (for now) but you can run it locally. It has two endpoints, `/movie/{movie_name}` and `/search/{movie_name}`. The first will pull one movie, the top result. The second will pull a list of _all_ valid movie results.
 
 The first, with `movie_name="bad boys"`:
 
 ```json
 {
   "name": "Bad Boys for Life",
   "tomatometer": 76,
@@ -270,7 +267,11 @@
       "directors": [
         "Rick Rosenthal 2"
       ]
     }
   ]
 }
 ```
+
+When deployed you can do this in the browser too...
+
+`http(s)://localhostordeployment/movie/bad_boys` for JSON response of the top result, or `http(s)://localhostordeployment/search/bad_boys` for a JSON response of all valid results.
```

### Comparing `rottentomatoes-python-0.5.17/setup.py` & `rottentomatoes-python-0.5.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.5.17"
+VERSION = "0.5.2"
 DESCRIPTION = (
     "Scrape Rotten Tomatoes's website for basic information on movies, without the "
     "use of their hard-to-attain official REST API."
 )
 
 
 def read_me():
```

