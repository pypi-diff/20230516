# Comparing `tmp/aij-1.0.6.tar.gz` & `tmp/aij-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.0.6.tar", last modified: Sun May 14 22:26:43 2023, max compression
+gzip compressed data, was "aij-1.0.7.tar", last modified: Tue May 16 14:26:12 2023, max compression
```

## Comparing `aij-1.0.6.tar` & `aij-1.0.7.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 22:26:44.000000 aij-1.0.6/
--rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-1.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-14 22:26:44.000000 aij-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-10 22:39:42.000000 aij-1.0.6/README.md
--rw-rw-rw-   0        0        0     6350 2023-05-14 22:26:34.000000 aij-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 22:26:44.000000 aij-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 22:26:44.000000 aij-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 22:26:44.000000 aij-1.0.6/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-14 22:26:44.000000 aij-1.0.6/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-05-14 22:26:44.000000 aij-1.0.6/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 22:26:44.000000 aij-1.0.6/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-05-14 22:26:44.000000 aij-1.0.6/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      207 2023-05-14 22:26:44.000000 aij-1.0.6/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-05-14 22:26:44.000000 aij-1.0.6/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 22:26:44.000000 aij-1.0.6/src/custom/
--rw-rw-rw-   0        0        0      440 2023-05-10 19:37:52.000000 aij-1.0.6/src/custom/__init__.py
--rw-rw-rw-   0        0        0     4531 2023-05-10 18:27:28.000000 aij-1.0.6/src/custom/generator.py
-drwxrwxrwx   0        0        0        0 2023-05-14 22:26:44.000000 aij-1.0.6/src/intro/
--rw-rw-rw-   0        0        0      440 2023-05-07 13:08:58.000000 aij-1.0.6/src/intro/__init__.py
--rw-rw-rw-   0        0        0     4524 2023-05-07 13:07:50.000000 aij-1.0.6/src/intro/intro.py
-drwxrwxrwx   0        0        0        0 2023-05-14 22:26:44.000000 aij-1.0.6/src/news/
--rw-rw-rw-   0        0        0      567 2023-05-07 13:07:50.000000 aij-1.0.6/src/news/__init__.py
--rw-rw-rw-   0        0        0     4492 2023-05-07 13:16:16.000000 aij-1.0.6/src/news/core.py
--rw-rw-rw-   0        0        0     1407 2023-05-07 13:18:00.000000 aij-1.0.6/src/news/publisher.py
--rw-rw-rw-   0        0        0     1196 2023-05-05 12:37:32.000000 aij-1.0.6/src/news/subscriber.py
-drwxrwxrwx   0        0        0        0 2023-05-14 22:26:44.000000 aij-1.0.6/src/setup/
--rw-rw-rw-   0        0        0     1162 2023-05-07 21:18:54.000000 aij-1.0.6/src/setup/__init__.py
--rw-rw-rw-   0        0        0     3739 2023-05-07 21:18:28.000000 aij-1.0.6/src/setup/install.py
-drwxrwxrwx   0        0        0        0 2023-05-14 22:26:44.000000 aij-1.0.6/src/speech/
--rw-rw-rw-   0        0        0      152 2023-05-14 22:21:56.000000 aij-1.0.6/src/speech/__init__.py
--rw-rw-rw-   0        0        0     1052 2023-05-14 22:20:36.000000 aij-1.0.6/src/speech/talk.py
--rw-rw-rw-   0        0        0      873 2023-05-14 22:05:06.000000 aij-1.0.6/src/speech/whisperx.py
--rw-rw-rw-   0        0        0      579 2023-05-14 21:57:48.000000 aij-1.0.6/src/speech/whisperxx.py
-drwxrwxrwx   0        0        0        0 2023-05-14 22:26:44.000000 aij-1.0.6/src/webcam/
--rw-rw-rw-   0        0        0    17500 2023-05-06 19:32:44.000000 aij-1.0.6/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/
+-rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-1.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-16 14:26:14.000000 aij-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-10 22:39:42.000000 aij-1.0.7/README.md
+-rw-rw-rw-   0        0        0     6363 2023-05-16 14:25:48.000000 aij-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 14:26:14.000000 aij-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-16 14:26:14.000000 aij-1.0.7/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2023-05-16 14:26:14.000000 aij-1.0.7/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 14:26:14.000000 aij-1.0.7/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-05-16 14:26:14.000000 aij-1.0.7/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      213 2023-05-16 14:26:14.000000 aij-1.0.7/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       41 2023-05-16 14:26:14.000000 aij-1.0.7/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/intro/
+-rw-rw-rw-   0        0        0        0 2023-05-16 08:04:50.000000 aij-1.0.7/src/intro/__init__.py
+-rw-rw-rw-   0        0        0     4532 2023-05-15 21:53:56.000000 aij-1.0.7/src/intro/intro.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/messaging/
+-rw-rw-rw-   0        0        0      213 2023-05-16 14:04:28.000000 aij-1.0.7/src/messaging/__init__.py
+-rw-rw-rw-   0        0        0     4151 2023-05-16 14:18:30.000000 aij-1.0.7/src/messaging/views.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/news/
+-rw-rw-rw-   0        0        0      466 2023-05-16 13:53:54.000000 aij-1.0.7/src/news/__init__.py
+-rw-rw-rw-   0        0        0     4292 2023-05-16 14:24:04.000000 aij-1.0.7/src/news/models.py
+-rw-rw-rw-   0        0        0     4768 2023-05-16 14:26:00.000000 aij-1.0.7/src/news/views.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/setup/
+-rw-rw-rw-   0        0        0     2974 2023-05-16 09:54:22.000000 aij-1.0.7/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/speech/
+-rw-rw-rw-   0        0        0      163 2023-05-15 20:59:02.000000 aij-1.0.7/src/speech/__init__.py
+-rw-rw-rw-   0        0        0     1070 2023-05-15 21:51:26.000000 aij-1.0.7/src/speech/talk.py
+-rw-rw-rw-   0        0        0      880 2023-05-15 21:52:02.000000 aij-1.0.7/src/speech/whisperx.py
+-rw-rw-rw-   0        0        0      579 2023-05-14 21:57:48.000000 aij-1.0.7/src/speech/whisperxx.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:26:14.000000 aij-1.0.7/src/webcam/
+-rw-rw-rw-   0        0        0    17500 2023-05-15 20:59:02.000000 aij-1.0.7/src/webcam/__init__.py
```

### Comparing `aij-1.0.6/LICENSE.txt` & `aij-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.0.6/PKG-INFO` & `aij-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.0.6
+Version: 1.0.7
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.0.6/README.md` & `aij-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.0.6/pyproject.toml` & `aij-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.6"
+version = "1.0.7"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -111,15 +111,16 @@
     "pandas",
     "gtts",
     "pygame",
     "cairosvg",
     "pika",
     "newsapi-python",
     "openai",
