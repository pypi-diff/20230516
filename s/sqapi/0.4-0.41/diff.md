# Comparing `tmp/sqapi-0.4.tar.gz` & `tmp/sqapi-0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqapi-0.4.tar", last modified: Wed May 10 02:47:17 2023, max compression
+gzip compressed data, was "sqapi-0.41.tar", last modified: Tue May 16 04:25:47 2023, max compression
```

## Comparing `sqapi-0.4.tar` & `sqapi-0.41.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-05-10 02:47:17.233500 sqapi-0.4/
--rw-r--r--   0 ariell     (501) staff       (20)     1061 2023-05-10 02:42:34.000000 sqapi-0.4/LICENSE.txt
--rw-r--r--   0 ariell     (501) staff       (20)    10851 2023-05-10 02:47:17.233583 sqapi-0.4/PKG-INFO
--rw-r--r--   0 ariell     (501) staff       (20)     9824 2023-04-21 06:07:59.000000 sqapi-0.4/README.md
--rw-r--r--   0 ariell     (501) staff       (20)       79 2023-05-10 02:47:17.233832 sqapi-0.4/setup.cfg
--rw-r--r--   0 ariell     (501) staff       (20)     1786 2023-05-10 02:42:22.000000 sqapi-0.4/setup.py
-drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-05-10 02:47:17.232721 sqapi-0.4/sqapi/
--rw-r--r--   0 ariell     (501) staff       (20)        0 2023-04-06 00:14:19.000000 sqapi-0.4/sqapi/__init__.py
--rw-r--r--   0 ariell     (501) staff       (20)    12728 2023-05-10 02:42:22.000000 sqapi-0.4/sqapi/annotate.py
--rw-r--r--   0 ariell     (501) staff       (20)     4202 2023-04-07 04:44:10.000000 sqapi-0.4/sqapi/api.py
--rw-r--r--   0 ariell     (501) staff       (20)     4902 2023-04-18 01:29:24.000000 sqapi-0.4/sqapi/helpers.py
--rw-r--r--   0 ariell     (501) staff       (20)     1632 2022-05-09 04:38:36.000000 sqapi-0.4/sqapi/media.py
--rw-r--r--   0 ariell     (501) staff       (20)     7454 2023-04-06 07:30:14.000000 sqapi-0.4/sqapi/request.py
-drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-05-10 02:47:17.233399 sqapi-0.4/sqapi.egg-info/
--rw-r--r--   0 ariell     (501) staff       (20)    10851 2023-05-10 02:47:17.000000 sqapi-0.4/sqapi.egg-info/PKG-INFO
--rw-r--r--   0 ariell     (501) staff       (20)      282 2023-05-10 02:47:17.000000 sqapi-0.4/sqapi.egg-info/SOURCES.txt
--rw-r--r--   0 ariell     (501) staff       (20)        1 2023-05-10 02:47:17.000000 sqapi-0.4/sqapi.egg-info/dependency_links.txt
--rw-r--r--   0 ariell     (501) staff       (20)       29 2023-05-10 02:47:17.000000 sqapi-0.4/sqapi.egg-info/requires.txt
--rw-r--r--   0 ariell     (501) staff       (20)        6 2023-05-10 02:47:17.000000 sqapi-0.4/sqapi.egg-info/top_level.txt
+drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-05-16 04:25:47.372913 sqapi-0.41/
+-rw-r--r--   0 ariell     (501) staff       (20)     1061 2023-05-10 02:42:34.000000 sqapi-0.41/LICENSE.txt
+-rw-r--r--   0 ariell     (501) staff       (20)    11898 2023-05-16 04:25:47.372972 sqapi-0.41/PKG-INFO
+-rw-r--r--   0 ariell     (501) staff       (20)    10870 2023-05-16 04:05:23.000000 sqapi-0.41/README.md
+-rw-r--r--   0 ariell     (501) staff       (20)       79 2023-05-16 04:25:47.373233 sqapi-0.41/setup.cfg
+-rw-r--r--   0 ariell     (501) staff       (20)     1787 2023-05-16 04:22:00.000000 sqapi-0.41/setup.py
+drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-05-16 04:25:47.372210 sqapi-0.41/sqapi/
+-rw-r--r--   0 ariell     (501) staff       (20)        0 2023-04-06 00:14:19.000000 sqapi-0.41/sqapi/__init__.py
+-rw-r--r--   0 ariell     (501) staff       (20)    12728 2023-05-10 02:42:22.000000 sqapi-0.41/sqapi/annotate.py
+-rw-r--r--   0 ariell     (501) staff       (20)     4202 2023-04-07 04:44:10.000000 sqapi-0.41/sqapi/api.py
+-rw-r--r--   0 ariell     (501) staff       (20)     4930 2023-05-16 04:03:19.000000 sqapi-0.41/sqapi/helpers.py
+-rw-r--r--   0 ariell     (501) staff       (20)     1632 2022-05-09 04:38:36.000000 sqapi-0.41/sqapi/media.py
+-rw-r--r--   0 ariell     (501) staff       (20)     7454 2023-04-06 07:30:14.000000 sqapi-0.41/sqapi/request.py
+drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-05-16 04:25:47.372825 sqapi-0.41/sqapi.egg-info/
+-rw-r--r--   0 ariell     (501) staff       (20)    11898 2023-05-16 04:25:47.000000 sqapi-0.41/sqapi.egg-info/PKG-INFO
+-rw-r--r--   0 ariell     (501) staff       (20)      282 2023-05-16 04:25:47.000000 sqapi-0.41/sqapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ariell     (501) staff       (20)        1 2023-05-16 04:25:47.000000 sqapi-0.41/sqapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ariell     (501) staff       (20)       29 2023-05-16 04:25:47.000000 sqapi-0.41/sqapi.egg-info/requires.txt
+-rw-r--r--   0 ariell     (501) staff       (20)        6 2023-05-16 04:25:47.000000 sqapi-0.41/sqapi.egg-info/top_level.txt
```

### Comparing `sqapi-0.4/LICENSE.txt` & `sqapi-0.41/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqapi-0.4/PKG-INFO` & `sqapi-0.41/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqapi
-Version: 0.4
+Version: 0.41
 Summary: A python package that simplifies interactions with the SQUIDLE+ API. It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.
 Home-page: https://bitbucket.org/ariell/pysq
 Download-URL: https://bitbucket.org/ariell/pysq/get/bede6badfc1ea09cd45b3ae3d4bc3551daa0b3e0.tar.gz
 Author: Greybits Engineering
 License: MIT
 Keywords: SQUIDLE+,API,SQ,Machine Learning
 Classifier: Development Status :: 3 - Alpha
