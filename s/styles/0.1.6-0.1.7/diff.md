# Comparing `tmp/styles-0.1.6.tar.gz` & `tmp/styles-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "styles-0.1.6.tar", last modified: Sun Jan  8 13:20:15 2023, max compression
+gzip compressed data, was "styles-0.1.7.tar", last modified: Tue May 16 07:28:57 2023, max compression
```

## Comparing `styles-0.1.6.tar` & `styles-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-01-08 13:20:15.592401 styles-0.1.6/
--rw-rw-rw-   0        0        0      537 2023-01-08 13:20:15.591418 styles-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      437 2022-11-21 13:37:43.000000 styles-0.1.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-01-08 13:20:15.592401 styles-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-01-08 13:20:03.000000 styles-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-08 13:20:15.572402 styles-0.1.6/styles/
--rw-rw-rw-   0        0        0     9904 2022-12-08 10:55:10.000000 styles-0.1.6/styles/Style.py
--rw-rw-rw-   0        0        0      344 2022-11-22 13:39:29.000000 styles-0.1.6/styles/__init__.py
--rw-rw-rw-   0        0        0     1889 2022-12-06 08:06:09.000000 styles-0.1.6/styles/figures.py
--rw-rw-rw-   0        0        0     2302 2022-12-06 08:09:20.000000 styles-0.1.6/styles/osInfo.py
-drwxrwxrwx   0        0        0        0 2023-01-08 13:20:15.588400 styles-0.1.6/styles.egg-info/
--rw-rw-rw-   0        0        0      537 2023-01-08 13:20:15.000000 styles-0.1.6/styles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-01-08 13:20:15.000000 styles-0.1.6/styles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-08 13:20:15.000000 styles-0.1.6/styles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-01-08 13:20:15.000000 styles-0.1.6/styles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 07:28:57.919157 styles-0.1.7/
+-rw-rw-rw-   0        0        0      537 2023-05-16 07:28:57.917140 styles-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2022-11-21 13:37:43.000000 styles-0.1.7/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-16 07:28:57.920141 styles-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-05-16 07:28:26.000000 styles-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:28:57.890141 styles-0.1.7/styles/
+-rw-rw-rw-   0        0        0     9823 2023-05-16 07:19:25.000000 styles-0.1.7/styles/Style.py
+-rw-rw-rw-   0        0        0      346 2023-05-16 07:22:06.000000 styles-0.1.7/styles/__init__.py
+-rw-rw-rw-   0        0        0     1889 2022-12-06 08:06:09.000000 styles-0.1.7/styles/figures.py
+-rw-rw-rw-   0        0        0     2302 2022-12-06 08:09:20.000000 styles-0.1.7/styles/osInfo.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:28:57.914138 styles-0.1.7/styles.egg-info/
+-rw-rw-rw-   0        0        0      537 2023-05-16 07:28:57.000000 styles-0.1.7/styles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-16 07:28:57.000000 styles-0.1.7/styles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 07:28:57.000000 styles-0.1.7/styles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 07:28:57.000000 styles-0.1.7/styles.egg-info/top_level.txt
```

### Comparing `styles-0.1.6/PKG-INFO` & `styles-0.1.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: styles
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Style pack for python
 Home-page: https://github.com/Xtarii/PythonStylePack
 Author: Lord Alvin Hansen
 Author-email: alvin.hansen@elev.ga.ntig.se
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `styles-0.1.6/setup.py` & `styles-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='styles',
-    version='0.1.6',
+    version='0.1.7',
     description='A Style pack for python',
     url='https://github.com/Xtarii/PythonStylePack',
     author='Lord Alvin Hansen',
     author_email='alvin.hansen@elev.ga.ntig.se',
     license='BSD 2-clause',
     packages=['styles'],
```

### Comparing `styles-0.1.6/styles/Style.py` & `styles-0.1.7/styles/Style.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     """
 
     print(Colors["BOLD"] + text + " ", sep="", end="", flush=True)
     for x in range(times):
         for x in r"-\|/-\|/":
             print("\b", Colors["FAIL"] + x, sep="", end="", flush=True)
             time.sleep(sleep)
