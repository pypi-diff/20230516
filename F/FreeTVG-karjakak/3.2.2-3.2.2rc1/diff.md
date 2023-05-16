# Comparing `tmp/FreeTVG-karjakak-3.2.2.tar.gz` & `tmp/FreeTVG-karjakak-3.2.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeTVG-karjakak-3.2.2.tar", last modified: Tue May 16 16:43:04 2023, max compression
+gzip compressed data, was "FreeTVG-karjakak-3.2.2rc1.tar", last modified: Mon May 15 16:00:34 2023, max compression
```

## Comparing `FreeTVG-karjakak-3.2.2.tar` & `FreeTVG-karjakak-3.2.2rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-16 16:43:04.559797 FreeTVG-karjakak-3.2.2/
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-16 16:43:04.555327 FreeTVG-karjakak-3.2.2/FreeTVG_karjakak.egg-info/
--rw-r--r--   0 karja      (501) staff       (20)     1448 2023-05-16 16:43:04.000000 FreeTVG-karjakak-3.2.2/FreeTVG_karjakak.egg-info/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      463 2023-05-16 16:43:04.000000 FreeTVG-karjakak-3.2.2/FreeTVG_karjakak.egg-info/SOURCES.txt
--rw-r--r--   0 karja      (501) staff       (20)        1 2023-05-16 16:43:04.000000 FreeTVG-karjakak-3.2.2/FreeTVG_karjakak.egg-info/dependency_links.txt
--rw-r--r--   0 karja      (501) staff       (20)       29 2023-05-16 16:43:04.000000 FreeTVG-karjakak-3.2.2/FreeTVG_karjakak.egg-info/entry_points.txt
--rw-r--r--   0 karja      (501) staff       (20)      136 2023-05-16 16:43:04.000000 FreeTVG-karjakak-3.2.2/FreeTVG_karjakak.egg-info/requires.txt
--rw-r--r--   0 karja      (501) staff       (20)        4 2023-05-16 16:43:04.000000 FreeTVG-karjakak-3.2.2/FreeTVG_karjakak.egg-info/top_level.txt
--rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.2.2/LICENSE.txt
--rw-r--r--   0 karja      (501) staff       (20)     1448 2023-05-16 16:43:04.559874 FreeTVG-karjakak-3.2.2/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.2.2/README.md
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-16 16:43:04.557616 FreeTVG-karjakak-3.2.2/TVG/
--rw-r--r--   0 karja      (501) staff       (20)   146625 2023-05-16 06:24:11.000000 FreeTVG-karjakak-3.2.2/TVG/FreeTVG.py
--rw-r--r--   0 karja      (501) staff       (20)   359943 2023-01-16 15:03:13.000000 FreeTVG-karjakak-3.2.2/TVG/Tutorial TVG.pdf
--rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.2.2/TVG/__init__.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-16 16:43:04.558107 FreeTVG-karjakak-3.2.2/TVG/structure/
--rw-r--r--   0 karja      (501) staff       (20)       82 2023-05-14 08:59:37.000000 FreeTVG-karjakak-3.2.2/TVG/structure/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)    14894 2023-05-16 16:03:03.000000 FreeTVG-karjakak-3.2.2/TVG/structure/frame_layouts.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-16 16:43:04.558800 FreeTVG-karjakak-3.2.2/TVG/utility/
--rw-r--r--   0 karja      (501) staff       (20)      923 2023-05-16 14:56:03.000000 FreeTVG-karjakak-3.2.2/TVG/utility/RegMail.py
--rw-r--r--   0 karja      (501) staff       (20)       84 2023-05-15 12:31:08.000000 FreeTVG-karjakak-3.2.2/TVG/utility/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)     5639 2023-01-12 09:34:49.000000 FreeTVG-karjakak-3.2.2/TVG/utility/mdh.py
--rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.2.2/pyproject.toml
--rw-r--r--   0 karja      (501) staff       (20)      960 2023-05-16 16:43:04.560164 FreeTVG-karjakak-3.2.2/setup.cfg
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 16:00:34.174347 FreeTVG-karjakak-3.2.2rc1/
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 16:00:34.169376 FreeTVG-karjakak-3.2.2rc1/FreeTVG_karjakak.egg-info/
+-rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-15 16:00:34.000000 FreeTVG-karjakak-3.2.2rc1/FreeTVG_karjakak.egg-info/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      463 2023-05-15 16:00:34.000000 FreeTVG-karjakak-3.2.2rc1/FreeTVG_karjakak.egg-info/SOURCES.txt
+-rw-r--r--   0 karja      (501) staff       (20)        1 2023-05-15 16:00:34.000000 FreeTVG-karjakak-3.2.2rc1/FreeTVG_karjakak.egg-info/dependency_links.txt
+-rw-r--r--   0 karja      (501) staff       (20)       29 2023-05-15 16:00:34.000000 FreeTVG-karjakak-3.2.2rc1/FreeTVG_karjakak.egg-info/entry_points.txt
+-rw-r--r--   0 karja      (501) staff       (20)      136 2023-05-15 16:00:34.000000 FreeTVG-karjakak-3.2.2rc1/FreeTVG_karjakak.egg-info/requires.txt
+-rw-r--r--   0 karja      (501) staff       (20)        4 2023-05-15 16:00:34.000000 FreeTVG-karjakak-3.2.2rc1/FreeTVG_karjakak.egg-info/top_level.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.2.2rc1/LICENSE.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-15 16:00:34.174476 FreeTVG-karjakak-3.2.2rc1/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.2.2rc1/README.md
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 16:00:34.172040 FreeTVG-karjakak-3.2.2rc1/TVG/
+-rw-r--r--   0 karja      (501) staff       (20)   146625 2023-05-15 15:59:19.000000 FreeTVG-karjakak-3.2.2rc1/TVG/FreeTVG.py
+-rw-r--r--   0 karja      (501) staff       (20)   359943 2023-01-16 15:03:13.000000 FreeTVG-karjakak-3.2.2rc1/TVG/Tutorial TVG.pdf
+-rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.2.2rc1/TVG/__init__.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 16:00:34.172712 FreeTVG-karjakak-3.2.2rc1/TVG/structure/
+-rw-r--r--   0 karja      (501) staff       (20)       82 2023-05-14 08:59:37.000000 FreeTVG-karjakak-3.2.2rc1/TVG/structure/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)    15881 2023-05-15 09:34:19.000000 FreeTVG-karjakak-3.2.2rc1/TVG/structure/frame_layouts.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-15 16:00:34.174024 FreeTVG-karjakak-3.2.2rc1/TVG/utility/
+-rw-r--r--   0 karja      (501) staff       (20)     1091 2022-12-04 14:36:50.000000 FreeTVG-karjakak-3.2.2rc1/TVG/utility/RegMail.py
+-rw-r--r--   0 karja      (501) staff       (20)       84 2023-05-15 12:31:08.000000 FreeTVG-karjakak-3.2.2rc1/TVG/utility/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)     5639 2023-01-12 09:34:49.000000 FreeTVG-karjakak-3.2.2rc1/TVG/utility/mdh.py
+-rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.2.2rc1/pyproject.toml
+-rw-r--r--   0 karja      (501) staff       (20)      963 2023-05-15 16:00:34.174806 FreeTVG-karjakak-3.2.2rc1/setup.cfg
```

### Comparing `FreeTVG-karjakak-3.2.2/FreeTVG_karjakak.egg-info/PKG-INFO` & `FreeTVG-karjakak-3.2.2rc1/FreeTVG_karjakak.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.2.2
+Version: 3.2.2rc1
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.2.2/LICENSE.txt` & `FreeTVG-karjakak-3.2.2rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.2/PKG-INFO` & `FreeTVG-karjakak-3.2.2rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.2.2
+Version: 3.2.2rc1
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.2.2/README.md` & `FreeTVG-karjakak-3.2.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.2/TVG/FreeTVG.py` & `FreeTVG-karjakak-3.2.2rc1/TVG/FreeTVG.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.2/TVG/Tutorial TVG.pdf` & `FreeTVG-karjakak-3.2.2rc1/TVG/Tutorial TVG.pdf`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.2/TVG/structure/frame_layouts.py` & `FreeTVG-karjakak-3.2.2rc1/TVG/structure/frame_layouts.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     def __init__(self, root):
         super().__init__()
         self.pack(side=TOP, fill="x")
         self.label = ttk.Label(self, text="Words")
         self.label.pack(side=LEFT, pady=3, fill="x")
         self.entry = ttk.Entry(
             self,
-            validate="none",
+            validate="focusin",
             validatecommand=self.focus,
             font="consolas 12",
         )
         self.entry.pack(side=LEFT, ipady=5, pady=(3, 1), fill="both", expand=1)
         self.entry.config(state="disable")
 
         self.rb = StringVar()
@@ -75,51 +75,66 @@
             case = ["child", "parent"]
             if self.entry.get() in case:
                 self.entry.delete(0, END)
                 return True
             else:
                 return False
 
-    def _make_entry(self, ch: bool = True):
-        if str(self.entry["state"]) == "disable":
-            self.entry.configure(state="normal")
-        if ch:
-            self.entry3.config(state="normal")
-            self.entry3.config(values=tuple([f"child{c}" for c in range(1, 51)]))
-            self.entry3.current(0)
-            self.entry3.config(state="readonly")
-        else:
-            self.entry3.config(state="normal")
-            self.entry3.config(values="")
-            self.entry3.delete(0, END)
-            self.entry3.config(state="readonly")
-        self.entry.configure(validate="focusin")
-
     def radiobut(self, event=None):
         """These are the switches on radio buttons, to apply certain rule on child"""
 
-        match self.rb.get():
-            case "parent":
-                match w := self.entry.get():
-                    case "child" | "":
-                        self._make_entry(False)
-                        if w:
-                            self.entry.delete(0, END)
-                        self.entry.insert(0, "parent")
-                    case w if w != "parent":
-                        self._make_entry(False)
-            case "child":
-                match w := self.entry.get():
-                    case "parent" | "":
-                        self._make_entry()
-                        if w:
-                            self.entry.delete(0, END)
-                        self.entry.insert(0, "child")
-                    case w if w != "child":
-                        self._make_entry()
+        match (self.rb.get(), str(self.entry.cget("state")), self.entry.get()):
+            case ("parent", "disable", _):
+                self.entry.config(state="normal")
+                self.entry.insert(0, "parent")
+            case ("child", "disable", _):
+                self.entry.config(state="normal")
+                self.entry.insert(0, "child")
+                self.entry3.config(state="normal")
+                self.entry3.config(values=tuple([f"child{c}" for c in range(1, 51)]))
+                self.entry3.current(0)
+                self.entry3.config(state="readonly")
+            case ("parent", _, "child"):
+                self.entry.delete(0, END)
+                self.entry.insert(0, "parent")
+                self.entry3.config(state="normal")
+                self.entry3.config(values="")
+                self.entry3.delete(0, END)
+                self.entry3.config(state="readonly")
+            case ("child", _, "parent"):
+                self.entry.delete(0, END)
+                self.entry.insert(0, "child")
+                self.entry3.config(state="normal")
+                self.entry3.config(values=tuple([f"child{c}" for c in range(1, 51)]))
+                self.entry3.current(0)
+                self.entry3.config(state="readonly")
+            case ("parent", _, ""):
+                self.entry.insert(0, "parent")
+                self.entry3.config(state="normal")
+                self.entry3.config(values="")
+                self.entry3.delete(0, END)
+                self.entry3.config(state="readonly")
+            case ("child", _, ""):
+                self.entry.insert(0, "child")
+                self.entry3.config(state="normal")
+                self.entry3.config(values=tuple([f"child{c}" for c in range(1, 51)]))
+                self.entry3.current(0)
+                self.entry3.config(state="readonly")
+            case ("parent", _, _):
+                self.entry3.config(state="normal")
+                self.entry3.config(values="")
+                self.entry3.delete(0, END)
+                self.entry3.config(state="readonly")
+            case ("child", _, _):
+                self.entry3.config(state="normal")
+                self.entry3.config(values=tuple([f"child{c}" for c in range(1, 51)]))
+                self.entry3.current(0)
+                self.entry3.config(state="readonly")
+
+        self.entry.configure(validate="focusin")
 
 
 @excpcls(m=2, filenm=DEFAULTFILE)
 class Lay2(ttk.Frame):
     def __init__(self, root):
         super().__init__()
         self.pack(side=TOP, fill="x")
```

