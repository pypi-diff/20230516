# Comparing `tmp/viewm2m-0.0.3.tar.gz` & `tmp/viewm2m-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viewm2m-0.0.3.tar", last modified: Tue May 16 13:58:28 2023, max compression
+gzip compressed data, was "viewm2m-0.0.4.tar", last modified: Tue May 16 14:13:05 2023, max compression
```

## Comparing `viewm2m-0.0.3.tar` & `viewm2m-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 13:58:28.740007 viewm2m-0.0.3/
--rw-r--r--   0 liufangjing   (501) staff       (20)      453 2023-05-16 13:58:28.739884 viewm2m-0.0.3/PKG-INFO
--rw-r--r--   0 liufangjing   (501) staff       (20)        0 2023-05-16 12:08:58.000000 viewm2m-0.0.3/README.md
--rw-r--r--   0 liufangjing   (501) staff       (20)       38 2023-05-16 13:58:28.740039 viewm2m-0.0.3/setup.cfg
--rw-r--r--   0 liufangjing   (501) staff       (20)     1924 2023-05-16 13:45:20.000000 viewm2m-0.0.3/setup.py
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 13:58:28.738886 viewm2m-0.0.3/viewm2m/
--rw-r--r--   0 liufangjing   (501) staff       (20)      367 2023-05-16 13:57:49.000000 viewm2m-0.0.3/viewm2m/__init__.py
--rw-r--r--   0 liufangjing   (501) staff       (20)     6540 2023-05-16 13:46:54.000000 viewm2m-0.0.3/viewm2m/captor.py
--rw-r--r--   0 liufangjing   (501) staff       (20)     6819 2023-05-16 13:43:11.000000 viewm2m-0.0.3/viewm2m/viewm2m.py
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 13:58:28.739731 viewm2m-0.0.3/viewm2m.egg-info/
--rw-r--r--   0 liufangjing   (501) staff       (20)      453 2023-05-16 13:58:28.000000 viewm2m-0.0.3/viewm2m.egg-info/PKG-INFO
--rw-r--r--   0 liufangjing   (501) staff       (20)      263 2023-05-16 13:58:28.000000 viewm2m-0.0.3/viewm2m.egg-info/SOURCES.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)        1 2023-05-16 13:58:28.000000 viewm2m-0.0.3/viewm2m.egg-info/dependency_links.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       50 2023-05-16 13:58:28.000000 viewm2m-0.0.3/viewm2m.egg-info/entry_points.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       29 2023-05-16 13:58:28.000000 viewm2m-0.0.3/viewm2m.egg-info/requires.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)        8 2023-05-16 13:58:28.000000 viewm2m-0.0.3/viewm2m.egg-info/top_level.txt
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 14:13:05.664034 viewm2m-0.0.4/
+-rw-r--r--   0 liufangjing   (501) staff       (20)      453 2023-05-16 14:13:05.663880 viewm2m-0.0.4/PKG-INFO
+-rw-r--r--   0 liufangjing   (501) staff       (20)        0 2023-05-16 12:08:58.000000 viewm2m-0.0.4/README.md
+-rw-r--r--   0 liufangjing   (501) staff       (20)       38 2023-05-16 14:13:05.664074 viewm2m-0.0.4/setup.cfg
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1924 2023-05-16 14:13:01.000000 viewm2m-0.0.4/setup.py
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 14:13:05.662877 viewm2m-0.0.4/viewm2m/
+-rw-r--r--   0 liufangjing   (501) staff       (20)      406 2023-05-16 14:12:49.000000 viewm2m-0.0.4/viewm2m/__init__.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)     6540 2023-05-16 14:11:57.000000 viewm2m-0.0.4/viewm2m/captor.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)     6819 2023-05-16 13:43:11.000000 viewm2m-0.0.4/viewm2m/viewm2m.py
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 14:13:05.663722 viewm2m-0.0.4/viewm2m.egg-info/
+-rw-r--r--   0 liufangjing   (501) staff       (20)      453 2023-05-16 14:13:05.000000 viewm2m-0.0.4/viewm2m.egg-info/PKG-INFO
+-rw-r--r--   0 liufangjing   (501) staff       (20)      263 2023-05-16 14:13:05.000000 viewm2m-0.0.4/viewm2m.egg-info/SOURCES.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)        1 2023-05-16 14:13:05.000000 viewm2m-0.0.4/viewm2m.egg-info/dependency_links.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       50 2023-05-16 14:13:05.000000 viewm2m-0.0.4/viewm2m.egg-info/entry_points.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       29 2023-05-16 14:13:05.000000 viewm2m-0.0.4/viewm2m.egg-info/requires.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)        8 2023-05-16 14:13:05.000000 viewm2m-0.0.4/viewm2m.egg-info/top_level.txt
```

### Comparing `viewm2m-0.0.3/setup.py` & `viewm2m-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="viewm2m",                                     # 包的分发名称，使用字母、数字、_、-
-    version="0.0.3",                                        # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
+    version="0.0.4",                                        # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
     author="byte",                                       # 作者名字
     author_email="liufangjing_byte@163.com",                      # 作者邮箱
     description="用于捕获接口并转换为可导入metersphere平台的json格式",                            # 包的简介描述
     long_description=long_description,                      # 包的详细介绍(一般通过加载README.md)
     long_description_content_type="text/markdown",          # 和上条命令配合使用，声明加载的是markdown文件
     url="https://github.com/zerobyte1o1/mitmproxy2metersphere",                              # 项目开源地址，我这里写的是同性交友官网，大家可以写自己真实的开源网址
     packages=setuptools.find_packages(),                    # 如果项目由多个文件组成，我们可以使用find_packages()自动发现所有包和子包，而不是手动列出每个包，在这种情况下，包列表将是example_pkg
