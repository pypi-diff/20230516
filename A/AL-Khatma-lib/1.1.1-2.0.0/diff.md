# Comparing `tmp/AL_Khatma_lib-1.1.1.tar.gz` & `tmp/AL_Khatma_lib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AL_Khatma_lib-1.1.1.tar", last modified: Sun Apr 30 03:25:05 2023, max compression
+gzip compressed data, was "AL_Khatma_lib-2.0.0.tar", last modified: Tue May 16 10:57:38 2023, max compression
```

## Comparing `AL_Khatma_lib-1.1.1.tar` & `AL_Khatma_lib-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-04-30 03:25:05.810463 AL_Khatma_lib-1.1.1/
--rw-r--r--   0 oaokm     (1000) oaokm     (1000)     1163 2023-04-16 18:02:45.000000 AL_Khatma_lib-1.1.1/LICENSE
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    30117 2023-04-30 03:25:05.810463 AL_Khatma_lib-1.1.1/PKG-INFO
--rw-r--r--   0 oaokm     (1000) oaokm     (1000)    29605 2023-04-30 02:59:13.000000 AL_Khatma_lib-1.1.1/README.md
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      585 2023-04-30 03:24:31.000000 AL_Khatma_lib-1.1.1/pyproject.toml
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       38 2023-04-30 03:25:05.810463 AL_Khatma_lib-1.1.1/setup.cfg
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-04-30 03:25:05.806463 AL_Khatma_lib-1.1.1/src/
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-04-30 03:25:05.810463 AL_Khatma_lib-1.1.1/src/AL_Khatma/
--rw-r--r--   0 oaokm     (1000) oaokm     (1000)     1035 2023-04-30 03:24:36.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma/__init__.py
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     2746 2023-04-30 03:13:55.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma/cheak.py
--rw-r--r--   0 oaokm     (1000) oaokm     (1000)     7657 2023-04-30 02:51:02.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma/khatma.py
--rw-r--r--   0 oaokm     (1000) oaokm     (1000)     1034 2023-04-30 02:22:42.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma/log.py
--rw-r--r--   0 oaokm     (1000) oaokm     (1000)    14667 2023-04-30 02:36:52.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma/quran.py
-drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-04-30 03:25:05.810463 AL_Khatma_lib-1.1.1/src/AL_Khatma_lib.egg-info/
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    30117 2023-04-30 03:25:05.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma_lib.egg-info/PKG-INFO
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      313 2023-04-30 03:25:05.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)        1 2023-04-30 03:25:05.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       10 2023-04-30 03:25:05.000000 AL_Khatma_lib-1.1.1/src/AL_Khatma_lib.egg-info/top_level.txt
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-16 10:57:38.029604 AL_Khatma_lib-2.0.0/
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1163 2023-05-14 01:34:18.000000 AL_Khatma_lib-2.0.0/LICENSE
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    61528 2023-05-16 10:57:38.029604 AL_Khatma_lib-2.0.0/PKG-INFO
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    61017 2023-05-16 10:43:17.000000 AL_Khatma_lib-2.0.0/README.md
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      656 2023-05-16 10:56:33.000000 AL_Khatma_lib-2.0.0/pyproject.toml
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       38 2023-05-16 10:57:38.029604 AL_Khatma_lib-2.0.0/setup.cfg
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-16 10:57:37.933599 AL_Khatma_lib-2.0.0/src/
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-16 10:57:38.025604 AL_Khatma_lib-2.0.0/src/AL_Khatma/
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1080 2023-05-16 02:45:36.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/__init__.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1974 2023-05-16 10:17:59.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/adkar.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     2640 2023-05-16 02:22:31.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/cheak.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     9584 2023-05-16 09:51:17.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/khatma.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     1034 2023-05-14 01:34:18.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/log.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     4034 2023-05-16 02:44:08.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/message.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     8766 2023-05-16 10:31:28.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/pdf_page.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    16035 2023-05-16 03:26:12.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/quran.py
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)     5226 2023-05-16 10:22:47.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma/tafser.py
+drwxrwxr-x   0 oaokm     (1000) oaokm     (1000)        0 2023-05-16 10:57:38.025604 AL_Khatma_lib-2.0.0/src/AL_Khatma_lib.egg-info/
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)    61528 2023-05-16 10:57:37.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)      411 2023-05-16 10:57:37.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)        1 2023-05-16 10:57:37.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 oaokm     (1000) oaokm     (1000)       10 2023-05-16 10:57:37.000000 AL_Khatma_lib-2.0.0/src/AL_Khatma_lib.egg-info/top_level.txt
```

### Comparing `AL_Khatma_lib-1.1.1/LICENSE` & `AL_Khatma_lib-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-1.1.1/pyproject.toml` & `AL_Khatma_lib-2.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AL_Khatma_lib"
-version = "1.1.1"
+version = "2.0.0"
 authors = [
   { name="Osamah Awadh", email="osamahawadh01@gmail.com" },
 ]
 description = "A library Specialized About Islamic"
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
@@ -16,7 +16,10 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/oaokm/AL-Khatma"
 "Bug Tracker" = "https://github.com/oaokm/AL-Khatma/issues"
