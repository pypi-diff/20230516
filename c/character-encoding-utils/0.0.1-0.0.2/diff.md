# Comparing `tmp/character-encoding-utils-0.0.1.tar.gz` & `tmp/character-encoding-utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "character-encoding-utils-0.0.1.tar", last modified: Tue May 16 05:06:23 2023, max compression
+gzip compressed data, was "character-encoding-utils-0.0.2.tar", last modified: Tue May 16 10:36:05 2023, max compression
```

## Comparing `character-encoding-utils-0.0.1.tar` & `character-encoding-utils-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:06:23.670114 character-encoding-utils-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-16 05:06:23.670114 character-encoding-utils-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 05:06:23.670114 character-encoding-utils-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:06:23.662114 character-encoding-utils-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:06:23.666113 character-encoding-utils-0.0.1/src/character_encoding_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/src/character_encoding_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/src/character_encoding_utils/big5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/src/character_encoding_utils/gb2312.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/src/character_encoding_utils/ksx1001.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/src/character_encoding_utils/shiftjis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:06:23.670114 character-encoding-utils-0.0.1/src/character_encoding_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-16 05:06:23.000000 character-encoding-utils-0.0.1/src/character_encoding_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-16 05:06:23.000000 character-encoding-utils-0.0.1/src/character_encoding_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 05:06:23.000000 character-encoding-utils-0.0.1/src/character_encoding_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 05:06:23.000000 character-encoding-utils-0.0.1/src/character_encoding_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:06:23.670114 character-encoding-utils-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/tests/test_big5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/tests/test_gb2312.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/tests/test_ksx1001.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-16 05:06:04.000000 character-encoding-utils-0.0.1/tests/test_shiftjis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:36:05.112311 character-encoding-utils-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-16 10:36:05.112311 character-encoding-utils-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:36:05.112311 character-encoding-utils-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:36:05.108311 character-encoding-utils-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:36:05.108311 character-encoding-utils-0.0.2/src/character_encoding_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/src/character_encoding_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/src/character_encoding_utils/big5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/src/character_encoding_utils/gb2312.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/src/character_encoding_utils/ksx1001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/src/character_encoding_utils/shiftjis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:36:05.108311 character-encoding-utils-0.0.2/src/character_encoding_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-16 10:36:05.000000 character-encoding-utils-0.0.2/src/character_encoding_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-16 10:36:05.000000 character-encoding-utils-0.0.2/src/character_encoding_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:36:05.000000 character-encoding-utils-0.0.2/src/character_encoding_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 10:36:05.000000 character-encoding-utils-0.0.2/src/character_encoding_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:36:05.112311 character-encoding-utils-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/tests/test_big5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/tests/test_gb2312.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/tests/test_ksx1001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/tests/test_shiftjis.py
```

### Comparing `character-encoding-utils-0.0.1/LICENSE` & `character-encoding-utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.1/PKG-INFO` & `character-encoding-utils-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: character-encoding-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Some character encoding utils.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/character-encoding-utils
 Project-URL: source, https://github.com/TakWolf/character-encoding-utils
 Project-URL: issues, https://github.com/TakWolf/character-encoding-utils/issues
