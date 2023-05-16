# Comparing `tmp/AISAPLibrary-1.0.5.tar.gz` & `tmp/AISAPLibrary-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Annas\SAP Modified\Build Wheel\AISAPLibrary\dist\.tmp-gcxn1g69\AISAPLibrary-1.0.5.tar", last modified: Tue May 16 04:03:17 2023, max compression
+gzip compressed data, was "D:\Annas\SAP Modified\Build Wheel\AISAPLibrary\dist\.tmp-1bms58zz\AISAPLibrary-1.0.6.tar", last modified: Tue May 16 04:33:01 2023, max compression
```

## Comparing `AISAPLibrary-1.0.5.tar` & `AISAPLibrary-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/
--rw-rw-rw-   0        0        0      310 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-03-13 07:56:31.000000 AISAPLibrary-1.0.5/README.md
--rw-rw-rw-   0        0        0      482 2023-05-16 04:02:45.000000 AISAPLibrary-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/src/AISAPLibrary/
--rw-rw-rw-   0        0        0    48431 2023-05-16 04:00:46.000000 AISAPLibrary-1.0.5/src/AISAPLibrary/AISAPLibrary.py
--rw-rw-rw-   0        0        0       38 2023-03-10 07:38:40.000000 AISAPLibrary-1.0.5/src/AISAPLibrary/__init__.py
--rw-rw-rw-   0        0        0      497 2023-05-16 03:58:34.000000 AISAPLibrary-1.0.5/src/AISAPLibrary/send_vkey_multithread.py
-drwxrwxrwx   0        0        0        0 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/src/AISAPLibrary.egg-info/
--rw-rw-rw-   0        0        0      310 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/src/AISAPLibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/src/AISAPLibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/src/AISAPLibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/src/AISAPLibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/
+-rw-rw-rw-   0        0        0      310 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-03-13 07:56:31.000000 AISAPLibrary-1.0.6/README.md
+-rw-rw-rw-   0        0        0      482 2023-05-16 04:32:41.000000 AISAPLibrary-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/src/AISAPLibrary/
+-rw-rw-rw-   0        0        0    50334 2023-05-16 04:30:54.000000 AISAPLibrary-1.0.6/src/AISAPLibrary/AISAPLibrary.py
+-rw-rw-rw-   0        0        0       38 2023-03-10 07:38:40.000000 AISAPLibrary-1.0.6/src/AISAPLibrary/__init__.py
+-rw-rw-rw-   0        0        0      497 2023-05-16 03:58:34.000000 AISAPLibrary-1.0.6/src/AISAPLibrary/send_vkey_multithread.py
+drwxrwxrwx   0        0        0        0 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/src/AISAPLibrary.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/src/AISAPLibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/src/AISAPLibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/src/AISAPLibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-16 04:33:01.000000 AISAPLibrary-1.0.6/src/AISAPLibrary.egg-info/top_level.txt
```

### Comparing `AISAPLibrary-1.0.5/src/AISAPLibrary/AISAPLibrary.py` & `AISAPLibrary-1.0.6/src/AISAPLibrary/AISAPLibrary.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,26 +104,60 @@
         if self.connection.Description == connection_name:
             self.session = self.connection.children(0)
         else:
             self.take_screenshot()
             message = "No existing connection for '%s' found." % connection_name
             raise ValueError(message)
         
-    def get_element_type_other_session(self, element_id, session_num='0'):
+    def doubleclick_element_other_session(self, element_id, item_id, column_id, session_num='1'):
+        """Performs a double-click on a given element. Used only for shell objects.
+        """
+
+        # Performing the correct method on an element, depending on the type of element
+        element_type = self.get_element_type_other_session(element_id,session_num=session_num)
+        if element_type == "GuiShell":
+            self.connection.children(int(session_num)).findById(element_id).doubleClickItem(item_id, column_id)
+        else:
+            self.take_screenshot()
+            message = "You cannot use 'doubleclick element' on element type '%s', maybe use 'click element' instead?" % element_type
+            raise Warning(message)
+        time.sleep(self.explicit_wait)
+        
+    def click_element_other_session(self, element_id, session_num='1'):
+        """Performs a single click on a given element. Used only for buttons, tabs and menu items.
+
+        In case you want to change a value of an element like checkboxes of selecting an option in dropdown lists,
+        use `select checkbox` or `select from list by label` instead.
+        """
+
+        # Performing the correct method on an element, depending on the type of element
+        element_type = self.get_element_type_other_session(element_id,session_num=session_num)
+        if (element_type == "GuiTab"
+                or element_type == "GuiMenu"):
+            self.connection.children(int(session_num)).findById(element_id).select()
+        elif element_type == "GuiButton":
+            self.connection.children(int(session_num)).findById(element_id).press()
+        else:
+            self.take_screenshot()
+            message = "You cannot use 'click_element' on element type '%s', maybe use 'select checkbox' instead?" % element_type
+            raise Warning(message)
+        time.sleep(self.explicit_wait)
+        
+    def get_element_type_other_session(self, element_id, session_num='1'):
         """Returns the Sap element type for the given element.
         """
         try:
             type = self.connection.children(int(session_num)).findById(element_id).type
             return type
         except com_error:
             self.take_screenshot()
             message = "Cannot find element with id '%s'" % element_id
             raise ValueError(message)
         