-    
+
     print("\b|", Colors["ENDC"] + "\n\n")
 
 
 #this is a loadingbar line
 def loadingbar_line(sleep=float(0.1), times=int(51), text=str("Loading: ")):
     """
     This is a animation of a loadingbar line: ############
@@ -68,15 +68,15 @@
     ends with two new lines, and the default color
     """
 
     print(Colors["BOLD"] + text + " ", sep="", end="", flush=True)
     for x in range(times):
         print(Colors["FAIL"] + "#", sep="", end="", flush=True)
         time.sleep(sleep)
-    
+
     print(Colors["ENDC"] + "\n\n")
 
 
 #this is a other loadingbar line
 def loadLineDL(sleep=float(0.1), text=str("Loading:")):
     """
     This loadingbar will look something like this:
@@ -101,24 +101,24 @@
         procent = x * 10
         t = t + "##"
         space = (space + "\b\b")
         line = (t + space)
 
         print(Colors["BOLD"] + text, Colors["FAIL"] + f"[{line}]", Colors["ENDC"] + f"{procent}%", end="\r")
         time.sleep(sleep)
-    
+
     #at the end print the hole line
     print(Colors["BOLD"] + text, Colors["FAIL"] + f"[{line}]", Colors["ENDC"] + "100%\n\n")
 
 
 #this is a loadingbar line with download style, but this one can count 1 and 10
 def loadLineDSE(sleep=float(0.1), text=str("Loading:")):
     """
     This is almost like styles.loadingLineDL but this one can count with 1
