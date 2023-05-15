# Comparing `tmp/flafl-0.0.4.tar.gz` & `tmp/flafl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flafl-0.0.4.tar", last modified: Tue Sep 15 22:57:59 2020, max compression
+gzip compressed data, was "flafl-0.0.6.tar", max compression
```

## Comparing `flafl-0.0.4.tar` & `flafl-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-15 22:57:59.369483 flafl-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (116)     5582 2020-09-15 22:57:59.369483 flafl-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3986 2020-09-15 22:57:52.000000 flafl-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-15 22:57:59.365483 flafl-0.0.4/flafl/
--rw-r--r--   0 runner    (1001) docker     (116)     4464 2020-09-15 22:57:52.000000 flafl-0.0.4/flafl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      998 2020-09-15 22:57:52.000000 flafl-0.0.4/flafl/bamboo.py
--rw-r--r--   0 runner    (1001) docker     (116)      459 2020-09-15 22:57:52.000000 flafl-0.0.4/flafl/context.py
--rw-r--r--   0 runner    (1001) docker     (116)      507 2020-09-15 22:57:52.000000 flafl-0.0.4/flafl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1110 2020-09-15 22:57:52.000000 flafl-0.0.4/flafl/helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)     2635 2020-09-15 22:57:52.000000 flafl-0.0.4/flafl/jsonparser.py
--rw-r--r--   0 runner    (1001) docker     (116)     7568 2020-09-15 22:57:52.000000 flafl-0.0.4/flafl/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-15 22:57:59.365483 flafl-0.0.4/flafl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5582 2020-09-15 22:57:59.000000 flafl-0.0.4/flafl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      297 2020-09-15 22:57:59.000000 flafl-0.0.4/flafl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-09-15 22:57:59.000000 flafl-0.0.4/flafl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2020-09-15 22:57:59.000000 flafl-0.0.4/flafl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2020-09-15 22:57:59.000000 flafl-0.0.4/flafl.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (116)     1576 2020-09-15 22:57:52.000000 flafl-0.0.4/flafld
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-09-15 22:57:59.369483 flafl-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      722 2020-09-15 22:57:52.000000 flafl-0.0.4/setup.py
+-rw-r--r--   0        0        0    11339 2023-05-15 22:02:04.248307 flafl-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4388 2023-05-15 22:02:04.248307 flafl-0.0.6/README.md
+-rw-r--r--   0        0        0     4461 2023-05-15 22:02:04.248307 flafl-0.0.6/flafl/__init__.py
+-rw-r--r--   0        0        0      998 2023-05-15 22:02:04.248307 flafl-0.0.6/flafl/bamboo.py
+-rw-r--r--   0        0        0      459 2023-05-15 22:02:04.248307 flafl-0.0.6/flafl/context.py
+-rw-r--r--   0        0        0      507 2023-05-15 22:02:04.248307 flafl-0.0.6/flafl/exceptions.py
+-rw-r--r--   0        0        0     1110 2023-05-15 22:02:04.248307 flafl-0.0.6/flafl/helpers.py
+-rw-r--r--   0        0        0     2635 2023-05-15 22:02:04.248307 flafl-0.0.6/flafl/jsonparser.py
+-rw-r--r--   0        0        0     7565 2023-05-15 22:02:04.248307 flafl-0.0.6/flafl/strategies.py
+-rw-r--r--   0        0        0     1036 2023-05-15 22:02:04.248307 flafl-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5487 1970-01-01 00:00:00.000000 flafl-0.0.6/PKG-INFO
```

### Comparing `flafl-0.0.4/PKG-INFO` & `flafl-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,155 +1,170 @@
 Metadata-Version: 2.1
 Name: flafl
-Version: 0.0.4
-Summary: Flask application for listening to Bitbucket webhooks
+Version: 0.0.6
+Summary: Flask application for listening to webhooks
 Home-page: https://github.com/msleigh/flafl