@@ -67,27 +67,26 @@
 > need to activate your API key.
 
 ## Examples
 ### Creating queries
 This is by no means an extensive list of possible API queries. The API is extensive and the models are documented
 [here](https://squidle.org/api/help?template=api_help_page.html) and the creation of queries is documented 
 [here](https://squidle.org/api/help?template=api_help_page.html#api_query). `SQAPI` enables a convenient mechanism 
-for creating these queries inside of Python. For example, a basic API query to list the 
-
-`# /api/annotation?template=models/annotation/list_thumbnails.html&q={"filters":[{"name":"point","op":"has","val":{"name":"has_xy","op":"eq","val":true}},{"name":"point","op":"has","val":{"name":"media","op":"has","val":{"name":"poses","op":"any","val":{"name":"geom","op":"geo_in_bbox","val":[{"lat":-32.020013585799155,"lon":115.49980113118502},{"lat":-32.01995006531625,"lon":115.49987604949759}]}}}}]}`
+for creating these queries inside of Python. For example, a basic API query to list all the annotations that have valid 
+labels starting with 'ecklonia' within a spatially constrained bounding box would be:
 ```json
 {
    "filters": [
       {
-         "name": "point",
+         "name": "label",
          "op": "has",
          "val": {
-            "name": "has_xy",
-            "op": "eq",
-            "val": true
+            "name": "name",
+            "op": "ilike",
+            "val": "ecklonia%"
          }
       },
       {
          "name": "point",
          "op": "has",
          "val": {
             "name": "media",
@@ -111,14 +110,26 @@
                }
             }
          }
       }
    ]
 }
 ```
+The result of that query can be accessed dynamically through [this link](https://squidle.org/api/annotation?template=models/annotation/list_thumbnails.html&q={"filters":[{"name":"point","op":"has","val":{"name":"has_xy","op":"eq","val":true}},{"name":"point","op":"has","val":{"name":"media","op":"has","val":{"name":"poses","op":"any","val":{"name":"geom","op":"geo_in_bbox","val":[{"lat":-32.020013585799155,"lon":115.49980113118502},{"lat":-32.01995006531625,"lon":115.49987604949759}]}}}}]}).
+Note with a logged in browser session, that link will extract cropped thumbnails around each annotation, but without logging in,
+you'll just see a thumbnail the whole image associated with that annotation.
+The Python code required to build that query could be something like:
+```python
+from sqapi.api import SQAPI, query_filter as qf
+api = SQAPI(host="https://squidle.org", )   # optionally pass in api_key to avoid log in prompt
+r = api.get("/api/annotation")
+r.filter("label", "has", qf("name","ilike","ecklonia%"))   # filter for label name, % here is a wildcard matching anything
+bbox = [{"lat": -32.020013585799155,"lon": 115.49980113118502},{"lat": -32.01995006531625,"lon": 115.49987604949759}]
+r.filter("point", "has", qf("media", "has", qf("poses", "any", qf("geom", "geo_in_bbox", bbox))))  # filter within bounding box
+```
 
 ### Random annotation BOT
 This is an example of an automated labelling bot that selects random class labels to assign to points.
 It provides terrible suggestions, however it provides a simple boiler-plate example of how to integrate a
 Machine Learning algorithm for label suggestions.
 
 Set up the environment and a mini project
@@ -135,54 +146,41 @@
 of the classifier is relatively straight forward.
 In your project directory, create a file named `run_bot.py`:
 
 ```python
 # run_bot.py
 import random
 from sqapi.annotate import Annotator
-from sqapi.request import query_filter as qf
-from sqapi.helpers import cli_init, create_parser
+from sqapi.helpers import cli_init
 from sqapi.media import SQMediaObject
 
 
 class RandoBOT(Annotator):
-    def __init__(self, user_group_id: int, **annotator_args):
-        """
-        Demo classifier that creates random class allocations and probabilities
-        :param user_group_id: the ID of the user_group that you wish to classify
-        """
-        super().__init__(**annotator_args)  # calls base class with all required inputs
-        self.user_group_id = user_group_id  # example of an extra parameter added to the init
-        self.possible_codes = ["ECK", "ASC", "SUB"]
-
+    """
+    An example of an automated labelling bot that selects random class labels to assign to points.
+    It provides terrible suggestions, however it provides a simple boiler-plate example of how to integrate a
+    Machine Learning algorithm for label suggestions.
+    """       
     def classify_point(self, mediaobj: SQMediaObject, x, y, t):
-        """Overridden method: predict label for x-y point"""
-        # image_data = mediaobj.data()            # cv2 image object containing media data
-        # media_path = mediaobj.url               # path to media item
-        classifier_code = random.sample(self.possible_codes, 1)[0]  # get a random code
-        prob = round(random.random(), 2)  # generate a random probability
-        # TODO: use the image_data, x and y point position to generate a real label and prob
-        return classifier_code, prob
+       # This method is used to generate a point prediction
+       # TODO: use the mediaobj, x and y point position to generate a real classifier_code and prob
+       classifier_code = random.randint(0,3)  # get a random code (0-3) to match with label_map_file
+       prob = round(random.random(), 2)  # generate a random probability
+       return classifier_code, prob
 
 
 if __name__ == '__main__':
-    # Get the cli arguments from the Class __init__ function signatures
-    parser = create_parser(RandoBOT)  # convenient method to build a parser from the bot class
+    # Instantiate the bot from the default CLI arguments
+    bot = cli_init(RandoBOT)  
     
-    # Add an extra argument to the parser to get an annotation_set id to classify
-    parser.add_argument('--annotation_set_id', help="Process annotation_set with specific ID", type=int)
+    # Build the annotation_set query (this can be far more complex, see examples for more)
+    annotation_set_id = input("Enter the ID of the annotation_set that you want to classify: ")
+    r = bot.sqapi.get("/api/annotation_set").filter(name="id", op="eq", val=annotation_set_id)  
     
-    # Instantiate the bot class
-    args = parser.parse_args()
-    bot = RandoBOT(**vars(args))
-    
-    # Initialise the request for the annotation_set that you want classified
-    # update the ID to the ID you want
-    r = bot.sqapi.get("/api/annotation_set").filter(name="id", op="in", val=args.annotation_set_id)
-
+    # Run the classifier with the annotation_set query
     bot.start(r)
 ```
 
 The `create_parser` method is a convenience tool that allows you to build a command line parser from the  
 signature of the `__init__` methods for the RandoBot class and all inherited base classes (eg: Annotator).
 
 This allows you to pass arguments from the command line, and helps to show how to use it:
@@ -197,39 +195,55 @@
 #### 2. Create a Label Mapper File
 Before you run it, you also need to create a label map file to pass into the `--label_map_file` argument. 
 This maps the outputs from your classifier to real class labels in the system.
 
 In your project directory, create a file named `rando_bot_label_map.json` 
 with the following content:
 ```json
+[
+  [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"214344"}}],
+  [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"1839"}}],
+  [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"82001000"}}],
+  null 
+]
+```
+The example above, shows a label_map file for a classifier that outputs an integer value classifier code, where `0-2` 
+would be a Label class that uses the vocab_element to lookup a Label across the Label Schemes. `3` would output nothing, 
+which won't be submitted.
+
+Note: if your classifier outputs a string code instead of an integer, you can define a similar 
+mapping file using a dict lookup, like:
+```json
 {
-  "ECK": [{"or":[{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"214344"}},{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"54079009"}}]}],
-  "ASC": [{"or":[{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"1839"}},{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"35000000"}}]}],
-  "SUB": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"82001000"}}]
+  "ECK": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"214344"}}],
+  "ASC": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"1839"}}],
+  "SUB": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"82001000"}}],
+  "NA": null 
 }
 ```
+That will attempt to map the classifier outputs `ECK`, `ASC` and `SUB` to a Label in SQ+.
 
 #### 3. Run your bot
 Now you're ready to run your classifier `RandoBot`, by simply executing this from the command line:
 ```shell
-python run_bot.py --label_map_file rando_bot_label_map.json --annotation_set_id=55 --poll_delay -1 --email_results
+python run_bot.py --label_map_file rando_bot_label_map.json --prob_thresh 0.5 --poll_delay -1 --email_results
 ```
 
-This will run the classifier once on the annotation_set with an `ID=55`
-and attempt to provide automated suggestions on the labels it contains using random class allocations and probabilities. 
-It will run once (as defined by the `--poll_delay=-1` parameter) and it will send an email to the owner the
-annotation_set once complete.
+This will prompt you for a annotation_set id and attempt to provide automated suggestions on the labels it contains 
+using random class allocations and probabilities. It will only submit suggestions with a probability > 0.5 and 
+it will run once (as defined by the `--poll_delay=-1` parameter) 
+and it will send an email to the owner the annotation_set once complete.
 
 Now all that's left is for you to make the labels and probabilities real, and bob's your uncle,
 you've made an automated classifier.
 
 The [examples](https://bitbucket.org/ariell/pysq/src/master/examples/) directory has some examples that you can use and/or adapt for 
 your purposes. Specifically with regard to classifiers:
 
-1. **[demo_randobot.py](https://bitbucket.org/ariell/pysq/src/master/examples/bots/demo_randobot.py)**: same as example above, but with additional command line 
+1. **[demo_randobot.py](https://bitbucket.org/ariell/pysq/src/master/examples/bots/demo_randobot.py)**: similar to example above, but with additional command line 
    arguments for filtering annotation_sets and to keep running as a service.
 2. **[keras_cnn_bot.py](https://bitbucket.org/ariell/pysq/src/master/examples/bots/keras_cnn_bot.py)**: a real classifier that uses a tensor_flow/keras model for 
    classifying points in images. The class received a number of additional parameters that can all be passed in as 
    command line arguments. Run `python keras_cnn_bot.py --help` for more information. This shows an example of how to 
    include additional model-specific arguments along with other parameters, as well as how to process the images and 
    for a real classifier.
```

### Comparing `sqapi-0.4/README.md` & `sqapi-0.41/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -45,27 +45,26 @@
 > need to activate your API key.
 
 ## Examples
 ### Creating queries
 This is by no means an extensive list of possible API queries. The API is extensive and the models are documented
 [here](https://squidle.org/api/help?template=api_help_page.html) and the creation of queries is documented 
 [here](https://squidle.org/api/help?template=api_help_page.html#api_query). `SQAPI` enables a convenient mechanism 
-for creating these queries inside of Python. For example, a basic API query to list the 
-
-`# /api/annotation?template=models/annotation/list_thumbnails.html&q={"filters":[{"name":"point","op":"has","val":{"name":"has_xy","op":"eq","val":true}},{"name":"point","op":"has","val":{"name":"media","op":"has","val":{"name":"poses","op":"any","val":{"name":"geom","op":"geo_in_bbox","val":[{"lat":-32.020013585799155,"lon":115.49980113118502},{"lat":-32.01995006531625,"lon":115.49987604949759}]}}}}]}`
+for creating these queries inside of Python. For example, a basic API query to list all the annotations that have valid 
+labels starting with 'ecklonia' within a spatially constrained bounding box would be:
 ```json
 {
    "filters": [
       {
-         "name": "point",
+         "name": "label",
          "op": "has",
          "val": {
-            "name": "has_xy",
-            "op": "eq",
-            "val": true
+            "name": "name",
+            "op": "ilike",
+            "val": "ecklonia%"
          }
       },
       {
          "name": "point",
          "op": "has",
          "val": {
             "name": "media",
@@ -89,14 +88,26 @@
                }
             }
          }
       }
    ]
 }
 ```
+The result of that query can be accessed dynamically through [this link](https://squidle.org/api/annotation?template=models/annotation/list_thumbnails.html&q={"filters":[{"name":"point","op":"has","val":{"name":"has_xy","op":"eq","val":true}},{"name":"point","op":"has","val":{"name":"media","op":"has","val":{"name":"poses","op":"any","val":{"name":"geom","op":"geo_in_bbox","val":[{"lat":-32.020013585799155,"lon":115.49980113118502},{"lat":-32.01995006531625,"lon":115.49987604949759}]}}}}]}).
+Note with a logged in browser session, that link will extract cropped thumbnails around each annotation, but without logging in,
+you'll just see a thumbnail the whole image associated with that annotation.
+The Python code required to build that query could be something like:
+```python
+from sqapi.api import SQAPI, query_filter as qf
+api = SQAPI(host="https://squidle.org", )   # optionally pass in api_key to avoid log in prompt
+r = api.get("/api/annotation")
+r.filter("label", "has", qf("name","ilike","ecklonia%"))   # filter for label name, % here is a wildcard matching anything
+bbox = [{"lat": -32.020013585799155,"lon": 115.49980113118502},{"lat": -32.01995006531625,"lon": 115.49987604949759}]
+r.filter("point", "has", qf("media", "has", qf("poses", "any", qf("geom", "geo_in_bbox", bbox))))  # filter within bounding box
+```
 
 ### Random annotation BOT
 This is an example of an automated labelling bot that selects random class labels to assign to points.
 It provides terrible suggestions, however it provides a simple boiler-plate example of how to integrate a
 Machine Learning algorithm for label suggestions.
 
 Set up the environment and a mini project
@@ -113,54 +124,41 @@
 of the classifier is relatively straight forward.
 In your project directory, create a file named `run_bot.py`:
 
 ```python
 # run_bot.py
 import random
 from sqapi.annotate import Annotator
-from sqapi.request import query_filter as qf
-from sqapi.helpers import cli_init, create_parser
+from sqapi.helpers import cli_init
 from sqapi.media import SQMediaObject
 
 
 class RandoBOT(Annotator):
-    def __init__(self, user_group_id: int, **annotator_args):
-        """
-        Demo classifier that creates random class allocations and probabilities
-        :param user_group_id: the ID of the user_group that you wish to classify
-        """
-        super().__init__(**annotator_args)  # calls base class with all required inputs
-        self.user_group_id = user_group_id  # example of an extra parameter added to the init
-        self.possible_codes = ["ECK", "ASC", "SUB"]
-
+    """
+    An example of an automated labelling bot that selects random class labels to assign to points.
+    It provides terrible suggestions, however it provides a simple boiler-plate example of how to integrate a
+    Machine Learning algorithm for label suggestions.
+    """       
     def classify_point(self, mediaobj: SQMediaObject, x, y, t):
-        """Overridden method: predict label for x-y point"""
-        # image_data = mediaobj.data()            # cv2 image object containing media data
-        # media_path = mediaobj.url               # path to media item
-        classifier_code = random.sample(self.possible_codes, 1)[0]  # get a random code
-        prob = round(random.random(), 2)  # generate a random probability
-        # TODO: use the image_data, x and y point position to generate a real label and prob
-        return classifier_code, prob
+       # This method is used to generate a point prediction
+       # TODO: use the mediaobj, x and y point position to generate a real classifier_code and prob
+       classifier_code = random.randint(0,3)  # get a random code (0-3) to match with label_map_file
+       prob = round(random.random(), 2)  # generate a random probability
+       return classifier_code, prob
 
 
 if __name__ == '__main__':
-    # Get the cli arguments from the Class __init__ function signatures
-    parser = create_parser(RandoBOT)  # convenient method to build a parser from the bot class
+    # Instantiate the bot from the default CLI arguments
+    bot = cli_init(RandoBOT)  
     
-    # Add an extra argument to the parser to get an annotation_set id to classify
-    parser.add_argument('--annotation_set_id', help="Process annotation_set with specific ID", type=int)
+    # Build the annotation_set query (this can be far more complex, see examples for more)
+    annotation_set_id = input("Enter the ID of the annotation_set that you want to classify: ")
+    r = bot.sqapi.get("/api/annotation_set").filter(name="id", op="eq", val=annotation_set_id)  
     
-    # Instantiate the bot class
-    args = parser.parse_args()
-    bot = RandoBOT(**vars(args))
-    
-    # Initialise the request for the annotation_set that you want classified
-    # update the ID to the ID you want
-    r = bot.sqapi.get("/api/annotation_set").filter(name="id", op="in", val=args.annotation_set_id)
-
+    # Run the classifier with the annotation_set query
     bot.start(r)
 ```
 
 The `create_parser` method is a convenience tool that allows you to build a command line parser from the  
 signature of the `__init__` methods for the RandoBot class and all inherited base classes (eg: Annotator).
 
 This allows you to pass arguments from the command line, and helps to show how to use it:
@@ -175,39 +173,55 @@
 #### 2. Create a Label Mapper File
 Before you run it, you also need to create a label map file to pass into the `--label_map_file` argument. 
 This maps the outputs from your classifier to real class labels in the system.
 
 In your project directory, create a file named `rando_bot_label_map.json` 
 with the following content:
 ```json
+[
+  [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"214344"}}],
+  [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"1839"}}],
+  [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"82001000"}}],
+  null 
+]
+```
+The example above, shows a label_map file for a classifier that outputs an integer value classifier code, where `0-2` 
+would be a Label class that uses the vocab_element to lookup a Label across the Label Schemes. `3` would output nothing, 
+which won't be submitted.
+
+Note: if your classifier outputs a string code instead of an integer, you can define a similar 
+mapping file using a dict lookup, like:
+```json
 {
-  "ECK": [{"or":[{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"214344"}},{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"54079009"}}]}],
-  "ASC": [{"or":[{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"1839"}},{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"35000000"}}]}],
-  "SUB": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"82001000"}}]
+  "ECK": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"214344"}}],
+  "ASC": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"1839"}}],
+  "SUB": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"82001000"}}],
+  "NA": null 
 }
 ```
+That will attempt to map the classifier outputs `ECK`, `ASC` and `SUB` to a Label in SQ+.
 
 #### 3. Run your bot
 Now you're ready to run your classifier `RandoBot`, by simply executing this from the command line:
 ```shell
-python run_bot.py --label_map_file rando_bot_label_map.json --annotation_set_id=55 --poll_delay -1 --email_results
+python run_bot.py --label_map_file rando_bot_label_map.json --prob_thresh 0.5 --poll_delay -1 --email_results
 ```
 
-This will run the classifier once on the annotation_set with an `ID=55`
-and attempt to provide automated suggestions on the labels it contains using random class allocations and probabilities. 
-It will run once (as defined by the `--poll_delay=-1` parameter) and it will send an email to the owner the
-annotation_set once complete.
+This will prompt you for a annotation_set id and attempt to provide automated suggestions on the labels it contains 
+using random class allocations and probabilities. It will only submit suggestions with a probability > 0.5 and 
+it will run once (as defined by the `--poll_delay=-1` parameter) 
+and it will send an email to the owner the annotation_set once complete.
 
 Now all that's left is for you to make the labels and probabilities real, and bob's your uncle,
 you've made an automated classifier.
 
 The [examples](https://bitbucket.org/ariell/pysq/src/master/examples/) directory has some examples that you can use and/or adapt for 
 your purposes. Specifically with regard to classifiers:
 
-1. **[demo_randobot.py](https://bitbucket.org/ariell/pysq/src/master/examples/bots/demo_randobot.py)**: same as example above, but with additional command line 
+1. **[demo_randobot.py](https://bitbucket.org/ariell/pysq/src/master/examples/bots/demo_randobot.py)**: similar to example above, but with additional command line 
    arguments for filtering annotation_sets and to keep running as a service.
 2. **[keras_cnn_bot.py](https://bitbucket.org/ariell/pysq/src/master/examples/bots/keras_cnn_bot.py)**: a real classifier that uses a tensor_flow/keras model for 
    classifying points in images. The class received a number of additional parameters that can all be passed in as 
    command line arguments. Run `python keras_cnn_bot.py --help` for more information. This shows an example of how to 
    include additional model-specific arguments along with other parameters, as well as how to process the images and 
    for a real classifier.
```

### Comparing `sqapi-0.4/setup.py` & `sqapi-0.41/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sqapi',
-    version='0.4',
+    version='0.41',
     packages=['sqapi'],
     install_requires=['requests', 'numpy', 'opencv-python'],
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='A python package that simplifies interactions with the SQUIDLE+ API. It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.',   # Give a short description about your library
     author='Greybits Engineering',                   # Type in your name
```

### Comparing `sqapi-0.4/sqapi/annotate.py` & `sqapi-0.41/sqapi/annotate.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.4/sqapi/api.py` & `sqapi-0.41/sqapi/api.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.4/sqapi/helpers.py` & `sqapi-0.41/sqapi/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 def create_parser(cls, parser=None):
     init = cls.__init__
     doc = inspect.getdoc(init)
     pparams = parse_docstring(doc)
     if parser is None:
         parser = argparse.ArgumentParser(
             description="{short_description}\n{long_description}".format(**pparams),
-            formatter_class=argparse.RawTextHelpFormatter)
+            formatter_class=argparse.RawTextHelpFormatter, conflict_handler='resolve')
     sig = inspect.signature(init)
     for name, param in sig.parameters.items():
         if name in ('self'):
             continue
         if param.kind is not inspect.Parameter.POSITIONAL_OR_KEYWORD:
             continue
```

### Comparing `sqapi-0.4/sqapi/media.py` & `sqapi-0.41/sqapi/media.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.4/sqapi/request.py` & `sqapi-0.41/sqapi/request.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.4/sqapi.egg-info/PKG-INFO` & `sqapi-0.41/sqapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqapi
-Version: 0.4
+Version: 0.41
 Summary: A python package that simplifies interactions with the SQUIDLE+ API. It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.
 Home-page: https://bitbucket.org/ariell/pysq
 Download-URL: https://bitbucket.org/ariell/pysq/get/bede6badfc1ea09cd45b3ae3d4bc3551daa0b3e0.tar.gz
 Author: Greybits Engineering
 License: MIT
 Keywords: SQUIDLE+,API,SQ,Machine Learning
 Classifier: Development Status :: 3 - Alpha
@@ -67,27 +67,26 @@
 > need to activate your API key.
 
 ## Examples
 ### Creating queries
 This is by no means an extensive list of possible API queries. The API is extensive and the models are documented
 [here](https://squidle.org/api/help?template=api_help_page.html) and the creation of queries is documented 
 [here](https://squidle.org/api/help?template=api_help_page.html#api_query). `SQAPI` enables a convenient mechanism 
-for creating these queries inside of Python. For example, a basic API query to list the 
-
-`# /api/annotation?template=models/annotation/list_thumbnails.html&q={"filters":[{"name":"point","op":"has","val":{"name":"has_xy","op":"eq","val":true}},{"name":"point","op":"has","val":{"name":"media","op":"has","val":{"name":"poses","op":"any","val":{"name":"geom","op":"geo_in_bbox","val":[{"lat":-32.020013585799155,"lon":115.49980113118502},{"lat":-32.01995006531625,"lon":115.49987604949759}]}}}}]}`
+for creating these queries inside of Python. For example, a basic API query to list all the annotations that have valid 
+labels starting with 'ecklonia' within a spatially constrained bounding box would be:
 ```json
 {
    "filters": [
       {
-         "name": "point",
+         "name": "label",
          "op": "has",
          "val": {
-            "name": "has_xy",
-            "op": "eq",
-            "val": true
+            "name": "name",
+            "op": "ilike",
+            "val": "ecklonia%"
          }
       },
       {
          "name": "point",
          "op": "has",
          "val": {
             "name": "media",
@@ -111,14 +110,26 @@
                }
             }
          }
       }
    ]
 }
 ```
+The result of that query can be accessed dynamically through [this link](https://squidle.org/api/annotation?template=models/annotation/list_thumbnails.html&q={"filters":[{"name":"point","op":"has","val":{"name":"has_xy","op":"eq","val":true}},{"name":"point","op":"has","val":{"name":"media","op":"has","val":{"name":"poses","op":"any","val":{"name":"geom","op":"geo_in_bbox","val":[{"lat":-32.020013585799155,"lon":115.49980113118502},{"lat":-32.01995006531625,"lon":115.49987604949759}]}}}}]}).
+Note with a logged in browser session, that link will extract cropped thumbnails around each annotation, but without logging in,
+you'll just see a thumbnail the whole image associated with that annotation.
+The Python code required to build that query could be something like:
+```python
+from sqapi.api import SQAPI, query_filter as qf
+api = SQAPI(host="https://squidle.org", )   # optionally pass in api_key to avoid log in prompt
+r = api.get("/api/annotation")
+r.filter("label", "has", qf("name","ilike","ecklonia%"))   # filter for label name, % here is a wildcard matching anything
+bbox = [{"lat": -32.020013585799155,"lon": 115.49980113118502},{"lat": -32.01995006531625,"lon": 115.49987604949759}]
+r.filter("point", "has", qf("media", "has", qf("poses", "any", qf("geom", "geo_in_bbox", bbox))))  # filter within bounding box
+```
 
 ### Random annotation BOT
 This is an example of an automated labelling bot that selects random class labels to assign to points.
 It provides terrible suggestions, however it provides a simple boiler-plate example of how to integrate a
 Machine Learning algorithm for label suggestions.
 
 Set up the environment and a mini project
@@ -135,54 +146,41 @@
 of the classifier is relatively straight forward.
 In your project directory, create a file named `run_bot.py`:
 
 ```python
 # run_bot.py
 import random
 from sqapi.annotate import Annotator
-from sqapi.request import query_filter as qf
-from sqapi.helpers import cli_init, create_parser
+from sqapi.helpers import cli_init
 from sqapi.media import SQMediaObject
 
 
 class RandoBOT(Annotator):
-    def __init__(self, user_group_id: int, **annotator_args):
-        """
-        Demo classifier that creates random class allocations and probabilities
-        :param user_group_id: the ID of the user_group that you wish to classify
-        """
-        super().__init__(**annotator_args)  # calls base class with all required inputs
-        self.user_group_id = user_group_id  # example of an extra parameter added to the init
-        self.possible_codes = ["ECK", "ASC", "SUB"]
-
+    """
+    An example of an automated labelling bot that selects random class labels to assign to points.
+    It provides terrible suggestions, however it provides a simple boiler-plate example of how to integrate a
+    Machine Learning algorithm for label suggestions.
+    """       
     def classify_point(self, mediaobj: SQMediaObject, x, y, t):
-        """Overridden method: predict label for x-y point"""
-        # image_data = mediaobj.data()            # cv2 image object containing media data
-        # media_path = mediaobj.url               # path to media item
-        classifier_code = random.sample(self.possible_codes, 1)[0]  # get a random code
-        prob = round(random.random(), 2)  # generate a random probability
-        # TODO: use the image_data, x and y point position to generate a real label and prob
-        return classifier_code, prob
+       # This method is used to generate a point prediction
+       # TODO: use the mediaobj, x and y point position to generate a real classifier_code and prob
+       classifier_code = random.randint(0,3)  # get a random code (0-3) to match with label_map_file
+       prob = round(random.random(), 2)  # generate a random probability
+       return classifier_code, prob
 
 
 if __name__ == '__main__':
-    # Get the cli arguments from the Class __init__ function signatures
-    parser = create_parser(RandoBOT)  # convenient method to build a parser from the bot class
+    # Instantiate the bot from the default CLI arguments
+    bot = cli_init(RandoBOT)  
     
-    # Add an extra argument to the parser to get an annotation_set id to classify
-    parser.add_argument('--annotation_set_id', help="Process annotation_set with specific ID", type=int)
+    # Build the annotation_set query (this can be far more complex, see examples for more)
+    annotation_set_id = input("Enter the ID of the annotation_set that you want to classify: ")
+    r = bot.sqapi.get("/api/annotation_set").filter(name="id", op="eq", val=annotation_set_id)  
     
-    # Instantiate the bot class
-    args = parser.parse_args()
-    bot = RandoBOT(**vars(args))
-    
-    # Initialise the request for the annotation_set that you want classified
-    # update the ID to the ID you want
-    r = bot.sqapi.get("/api/annotation_set").filter(name="id", op="in", val=args.annotation_set_id)
-
+    # Run the classifier with the annotation_set query
     bot.start(r)
 ```
 
 The `create_parser` method is a convenience tool that allows you to build a command line parser from the  
 signature of the `__init__` methods for the RandoBot class and all inherited base classes (eg: Annotator).
 
 This allows you to pass arguments from the command line, and helps to show how to use it:
@@ -197,39 +195,55 @@
 #### 2. Create a Label Mapper File
 Before you run it, you also need to create a label map file to pass into the `--label_map_file` argument. 
 This maps the outputs from your classifier to real class labels in the system.
 
 In your project directory, create a file named `rando_bot_label_map.json` 
 with the following content:
 ```json
+[
+  [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"214344"}}],
+  [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"1839"}}],
+  [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"82001000"}}],
+  null 
+]
+```
+The example above, shows a label_map file for a classifier that outputs an integer value classifier code, where `0-2` 
+would be a Label class that uses the vocab_element to lookup a Label across the Label Schemes. `3` would output nothing, 
+which won't be submitted.
+
+Note: if your classifier outputs a string code instead of an integer, you can define a similar 
+mapping file using a dict lookup, like:
+```json
 {
-  "ECK": [{"or":[{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"214344"}},{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"54079009"}}]}],
-  "ASC": [{"or":[{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"1839"}},{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"35000000"}}]}],
-  "SUB": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"82001000"}}]
+  "ECK": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"214344"}}],
+  "ASC": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"1839"}}],
+  "SUB": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"82001000"}}],
+  "NA": null 
 }
 ```
+That will attempt to map the classifier outputs `ECK`, `ASC` and `SUB` to a Label in SQ+.
 
 #### 3. Run your bot
 Now you're ready to run your classifier `RandoBot`, by simply executing this from the command line:
 ```shell
-python run_bot.py --label_map_file rando_bot_label_map.json --annotation_set_id=55 --poll_delay -1 --email_results
+python run_bot.py --label_map_file rando_bot_label_map.json --prob_thresh 0.5 --poll_delay -1 --email_results
 ```
 
-This will run the classifier once on the annotation_set with an `ID=55`
-and attempt to provide automated suggestions on the labels it contains using random class allocations and probabilities. 
-It will run once (as defined by the `--poll_delay=-1` parameter) and it will send an email to the owner the
-annotation_set once complete.
+This will prompt you for a annotation_set id and attempt to provide automated suggestions on the labels it contains 
+using random class allocations and probabilities. It will only submit suggestions with a probability > 0.5 and 
+it will run once (as defined by the `--poll_delay=-1` parameter) 
+and it will send an email to the owner the annotation_set once complete.
 
 Now all that's left is for you to make the labels and probabilities real, and bob's your uncle,
 you've made an automated classifier.
 
 The [examples](https://bitbucket.org/ariell/pysq/src/master/examples/) directory has some examples that you can use and/or adapt for 
 your purposes. Specifically with regard to classifiers:
 
-1. **[demo_randobot.py](https://bitbucket.org/ariell/pysq/src/master/examples/bots/demo_randobot.py)**: same as example above, but with additional command line 
+1. **[demo_randobot.py](https://bitbucket.org/ariell/pysq/src/master/examples/bots/demo_randobot.py)**: similar to example above, but with additional command line 
    arguments for filtering annotation_sets and to keep running as a service.
 2. **[keras_cnn_bot.py](https://bitbucket.org/ariell/pysq/src/master/examples/bots/keras_cnn_bot.py)**: a real classifier that uses a tensor_flow/keras model for 
    classifying points in images. The class received a number of additional parameters that can all be passed in as 
    command line arguments. Run `python keras_cnn_bot.py --help` for more information. This shows an example of how to 
    include additional model-specific arguments along with other parameters, as well as how to process the images and 
    for a real classifier.
```