-    
+
     sleep:  time delay before next character is printed
     text:   text before loading, default look: Loading: [######    ] 60%
 
     this loadingbar will load from 1 - 100%, it will have [#####   ]
     and a text displaying what "text" is set to
 
     this function will exit with two new lines
@@ -139,32 +139,32 @@
 
         #this is set only when to aply more "###" to loadingbar line
         if prev == 0:
             prev = x
         elif (x - prev) == 5:
             t = t + "#"
             space = (space + "\b")
-            
+
             prev = x
 
         line = (t + space)
 
         #printing the line and waiting for "sleep" amount of seconds
         print(Colors["BOLD"] + text, Colors["FAIL"] + f"[{line}]", Colors["ENDC"] + f"{procent}%", end="\r")
         time.sleep(sleep)
-    
+
     #end
     print(Colors["BOLD"] + text, Colors["FAIL"] + f"[{line}]", Colors["ENDC"] + "100%\n\n")
 
 
 #this is a loadingbar line with download style, but this one can count 1 and 10, and it uses "-"
 def loadLineDSEL(sleep=float(0.1), text=str("Loading:")):
     """
     This is almost like styles.loadLineDSE but this one uses "-" and not "#"
-    
+
     sleep:  time delay before next character is printed
     text:   text before loading, default look: Loading: [------    ] 60%
 
     this loadingbar will load from 1 - 100%, it will have [----   ]
     and a text displaying what "text" is set to
 
     this function will exit with two new lines
@@ -186,47 +186,47 @@
 
         #this is set only when to aply more "###" to loadingbar line
         if prev == 0:
             prev = x
         elif (x - prev) == 5:
             t = t + "-"
             space = (space + "\b")
-            
+
             prev = x
 
         line = (t + space)
 
         #printing the line and waiting for "sleep" amount of seconds
         print(Colors["BOLD"] + text, Colors["FAIL"] + f"[{line}]", Colors["ENDC"] + f"{procent}%", end="\r")
         time.sleep(sleep)
-    
+
     #end
     print(Colors["BOLD"] + text, Colors["FAIL"] + f"[{line}]", Colors["ENDC"] + "100%\n\n")
 
 
 #this will make a line with a spinningwheel
 def lineSpinning(sleep=float(0.1), text=str("Loading:"), times=int(10)):
     """
     This loadingbar will look like this-- Loading: ----------/
 
     sleep:  delay between next printing figure
     text:   the text that displays before loadingbar
     times:  the amount of times we gona print ---- and make a spinning animation
-    
+
     this will exit with two new lines, and will use colors that is not changeble
     """
     print(Colors["BOLD"] + text + "  ", sep="", end="", flush=True)
     #start a loop
     for x in range(times):
         print("\b" + Colors["FAIL"] + "--", sep="", end="", flush=True)
         for x in r"/-\|/-\|":
             print("\b" + Colors["FAIL"] + x, sep="", end="", flush=True)
             time.sleep(sleep)
         time.sleep(sleep)
-    
+
     #end
     print(Colors["ENDC"] + "\n\n")
 
 
 #this will make a spinning wheel with % at the end
 def lineSpinningP(sleep=float(0.1), text=str("Loading:")):
     """
@@ -235,15 +235,15 @@
 
     sleep:  delay between next printing figure
     text:   the text that displays before loadingbar
 
     Note: text don't need to end with space, this program add space
     and sleep for the spinningwheel is 5 times faster than sleep time
     so it is (sleep / 5)
-    
+
     this time you can't set time.
     this will exit with two new lines, and will use colors that is not changeble
     """
     #extras
     lf = ""
     prev = 0
 
@@ -260,54 +260,54 @@
             elif(i - prev) == 5:
                 prev = i
                 lf = ("-" + (lf))
 
             print(Colors["BOLD"] + text + " ", Colors["FAIL"] + lf + x + " ", Colors["ENDC"] + str(procent) + "%", "\r", sep="", end="", flush=True)
             time.sleep(sleep / 5)
         time.sleep(sleep)
-    
+
     #end
     print(Colors["BOLD"] + text + " ", Colors["FAIL"] + lf + x, Colors["ENDC"] + "100%\n\n")
 
 
 #this is a loadingbar that will let you pick colors and will look like this: 50% [working]
 def loadingbarPFT(sleep=float(0.1), text=str("working"), loading_color=Colors["FAIL"], end_color=Colors["ENDC"], text_color=Colors["FAIL"]):
     """
     This will be a custom loadingbar,
     PFT = Procent First with Text
 
     sleep: amount of delay before next procent
     text:  the display text, will be inside [ ]
-    
+
     loading_color:  This will be the loadingbar color, default "FAIL"
     end_color:      This will be the exit color, default "ENDC"
     text_color:     This color will be the color of the text, default "FAIL"
 
     Note: The Colors are recomended to be styles.Colors[color], if you have other
     colors you can try, but it may give an error
     and recomended color combines are:
         text = BLUE
         loading = FAIL (default) or WARNING
         end = ENDC (default)
 
     this one will print from 1% - 100%
     it will look something like this:   50% [working]
 
-    this will en with 2 new lines
+    this will end with 2 new lines
     """
     for x in range(100):
         if x < 10:
             #here we set the space to 3
             line = (str(x) + "%" + "   " + text_color + f"[{text}]")
             print(loading_color + line, "\r", sep="", end="", flush=True)
-        
+
         else:
             #this will set the space from 3 to 2
             line = (str(x) + "%" + "  " + text_color + f"[{text}]")
             print(loading_color + line, "\r", sep="", end="", flush=True)
 
         #delay
         time.sleep(sleep)
-    
+
     #end, it will end with space
     print(loading_color + str(100) + "%", text_color + f" [{text}]")
-    print(end_color + "\n")
+    print(end_color + "\n")
```

### Comparing `styles-0.1.6/styles/figures.py` & `styles-0.1.7/styles/figures.py`

 * *Files identical despite different names*

### Comparing `styles-0.1.6/styles/osInfo.py` & `styles-0.1.7/styles/osInfo.py`

 * *Files identical despite different names*

### Comparing `styles-0.1.6/styles.egg-info/PKG-INFO` & `styles-0.1.7/styles.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: styles
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Style pack for python
 Home-page: https://github.com/Xtarii/PythonStylePack
 Author: Lord Alvin Hansen
 Author-email: alvin.hansen@elev.ga.ntig.se
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

