# Comparing `tmp/slack_approval-0.1.1.tar.gz` & `tmp/slack_approval-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack_approval-0.1.1.tar", last modified: Mon Mar  6 17:18:46 2023, max compression
+gzip compressed data, was "slack_approval-0.1.2.tar", last modified: Tue May 16 17:38:19 2023, max compression
```

## Comparing `slack_approval-0.1.1.tar` & `slack_approval-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2023-03-06 17:18:46.435864 slack_approval-0.1.1/
--rw-r--r--   0 austennovis   (501) staff       (20)     4929 2023-03-06 17:18:46.435524 slack_approval-0.1.1/PKG-INFO
--rw-r--r--   0 austennovis   (501) staff       (20)     4079 2023-03-06 17:18:26.000000 slack_approval-0.1.1/README.md
--rw-r--r--   0 austennovis   (501) staff       (20)       38 2023-03-06 17:18:46.435978 slack_approval-0.1.1/setup.cfg
--rw-r--r--   0 austennovis   (501) staff       (20)     2826 2023-03-06 17:18:26.000000 slack_approval-0.1.1/setup.py
-drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2023-03-06 17:18:46.432231 slack_approval-0.1.1/slack_approval/
--rw-r--r--   0 austennovis   (501) staff       (20)        0 2022-12-12 16:40:33.000000 slack_approval-0.1.1/slack_approval/__init__.py
--rw-r--r--   0 austennovis   (501) staff       (20)      293 2022-12-12 16:40:33.000000 slack_approval-0.1.1/slack_approval/cli.py
--rw-r--r--   0 austennovis   (501) staff       (20)     3881 2022-12-12 16:40:33.000000 slack_approval-0.1.1/slack_approval/slack_provision.py
--rw-r--r--   0 austennovis   (501) staff       (20)     4422 2023-03-06 17:18:26.000000 slack_approval-0.1.1/slack_approval/slack_request.py
-drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2023-03-06 17:18:46.434960 slack_approval-0.1.1/slack_approval.egg-info/
--rw-r--r--   0 austennovis   (501) staff       (20)     4929 2023-03-06 17:18:45.000000 slack_approval-0.1.1/slack_approval.egg-info/PKG-INFO
--rw-r--r--   0 austennovis   (501) staff       (20)      363 2023-03-06 17:18:46.000000 slack_approval-0.1.1/slack_approval.egg-info/SOURCES.txt
--rw-r--r--   0 austennovis   (501) staff       (20)        1 2023-03-06 17:18:45.000000 slack_approval-0.1.1/slack_approval.egg-info/dependency_links.txt
--rw-r--r--   0 austennovis   (501) staff       (20)       59 2023-03-06 17:18:46.000000 slack_approval-0.1.1/slack_approval.egg-info/entry_points.txt
--rw-r--r--   0 austennovis   (501) staff       (20)       36 2023-03-06 17:18:46.000000 slack_approval-0.1.1/slack_approval.egg-info/requires.txt
--rw-r--r--   0 austennovis   (501) staff       (20)       15 2023-03-06 17:18:46.000000 slack_approval-0.1.1/slack_approval.egg-info/top_level.txt
+drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-16 17:38:19.532882 slack_approval-0.1.2/
+-rw-r--r--   0 austen.novis   (502) staff       (20)     4910 2023-05-16 17:38:19.532754 slack_approval-0.1.2/PKG-INFO
+-rw-r--r--   0 austen.novis   (502) staff       (20)     4079 2023-05-16 17:36:53.000000 slack_approval-0.1.2/README.md
+-rw-r--r--   0 austen.novis   (502) staff       (20)       38 2023-05-16 17:38:19.532934 slack_approval-0.1.2/setup.cfg
+-rw-r--r--   0 austen.novis   (502) staff       (20)     2826 2023-05-16 17:38:16.000000 slack_approval-0.1.2/setup.py
+drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-16 17:38:19.531652 slack_approval-0.1.2/slack_approval/
+-rw-r--r--   0 austen.novis   (502) staff       (20)        0 2023-05-16 17:36:53.000000 slack_approval-0.1.2/slack_approval/__init__.py
+-rw-r--r--   0 austen.novis   (502) staff       (20)      293 2023-05-16 17:36:53.000000 slack_approval-0.1.2/slack_approval/cli.py
+-rw-r--r--   0 austen.novis   (502) staff       (20)     3881 2023-05-16 17:36:53.000000 slack_approval-0.1.2/slack_approval/slack_provision.py
+-rw-r--r--   0 austen.novis   (502) staff       (20)     4430 2023-05-16 17:36:53.000000 slack_approval-0.1.2/slack_approval/slack_request.py
+drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-16 17:38:19.532552 slack_approval-0.1.2/slack_approval.egg-info/
+-rw-r--r--   0 austen.novis   (502) staff       (20)     4910 2023-05-16 17:38:19.000000 slack_approval-0.1.2/slack_approval.egg-info/PKG-INFO
+-rw-r--r--   0 austen.novis   (502) staff       (20)      363 2023-05-16 17:38:19.000000 slack_approval-0.1.2/slack_approval.egg-info/SOURCES.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)        1 2023-05-16 17:38:19.000000 slack_approval-0.1.2/slack_approval.egg-info/dependency_links.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)       59 2023-05-16 17:38:19.000000 slack_approval-0.1.2/slack_approval.egg-info/entry_points.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)       36 2023-05-16 17:38:19.000000 slack_approval-0.1.2/slack_approval.egg-info/requires.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)       15 2023-05-16 17:38:19.000000 slack_approval-0.1.2/slack_approval.egg-info/top_level.txt
```

### Comparing `slack_approval-0.1.1/PKG-INFO` & `slack_approval-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: slack_approval
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library for managing and deploying a lightweight approval workflow based on Slack and GCP
 Home-page: https://github.com/premisedata/slack-approval
 Author: Austen
 Author-email: austen.novis@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -104,8 +103,7 @@
 * `goblet deploy --stage request` 
 
 * `goblet deploy --stage provision`
 
 ## Blog post
 ____________
 See the blog post [Tutorial: Setting Up Approval Processes with Slack Apps](https://engineering.premise.com/tutorial-setting-up-approval-processes-with-slack-apps-d325aee31763) for more detailed slack and GCP setup steps.
-
```

### Comparing `slack_approval-0.1.1/README.md` & `slack_approval-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `slack_approval-0.1.1/setup.py` & `slack_approval-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    version="0.1.1",
+    version="0.1.2",
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

### Comparing `slack_approval-0.1.1/slack_approval/slack_provision.py` & `slack_approval-0.1.2/slack_approval/slack_provision.py`

 * *Files identical despite different names*

### Comparing `slack_approval-0.1.1/slack_approval/slack_request.py` & `slack_approval-0.1.2/slack_approval/slack_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class SlackRequest:
     def __init__(self, request):
         """requesters_channel only necessary for `pending` messages
         """
         self.inputs = request.json
         self.name = self.inputs["provision_class"]
-        self.value = self.inputs # save inputs before hiding anything
+        self.value = self.inputs.copy() # save inputs before hiding anything
         hide = self.inputs.get("hide")
         if hide:
             logger.info(f"Hidden fields: {hide}")
             for field in hide:
                 self.inputs.pop(field)
             self.inputs.pop("hide")
         self.token = os.environ.get("SLACK_BOT_TOKEN")
@@ -111,8 +111,8 @@
         # Send to approvers channel with `approve` and `reject` buttons
         try:
             response = slack_web_client.chat_postMessage(
                 channel=self.approvers_channel, text="fallback", blocks=blocks
             )
             logger.info(response.status_code)
         except errors.SlackApiError as e:
-            logger.error(e)
+            logger.error(e)
```

### Comparing `slack_approval-0.1.1/slack_approval.egg-info/PKG-INFO` & `slack_approval-0.1.2/slack_approval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: slack-approval
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library for managing and deploying a lightweight approval workflow based on Slack and GCP
 Home-page: https://github.com/premisedata/slack-approval
 Author: Austen
 Author-email: austen.novis@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -104,8 +103,7 @@
 * `goblet deploy --stage request` 
 
 * `goblet deploy --stage provision`
 
 ## Blog post
 ____________
 See the blog post [Tutorial: Setting Up Approval Processes with Slack Apps](https://engineering.premise.com/tutorial-setting-up-approval-processes-with-slack-apps-d325aee31763) for more detailed slack and GCP setup steps.
-
```

