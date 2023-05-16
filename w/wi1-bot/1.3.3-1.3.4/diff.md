# Comparing `tmp/wi1-bot-1.3.3.tar.gz` & `tmp/wi1-bot-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wi1-bot-1.3.3.tar", last modified: Fri Apr 28 06:44:47 2023, max compression
+gzip compressed data, was "wi1-bot-1.3.4.tar", last modified: Tue May 16 02:51:25 2023, max compression
```

## Comparing `wi1-bot-1.3.3.tar` & `wi1-bot-1.3.4.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.121776 wi1-bot-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.117776 wi1-bot-1.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.117776 wi1-bot-1.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-28 06:44:47.121776 wi1-bot-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/config.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 06:44:47.121776 wi1-bot-1.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.117776 wi1-bot-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/tests/movie_downloaded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.117776 wi1-bot-1.3.3/wi1_bot/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 06:44:46.000000 wi1-bot-1.3.3/wi1_bot/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.117776 wi1-bot-1.3.3/wi1_bot/arr/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/arr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/arr/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/arr/episode.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/arr/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/arr/radarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/arr/sonarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.121776 wi1-bot-1.3.3/wi1_bot/discord/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/discord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.121776 wi1-bot-1.3.3/wi1_bot/discord/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/discord/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/discord/cogs/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/discord/cogs/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/discord/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/push.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.121776 wi1-bot-1.3.3/wi1_bot/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/scripts/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/scripts/transcode_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.121776 wi1-bot-1.3.3/wi1_bot/transcoder/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/transcoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/transcoder/transcode_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/transcoder/transcoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-28 06:44:31.000000 wi1-bot-1.3.3/wi1_bot/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:44:47.117776 wi1-bot-1.3.3/wi1_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-28 06:44:46.000000 wi1-bot-1.3.3/wi1_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-28 06:44:47.000000 wi1-bot-1.3.3/wi1_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 06:44:46.000000 wi1-bot-1.3.3/wi1_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 06:44:46.000000 wi1-bot-1.3.3/wi1_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-28 06:44:46.000000 wi1-bot-1.3.3/wi1_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 06:44:47.000000 wi1-bot-1.3.3/wi1_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.018636 wi1-bot-1.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.018636 wi1-bot-1.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/config.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.018636 wi1-bot-1.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/tests/movie_downloaded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.018636 wi1-bot-1.3.4/wi1_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 02:51:23.000000 wi1-bot-1.3.4/wi1_bot/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/wi1_bot/arr/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/arr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/arr/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/arr/episode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/arr/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/arr/radarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/arr/sonarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/wi1_bot/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/discord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/wi1_bot/discord/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/discord/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/discord/cogs/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/discord/cogs/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/discord/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/push.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/wi1_bot/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/scripts/add_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/scripts/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/scripts/transcode_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.022636 wi1-bot-1.3.4/wi1_bot/transcoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/transcoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/transcoder/transcode_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/transcoder/transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-16 02:51:04.000000 wi1-bot-1.3.4/wi1_bot/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:51:25.018636 wi1-bot-1.3.4/wi1_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-16 02:51:24.000000 wi1-bot-1.3.4/wi1_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-16 02:51:25.000000 wi1-bot-1.3.4/wi1_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 02:51:24.000000 wi1-bot-1.3.4/wi1_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-16 02:51:24.000000 wi1-bot-1.3.4/wi1_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-16 02:51:24.000000 wi1-bot-1.3.4/wi1_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 02:51:24.000000 wi1-bot-1.3.4/wi1_bot.egg-info/top_level.txt
```

### Comparing `wi1-bot-1.3.3/.github/workflows/pypi-publish.yml` & `wi1-bot-1.3.4/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/.pre-commit-config.yaml` & `wi1-bot-1.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/LICENSE` & `wi1-bot-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/PKG-INFO` & `wi1-bot-1.3.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.3.3
+Version: 1.3.4
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
         
@@ -53,22 +53,38 @@
 3. `pip install -e .[dev]`
 4. `pre-commit install`
 
 Requires Python >=3.10.
 
 ### TODO
 