-    "langchain"
+    "langchain",
+    "plyer"
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
```

### Comparing `aij-1.0.6/src/aij.egg-info/PKG-INFO` & `aij-1.0.7/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.0.6
+Version: 1.0.7
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.0.6/src/custom/generator.py` & `aij-1.0.7/src/intro/intro.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-import datetime
 import cv2
 import os
 import random
 import numpy as np
 import threading
 from pygame import mixer
 
 user_profile = os.environ['USERPROFILE']
 SEP = os.path.sep
 
-class VideoThread(threading.Thread):
+
+class AnimationThread(threading.Thread):
     """
     This class represents a thread that generates an animation video
-    @param: None
-    @return: None
     """
+
     def __init__(self):
         """
         This method is called when the object is created
-        @param: None
-        @return: None
         """
         threading.Thread.__init__(self)
         # Path to the album directory containing all the images
         self.album_path = user_profile + SEP + '.aij' + SEP + 'image' + SEP + 'intro'
         self.audio_path = user_profile + SEP + '.aij' + SEP + 'audio'
         self.audio_intro_abs = self.audio_path + SEP + 'intro.mp3'
         self.audio_next_abs = self.audio_path + SEP + 'next.mp3'
@@ -51,21 +48,20 @@
         # Shuffle the images
         random.shuffle(self.images)
 
         # Define the animation parameters
         self.animation_width = 1920
         self.animation_height = 1080
         self.fps = 60