```

### Comparing `character-encoding-utils-0.0.1/README.md` & `character-encoding-utils-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.1/pyproject.toml` & `character-encoding-utils-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "character-encoding-utils"
-version = "0.0.1"
+version = "0.0.2"
 description = "Some character encoding utils."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `character-encoding-utils-0.0.1/src/character_encoding_utils/big5.py` & `character-encoding-utils-0.0.2/src/character_encoding_utils/gb2312.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 
-class Big5Exception(Exception):
+_euc_offset = 0xA0
+
+
+class GB2312Exception(Exception):
     pass
 
 
-class Big5EncodeError(Big5Exception):
+class GB2312EncodeError(GB2312Exception):
     def __init__(self, obj: str, position: int, reason: str):
         self.object = obj
         self.position = position
         self.reason = reason
-        super().__init__(f"'big5' codec can't encode character '\\u{ord(obj):x}' in position {position}: {reason}")
+        super().__init__(f"'gb2312' codec can't encode character '\\u{ord(obj):x}' in position {position}: {reason}")
 
 
-class Big5DecodeError(Big5Exception):
+class GB2312DecodeError(GB2312Exception):
     def __init__(self, obj: bytes, position: int, reason: str):
         self.object = obj
         self.position = position
         self.reason = reason
-        super().__init__(f"'big5' codec can't decode byte 0x{obj[0]:x} in position {position}: {reason}")
+        super().__init__(f"'gb2312' codec can't decode byte 0x{obj[0]:x} in position {position}: {reason}")
 
 
 def encode(cs: str) -> bytes:
     bs = bytearray()
     for position, c in enumerate(cs):
-        # 此处默认编码器映射错误
-        if c == '〸':
-            bs.extend(b'\xa2\xcc')
-            continue
-        elif c == '〺':
-            bs.extend(b'\xa2\xce')
-            continue
         try:
-            bs.extend(c.encode('big5'))
+            bs.extend(c.encode('gb2312'))
         except UnicodeEncodeError as e:
-            raise Big5EncodeError(c, position, e.reason) from e
+            raise GB2312EncodeError(c, position, e.reason) from e
     return bytes(bs)
 
 
 def decode(bs: bytes) -> str:
     cs = []
     bs = iter(bs)
     position = -1
@@ -53,81 +49,78 @@
                 position += 1
             except StopIteration:
                 pass
         if b2 is None:
             bc = bytes([b1])
         else:
             bc = bytes([b1, b2])
-        # 此处默认编码器映射错误
-        if bc == b'\xa2\xcc':
-            cs.append('〸')
-            continue
-        elif bc == b'\xa2\xce':
-            cs.append('〺')
-            continue
         try:
-            cs.append(bc.decode('big5'))
+            cs.append(bc.decode('gb2312'))
         except UnicodeDecodeError as e:
-            raise Big5DecodeError(bc, position, e.reason) from e
+            raise GB2312DecodeError(bc, position, e.reason) from e
     return ''.join(cs)
 
 
-def query_code(c: str) -> int:
+def query_coord(c: str) -> tuple[int, int]:
     if len(c) != 1:
-        raise Big5Exception('must be one character')
+        raise GB2312Exception('must be one character')
     try:
         bs = encode(c)
-    except Big5EncodeError as e:
-        raise Big5Exception(f"'{c}' is not a 'big5' character") from e
+    except GB2312EncodeError as e:
+        raise GB2312Exception(f"'{c}' is not a 'gb2312' character") from e
     if len(bs) == 1:
-        raise Big5Exception(f"'{c}' is a ascii character")
-    code = int(f'{bs[0]:02x}{bs[1]:02x}', 16)
-    return code
+        raise GB2312Exception(f"'{c}' is a ascii character")
+    row = bs[0] - _euc_offset
+    col = bs[1] - _euc_offset
+    return row, col
 
 
-def query_chr(code: int) -> str:
+def query_chr(row: int, col: int) -> str:
+    if row < 1 or row > 94 or col < 1 or col > 94:
+        raise GB2312Exception(f"'row' and 'col' must between 1 and 94")
     try:
-        return decode(bytes.fromhex(f'{code:X}'))
-    except Big5DecodeError as e:
-        raise Big5Exception(f"'big5' code 0x{code:04X} is undefined") from e
+        return decode(bytes([row + _euc_offset, col + _euc_offset]))
+    except GB2312DecodeError as e:
+        raise GB2312Exception(f"'gb2312' coord at ({row}, {col}) is undefined'") from e
 
 
 def get_categories() -> list[str]:
     return ['other', 'level-1', 'level-2']
 
 
 def query_category(c: str) -> str | None:
     try:
-        code = query_code(c)
-    except Big5Exception:
+        row = query_coord(c)[0]
+    except GB2312Exception:
         return None
-    if 0xA140 <= code <= 0xA3BF:
+    if 1 <= row <= 9:
         return 'other'
-    elif 0xA440 <= code <= 0xC67E:
+    elif 16 <= row <= 55:
         return 'level-1'
-    elif 0xC940 <= code <= 0xF9D5:
+    elif 56 <= row <= 87:
         return 'level-2'
     else:
-        return None
+        raise None
 
 
-def _build_alphabet_by_codes_between(code_start: int, code_end: int) -> list[str]:
+def _build_alphabet_by_rows_between(row_start: int, row_end: int) -> list[str]:
     alphabet = []
-    for code in range(code_start, code_end + 1):
-        try:
-            c = query_chr(code)
-            alphabet.append(c)
-        except Big5Exception:
-            pass
+    for row in range(row_start, row_end + 1):
+        for col in range(1, 94 + 1):
+            try:
+                c = query_chr(row, col)
+                alphabet.append(c)
+            except GB2312Exception:
+                pass
     return alphabet
 
 
-_alphabet_other = _build_alphabet_by_codes_between(0xA140, 0xA3BF)
-_alphabet_level_1 = _build_alphabet_by_codes_between(0xA440, 0xC67E)
-_alphabet_level_2 = _build_alphabet_by_codes_between(0xC940, 0xF9D5)
+_alphabet_other = _build_alphabet_by_rows_between(1, 9)
+_alphabet_level_1 = _build_alphabet_by_rows_between(16, 55)
+_alphabet_level_2 = _build_alphabet_by_rows_between(56, 87)
 _alphabet = _alphabet_other + _alphabet_level_1 + _alphabet_level_2
 
 
 def get_alphabet_other() -> list[str]:
     return list(_alphabet_other)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `character-encoding-utils-0.0.1/src/character_encoding_utils/gb2312.py` & `character-encoding-utils-0.0.2/src/character_encoding_utils/big5.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,55 @@
 