-- Use Discord slash commands instead of normal text commands (difficult: can't have "conversation" with slash commands)
-- Web dashboard for seeing transcode queue, transcode progress, quotas
+- have config.discord.users be a dict with 'quotas' and 'name' for *arr tags
+- Better pushover notifications
+  - Failures for pretty much everything
+  - Notifications for grabs/downloads of personal watchlist
+- Tag user who added movie when it's downloaded
+  - Would replace Radarr/Sonarr's Discord webhooks
+  - !notify \<query\> to also be tagged when a movie/show someone else added is downloaded
+    - react to "added movie/show" instead of having to !notify
+    - react to notification to stop notifications
+    - if user tries to add movie that's already present, add them to list to notify
+    - Would require a DB; don't use tags as those are to strictly track quotas
+      - DB is useful for caching other information as well
+- Use Discord slash commands instead of normal text commands
+  - This is difficult/impossible currently, can't have "conversation" with slash commands
 - Enforce quotas
+- Testing
+  - docker(-compose) for spinning up Sonarr and Radarr instances to test API interactions
+- Web dashboard for seeing transcode queue, transcode progress, quotas
 - !linktmdb
-    - !rate / !ratings (https://developers.themoviedb.org/3/movies/rate-movie)
-    - !movierec based off of ratings and similar-to-user ratings?
-        - https://towardsdatascience.com/the-4-recommendation-engines-that-can-predict-your-movie-tastes-109dc4e10c52
-        - or just use TMDB's API to get recommendations (if that's possible?)
+  - !rate / !ratings (https://developers.themoviedb.org/3/movies/rate-movie)
+  - !movierec based off of ratings and similar-to-user ratings?
+    - https://towardsdatascience.com/the-4-recommendation-engines-that-can-predict-your-movie-tastes-109dc4e10c52
+    - or just use TMDB's API to get recommendations (if that's possible?)
 - !movieinfo showing user/public ratings and other general info (runtime, cast, director)
-    - Use TMDB API to get movie metadata
-    - If movie isn't on Radarr, react to message to add it?
-    - Tautulli API (get_history) to show who has already seen the movie
+  - use TMDB API to get movie metadata
+  - if movie isn't on Radarr, react to message to add it?
+  - Tautulli API (get_history) to show who has already seen the movie
 - User leaderboard
+  - movies/shows added, Tautulli watch counts
```

### Comparing `wi1-bot-1.3.3/README.md` & `wi1-bot-1.3.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -15,20 +15,36 @@
 3. `pip install -e .[dev]`
 4. `pre-commit install`
 
 Requires Python >=3.10.
 
 ### TODO
 
-- Use Discord slash commands instead of normal text commands (difficult: can't have "conversation" with slash commands)
-- Web dashboard for seeing transcode queue, transcode progress, quotas
+- have config.discord.users be a dict with 'quotas' and 'name' for *arr tags
+- Better pushover notifications
+  - Failures for pretty much everything
+  - Notifications for grabs/downloads of personal watchlist
+- Tag user who added movie when it's downloaded
+  - Would replace Radarr/Sonarr's Discord webhooks
+  - !notify \<query\> to also be tagged when a movie/show someone else added is downloaded
+    - react to "added movie/show" instead of having to !notify
+    - react to notification to stop notifications
+    - if user tries to add movie that's already present, add them to list to notify
+    - Would require a DB; don't use tags as those are to strictly track quotas
+      - DB is useful for caching other information as well
+- Use Discord slash commands instead of normal text commands
+  - This is difficult/impossible currently, can't have "conversation" with slash commands
 - Enforce quotas
+- Testing
+  - docker(-compose) for spinning up Sonarr and Radarr instances to test API interactions
+- Web dashboard for seeing transcode queue, transcode progress, quotas
 - !linktmdb
-    - !rate / !ratings (https://developers.themoviedb.org/3/movies/rate-movie)
-    - !movierec based off of ratings and similar-to-user ratings?
-        - https://towardsdatascience.com/the-4-recommendation-engines-that-can-predict-your-movie-tastes-109dc4e10c52
-        - or just use TMDB's API to get recommendations (if that's possible?)
+  - !rate / !ratings (https://developers.themoviedb.org/3/movies/rate-movie)
+  - !movierec based off of ratings and similar-to-user ratings?
+    - https://towardsdatascience.com/the-4-recommendation-engines-that-can-predict-your-movie-tastes-109dc4e10c52
+    - or just use TMDB's API to get recommendations (if that's possible?)
 - !movieinfo showing user/public ratings and other general info (runtime, cast, director)
-    - Use TMDB API to get movie metadata
-    - If movie isn't on Radarr, react to message to add it?
-    - Tautulli API (get_history) to show who has already seen the movie
+  - use TMDB API to get movie metadata
+  - if movie isn't on Radarr, react to message to add it?
+  - Tautulli API (get_history) to show who has already seen the movie
 - User leaderboard
+  - movies/shows added, Tautulli watch counts
```

### Comparing `wi1-bot-1.3.3/config.yaml.template` & `wi1-bot-1.3.4/config.yaml.template`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/pyproject.toml` & `wi1-bot-1.3.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10"
 ]
 dynamic = ["version"]
 requires-python = ">=3.10"
 dependencies = [
     "discord.py==2.2.2",
-    "Flask==2.2.3",
+    "Flask==2.2.5",
     "mongoengine==0.27.0",
     "pyarr==3.1.3",
     "PyYAML==6.0",
     "requests==2.28.2"
 ]
 
 [project.optional-dependencies]
@@ -37,14 +37,15 @@
 
 [project.urls]
 Homepage = "https://github.com/wthueb/wi1-bot"
 
 [project.scripts]
 wi1-bot = "wi1_bot.scripts.start:main"
 transcode-item = "wi1_bot.scripts.transcode_item:main"
+add-tag = "wi1_bot.scripts.add_tag:main"
 
 [tool.setuptools]
 packages = ["wi1_bot"]
 
 [tool.setuptools_scm]
 write_to = "wi1_bot/_version.py"
```

### Comparing `wi1-bot-1.3.3/wi1_bot/arr/download.py` & `wi1-bot-1.3.4/wi1_bot/arr/download.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot/arr/episode.py` & `wi1-bot-1.3.4/wi1_bot/arr/episode.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot/arr/movie.py` & `wi1-bot-1.3.4/wi1_bot/arr/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot/arr/radarr.py` & `wi1-bot-1.3.4/wi1_bot/arr/radarr.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot/arr/sonarr.py` & `wi1-bot-1.3.4/wi1_bot/arr/sonarr.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot/config.py` & `wi1-bot-1.3.4/wi1_bot/config.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot/discord/bot.py` & `wi1-bot-1.3.4/wi1_bot/discord/bot.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot/discord/cogs/movie.py` & `wi1-bot-1.3.4/wi1_bot/discord/cogs/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot/discord/cogs/series.py` & `wi1-bot-1.3.4/wi1_bot/discord/cogs/series.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot/discord/helpers.py` & `wi1-bot-1.3.4/wi1_bot/discord/helpers.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot/push.py` & `wi1-bot-1.3.4/wi1_bot/push.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot/scripts/start.py` & `wi1-bot-1.3.4/wi1_bot/scripts/start.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot/scripts/transcode_item.py` & `wi1-bot-1.3.4/wi1_bot/scripts/transcode_item.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot/transcoder/transcode_queue.py` & `wi1-bot-1.3.4/wi1_bot/transcoder/transcode_queue.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot/transcoder/transcoder.py` & `wi1-bot-1.3.4/wi1_bot/transcoder/transcoder.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot/webhook.py` & `wi1-bot-1.3.4/wi1_bot/webhook.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.3/wi1_bot.egg-info/PKG-INFO` & `wi1-bot-1.3.4/wi1_bot.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.3.3
+Version: 1.3.4
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
         
@@ -53,22 +53,38 @@
 3. `pip install -e .[dev]`
 4. `pre-commit install`
 
 Requires Python >=3.10.
 
 ### TODO
 
-- Use Discord slash commands instead of normal text commands (difficult: can't have "conversation" with slash commands)
-- Web dashboard for seeing transcode queue, transcode progress, quotas
+- have config.discord.users be a dict with 'quotas' and 'name' for *arr tags
+- Better pushover notifications
+  - Failures for pretty much everything
+  - Notifications for grabs/downloads of personal watchlist
+- Tag user who added movie when it's downloaded
+  - Would replace Radarr/Sonarr's Discord webhooks
+  - !notify \<query\> to also be tagged when a movie/show someone else added is downloaded
+    - react to "added movie/show" instead of having to !notify
+    - react to notification to stop notifications
+    - if user tries to add movie that's already present, add them to list to notify
+    - Would require a DB; don't use tags as those are to strictly track quotas
+      - DB is useful for caching other information as well
+- Use Discord slash commands instead of normal text commands
+  - This is difficult/impossible currently, can't have "conversation" with slash commands
 - Enforce quotas
+- Testing
+  - docker(-compose) for spinning up Sonarr and Radarr instances to test API interactions
+- Web dashboard for seeing transcode queue, transcode progress, quotas
 - !linktmdb
-    - !rate / !ratings (https://developers.themoviedb.org/3/movies/rate-movie)
-    - !movierec based off of ratings and similar-to-user ratings?
-        - https://towardsdatascience.com/the-4-recommendation-engines-that-can-predict-your-movie-tastes-109dc4e10c52
-        - or just use TMDB's API to get recommendations (if that's possible?)
+  - !rate / !ratings (https://developers.themoviedb.org/3/movies/rate-movie)
+  - !movierec based off of ratings and similar-to-user ratings?
+    - https://towardsdatascience.com/the-4-recommendation-engines-that-can-predict-your-movie-tastes-109dc4e10c52
+    - or just use TMDB's API to get recommendations (if that's possible?)
 - !movieinfo showing user/public ratings and other general info (runtime, cast, director)
-    - Use TMDB API to get movie metadata
-    - If movie isn't on Radarr, react to message to add it?
-    - Tautulli API (get_history) to show who has already seen the movie
+  - use TMDB API to get movie metadata
+  - if movie isn't on Radarr, react to message to add it?
+  - Tautulli API (get_history) to show who has already seen the movie
 - User leaderboard
+  - movies/shows added, Tautulli watch counts
```

### Comparing `wi1-bot-1.3.3/wi1_bot.egg-info/SOURCES.txt` & `wi1-bot-1.3.4/wi1_bot.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -28,12 +28,13 @@
 wi1_bot/discord/__init__.py
 wi1_bot/discord/bot.py
 wi1_bot/discord/helpers.py
 wi1_bot/discord/cogs/__init__.py
 wi1_bot/discord/cogs/movie.py
 wi1_bot/discord/cogs/series.py
 wi1_bot/scripts/__init__.py
+wi1_bot/scripts/add_tag.py
 wi1_bot/scripts/start.py
 wi1_bot/scripts/transcode_item.py
 wi1_bot/transcoder/__init__.py
 wi1_bot/transcoder/transcode_queue.py
 wi1_bot/transcoder/transcoder.py
```