-        self.duration = 10 # in seconds
+        self.duration = 10  # in seconds
 
         # Create the video writer object
         fourcc = cv2.VideoWriter_fourcc(*'mp4v')
-        self.video_writer = cv2.VideoWriter('animation.mp4', fourcc, self.fps, (self.animation_width, self.animation_height))
-
-
+        self.video_writer = cv2.VideoWriter('animation.mp4', fourcc, self.fps,
+                                            (self.animation_width, self.animation_height))
 
     def run(self):
         """
         This method is called when the thread is started
         @param: None
         @return: None
         """
@@ -75,15 +71,16 @@
 
         # Generate the animation frames
         num_frames = self.fps * self.duration
         for i in range(num_frames):
             # Create a blank frame
             frame = np.zeros((self.animation_height, self.animation_width, 3), dtype=np.uint8)
 
-            # Choose a random image and resize it to 1920x1080 pixels (Full HD). Make sure the aspect ratio is maintained while resizing
+            # Choose a random image and resize it to 1920x1080 pixels (Full HD).
+            # Make sure the aspect ratio is maintained while resizing
             img = self.images[i % len(self.images)]
             img = cv2.resize(img, (1920, 1080), interpolation=cv2.INTER_AREA)
 
             # Update the image position
             x += random.randint(-50, 50)
             y += random.randint(-50, 50)
             x = max(0, min(x, self.animation_width - img.shape[1]))
@@ -93,40 +90,42 @@
             if img.shape[0] > self.animation_height:
                 img = img[:self.animation_height, :, :]
             if img.shape[1] > self.animation_width:
                 img = img[:, :self.animation_width, :]
 
             # Draw the image on the frame
             img_height, img_width, _ = img.shape
-            frame[y:y+img_height, x:x+img_width] = img
+            frame[y:y + img_height, x:x + img_width] = img
 
             # Write the frame to the video writer
             self.video_writer.write(frame)
 
         # Release the video writer
         self.video_writer.release()
 
         # merge the audio and video files
-        os.system('ffmpeg -i animation.mp4 -i ' + self.audio_intro_abs + ' -c:v copy -c:a aac -strict experimental animation_with_audio.mp4')
+        os.system(
+            'ffmpeg -i animation.mp4 -i ' + self.audio_intro_abs +
+            ' -c:v copy -c:a aac -strict experimental animation_with_audio.mp4')
 
         # Print the path of the animation video
         print('Animation video generated at: ' + os.getcwd() + SEP + 'animation_with_audio.mp4')
 
+
 def main():
     """
     This function is the entry point of the program
     @param: None
     @return: None
     """
     # Create and start the animation thread
-    animation_thread = VideoThread()
+    animation_thread = AnimationThread()
     animation_thread.start()
 
     # Do some other work here
     print('Doing some other work here...')
 
     # Wait for the animation thread to finish
     animation_thread.join()
 
     # Destroy all windows
     cv2.destroyAllWindows()
-
```

### Comparing `aij-1.0.6/src/news/core.py` & `aij-1.0.7/src/news/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,106 +1,100 @@
 import json
-import os
+import logging as log
 import time
 from threading import Timer
 
-import pandas as pd
 import pika
 from newsapi import NewsApiClient
-
 from newsapi.newsapi_exception import NewsAPIException
 
 
 class NewsPublisher:
     """
     A class to publish news articles to a RabbitMQ queue using the NewsAPI
     @param api_key: the api key to access the NewsAPI
     @param host: the host name of the RabbitMQ server
     @param queue_name: the name of the queue to publish the news articles
     """
+
     def __init__(self, api_key, host='localhost', queue_name='news_stream'):
         self.api = NewsApiClient(api_key=api_key)
         self.host = host
         self.queue_name = queue_name
         # set up a connection to RabbitMQ
         self.connection = pika.BlockingConnection(pika.ConnectionParameters(host=self.host))
         self.channel = self.connection.channel()