-_euc_offset = 0xA0
-
-
-class GB2312Exception(Exception):
+class Big5Exception(Exception):
     pass
 
 
-class GB2312EncodeError(GB2312Exception):
+class Big5EncodeError(Big5Exception):
     def __init__(self, obj: str, position: int, reason: str):
         self.object = obj
         self.position = position
         self.reason = reason
-        super().__init__(f"'gb2312' codec can't encode character '\\u{ord(obj):x}' in position {position}: {reason}")
+        super().__init__(f"'big5' codec can't encode character '\\u{ord(obj):x}' in position {position}: {reason}")
 
 
-class GB2312DecodeError(GB2312Exception):
+class Big5DecodeError(Big5Exception):
     def __init__(self, obj: bytes, position: int, reason: str):
         self.object = obj
         self.position = position
         self.reason = reason
-        super().__init__(f"'gb2312' codec can't decode byte 0x{obj[0]:x} in position {position}: {reason}")
+        super().__init__(f"'big5' codec can't decode byte 0x{obj[0]:x} in position {position}: {reason}")
 
 
 def encode(cs: str) -> bytes:
     bs = bytearray()
     for position, c in enumerate(cs):
+        # 此处默认编码器映射错误
+        if c == '〸':  # 0x3038
+            bs.extend(b'\xa2\xcc')
+            continue
+        elif c == '〹':  # 0x3039
+            bs.extend(b'\xa2\xcd')
+            continue
+        elif c == '〺':  # 0x303A
+            bs.extend(b'\xa2\xce')
+            continue
+        elif c == '十':  # 0x5341
+            bs.extend(b'\xa4\x51')
+            continue
+        elif c == '卄':  # 0x5344
+            # Big5 不包含汉字的 '卄'
+            raise Big5EncodeError(c, position, 'illegal multibyte sequence')
+        elif c == '卅':  # 0x5345
+            bs.extend(b'\xa4\xca')
+            continue
+
         try:
