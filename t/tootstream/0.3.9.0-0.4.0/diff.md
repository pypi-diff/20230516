# Comparing `tmp/tootstream-0.3.9.0.tar.gz` & `tmp/tootstream-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tootstream-0.3.9.0.tar", last modified: Sun Feb 26 15:02:15 2023, max compression
+gzip compressed data, was "tootstream-0.4.0.tar", last modified: Tue May 16 12:42:13 2023, max compression
```

## Comparing `tootstream-0.3.9.0.tar` & `tootstream-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 craig     (1000) craig     (1000)        0 2023-02-26 15:02:15.291741 tootstream-0.3.9.0/
--rw-rw-r--   0 craig     (1000) craig     (1000)     5313 2023-02-26 14:59:45.000000 tootstream-0.3.9.0/CHANGELOG.md
--rw-rw-r--   0 craig     (1000) craig     (1000)     1592 2017-10-09 14:09:03.000000 tootstream-0.3.9.0/CONTRIBUTING.md
--rw-rw-r--   0 craig     (1000) craig     (1000)     1068 2017-10-09 14:09:03.000000 tootstream-0.3.9.0/LICENSE.md
--rw-rw-r--   0 craig     (1000) craig     (1000)       41 2017-10-09 14:09:03.000000 tootstream-0.3.9.0/MANIFEST.in
--rw-rw-r--   0 craig     (1000) craig     (1000)      425 2023-02-26 15:02:15.291741 tootstream-0.3.9.0/PKG-INFO
--rw-rw-r--   0 craig     (1000) craig     (1000)     3906 2018-05-31 00:06:11.000000 tootstream-0.3.9.0/README.md
--rw-rw-r--   0 craig     (1000) craig     (1000)       75 2023-02-26 14:54:44.000000 tootstream-0.3.9.0/requirements.txt
--rw-rw-r--   0 craig     (1000) craig     (1000)       38 2023-02-26 15:02:15.291741 tootstream-0.3.9.0/setup.cfg
--rw-rw-r--   0 craig     (1000) craig     (1000)      823 2023-02-26 14:54:44.000000 tootstream-0.3.9.0/setup.py
-drwxrwxr-x   0 craig     (1000) craig     (1000)        0 2023-02-26 15:02:15.267741 tootstream-0.3.9.0/src/
-drwxrwxr-x   0 craig     (1000) craig     (1000)        0 2023-02-26 15:02:15.291741 tootstream-0.3.9.0/src/tootstream/
--rw-rw-r--   0 craig     (1000) craig     (1000)        0 2017-10-09 14:09:03.000000 tootstream-0.3.9.0/src/tootstream/__init__.py
--rw-rw-r--   0 craig     (1000) craig     (1000)     2105 2022-12-27 03:35:48.000000 tootstream-0.3.9.0/src/tootstream/config.py
--rw-rw-r--   0 craig     (1000) craig     (1000)    66421 2023-02-26 14:54:44.000000 tootstream-0.3.9.0/src/tootstream/toot.py
--rw-rw-r--   0 craig     (1000) craig     (1000)     9505 2023-02-26 14:54:44.000000 tootstream-0.3.9.0/src/tootstream/toot_parser.py
-drwxrwxr-x   0 craig     (1000) craig     (1000)        0 2023-02-26 15:02:15.291741 tootstream-0.3.9.0/src/tootstream.egg-info/
--rw-rw-r--   0 craig     (1000) craig     (1000)      425 2023-02-26 15:02:14.000000 tootstream-0.3.9.0/src/tootstream.egg-info/PKG-INFO
--rw-rw-r--   0 craig     (1000) craig     (1000)      422 2023-02-26 15:02:15.000000 tootstream-0.3.9.0/src/tootstream.egg-info/SOURCES.txt
--rw-rw-r--   0 craig     (1000) craig     (1000)        1 2023-02-26 15:02:14.000000 tootstream-0.3.9.0/src/tootstream.egg-info/dependency_links.txt
--rw-rw-r--   0 craig     (1000) craig     (1000)       52 2023-02-26 15:02:14.000000 tootstream-0.3.9.0/src/tootstream.egg-info/entry_points.txt
--rw-rw-r--   0 craig     (1000) craig     (1000)       75 2023-02-26 15:02:14.000000 tootstream-0.3.9.0/src/tootstream.egg-info/requires.txt
--rw-rw-r--   0 craig     (1000) craig     (1000)       11 2023-02-26 15:02:15.000000 tootstream-0.3.9.0/src/tootstream.egg-info/top_level.txt
+drwxrwxr-x   0 craig     (1000) craig     (1000)        0 2023-05-16 12:42:13.562994 tootstream-0.4.0/
+-rw-rw-r--   0 craig     (1000) craig     (1000)     6833 2023-05-16 12:39:49.000000 tootstream-0.4.0/CHANGELOG.md
+-rw-rw-r--   0 craig     (1000) craig     (1000)     1592 2017-10-09 14:09:03.000000 tootstream-0.4.0/CONTRIBUTING.md
+-rw-rw-r--   0 craig     (1000) craig     (1000)     1068 2017-10-09 14:09:03.000000 tootstream-0.4.0/LICENSE.md
+-rw-rw-r--   0 craig     (1000) craig     (1000)       41 2017-10-09 14:09:03.000000 tootstream-0.4.0/MANIFEST.in
+-rw-rw-r--   0 craig     (1000) craig     (1000)      423 2023-05-16 12:42:13.562994 tootstream-0.4.0/PKG-INFO
+-rw-rw-r--   0 craig     (1000) craig     (1000)     3906 2018-05-31 00:06:11.000000 tootstream-0.4.0/README.md
+-rw-rw-r--   0 craig     (1000) craig     (1000)       87 2023-05-16 12:39:39.000000 tootstream-0.4.0/requirements.txt
+-rw-rw-r--   0 craig     (1000) craig     (1000)       38 2023-05-16 12:42:13.562994 tootstream-0.4.0/setup.cfg
+-rw-rw-r--   0 craig     (1000) craig     (1000)      821 2023-05-16 12:39:39.000000 tootstream-0.4.0/setup.py
+drwxrwxr-x   0 craig     (1000) craig     (1000)        0 2023-05-16 12:42:13.550994 tootstream-0.4.0/src/
+drwxrwxr-x   0 craig     (1000) craig     (1000)        0 2023-05-16 12:42:13.562994 tootstream-0.4.0/src/tootstream/
+-rw-rw-r--   0 craig     (1000) craig     (1000)        0 2017-10-09 14:09:03.000000 tootstream-0.4.0/src/tootstream/__init__.py
+-rw-rw-r--   0 craig     (1000) craig     (1000)     2190 2023-05-06 15:04:07.000000 tootstream-0.4.0/src/tootstream/config.py
+-rw-rw-r--   0 craig     (1000) craig     (1000)    76501 2023-05-16 12:39:39.000000 tootstream-0.4.0/src/tootstream/toot.py
+-rw-rw-r--   0 craig     (1000) craig     (1000)     9505 2023-02-26 14:54:44.000000 tootstream-0.4.0/src/tootstream/toot_parser.py
+drwxrwxr-x   0 craig     (1000) craig     (1000)        0 2023-05-16 12:42:13.562994 tootstream-0.4.0/src/tootstream.egg-info/
+-rw-rw-r--   0 craig     (1000) craig     (1000)      423 2023-05-16 12:42:12.000000 tootstream-0.4.0/src/tootstream.egg-info/PKG-INFO
+-rw-rw-r--   0 craig     (1000) craig     (1000)      422 2023-05-16 12:42:13.000000 tootstream-0.4.0/src/tootstream.egg-info/SOURCES.txt
+-rw-rw-r--   0 craig     (1000) craig     (1000)        1 2023-05-16 12:42:12.000000 tootstream-0.4.0/src/tootstream.egg-info/dependency_links.txt
+-rw-rw-r--   0 craig     (1000) craig     (1000)       52 2023-05-16 12:42:13.000000 tootstream-0.4.0/src/tootstream.egg-info/entry_points.txt
+-rw-rw-r--   0 craig     (1000) craig     (1000)       87 2023-05-16 12:42:13.000000 tootstream-0.4.0/src/tootstream.egg-info/requires.txt
+-rw-rw-r--   0 craig     (1000) craig     (1000)       11 2023-05-16 12:42:13.000000 tootstream-0.4.0/src/tootstream.egg-info/top_level.txt
```

### Comparing `tootstream-0.3.9.0/CHANGELOG.md` & `tootstream-0.4.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,166 +1,204 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
-### Release
-### [0.3.9.0] - 2023-02-26
+## Released
 
