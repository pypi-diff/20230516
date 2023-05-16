# Comparing `tmp/ilds-2023.4.3.tar.gz` & `tmp/ilds-2023.5.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ilds-2023.4.3.tar", last modified: Mon Apr  3 10:59:19 2023, max compression
+gzip compressed data, was "dist\ilds-2023.5.16.tar", last modified: Tue May 16 08:29:59 2023, max compression
```

## Comparing `ilds-2023.4.3.tar` & `ilds-2023.5.16.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/
-drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds/
--rw-rw-rw-   0        0        0     1797 2021-09-26 05:21:21.000000 ilds-2023.4.3/ilds/cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds/django/
--rw-rw-rw-   0        0        0     3407 2019-10-30 05:10:14.000000 ilds-2023.4.3/ilds/django/admin.py
--rw-rw-rw-   0        0        0    14906 2019-10-30 03:18:15.000000 ilds-2023.4.3/ilds/django/import_export.py
--rw-rw-rw-   0        0        0    15417 2019-11-27 09:35:07.000000 ilds-2023.4.3/ilds/django/model.py
--rw-rw-rw-   0        0        0     1840 2019-04-12 05:15:43.000000 ilds-2023.4.3/ilds/django/user.py
--rw-rw-rw-   0        0        0     2085 2021-09-28 08:04:39.000000 ilds-2023.4.3/ilds/django/util.py
--rw-rw-rw-   0        0        0        0 2018-08-07 03:24:52.000000 ilds-2023.4.3/ilds/django/__init__.py
--rw-rw-rw-   0        0        0     9150 2021-12-06 10:18:15.000000 ilds-2023.4.3/ilds/everything.py
--rw-rw-rw-   0        0        0     9470 2019-03-29 08:26:49.000000 ilds-2023.4.3/ilds/excel_xlrd.py
--rw-rw-rw-   0        0        0     7970 2022-10-19 09:11:30.000000 ilds-2023.4.3/ilds/excel_xlsx.py
--rw-rw-rw-   0        0        0    26848 2023-04-03 10:59:15.000000 ilds-2023.4.3/ilds/file.py
--rw-rw-rw-   0        0        0     1530 2021-09-26 05:15:22.000000 ilds-2023.4.3/ilds/json.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds/lib/
--rw-rw-rw-   0        0        0    13740 2018-11-26 09:16:44.000000 ilds-2023.4.3/ilds/lib/browsercookie.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds/lib/configobj/
--rw-rw-rw-   0        0        0    46989 2019-05-06 20:45:36.000000 ilds-2023.4.3/ilds/lib/configobj/validate.py
--rw-rw-rw-   0        0        0       44 2019-05-06 20:45:36.000000 ilds-2023.4.3/ilds/lib/configobj/_version.py
--rw-rw-rw-   0        0        0    88030 2019-05-06 20:45:36.000000 ilds-2023.4.3/ilds/lib/configobj/__init__.py
--rw-rw-rw-   0        0        0    13829 2018-10-24 05:15:43.000000 ilds-2023.4.3/ilds/lib/hexdump.py
--rw-rw-rw-   0        0        0        0 2018-10-24 05:29:38.000000 ilds-2023.4.3/ilds/lib/__init__.py
--rw-rw-rw-   0        0        0    15494 2021-10-24 10:49:44.000000 ilds-2023.4.3/ilds/match_data.py
--rw-rw-rw-   0        0        0     7121 2019-11-18 03:49:54.000000 ilds-2023.4.3/ilds/md.py
--rw-rw-rw-   0        0        0     4832 2022-09-07 09:59:12.000000 ilds-2023.4.3/ilds/md5summer.py
--rw-rw-rw-   0        0        0     3513 2019-10-11 11:13:36.000000 ilds-2023.4.3/ilds/mycsv.py
--rw-rw-rw-   0        0        0     5123 2022-12-12 02:45:33.000000 ilds-2023.4.3/ilds/net.py
--rw-rw-rw-   0        0        0     7906 2023-04-03 10:59:05.000000 ilds-2023.4.3/ilds/pd.py
--rw-rw-rw-   0        0        0     7064 2019-09-09 02:27:39.000000 ilds-2023.4.3/ilds/spider.py
--rw-rw-rw-   0        0        0    13238 2021-03-05 07:49:55.000000 ilds-2023.4.3/ilds/time.py
--rw-rw-rw-   0        0        0     7637 2022-10-08 10:21:44.000000 ilds-2023.4.3/ilds/util.py
--rw-rw-rw-   0        0        0       22 2023-04-03 10:59:05.000000 ilds-2023.4.3/ilds/versions.py
--rw-rw-rw-   0        0        0        0 2018-07-04 06:42:08.000000 ilds-2023.4.3/ilds/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1316 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       75 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/requires.txt
--rw-rw-rw-   0        0        0      708 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        5 2023-04-03 10:59:19.000000 ilds-2023.4.3/ilds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1316 2023-04-03 10:59:19.000000 ilds-2023.4.3/PKG-INFO
--rw-rw-rw-   0        0        0      456 2019-10-24 10:28:45.000000 ilds-2023.4.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-03 10:59:19.000000 ilds-2023.4.3/setup.cfg
--rw-rw-rw-   0        0        0     6394 2021-04-15 11:13:47.000000 ilds-2023.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:29:59.000000 ilds-2023.5.16/
+drwxrwxrwx   0        0        0        0 2023-05-16 08:29:59.000000 ilds-2023.5.16/ilds/
+-rw-rw-rw-   0        0        0     1797 2021-09-26 05:21:21.000000 ilds-2023.5.16/ilds/cmd.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:29:59.000000 ilds-2023.5.16/ilds/django/
+-rw-rw-rw-   0        0        0     3407 2019-10-30 05:10:14.000000 ilds-2023.5.16/ilds/django/admin.py
+-rw-rw-rw-   0        0        0    14906 2019-10-30 03:18:15.000000 ilds-2023.5.16/ilds/django/import_export.py
+-rw-rw-rw-   0        0        0    15417 2019-11-27 09:35:07.000000 ilds-2023.5.16/ilds/django/model.py
+-rw-rw-rw-   0        0        0     1840 2019-04-12 05:15:43.000000 ilds-2023.5.16/ilds/django/user.py
+-rw-rw-rw-   0        0        0     2085 2021-09-28 08:04:39.000000 ilds-2023.5.16/ilds/django/util.py
+-rw-rw-rw-   0        0        0        0 2018-08-07 03:24:52.000000 ilds-2023.5.16/ilds/django/__init__.py
+-rw-rw-rw-   0        0        0     9150 2021-12-06 10:18:15.000000 ilds-2023.5.16/ilds/everything.py
+-rw-rw-rw-   0        0        0     9470 2019-03-29 08:26:49.000000 ilds-2023.5.16/ilds/excel_xlrd.py
+-rw-rw-rw-   0        0        0     9462 2023-05-16 08:14:48.000000 ilds-2023.5.16/ilds/excel_xlsx.py
+-rw-rw-rw-   0        0        0    27734 2023-05-16 08:23:40.000000 ilds-2023.5.16/ilds/file.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:29:59.000000 ilds-2023.5.16/ilds/lib/
+-rw-rw-rw-   0        0        0    13740 2018-11-26 09:16:44.000000 ilds-2023.5.16/ilds/lib/browsercookie.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:29:59.000000 ilds-2023.5.16/ilds/lib/configobj/
+-rw-rw-rw-   0        0        0    46989 2019-05-06 20:45:36.000000 ilds-2023.5.16/ilds/lib/configobj/validate.py
+-rw-rw-rw-   0        0        0       44 2019-05-06 20:45:36.000000 ilds-2023.5.16/ilds/lib/configobj/_version.py
+-rw-rw-rw-   0        0        0    88030 2019-05-06 20:45:36.000000 ilds-2023.5.16/ilds/lib/configobj/__init__.py
+-rw-rw-rw-   0        0        0    13829 2018-10-24 05:15:43.000000 ilds-2023.5.16/ilds/lib/hexdump.py
+-rw-rw-rw-   0        0        0        0 2018-10-24 05:29:38.000000 ilds-2023.5.16/ilds/lib/__init__.py
+-rw-rw-rw-   0        0        0    17951 2023-04-27 08:50:24.000000 ilds-2023.5.16/ilds/match_data.py
+-rw-rw-rw-   0        0        0     7121 2019-11-18 03:49:54.000000 ilds-2023.5.16/ilds/md.py
+-rw-rw-rw-   0        0        0     4832 2022-09-07 09:59:12.000000 ilds-2023.5.16/ilds/md5summer.py
+-rw-rw-rw-   0        0        0     3513 2019-10-11 11:13:36.000000 ilds-2023.5.16/ilds/mycsv.py
+-rw-rw-rw-   0        0        0     5123 2022-12-12 02:45:33.000000 ilds-2023.5.16/ilds/net.py
+-rw-rw-rw-   0        0        0     8384 2023-05-16 07:09:24.000000 ilds-2023.5.16/ilds/pd.py
+-rw-rw-rw-   0        0        0     7064 2019-09-09 02:27:39.000000 ilds-2023.5.16/ilds/spider.py
+-rw-rw-rw-   0        0        0    13238 2021-03-05 07:49:55.000000 ilds-2023.5.16/ilds/time.py
+-rw-rw-rw-   0        0        0     7637 2022-10-08 10:21:44.000000 ilds-2023.5.16/ilds/util.py
+-rw-rw-rw-   0        0        0       23 2023-05-16 08:29:14.000000 ilds-2023.5.16/ilds/versions.py
+-rw-rw-rw-   0        0        0        0 2018-07-04 06:42:08.000000 ilds-2023.5.16/ilds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:29:59.000000 ilds-2023.5.16/ilds.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-16 08:29:58.000000 ilds-2023.5.16/ilds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1317 2023-05-16 08:29:58.000000 ilds-2023.5.16/ilds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2023-05-16 08:29:58.000000 ilds-2023.5.16/ilds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      695 2023-05-16 08:29:58.000000 ilds-2023.5.16/ilds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        5 2023-05-16 08:29:58.000000 ilds-2023.5.16/ilds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1317 2023-05-16 08:29:59.000000 ilds-2023.5.16/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2019-10-24 10:28:45.000000 ilds-2023.5.16/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-16 08:29:59.000000 ilds-2023.5.16/setup.cfg
+-rw-rw-rw-   0        0        0     6394 2021-04-15 11:13:47.000000 ilds-2023.5.16/setup.py
```

### Comparing `ilds-2023.4.3/ilds/cmd.py` & `ilds-2023.5.16/ilds/cmd.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/django/admin.py` & `ilds-2023.5.16/ilds/django/admin.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/django/import_export.py` & `ilds-2023.5.16/ilds/django/import_export.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/django/model.py` & `ilds-2023.5.16/ilds/django/model.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/django/user.py` & `ilds-2023.5.16/ilds/django/user.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/django/util.py` & `ilds-2023.5.16/ilds/django/util.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/everything.py` & `ilds-2023.5.16/ilds/everything.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/excel_xlrd.py` & `ilds-2023.5.16/ilds/excel_xlrd.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/excel_xlsx.py` & `ilds-2023.5.16/ilds/excel_xlsx.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 ﻿# -*- coding: utf-8 -*-
 #
 # ---------------------------------------
 #   程序：excel_xlsx.py
