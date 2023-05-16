# Comparing `tmp/aio_dt_protocol-0.9.3.tar.gz` & `tmp/aio_dt_protocol-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_dt_protocol-0.9.3.tar", last modified: Fri Apr  7 08:37:13 2023, max compression
+gzip compressed data, was "aio_dt_protocol-0.9.4.tar", last modified: Tue May 16 08:57:38 2023, max compression
```

## Comparing `aio_dt_protocol-0.9.3.tar` & `aio_dt_protocol-0.9.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 08:37:13.760469 aio_dt_protocol-0.9.3/
--rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-0.9.3/LICENSE
--rw-rw-rw-   0        0        0     6559 2023-04-07 08:37:13.760934 aio_dt_protocol-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     5815 2023-04-06 13:39:16.000000 aio_dt_protocol-0.9.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 08:37:13.451966 aio_dt_protocol-0.9.3/aio_dt_protocol/
--rw-rw-rw-   0        0        0    34959 2023-04-05 07:22:52.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/Actions.py
--rw-rw-rw-   0        0        0    52666 2023-04-06 19:40:03.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/Browser.py
--rw-rw-rw-   0        0        0     9971 2023-04-04 10:33:45.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/BrowserEx.py
--rw-rw-rw-   0        0        0    35317 2023-04-05 07:22:52.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/DOMElement.py
--rw-rw-rw-   0        0        0    32529 2023-04-05 17:29:55.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/Data.py
--rw-rw-rw-   0        0        0    22749 2023-04-06 07:01:02.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/Page.py
--rw-rw-rw-   0        0        0    16198 2023-04-06 13:11:03.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/PageEx.py
--rw-rw-rw-   0        0        0      399 2023-04-07 08:27:54.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 08:37:13.759437 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/
--rw-rw-rw-   0        0        0     3631 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/BackgroundService.py
--rw-rw-rw-   0        0        0    13809 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Browser.py
--rw-rw-rw-   0        0        0     7070 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/CSS.py
--rw-rw-rw-   0        0        0     2045 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Console.py
--rw-rw-rw-   0        0        0    16735 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/DOM.py
--rw-rw-rw-   0        0        0     1846 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/DeviceOrientation.py
--rw-rw-rw-   0        0        0    24645 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Emulation.py
--rw-rw-rw-   0        0        0    23128 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Fetch.py
--rw-rw-rw-   0        0        0     2066 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Log.py
--rw-rw-rw-   0        0        0    22099 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Network.py
--rw-rw-rw-   0        0        0     2124 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Overlay.py
--rw-rw-rw-   0        0        0    35374 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Page.py
--rw-rw-rw-   0        0        0    32897 2023-04-05 17:56:11.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Runtime.py
--rw-rw-rw-   0        0        0     1712 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/SystemInfo.py
--rw-rw-rw-   0        0        0    17569 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Target.py
--rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/domains/__init__.py
--rw-rw-rw-   0        0        0     3148 2023-04-05 17:16:11.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/exceptions.py
--rw-rw-rw-   0        0        0     1645 2023-04-06 13:08:53.000000 aio_dt_protocol-0.9.3/aio_dt_protocol/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 08:37:13.479895 aio_dt_protocol-0.9.3/aio_dt_protocol.egg-info/
--rw-rw-rw-   0        0        0     6559 2023-04-07 08:37:13.000000 aio_dt_protocol-0.9.3/aio_dt_protocol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1083 2023-04-07 08:37:13.000000 aio_dt_protocol-0.9.3/aio_dt_protocol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 08:37:13.000000 aio_dt_protocol-0.9.3/aio_dt_protocol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-07 08:37:13.000000 aio_dt_protocol-0.9.3/aio_dt_protocol.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-07 08:37:13.000000 aio_dt_protocol-0.9.3/aio_dt_protocol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-0.9.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-07 08:37:13.761932 aio_dt_protocol-0.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1503 2023-04-06 10:09:07.000000 aio_dt_protocol-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:57:38.187239 aio_dt_protocol-0.9.4/
+-rw-rw-rw-   0        0        0     1526 2023-04-05 18:37:56.000000 aio_dt_protocol-0.9.4/LICENSE
+-rw-rw-rw-   0        0        0     6559 2023-05-16 08:57:38.187239 aio_dt_protocol-0.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5815 2023-04-06 13:39:16.000000 aio_dt_protocol-0.9.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 08:57:38.019294 aio_dt_protocol-0.9.4/aio_dt_protocol/
+-rw-rw-rw-   0        0        0    34959 2023-04-05 07:22:52.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/Actions.py
+-rw-rw-rw-   0        0        0    53858 2023-05-16 08:36:51.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/Browser.py
+-rw-rw-rw-   0        0        0     9971 2023-04-04 10:33:45.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/BrowserEx.py
+-rw-rw-rw-   0        0        0    35317 2023-04-05 07:22:52.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/DOMElement.py
+-rw-rw-rw-   0        0        0    32529 2023-04-05 17:29:55.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/Data.py
+-rw-rw-rw-   0        0        0    22749 2023-04-06 07:01:02.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/Page.py
+-rw-rw-rw-   0        0        0    16198 2023-04-06 13:11:03.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/PageEx.py
+-rw-rw-rw-   0        0        0      453 2023-05-16 08:36:51.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:57:38.186238 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/
+-rw-rw-rw-   0        0        0     3631 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/BackgroundService.py
+-rw-rw-rw-   0        0        0    13809 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Browser.py
+-rw-rw-rw-   0        0        0     7070 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/CSS.py
+-rw-rw-rw-   0        0        0     2045 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Console.py
+-rw-rw-rw-   0        0        0    16735 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/DOM.py
+-rw-rw-rw-   0        0        0     1846 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/DeviceOrientation.py
+-rw-rw-rw-   0        0        0    24645 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Emulation.py
+-rw-rw-rw-   0        0        0    23128 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Fetch.py
+-rw-rw-rw-   0        0        0     2066 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Log.py
+-rw-rw-rw-   0        0        0    22099 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Network.py
+-rw-rw-rw-   0        0        0     2124 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Overlay.py
+-rw-rw-rw-   0        0        0    35374 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Page.py
+-rw-rw-rw-   0        0        0    32897 2023-04-05 17:56:11.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Runtime.py
+-rw-rw-rw-   0        0        0     1712 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/SystemInfo.py
+-rw-rw-rw-   0        0        0    17569 2023-04-04 09:48:23.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Target.py
+-rw-rw-rw-   0        0        0        0 2021-06-02 19:57:07.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/domains/__init__.py
+-rw-rw-rw-   0        0        0     3148 2023-04-05 17:16:11.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/exceptions.py
+-rw-rw-rw-   0        0        0     1645 2023-04-06 13:08:53.000000 aio_dt_protocol-0.9.4/aio_dt_protocol/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:57:38.041289 aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/
+-rw-rw-rw-   0        0        0     6559 2023-05-16 08:57:37.000000 aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1083 2023-05-16 08:57:37.000000 aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 08:57:37.000000 aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-16 08:57:37.000000 aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-16 08:57:37.000000 aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-04-06 10:50:43.000000 aio_dt_protocol-0.9.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 08:57:38.189237 aio_dt_protocol-0.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1503 2023-04-06 10:09:07.000000 aio_dt_protocol-0.9.4/setup.py
```

### Comparing `aio_dt_protocol-0.9.3/LICENSE` & `aio_dt_protocol-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/PKG-INFO` & `aio_dt_protocol-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio_dt_protocol
-Version: 0.9.3
+Version: 0.9.4
 Summary: Asynchronous wrapper over Chromium browser debugger protocol.
 Home-page: https://github.com/PieceOfGood/aio_dt_protocol
 Author: PieceOfGood
 Author-email: 78sanchezz@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aio_dt_protocol-0.9.3/README.md` & `aio_dt_protocol-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/Actions.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/Actions.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/Browser.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/Browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         return {} if for_port else result
 
     def __init__(
             self,
             profile_path: str = "testProfile",
             dev_tool_profiles:  bool = False,
             url: Optional[Union[str, bytes]] = None,
-            flags:  Optional[List[str]] = None,
+            flags:  Optional["FlagBuilder"] = None,
             browser_path: str = "",
             debug_port:   Union[str, int] = 9222,
             browser_pid:  int = 0,
             app:         bool = False,
             browser_exe:  str = "chrome",
             proxy_address:str = "http://127.0.0.1",
             proxy_port:   Union[str, int] = "",
@@ -224,15 +224,15 @@
             browser_path = browser_path if browser_path else os.popen("which " + browser_exe).read().strip()
 
         if not os.path.exists(browser_path) or not os.path.isfile(browser_path):
             raise FileNotFoundError(f"Переданный 'browser_path' => '{browser_path}' — не существует, или содержит ошибку")
         self.browser_path = browser_path
 
         if int(debug_port) <= 0:
-            raise ValueError(f"Значение 'debug_port' => '{debug_port}' — должно быть положителным целым числом!")
+            raise ValueError(f"Значение 'debug_port' => '{debug_port}' — должно быть положительным целым числом!")
         self.debug_port = str(debug_port)
         self.proxy_addres = proxy_address
         self.proxy_port = str(proxy_port)
         self.verbose = verbose
 
         # https://stackoverflow.com/questions/2381241/what-is-the-subprocess-popen-max-length-of-the-args-parameter
         # data_url_len_is_high = len(url[0]) > 32_767
@@ -266,15 +266,15 @@
                         # иначе декодировать и установить её как Base64
                         "data:text/html;Base64," + url.decode()
         )
 
         self.is_headless_mode = False
         self.browser_pid = browser_pid if browser_pid > 0 else self._RunBrowser(_url_, flags, position, sizes)
 
