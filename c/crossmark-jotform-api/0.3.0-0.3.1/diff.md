# Comparing `tmp/crossmark-jotform-api-0.3.0.tar.gz` & `tmp/crossmark-jotform-api-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossmark-jotform-api-0.3.0.tar", last modified: Tue May 16 17:58:31 2023, max compression
+gzip compressed data, was "crossmark-jotform-api-0.3.1.tar", last modified: Tue May 16 18:36:04 2023, max compression
```

## Comparing `crossmark-jotform-api-0.3.0.tar` & `crossmark-jotform-api-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 17:58:31.350073 crossmark-jotform-api-0.3.0/
--rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     2630 2023-05-16 17:58:31.349076 crossmark-jotform-api-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      730 2023-05-16 17:57:54.000000 crossmark-jotform-api-0.3.0/README.md
--rw-rw-rw-   0        0        0      789 2023-05-16 17:57:19.000000 crossmark-jotform-api-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 17:58:31.350073 crossmark-jotform-api-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 17:58:31.310074 crossmark-jotform-api-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 17:58:31.323075 crossmark-jotform-api-0.3.0/src/crossmark_jotform_api/
--rw-rw-rw-   0        0        0    12830 2023-05-16 17:56:23.000000 crossmark-jotform-api-0.3.0/src/crossmark_jotform_api/jotForm.py
-drwxrwxrwx   0        0        0        0 2023-05-16 17:58:31.342080 crossmark-jotform-api-0.3.0/src/crossmark_jotform_api.egg-info/
--rw-rw-rw-   0        0        0     2630 2023-05-16 17:58:31.000000 crossmark-jotform-api-0.3.0/src/crossmark_jotform_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-16 17:58:31.000000 crossmark-jotform-api-0.3.0/src/crossmark_jotform_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 17:58:31.000000 crossmark-jotform-api-0.3.0/src/crossmark_jotform_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-16 17:58:31.000000 crossmark-jotform-api-0.3.0/src/crossmark_jotform_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 17:58:31.348073 crossmark-jotform-api-0.3.0/test/
--rw-rw-rw-   0        0        0      270 2023-05-10 23:06:10.000000 crossmark-jotform-api-0.3.0/test/test_jotform_class.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:36:04.826363 crossmark-jotform-api-0.3.1/
+-rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     2770 2023-05-16 18:36:04.825364 crossmark-jotform-api-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      870 2023-05-16 18:35:40.000000 crossmark-jotform-api-0.3.1/README.md
+-rw-rw-rw-   0        0        0      789 2023-05-16 18:34:10.000000 crossmark-jotform-api-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 18:36:04.826363 crossmark-jotform-api-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 18:36:04.795361 crossmark-jotform-api-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 18:36:04.806360 crossmark-jotform-api-0.3.1/src/crossmark_jotform_api/
+-rw-rw-rw-   0        0        0    12969 2023-05-16 18:34:02.000000 crossmark-jotform-api-0.3.1/src/crossmark_jotform_api/jotForm.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:36:04.823363 crossmark-jotform-api-0.3.1/src/crossmark_jotform_api.egg-info/
+-rw-rw-rw-   0        0        0     2770 2023-05-16 18:36:04.000000 crossmark-jotform-api-0.3.1/src/crossmark_jotform_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-16 18:36:04.000000 crossmark-jotform-api-0.3.1/src/crossmark_jotform_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 18:36:04.000000 crossmark-jotform-api-0.3.1/src/crossmark_jotform_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-16 18:36:04.000000 crossmark-jotform-api-0.3.1/src/crossmark_jotform_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 18:36:04.824361 crossmark-jotform-api-0.3.1/test/
+-rw-rw-rw-   0        0        0      270 2023-05-10 23:06:10.000000 crossmark-jotform-api-0.3.1/test/test_jotform_class.py
```

### Comparing `crossmark-jotform-api-0.3.0/LICENSE` & `crossmark-jotform-api-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.3.0/PKG-INFO` & `crossmark-jotform-api-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.3.0
+Version: 0.3.1
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -41,7 +41,8 @@
 
 ## updates
 - 2023-04-26: added `set_new_submission` function, time to time it cannot find the submission, in that cases pulls the data directly from the api and sets as it is.
 - 2023-05-01: added a logic for get_emails function. and added a TODO there.
 - 2023-05-01: setted set_answer function.
 - 2023-05-10: deleted submissions array and enhanced the logic according to it
 - 2023-05-16: created emails on class initilaization so that one dont need to call get_emails function
+- 2023-05-16: summary for get_form function, format document, cleared some of the self.update and its fucntionality for faster performance
```

### Comparing `crossmark-jotform-api-0.3.0/pyproject.toml` & `crossmark-jotform-api-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests>=2.22.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crossmark-jotform-api"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Renas Mirkan Kilic", email="mirkanbaba1@gmail.com" },
 ]
 description = "Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `crossmark-jotform-api-0.3.0/src/crossmark_jotform_api/jotForm.py` & `crossmark-jotform-api-0.3.1/src/crossmark_jotform_api/jotForm.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
         self.url = "https://api.jotform.com/form/" + form_id + \
             "/submissions?limit=1000&apiKey=" + api_key
         self.set_url_param("offset", "0")
         self.submission_ids = set()
         self.submission_data = {}
         self.updating_process = False
         self.submission_count = 0