-#   版本：0.4
+#   版本：0.5
 #   作者：lds
-#   日期：2020-03-20
+#   日期：2023-05-16
 #   语言：Python 3.X
 #   说明：读取excel文件内容
 # ---------------------------------------
 
+import os
 from time import time
 from warnings import warn
 
 # ReadExcel
 from openpyxl import load_workbook
 from openpyxl.styles import numbers, is_date_format
 
@@ -23,14 +24,17 @@
     XL_CELL_DATE,
     XL_CELL_BOOLEAN,
     XL_CELL_ERROR,
     XL_CELL_BLANK,
 ) = range(7)
 
 
+# warn('我们把 excel_xlsx 重命名为 excel，以后会删除 excel_xlsx', DeprecationWarning, stacklevel=2)
+
+
 def get_title_style(workbook, style_colour='#daeef3', is_bold=False):
     """
     获取自定义颜色的标题风格
     :param workbook:
     :param style_colour: 默认颜色为什么浅色
     :param is_bold: 是否设置粗体字体
     :return:
@@ -47,14 +51,60 @@
     # 设置边框
     head_style.set_border()
     # 调整行的高度以适应文本
     head_style.set_text_wrap()
     return head_style
 
 
+def get_excel_info(file, only_read_first_table=False):
+    """
+    读取 Excel 信息
+
+    :param file: Excel 文件
+    :param only_read_first_table: 只读取第一个表格
+    :return: {sheet_name: {'file_name', 'index', 'sheet_name', 'sheet_names', 'max_row', 'max_column', 'columns'}, }
+    """
+    data = {}
+
+    file_name = os.path.basename(file)
+
+    wb = load_workbook(file, read_only=True)
+    sheet_names = wb.sheetnames
+
+    for index, sheet_name in enumerate(sheet_names):
+        ws = wb[sheet_name]
+
+        # 获取第一行数据
+        columns = next(ws.iter_rows(min_row=1, max_row=1, values_only=True))
+
+        df_data = {
+            'file_name': file_name,
+            'index': index,
+            'sheet_name': sheet_name,
+            'sheet_names': sheet_names,
+            'sheet_state': ws.sheet_state,
+            'max_row': ws.max_row,
+            'max_column': ws.max_column,
+            'columns': list(columns),
+
+        }
+
+        # 我们添加 count 为了和以前获取信息相同，以后会去掉，用 max_row 替代
+        # df_data['count'] = df_data['max_row']
+
+        if only_read_first_table:
+            return df_data
+
+        data[sheet_name] = df_data
+
+    wb.close()
+
+    return data
+
+
 class ReadXlsx(object):
 
     def __init__(self, *args, **kwargs):
         """
         读取 Excel 文件的类 用 openpyxl 重写
 
         # 例子
