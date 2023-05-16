# Comparing `tmp/logop-0.5.0.tar.gz` & `tmp/logop-0.6.0.tar.gz`

## Comparing `logop-0.5.0.tar` & `logop-0.6.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    14151 2020-02-02 00:00:00.000000 logop-0.5.0/src/logop/__init__.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 logop-0.5.0/LICENSE
--rw-r--r--   0        0        0     7956 2020-02-02 00:00:00.000000 logop-0.5.0/README.md
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 logop-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     8149 2020-02-02 00:00:00.000000 logop-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    15295 2020-02-02 00:00:00.000000 logop-0.6.0/src/logop/__init__.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 logop-0.6.0/LICENSE
+-rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 logop-0.6.0/README.md
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 logop-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 logop-0.6.0/PKG-INFO
```

### Comparing `logop-0.5.0/src/logop/__init__.py` & `logop-0.6.0/src/logop/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import datetime
 import threading
 import multiprocessing
 
 from typing import Union
 
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 
 ALL      = - 0x80
 TRACE    = - 0x40
 DEBUG    = - 0x20
 INFO     =   0x00
 WARN     =   0x20
@@ -66,15 +66,15 @@
     'warn': (WARN, 'WARN'),
     'warning': (WARNING, 'WARNING'),
     'severe': (SEVERE, 'SEVERE'),
     'error': (ERROR, 'ERROR'),
     'fatal': (FATAL, 'FATAL'),
     'critical': (CRITICAL, 'CRITICAL')
 }
-#? levelTable[alias] = [level, levelname]
+# ? levelTable[alias] = [level, levelname]
 
 
 
 def op_character_variable(op_format: str, table: dict) -> str:
     if not isinstance(op_format, str):
         raise TypeError('The op_format type is not str.')
 
@@ -126,15 +126,15 @@
 
         if level < 0x10:
             sys.stdout.write(ops)
             sys.stdout.flush()
 
         else:
             sys.stderr.write(ops)
-            sys.stdout.flush()
+            sys.stderr.flush()
 
 
 
 class Logop_standard_up(BaseLogop):
     def call(self, content: dict, op_format: str = FORMAT.DEFAULT) -> None:
         if not isinstance(content, dict):
             raise TypeError('The content type is not dict.')
@@ -161,15 +161,15 @@
 
         if level < 0x10:
             sys.stdout.write(ops)
             sys.stdout.flush()
 
         else:
             sys.stderr.write(ops)
-            sys.stdout.flush()
+            sys.stderr.flush()
 
 
 
 class Logop_file(BaseLogop):
     op_name = 'logfile'
     op_type = 'logfile'
 
@@ -220,44 +220,46 @@
                  *, stdout: bool = True, asynchronous: bool = False, threadname: str = 'LoggingThread'):
         self.__level = INFO
         self.__op_format = FORMAT.DEFAULT
         self.__op_list = []
 
         self.__call_lock = threading.RLock()
         self.__set_lock = threading.RLock()
+        self.__is_close = False
 
         self.setlevel(level)
         self.setformat(op_format)
 
         if stdout: self.add_op(Logop_standard())
 
-        self.__asynchronous = True if asynchronous else False
+        self.__asynchronous = bool(asynchronous)
 
         if self.__asynchronous:
             self.__call_event = threading.Event()
             self.__message_list = []
-            self.__asynchronous_task = threading.Thread(None,self.__run_cycle, threadname, (), {}, daemon=True)
+            self.__asynchronous_task = threading.Thread(None,self.__run_cycle, threadname, (), {}, daemon=False)
             self.__asynchronous_task.start()
+            self.__asynchronous_stop = False
 
 
     def setlevel(self, level:   Union[int, str]) -> None:
         with self.__set_lock:
             if isinstance(level, int):
                 lv = level
 
             elif isinstance(level, str):
                 if level not in levelTable:
                     raise ValueError('The level alias does not exist.')
-                
+
                 lv = levelTable[level][0]
 
             else:
                 raise TypeError('The level type is not int.')
 
-            if not -0x80 <= level <= 0x7F:
+            if not -0x80 <= lv <= 0x7F:
                 raise ValueError('level should be somewhere between -0x80 to 0x7F .')
 
             self.__level = lv
 
 
     def setformat(self, op_format: str) -> None:
         with self.__set_lock:
@@ -350,14 +352,44 @@
             for opobj in self.__op_list:
                 if opobj.op_type == BaseLogop.op_type:
                     return opobj.op_ident
 
             else:
                 return None
 
+
+    def join(self, timeout: Union[float, None] = None) -> None:
+        if not self.__asynchronous:
+            raise RuntimeError("The logging mode is not asynchronous.")
+
+        self.__asynchronous_task.join(timeout)
+
+
+    def close(self) -> None:
+        with self.__set_lock:
+            # if self.__is_close:
+            #     raise RuntimeError("")
+
+            # if not self.__asynchronous:
+            #     raise RuntimeError("The logging mode is not asynchronous.")
+
+            # if self.__asynchronous_stop:
+            #     raise RuntimeError("This method can only be called once.")
+
+            self.__is_close = True
+
+            if self.__asynchronous:
+                self.__asynchronous_stop = True
+                self.__call_event.set()
+
+
+    def is_close(self) -> bool:
+        with self.__set_lock:
+            return self.__is_close
+
     #! fallibility
     def __try_op_call(self, content: dict) -> None:
         with self.__set_lock:
             call_list = self.__op_list.copy()
 
         with self.__call_lock:
             for stdop in call_list:
@@ -382,27 +414,33 @@
 
 
     def __run_cycle(self, *args, **kwds):
         while True:
             self.__call_event.wait()
             self.__try_op_call_asynchronous()
             self.__call_event.clear()