+
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
```

### Comparing `AL_Khatma_lib-1.1.1/src/AL_Khatma/__init__.py` & `AL_Khatma_lib-2.0.0/src/AL_Khatma/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
     MIT License | Copyright (C) 2023 Osamah Awadh (https://github.com/oaokm)
 '''
 
 import os
 from .log import log
 from .cheak import cheak
 
-__version__   = '1.1.1'
+#! لا تقم بتغير رقم الإصدار
+#! Do not change the version
+__version__   = '2.0.0'
 __main_path__ = os.path.dirname(__file__)
 
-os.chdir(path=__main_path__)
-
 
 def Download_DATA():
     log(
         f'{__file__} | Download DATA Request ', 
         f'The user to been request the cheak and download files form Github'
         ).write_message()
     down       = cheak()
@@ -33,8 +33,7 @@
 
 def show_me_log():
     log(
         f'{__file__} | Show Me Log Request ', 
         f'The user to been request the path log file'
         ).write_message()
     return f"{__main_path__}/DATA/loging.log"
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AL_Khatma_lib-1.1.1/src/AL_Khatma/cheak.py` & `AL_Khatma_lib-2.0.0/src/AL_Khatma/cheak.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 main_path = os.path.dirname(__file__)
 
 class cheak:
 
     def __init__(self):
         self.download_file = list()
         self.path_url      = list()
-        # self.JSONFILE      = json.load(open('./cheak_download.json', 'r', encoding='utf8'))
         try:
             self.JSONFILE      = requests.get(
-                url="https://raw.githubusercontent.com/oaokm/AL-Khatma/main/cheak_download.json"
-                ).json()
+                url="https://raw.githubusercontent.com/oaokm/AL-Khatma/main/DATA/cheak_download.json").json()
         except requests.exceptions.ConnectionError as e:
             log(
             f"{__file__} > cheak > __init__ | Check The Internet Status",
             f"The WiFi connection error, please check your internet"
             ).write_message()
             print(f"[ cheak | __init__ > The WiFi connection error ] {e}")
```

### Comparing `AL_Khatma_lib-1.1.1/src/AL_Khatma/khatma.py` & `AL_Khatma_lib-2.0.0/src/AL_Khatma/khatma.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,45 @@
 from .quran import Quran
+from .message import message
 from .log import log
+from .pdf_page import quran_pdf
 from tqdm import tqdm
+from time import perf_counter
+import os
+
+__main_path__ = os.path.dirname(__file__)
+file_name     = __file__.split('/')[-1]
 
 class khatma:
     def __init__(self, days:int):
         log(
-            f"{__file__} > khatma | Status The Class",
+            f"{file_name} > khatma | Status The Class",
             f"True, days(int): {days}"
             ).write_message()
+        
+        #! التحقق من وجود تحديث جديد للمكتبة
+        message().cheak_version()
+
         self.days       = days
         self.werrd_page = list()
         self.quran      = Quran().quran_blocks()
 
     #* دالة تقوم على تقسيم صفحات القرآن لهدف إنهاء قراءة القرآن في يوم معين
-    def Khatma_page(self, report=False, werrd=False):
+    def Khatma_page(self, report=False, werrd=False, pdf=False, down_path_pdf=str()):
         """
         Khatma_page(func): هي دالة تقوم بتقسيم صفحات القرآن الكريم بهدف إنهاء قراءتها
         report(bool): في حال تفعيل الخيار يتم طباعة تقرير عن النتائج التي تم تحليلها من هذه الدالة
         werrd(bool): في حال تفعيل الخيار تتم عملية تقسيم القرآن بناءًا على عدد الأيام الذي أدخلها المستخدم. في حال عدم تفعيل هذا الخيار يقوم البرنامج بإعادة قيمة عدد الصفحات اليومية الازمة لإنهاء قراءة القرآن كاملة
+        pdf(bool): في حال تفعيل هذا الخيار، سيتم تطبيق التقسيم وإنشاء ملفات بي دي أف للقرأن
+        dwon_path_pdf(str): مسار تنزيل ملفات البي دي أف
         """
+        #! التحقق من وجود تحديث جديد للمكتبة
+        message().cheak_version()
         log(
-            f"{__file__} > khatma > Khatma_page | Info",
+            f"{file_name} > khatma > Khatma_page | Info",
             f"Days:{self.days}, report: {report}, werrd: {werrd}"
             ).write_message()
         #* عدد صفحات القرآن الكريم حسب نسخة مجمع الملك فهد لطباعة المصحف الشريف
         pages            = 604
         #* الأيام التي نريد ختم القرآن به
         Fdays            = self.days
         Fdays_pages      = list()
@@ -45,38 +60,38 @@
             for i in range(len(rest)):
                 Fdays_pages_N[i] += rest[i]
             report_pages_N = f"[REPORT KHATMA]\nDays: {self.days}\nReading Rate: {int(sum(Fdays_pages_N)/len(Fdays_pages_N))} (Page/Day)\nWeerd: {Fdays_pages_N}"
             #? التحقق من أن مجموع الصفحات المقسمة تساوي عدد صفحات القرآن الكريم
             if sum(Fdays_pages_N) == 604:
                 self.werrd_page = Fdays_pages_N
                 #* في حالة طلب المستخدم عدم تفعيل التقسيم على القرآن يتم تنفيذ هذه العملية
-                if werrd == False:
+                if werrd or pdf == False:
                     if report: print(report_pages_N)
                     return Fdays_pages_N
             #! في حال وجود مشكلة يتم تنفيذ هذا الأمر، وهي مشكلة في عملية الموازنة
             else:
                 log(
-                f"{__file__} > khatma > Khatma_page | Partition Error ",
+                f"{file_name} > khatma > Khatma_page | Partition Error ",
                 f"An error has occurred that is not supposed to happen. Value: len(Fdays_pages) > self.days: {len(Fdays_pages) > self.days}, len(Fdays_pages):{len(Fdays_pages)}, Fdays_pages: {Fdays_pages}, days: {self.days}"
                 ).write_message()
                 print("[ khatma > Khatma_page | Partition Error ] An error has occurred that is not supposed to happen, Visit the library's Issues page: https://github.com/oaokm/AL-Khatma/issues")
         #* إذا كانت عملية التقسيم تساوية مع عدد الأيام يتم تنفيذ هذا الأمر مباشرًا
         else:
             report = f"[REPORT KHATMA]\nDays: {self.days}\nReading Rate: {int(sum(Fdays_pages)/len(Fdays_pages))} (Page/Day)\nWeerd: {Fdays_pages}"
             #? التحقق من أن مجموع الصفحات المقسمة تساوي عدد صفحات القرآن الكريم
             if sum(Fdays_pages) == 604:
                 self.werrd_page = Fdays_pages
-                if werrd == False:
+                if werrd or pdf == False:
                     if report: print(report)
                     return Fdays_pages
             else: 
-                if werrd == False:
+                if werrd or pdf == False:
                     if report: print(report)
                     return Fdays_pages
-        
+
         #* في حال تفعيل هذا الخيار، تبدأ عملية تقسيم القرآن الكريم على عدد الأيام المدخلة
         if werrd:
             """
             [تعريف المتغيرات]
             0. page_per_day(list): يكون عدد العناصر في هذا المتغير مساوي لعدد الأيام المدخلة، وكل عنصر يحتوي على عدد الأيات التي يجب قرأتها
             1. for_day(list): يتم تسجيل معلومات الأيات لكي تم لاحقًا إلى متغير page_per_day
             2. stop_id(int): هذا المتغير يساعد في عملية التقسيم، ووضيفته هو معرفة مُعرف الأية الكريمة لتتم عملية التقسيم بسهولة
@@ -105,13 +120,31 @@
                 if len(page_per_day) == len(self.werrd_page)-1:
                     page_per_day.append(self.quran[stop_id:])
                 else:
                     continue
             report = f"[REPORT KHATMA]\nDays: {self.days}\nReading Rate: {int(sum(self.werrd_page)/len(self.werrd_page))} (Page/Day)\nWeerd: {self.werrd_page}\nNumber of Werrd: {len(page_per_day)}"
             if report: print(report)
             log(
-                f"{__file__} > khatma > Khatma_page > (werrd) | Status",
+                f"{file_name} > khatma > Khatma_page > (werrd) | Status",
                 f"True"
                 ).write_message()
             #* إرجاع قيمة العملية
             return page_per_day
+
+        #* تطبيق التقسيم مباشرًأ على pdf
+        elif pdf and down_path_pdf != '':
+            last_value = 1
+            pdf        = quran_pdf()
+            start      = perf_counter()
+            for day in range(len(self.werrd_page)):
+                print(f"# {day+1} of {self.days}\tFrom {last_value} -> {self.werrd_page[day]+last_value-1} Page")
+                pdf.creating('./weerds',
+                            From=last_value, to=self.werrd_page[day]+last_value-1, 
+                            cover=True, 
+                            cover_title=f'Number of Weerd: {day+1} of {self.days} Days')
+                last_value += self.werrd_page[day]
+            end    = perf_counter()
+            report = f"\n[REPORT KHATMA - PDF]\nRuning Time: {end-start}\nDays: {self.days}\nReading Rate: {int(sum(self.werrd_page)/len(self.werrd_page))} (Page/Day)\nWeerd: {self.werrd_page}\nNumber of Werrd: {len(self.werrd_page)}\nPath: {os.path.abspath(down_path_pdf)}"
+            if report: print(report) 
+        elif down_path_pdf == '':print("[Khatma | PDF] The option (down_path_pdf) is False, Please change to True, like this:\n\n\tkhatma(30).Khatma_page(pdf=True, dwon_path_pdf='./weerds', report=True)\n\n")
+
         else: pass
```

### Comparing `AL_Khatma_lib-1.1.1/src/AL_Khatma/log.py` & `AL_Khatma_lib-2.0.0/src/AL_Khatma/log.py`

 * *Files identical despite different names*

### Comparing `AL_Khatma_lib-1.1.1/src/AL_Khatma/quran.py` & `AL_Khatma_lib-2.0.0/src/AL_Khatma/quran.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,84 +1,94 @@
-import AL_Khatma
 from .log import log
+from .message import message
+from .tafser import tafser
 import json
 import requests
 import os
 from tqdm import tqdm
 import urllib3
 from time import perf_counter
 
 __main_path__ = os.path.dirname(__file__)
+file_name     = __file__.split('/')[-1]
 
 class Quran:
     def __init__(self, lang='main'):
         """
         Quran(class): 
         lang: اللغة التي تريد عرضها
         """
+        #! التحقق من وجود تحديث جديد للمكتبة
+        message().cheak_version()
+        
         try:
             #* قراءة ملف اللغات
-            os.chdir(path=__main_path__)
-            self.quran = json.load(open(f"./DATA/Language/{lang}.json", "r", encoding="utf8"))
+            # os.chdir(path=__main_path__)
+            self.quran = json.load(open(f"{__main_path__}/DATA/Language/{lang}.json", "r", encoding="utf8"))
             log(
-                f'{__file__} > Quran | Status JSON File ', 
+                f'{file_name} > Quran | Status JSON File ', 
                 f'Read: True, Language: {lang}'
                 ).write_message()
         except FileNotFoundError as e:
             #* في حال طلب المستخدم استعراض اللغات
 
             if lang == '?':
                 log(
-                f'{__file__} > Quran | Show All Language ', 
+                f'{file_name} > Quran | Show All Language ', 
                 f'The user has requested to view the available languages of the Quran'
                 ).write_message()
 
-                lang = os.listdir(path='./DATA/Language')
+                lang = os.listdir(path=f'{__main_path__}/DATA/Language')
                 print('the available languages of the Quran'.title())
                 for i in range(len(lang)):
                     nameFile = lang[i].split(".")[0]
                     if nameFile == 'main': print(f"[{i}] ar, en ({nameFile})")
                     else: print(f"[{i}] {nameFile}")
             else:
                 log(
-                f'{__file__} > Quran | Status JSON File ', 
+                f'{file_name} > Quran | Status JSON File ', 
                 f'Falus | The user has been entered for an unavailable language'
                 ).write_message()
                 
                 print('[Quran] Sorry, the language is your enter is not available.\nthe available languages of the Quran:')
                 
                 #// إنتبه: قم بتغير مسار لكي لا تحصل مشاكل
                 #// قم بوضع طريقة لقراءة جميع الملفات دون مشاكل عدم معرفه موقعها
-                lang = os.listdir(path='./DATA/Language')               
+                lang = os.listdir(path=f'{__main_path__}/DATA/Language')               
                 for i in range(len(lang)):
                     nameFile = lang[i].split(".")[0]
                     if nameFile == 'main': print(f"[{i}] ar, en ({nameFile})")
                     else: print(f"[{i}] {nameFile}")
 
 
     def show_block_aya(
             self,
             verses_no:int,
             verses_number:list,
+            tafser_aya=False,
+            tafser_type=str(),
             orderly=False,
             ):
         """
         show_block_aya(func): هي دالة تقوم بإستخراج ما يدرده المستخدم من ملف اللغة
-        verses_no(int): أستخراج السروة التي تريدها
-        verses_number(list): في حالة أنك ترد صورة بعينها يمكنك ذلك بكتابة رقم أيتها. ويمكن أن تجعلعا فارغة
+        verses_no(int): أستخراج السورة التي تريدها
+        verses_number(list): في حالة أنك تريد سورة بعينها يمكنك ذلك بكتابة رقم أيتها. ويمكن أن تجعلعا فارغة
         orderly(bool): إذا أردت أن ترى النتيجة مطبوعة بشكل يمكن قراءتها
         """
+        #! التحقق من وجود تحديث جديد للمكتبة
+        message().cheak_version()
+
         log(
-            "quran.py > Quran > show_block_aya | info",
+            f"{file_name} > Quran > show_block_aya | info",
             f"verses_no: {verses_no}, verses_number: {verses_number}, orderly: {orderly}"
         ).write_message()
 
         if verses_no <= 114:
             log(
-            f"{__file__} > Quran > show_block_aya | number of Surahs of the Qur’an is good",
+            f"{file_name} > Quran > show_block_aya | number of Surahs of the Qur’an is good",
             f"The number entered did not exceed the number of Surahs of the Qur’an"
             ).write_message()
             #? لتدوين أيات جميع السورة المحددة
             results = list()
             #? تدوين أعداد السورة المطلوبة
             verses = list()
             #* يحدث عملية البحث عن السورة المطلوبة
@@ -93,32 +103,37 @@
                         #? هنا تحدث عملية رصد الأيات المطلوبة تزامُنا مع علميلة رصد أيات السورة المطلوبة
                         for cheaking in verses_number:
                             #? التحقق من أن الأية المطلوبة ضمن عدد أيات السورة + التأكد من الأية بعينها لإضافتها في قائمة مخصصة
                             if self.quran[search+i]['total_verses'] >= cheaking and cheaking == self.quran[search+i]['verses_number']:
                                 verses.append(self.quran[search+i])
                             else:
                                 continue
+                    #? نتائج البجث عن تفسير الأيات، يتم تحديدها من رقم السورة أو رقم السورة وأيات يتم تحديدها من "verses_number"
+                    results_tafser = list()
+                    if tafser_aya:
+                        taf            = tafser(tafser_book='muyassar')
+                        results_tafser = taf.call_block(verses_no, verses_number)
 
-                    #* طباعة تقرير مُنسق مع إرجاع قينتين للعمليتين السابقتين
+                    #* طباعة تقرير مُنسق مع إرجاع ثلاثة قيم للعمليات السابقة
                     if orderly:
                         txt = ('results'.upper(), 'verses'.upper())
                         print(f'\n\n\n{txt[0]:.^50}\n\n\n')
                         print(json.dumps(results, indent=4, ensure_ascii=False))
                         print(f'\n\n\n{txt[1]:.^50}\n\n\n')
                         print(json.dumps(verses, indent=4, ensure_ascii=False))
                         
-                        return (results, verses)
-                    #* إرجاع القيمتين السابقين فقط
-                    else: return (results, verses)
+                        return (results, verses, results_tafser)
+                    #* إرجاع ثلاثة قيم 
+                    else: return (results, verses, results_tafser)
                 #? هذا في حالة عدم إجاد السورة فإنه يستمر حتى يجد السورة المطلوب
                 else: continue
         #? في حالة تجاوز 114 سورة قرأنية يتم رفض الطلب
         else:
             log(
-            f"{__file__} > Quran > show_block_aya | Verses Over Error",
+            f"{file_name} > Quran > show_block_aya | Verses Over Error",
             f"I have exceeded 114 Quranic chapters. Please adhere to the number of Quranic chapters (from 1 to 114)."
             ).write_message()
             print('I have exceeded 114 Quranic chapters. Please adhere to the number of Quranic chapters (from 1 to 114).')
             return (False,)
 
 
     #* هذا للبحث عن كلمة أو مجموعة كلمات في القرآن
@@ -130,23 +145,26 @@
             ):
         """
         searching(func): هي دالة للبحث بين السطور القرآنية
         text(str): الكلمة المراد بحثها
         search_second_lang(bool): في حال تفعيل هذه الخاصية سيتم البحث بنائا على اللغة الثانية في ملف اللغة
         print_report(bool): في حال تفعيل هذه الخاصية قوم بطباعة تقرير منظم عن نتائج البحث
         """
+        #! التحقق من وجود تحديث جديد للمكتبة
+        message().cheak_version()
+
         log(
-            f"{__file__} > Quran > searching | Search Info",
+            f"{file_name} > Quran > searching | Search Info",
             f"Search: {text}, search_my_lang: {search_second_lang}, print_report: {print_report}"
             ).write_message()
         start = perf_counter()
         #? في حال إذا كان النص فارغ لا يتم تنفيذ الطلب
         if text != '':
             log(
-            f"{__file__} > Quran > searching | The Search Status",
+            f"{file_name} > Quran > searching | The Search Status",
             f"True"
             ).write_message()
             end = perf_counter()
             # * يكون جميع النص lower
             text    = text.lower()
             #* لتحزين النتائج
             results = list()
@@ -181,26 +199,29 @@
             #* إرجاع قيمة البحث
             end = perf_counter()
             if print_report: print(f"[REPORT]\nRuning Time: {end-start}\nCount Search: {len(results)}\nResult Search: {json.dumps(results, indent=4, ensure_ascii=False)}")
             return results
         
         else:
             log(
-            f"{__file__} > Quran > searching | The Search Status",
+            f"{file_name} > Quran > searching | The Search Status",
             f"The search failed; the user has not made any input in search zone or input empty."
             ).write_message()
             end = perf_counter()
             if print_report: print(f"[REPORT]\nRuning Time: {end-start}\nResults Search: {json.dumps(results, indent=4, ensure_ascii=False)}\nThe Number Of Search Results: {len(results)}")
             return (False, )
     
 
     #? لإرجاع قيمة self.quran
     def quran_blocks(self):
+        #! التحقق من وجود تحديث جديد للمكتبة
+        message().cheak_version()
+
         log(
-                f'{__file__} > quran_blocks | Return All The Quran Data ', 
+                f'{file_name} > quran_blocks | Return All The Quran Data ', 
                 f'The user return all data quran from json file'
                 ).write_message()
         return self.quran
     
 
     #* تحميل صفحات القرآن الكريم
     def page_pic(
@@ -213,43 +234,46 @@
         """
         page_pic(func): دالة تقوم على تحميل صفحات القرآن من الإنترنت
         page(list): تقوم بوضع عدد الأيات التي تريد تحميلها
         path(str): المسار تنزيل الصور
         name_folder(str): أسم الملف الذي ستكون فيها الصور الصفحات
         return_imge(bool): في حال تم تفعيل الخيار، سيتم تحميل الصفحات على شكل بايت (Binary)
         """
+        #! التحقق من وجود تحديث جديد للمكتبة
+        message().cheak_version()
+
         #? التحقق من موجود إنترنت
         try:
             requests.get('https://github.com/oaokm')
             log(
-            f"{__file__} > Quran > page_pic | Check The Internet Status",
+            f"{file_name} > Quran > page_pic | Check The Internet Status",
             f"The internet is good"
             ).write_message()
 
             #* قراءة ملف الذي يحتوي على رابط صفحات القرأن كاملة وبجودة عالية
-            quran_books = json.load(open('./DATA/quran_books.json', 'r', encoding='utf8'))
+            quran_books = json.load(open(f'{__main_path__}/DATA/quran_books.json', 'r', encoding='utf8'))
             try:
                 log(
-                    f"{__file__} > Quran > page_pic | Check For Read JSON File",
+                    f"{file_name} > Quran > page_pic | Check For Read JSON File",
                     f"The file (quran_books.json) is good"
                 ).write_message()
                 
                 web_pic = quran_books[type]
             except KeyError as e:
                 log(
-                    f"{__file__} > Quran > page_pic | Check For Read JSON File",
+                    f"{file_name} > Quran > page_pic | Check For Read JSON File",
                     f"Error(keyError): {e}"
                 ).write_message()
                 print(f'[ Quran > page_pic | KeyError ]: {e}')
             #* في حالة إذا كان خاصية (return_imge) مفعلة يتم تسجيل محتويات الصورة كبِّت(صيغة ثنائية)
             pics = list()
             
             #? هنا تبدأ عملية الوصول للصفحات وتحميلها
             PATH = f'{path}/{name_folder}'
-            print(f"# Download Pages From Quran | [{os.path.abspath(PATH)}]")
+            print(f"# Download Pages From Quran | Type: {type} | Path:[{os.path.abspath(PATH)}] | From: {page[0]} to {page[-1]}")
             for p in tqdm(page):
                 #? التحقق من إذا كان المدخل لا يتخطى عدد صفحات القرأن
                 if p <= 604:
                     #* عملية الإتصال بالموقع لسحب الصورة الصفحة
                     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
                     url    = web_pic.format(p)
                     r_page = requests.get(url=url, verify=False)
@@ -271,14 +295,17 @@
                     print('I have exceeded 604 Page. Please adhere to the number of Page (from 1 to 604).')
             #? في جال إذا خيار return_imge مُفعل، يتم إرجاع قيمتها
             if return_imge:
                 return pics
         #? في حال عدم وجود إنترنت يتم رفض الأمر
         except requests.exceptions.ConnectionError as e:
             log(
-            f"{__file__} > Quran > page_pic | Check The Internet Status",
+            f"{file_name} > Quran > page_pic | Check The Internet Status",
             f"The WiFi connection error, please check your internet"
             ).write_message()
             print(f"[ Quran | page_pic > The WiFi connection error ] {e}")
+    
 
 if __name__ == '__main__':
+    #! التحقق من وجود تحديث جديد للمكتبة
+    message().cheak_version()
     print('[quran.py] This file is not to run')
```