-            bs.extend(c.encode('gb2312'))
+            bs.extend(c.encode('big5'))
         except UnicodeEncodeError as e:
-            raise GB2312EncodeError(c, position, e.reason) from e
+            raise Big5EncodeError(c, position, e.reason) from e
     return bytes(bs)
 
 
 def decode(bs: bytes) -> str:
     cs = []
     bs = iter(bs)
     position = -1
@@ -49,78 +66,92 @@
                 position += 1
             except StopIteration:
                 pass
         if b2 is None:
             bc = bytes([b1])
         else:
             bc = bytes([b1, b2])
+
+        # 此处默认编码器映射错误
+        if bc == b'\xa2\xcc':
+            cs.append('〸')  # 0x3038
+            continue
+        elif bc == b'\xa2\xcd':
+            cs.append('〹')  # 0x3039
+            continue
+        elif bc == b'\xa2\xce':
+            cs.append('〺')  # 0x303A
+            continue
+        elif bc == b'\xa4\x51':
+            cs.append('十')  # 0x5341
+            continue
+        elif bc == b'\xa4\xca':
+            cs.append('卅')  # 0x5345
+            continue
+
         try:
-            cs.append(bc.decode('gb2312'))
+            cs.append(bc.decode('big5'))
         except UnicodeDecodeError as e:
-            raise GB2312DecodeError(bc, position, e.reason) from e
+            raise Big5DecodeError(bc, position, e.reason) from e
     return ''.join(cs)
 
 
-def query_coord(c: str) -> tuple[int, int]:
+def query_code(c: str) -> int:
     if len(c) != 1:
-        raise GB2312Exception('must be one character')
+        raise Big5Exception('must be one character')
     try:
         bs = encode(c)
-    except GB2312EncodeError as e:
-        raise GB2312Exception(f"'{c}' is not a 'gb2312' character") from e
+    except Big5EncodeError as e:
+        raise Big5Exception(f"'{c}' is not a 'big5' character") from e
     if len(bs) == 1:
-        raise GB2312Exception(f"'{c}' is a ascii character")
-    row = bs[0] - _euc_offset
-    col = bs[1] - _euc_offset
-    return row, col
+        raise Big5Exception(f"'{c}' is a ascii character")
+    code = int(f'{bs[0]:02x}{bs[1]:02x}', 16)
+    return code
 
 
-def query_chr(row: int, col: int) -> str:
-    if row < 1 or row > 94 or col < 1 or col > 94:
-        raise GB2312Exception(f"'row' and 'col' must between 1 and 94")
+def query_chr(code: int) -> str:
     try:
-        return decode(bytes([row + _euc_offset, col + _euc_offset]))
-    except GB2312DecodeError as e:
-        raise GB2312Exception(f"'gb2312' coord at ({row}, {col}) is undefined'") from e
+        return decode(bytes.fromhex(f'{code:X}'))
+    except Big5DecodeError as e:
+        raise Big5Exception(f"'big5' code 0x{code:04X} is undefined") from e
 
 
 def get_categories() -> list[str]:
     return ['other', 'level-1', 'level-2']
 
 
 def query_category(c: str) -> str | None:
     try:
-        row = query_coord(c)[0]
-    except GB2312Exception:
+        code = query_code(c)
+    except Big5Exception:
         return None
-    if 1 <= row <= 9:
+    if 0xA140 <= code <= 0xA3BF:
         return 'other'
-    elif 16 <= row <= 55:
+    elif 0xA440 <= code <= 0xC67E:
         return 'level-1'
-    elif 56 <= row <= 87:
+    elif 0xC940 <= code <= 0xF9D5:
         return 'level-2'
     else:
-        raise None
+        return None
 
 
-def _build_alphabet_by_rows_between(row_start: int, row_end: int) -> list[str]:
+def _build_alphabet_by_codes_between(code_start: int, code_end: int) -> list[str]:
     alphabet = []