-#### Fixed
+## [0.4.0] - 2023-05-16
+
+### Fixed
+- Toots with content warnings will not automatically display. Use the `show` command to display the contents.
+- Updating colors to be more consistent / better contrast.
+- Display no-content, image-only toots.
+- Use search with limit 1 when we only want one account, bypassing Mastodon's questionable search algorithm.
+- `view` command doesn't bring back a list of users that are close to what you were searching for.
+- edits no longer break `note` command.
+- Commands using `step` now find the original toot for a reblogged toot.
+
+### Added
+- Filter support (list filters, toots with filters honor the filter settings).
+- `show` command, which shows the contents of a toot.
+- `next` and `prev` commands for pagination of the current timeline context.
+- `mute` now has time duration (30s, 1d, etc.).
+- `view` command now shows which user you are viewing and allows pagination.
+- `vote` command for voting in polls.
+- `user` command for showing a user profile.
+- Displays poll results, whether the poll is expired, and if the poll supports multiple votes (along with a URI).
+- Update the current prompt with the current context.
+- Added `mentions` command to just show mentions.
+- Added poll and update filters to `note` command.
+- Changed command to abort step from "a" to "q" to maintain consistency.
+- Allow favoriting / unfavoriting multiple toots at once.
+- `showthread` will show all toots in a thread with content warnings / filters removed.
+- Added `follow_request` to note; added `-r` to filter requests.
+
+## Release
+
+## [0.3.9.0] - 2023-02-26
+
+### Fixed
 - Remove duplicate code (thanks to Jesse Weinstein)
 - Upgrade to Mastodon.py version to Mastodon.py 1.8.0
 
-#### Added
+### Added
 - Added support for bookmarks (thanks to Jessee Weinstein)
 
-### Release
-### [0.3.8.1] - 2020-01-22
+## Release
 
-#### Fixed
+## [0.3.8.1] - 2020-01-22
+
+### Fixed
 - Upgrade to Mastodon.py 1.5.0
 - PEP8 code formatting
 
-### Release
-### [0.3.7] - 2019-07-20
+## Release
 
-#### Fixed
+## [0.3.7] - 2019-07-20
+
+### Fixed
 - Upgrade to Mastodon.py 1.4.5
 - Rudimentary support for polls (shows links to polls)
 - Update colored minimum version to 1.3.93 (Fixes GPL license incompatibility)
 - Support Pleroma FlakeIDs
 - Minor fix for stream command being closed without receiving a toot getting a Nonetype for handle
 
-### Release
-### [0.3.6] - 2018-09-29
+## Release
 
-#### Added
+## [0.3.6] - 2018-09-29
+
+### Added
 - Updated to Mastodon.py 1.3.1 (No additional features yet)
 - Added links command to show links in a toot and optionally open them in a browser
 - Added puburl command to show the public URL of a toot
 
-#### Fixed
+### Fixed
 - Upgrade to Mastodon.py 1.3.1 fixes searching for users issue noted in 0.3.5
 - Spelling mistakes 
 - Added better error message for streaming support not supported on older mastodon instances
 
-### Release
-### [0.3.5] - 2018-08-08
+## Release
+
+## [0.3.5] - 2018-08-08
 
-#### Added
+### Added
 - Updated to Mastodon.py 1.3 (no additional features yet)
 
-#### Fixed
+### Fixed
 - List renames did not work
 
 
-### Release
-### [0.3.4] - 2018-05-30
+## Release
+
+## [0.3.4] - 2018-05-30
 
-#### Added
+### Added
 - Added ability to execute commands while streaming (toot, fav, rep, etc.)
 - Added step switch for stepping through the timelines (ex: home step, listhome step)
 - Execute commands on stepped toots (fav, boost, rep, etc.)
 - Added ability to show links and optionally open those links in a browser (see "help links" for details).
 - Display media links by default
 - Display message when no notifications are present
 
-#### Fixed
+### Fixed
 - Privacy settings now default to server privacy settings for toots
 - CTRL-C in streaming adds a linefeed to preserve prompt spacing
 - Streaming now supports lists with spaces
 - Added broad exception handling so tootstream shouldn't crash while running commands.
 - Minor formatting fixes
 
-### Release
-### [0.3.3] - 2018-02-17
+## Release
 
-#### Added
+## [0.3.3] - 2018-02-17
+
+### Added
 - List support for servers that support it. (See ``help list`` for more details.)
 - Bumped to Mastodon.py 1.2.2
 
-#### Added (awaiting proper config)
+### Added (awaiting proper config)
 ( The following items are active but require a re-working of the configuration file to make active. Currently they are flags inside the ``toot_parser.py`` file. Intrepid explorers may find them.)
 - Added emoji shortcode (defaults to "off").
 - Added emoji "demoji" to show shortcodes for emoji (defaults to off).
 
-#### Fixed
+### Fixed
 - Fixed boosting private toots
 - Fixed message for boosting toots
 - Fixed leading / trailing whitespace from media filepath
 - Added better exception handling around streaming API
 
-####
+###
+
+## Release
 
-### Release
-### [0.3.2] - 2017-12-23
+## [0.3.2] - 2017-12-23
 
-#### Added
+### Added
 - Reworked the Tootstream Parser to add styling, link-shortening, link retrieval, and emoji code shortening
 - About shows current version of Tootstream and the connected instance
 - Notifications may now be filtered
 
-#### Fixed
+### Fixed
 - Replies no longer include the logged-in user
 - Allow user to edit a toot when an API error occurs
 - Compatibility with Mastodon.py 1.2.1
 
-### Release
-### [0.3.1] - 2017-11-21
+## Release
+## [0.3.1] - 2017-11-21
 
-#### Fixed
+### Fixed
 - Compatibility with Mastodon 1.1.2 fix
 
-### Release
-### [0.3.0] - 2017-11-17
-### Dedicated to the memory of Natalie Nguyen (aka Tipsy Tentacle). May she live on in our hearts and our changelog.
-#### Added
+## Release
+## [0.3.0] - 2017-11-17
+## Dedicated to the memory of Natalie Nguyen (aka Tipsy Tentacle). May she live on in our hearts and our changelog.
+### Added
 - Upload media via a toot and set visibility
 - Set content warnings on a toot
 - Set visibility of a toot (public, unlisted, private, direct)
 - Thread and history commands for viewing a toot's thread
 - "Humanized" time formats for toots (how long ago did this occur from now?)
 - Clear out notifications / dismiss individual notifications
 
-##### Changed
+#### Changed
 - Help is split into sections (Help, Toots, Timeline, Users, Discover, and Profile)
 - Can type "help section" to see the help for that section
 
-##### Fixed
+#### Fixed
 - Changed the glyphs so they are encoded
 - Python 3 requirement is now explicit
 
-### Release
-### [0.2.0] - 2017-10-17
-#### Added
+## Release
+## [0.2.0] - 2017-10-17
+### Added
 - Command auto-complete
 - Nickname autocomplete for local and federated users
 - View command: view the latest toots from a user
 - Search function
 - Followers / Following list
 - Block / Unblock function
 - Mute / Unmute function
 - Follow requests (accept / reject)
 - Bring up the default editor when no text is added for toot and rep commands
 - Added --profile command line option
 - Proper Python Packaging
 
-#### Changed
+### Changed
 - Using Mastodon.py 1.1.0
 - ``get_userid`` check API results list for exact match to user input
 - Many formatting changes (now using glyphs and content warning, timestamps on metions)
 - Refactored login and user prompts
 - Simplified the requirements to only include requirements for tootstream
 
-#### Fixed
+### Fixed
 - Favorite / Boost/ Reply won't crash without ID
 - Local timeline actually shows local timeline
 - Accept / Reject Status fixed.
 - Configuration file more resilient
 - Empty toots could crash the program with later Mastodon.py
 
-### Release
-### [0.1.0] - 2017-05-02
-#### Added
+## Release
+## [0.1.0] - 2017-05-02
+### Added
 - Contribution guide
 - License
```

### Comparing `tootstream-0.3.9.0/CONTRIBUTING.md` & `tootstream-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tootstream-0.3.9.0/LICENSE.md` & `tootstream-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tootstream-0.3.9.0/README.md` & `tootstream-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tootstream-0.3.9.0/setup.py` & `tootstream-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name="tootstream",
-    version="0.3.9.0",
+    version="0.4.0",
     python_requires=">=3",
     install_requires=[line.strip() for line in open('requirements.txt')],
 
     packages=find_packages('src'),
     package_dir={'': 'src'}, include_package_data=True,
     package_data={
     },
