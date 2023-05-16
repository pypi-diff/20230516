# Comparing `tmp/AISAPLibrary-1.0.4.tar.gz` & `tmp/AISAPLibrary-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Annas\SAP Modified\Build Wheel\AISAPLibrary\dist\.tmp-u2ad2y4k\AISAPLibrary-1.0.4.tar", last modified: Wed May 10 04:22:06 2023, max compression
+gzip compressed data, was "D:\Annas\SAP Modified\Build Wheel\AISAPLibrary\dist\.tmp-gcxn1g69\AISAPLibrary-1.0.5.tar", last modified: Tue May 16 04:03:17 2023, max compression
```

## Comparing `AISAPLibrary-1.0.4.tar` & `AISAPLibrary-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 04:22:06.000000 AISAPLibrary-1.0.4/
--rw-rw-rw-   0        0        0      315 2023-05-10 04:22:06.000000 AISAPLibrary-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-03-13 07:56:31.000000 AISAPLibrary-1.0.4/README.md
--rw-rw-rw-   0        0        0      487 2023-05-10 04:21:43.000000 AISAPLibrary-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 04:22:06.000000 AISAPLibrary-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 04:22:06.000000 AISAPLibrary-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 04:22:06.000000 AISAPLibrary-1.0.4/src/AISAPLibrary/
--rw-rw-rw-   0        0        0    42634 2023-05-10 03:45:13.000000 AISAPLibrary-1.0.4/src/AISAPLibrary/AISAPLibrary.py
--rw-rw-rw-   0        0        0       38 2023-03-10 07:38:40.000000 AISAPLibrary-1.0.4/src/AISAPLibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 04:22:06.000000 AISAPLibrary-1.0.4/src/AISAPLibrary.egg-info/
--rw-rw-rw-   0        0        0      315 2023-05-10 04:22:06.000000 AISAPLibrary-1.0.4/src/AISAPLibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-05-10 04:22:06.000000 AISAPLibrary-1.0.4/src/AISAPLibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 04:22:06.000000 AISAPLibrary-1.0.4/src/AISAPLibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-10 04:22:06.000000 AISAPLibrary-1.0.4/src/AISAPLibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/
+-rw-rw-rw-   0        0        0      310 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-03-13 07:56:31.000000 AISAPLibrary-1.0.5/README.md
+-rw-rw-rw-   0        0        0      482 2023-05-16 04:02:45.000000 AISAPLibrary-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/src/AISAPLibrary/
+-rw-rw-rw-   0        0        0    48431 2023-05-16 04:00:46.000000 AISAPLibrary-1.0.5/src/AISAPLibrary/AISAPLibrary.py
+-rw-rw-rw-   0        0        0       38 2023-03-10 07:38:40.000000 AISAPLibrary-1.0.5/src/AISAPLibrary/__init__.py
+-rw-rw-rw-   0        0        0      497 2023-05-16 03:58:34.000000 AISAPLibrary-1.0.5/src/AISAPLibrary/send_vkey_multithread.py
+drwxrwxrwx   0        0        0        0 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/src/AISAPLibrary.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/src/AISAPLibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/src/AISAPLibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/src/AISAPLibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-16 04:03:17.000000 AISAPLibrary-1.0.5/src/AISAPLibrary.egg-info/top_level.txt
```

### Comparing `AISAPLibrary-1.0.4/src/AISAPLibrary/AISAPLibrary.py` & `AISAPLibrary-1.0.5/src/AISAPLibrary/AISAPLibrary.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,14 +45,15 @@
             'Popup Change Password' : 'Failed to login, Please create new password!',
             'Failed Login Attempt' : 'Success Login'
         }
 
         self.sapapp = -1
         self.session = -1
         self.connection = -1
+        self.connection_name = None
 
         self.take_screenshots = screenshots_on_error
         self.screenshot = screenshot.Screenshot()
 
         if screenshot_directory is not None:
             if not os.path.exists(screenshot_directory):
                 os.makedirs(screenshot_directory)
@@ -102,15 +103,116 @@
         self.connection = self.sapapp.Children(0)
         if self.connection.Description == connection_name:
             self.session = self.connection.children(0)
         else:
             self.take_screenshot()
             message = "No existing connection for '%s' found." % connection_name
             raise ValueError(message)
+        
+    def get_element_type_other_session(self, element_id, session_num='0'):
+        """Returns the Sap element type for the given element.
+        """
+        try:
+            type = self.connection.children(int(session_num)).findById(element_id).type
+            return type
+        except com_error:
+            self.take_screenshot()
+            message = "Cannot find element with id '%s'" % element_id
+            raise ValueError(message)
+        
+    def input_text_other_session(self, element_id, text,  session_num='0'):
+        """Inserts the given text into the text field identified by locator.
+        Use keyword `input password` to insert a password in a text field.
+        """
+        element_type = self.get_element_type_other_session(element_id,session_num=session_num)
+        if (element_type == "GuiTextField"
+                or element_type == "GuiCTextField"
+                or element_type == "GuiShell"
+                or element_type == "GuiPasswordField"):
+            self.connection.children(int(session_num)).findById(element_id).text = text
+            logger.info("Typing text '%s' into text field '%s'." % (text, element_id))
+            time.sleep(self.explicit_wait)
+        else:
+            self.take_screenshot()
+            message = "Cannot use keyword 'input text' for element type '%s'" % element_type
+            raise ValueError(message)
+        
+    def select_radio_button_other_session(self, element_id, session_num='0'):
+        """Sets radio button to the specified value.
+        """
+        element_type = self.get_element_type_other_session(element_id,session_num=session_num)
+        if element_type == "GuiRadioButton":
+            self.connection.children(int(session_num)).findById(element_id).selected = True
+        else:
+            self.take_screenshot()
+            message = "Cannot use keyword 'select radio button' for element type '%s'" % element_type
+            raise ValueError(message)
+        time.sleep(self.explicit_wait)
+        
+    def run_transaction_other_session(self, transaction, session_num='0'):
+        self.connection.children(int(session_num)).findById("wnd[0]/tbar[0]/okcd").text = transaction
+        time.sleep(self.explicit_wait)
+        self.send_vkey_other_session(0, session_num=session_num)
+
+        if transaction == '/nex':
+            return
 