@@ -213,14 +263,15 @@
     """
     打印模块说明文档
     """
     doc_text = """"""
     doc_text += '\n'
     doc_text += '{fun.__name__}{fun.__doc__}\n'.format(fun=ReadXlsx)
     doc_text += '{fun.__name__}{fun.__doc__}\n'.format(fun=get_title_style)
+    doc_text += '{fun.__name__}{fun.__doc__}\n'.format(fun=get_excel_info)
 
     print(doc_text)
 
 
 if __name__ == "__main__":
     t1 = time()
```

### Comparing `ilds-2023.4.3/ilds/file.py` & `ilds-2023.5.16/ilds/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #   语言：Python 3.X
 #   说明：常用的文件操作函数集合
 # ---------------------------------------
 
 
 import os
 import sys
+import json
 import random
 import shutil
 # get_file_md5
 import hashlib
 # get_encoding
 import chardet
 from chardet.universaldetector import UniversalDetector
@@ -328,16 +329,17 @@
 def exists_file(_file):
     """
     判断文件是否存在，如果存在就返回重命名的文件，不存在就直接返回
     :param _file:
     :return:
     """
 
-    warnings.warn('exists_file 已经弃用，因为它对人类不友好，也没有检查新名字是否已经存在\n建议用 check_filename_available 替代',
-                  DeprecationWarning)
+    warnings.warn(
+        'exists_file 已经弃用，因为它对人类不友好，也没有检查新名字是否已经存在\n建议用 check_filename_available 替代',
+        DeprecationWarning)
 
     if os.path.exists(_file):
         while True:
             f_name, f_ext = os.path.splitext(_file)
             _file2 = f_name + '-' + str(random.randint(0, 10000000)) + f_ext
             if _file != _file2:
                 break