```

### Comparing `viewm2m-0.0.3/viewm2m/captor.py` & `viewm2m-0.0.4/viewm2m/captor.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     await master.run()
     return master
 
 
 def run_asyncio_loop(loop):
     asyncio.set_event_loop(loop)
-    loop.run_until_complete(start_proxy('127.0.0.1', 8082))
+    loop.run_until_complete(start_proxy('127.0.0.1', 8083))
     loop.stop()
 
 
 class Middle:
     """
     中间层，用来记录中间数据
     """
@@ -134,15 +134,15 @@
         self.t.start()
         hb = BoxLayout(orientation='horizontal', size_hint_y=0.1)
         self.text_input = TextInput(text='graphql',
                                     font_size="25sp",
                                     size_hint_x=0.6,
                                     padding_y=20,
                                     foreground_color=[0, 0, 0, 0.8])
-        Middle.info_desk = '\n* Listening to localhost: 8082\n'
+        Middle.info_desk = '\n* Listening to localhost: 8083\n'
         Middle.info_desk += '* Cleared history and locking keywords: ' + Middle.keyword + '\n'
 
         Middle.info_desk += '-------------------------------------------------------------' \
                             '-----------------------------------------------------\n'
         hb.add_widget(self.text_input)
         button = Button(text='Update Keywords',
                         size_hint_x=0.2,
@@ -169,15 +169,15 @@
         superBox.add_widget(vb)
         Clock.schedule_interval(self.update_label, 0)
         return superBox
 
     def change_keyword(self, instance):
         Middle.keyword = self.text_input.text
         Middle.new_status = True
-        Middle.info_desk = '\n* Listening to localhost: 8082\n'
+        Middle.info_desk = '\n* Listening to localhost: 8083\n'
         Middle.info_desk += '* Cleared history and locking keywords: ' + Middle.keyword + '\n'
 
         Middle.info_desk += '-------------------------------------------------------------' \
                             '-----------------------------------------------------\n'
 
     def toggle_record(self, instance):
         Middle.record = not Middle.record
```

### Comparing `viewm2m-0.0.3/viewm2m/viewm2m.py` & `viewm2m-0.0.4/viewm2m/viewm2m.py`

 * *Files identical despite different names*