-        self.sources = 'bbc-news, cnn, fox-news, google-news, time, wired, the-new-york-times, the-wall-street-journal, the-washington-post, usa-today, abc-news, associated-press, bloomberg, business-insider, cbs-news, cnbc, entertainment-weekly, espn, fortune, fox-sports, mtv-news, national-geographic, nbc-news, new-scientist, newsweek, politico, reddit-r-all, reuters, the-hill, the-huffington-post, the-verge, the-washington-times, vice-news'
+        self.sources = 'bbc-news, cnn, fox-news, google-news, time, wired, the-new-york-times, ' \
+                       'the-wall-street-journal, the-washington-post, usa-today, abc-news, associated-press, ' \
+                       'bloomberg, business-insider, cbs-news, cnbc, entertainment-weekly, espn, fortune, fox-sports, ' \
+                       'mtv-news, national-geographic, nbc-news, new-scientist, newsweek, politico, reddit-r-all, ' \
+                       'reuters, the-hill, the-huffington-post, the-verge, the-washington-times, vice-news'
 
         try:
             self.articles = self.api.get_everything(sources=self.sources)
             self.headlines = self.api.get_top_headlines(sources=self.sources)
         except NewsAPIException as api_exception:
-            print(f"Could not request results from NewsAPI; {api_exception}")
-            print("Loading the news from the database...")
+            log.error(f"Could not request results from NewsAPI; {api_exception}")
 
     def publish(self):
         """
         Publish the news articles to the RabbitMQ queue one by one and save the news to the database
         """
         try:
             for _article in self.articles['articles']:
                 _body = json.dumps(_article).encode('utf-8')
                 self.channel.basic_publish(exchange='', routing_key=self.queue_name, body=_body)
-                print(f"Published a news article to the queue: {_article['title']}")
+                log.info(f"Published a news article to the queue: {_article['title']}")
                 # wait for 1 second before publishing the next article
                 time.sleep(1)
 
             for _headline in self.headlines['articles']:
                 _body = json.dumps(_headline).encode('utf-8')
                 self.channel.basic_publish(exchange='', routing_key=f"{self.queue_name}_headlines", body=_body)
-                print(f"Published a news headline to the queue: {_headline['title']}")
+                log.info(f"Published a news headline to the queue: {_headline['title']}")
                 # wait for 1 second before publishing the next article
                 time.sleep(1)
         except NewsAPIException as api_exception:
-            print(f"Could not request results from NewsAPI; {api_exception}")
-            print("Loading the news from the database...")
-            
+            log.error(f"Could not request results from NewsAPI; {api_exception}")
 
         # do not close the connection until the message is delivered
         if self.connection.is_open:
             self.connection.close()
 
         # call the function again after 100 seconds because there are max. 100 results per page
-        Timer(100, self.publish).start()
-
+        Timer(60 * 5, self.publish).start()
 
     def destroy(self):
         """
         Destroy the connection to the RabbitMQ server
         """
         self.connection.close()
 
 
 class NewsSubscriber:
     """
     This class implements a RabbitMQ consumer.
     """
-    def __init__(self, host, callback_function):
+
+    def __init__(self, host='localhost', queue_name = 'news_stream', callback=None):
         """
         This method initializes the consumer.
         """
         self.connection = pika.BlockingConnection(pika.ConnectionParameters(host))
         self.channel = self.connection.channel()
-        self.channel.queue_declare(queue='news_stream')
-        self.callback_function = callback_function
+        self.channel.queue_declare(queue=queue_name)
+        self.callback = callback
+        self.queue_name = queue_name
 
     def subscribe(self):
         """
         This method starts consuming messages from the RabbitMQ queue.
         """
-        self.channel.basic_consume(queue='news_stream', on_message_callback=self.callback, auto_ack=True)
+        self.channel.basic_consume(queue=self.queue_name, on_message_callback=self.callback, auto_ack=True)
         self.channel.start_consuming()
 