@@ -469,16 +471,17 @@
                     else:
                         fileno += 1
                         # print('忽略 --------------------', _file)
                 else:
                     fileok += 1
                     info.append(func(_file, *args, **kwargs))
 
-        print(' ----------- 处理 %s 个文件（跳过名称前面是：“%s”，处理后缀：“%s”） ----------- 忽略 %s 个文件 ----------- ' % (
-            fileok, prefix, suffix, fileno))
+        print(
+            ' ----------- 处理 %s 个文件（跳过名称前面是：“%s”，处理后缀：“%s”） ----------- 忽略 %s 个文件 ----------- ' % (
+                fileok, prefix, suffix, fileno))
     else:
         raise FileExistsError('请输入文件路径！')
     return info
 
 
 def get_walk_files(dir_path, endswith=''):
     """
@@ -779,14 +782,46 @@
 
     if remove_src:
         print(f'修改 {count} 删除 {remove_count}')
     else:
         print(f'修改 {count} 需要删除的文件 {remove_count}')
 
 
+def json_read(path):
+    """
+    读取 json 文件
+    """
+    try:
+        if not os.path.exists(path):
+            return False
+        with open(path, 'r', encoding='utf-8') as f:
+            obj = json.load(f)
+        return obj
+    except Exception as e:
+        print('json_read', e)
+        return False
+
+
+def json_save(obj, path):
+    """
+    保存 json 文件
+    """
+
+    if obj is None:
+        return False
+    else:
+        try:
+            with open(path, 'w', encoding='utf-8') as f:
+                json.dump(obj, f, ensure_ascii=False, indent=2)
+            return True
+        except Exception as e:
+            print('json_save', e)
+            return False
+
+
 def doc():
     """
     打印模块说明文档
     """
     doc_text = """
     # 默认字典的例子
     from collections import defaultdict
