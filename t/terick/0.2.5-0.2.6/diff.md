# Comparing `tmp/terick-0.2.5.tar.gz` & `tmp/terick-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terick-0.2.5.tar", last modified: Fri May 12 18:24:37 2023, max compression
+gzip compressed data, was "terick-0.2.6.tar", last modified: Tue May 16 11:10:51 2023, max compression
```

## Comparing `terick-0.2.5.tar` & `terick-0.2.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 18:24:37.374349 terick-0.2.5/
--rw-rw-rw-   0        0        0      470 2023-05-12 18:24:37.372987 terick-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-05-05 21:36:01.000000 terick-0.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-12 18:24:37.374349 terick-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      887 2023-05-12 18:24:10.000000 terick-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:24:37.366077 terick-0.2.5/terick/
--rw-rw-rw-   0        0        0     8142 2023-05-12 18:06:52.000000 terick-0.2.5/terick/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 18:24:37.370986 terick-0.2.5/terick.egg-info/
--rw-rw-rw-   0        0        0      470 2023-05-12 18:24:37.000000 terick-0.2.5/terick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-05-12 18:24:37.000000 terick-0.2.5/terick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 18:24:37.000000 terick-0.2.5/terick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-12 18:24:37.000000 terick-0.2.5/terick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 11:10:51.367541 terick-0.2.6/
+-rw-rw-rw-   0        0        0      909 2023-05-16 11:10:51.367541 terick-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-05-16 11:08:07.000000 terick-0.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 11:10:51.371053 terick-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      927 2023-05-16 11:10:34.000000 terick-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:10:51.347881 terick-0.2.6/terick/
+-rw-rw-rw-   0        0        0     8760 2023-05-16 11:05:31.000000 terick-0.2.6/terick/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:10:51.367541 terick-0.2.6/terick.egg-info/
+-rw-rw-rw-   0        0        0      909 2023-05-16 11:10:51.000000 terick-0.2.6/terick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-05-16 11:10:51.000000 terick-0.2.6/terick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 11:10:51.000000 terick-0.2.6/terick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 11:10:51.000000 terick-0.2.6/terick.egg-info/top_level.txt
```

### Comparing `terick-0.2.5/setup.py` & `terick-0.2.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.5'
+VERSION = '0.2.6'
 DESCRIPTION = 'Package full of simple functions'
 
 # Setting up
 setup(
     name="terick",
     version=VERSION,
     author="HaxoTF",
     author_email="<haxotf@gmail.com>",
     description=DESCRIPTION,
+    long_description=long_description,
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'regular', 'helper'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
```

### Comparing `terick-0.2.5/terick/__init__.py` & `terick-0.2.6/terick/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,23 +54,33 @@
     return int(result)
 
 # --- toggle bool v1.0
 def toggle(var:bool):
     if var: return False
     else: return True
 
-# --- unit 1.0
+# --- short num 1.0v
 def short_num(number:float):
     units = "KMBT"
+
+    if number<1000: return str(int(number))
+    for u in units:
+        if number>=1000: number /= 1000
+        if number<1000: return str(int(number))+u
+    return str(int(number))+units[-1]
+
+# --- short bytes 1.0v
+def short_bytes(nbytes:int):
+    units = "KMGTP"
+
+    if nbytes<1024: return str(int(nbytes))+"B"
     for u in units:
-        if number>=1000:
-            number = int(number/1000)
-            if number<1000: return str(number)+u
-        else: return str(number)
-    return str(number)+units[-1]
+        if nbytes>=1024: nbytes /= 1024
+        if nbytes<1024: return str(int(nbytes))+u+"B"
+    return str(int(nbytes))+units[-1]+"B"
 
 # --- string limit v1.0
 def limit_str(text:str, max:int):
     result = ""
     if len(text)<max: return text
 
     for i in range(0, max):
@@ -105,17 +115,40 @@
 
 # --- divide time v1.0
 def div_time(seconds:float, as_text=False):
     s = int(seconds)
     m = int(seconds/60); s -= m*60
     h = int(m/60); m -= h*60
 
-    if as_text: return f"{h}h {m}m {s}s"
+    if as_text:
+        result = ""
+        if h>0: result += f"{h}h "
+        if m>0: result += f"{m}m "
+        if s>0 or (m==0 and h==0): result += f"{s}s "
+
+        return result
+
     else: return h, m, s
 
+# --- get most common v1.0
+def sort_by_rarity(values:list):
+
+    items = count_items(values)
+    copy = items
+    result = []
+    
+    for item in items:
+        index = 0
+        for i in range(0, len(copy)):
+            if copy[i][1]>copy[index][1]: index = i
+            
+        result.append(copy.pop(index)[0])
+    return result
+
+
 # ----====[ Numbers ]====----
 
 
 # --- number limit v1.0
 def limit(value:float, min:float, max:float):
     if value>max: return max
     if value<min: return min
@@ -159,43 +192,52 @@
             if len(result)+1<len(data): result.append(unlist_words(line)+"\n")
             else: result.append(unlist_words(line))
         f.writelines(result)
     f.close()
 
 # --- zip directory v1.0
 def zipdir(dir:str, filename:str):
-    walkvar = file_walk(dir)
+    walkvar = scan_dir(dir)
 
     zipf = zip.ZipFile(filename, "w")
     for file in walkvar:
         zipf.write(file, compress_type=zip.ZIP_DEFLATED)
     zipf.close()
 
 # --- unzip v1.0
 def unzip(dir_from:str, dir_to:str):
     zipf = zip.ZipFile(dir_from)
     zipf.extractall(dir_to)
     zipf.close()
 
 # --- file walk v1.0
-def file_walk(dir:str, catch_folders=False):
+def scan_dir(dir:str, catch_folders=False):
     walkvar = []
     
     def walk(dir:str):
         for f in os.listdir(dir):
             
             path = f"{dir}/{f}"
             if os.path.isdir(path):
                 if catch_folders: walkvar.append(path)
                 walk(path)
             else:
                 walkvar.append(path)
     walk(dir)
     return walkvar
 
+# --- calc dir size
+def calc_dir_size(path:str):
+    result = 0
+    files = scan_dir(path)
+
+    for f in files:
+        result += os.path.getsize(f)
+    return result
+
 
 # ----====[ Math ]====----
 
 
 # -- get average v1.0
 def calc_avg(values:list):
     total = 0
@@ -243,30 +285,14 @@
     result = [None, 0]
 
     for item in items:
         if item[1]>result[1]: result = item
     
     return result[0]
 
-# get most common v1.0
-def sort_by_rarity(values:list):
-
-    items = count_items(values)
-    copy = items
-    result = []
-    
-    for item in items:
-        index = 0
-        for i in range(0, len(copy)):
-            if copy[i][1]>copy[index][1]: index = i
-            
-        result.append(copy.pop(index)[0])
-    return result
-
-
 # ----====[ Classes ]====----
 
 
 class Timer():
     def __init__(self):
         self.begin = time.time()
         self.end = self.begin
```