-    def _RunBrowser(self, url: str, flags: list, position: Optional[Tuple[int, int]] = None,
+    def _RunBrowser(self, url: str, flags: "FlagBuilder", position: Optional[Tuple[int, int]] = None,
                     sizes: Optional[Tuple[int, int]] = None) -> int:
         """
         Запускает браузер с переданными флагами.
         :param url:             Адрес. Если передан, будет загружен в первой вкладке.
         :param flags:           Флаги
         :return:                ProcessID запущенного браузера
         """
@@ -287,14 +287,15 @@
             (CMDFlags.Background.disable_breakpad, []),
             (CMDFlags.Background.no_recovery_component, []),
             (CMDFlags.Background.disable_sync, []),
             (CMDFlags.Background.disable_domain_reliability, []),
             (CMDFlags.Background.no_service_autorun, []),
             (CMDFlags.Performance.disable_gpu_shader_disk_cache, []),
             (CMDFlags.Performance.disk_cache_dir, ["null"]),
+            (CMDFlags.Performance.media_cache_dir, ["null"]),
             (CMDFlags.Render.enable_features_WebUIDarkMode, []),
             (CMDFlags.Render.force_dark_mode, []),
         )
         run_args = [ self.browser_path ]
         flag_box.custom(url)
 
         # ! Default mode