+            if self.__asynchronous_stop:
+                raise SystemExit()
 
 
     def __run_call_asynchronous(self, content: dict) -> None:
         with self.__call_lock: self.__message_list.append(content)
         self.__call_event.set()
 
 
     def __run_call(self, content: dict) -> None:
         if self.__asynchronous: self.__run_call_asynchronous(content)
         else: self.__try_op_call(content)
 
 
     def call(self, level: int = INFO, levelname: str = 'INFO', message: str = '', *, double_back: bool = False) -> None:
+        with self.__set_lock:
+            if self.__is_close:
+                raise ValueError("call of closed logging.")
+
         if level < self.__level: return None
 
         now = datetime.datetime.now()
 
         content = {}
         content['level'] = level
         content['levelname'] = levelname
```

### Comparing `logop-0.5.0/LICENSE` & `logop-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logop-0.5.0/README.md` & `logop-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 # 在日志对象需要进行输出时会调用这个方法
 # content: 日志内容, 通常是日志对象收集到的信息
 # op_format: 日志格式
 # BaseLogop 的 call 方法不会进行任何输出
 
 .add_exception_count() -> None
 # 增加异常计数
-# 在日志对象调用输出对象的 call 方法发送异常时会调用这个方法,
+# 在日志对象调用输出对象的 call 方法发生异常时会调用这个方法,
 # 使得输出对象内部的异常计数 + 1.
 
 
 .op_type -> str
 # 输出对象的类型标识
 # 非标准输出对象需要重写这个标识
 
@@ -259,21 +259,38 @@
 # 获取到输出对象
 # 当提供的 ident 标识存在时返回这个输出对象, 否则返回 None.
 
 .get_stdop_object() -> BaseLogop | None
 # 获取到标准输出对象
 # 当存在标准输出对象时返回输出对象, 否则返回 None.
 
+# v0.6.0 new
+.join(timeout: float | None = None) -> None
+# 等待日志记录器线程结束
+# 仅在异步模式下有效, 否则抛出 RuntimeError 异常.
+# timeout: 超时时间, 单位为秒.
+
+# v0.6.0 new
+.close() -> None
+# 关闭日志记录器
+# 关闭之后日志记录器不再可用.
+
+# v0.6.0 new
+.is_close() -> bool
+# 日志记录器是否已被关闭
+
 .call(level: int = INFO, levelname: str = 'INFO', message: str = '',
       *, double_back: bool = False) -> None
 # 输出日志
 # level: 日志等级, 当等级低于设置等级时不进行日志输出.
 # levelname: 日志名称, 任意, 但推荐为 INFO, WARN, ERROR, DEBUG 等标准名称.
 # message: 日志消息.
 # double_back: 是否要从上上个栈帧中获取状态信息, 对该方法进行包装时会用到它.
+# v0.6.0 new
+# 若日志记录器被关闭, 会直接抛出 ValueError 异常.
 
 .trace(message) -> None
 # 输出一个 TRACE 级别的日志
 
 .debug(message) -> None
 .info(message) -> None
 .warn(message) -> None
```

### Comparing `logop-0.5.0/pyproject.toml` & `logop-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "logop"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
   { name="numLinka", email="numlinka@163.com" },
 ]
 description = "A simple log module"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `logop-0.5.0/PKG-INFO` & `logop-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logop
-Version: 0.5.0
+Version: 0.6.0
 Summary: A simple log module
 Project-URL: Homepage, https://github.com/numlinka/pylogop
 Project-URL: Bug Tracker, https://github.com/numlinka/pylogop/issues
 Author-email: numLinka <numlinka@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -169,15 +169,15 @@
 # 在日志对象需要进行输出时会调用这个方法
 # content: 日志内容, 通常是日志对象收集到的信息
 # op_format: 日志格式
 # BaseLogop 的 call 方法不会进行任何输出
 
 .add_exception_count() -> None
 # 增加异常计数
-# 在日志对象调用输出对象的 call 方法发送异常时会调用这个方法,
+# 在日志对象调用输出对象的 call 方法发生异常时会调用这个方法,
 # 使得输出对象内部的异常计数 + 1.
 
 
 .op_type -> str
 # 输出对象的类型标识
 # 非标准输出对象需要重写这个标识
 
@@ -273,21 +273,38 @@
 # 获取到输出对象
 # 当提供的 ident 标识存在时返回这个输出对象, 否则返回 None.
 
 .get_stdop_object() -> BaseLogop | None
 # 获取到标准输出对象
 # 当存在标准输出对象时返回输出对象, 否则返回 None.
 
+# v0.6.0 new
+.join(timeout: float | None = None) -> None
+# 等待日志记录器线程结束
+# 仅在异步模式下有效, 否则抛出 RuntimeError 异常.
+# timeout: 超时时间, 单位为秒.
+
+# v0.6.0 new
+.close() -> None
+# 关闭日志记录器
+# 关闭之后日志记录器不再可用.
+
+# v0.6.0 new
+.is_close() -> bool
+# 日志记录器是否已被关闭
+
 .call(level: int = INFO, levelname: str = 'INFO', message: str = '',
       *, double_back: bool = False) -> None
 # 输出日志
 # level: 日志等级, 当等级低于设置等级时不进行日志输出.
 # levelname: 日志名称, 任意, 但推荐为 INFO, WARN, ERROR, DEBUG 等标准名称.
 # message: 日志消息.
 # double_back: 是否要从上上个栈帧中获取状态信息, 对该方法进行包装时会用到它.
+# v0.6.0 new
+# 若日志记录器被关闭, 会直接抛出 ValueError 异常.
 
 .trace(message) -> None
 # 输出一个 TRACE 级别的日志
 
 .debug(message) -> None
 .info(message) -> None
 .warn(message) -> None
```