-    for row in range(row_start, row_end + 1):
-        for col in range(1, 94 + 1):
-            try:
-                c = query_chr(row, col)
-                alphabet.append(c)
-            except GB2312Exception:
-                pass
+    for code in range(code_start, code_end + 1):
+        try:
+            c = query_chr(code)
+            alphabet.append(c)
+        except Big5Exception:
+            pass
     return alphabet
 
 
-_alphabet_other = _build_alphabet_by_rows_between(1, 9)
-_alphabet_level_1 = _build_alphabet_by_rows_between(16, 55)
-_alphabet_level_2 = _build_alphabet_by_rows_between(56, 87)
+_alphabet_other = _build_alphabet_by_codes_between(0xA140, 0xA3BF)
+_alphabet_level_1 = _build_alphabet_by_codes_between(0xA440, 0xC67E)
+_alphabet_level_2 = _build_alphabet_by_codes_between(0xC940, 0xF9D5)
 _alphabet = _alphabet_other + _alphabet_level_1 + _alphabet_level_2
 
 
 def get_alphabet_other() -> list[str]:
     return list(_alphabet_other)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `character-encoding-utils-0.0.1/src/character_encoding_utils/ksx1001.py` & `character-encoding-utils-0.0.2/src/character_encoding_utils/ksx1001.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,19 +49,21 @@
                 position += 1
             except StopIteration:
                 pass
         if b2 is None:
             bc = bytes([b1])
         else:
             bc = bytes([b1, b2])
+
         # 'euc_kr' 编码器对字符 'Hangul Filler (0x3164, row = 4, col= 52)' 的处理不正确，但是官方开发者并不认为这是一个错误
         # 问题详情见： https://github.com/python/cpython/issues/101863
         if bc == b'\xa4\xd4':
             cs.append(chr(0x3164))
             continue
+
         try:
             cs.append(bc.decode('ksx1001'))
         except UnicodeDecodeError as e:
             raise KSX1001DecodeError(bc, position, e.reason) from e
     return ''.join(cs)
```

### Comparing `character-encoding-utils-0.0.1/src/character_encoding_utils/shiftjis.py` & `character-encoding-utils-0.0.2/src/character_encoding_utils/shiftjis.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,19 @@
         self.reason = reason
         super().__init__(f"'shift-jis' codec can't decode byte 0x{obj[0]:x} in position {position}: {reason}")
 
 
 def encode(cs: str) -> bytes:
     bs = bytearray()
     for position, c in enumerate(cs):
+        if c == '\\':
+            raise ShiftJISEncodeError(c, position, f"in 'shift-jis' the character '\\' is replaced with '¥'")
+        elif c == '~':
+            raise ShiftJISEncodeError(c, position, f"in 'shift-jis' the character '~' is replaced with '‾'")
+
         try:
             bs.extend(c.encode('shift-jis'))
         except UnicodeEncodeError as e:
             raise ShiftJISEncodeError(c, position, e.reason) from e
     return bytes(bs)
 
 
@@ -48,14 +53,22 @@
                 position += 1
             except StopIteration:
                 pass
         if b2 is None:
             bc = bytes([b1])
         else:
             bc = bytes([b1, b2])
+
+        if bc == b'\\':
+            cs.append('¥')
+            continue
+        elif bc == b'~':
+            cs.append('‾')
+            continue
+
         try:
             cs.append(bc.decode('shift-jis'))
         except UnicodeDecodeError as e:
             raise ShiftJISDecodeError(bc, position, e.reason) from e
     return ''.join(cs)
```

### Comparing `character-encoding-utils-0.0.1/src/character_encoding_utils.egg-info/PKG-INFO` & `character-encoding-utils-0.0.2/src/character_encoding_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: character-encoding-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Some character encoding utils.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/character-encoding-utils
 Project-URL: source, https://github.com/TakWolf/character-encoding-utils
 Project-URL: issues, https://github.com/TakWolf/character-encoding-utils/issues
