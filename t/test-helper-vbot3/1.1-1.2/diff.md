# Comparing `tmp/test_helper_vbot3-1.1.tar.gz` & `tmp/test_helper_vbot3-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_helper_vbot3-1.1.tar", last modified: Sun May 14 16:10:45 2023, max compression
+gzip compressed data, was "test_helper_vbot3-1.2.tar", last modified: Tue May 16 07:12:08 2023, max compression
```

## Comparing `test_helper_vbot3-1.1.tar` & `test_helper_vbot3-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 16:10:45.304287 test_helper_vbot3-1.1/
--rw-rw-rw-   0        0        0     1094 2023-05-13 15:59:41.000000 test_helper_vbot3-1.1/LICENSE
--rw-rw-rw-   0        0        0       60 2023-05-14 08:37:46.000000 test_helper_vbot3-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1036 2023-05-14 16:10:45.304287 test_helper_vbot3-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-05-14 08:39:31.000000 test_helper_vbot3-1.1/README.md
--rw-rw-rw-   0        0        0      110 2023-05-14 08:37:46.000000 test_helper_vbot3-1.1/pyproject.toml
--rw-rw-rw-   0        0        0      707 2023-05-14 16:10:45.319913 test_helper_vbot3-1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 16:10:45.304287 test_helper_vbot3-1.1/test_helper_vbot3.egg-info/
--rw-rw-rw-   0        0        0     1036 2023-05-14 16:10:45.000000 test_helper_vbot3-1.1/test_helper_vbot3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-05-14 16:10:45.000000 test_helper_vbot3-1.1/test_helper_vbot3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 16:10:45.000000 test_helper_vbot3-1.1/test_helper_vbot3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-14 16:10:45.000000 test_helper_vbot3-1.1/test_helper_vbot3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-14 16:10:45.000000 test_helper_vbot3-1.1/test_helper_vbot3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 16:10:45.304287 test_helper_vbot3-1.1/tester_vbot3/
--rw-rw-rw-   0        0        0     3152 2023-05-14 15:59:18.000000 test_helper_vbot3-1.1/tester_vbot3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:12:08.805372 test_helper_vbot3-1.2/
+-rw-rw-rw-   0        0        0     1094 2023-05-13 15:59:41.000000 test_helper_vbot3-1.2/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-05-14 08:37:46.000000 test_helper_vbot3-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1036 2023-05-16 07:12:08.805872 test_helper_vbot3-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-05-14 08:39:31.000000 test_helper_vbot3-1.2/README.md
+-rw-rw-rw-   0        0        0      110 2023-05-14 08:37:46.000000 test_helper_vbot3-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      707 2023-05-16 07:12:08.807873 test_helper_vbot3-1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 07:12:08.795365 test_helper_vbot3-1.2/test_helper_vbot3.egg-info/
+-rw-rw-rw-   0        0        0     1036 2023-05-16 07:12:08.000000 test_helper_vbot3-1.2/test_helper_vbot3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-05-16 07:12:08.000000 test_helper_vbot3-1.2/test_helper_vbot3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 07:12:08.000000 test_helper_vbot3-1.2/test_helper_vbot3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-16 07:12:08.000000 test_helper_vbot3-1.2/test_helper_vbot3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-16 07:12:08.000000 test_helper_vbot3-1.2/test_helper_vbot3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 07:12:08.803371 test_helper_vbot3-1.2/tester_vbot3/
+-rw-rw-rw-   0        0        0     4078 2023-05-16 07:09:11.000000 test_helper_vbot3-1.2/tester_vbot3/__init__.py
```

### Comparing `test_helper_vbot3-1.1/LICENSE` & `test_helper_vbot3-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `test_helper_vbot3-1.1/PKG-INFO` & `test_helper_vbot3-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_helper_vbot3
-Version: 1.1
+Version: 1.2
 Summary: Tester for Vbot3
 Home-page: https://github.com/vb64/test.helper.vbot3
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
 Project-URL: Bug Tracker, https://github.com/vb64/test.helper.vbot3/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `test_helper_vbot3-1.1/README.md` & `test_helper_vbot3-1.2/README.md`

 * *Files identical despite different names*

### Comparing `test_helper_vbot3-1.1/setup.cfg` & `test_helper_vbot3-1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6573 745f 6865 6c70 6572 5f76   = test_helper_v
 00000020: 626f 7433 0d0a 7665 7273 696f 6e20 3d20  bot3..version = 