```

### Comparing `tootstream-0.3.9.0/src/tootstream/config.py` & `tootstream-0.4.0/src/tootstream/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sys
 import os.path
 import configparser
 from colored import fg, bg, attr, stylize
 
+
 def cprint(text, style, end="\n"):
     print(stylize(text, style), end=end)
 
 
 class Config:
-
     def __init__(self, filename):
         self.filename = filename
         self.config = None
 
     def parse_config(self):
         """
         Reads configuration from the specified file.
@@ -20,23 +20,28 @@
         data from the file.  If the file does not exist,
         returns an empty ConfigParser object.
 
         Exits the program with error if the specified file
         cannot be parsed to prevent damaging unknown files.
         """
         if not os.path.isfile(self.filename):
-            cprint("...No configuration found, generating...", fg('cyan'))
+            cprint("...No configuration found, generating...", fg("cyan"))
             self.config = configparser.ConfigParser()
             return self.config
 
         self.config = configparser.ConfigParser()
         try:
             self.config.read(self.filename)
         except configparser.Error:
-            cprint("This does not look like a valid configuration: {}".format(self.filename), fg('red'))
+            cprint(
+                "This does not look like a valid configuration: {}".format(
+                    self.filename
+                ),
+                fg("red"),
+            )
             sys.exit(1)
 
         return self.config
 
 
 def save_config(self):
     """
@@ -52,15 +57,15 @@
         os.makedirs(dirpath)
 
     # create as user-rw-only if possible
     if not os.path.exists(self.filename):
         try:
             os.open(self.filename, flags=os.O_CREAT | os.O_APPEND, mode=0o600)
         except Exception as e:
-            cprint("Unable to create file {}: {}".format(self.filename, e), fg('red'))
+            cprint("Unable to create file {}: {}".format(self.filename, e), fg("red"))
 
     try:
-        with open(self.filename, 'w') as configfile:
+        with open(self.filename, "w") as configfile:
             self.config.write(configfile)
     except os.error:
-        cprint("Unable to write configuration to {}".format(self.filename), fg('red'))
+        cprint("Unable to write configuration to {}".format(self.filename), fg("red"))
     return
```

### Comparing `tootstream-0.3.9.0/src/tootstream/toot.py` & `tootstream-0.4.0/src/tootstream/toot.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 import configparser
 import random
 import readline
 import bisect
 import shutil
 from collections import OrderedDict
 import webbrowser
+import dateutil
 
 # Get the version of Tootstream
 import pkg_resources  # part of setuptools
 import click
-import dateutil
 from tootstream.toot_parser import TootParser
 from mastodon import Mastodon, StreamListener
 from colored import fg, bg, attr, stylize
 import humanize
 import emoji
+import pytimeparse
 
 
 version = pkg_resources.require("tootstream")[0].version
 
 # placeholder variable for converting emoji to shortcodes until we get it in config
 convert_emoji_to_shortcode = False
 
@@ -57,14 +58,15 @@
     "followed_by": "\U0001f43e",  # pawprints '\U0001f43e'
     "following": "\U0001f463",  # footprints '\U0001f463'
     # thumbsdown '\U0001f44e', big X '\U0000274c', stopsign '\U0001f6d1'
     "blocking": "\U0000274c",
     # mute-spkr '\U0001f507', mute-bell '\U0001f515', prohibited '\U0001f6ab'
     "muting": "\U0001f6ab",
     "requested": "\U00002753",  # hourglass '\U0000231b', question '\U00002753'
+    "voted": "\U00002714",  # Checkmark
     # catchall
     "unknown": "\U0001f34d",
 }
 
 # reserved config sections (disallowed as profile names)
 RESERVED = ("theme", "global")
 
@@ -112,14 +114,17 @@
         printToot(status)
         print()
         redisplay_prompt()
 
 
 IDS = IdDict()
 
+LAST_PAGE = None
+LAST_CONTEXT = None
+
 # Get the current width of the terminal
 terminal_size = shutil.get_terminal_size((80, 20))
 toot_parser = TootParser(
     indent="  ",
     width=int(terminal_size.columns) - 2,
     convert_emoji_to_unicode=False,
     convert_emoji_to_shortcode=convert_emoji_to_shortcode,
@@ -129,14 +134,40 @@
 
 
 #####################################
 ######## UTILITY FUNCTIONS   ########
 #####################################
 
 
+def find_original_toot_id(toot):
+    """ Locates the original toot ID in case of a reblog"""
+    reblog = toot.get("reblog")
+    if reblog:
+        original_toot = reblog
+    else:
+        original_toot = toot
+    original_toot_id = original_toot.get("id")
+    return IDS.to_local(original_toot_id)
+
+
+def rest_to_list(rest):
+    rest = (",".join(rest.split()))
+    rest = rest.replace(",,", ",")
+    rest = [x.strip() for x in rest.split(",")]
+    return rest
+
+
+def update_prompt(username, context, profile):
+    if context:
+        prompt = f"[@{username} <{context}> ({profile})]: "
+    else:
+        prompt = f"[@{username} ({profile})]: "
+    return prompt
+
+
 def list_support(mastodon, silent=False):
     lists_available = mastodon.verify_minimum_version("2.1.0")
     if lists_available is False and silent is False:
         cprint("List support is not available with this version of Mastodon", fg("red"))
     return lists_available
 
 
@@ -144,73 +175,94 @@
     if "step" in rest:
         return True, rest.replace(" step", "")
     else:
         return False, rest
 
 
 def get_content(toot):
-    html = toot["content"]
+    html = toot.get("content")
+    if html is None:
+        return ""
     toot_parser.parse(html)
     return toot_parser.get_text()
 
 
+def get_media_attachments(toot):
+    out = []
+    nsfw = "CW " if toot.get("sensitive") else ""
+    out.append(
+        stylize(
+            "  " + nsfw + "media: " + str(len(toot.get("media_attachments"))),
+            fg("magenta"),
+        )
+    )
+    if show_media_links:
+        for media in toot.get("media_attachments"):
+            out.append(stylize("   " + nsfw + " " + media.url, fg("green")))
+    return out
+
+
 def get_poll(toot):
     poll = getattr(toot, "poll", None)
     if poll:
+        poll_results = ""
+        total_votes_count = poll.get("votes_count")
+        poll_options = poll.get("options")
+        own_votes = poll.get("own_votes")
+        for i, poll_element in enumerate(poll_options):
+            selected = " "
+            poll_title = poll_element.get("title")
+            poll_votes_count = poll_element.get("votes_count")
+            if total_votes_count > 0:
+                poll_percentage = (poll_votes_count / total_votes_count) * 100
+            else:
+                poll_percentage = 0
+            if i in own_votes:
+                selected = GLYPHS.get("voted")
+            poll_results += (
+                f"{selected} {i}: {poll_title} ({poll_votes_count}: {poll_percentage:.2f}%)\n"
+            )
+        poll_results += f"  Total votes: {total_votes_count}"
+        if poll.multiple:
+            poll_results += f"\n  (Multiple votes may be cast.)"
+        if poll.expired:
+            poll_results += f"\n  Polling is over."
         uri = toot["uri"]
-        return "  [poll]: {}".format(uri)
+        return f"  [poll] {poll['id']} ({uri})\n{poll_results}"
 
 
-def get_userid(mastodon, rest):
-    # we got some user input.  we need a userid (int).
-    # returns userid as int, -1 on error, or list of users if ambiguous.
-    if not rest:
-        return -1
+def get_unique_userid(mastodon, rest, exact=True):
+    """Get a unique user ID by limiting the search to the top result.
+    params:
+        rest: rest of the command
+        exact: whether to do an exact search or not.
+            Most commands should require precision, so
 