```

### Comparing `character-encoding-utils-0.0.1/src/character_encoding_utils.egg-info/SOURCES.txt` & `character-encoding-utils-0.0.2/src/character_encoding_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.1/tests/test_big5.py` & `character-encoding-utils-0.0.2/tests/test_big5.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,39 @@
 
     with pytest.raises(Big5DecodeError) as info:
         big5.decode(b'abc\xa4\xa4\xb0')
     assert info.value.object == b'\xb0'
     assert info.value.position == 5
     assert info.value.reason == 'incomplete multibyte sequence'
 
+    c = '〸'
+    assert ord(c) == 0x3038
+    assert big5.decode(big5.encode(c)) == c
+
+    c = '〹'
+    assert ord(c) == 0x3039
+    assert big5.decode(big5.encode(c)) == c
+
+    c = '〺'
+    assert ord(c) == 0x303A
+    assert big5.decode(big5.encode(c)) == c
+
+    c = '十'
+    assert ord(c) == 0x5341
+    assert big5.decode(big5.encode(c)) == c
+
+    c = '卄'
+    assert ord(c) == 0x5344
+    with pytest.raises(Big5EncodeError):
+        big5.encode(c)
+
+    c = '卅'
+    assert ord(c) == 0x5345
+    assert big5.decode(big5.encode(c)) == c
+
 
 def test_query_code():
     assert big5.query_code('　') == 0xA140
     assert big5.query_code('¢') == 0xA246
     assert big5.query_code('一') == 0xA440
     assert big5.query_code('訐') == 0xB050
     assert big5.query_code('乂') == 0xC940
```

### Comparing `character-encoding-utils-0.0.1/tests/test_gb2312.py` & `character-encoding-utils-0.0.2/tests/test_gb2312.py`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.1/tests/test_ksx1001.py` & `character-encoding-utils-0.0.2/tests/test_ksx1001.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
     with pytest.raises(KSX1001DecodeError) as info:
         ksx1001.decode(b'abc\xb0\xa1\xc3')
     assert info.value.object == b'\xc3'
     assert info.value.position == 5
     assert info.value.reason == 'incomplete multibyte sequence'
 
+    assert ksx1001.decode(ksx1001.encode(chr(0x3164))) == chr(0x3164)
+
 
 def test_query_coord():
     assert ksx1001.query_coord('ㆌ') == (4, 92)
     assert ksx1001.query_coord('φ') == (5, 85)
     assert ksx1001.query_coord('떰') == (22, 22)
     assert ksx1001.query_coord('틘') == (38, 24)
     assert ksx1001.query_coord('紺') == (42, 90)
```

### Comparing `character-encoding-utils-0.0.1/tests/test_shiftjis.py` & `character-encoding-utils-0.0.2/tests/test_shiftjis.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,31 @@
 
     with pytest.raises(ShiftJISDecodeError) as info:
         shiftjis.decode(b'abc\x93\xfa\x96')
     assert info.value.object == b'\x96'
     assert info.value.position == 5
     assert info.value.reason == 'incomplete multibyte sequence'
 
+    with pytest.raises(ShiftJISEncodeError) as info:
+        shiftjis.encode('\\')
+    assert info.value.object == '\\'
+    assert info.value.position == 0
+    assert '\\' in info.value.reason
+    assert '¥' in info.value.reason
+
+    with pytest.raises(ShiftJISEncodeError) as info:
+        shiftjis.encode('~')
+    assert info.value.object == '~'
+    assert info.value.position == 0
+    assert '~' in info.value.reason
+    assert '‾' in info.value.reason
+
+    assert shiftjis.decode(shiftjis.encode('¥')) == '¥'
+    assert shiftjis.decode(shiftjis.encode('‾')) == '‾'
+
 
 def test_query_category():
     categories = shiftjis.get_categories()
     assert len(categories) == 5
     assert 'single-byte-ascii-control' in categories
     assert 'single-byte-ascii-printable' in categories
     assert 'single-byte-half-width-katakana' in categories
```

