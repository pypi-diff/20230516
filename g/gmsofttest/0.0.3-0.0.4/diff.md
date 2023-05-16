# Comparing `tmp/gmsofttest-0.0.3.tar.gz` & `tmp/gmsofttest-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gmsofttest-0.0.3.tar", last modified: Mon May 15 13:07:33 2023, max compression
+gzip compressed data, was "dist\gmsofttest-0.0.4.tar", last modified: Tue May 16 02:50:11 2023, max compression
```

## Comparing `gmsofttest-0.0.3.tar` & `gmsofttest-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 13:07:33.000000 gmsofttest-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-02-11 08:11:24.000000 gmsofttest-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      787 2023-05-15 13:07:33.000000 gmsofttest-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-15 13:05:45.000000 gmsofttest-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-15 13:07:33.000000 gmsofttest-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      801 2023-05-15 13:07:28.000000 gmsofttest-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 13:07:33.000000 gmsofttest-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-15 13:07:33.000000 gmsofttest-0.0.3/src/gmsofttest/
--rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.3/src/gmsofttest/__init__.py
--rw-rw-rw-   0        0        0    89848 2023-04-22 07:37:37.000000 gmsofttest-0.0.3/src/gmsofttest/china_address.py
--rw-rw-rw-   0        0        0     2071 2023-03-11 05:43:46.000000 gmsofttest-0.0.3/src/gmsofttest/getrandomdata.py
--rw-rw-rw-   0        0        0    12336 2023-05-15 13:03:09.000000 gmsofttest-0.0.3/src/gmsofttest/mysqlconn.py
-drwxrwxrwx   0        0        0        0 2023-05-15 13:07:33.000000 gmsofttest-0.0.3/src/gmsofttest.egg-info/
--rw-rw-rw-   0        0        0      787 2023-05-15 13:07:33.000000 gmsofttest-0.0.3/src/gmsofttest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-05-15 13:07:33.000000 gmsofttest-0.0.3/src/gmsofttest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 13:07:33.000000 gmsofttest-0.0.3/src/gmsofttest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-15 13:07:33.000000 gmsofttest-0.0.3/src/gmsofttest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-02-11 08:11:24.000000 gmsofttest-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      908 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-05-16 02:49:52.000000 gmsofttest-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      801 2023-05-16 02:49:57.000000 gmsofttest-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/src/gmsofttest/
+-rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.4/src/gmsofttest/__init__.py
+-rw-rw-rw-   0        0        0    89848 2023-04-22 07:37:37.000000 gmsofttest-0.0.4/src/gmsofttest/china_address.py
+-rw-rw-rw-   0        0        0      983 2023-05-16 01:57:10.000000 gmsofttest-0.0.4/src/gmsofttest/gm_parse_response.py
+-rw-rw-rw-   0        0        0     2137 2023-05-16 01:35:08.000000 gmsofttest-0.0.4/src/gmsofttest/gm_randomdata.py
+-rw-rw-rw-   0        0        0    12431 2023-05-16 01:35:08.000000 gmsofttest-0.0.4/src/gmsofttest/gm_sqlconn.py
+-rw-rw-rw-   0        0        0     3127 2023-05-16 01:56:18.000000 gmsofttest-0.0.4/src/gmsofttest/gm_timestamp.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/src/gmsofttest.egg-info/
+-rw-rw-rw-   0        0        0      908 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/src/gmsofttest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/src/gmsofttest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/src/gmsofttest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/src/gmsofttest.egg-info/top_level.txt
```

### Comparing `gmsofttest-0.0.3/LICENSE` & `gmsofttest-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.3/setup.py` & `gmsofttest-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gmsofttest",
-    version="0.0.3",
+    version="0.0.4",
     author="ronaldsu",
     author_email="uph4rmt@dingtalk.com",
     description="大家软件内部测试技术线支撑工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.gec123.com",
     project_urls={
```

### Comparing `gmsofttest-0.0.3/src/gmsofttest/china_address.py` & `gmsofttest-0.0.4/src/gmsofttest/china_address.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.3/src/gmsofttest/getrandomdata.py` & `gmsofttest-0.0.4/src/gmsofttest/gm_randomdata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Name : getrandomdata.py
+Name : gm_randomdata.py
 Author  : 写上自己的名字
 Contact : 邮箱地址
 Time    : 2023-02-13 10:11
 Desc:
 """
 
 """
@@ -67,15 +67,19 @@
     return fake.pyint(min_value=min_value, max_value=max_value, step=step)
 
 def getFloat(min_value=0, max_value=10000, step=1):
     """生成长度在min_chars到max_chars之间的浮点数"""
     return fake.pyint(min_value=min_value, max_value=max_value, step=step)
 
 def getStr(min_chars=None, max_chars=20):
-    """生成长度在min_chars到max_chars之间的字符串"""
+    """生成长度在min_chars到max_chars之间的字符串
+    :param min_chars:
+    :param max_chars:
+    :return:
+    """
     return fake.pystr(min_chars=min_chars, max_chars=max_chars)
 
 def getLinuxTimestamp(t=1):
     """获取当前linux时间戳"""
     if t == 1:
         st = round(time.time()*1000)
     return st
```

### Comparing `gmsofttest-0.0.3/src/gmsofttest/mysqlconn.py` & `gmsofttest-0.0.4/src/gmsofttest/gm_sqlconn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Name : mysqlconn.py
+Name : gm_sqlconn.py
 Author  : 写上自己的名字
 Contact : 邮箱地址
 Time    : 2021/3/22 15:52
 Desc: 操作MYSQL数据库
 """
 
 
@@ -36,14 +36,15 @@
 # 使用15服务器的sql容器
 test2_zcj_sql_port = 34404
 test2_xcj_sql_port = 34004
 test2_inner_sql_port = 34604
 
 
 class OperateMysql(object):
+    """快速连接gmsoft内部测试数据库"""
     def __init__(self, env, host):
 
         # 账号密码初始化
         self.user = user
         self.password = password
         self.host = host
 
@@ -55,15 +56,15 @@
             self.jydw_port = test2_jydw_sql_port
             try:
                 self.jydn_conn = pymysql.connect(host=self.env, user=self.user,
                                                      password=self.password, port=self.jydn_port, charset='utf8mb4')
                 self.jydw_conn = pymysql.connect(host=self.env, user=self.user,
                                                      password=self.password, port=self.jydw_port, charset='utf8mb4')
             except TimeoutError as e:
-                print("连接超时：{}".format(e))
+                print('连接超时：{}'.format(e))
 
             print("已创建jydn数据库连接,链接信息{}:{}".format(self.host, self.jydn_port))
             print("已创建jydw数据库连接,链接信息{}:{}".format(self.host, self.jydw_port))
 
         elif env == 'test2':
             # test2特殊处理，ip应该是192.168.2.15
             self.env = env15
@@ -74,17 +75,17 @@
                 self.zcj_conn = pymysql.connect(host=self.env, user=self.user,
                                                      password=self.password, port=self.zcj_port, charset='utf8mb4')
                 self.xcj_conn = pymysql.connect(host=self.env, user=self.user,
                                                      password=self.password, port=self.xcj_port, charset='utf8mb4')
                 self.inner_conn = pymysql.connect(host=self.env, user=self.user,
                                                        password=self.password, port=self.inner_port, charset='utf8mb4')
             except TimeoutError as e:
-                print("连接超时：{}".format(e))
-            print("已创建zcj数据库连接,链接信息{}:{}".format(self.env, self.zcj_port))
-            print("已创建xcj数据库连接,链接信息{}:{}".format(self.env, self.xcj_port))
+                print('连接超时：{}'.format(e))
+            print('已创建zcj数据库连接,链接信息{}:{}'.format(self.env, self.zcj_port))
+            print('已创建xcj数据库连接,链接信息{}:{}'.format(self.env, self.xcj_port))
             print("已创建inner数据库连接,链接信息{}:{}".format(self.env, self.inner_port))
 
         elif env == 'show':
             self.env = env20
             self.xcj_port = show_xcj_sql_port
             self.zcj_port = show_zcj_sql_port
             self.inner_port = show_inner_sql_port
@@ -230,15 +231,16 @@
             print("SQL执行时类型错误！请检查,{}".format(e))
         except Exception as e:
             print("执行sql异常:%s" % e)
 
     def delete_data(self, host, sql):
         """
         查询所有数据
-        :param sql:
+        :param host:  zcj、xcj
+        :param sql: SQL查询
         :return:
         """
         try:
             if host == 'zcj':
                 self.zcj_cursor.execute(sql)
                 self.zcj_cursor.commit()
             elif host == 'xcj':
```