@@ -815,14 +850,16 @@
     doc_text += '{fun.__name__}{fun.__doc__}\n'.format(fun=exists_file)
     doc_text += '{fun.__name__}{fun.__doc__}\n'.format(fun=exists_file_to_bak)
     doc_text += '{fun.__name__}{fun.__doc__}\n'.format(fun=get_name)
     doc_text += '{fun.__name__}{fun.__doc__}\n'.format(fun=list_dir)
     doc_text += '{fun.__name__}{fun.__doc__}\n'.format(fun=from_dir_func)
     doc_text += '{fun.__name__}{fun.__doc__}\n'.format(fun=save_file)
     doc_text += '{fun.__name__}{fun.__doc__}\n'.format(fun=dir_compare)
+    doc_text += '{fun.__name__}{fun.__doc__}\n'.format(fun=json_read)
+    doc_text += '{fun.__name__}{fun.__doc__}\n'.format(fun=json_save)
     print(doc_text)
 
 
 if __name__ == '__main__':
     # 记录运行时间 --------------------------------------------------
     from time import time, sleep
```

### Comparing `ilds-2023.4.3/ilds/lib/browsercookie.py` & `ilds-2023.5.16/ilds/lib/browsercookie.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/lib/configobj/validate.py` & `ilds-2023.5.16/ilds/lib/configobj/validate.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/lib/configobj/__init__.py` & `ilds-2023.5.16/ilds/lib/configobj/__init__.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/lib/hexdump.py` & `ilds-2023.5.16/ilds/lib/hexdump.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/match_data.py` & `ilds-2023.5.16/ilds/match_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # ---------------------------------------
 #   程序：match_data.py
-#   版本：0.1
+#   版本：0.2
 #   作者：lds
-#   日期：2021-10-24
+#   日期：2023-04-27
 #   语言：Python 3.X
 #   说明：使用 pandas 匹配的函数集合
 # ---------------------------------------
 
 
 import os
 from collections import OrderedDict
@@ -111,14 +111,64 @@
         # print(df)
 
     # print(infos)
 
     return {'infos': infos, 'data': df}
 
 