-    def input_text_other_session(self, element_id, text,  session_num='0'):
+    def input_text_other_session(self, element_id, text,  session_num='1'):
         """Inserts the given text into the text field identified by locator.
         Use keyword `input password` to insert a password in a text field.
         """
         element_type = self.get_element_type_other_session(element_id,session_num=session_num)
         if (element_type == "GuiTextField"
                 or element_type == "GuiCTextField"
                 or element_type == "GuiShell"
@@ -132,27 +166,27 @@
             logger.info("Typing text '%s' into text field '%s'." % (text, element_id))
             time.sleep(self.explicit_wait)
         else:
             self.take_screenshot()
             message = "Cannot use keyword 'input text' for element type '%s'" % element_type
             raise ValueError(message)
         
-    def select_radio_button_other_session(self, element_id, session_num='0'):
+    def select_radio_button_other_session(self, element_id, session_num='1'):
         """Sets radio button to the specified value.
         """
         element_type = self.get_element_type_other_session(element_id,session_num=session_num)
         if element_type == "GuiRadioButton":
             self.connection.children(int(session_num)).findById(element_id).selected = True
         else:
             self.take_screenshot()
             message = "Cannot use keyword 'select radio button' for element type '%s'" % element_type
             raise ValueError(message)
         time.sleep(self.explicit_wait)
         
-    def run_transaction_other_session(self, transaction, session_num='0'):
+    def run_transaction_other_session(self, transaction, session_num='1'):
         self.connection.children(int(session_num)).findById("wnd[0]/tbar[0]/okcd").text = transaction
         time.sleep(self.explicit_wait)
         self.send_vkey_other_session(0, session_num=session_num)
 
         if transaction == '/nex':
             return
 
@@ -160,15 +194,15 @@
         if pane_value in ("Transactie %s bestaat niet" % transaction.upper(),
                           "Transaction %s does not exist" % transaction.upper(),
                           "Transaktion %s existiert nicht" % transaction.upper()):
             self.take_screenshot()
             message = "Unknown transaction: '%s'" % transaction
             raise ValueError(message)
         
-    def send_vkey_other_session(self, vkey_id, window=0, session_num='0'):
+    def send_vkey_other_session(self, vkey_id, window=0, session_num='1'):
         vkey_id = str(vkey_id)
         vkeys_array = ["ENTER", "F1", "F2", "F3", "F4", "F5", "F6", "F7", "F8", "F9", "F10", "F11", "F12",
                        None, "SHIFT+F2", "SHIFT+F3", "SHIFT+F4", "SHIFT+F5", "SHIFT+F6", "SHIFT+F7", "SHIFT+F8",
                        "SHIFT+F9", "CTRL+SHIFT+0", "SHIFT+F11", "SHIFT+F12", "CTRL+F1", "CTRL+F2", "CTRL+F3", "CTRL+F4",
                        "CTRL+F5", "CTRL+F6", "CTRL+F7", "CTRL+F8", "CTRL+F9", "CTRL+F10", "CTRL+F11", "CTRL+F12",
                        "CTRL+SHIFT+F1", "CTRL+SHIFT+F2", "CTRL+SHIFT+F3", "CTRL+SHIFT+F4", "CTRL+SHIFT+F5",
                        "CTRL+SHIFT+F6", "CTRL+SHIFT+F7", "CTRL+SHIFT+F8", "CTRL+SHIFT+F9", "CTRL+SHIFT+F10",
@@ -202,15 +236,15 @@
             self.connection.children(int(session_num)).findById("wnd[% s]" % window).sendVKey(vkey_id)
         except com_error:
             self.take_screenshot()
             message = "Cannot send Vkey to given window, is window wnd[% s] actually open?" % window
             raise ValueError(message)
         time.sleep(self.explicit_wait)
         
-    def send_vkey_other_session_process(self, vkey_id, window=0, session_num='0'):
+    def send_vkey_other_session_process(self, vkey_id, window=0, session_num='1'):
         Popen(["python", os.path.dirname(os.path.realpath(__file__))+'\\send_vkey_multithread.py',self.connection_name,vkey_id,str(window),session_num])
         
     def connect_to_session(self, explicit_wait=0):
         """Connects to an open session SAP.
 
         See `Opening a connection / Before running tests` for details about requirements before connecting to a session.
```