@@ -306,28 +307,27 @@
                 flag_box.add(CMDFlags.Screen.window_size, *sizes)
 
         # ! Headless mode
         else:
             flag_box.add(CMDFlags.Headless.headless)
             self.is_headless_mode = True
 
-
         if self.proxy_port:
             flag_box.add(CMDFlags.Other.proxy_server, self.proxy_addres + ":" + self.proxy_port)
             if self.verbose:
                 log(f"Run browser {self.browser_name!r} on port: {self.debug_port} with proxy " +
                       f"on http://127.0.0.1:{self.proxy_port}")
         else:
             if self.verbose:
                 log(f"Run browser {self.browser_name!r} on port: {self.debug_port}")
 
-        run_args += flag_box.flags()
-
         if flags is not None:
-            run_args += flags
+            flag_box += flags
+
+        run_args += flag_box.flags()
         return subprocess.Popen(run_args).pid
 
     def KillBrowser(self) -> None:
         """
         "Убивает" процесс браузера. Рекомендуется только в крайних случаях.
             Лучше всего вызывать метод Call("Browser.close") у инстанса страницы
         :return:
@@ -496,55 +496,72 @@
                                 всех событий страницы в виде словаря.
         :return:        <Page>
         """
         return await self.GetPageBy("url", value, match_mode, index, callback)
 
 
 class FlagBuilder:
-
+    """ Обеспечивает последовательность неповторяющихся флагов
+    для запуска браузера.
+    """
     def __init__(self):
-        self._flags: set = set()
+        self._flags: Dict[str, Tuple[str]] = {}
 
-    def add(self, flag: "CMDFlag", *args: Union[str, int, float], separator: str = ",") -> None:
-        """
-        Принимает один флаг, его аргументы и разделитель аргументов.
-        """
-        f = flag.value
+    def add(self, flag: "CMDFlag", *args: Union[str, int, float]) -> None:
+        """ Принимает один флаг и его аргументы. """
+        f: str = flag.value
         if f[-1] == "=":
             if not args:
                 raise FlagArgumentContainError(
                     f"Для флага {flag.name} ожидается аргумент, или список аргументов.")
-            for arg in args:
-                f += str(arg) + separator
-            f = f[:-1]
-        self._flags.add(f)
-
-    def set(self, *flags: Sequence["CMDFlag", Sequence[Union[str, int, float]]], separator: str = ",") -> None:
-        """
-        Принимает произвольную последовательность флагов, из последовательностей, содержащих сам флаг и
-            его аргументы, а так же разделитель аргументов:
-                object.set(
-                    (CMDFlags.Background.disable_breakpad, []),
-                    (CMDFlags.Background.no_recovery_component, []),
-                    separator=" "
-                )
-        """
-        for flag in flags:
-            cmd_flag, args = flag
-            self.add(cmd_flag, *args, separator=separator)
 