+def df_search(_df, column, keyword, case=True, flags=0, na=None, regex=True):
+    """
+    在 DataFrame 中搜索
+
+    实现依靠 re.search，也可以是用 re.match
+
+    @param _df: 要搜索的 pandas.DataFrame
+    @param column: 要搜索的列名
+    @param keyword: str 要搜索的字符或正则表达式
+    @param case: 默认为 True，如果为 True 则区分大小写
+    @param flags: 默认0（无标志），标志将传递到RE模块，例如 re.IGNORECASE
+    @param na: 缺失值的可选填充值
+    @param regex: 默认为 True，如果为 True，则使用正则表达式。 如果是 False 则将视为字面字符串
+    @return: 搜索到的 pandas.DataFrame
+
+    # 可以看看
+    https://pandas.pydata.org/docs/reference/api/pandas.Series.str.contains.html?highlight=contains
+    https://pandas.pydata.org/docs/reference/api/pandas.Series.str.match.html#pandas.Series.str.match
+    https://pandas.pydata.org/docs/reference/api/pandas.Series.str.startswith.html#pandas.Series.str.startswith
+    https://pandas.pydata.org/docs/reference/api/pandas.Series.str.endswith.html#pandas.Series.str.endswith
+    https://pandas.pydata.org/docs/reference/api/pandas.Series.str.fullmatch.html#pandas.Series.str.fullmatch
+    https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.isin.html
+
+    ## 例子
+    # 创建一个 DataFrame
+    data = {
+        'name': ['Alice', 'Bob', 'Charlie', 'David', 'Eva'],
+        'age': [25, 30, 35, 40, 45],
+        'gender': ['F', 'M', 'M', 'M', 'F']
+    }
+    df = pd.DataFrame(data)
+
+    # 进行搜索
+    result = df_search(df, 'name', 'a', case=True, flags=0, na=None, regex=True)
+    print(result)
+
+    # 显示 DataFrame 的索引号和内容
+    for index, row in result.iterrows():
+        print(f'索引({type(index)}): {index}, 数据({type(row)}): {row}')
+    for index, row in zip(result.index, result.values):
+        print(f'索引({type(index)}): {index}, 数据({type(row)}): {row}')
+
+    # 在 pandas 中，可以使用比较运算符（如 >, <, ==, != 等）或 isin() 方法搜索指定的数字。
+    print(df[df['age'] == 25])
+    # 如果要搜索多个数字，可以使用 isin() 方法。例如，以下代码搜索 age 列中值为 25 或 30 的所有行：
+    print(df[df['age'].isin([25, 30])])
+    """
+    return _df[_df[column].str.contains(keyword, case=case, flags=flags, na=na, regex=regex)]
+
+
 def match_data(df1, df2, check_columns, replace_columns, is_digital):
     """
     匹配数据并填充匹配到的数据
     """
 
     infos = []
```

### Comparing `ilds-2023.4.3/ilds/md.py` & `ilds-2023.5.16/ilds/md.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/md5summer.py` & `ilds-2023.5.16/ilds/md5summer.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/mycsv.py` & `ilds-2023.5.16/ilds/mycsv.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/net.py` & `ilds-2023.5.16/ilds/net.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/pd.py` & `ilds-2023.5.16/ilds/pd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
 #
 # ---------------------------------------
 #   程序：pd.py
-#   版本：0.5
+#   版本：0.6
 #   作者：lds
-#   日期：2023-04-03
+#   日期：2023-04-27
 #   语言：Python 3.X
 #   说明：pandas 常用的函数集合，TODO 添加一些小抄在这里！
 # ---------------------------------------
 import os
 from pathlib import Path
 from collections import OrderedDict
 
 from colorama import Fore, Back, Style
 
 from ilds.file import get_dir_files
+from openpyxl import load_workbook
 
 try:
     import pandas as pd
 except ImportError as e:
     print(Fore.RED + "注：导入 pandas 失败，请安装它: pip install pandas", Style.RESET_ALL)
     pass
 