-Author: M Sleigh
-Author-email: author@example.com
-License: UNKNOWN
-Description: # FLAFL
-        
-        <h2 align="center">Flask Application For Listening...</h2>
-        
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
-        
-        Listens for events triggered by Webhooks in an Atlassian Bitbucket
-        server and responds.
-        
-        It assumes the main purpose is to trigger test plans in an associated Bamboo instance, but can be persuaded to take other actions.
-        
-        ---
-        
-        ## Requirements
-        
-        - User must have a netrc file containing valid login details for the Bamboo
-          hostname used
-        
-        ## Installation
-        
-            git clone .../flafl.git
-            cd flafl
-            python3 -m venv /path/to/virtual/environment
-            source /path/to/virtual/environment/bin/activate
-            pip3 install -r requirements.txt
-        
-        ## Local configuration
-        
-        Export the following variables with the correct information:
-        
-            export NETRC_FILE="/path/to/netrc/file"
-            export BAMB_HOSTNAME="bamboo.yourorg.com"
-            export BITB_HOSTNAME="bitbucket.yourorg.com"
-        
-        To run the tests (see below), these environment variables must be defined,
-        but do not need to have the correct values.
-        
-            export BITB_PROJECT="test"
-            export BITB_REPO="test"
-        
-        ## Tests
-        
-        To check set-up, run:
-        
-            python3 -m pytest
-        
-        or to get test-coverage information run:
-        
-            coverage run -m pytest
-        
-        which allows a test-coverage report to be produced:
-        
-            coverage report
-        
-        or as a web page:
-        
-            coverage html
-            xdg-open htmlcov/index.html
-        
-        ## Usage
-        
-        The main application runs as a background service.
-        
-        In the `flafl` directory run:
-        
-            ./flafld <command>
-        
-        to control the service. Specifically:
-        
-        - `flafld start` or `flafld run` start the service in the background, recording
-          the process ID to `${TMP:-/tmp}/.flafl.pid`
-        - `flafld stop` stops the process (and its children)
-        - `flafld restart` stops the running service and starts it again
-        
-        On starting the service, the port number of the Flask application is printed. Make a
-        note of this for use in setting webhooks up in Bitbucket.
-        
-        ## Bitbucket configuration
-        
-        In a browser, go to the webhook set-up page of your repository in your Bitbucket server:
-        
-            https://<bitbucket.yourorg.com>/plugins/servlet/webhooks/projects/<project>/repos/<repo>
-        
-        Create webhook by clicking "Create webhook", giving it a name (e.g. "flafl"),
-        and specifying the URL of your running FLAFL application, e.g.:
-        
-            https://<flafl-app-host.yourorg.com>:8080/flafl/api/v1.0/events
-        
-        No "Secret" is required. Click "Test connection", and you should get a return
-        code of "200", and in "View details", the body of the response from the
-        applications should be:
-        
-            {
-              "debug_info": {
-                "payloadReceived": {
-                  "test": true
-                }
-              }, 
-              "message": "Successful connection."
-            }
-        
-        Now select which events should send webhooks to the app. Under the
-        "Repository" column, the following webhooks, if selected, will trigger a respose:
-        
-        - Push
-        
-        and under the "Pull request" column, the following:
-        
-        - Opened
-        - Modified
-        - Merged
-        - Declined
-        - Deleted
-        - Comment added
-        
-        Others will be quietly ignored. FLAFL can easily be extended to add responses
-        to other tiggers of interest.
-        
-        Click "Save".
-        
-        To test the Bitbucket configuration, create a new pull request (the target
-        branch must be within the repository that has the webhooks; the source branch
-        can be outside, e.g. in a fork).
-        
-        In the directory containing the FLAFL application code, a log file should have been
-        created with some diagnostic output, e.g.:
-        
-            2019-12-17 17:18:54.360661
-            Success payload:
-            {
-                "message": "Created PR with ID 321 from project/repo/feature-branch to project/repo/develop. Sent API call to Bamboo and got return code 204",
-                "status": "success"
-            }
-        
-        Also, the application should have automatically added a comment to the PR
-        asking the PR author to add a Jira ticket ID to the PR title. This is an
-        example of the kind of checks the application can perform.
-        
-        Adding a comment to the PR, and deleting or declining the PR, should also add
-        similar diagnostic output to the `flafl.log` file.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+License: Apache-2.0
+Author: msleigh
+Author-email: msleigh@noreply.users.github.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: Flask (>=2.3.2,<3.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Project-URL: Bug Tracker, https://github.com/msleigh/flafl/issues
+Project-URL: CI, https://github.com/msleigh/flafl/actions
+Project-URL: Changelog, https://github.com/msleigh/flafl/releases
 Description-Content-Type: text/markdown
+
+# FLAFL
+
+<h2 align="center">Flask Application For Listening...</h2>
+
+[![PyPI](https://img.shields.io/pypi/v/flafl.svg)](https://pypi.org/project/flafl/)
+[![Changelog](https://img.shields.io/github/v/release/msleigh/flafl?include_prereleases&label=changelog)](https://github.com/msleigh/flafl/releases)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/msleigh/flafl/blob/main/LICENSE)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+
+Listens for events triggered by Webhooks in an Atlassian Bitbucket
+server and responds.
+
+It assumes the main purpose is to trigger test plans in an associated Bamboo instance, but can be persuaded to take other actions.
+
+---
+
+## Requirements
+
+FLAFL requires Python 3.7+. It is tested on Linux and macOS.
+
+You  must have a netrc file containing valid login details for the Bamboo hostname used.
+
+## Installation
+
+FLAFL is published as a Python package and can be installed with `pip`, ideally by using a virtual environment. Open up a terminal and install with:
+
+    pip install flafl
+
+## Configuration
+
+Export the following variables with the correct information:
+
+    export NETRC_FILE="/path/to/netrc/file"
+    export BAMB_HOSTNAME="bamboo.yourorg.com"
+    export BITB_HOSTNAME="bitbucket.yourorg.com"
+
+To run the tests (see below), these environment variables must be defined,
+but do not need to have the correct values.
+
+    export BITB_PROJECT="test"
+    export BITB_REPO="test"
+
+## Tests
+
+To check set-up, run:
+
+    python3 -m pytest
+
+or to get test-coverage information run:
+
+    coverage run -m pytest
+
+which allows a test-coverage report to be produced:
+
+    coverage report
+
+or as a web page:
+
+    coverage html
+    xdg-open htmlcov/index.html
+
+## Usage
+
+The main application runs as a background service.
+
+In the `flafl` directory run:
+
+    ./flafld <command>
+
+to control the service. Specifically:
+
+- `flafld start` or `flafld run` start the service in the background, recording
+  the process ID to `${TMP:-/tmp}/.flafl.pid`
+- `flafld stop` stops the process (and its children)
+- `flafld restart` stops the running service and starts it again
+
+On starting the service, the port number of the Flask application is printed. Make a
+note of this for use in setting webhooks up in Bitbucket.
+
+## Bitbucket configuration
+
+In a browser, go to the webhook set-up page of your repository in your Bitbucket server:
+
+    https://<bitbucket.yourorg.com>/plugins/servlet/webhooks/projects/<project>/repos/<repo>
+
+Create webhook by clicking "Create webhook", giving it a name (e.g. "flafl"),
+and specifying the URL of your running FLAFL application, e.g.:
+
+    https://<flafl-app-host.yourorg.com>:8080/flafl/api/v1.0/events
+
+No "Secret" is required. Click "Test connection", and you should get a return
+code of "200", and in "View details", the body of the response from the
+applications should be:
+
+    {
+      "debug_info": {
+        "payloadReceived": {
+          "test": true
+        }
+      },
+      "message": "Successful connection."
+    }
+
+Now select which events should send webhooks to the app. Under the
+"Repository" column, the following webhooks, if selected, will trigger a respose:
+
+- Push
+
+and under the "Pull request" column, the following:
+
+- Opened
+- Modified
+- Merged
+- Declined
+- Deleted
+- Comment added
+
+Others will be quietly ignored. FLAFL can easily be extended to add responses
+to other tiggers of interest.
+
+Click "Save".
+
+To test the Bitbucket configuration, create a new pull request (the target
+branch must be within the repository that has the webhooks; the source branch
+can be outside, e.g. in a fork).
+
+In the directory containing the FLAFL application code, a log file should have been
+created with some diagnostic output, e.g.:
+
+    2019-12-17 17:18:54.360661
+    Success payload:
+    {
+        "message": "Created PR with ID 321 from project/repo/feature-branch to project/repo/develop. Sent API call to Bamboo and got return code 204",
+        "status": "success"
+    }
+
+Also, the application should have automatically added a comment to the PR
+asking the PR author to add a Jira ticket ID to the PR title. This is an
+example of the kind of checks the application can perform.
+
+Adding a comment to the PR, and deleting or declining the PR, should also add
+similar diagnostic output to the `flafl.log` file.
+
```

### Comparing `flafl-0.0.4/README.md` & `flafl-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # FLAFL
 
 <h2 align="center">Flask Application For Listening...</h2>
 
+[![PyPI](https://img.shields.io/pypi/v/flafl.svg)](https://pypi.org/project/flafl/)
+[![Changelog](https://img.shields.io/github/v/release/msleigh/flafl?include_prereleases&label=changelog)](https://github.com/msleigh/flafl/releases)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/msleigh/flafl/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 
 Listens for events triggered by Webhooks in an Atlassian Bitbucket
 server and responds.
 
 It assumes the main purpose is to trigger test plans in an associated Bamboo instance, but can be persuaded to take other actions.
 
 ---
 
 ## Requirements
 
-- User must have a netrc file containing valid login details for the Bamboo
-  hostname used
+FLAFL requires Python 3.7+. It is tested on Linux and macOS.
+
+You  must have a netrc file containing valid login details for the Bamboo hostname used.
 
 ## Installation
 
-    git clone .../flafl.git
-    cd flafl
-    python3 -m venv /path/to/virtual/environment
-    source /path/to/virtual/environment/bin/activate
-    pip3 install -r requirements.txt
+FLAFL is published as a Python package and can be installed with `pip`, ideally by using a virtual environment. Open up a terminal and install with:
+
+    pip install flafl
 
-## Local configuration
+## Configuration
 
 Export the following variables with the correct information:
 
     export NETRC_FILE="/path/to/netrc/file"
     export BAMB_HOSTNAME="bamboo.yourorg.com"
     export BITB_HOSTNAME="bitbucket.yourorg.com"
 
@@ -91,15 +93,15 @@
 applications should be:
 
     {
       "debug_info": {
         "payloadReceived": {
           "test": true
         }
-      }, 
+      },
       "message": "Successful connection."
     }
 
 Now select which events should send webhooks to the app. Under the
 "Repository" column, the following webhooks, if selected, will trigger a respose:
 
 - Push
```

### Comparing `flafl-0.0.4/flafl/__init__.py` & `flafl-0.0.6/flafl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,14 @@
     response = jsonify(error.to_dict())
     response.status_code = error.status_code
     return response
 
 
 @app.route("/flafl/api/v1.0/events", methods=["POST"])
 def post_event():
-
     debug_info = {}
     debug_info["payloadReceived"] = request.json
 
     # Verbose
     # helpers.log(json.dumps(request.json, sort_keys=True, indent=4))
 
     # For 'Test Connection' function in Bamboo webhook settings
@@ -100,15 +99,14 @@
     event_key, event_trigger = jsonparser.get_event_key(request.json, debug_info)
 
     debug_info["eventKey"] = event_key
     debug_info["eventTrigger"] = event_trigger
 
     # Select the appropriate strategy
     if event_key.startswith("pr:"):
-
         if event_trigger == "opened":
             concrete_strategy = strategies.PrCreate()
 
         if event_trigger == "deleted":
             concrete_strategy = strategies.PrDestroy()
 
         if event_trigger == "merged":
@@ -120,15 +118,14 @@
         if event_trigger == "modified":
             concrete_strategy = strategies.PrModify()
 
         if event_trigger == "comment":
             concrete_strategy = strategies.PrComment()
 
     if event_key.startswith("repo:"):
-
         if event_trigger == "refs_changed":
             concrete_strategy = strategies.RepoPush()
 
         else:
             concrete_strategy = strategies.RepoAll()
 
     # Execute the strategy
```

### Comparing `flafl-0.0.4/flafl/bamboo.py` & `flafl-0.0.6/flafl/bamboo.py`

 * *Files identical despite different names*

### Comparing `flafl-0.0.4/flafl/helpers.py` & `flafl-0.0.6/flafl/helpers.py`

 * *Files identical despite different names*

### Comparing `flafl-0.0.4/flafl/jsonparser.py` & `flafl-0.0.6/flafl/jsonparser.py`

 * *Files identical despite different names*

### Comparing `flafl-0.0.4/flafl/strategies.py` & `flafl-0.0.6/flafl/strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
         pass
 
 
 class PrCreate(Strategy):
     """Class for pull-request creation response."""
 
     def execute(self, json_data, debug_info, conns):
-
         jsonparser.verify_pull_request_id(json_data, debug_info)
 
         # Get the required info from the PR webhook payload
         pull_request_id = json_data["pullRequest"]["id"]
         pull_request_title = json_data["pullRequest"]["title"]
         to_ref_slug = json_data["pullRequest"]["toRef"]["repository"]["slug"]
         to_ref_proj = json_data["pullRequest"]["toRef"]["repository"]["project"]["key"]
@@ -100,15 +99,14 @@
         return jsonify({"message": message, "status": "success"})
 
 
 class PrDestroy(Strategy):
     """Class for pull-request closure response."""
 
     def execute(self, json_data, debug_info, conns):
-
         jsonparser.verify_pull_request_id(json_data, debug_info)
 
         message = (
             "Destroyed PR with ID "
             + str(json_data["pullRequest"]["id"])
             + " in repository "
             + json_data["pullRequest"]["fromRef"]["repository"]["project"]["key"]
@@ -118,15 +116,14 @@
         return jsonify({"message": message, "status": "success"})
 
 
 class PrModify(Strategy):
     """Class for pull-request modification response."""
 
     def execute(self, json_data, debug_info, conns):
-
         jsonparser.verify_pull_request_id(json_data, debug_info)
 
         pull_request_id = json_data["pullRequest"]["id"]
         pull_request_title = json_data["pullRequest"]["title"]
         to_ref_slug = json_data["pullRequest"]["toRef"]["repository"]["slug"]
         to_ref_proj = json_data["pullRequest"]["toRef"]["repository"]["project"]["key"]
```