-    def custom(self, flag: str) -> None:
+            self._flags[f] = tuple(map(str, args))
+        else:
+            self._flags[f] = tuple()
+
+    def set(self, *flags: Tuple["CMDFlag", Sequence[Union[str, int, float]]]) -> None:
+        """ Принимает произвольную последовательность флагов, из кортежей,
+         содержащих сам флаг и его аргументы:
+            object.set(
+                (CMDFlags.Background.disable_breakpad, []),
+                (CMDFlags.Background.no_recovery_component, [])
+            )
         """
-        Принимает строку в качестве флага.
-            object.custom("--mute-audio")
+        for cmd_flag, args in flags:
+            self.add(cmd_flag, *args)
+
+    def custom(self, flag: str) -> None:
+        """ Принимает строку в качестве флага.
+        object.custom("--mute-audio")
         """
-        self._flags.add(flag)
+        self._flags[flag] = tuple()
 
-    def flags(self) -> list[str]:
-        return list(self._flags)
+    def flags(self) -> List[str]:
+        result: List[str] = []
+        for cmd_flag, args in self._flags.items():
+            result.append(cmd_flag + ",".join(args))
+        return result
+
+    def __str__(self) -> str:
+        return str(self.flags())
+
+    def __add__(self, other: "FlagBuilder") -> "FlagBuilder":
+        if not isinstance(other, FlagBuilder):
+            raise TypeError(f"Ожидаемый тип: {self.__class__.__name__}; "
+                            f"полученный тип: {other.__class__.__name__}")
+
+        flags = {}
+        for cmd_flag, args in self._flags.items():
+            flags[cmd_flag] = args
+        for cmd_flag, args in other._flags.items():
+            flags[cmd_flag] = args
+
+        result = FlagBuilder()
+        setattr(result, "_flags", flags)
+        return result
 
 
 class CMDFlag(Enum): pass
 
 class CMDFlags:
     """https://github.com/GoogleChrome/chrome-launcher/blob/master/docs/chrome-flags-for-tools.md"""
 
@@ -613,14 +630,18 @@
         js_flags = "--js-flags="                # * $
         # ! Отключает шейдеры GPU в кеше на диске.
         disable_gpu_shader_disk_cache = "--disable-gpu-shader-disk-cache"
         # ! Принимает путь расположения кэша на диске, отличный от UserDatadir. Отключить: '--disk-cache-dir=null'
         disk_cache_dir = "--disk-cache-dir="    # * $
         # ! Задает максимальное дисковое пространство, используемое дисковым кешем, в байтах.
         disk_cache_size = "--disk-cache-size="  # * $
+        # ! Принимает путь расположения media-кэша на диске, отличный от UserDatadir. Отключить: '--media-cache-dir=null'
+        media_cache_dir = "--media-cache-dir="    # * $
+        # ! Задает максимальное дисковое пространство, используемое дисковым кешем для медиа, в байтах.
+        media_cache_size = "--media-cache-size="  # * $
 
     class Test(CMDFlag):
         # ? Test & debugging flags
         # ! Сообщает, выполняются ли в коде тесты браузера (это изменяет URL-адрес запуска, используемый оболочкой
         # !     содержимого, а также отключает функции, которые могут сделать тесты ненадежными [например, мониторинг
         # !     нехватки памяти]).
         browser_test = "--browser-test"
```

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/BrowserEx.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/BrowserEx.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/DOMElement.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/DOMElement.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/Data.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/Data.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/Page.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/Page.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/PageEx.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/PageEx.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/domains/BackgroundService.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/BackgroundService.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Browser.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Browser.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/domains/CSS.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/CSS.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Console.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Console.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/domains/DOM.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/DOM.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/domains/DeviceOrientation.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/DeviceOrientation.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Emulation.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Emulation.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Fetch.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Fetch.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Log.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Log.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Network.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Network.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Overlay.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Overlay.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Page.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Page.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Runtime.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Runtime.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/domains/SystemInfo.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/SystemInfo.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/domains/Target.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/domains/Target.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/exceptions.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol/utils.py` & `aio_dt_protocol-0.9.4/aio_dt_protocol/utils.py`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol.egg-info/PKG-INFO` & `aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-dt-protocol
-Version: 0.9.3
+Version: 0.9.4
 Summary: Asynchronous wrapper over Chromium browser debugger protocol.
 Home-page: https://github.com/PieceOfGood/aio_dt_protocol
 Author: PieceOfGood
 Author-email: 78sanchezz@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aio_dt_protocol-0.9.3/aio_dt_protocol.egg-info/SOURCES.txt` & `aio_dt_protocol-0.9.4/aio_dt_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aio_dt_protocol-0.9.3/setup.py` & `aio_dt_protocol-0.9.4/setup.py`

 * *Files identical despite different names*