-    # maybe it's already an int
+    """
+    # Check if the ID is already in numeric form
     try:
-        return int(rest)
+        userid = int(rest)
+        return userid
     except ValueError:
         pass
 
-    # not an int
-    users = mastodon.account_search(rest)
-    if not users:
-        return -1
-    elif len(users) > 1:
-        # Mastodon's search is fuzzier than we want; check for exact match
-
-        query = rest[1:] if rest.startswith("@") else rest
-        (quser, _, qinstance) = query.partition("@")
-        localinstance = mastodon.instance()
-
-        # on uptodate servers, exact match should be first in list
-        for user in users:
-            # match user@remoteinstance, localuser
-            if query == user["acct"]:
-                return user["id"]
-            # match user@localinstance
-            elif quser == user["acct"] and qinstance == localinstance["uri"]:
-                return user["id"]
-
-        # no exact match; return list
-        return users
-    else:
-        return users[0]["id"]
-
-
-def get_userid2(mastodon, rest):
-    userid = get_userid(mastodon, rest)
-    if isinstance(userid, list):
-        cprint("  multiple matches found:", fg("red"))
-        printUsersShort(userid)
-        raise AlreadyPrintedException()
-    elif userid == -1:
-        raise Exception("  username '{}' not found".format(rest))
-
+    user_list = mastodon.account_search(rest, limit=1)
+    if not user_list:
+        raise Exception(f"  username '{rest}' not found")
+        return
+    user = user_list.pop()
+    if exact:
+        username_check = rest.lstrip("@").strip()
+        username_acct = user.get("acct").lstrip("@").strip()
+        if username_check != username_acct:
+            if "@" not in username_check:
+                raise ValueError("  Please use a more exact username for this command.")
+            else:
+                raise Exception(f"  {username_check} not found.")
+    userid = user.get("id")
     return userid
 
 
 def get_list_id(mastodon, rest):
     """Get the ID for a list"""
     if not rest or not rest.strip():
         raise Exception("List argument missing.")
@@ -248,24 +300,37 @@
             if k in args:
                 kwargs[flags[k]] = not kwargs[flags[k]]
 
     return (rest, kwargs)
 
 
 def flaghandler_note(mastodon, rest):
-    return flaghandler(rest, True, {"m": "mention", "f": "favourite", "b": "reblog", "F": "follow", "p": "poll"})
+    return flaghandler(
+        rest,
+        True,
+        {
+            "m": "mention",
+            "f": "favourite",
+            "b": "reblog",
+            "F": "follow",
+            "r": "follow_request",
+            "p": "poll",
+            "u": "update"},
+    )
 
 
 def flaghandler_tootreply(mastodon, rest):
     """Parse input for flags and prompt user.  On success, returns
     a tuple of the input string (minus flags) and a dict of keyword
     arguments for Mastodon.status_post().  On failure, returns
     (None, None)."""
 
-    (rest, flags) = flaghandler(rest, False, {"v":"visibility","c":"cw","C":"noCW","m":"media"})
+    (rest, flags) = flaghandler(
+        rest, False, {"v": "visibility", "c": "cw", "C": "noCW", "m": "media"}
+    )
 
     # if any flag is true, print a general usage message
     if True in flags.values():
         print("Press Ctrl-C to abort and return to the main prompt.")
 
     # initialize kwargs to default values
     kwargs = {
@@ -331,15 +396,15 @@
 
             # expand paths and check file access
             fname = os.path.expanduser(fname).strip()
             if os.path.isfile(fname) and os.access(fname, os.R_OK):
                 media.append(fname)
                 count += 1
             else:
-                cprint("error: cannot find file {}".format(fname), fg("red"))
+                raise Exception(f"error: cannot find file {fname}")
 
         # upload, verify
         if count:
             print("Attaching files:")
             c = 1
             kwargs["media_ids"] = []
             for m in media:
@@ -366,14 +431,15 @@
 
 def print_toots(
     mastodon,
     listing,
     stepper=False,
     ctx_name=None,
     add_completion=True,
+    show_toot=False,
     sort_toots=True,
 ):
     """Print toot listings and allow context dependent commands.
 
     If `stepper` is True it lets user step through listings with
     enter key. Entering [a] aborts stepping.
 
@@ -382,66 +448,72 @@
     parameters are necessary.
 
     Args:
         mastodon: Mastodon instance
         listing: Iterable containing toots
         ctx_name (str, optional): Displayed in command prompt
         add_completion (bool, optional): Add toots to completion list
+        show:toot (bool, optional): whether to show the toot by default or not
 
     Examples:
         >>> print_toots(mastodon, mastodon.timeline_home(), ctx_name='home')
 
     sort_toots is used to apply reversed (chronological) sort to the list of toots.
         Default is true; threading needs this to be false.
     """
+    if listing is None:
+        cprint(
+            "No toots in current context.",
+            fg("white") + bg("red"),
+        )
+        return
     user = mastodon.account_verify_credentials()
     ctx = "" if ctx_name is None else " in {}".format(ctx_name)
 
     def say_error(*args, **kwargs):
         cprint(
-            "Invalid command. Use 'help' for a list of commands or press [enter] for next toot, [a] to abort.",
+            "Invalid command. Use 'help' for a list of commands. Press [enter] for next toot, [q] to abort.",
             fg("white") + bg("red"),
         )
 
     if sort_toots:
         toot_list = enumerate(reversed(listing))
     else:
         toot_list = enumerate(listing)
 
     for pos, toot in toot_list:
-        printToot(toot)
+        printToot(toot, show_toot)
         if add_completion is True:
             completion_add(toot)
 
         if stepper:
-            prompt = "[@{} {}/{}{}]: ".format(
-                str(user["username"]), pos + 1, len(listing), ctx
-            )
+            username = user.get("username")
+            prompt = f"[@{username} {pos+1}/{len(listing)}{ctx}]: "
             command = None
-            while command not in ["", "a"]:
+            while command not in ["", "q"]:
                 command = input(prompt).split(" ", 1)
 
                 try:
                     rest = command[1]
                 except IndexError:
                     rest = ""
                 command = command[0]
-                if command not in ["", "a"]:
+                if command not in ["", "q"]:
                     cmd_func = commands.get(command, say_error)
                     if (
                         hasattr(cmd_func, "__argstr__")
                         and cmd_func.__argstr__ is not None
                     ):
                         if cmd_func.__argstr__.startswith("<id>"):
-                            rest = str(IDS.to_local(toot["id"])) + " " + rest
+                            rest = str(find_original_toot_id(toot)) + " " + rest
                         if cmd_func.__argstr__.startswith("<user>"):
                             rest = "@" + toot["account"]["username"] + " " + rest
                     cmd_func(mastodon, rest)
 
-            if command == "a":
+            if command == "q":
                 break
 
 
 def toot_visibility(mastodon, flag_visibility=None, parent_visibility=None):
     """Return the visibility of a toot.
     We use the following precedence for flagging the privacy of a toot:
     flags > parent (if not public) > account settings
@@ -752,20 +824,23 @@
 
 def format_toot_idline(toot):
     """Get boost/faves counts, toot ID, visibility, and
     already-faved/boosted indicators for a typical toot printout."""
     # id-and-counts line: boosted count, faved count, tootid, visibility, favourited-already, boosted-already
     if not toot:
         return ""