-    def callback(self, ch, method, properties, body):
-        """
-        This method is called when a message is received from the RabbitMQ queue.
-        """
-        self.callback_function(method.routing_key, body)
-        time.sleep(1)
-
     def destroy(self):
         """
         This method closes the connection to the RabbitMQ server.
         """
         if self.connection.is_open:
-            self.connection.close()
+            self.connection.close()
```

### Comparing `aij-1.0.6/src/speech/talk.py` & `aij-1.0.7/src/speech/talk.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,41 @@
-import os
-import time
-from langchain.llms import OpenAI
-from gtts import gTTS
-from io import BytesIO
-from pygame import mixer
-
-
-user_profile = os.environ['USERPROFILE']
-SEP = os.path.sep
-JOKE_PATH = f"{user_profile}{SEP}Desktop{SEP}joke.mp3"
-
-class AIJoke():
-    """
-    A class to tell a joke using OpenAI's API
-    """
-    
-    def __init__(self, output_path=JOKE_PATH):
-
-        self.llm = OpenAI(model_name="text-ada-001", n=2, best_of=2)
-        self.answer = self.llm("Tell me a joke")
-        self.answer = "\n".join([line for line in self.answer.split("\n") if line.strip() != ""])
-        self.out = output_path
-
-
-    def save_as_audio(self):
-        """
-        Save the joke as an audio file
-        """
-        tts = gTTS(self.answer, lang="en")
-        # save to file
-        tts.save(self.out)
-        
-    def play_audio(self):
-        """
-        Play the audio file
-        """
-        mixer.init()
-        mixer.music.load(self.out)
-        mixer.music.play()
-
-        while mixer.music.get_busy():
-            time.sleep(1)
-        
+import os
+import time
+from langchain.llms import OpenAI
+from gtts import gTTS
+from io import BytesIO
+from pygame import mixer
+
+user_profile = os.environ['USERPROFILE']
+SEP = os.path.sep
+JOKE_PATH = f"{user_profile}{SEP}Desktop{SEP}joke.mp3"
+
+
+class AIJoke():
+    """
+    A class to tell a joke using OpenAI's API
+    """
+
+    def __init__(self, output_path=JOKE_PATH):
+        self.llm = OpenAI(model_name="text-ada-001", n=2, best_of=2)
+        self.answer = self.llm("Tell me a joke")
+        self.answer = "\n".join([line for line in self.answer.split("\n") if line.strip() != ""])
+        self.out = output_path
+
+    def save_as_audio(self):
+        """
+        Save the joke as an audio file
+        """
+        tts = gTTS(self.answer, lang="en")
+        # save to file
+        tts.save(self.out)
+
+    def play_audio(self):
+        """
+        Play the audio file
+        """
+        mixer.init()
+        mixer.music.load(self.out)
+        mixer.music.play()
+
+        while mixer.music.get_busy():
+            time.sleep(1)
```

### Comparing `aij-1.0.6/src/speech/whisperx.py` & `aij-1.0.7/src/speech/whisperx.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 # transcribe each video
 for video in videos:
     #  ffmpeg data conversion from mp4 to wav
     audio = video.replace('.mp4', '.wav')
     if not os.path.exists(audio):
         os.system(f"ffmpeg -i {video} -vn -acodec pcm_s16le -ar 16000 -ac 1 {video.replace('.mp4', '.wav')}")
-   
+
     result = whisper.transcribe(model, audio)
     print(f"Transcription for {audio}:")
-   
+
     # print to a file with the same name as the audio (wav) but with a .txt extension
     with open(audio.replace('.wav', '.txt'), 'w', encoding="utf-8") as f:
         f.write(result['text'])
 
-print(
-    result['text']
-)
+    print(
+        result['text']
+    )
```

### Comparing `aij-1.0.6/src/speech/whisperxx.py` & `aij-1.0.7/src/speech/whisperxx.py`

 * *Files identical despite different names*

### Comparing `aij-1.0.6/src/webcam/__init__.py` & `aij-1.0.7/src/webcam/__init__.py`

 * *Files identical despite different names*