-        self.submissions = (lambda: [i.to_dict() for k,i in self.submission_data.items()])
+        self.submissions = (lambda: [i.to_dict()
+                            for k, i in self.submission_data.items()])
         self.timeout = timeout
         self.debug = debug
         self.set_data()
 
     def __print(self, text):
         if self.debug:
             print(text)
@@ -36,47 +37,43 @@
 
     def __set_submission_ids(self):
         """This function sets the submission memory. It is used for easier for loop for submissions. 
         It is called in the constructor, and time to time in other functions"""
         self.submission_ids = set()
         for key, value in self.submission_data.items():
             self.submission_ids.add(value.id)
-    
+
     def set_submission_count(self):
         self.submission_count = len(self.submission_ids)
 
     def get_submission_data(self):
         self.update()
         return self.submission_data
 
     def get_submission_count(self):
-        self.update()
         return self.submission_count
 
     def get_submission_answers(self, submission_id):
         self.update()
         return self.submission_data[submission_id].answers
 
     def get_submission_by_request(self, submission_id):
         requests.get("https://api.jotform.com/submission/" +
                      submission_id + "?apiKey=" + self.api_key, timeout=self.timeout)
 
     def get_submission(self, submission_id):
-        self.update()
         return self.submission_data[submission_id]
 
     def get_submission_id_by_text(self, text):
-        self.update()
         for key, submission_object in self.submission_data.items():
             if submission_object.get_answer_by_text(text):
                 return submission_object
         return None
 
     def get_submission_by_case_id(self, case_id, tried=0):
-        self.update()
         for key, submission_object in self.submission_data.items():
             if submission_object.case_id == case_id:
                 return submission_object
         if not tried:
             self.request_submission_by_case_id(case_id)
             return self.get_submission_by_case_id(case_id, 1)
         return None
@@ -105,15 +102,14 @@
         self.update()
         submission_answers = self.get_submission_answers(submission_id)
         submission_answers_by_question_id = {}
         for answer in submission_answers:
             submission_answers_by_question_id[answer["id"]] = answer["answer"]
 
     def update_submission_answer(self, submission_id, answer_id, answer):
-        self.update()
         query = f'submission[{answer_id}]={answer}'
         url = f"https://api.jotform.com/submission/{submission_id}?apiKey={self.api_key}&{query}"
         response = requests.request("POST", url, timeout=self.timeout)
         if response.status_code == 200:
             self.submission_data[submission_id].set_answer(answer_id, answer)
             return True
         else:
@@ -177,38 +173,44 @@
             self.__set_get_submission_data(
                 [submission]
             )
         )
         self.set_global_data()
 
     def get_form(self):
+        """
+        Gets form data directly from Jotform so there is no data diffirence on this function.
+        It is slow since we are requesting data from Jotform.
+
+        Returns:
+            _type_: either JSON or None
+        """
         url = f"https://api.jotform.com/form/{self.form_id}?apiKey={self.api_key}"
         response = requests.request("GET", url, timeout=self.timeout)
         if response.status_code == 200:
             return response.json()
         else:
             return None
 
     def get_submissions_count(self):
         form = self.get_form()
         if form:
-            return form['content']['count']
+            return int(form['content']['count'])
 
     def update(self):
-        form = self.get_form()
-        if not self.updating_process and form:
+        if not self.updating_process:
             self.updating_process = True
-            count = int(form['content']['count'])
+            count = self.get_submissions_count()
             if count <= self.submission_count:
                 self.__print("[INFO] No new submissions.")
             else:
                 now = datetime.now().timestamp()
                 its_been = now - self.update_timestamp
                 self.__print(
-                    f"[INFO] Its been {int(its_been/60)} minutes. Updating submission data...")
+                    f"[INFO] Its been {int(its_been/60)} minutes since last update. Updating submission data...")
                 self.set_data()
                 self.update_timestamp = now
             self.updating_process = False
 
 
 class JotFormSubmission(ABC):
     def __init__(self, submission_object):
@@ -265,15 +267,15 @@
                 'type': _type,
                 'text': text,
                 'file': file,
                 'selectedFields': selectedFields
             })
         return answers_arr
 
-    def set_answer(self, answer_id:str, answer_value:str):
+    def set_answer(self, answer_id: str, answer_value: str):
         for i in range(len(self.answers_arr)):
             if self.answers_arr[i]['key'] == answer_id:
                 self.answers_arr[i]['answer'] = answer_value
         self.answers[answer_id]['answer'] = answer_value
 
     def get_answers(self):
         return self.answers_arr
```

### Comparing `crossmark-jotform-api-0.3.0/src/crossmark_jotform_api.egg-info/PKG-INFO` & `crossmark-jotform-api-0.3.1/src/crossmark_jotform_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.3.0
+Version: 0.3.1
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -41,7 +41,8 @@
 
 ## updates
 - 2023-04-26: added `set_new_submission` function, time to time it cannot find the submission, in that cases pulls the data directly from the api and sets as it is.
 - 2023-05-01: added a logic for get_emails function. and added a TODO there.
 - 2023-05-01: setted set_answer function.
 - 2023-05-10: deleted submissions array and enhanced the logic according to it
 - 2023-05-16: created emails on class initilaization so that one dont need to call get_emails function
+- 2023-05-16: summary for get_form function, format document, cleared some of the self.update and its fucntionality for faster performance
```