### Comparing `FreeTVG-karjakak-3.2.2/TVG/utility/RegMail.py` & `FreeTVG-karjakak-3.2.2rc1/TVG/utility/RegMail.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 def composemail(sub: str, body: str):
     subject = f"[TVG]-{sub}"
     if platform.startswith("win"):
         # For default Windows "Mail" app
         webbrowser.open(f"mailto:?subject={subject}&body={parse.quote(body)}", new=1)
     else:
         # For default MacOsX default "Mail" app
-        body = demoji.replace_with_desc(body).strip().replace('"', "'")
+        if body.encode("unicode_escape").decode().partition("\\U")[1]:
+            body = f"{demoji.replace_with_desc(body)!r}".strip().replace('"', "'")[1:-1]
+        else:
+            body = f"{body!r}".strip().replace('"', "'")[1:-1]
         webbrowser.open(f"mailto:?subject={subject}&body={body}", new=1)
 
 
 def wrwords(text: str, wd: int, num: int):
     regex = re.compile(r"\s+")
     get = regex.match(text)
     if get:
```

### Comparing `FreeTVG-karjakak-3.2.2/TVG/utility/mdh.py` & `FreeTVG-karjakak-3.2.2rc1/TVG/utility/mdh.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.2/setup.cfg` & `FreeTVG-karjakak-3.2.2rc1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FreeTVG-karjakak
-version = 3.2.2
+version = 3.2.2rc1
 author = karjakak
 author_email = kakkarja.github@gmail.com
 description = Tree View Gui for outline treeview note.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kakkarja/FreeTVG#latest-notice
 license = MIT License
```