+        pane_value = self.connection.children(int(session_num)).findById("wnd[0]/sbar/pane[0]").text
+        if pane_value in ("Transactie %s bestaat niet" % transaction.upper(),
+                          "Transaction %s does not exist" % transaction.upper(),
+                          "Transaktion %s existiert nicht" % transaction.upper()):
+            self.take_screenshot()
+            message = "Unknown transaction: '%s'" % transaction
+            raise ValueError(message)
+        
+    def send_vkey_other_session(self, vkey_id, window=0, session_num='0'):
+        vkey_id = str(vkey_id)
+        vkeys_array = ["ENTER", "F1", "F2", "F3", "F4", "F5", "F6", "F7", "F8", "F9", "F10", "F11", "F12",
+                       None, "SHIFT+F2", "SHIFT+F3", "SHIFT+F4", "SHIFT+F5", "SHIFT+F6", "SHIFT+F7", "SHIFT+F8",
+                       "SHIFT+F9", "CTRL+SHIFT+0", "SHIFT+F11", "SHIFT+F12", "CTRL+F1", "CTRL+F2", "CTRL+F3", "CTRL+F4",
+                       "CTRL+F5", "CTRL+F6", "CTRL+F7", "CTRL+F8", "CTRL+F9", "CTRL+F10", "CTRL+F11", "CTRL+F12",
+                       "CTRL+SHIFT+F1", "CTRL+SHIFT+F2", "CTRL+SHIFT+F3", "CTRL+SHIFT+F4", "CTRL+SHIFT+F5",
+                       "CTRL+SHIFT+F6", "CTRL+SHIFT+F7", "CTRL+SHIFT+F8", "CTRL+SHIFT+F9", "CTRL+SHIFT+F10",
+                       "CTRL+SHIFT+F11", "CTRL+SHIFT+F12", None, None, None, None, None, None, None, None, None, None,
+                       None, None, None, None, None, None, None, None, None, None, None, "CTRL+E", "CTRL+F", "CTRL+A",
+                       "CTRL+D", "CTRL+N", "CTRL+O", "SHIFT+DEL", "CTRL+INS", "SHIFT+INS", "ALT+BACKSPACE",
+                       "CTRL+PAGEUP", "PAGEUP",
+                       "PAGEDOWN", "CTRL+PAGEDOWN", "CTRL+G", "CTRL+R", "CTRL+P", "CTRL+B", "CTRL+K", "CTRL+T",
+                       "CTRL+Y",
+                       "CTRL+X", "CTRL+C", "CTRL+V", "SHIFT+F10", None, None, "CTRL+#"]
+
+        # If a key combi is given, replace vkey_id by correct id based on given combination
+        if not vkey_id.isdigit():
+            search_comb = vkey_id.upper()
+            search_comb = search_comb.replace(" ", "")
+            search_comb = search_comb.replace("CONTROL", "CTRL")
+            search_comb = search_comb.replace("DELETE", "DEL")
+            search_comb = search_comb.replace("INSERT", "INS")
+            try:
+                vkey_id = vkeys_array.index(search_comb)
+            except ValueError:
+                if search_comb == "CTRL+S":
+                    vkey_id = 11
+                elif search_comb == "ESC":
+                    vkey_id = 12
+                else:
+                    message = "Cannot find given Vkey, provide a valid Vkey number or combination"
+                    raise ValueError(message)
+
+        try:
+            self.connection.children(int(session_num)).findById("wnd[% s]" % window).sendVKey(vkey_id)
+        except com_error:
+            self.take_screenshot()
+            message = "Cannot send Vkey to given window, is window wnd[% s] actually open?" % window
+            raise ValueError(message)
+        time.sleep(self.explicit_wait)
+        
+    def send_vkey_other_session_process(self, vkey_id, window=0, session_num='0'):
+        Popen(["python", os.path.dirname(os.path.realpath(__file__))+'\\send_vkey_multithread.py',self.connection_name,vkey_id,str(window),session_num])
+        
     def connect_to_session(self, explicit_wait=0):
         """Connects to an open session SAP.
 
         See `Opening a connection / Before running tests` for details about requirements before connecting to a session.
 
         Optionally `set explicit wait` can be used to set the explicit wait time.
 
@@ -861,14 +963,17 @@
             except :
                 time.sleep(2)
         
         if self.sapapp == -1:
             raise RuntimeError('Cannot connect to session')
 
         self.open_connection(config['connection'])
+        
+        self.connection_name = config['connection']
+        
         self.input_text("wnd[0]/usr/txtRSYST-BNAME",config["username"])
         self.input_password("wnd[0]/usr/pwdRSYST-BCODE",config["password"])
         self.input_text("wnd[0]/usr/txtRSYST-MANDT",config['client'])
         self.send_vkey(0)
 
         time.sleep(time_wait)
```