-    out = [
-        stylize(GLYPHS["boost"] + ":" + str(toot["reblogs_count"]), fg("cyan")),
-        stylize(GLYPHS["fave"] + ":" + str(toot["favourites_count"]), fg("yellow")),
-        stylize("id:" + str(IDS.to_local(toot["id"])), fg("red")),
-        stylize("vis:" + GLYPHS[toot["visibility"]], fg("blue")),
-    ]
+    reblogs_count = toot.get("reblogs_count", 0)
+    favourites_count = toot.get("favourites_count", 0)
+    visibility = toot.get("visibility")
+    out = []
+    out.append(stylize(GLYPHS["boost"] + ":" + str(reblogs_count), fg("cyan")))
+    out.append(stylize(GLYPHS["fave"] + ":" + str(favourites_count), fg("yellow")))
+    out.append(stylize("id:" + str(IDS.to_local(toot.get("id"))), fg("white")))
+    if visibility:
+        out.append(stylize("vis:" + GLYPHS[visibility], fg("blue")))
 
     # app used to post. frequently empty
     if toot.get("application") and toot.get("application").get("name"):
         out.append(
             "".join(
                 (
                     stylize("via ", fg("white")),
@@ -778,18 +853,19 @@
         out.append(stylize(GLYPHS["favourited"], fg("magenta")))
     if toot.get("reblogged"):
         out.append(stylize(GLYPHS["reblogged"], fg("magenta")))
 
     return " ".join(out)
 
 
-def printToot(toot):
+def printToot(toot, show_toot=False, dim=False):
     if not toot:
         return
 
+    show_toot_text = True
     out = []
     # if it's a boost, only output header line from toot
     # then get other data from toot['reblog']
     if toot.get("reblog"):
         header = stylize("  Boosted by ", fg("yellow"))
         display_name = format_display_name(toot["account"]["display_name"])
         name = " ".join((display_name, format_username(toot["account"]) + ":"))
@@ -799,39 +875,45 @@
     # get the first two lines
     random.seed(toot["account"]["display_name"])
     out += [
         "  " + format_toot_nameline(toot, fg(random.choice(COLORS))),
         "  " + format_toot_idline(toot),
     ]
 
-    if toot["spoiler_text"] != "":
+    if toot.get("spoiler_text", "") != "":
         # pass CW through get_content for wrapping/indenting
         faketoot = {"content": "[CW: " + toot["spoiler_text"] + "]"}
         out.append(stylize(get_content(faketoot), fg("red")))
+        show_toot_text = False
+
+    if toot.get("filtered"):
+        filter_titles = ", ".join([x["filter"]["title"] for x in toot.filtered])
+        faketoot = {"content": "[Filter: " + filter_titles + "]"}
+        out.append(stylize(get_content(faketoot), fg("red")))
+        show_toot_text = False
+
+    if show_toot_text or show_toot:
+        out.append(get_content(toot))
 
-    out.append(get_content(toot))
+    if toot.get("status"):
+        out.append(get_content(toot.get("status")))
+        if toot.get("status").get("media_attachments"):
+            out.append("\n".join(get_media_attachments(toot.get("status"))))
 
-    if toot.get("media_attachments"):
+    if toot.get("media_attachments") and (show_toot_text or show_toot):
         # simple version: output # of attachments. TODO: urls instead?
-        nsfw = "CW " if toot["sensitive"] else ""
-        out.append(
-            stylize(
-                "  " + nsfw + "media: " + str(len(toot["media_attachments"])),
-                fg("magenta"),
-            )
-        )
-        if show_media_links:
-            for media in toot["media_attachments"]:
-                out.append(stylize("   " + nsfw + " " + media.url, fg("green")))
+        out.append("\n".join(get_media_attachments(toot)))
 
     if toot.get("poll"):
-        # if there's a poll then just show that it exists for now
-        out.append("  [poll]")
+        out.append(get_poll(toot))
 
-    print("\n".join(out))
+    if dim:
+        cprint("\n".join(out), attr("dim"))
+    else:
+        print("\n".join(out))
     print()
 
 
 def edittoot(text):
     global is_streaming
     if is_streaming:
         cprint(
@@ -846,14 +928,23 @@
 
 def printList(list_item):
     """Prints list entry nicely with hardcoded colors."""
     cprint(list_item["title"], fg("cyan"), end=" ")
     cprint("(id: %s)" % list_item["id"], fg("red"))
 
 
+def printFilter(filter_item):
+    """Prints filter entry nicely with hardcoded colors."""
+    cprint(filter_item["phrase"], fg("cyan"), end=" ")
+    cprint("(id: %s," % filter_item["id"], fg("red"), end=" ")
+    cprint("context: %s, " % filter_item["context"], fg("red"), end=" ")
+    cprint("expires_at: %s, " % filter_item["expires_at"], fg("red"), end=" ")
+    cprint("whole_word: %s)" % filter_item["whole_word"], fg("red"))
+
+
 #####################################
 ######## DECORATORS          ########
 #####################################
 commands = OrderedDict()
 
 
 def command(argstr=None, section=None):
@@ -901,15 +992,15 @@
     if rest and rest != "":
 
         args = rest.split()
         if args[0] in commands.keys():
             # Show Command Help
             try:
                 cmd_func = commands[args[0]]
-            except:
+            except Exception:
                 print(__friendly_cmd_error__.format(rest))
                 return
 
             try:
                 cmd_args = cmd_func.__argstr__
             except Exception:
                 cmd_args = ""
@@ -1092,28 +1183,71 @@
     )
 
     while posted is False:
         try:
             reply_toot = mastodon.status_post(
                 "%s %s" % (mentions, text), in_reply_to_id=parent_id, **kwargs
             )
-            msg = "  Replied with: " + get_content(reply_toot)
-            cprint(msg, fg("red"))
+            msg = "  Replied with:\n" + get_content(reply_toot)
+            cprint(msg, attr("dim"))
             posted = True
         except Exception as e:
             cprint("error while posting: {}".format(type(e).__name__), fg("red"))
 
         if posted is False:
             retry = input("Edit toot and re-try? [Y/N]: ")
             if retry.lower() == "y":
                 text = edittoot(text=text)
             else:
                 posted = True
 
 
+@command("<id> [votes]", "Toots")
+def vote(mastodon, rest):
+    """Vote  your toot by ID
+
+    Example:
+        >>> vote 23 1
+        >>> vote 23 1,2,3
+    """
+    try:
+        poll_id = None
+        toot_id, rest = rest.split(" ", 1)
+        global_id = IDS.to_global(toot_id)
+        poll = mastodon.status(global_id).get("poll")
+        if poll:
+            poll_id = poll.get("id")
+        if poll_id is None:
+            cprint(f"  {toot_id} does not point to a valid poll.", fg("red"))
+            return
+
+        if rest is None:
+            cprint(
+                "Note has no options.",
+                fg("white") + bg("red"),
+            )
+            return
+
+        vote_options = rest_to_list(rest)
+        if len(vote_options) > 1 and not poll.get("multiple"):
+            cprint(
+                "Too many votes cast.",
+                fg("white") + bg("red"),
+            )
+            return
+
+        mastodon.poll_vote(poll_id, vote_options)
+        print("Vote cast.")
+    except Exception as e:
+        cprint(
+            f"  {e}",
+            fg("red"),
+        )
+
+
 @command("<id>", "Toots")
 def delete(mastodon, rest):
     """Deletes your toot by ID"""
     rest = IDS.to_global(rest)
     if rest is None:
         return
     mastodon.status_delete(rest)
@@ -1125,55 +1259,89 @@
     """Boosts a toot by ID."""
     rest = IDS.to_global(rest)
     if rest is None:
         return
     try:
         mastodon.status_reblog(rest)
         boosted = mastodon.status(rest)
-        msg = "  You boosted: " + fg("white") + get_content(boosted)
-        cprint(msg, fg("green"))
+        msg = "  You boosted:\n " + fg("white") + get_content(boosted)
+        cprint(msg, attr("dim"))
     except Exception as e:
         cprint("Received error: ", fg("red") + attr("bold"), end="")
         cprint(e, fg("magenta") + attr("bold") + attr("underlined"))
 
 
 @command("<id>", "Toots")
 def unboost(mastodon, rest):
     """Removes a boosted toot by ID."""
     rest = IDS.to_global(rest)
     if rest is None:
         return
     mastodon.status_unreblog(rest)
     unboosted = mastodon.status(rest)
-    msg = "  Removed boost: " + get_content(unboosted)
-    cprint(msg, fg("red"))
+    msg = "  Removed boost:\n " + get_content(unboosted)
+    cprint(msg, attr("dim"))
 
 
-@command("<id>", "Toots")
+@command("<id> [<id>]", "Toots")
 def fav(mastodon, rest):
-    """Favorites a toot by ID."""
-    rest = IDS.to_global(rest)
-    if rest is None:
-        return
-    mastodon.status_favourite(rest)
-    faved = mastodon.status(rest)
-    msg = "  Favorited:\n" + get_content(faved)
-    cprint(msg, fg("red"))
+    """Favorites a toot by ID or IDs."""
+    favorite_ids = rest_to_list(rest)
+    multiple = len(favorite_ids) > 1
+    for favorite_id in favorite_ids:
+        if favorite_id:
+            favorite_global_id = IDS.to_global(favorite_id)
+            if favorite_global_id is None:
+                cprint(f"  Can't favorite id {favorite_id}: Not found", fg("red") + attr("bold"))
+                next
+            faved = mastodon.status_favourite(favorite_global_id)
+            msg = f"  Favorited ({favorite_id}):\n" + get_content(faved)
+            cprint(msg, attr("dim"))
+            if multiple:
+                print()
 
 
-@command("<id>", "Toots")
+@command("<id> [<id>]", "Toots")
 def unfav(mastodon, rest):
-    """Removes a favorite toot by ID."""
+    """Removes a favorite toot by ID or IDs."""
+    favorite_ids = rest_to_list(rest)
+    multiple = len(favorite_ids) > 1
+    for favorite_id in favorite_ids:
+        if favorite_id:
+            favorite_global_id = IDS.to_global(favorite_id)
+            if favorite_global_id is None:
+                cprint(f"  Can't unfavorite id {favorite_id}: Not found", fg("red") + attr("bold"))
+                next
+            unfaved = mastodon.status_unfavourite(favorite_global_id)
+            msg = f"  Removed favorite ({favorite_id}):\n" + get_content(unfaved)
+            cprint(msg, fg("yellow"))
+            if multiple:
+                print()
+
+
+@command("<id>", "Toots")
+def show(mastodon, rest):
+    """Shows a toot by ID"""
     rest = IDS.to_global(rest)
     if rest is None:
         return
-    mastodon.status_unfavourite(rest)
-    unfaved = mastodon.status(rest)
-    msg = "  Removed favorite: " + get_content(unfaved)
-    cprint(msg, fg("yellow"))
+    printToot(mastodon.status(rest), show_toot=True)
+
+
+@command("", "Filter")
+def filters(mastodon, rest):
+    """Shows the filters that the user has created."""
+    if not (list_support(mastodon)):
+        return
+    user_filters = mastodon.filters()
+    if len(user_filters) == 0:
+        cprint("No filters found", fg("red"))
+        return
+    for filter_item in user_filters:
+        printFilter(filter_item)
 
 
 @command("<id>", "Toots")
 def bookmark(mastodon, rest):
     """Bookmark a toot by ID."""
     rest = IDS.to_global(rest)
     if rest is None:
@@ -1193,15 +1361,22 @@
     mastodon.status_unbookmark(rest)
     item = mastodon.status(rest)
     msg = "  Removed bookmark: " + get_content(item)
     cprint(msg, fg("yellow"))
 
 
 @command("<id>", "Toots")
-def history(mastodon, rest):
+def showhistory(mastodon, rest):
+    """Shows the history of the conversation for an ID with CWs/ Filters displayed"""
+    history(mastodon, rest, show_toot=True)
+
+
+
+@command("<id>", "Toots")
+def history(mastodon, rest, show_toot=False):
     """Shows the history of the conversation for an ID.
 
     ex: history 23"""
     stepper, rest = step_flag(rest)
     rest = IDS.to_global(rest)
     if rest is None:
         return
@@ -1210,48 +1385,57 @@
         current_toot = mastodon.status(rest)
         conversation = mastodon.status_context(rest)
         print_toots(
             mastodon,
             conversation["ancestors"],
             stepper,
             ctx_name="Previous toots",
+            show_toot=show_toot,
             sort_toots=False,
         )
 
         if stepper is False:
             cprint("Current Toot:", fg("yellow"))
-        print_toots(mastodon, [current_toot], stepper, ctx_name="Current toot")
+        print_toots(mastodon, [current_toot], stepper, ctx_name="Current toot", show_toot=show_toot)
         # printToot(current_toot)
         # completion_add(current_toot)
     except Exception as e:
         cprint("{}: please try again later".format(type(e).__name__), fg("red"))
 
 
 @command("<id>", "Toots")
-def thread(mastodon, rest):
+def showthread(mastodon, rest):
+    """Shows the complete thread of the conversation for an ID while showing CWs / filters.
+
+    ex: showthread 23"""
+    thread(mastodon, rest, show_toot=True)
+
+
+@command("<id>", "Toots")
+def thread(mastodon, rest, show_toot=False):
     """Shows the complete thread of the conversation for an ID.
 
     ex: thread 23"""
 
     # Save the original "rest" so the history command can use it
     original_rest = rest
     stepper, rest = step_flag(rest)
 
     rest = IDS.to_global(rest)
     if rest is None:
         return
 
     try:
         # First display the history
-        history(mastodon, original_rest)
+        history(mastodon, original_rest, show_toot)
 
         # Then display the rest
         # current_toot = mastodon.status(rest)
         conversation = mastodon.status_context(rest)
-        print_toots(mastodon, conversation["descendants"], stepper, sort_toots=False)
+        print_toots(mastodon, conversation["descendants"], stepper, show_toot=show_toot, sort_toots=False)
 
     except Exception as e:
         raise e
         cprint("{}: please try again later".format(type(e).__name__), fg("red"))
 
 
 @command("<id>", "Toots")
@@ -1348,32 +1532,89 @@
             else:
                 cprint("Links argument was not correct. Please try again.", fg("red"))
 
 
 @command("", "Timeline")
 def home(mastodon, rest):
     """Displays the Home timeline."""
+    global LAST_PAGE, LAST_CONTEXT
     stepper, rest = step_flag(rest)
-    print_toots(mastodon, mastodon.timeline_home(), stepper, ctx_name="home")
+    LAST_PAGE = mastodon.timeline_home()
+    LAST_CONTEXT = "home"
+    print_toots(mastodon, LAST_PAGE, stepper, ctx_name=LAST_CONTEXT)
 
 
 @command("", "Timeline")
 def fed(mastodon, rest):
     """Displays the Federated timeline."""
+    global LAST_PAGE, LAST_CONTEXT
     stepper, rest = step_flag(rest)
-    print_toots(
-        mastodon, mastodon.timeline_public(), stepper, ctx_name="federated timeline"
-    )
+    LAST_PAGE = mastodon.timeline_public()
+    LAST_CONTEXT = "federated timeline"
+    print_toots(mastodon, LAST_PAGE, stepper, ctx_name=LAST_CONTEXT)
 
 
 @command("", "Timeline")
 def local(mastodon, rest):
     """Displays the Local timeline."""
+    global LAST_PAGE, LAST_CONTEXT
+    stepper, rest = step_flag(rest)
+    LAST_PAGE = mastodon.timeline_local()
+    LAST_CONTEXT = "local timeline"
+    print_toots(mastodon, LAST_PAGE, stepper, ctx_name=LAST_CONTEXT)
+
+
+@command("", "Timeline")
+def next(mastodon, rest):
+    """Displays the next page of paginated results."""
+    global LAST_PAGE, LAST_CONTEXT
+    curr_page = LAST_PAGE
+    stepper, rest = step_flag(rest)
+    if LAST_PAGE:
+        LAST_PAGE = mastodon.fetch_next(LAST_PAGE)
+        if LAST_PAGE:
+            print_toots(mastodon, LAST_PAGE, stepper, ctx_name=LAST_CONTEXT)
+            return
+        else:
+            LAST_PAGE = curr_page
+    if LAST_CONTEXT:
+        cprint(
+            "No more toots in current context: " + LAST_CONTEXT,
+            fg("white") + bg("red"),
+        )
+    else:
+        cprint(
+            "No current context.",
+            fg("white") + bg("red"),
+        )
+
+
+@command("", "Timeline")
+def prev(mastodon, rest):
+    """Displays the previous page of paginated results."""
+    global LAST_PAGE, LAST_CONTEXT
     stepper, rest = step_flag(rest)
-    print_toots(mastodon, mastodon.timeline_local(), stepper, ctx_name="local timeline")
+    curr_page = LAST_PAGE
+    if LAST_PAGE:
+        LAST_PAGE = mastodon.fetch_previous(LAST_PAGE)
+        if LAST_PAGE:
+            print_toots(mastodon, LAST_PAGE, stepper, ctx_name=LAST_CONTEXT)
+            return
+        else:
+            LAST_PAGE = curr_page
+    if LAST_CONTEXT:
+        cprint(
+            "No more toots in current context: " + LAST_CONTEXT,
+            fg("white") + bg("red"),
+        )
+    else:
+        cprint(
+            "No current context.",
+            fg("white") + bg("red"),
+        )
 
 
 @command("<timeline>", "Timeline")
 def stream(mastodon, rest):
     """Streams a timeline. Specify home, fed, local, list, or a #hashtagname.
 
     Timeline 'list' requires a list name (ex: stream list listname).
@@ -1470,30 +1711,43 @@
             handle.close()
         except AttributeError:
             handle.running = False
             pass  # Trap for handle not getting set if no toots were received while streaming
         is_streaming = False
 
 
+@command("", "Timeline")
+def mentions(mastodon, rest):
+    """Displays the Notifications timeline with only mentions
+
+    ex: 'mentions'"""
+    note(mastodon, "-bfFpru")
+
+
 @command("[<filter>]", "Timeline")
 def note(mastodon, rest):
     """Displays the Notifications timeline.
 
     ex: 'note'
                  will show all notifications
         'note -b'
                  will show all notifications minus boosts
-        'note -f -F -b' (or 'note -fFb')
+        'note -f -F -b -u' (or 'note -fFb')
                 will only show mentions
 
     Options:
         -b    Filter boosts
         -f    Filter favorites
         -F    Filter follows
-        -m    Filter mentions"""
+        -m    Filter mentions
+        -p    Filter polls
+        -r    Filter follow requests
+        -u    Filter updates"""
+
+    displayed_notification = False
 
     # Fill in Content fields first.
     try:
         (text, kwargs) = flaghandler_note(mastodon, rest)
     except KeyboardInterrupt:
         # user abort, return to main prompt
         print("")
@@ -1503,76 +1757,79 @@
         mastodon.notifications()
     )  # TODO: Check if fetch_remaining should be used here
     if not (len(notifications) > 0):
         cprint("You don't have any notifications yet.", fg("magenta"))
         return
 
     for note in reversed(notifications):
-        display_name = "  " + format_display_name(note["account"]["display_name"])
-        username = format_username(note["account"])
-        note_id = str(note["id"])
+        note_type = note.get("type")
+        note_status = note.get("status", {})
+        note_created_at = note_status.get("created_at")
+        if note_created_at:
+            note_time = " " + stylize(
+                format_time(note_created_at), attr("dim")
+            )
+        note_media_attachments = note_status.get("media_attachments")
+        display_name = "  " + format_display_name(note.get("account").get("display_name"))
+        username = format_username(note.get("account"))
+        note_id = str(note.get("id"))
 
         random.seed(display_name)
 
         # Check if we should even display this note type
-        if kwargs[note["type"]]:
+        if kwargs[note_type]:
             # Display Note ID
             cprint(" note: " + note_id, fg("magenta"))
 
             # Mentions
-            if note["type"] == "mention":
-                time = " " + stylize(
-                    format_time(note["status"]["created_at"]), attr("dim")
-                )
+            if note_type == "mention":
+                displayed_notification = True
                 cprint(display_name + username, fg("magenta"))
-                print("  " + format_toot_idline(note["status"]) + "  " + time)
-                cprint(get_content(note["status"]), attr("bold"), fg("white"))
+                print("  " + format_toot_idline(note_status) + "  " + note_time)
+                cprint(get_content(note_status), attr("bold"), fg("white"))
                 print(stylize("", attr("dim")))
-
-            # Favorites
-            elif note["type"] == "favourite":
-                tz_info = note["status"]["created_at"].tzinfo
-                note_time_diff = (
-                    datetime.datetime.now(tz_info) - note["status"]["created_at"]
-                )
-                countsline = format_toot_idline(note["status"])
-                format_time(note["status"]["created_at"])
-                time = " " + stylize(
-                    format_time(note["status"]["created_at"]), attr("dim")
-                )
-                content = get_content(note["status"])
-                cprint(display_name + username, fg(random.choice(COLORS)), end="")
-                cprint(" favorited your status:", fg("yellow"))
-                print("  " + countsline + stylize(time, attr("dim")))
-                cprint(content, attr("dim"))
-                if getattr(note["status"], "poll", None):
-                    poll = get_poll(note["status"])
-                    cprint(poll, attr("dim"))
-
-            # Boosts
-            elif note["type"] == "reblog":
-                cprint(display_name + username + " boosted your status:", fg("yellow"))
-                cprint(get_content(note["status"]), attr("dim"))
-                if getattr(note["status"], "poll", None):
-                    poll = get_poll(note["status"])
-                    cprint(poll, attr("dim"))
+                if note_media_attachments:
+                    print("\n".join(get_media_attachments(note_status)))
 
             # Follows
-            elif note["type"] == "follow":
+            elif note_type == "follow":
+                displayed_notification = True
                 print("  ", end="")
                 cprint(display_name + username + " followed you!", fg("yellow"))
 
-            # Poll
-            elif note["type"] == "poll":
-                cprint(get_content(note["status"]), attr("dim"))
-                cprint(get_poll(note["status"]), attr("dim"))
+            elif note_type == "follow_request":
+                displayed_notification = True
+                cprint(display_name + username + " sent a follow request", fg("yellow"))
+                cprint("  Use 'accept' or 'reject' to accept or reject the request", fg("yellow"))
+
+            # Update
+            elif note_type in ["update", "favourite", "reblog", "poll"]:
+                displayed_notification = True
+                countsline = format_toot_idline(note_status)
+                content = get_content(note_status)
+                cprint(display_name + username, fg(random.choice(COLORS)), end="")
+                if note_type == "update":
+                    cprint(f" updated their status:", fg("yellow"))
+                elif note_type == "reblog":
+                    cprint(f" boosted your status:", fg("yellow"))
+                elif note_type == "poll":
+                    cprint(f" ended their poll:", fg("yellow"))
+                else:
+                    cprint(f" favorited your status:", fg("yellow"))
+                print("  " + countsline + stylize(note_time, attr("dim")))
+                cprint(content, attr("dim"))
+                if getattr(note_status, "poll", None):
+                    poll = get_poll(note_status)
+                    cprint(poll, attr("dim"))
 
-            # blank line
             print()
 
+    if not displayed_notification:
+        cprint("No notifications of this type are available.", fg("magenta"))
+
 
 @command("[<note_id>]", "Timeline")
 def dismiss(mastodon, rest):
     """Dismisses notifications.
 
     ex: dismiss or dismiss 1234567
 
@@ -1597,160 +1854,194 @@
 @command("<user>", "Users")
 def block(mastodon, rest):
     """Blocks a user by username or id.
 
     ex: block 23
         block @user
         block @user@instance.example.com"""
-    userid = get_userid2(mastodon, rest)
+    userid = get_unique_userid(mastodon, rest)
     relations = mastodon.account_block(userid)
     if relations["blocking"]:
         cprint("  user " + str(userid) + " is now blocked", fg("blue"))
+        username = "@" + mastodon.account(userid)["acct"]
+        if username in completion_list:
+            completion_list.remove(username)
 
 
 @command("<user>", "Users")
 def unblock(mastodon, rest):
     """Unblocks a user by username or id.
 
     ex: unblock 23
-        unblock @user
         unblock @user@instance.example.com"""
-    userid = get_userid2(mastodon, rest)
+    userid = get_unique_userid(mastodon, rest)
     relations = mastodon.account_unblock(userid)
     if not relations["blocking"]:
         cprint("  user " + str(userid) + " is now unblocked", fg("blue"))
+        username = "@" + mastodon.account(userid)["acct"]
+        if username not in completion_list:
+            bisect.insort(completion_list, username)
 
 
 @command("<user>", "Users")
 def follow(mastodon, rest):
     """Follows an account by username or id.
 
     ex: follow 23
-        follow @user
         follow @user@instance.example.com"""
-    userid = get_userid2(mastodon, rest)
+    userid = get_unique_userid(mastodon, rest)
     relations = mastodon.account_follow(userid)
     if relations["following"]:
         cprint("  user " + str(userid) + " is now followed", fg("blue"))
         username = "@" + mastodon.account(userid)["acct"]
         if username not in completion_list:
             bisect.insort(completion_list, username)
 
 
 @command("<user>", "Users")
 def unfollow(mastodon, rest):
     """Unfollows an account by username or id.
 
     ex: unfollow 23
-        unfollow @user
         unfollow @user@instance.example.com"""
-    userid = get_userid2(mastodon, rest)
+    userid = get_unique_userid(mastodon, rest)
     relations = mastodon.account_unfollow(userid)
-    if not relations["following"]:
+    if not relations.get("following"):
         cprint("  user " + str(userid) + " is now unfollowed", fg("blue"))
     username = "@" + mastodon.account(userid)["acct"]
     if username in completion_list:
         completion_list.remove(username)
 
 
-@command("<user>", "Users")
+@command("<user> [<duration>]", "Users")
 def mute(mastodon, rest):
     """Mutes a user by username or id.
 
     ex: mute 23
-        mute @user
-        mute @user@instance.example.com"""
-    userid = get_userid2(mastodon, rest)
-    relations = mastodon.account_mute(userid)
-    if relations["muting"]:
-        cprint("  user " + str(userid) + " is now muted", fg("blue"))
+        mute @user@instance.example.com
+        mute @user 30s"""
+    mute_time = None
+    mute_seconds = None
+    if " " in rest:
+        username, mute_time = rest.split(" ")
+    else:
+        username = rest
+    if mute_time:
+        mute_seconds = pytimeparse.parse(mute_time)
+    userid = get_unique_userid(mastodon, username)
+    relations = mastodon.account_mute(userid, duration=mute_seconds)
+    if relations.get("muting"):
+        if mute_seconds:
+            cprint("  user " + username + " is now muted for " + mute_time, fg("blue"))
+        else:
+            cprint("  user " + username + " is now muted", fg("blue"))
 
 
 @command("<user>", "Users")
 def unmute(mastodon, rest):
     """Unmutes a user by username or id.
 
     ex: unmute 23
-        unmute @user
         unmute @user@instance.example.com"""
-    userid = get_userid2(mastodon, rest)
+    userid = get_unique_userid(mastodon, rest)
     relations = mastodon.account_unmute(userid)
+    username = rest
     if not relations["muting"]:
-        cprint("  user " + str(userid) + " is now unmuted", fg("blue"))
+        cprint("  user " + username + " is now unmuted", fg("blue"))
 
 
 @command("<query>", "Discover")
 def search(mastodon, rest):
     """Search for a #tag or @user.
 
     ex:  search #tagname
          search @user
          search @user@instance.example.com"""
+    global LAST_PAGE, LAST_CONTEXT
     usage = str("  usage: search #tagname\n" + "         search @username")
     stepper, rest = step_flag(rest)
     try:
         indicator = rest[:1]
         query = rest[1:]
-    except:
+    except Exception:
         cprint(usage, fg("red"))
         return
 
     # @ user search
     if indicator == "@" and not query == "":
         users = mastodon.account_search(query)
 
         for user in users:
             printUser(user)
     # end @
 
     # # hashtag search
     elif indicator == "#" and not query == "":
+        LAST_PAGE = mastodon.timeline_hashtag(query)
+        LAST_CONTEXT = "search for #{}".format(query)
         print_toots(
             mastodon,
-            mastodon.timeline_hashtag(query),
+            LAST_PAGE,
             stepper,
-            ctx_name="search for #{}".format(query),
+            ctx_name=LAST_CONTEXT,
             add_completion=False,
         )
     # end #
 
     else:
-        cprint("  Invalid format. (General search coming soon.)\n" + usage, fg("red"))
-
+        raise ValueError("  Invalid format.\n" + usage)
     return
 
 
 @command("<user> [<N>]", "Discover")
+def user(mastodon, rest):
+    """Displays profile information for another user
+
+     <user>:   a userID, @username, or @user@instance
+
+    ex: user 23
+        user @user
+        user @user@instance.example.com"""
+    userid = get_unique_userid(mastodon, rest, exact=False)
+    profile = mastodon.account(userid)
+    if profile:
+        printUser(profile)
+        return
+    raise Exception("user {rest} not found")
+
+
+@command("<user> [<N>]", "Discover")
 def view(mastodon, rest):
     """Displays toots from another user.
 
      <user>:   a userID, @username, or @user@instance
         <N>:   (optional) show N toots maximum
 
     ex: view 23
         view @user 10
         view @user@instance.example.com"""
-    (userid, _, count) = rest.partition(" ")
+    global LAST_PAGE, LAST_CONTEXT
+    (user, _, count) = rest.partition(" ")
 
     # validate count argument
     if not count:
         count = None
     else:
         try:
             count = int(count)
         except ValueError:
-            cprint("  invalid count: {}".format(count), fg("red"))
-            return
+            raise ValueError("  invalid count: {count}")
 
-    # validate userid argument
-    userid = get_userid2(mastodon, userid)
+    userid = get_unique_userid(mastodon, user, exact=False)
+    LAST_PAGE = mastodon.account_statuses(userid, limit=count)
+    LAST_CONTEXT = f"{user} timeline"
     print_toots(
         mastodon,
-        mastodon.account_statuses(userid, limit=count),
-        ctx_name="user timeline",
+        LAST_PAGE,
+        ctx_name=LAST_CONTEXT,
         add_completion=False,
     )
 
 
 @command("", "Profile")
 def info(mastodon, rest):
     """Prints your user info."""
@@ -1827,31 +2118,29 @@
 
 
 @command("<user>", "Profile")
 def accept(mastodon, rest):
     """Accepts a user's follow request by username or id.
 
     ex: accept 23
-        accept @user
         accept @user@instance.example.com"""
-    userid = get_userid2(mastodon, rest)
+    userid = get_unique_userid(mastodon, rest)
     mastodon.follow_request_authorize(userid)
-    cprint("  user {}'s request is accepted".format(userid), fg("blue"))
+    cprint(f"  user {rest}'s follow request is accepted", fg("blue"))
 
 
 @command("<user>", "Profile")
 def reject(mastodon, rest):
     """Rejects a user's follow request by username or id.
 
     ex: reject 23
-        reject @user
         reject @user@instance.example.com"""
-    userid = get_userid2(mastodon, rest)
+    userid = get_unique_userid(mastodon, rest)
     mastodon.follow_request_reject(userid)
-    cprint("  user {}'s request is rejected".format(userid), fg("blue"))
+    cprint(f"  user {rest}'s follow request is rejected", fg("blue"))
 
 
 @command("", "Profile")
 def faves(mastodon, rest):
     """Displays posts you've favourited."""
     print_toots(
         mastodon, mastodon.favourites(), ctx_name="favourites", add_completion=False
@@ -1890,14 +2179,20 @@
 
 @command("", "Profile")
 def quit(mastodon, rest):
     """Ends the program."""
     sys.exit("Goodbye!")
 
 
+@command("", "Profile")
+def exit(mastodon, rest):
+    """Ends the program."""
+    sys.exit("Goodbye!")
+
+
 @command("", "List")
 def lists(mastodon, rest):
     """Shows the lists that the user has created."""
     if not (list_support(mastodon)):
         return
     user_lists = mastodon.lists()
     if len(user_lists) == 0:
@@ -1952,38 +2247,43 @@
 
 
 @command("<list>", "List")
 def listhome(mastodon, rest):
     """Show the toots from a list.
     ex:  listhome listname
          listhome 23"""
+    global LAST_PAGE, LAST_CONTEXT
     if not (list_support(mastodon)):
         return
     if not rest:
         cprint("Argument required.", fg("red"))
         return
     stepper, rest = step_flag(rest)
-
-    item = get_list_id(mastodon, rest)
-    list_toots = mastodon.timeline_list(item)
-    print_toots(mastodon, list_toots, stepper, ctx_name="list")
+    list_name = rest.strip()
+    item = get_list_id(mastodon, list_name)
+    LAST_PAGE = mastodon.timeline_list(item)
+    LAST_CONTEXT = f"list ({list_name})"
+    print_toots(mastodon, LAST_PAGE, stepper, ctx_name=LAST_CONTEXT)
 
 
 @command("<list>", "List")
 def listaccounts(mastodon, rest):
     """Show the accounts for the list.
     ex:  listaccounts listname
          listaccounts 23"""
     if not (list_support(mastodon)):
         return
     item = get_list_id(mastodon, rest)
     list_accounts = mastodon.fetch_remaining(mastodon.list_accounts(item))
 
     cprint("List: %s" % rest, fg("green"))
     for user in list_accounts:
+        username = "@" + user.get("acct")
+        if username not in completion_list:
+            bisect.insort(completion_list, username)
         printUser(user)
 
 
 @command("<list> <user>", "List")
 def listadd(mastodon, rest):
     """Add user to list.
     ex:  listadd listname @user@instance.example.com
@@ -1995,15 +2295,15 @@
         return
     items = rest.split(" ")
     if len(items) < 2:
         cprint("Not enough arguments.", fg("red"))
         return
 
     list_id = get_list_id(mastodon, items[0])
-    account_id = get_userid2(mastodon, items[1])
+    account_id = get_unique_userid(mastodon, items[1])
     mastodon.list_accounts_add(list_id, account_id)
     cprint("Added {} to list {}.".format(items[1], items[0]), fg("green"))
 
 
 @command("<list> <user>", "List")
 def listremove(mastodon, rest):
     """Remove user from list.
@@ -2017,15 +2317,15 @@
         return
     items = rest.split(" ")
     if len(items) < 2:
         cprint("Not enough arguments.", fg("red"))
         return
 
     list_id = get_list_id(mastodon, items[0])
-    account_id = get_userid2(mastodon, items[1])
+    account_id = get_unique_userid(mastodon, items[1])
     mastodon.list_accounts_delete(list_id, account_id)
     cprint("Removed {} from list {}.".format(items[1], items[0]), fg("green"))
 
 
 #####################################
 ######### END COMMAND BLOCK #########
 #####################################
@@ -2121,15 +2421,16 @@
 
     about(mastodon, "")
 
     print("Enter a command. Use 'help' for a list of commands.")
     print("\n")
 
     user = mastodon.account_verify_credentials()
-    prompt = "[@{} ({})]: ".format(str(user["username"]), profile)
+    username = str(user.get("username"))
+    prompt = update_prompt(username=username, context=LAST_CONTEXT, profile=profile)
 
     # Completion setup stuff
     if list_support(mastodon, silent=True):
         for i in mastodon.lists():
             bisect.insort(completion_list, i["title"].lower())
 
     for i in mastodon.account_following(user["id"], limit=80):
@@ -2149,11 +2450,12 @@
             command = command[0]
             cmd_func = commands.get(command, say_error)
             cmd_func(mastodon, rest)
         except AlreadyPrintedException:
             pass
         except Exception as e:
             cprint(e, fg("red"))
+        prompt = update_prompt(username=username, context=LAST_CONTEXT, profile=profile)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `tootstream-0.3.9.0/src/tootstream/toot_parser.py` & `tootstream-0.4.0/src/tootstream/toot_parser.py`

 * *Files identical despite different names*