-00000030: 312e 310d 0a61 7574 686f 7220 3d20 5669  1.1..author = Vi
+00000030: 312e 320d 0a61 7574 686f 7220 3d20 5669  1.2..author = Vi
 00000040: 7461 6c79 2042 6f67 6f6d 6f6c 6f76 0d0a  taly Bogomolov..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 206d  author_email = m
 00000060: 6169 6c40 7669 7461 6c79 2d62 6f67 6f6d  ail@vitaly-bogom
 00000070: 6f6c 6f76 2e72 750d 0a64 6573 6372 6970  olov.ru..descrip
 00000080: 7469 6f6e 203d 2054 6573 7465 7220 666f  tion = Tester fo
 00000090: 7220 5662 6f74 330d 0a6c 6f6e 675f 6465  r Vbot3..long_de
 000000a0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
```

### Comparing `test_helper_vbot3-1.1/test_helper_vbot3.egg-info/PKG-INFO` & `test_helper_vbot3-1.2/test_helper_vbot3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-helper-vbot3
-Version: 1.1
+Version: 1.2
 Summary: Tester for Vbot3
 Home-page: https://github.com/vb64/test.helper.vbot3
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
 Project-URL: Bug Tracker, https://github.com/vb64/test.helper.vbot3/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `test_helper_vbot3-1.1/tester_vbot3/__init__.py` & `test_helper_vbot3-1.2/tester_vbot3/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Vbot3 tester."""
 from telemulator3 import Telemulator, private_command, private_text
+from telemulator3.update.message import Text, Command
 from tester_flask import TestFlask
 from test_helper_gae3 import TestGae3
 
 
 class MockReq:
     """Mock flask request."""
 
@@ -30,30 +31,50 @@
 
 class Vbot3Tester(TestFlask, TestGae3, Telemulator):
     """Tester for Vbot3."""
 
     teleuser = None
     private = None
     group = None
+    tele_message = None
+    group_message = None
 
     def init(self, flask_app, vbot3, bot_name, bot_username, queue_yaml_dir):
         """Init tests stuff."""
         TestFlask.set_up(self, flask_app)
         TestGae3.set_up(self, queue_yaml_dir)
         self.set_tested_bot(vbot3, name=bot_name, username=bot_username)
 
         self.teleuser = self.api.create_user('Test', 'User', language_code='en')
         self.private = self.teleuser.private()
         self.group = self.teleuser.create_group("Test group")
+        self.tele_message = Text(self.private, self.teleuser, "Hello private!")
+        self.group_message = Text(self.group, self.teleuser, "Hello group!")
 
     def tearDown(self):
         """Clear tests."""
         TestGae3.tear_down(self)
         super().tearDown()
 
+    def send2chat(self, chat, message):
+        """Send message to given chat."""
+        with self.app.test_request_context():
+            return chat.send(message)
+
+    def send_command(self, chat, command, from_user=None, **kwargs):
+        """Send command to given chat."""
+        from_user = from_user or self.teleuser
+        return self.send2chat(chat, Command(chat, from_user, command, **kwargs))
+
+    def tg_button(self, row, index=0, chat=None, user=None):
+        """Send custom keyboard item to chat."""
+        chat = chat or self.private
+        user = user or self.teleuser
+        chat.keyboard.menu_item(user, index, row=row)
+
     def private_command(self, cmd, from_user=None):
         """Call private command."""
         from_user = from_user or self.teleuser
         with self.app.test_request_context():
             private_command(cmd, from_user)
 
     def private_text(self, text, from_user=None):
```