@@ -71,22 +72,32 @@
     :param add_source_column: 添加内容来源
     :param only_read_first_table: 只读取第一个表格
     :param is_print: 打印读取信息
     :return: {'file_name', 'index', 'sheet_name', 'sheet_names', 'count', 'columns', 'df'}
     """
     data = OrderedDict()
 
+    try:
+        wb = load_workbook(file, read_only=True)
+        sheet_state_data = {name: wb[name].sheet_state for name in wb.sheetnames}
+        # print(sheet_state_data)
+        wb.close()
+    except Exception as e:
+        print('get_excel_data 错误', e)
+        sheet_state_data = {}
+
     with pd.ExcelFile(file) as excel:
         sheet_names = excel.sheet_names
         if is_print:
             print('表薄名称列表：', sheet_names)
         # 通过表薄名字读取表单
         # data['总表'] = pd.read_excel(excel, sheet_name='总表')
         # 读取全部表
         for index, sheet_name in enumerate(sheet_names):
+            sheet_state = sheet_state_data.get(sheet_name, None)
             _df = pd.read_excel(excel, sheet_name=sheet_name, header=0)
             file_name = os.path.basename(file)
             count = len(_df)
 
             if is_print:
                 print('表薄名称：', sheet_name, '\t', '行数：', count, '\t', '文件：', file)
 
@@ -98,14 +109,15 @@
                 _df = _df[columns]
 
             df_data = {
                 'file_name': file_name,
                 'index': index,
                 'sheet_name': sheet_name,
                 'sheet_names': sheet_names,
+                'sheet_state': sheet_state,
                 'count': count,
                 'columns': list(_df.columns),
                 'df': _df,
             }
 
             if only_read_first_table:
                 data = df_data
@@ -129,36 +141,37 @@
     df_list = get_df_list(file, concat_columns, add_source_column, is_print)
     count = sum([len(df) for df in df_list])
     df = pd.concat(df_list, **concat_kwargs)  # result
     print('合并数据行数：', len(df), '导入数据行数统计：', count)
     return df
 
 
-def merging_excel_file_data(file_dir, ext='', concat_columns=None, add_source_column=True, is_print=True,
-                            get_files_function=None, **concat_kwargs):
+def merging_excel_file_data(file_dir_or_file_list, ext='', concat_columns=None, add_source_column=True, is_print=True,
+                            **concat_kwargs):
     """
     合并多个 Excel 文件内容
 
-    :param file_dir: 合并文件的路径
+    :param file_dir_or_file_list: 合并文件的路径或者文件列表
     :param ext: 要合并的文件后缀名，默认是文件夹中的全部文件
     :param concat_columns: 指定要合并的列名列表
     :param add_source_column: 是否添加原始来源
     :param is_print: 打印信息
-    :param get_files_function: 支持自定义获取文件的函数
     :return:
     """
-
-    if get_files_function is None:
-        get_files_function = get_dir_files
-
     all_len = 0
     frames = []
-    for file in get_files_function(file_dir, ext):
+
+    if isinstance(file_dir_or_file_list, list):
+        file_list = file_dir_or_file_list
+    else:
+        file_list = get_dir_files(file_dir_or_file_list, ext)
+
+    for file in file_list:
         if is_print:
-            print(file)
+            print('处理文件:', file)
         df_list = get_df_list(file, concat_columns, add_source_column, is_print)
         all_len += sum([len(df) for df in df_list])
         frames.extend(df_list)
 
     _df = pd.concat(frames, **concat_kwargs)  # result
     if is_print:
         print('合并数据行数：', len(_df), '原始数据行数：', all_len)
```

### Comparing `ilds-2023.4.3/ilds/spider.py` & `ilds-2023.5.16/ilds/spider.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/time.py` & `ilds-2023.5.16/ilds/time.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds/util.py` & `ilds-2023.5.16/ilds/util.py`

 * *Files identical despite different names*

### Comparing `ilds-2023.4.3/ilds.egg-info/PKG-INFO` & `ilds-2023.5.16/ilds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ilds
-Version: 2023.4.3
+Version: 2023.5.16
 Summary: 常用模块的集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/ilds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/ilds
 Description: ====================
```

### Comparing `ilds-2023.4.3/ilds.egg-info/SOURCES.txt` & `ilds-2023.5.16/ilds.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 setup.py
 ilds/__init__.py
 ilds/cmd.py
 ilds/everything.py
 ilds/excel_xlrd.py
 ilds/excel_xlsx.py
 ilds/file.py
-ilds/json.py
 ilds/match_data.py
 ilds/md.py
 ilds/md5summer.py
 ilds/mycsv.py
 ilds/net.py
 ilds/pd.py
 ilds/spider.py
```

### Comparing `ilds-2023.4.3/PKG-INFO` & `ilds-2023.5.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ilds
-Version: 2023.4.3
+Version: 2023.5.16
 Summary: 常用模块的集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/ilds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/ilds
 Description: ====================
```

### Comparing `ilds-2023.4.3/setup.py` & `ilds-2023.5.16/setup.py`

 * *Files identical despite different names*

