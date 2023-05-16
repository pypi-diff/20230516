# Comparing `tmp/phable-0.1.6.tar.gz` & `tmp/phable-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phable-0.1.6.tar", max compression
+gzip compressed data, was "phable-0.1.7.tar", max compression
```

## Comparing `phable-0.1.6.tar` & `phable-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-03-18 20:20:49.329618 phable-0.1.6/LICENSE
--rw-r--r--   0        0        0     2685 2023-04-26 19:55:25.085338 phable-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-03-18 18:42:50.546791 phable-0.1.6/phable/__init__.py
--rw-r--r--   0        0        0     3113 2023-04-26 19:54:55.255634 phable-0.1.6/phable/http.py
--rw-r--r--   0        0        0     5896 2023-04-30 19:19:25.687621 phable-0.1.6/phable/json_parser.py
--rw-r--r--   0        0        0     3266 2023-04-25 15:37:14.607396 phable-0.1.6/phable/kinds.py
--rw-r--r--   0        0        0     3251 2023-04-30 19:48:57.508637 phable-0.1.6/phable/phable.py
--rw-r--r--   0        0        0    16673 2023-04-30 17:57:04.940932 phable-0.1.6/phable/scram.py
--rw-r--r--   0        0        0      721 2023-04-30 22:19:16.782060 phable-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 phable-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-18 20:20:49.329618 phable-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1208 2023-05-16 00:55:42.481814 phable-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-03-18 18:42:50.546791 phable-0.1.7/phable/__init__.py
+-rw-r--r--   0        0        0     3135 2023-05-07 00:57:47.871901 phable-0.1.7/phable/http.py
+-rw-r--r--   0        0        0     8540 2023-05-15 15:18:43.774165 phable-0.1.7/phable/json_parser.py
+-rw-r--r--   0        0        0     3188 2023-05-15 15:14:57.155754 phable-0.1.7/phable/kinds.py
+-rw-r--r--   0        0        0     4242 2023-05-16 00:48:45.882638 phable-0.1.7/phable/phable.py
+-rw-r--r--   0        0        0    15105 2023-05-15 15:11:51.287039 phable-0.1.7/phable/scram.py
+-rw-r--r--   0        0        0      721 2023-05-16 00:57:02.754083 phable-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 phable-0.1.7/PKG-INFO
```

### Comparing `phable-0.1.6/LICENSE` & `phable-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `phable-0.1.6/phable/http.py` & `phable-0.1.7/phable/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         Decode body's JSON.
         Returns:
             Pythonic representation of the JSON object
         """
         try:
             output = json.loads(self.body)
         except json.JSONDecodeError:
-            output = ""
+            output = {}  # Previously was: ""
         return output
 
 
 def request(
     url: str,
     data: Optional[dict[str, Any]] = None,
     params: Optional[dict[str, Any]] = None,
```

### Comparing `phable-0.1.6/phable/kinds.py` & `phable-0.1.7/phable/kinds.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,30 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import date, datetime, time
 from typing import Any, Optional
 
-# from phable.json_parser import parse_kinds
-
 
 @dataclass(frozen=True, slots=True)
 class Grid:
     meta: dict[str, Any]
     cols: list[dict[str, Any]]
     rows: list[dict[str, Any]]
 
-    # @staticmethod
-    # def dict_to_grid(d: dict[str, Any]) -> Grid:
-    #     rows = [d]
-    #     cols = [{"name": name} for name in rows[0].keys()]
-    #     meta = {"ver": "3.0"}
-    #     return Grid(meta=meta, cols=cols, rows=rows)
-
     @staticmethod
     def to_grid(rows: dict[str, Any] | list[dict[str, Any]]) -> Grid:
         if isinstance(rows, dict):
             rows = [rows]
 
         cols = [{"name": name} for name in rows[0].keys()]
         meta = {"ver": "3.0"}
 
         return Grid(meta=meta, cols=cols, rows=rows)
 
-    # @staticmethod
-    # def json_to_grid(d: dict[str, Any]) -> Grid:
-    #     parse_kinds(d)
-    #     return Grid(meta=d["meta"], cols=d["cols"], rows=d["rows"])
-
     def to_json(self: Grid) -> dict[str, Any]:
         return {
             "_kind": "grid",
             "meta": self.meta,
             "cols": self.cols,
             "rows": self.rows,
         }
@@ -89,46 +75,62 @@
         return NA.__instance
 
     def __repr__(self):
         return "NA"
 
 
 # TODO: Determine if I need make_handle func on Ref()
+# TODO:  Should dis in Ref be mandatory?
 @dataclass(frozen=True, slots=True)
 class Ref:
     val: str
     dis: Optional[str] = None
 
+    def __repr__(self) -> str:
+        return self.dis
+
 
 @dataclass(frozen=True, slots=True)
 class Date:
     val: date
 
+    def __repr__(self):
+        return self.val.isoformat()
+
 
 @dataclass(frozen=True, slots=True)
 class Time:
     val: time
 
+    # def __repr__(self):
+    #     return time.strftime(self.val, "%H:%M:%S%p")
+
+    def __repr__(self):
+        return self.val.isoformat()
+
 
 # TODO:
 # - See if we can expose a nicer time zone display to end user
 # - Map Haystack tz to IANA time zone database tz
 # https://docs.python.org/3/library/zoneinfo.html#zoneinfo.ZoneInfo.key
 @dataclass(frozen=True, slots=True)
 class DateTime:
     """
     Note:  tz attribute is the just the city name from the IANA database according to
     Haystack.
     """
 
     val: datetime
-    tz: str
+    tz: Optional[str]
+
+    # def __repr__(self):
+    #     return datetime.strftime(self.val, "%d-%b-%Y %a %H:%M:%S%p %Z")
 
     def __repr__(self):
-        return datetime.strftime(self.val, "%d-%b-%Y %a %H:%M:%S%p %Z")
+        return self.val.isoformat()
 
 
 @dataclass(frozen=True, slots=True)
 class Uri:
     val: str
```

### Comparing `phable-0.1.6/phable/scram.py` & `phable-0.1.7/phable/scram.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,42 +13,15 @@
 from phable.http import request
 
 from .http import Response
 
 logger = logging.getLogger(__name__)
 
 
-# -----------------------------------------------------------------------
-#
-# -----------------------------------------------------------------------
-
-
-def get_auth_token(host_url: str, username: str, password: str):
-    sc = ScramClient(username, password)
-
-    # send hello msg & set the response
-    hello_resp = request(host_url, headers=sc.get_hello_req())
-    # logger.critical(f"Here are the headers from the hello resp:\n{hello_resp.headers}")
-    sc.set_hello_resp(hello_resp)
-
-    # send first msg & set the response
-    first_resp = request(host_url, headers=sc.get_first_req())
-    sc.set_first_resp(first_resp)
-
-    # send last msg & set the response
-    last_resp = request(host_url, headers=sc.get_last_req())
-    sc.set_last_resp(last_resp)
-
-    # return the auth token
-    return sc.auth_token
-
-
-# -----------------------------------------------------------------------
-# define exceptions
-# -----------------------------------------------------------------------
+# TODO: Check the validity of the server final message
 
 
 class ScramException(Exception):
     def __init__(self, message: str, server_error: Optional[str] = None):
         super().__init__(message)
         self.server_error = server_error
 
@@ -58,143 +31,142 @@
 
 
 @dataclass
 class NotFoundError(Exception):
     help_msg: str
 
 
-# -----------------------------------------------------------------------
-# define the ScramClient
-# -----------------------------------------------------------------------
-
-
 class ScramClient:
-    def __init__(self, username: str, password: str, hash: str = "sha256"):
+    def __init__(
+        self, host_url: str, username: str, password: str, hash: str = "sha256"
+    ):
         if hash not in ["sha256"]:
             raise ScramException(
                 "The 'hash' parameter must be a str equal to 'sha256'."
             )
 
+        self.host_url = host_url
         self._username = username
         self._password = password
+        self.auth_token = self._get_auth_token()
         self._hash = hash
 
-    def get_hello_req(self) -> dict[str, str]:
+    def _get_auth_token(self):
+        host_url = self.host_url
+
+        # send hello msg & set the response
+        hello_resp = request(host_url, headers=self._get_hello_req())
+        self._set_hello_resp(hello_resp)
+
+        # send first msg & set the response
+        first_resp = request(host_url, headers=self._get_first_req())
+        self._set_first_resp(first_resp)
+
+        # send last msg & receive the response
+        last_resp = request(host_url, headers=self._get_last_req())
+
+        # parse the auth token from the last response
+        auth_token = _parse_auth_token(last_resp.headers.as_string())
+
+        return auth_token
+
+    def _get_hello_req(self) -> dict[str, str]:
         """
         Return the HTTP headers required for the client's hello message.
 
         Note:  There is no data required for the client's hello message.
         """
-        username = to_base64(self._username)
+        username = _to_base64(self._username)
         headers = {"Authorization": f"HELLO username={username}"}
         return headers
 
-    def set_hello_resp(self, resp: Response) -> None:
+    def _set_hello_resp(self, resp: Response) -> None:
         """
         Save server's response data as class attributes to be able to get other
         request messages.
         """
         auth_header = resp.headers["WWW-Authenticate"]
-        self.handshake_token = parse_handshake_token(auth_header)
-        self._hash = parse_hash_func(auth_header)
+        self.handshake_token = _parse_handshake_token(auth_header)
+        self._hash = _parse_hash_func(auth_header)
 
-    def get_first_req(self) -> dict[str, str]:
+    def _get_first_req(self) -> dict[str, str]:
         gs2_header = "n,,"
 
-        self.c_nonce: str = gen_nonce()
-        self.c1_bare: str = f"n={self._username},r={self.c_nonce}"
+        self._c_nonce: str = _gen_nonce()
+        self._c1_bare: str = f"n={self._username},r={self._c_nonce}"
 
         headers = {
             "Authorization": f"scram handshakeToken={self.handshake_token}, "
-            f"hash={self._hash}, data={to_base64(gs2_header+self.c1_bare)}"
+            f"hash={self._hash}, data={_to_base64(gs2_header+self._c1_bare)}"
         }
         return headers
 
-    def set_first_resp(self, resp: Response) -> None:
+    def _set_first_resp(self, resp: Response) -> None:
         auth_header = resp.headers["WWW-Authenticate"]
-        r, s, i = parse_scram_data(auth_header)
-        self.s_nonce: str = r
-        self.salt: str = s
-        self.iter_count: int = i
+        r, s, i = _parse_scram_data(auth_header)
+        self._s_nonce: str = r
+        self._salt: str = s
+        self._iter_count: int = i
 
-    def get_last_req(self):
+    def _get_last_req(self):
         # define the client final no proof
-        client_final_no_proof = f"c={to_base64('n,,')},r={self.s_nonce}"
-        # logger.debug(f"client-final-no-proof:\n{client_final_no_proof}\n")
+        client_final_no_proof = f"c={_to_base64('n,,')},r={self._s_nonce}"
 
         # define the auth msg
         auth_msg = (
-            f"{self.c1_bare},r={self.s_nonce},s={self.salt},"
-            + f"i={self.iter_count},{client_final_no_proof}"
+            f"{self._c1_bare},r={self._s_nonce},s={self._salt},"
+            + f"i={self._iter_count},{client_final_no_proof}"
         )
-        # logger.debug(f"auth-msg:\n{auth_msg}\n")
 
         # define the client key
         client_key = hmac.new(
             unhexlify(
-                salted_password(
-                    self.salt,
-                    self.iter_count,
+                _salted_password(
+                    self._salt,
+                    self._iter_count,
                     self._hash,
                     self._password,
                 )
             ),
             "Client Key".encode("UTF-8"),
             self._hash,
         ).hexdigest()
-        # logger.debug(f"client-key:\n{client_key}\n")
 
         # find the stored key
         hashFunc = hashlib.new(self._hash)
         hashFunc.update(unhexlify(client_key))
         stored_key = hashFunc.hexdigest()
-        # logger.debug(f"stored-key:\n{stored_key}\n")
 
         # find the client signature
         client_signature = hmac.new(
             unhexlify(stored_key), auth_msg.encode("utf-8"), self._hash
         ).hexdigest()
-        # logger.debug(f"client-signature:\n{client_signature}\n")
 
         # find the client proof
         client_proof = hex(int(client_key, 16) ^ int(client_signature, 16))[2:]
-        # logger.debug(f"Here is the length of the client proof: {len(client_proof)}")
 
         # may need to do some padding before converting the hex to its
         # binary representation
         while len(client_proof) < 64:
             client_proof = "0" + client_proof
 
-        client_proof_encode = to_base64(unhexlify(client_proof))
-        # logger.debug(f"client-proof:\n{client_proof}\n")
+        client_proof_encode = _to_base64(unhexlify(client_proof))
 
         client_final = client_final_no_proof + ",p=" + client_proof_encode
-        client_final_base64 = to_base64(client_final)
+        client_final_base64 = _to_base64(client_final)
 
         final_msg = (
             f"scram handshaketoken={self.handshake_token},data={client_final_base64}"
         )
-        # logger.debug(f"Here is the final msg being sent: {final_msg}")
 
         headers = {"Authorization": final_msg}
         return headers
 
-    def set_last_resp(self, resp: Response) -> None:
-        self.auth_token = parse_auth_token(resp.headers.as_string())
-
-
-# -
-# define helper funcs used in ScramClient
-# -
-
-
-# TODO: Consider introducing a NamedTuple instead of a tuple
-
 
-def parse_scram_data(auth_header: str) -> tuple[str, str, int]:
+def _parse_scram_data(auth_header: str) -> tuple[str, str, int]:
     """Parses and decodes scram data from the contents of a 'WWW-Authenticate' header.
 
     Args:
         auth_header (str): Contents of the 'WWW-Authenticate' header in the HTTP
         response received from the server.  Search 'WWW-Authenticate' in the Project
         Haystack docs for more details.
 
@@ -230,15 +202,15 @@
     scram_data = re.search(f"({exclude_msg})[a-zA-Z0-9]+", auth_header)
 
     if scram_data is None:
         raise NotFoundError(
             f"Scram data not found in the 'WWW-Authenticate' header:\n{auth_header}"
         )
 
-    decoded_scram_data = from_base64(scram_data.group(0)[len(exclude_msg) :])
+    decoded_scram_data = _from_base64(scram_data.group(0)[len(exclude_msg) :])
     s_nonce, salt, iteration_count = decoded_scram_data.replace(" ", "").split(",")
 
     if "r=" not in s_nonce:
         raise NotFoundError(
             f"Server nonce not found in the 'WWW-Authenticate' header:\n{auth_header}"
         )
     elif "s=" not in salt:
@@ -256,15 +228,15 @@
     return (
         s_nonce.replace("r=", ""),
         salt.replace("s=", ""),
         int(iteration_count.replace("i=", "")),
     )
 
 
-def parse_handshake_token(auth_header: str) -> str:
+def _parse_handshake_token(auth_header: str) -> str:
     """Parses the handshake token from the contents of a 'WWW-Authenticate' header.
 
     Args:
         auth_header (str): Contents of the 'WWW-Authenticate' header in the HTTP
         response received from the server.  Search 'WWW-Authenticate' in the Project
         Haystack docs for more details.
 
@@ -302,15 +274,15 @@
                 + f"\n{auth_header}"
             )
         )
 
     return s.group(0)[len(exclude_msg) :]
 
 
-def parse_hash_func(auth_header: str) -> str:
+def _parse_hash_func(auth_header: str) -> str:
     """Parses the hash function from the contents of a 'WWW-Authenticate' header.
 
     Args:
         auth_header (str): Contents of the 'WWW-Authenticate' header in the HTTP
         response received from the server.  Search 'WWW-Authenticate' in the Project
         Haystack docs for more details.
 
@@ -350,15 +322,15 @@
 
     if s_new == "SHA-256":
         s_new = "sha256"
 
     return s_new
 
 
-def parse_auth_token(auth_header: str) -> str:
+def _parse_auth_token(auth_header: str) -> str:
     """Parses the auth token from the contents of a 'WWW-Authenticate' header.
 
     Args:
         auth_header (str): Contents of the 'WWW-Authenticate' header in the HTTP
         response received from the server.  Search 'WWW-Authenticate' in the Project
         Haystack docs for more details.
 
@@ -391,20 +363,15 @@
         raise NotFoundError(
             f"Auth token not found in the 'WWW-Authenticate' header:\n{auth_header}"
         )
 
     return s.group(0)[len(exclude_msg) :]
 
 
-# --------------------------------------------------------------------
-# Nonce & related helper funcs
-# --------------------------------------------------------------------
-
-
-def to_custom_hex(x: int, length: int) -> str:
+def _to_custom_hex(x: int, length: int) -> str:
     """
     Convert an integer x to hexadecimal string representation without a
     prepended '0x' str.  Prepend leading zeros as needed to ensure the
     specified number of nibble characters.
     """
 
     # Convert x to a hexadecimal number
@@ -416,58 +383,50 @@
     # Prepend 0s as needed
     if len(x_hex) < length:
         x_hex = "0" * (length - len(x_hex)) + x_hex
 
     return x_hex
 
 
-def gen_nonce() -> str:
+def _gen_nonce() -> str:
     """Generate a nonce."""
     # Notes:
     #   getrandbits() defines a random 64 bit integer
     #   time_ns() defines ticks since the Unix epoch (1 January 1970)
 
     # Define nonce random mask for this VM
     nonce_mask: int = getrandbits(64)
 
     rand = getrandbits(64)
     ticks = time_ns() ^ nonce_mask ^ rand
-    return to_custom_hex(rand, 16) + to_custom_hex(ticks, 16)
-
+    return _to_custom_hex(rand, 16) + _to_custom_hex(ticks, 16)
 
-# --------------------------------------------------------------------
-# Misc
-# --------------------------------------------------------------------
 
-
-def salted_password(salt: str, iterations: int, hash_func: str, password: str) -> bytes:
+def _salted_password(
+    salt: str, iterations: int, hash_func: str, password: str
+) -> bytes:
     # Need hash_func to be a str here
     dk = pbkdf2_hmac(hash_func, password.encode(), urlsafe_b64decode(salt), iterations)
     encrypt_password = hexlify(dk)
     return encrypt_password
 
 
-# --------------------------------------------------------------------
-# Base64uri conversions & related helper funcs
-# --------------------------------------------------------------------
-
-
-def to_base64(msg: str | bytes) -> str:
+def _to_base64(msg: str | bytes) -> str:
     """Perform base64uri encoding of a message as defined by RFC 4648.
 
     Args:
         msg (str | bytes): A message to be encoded.
 
     Returns:
         str: A base64uri encoded message
 
     Examples:
-        >>> to_base64("example")
+        >>> _to_base64("example")
         'ZXhhbXBsZQ'
-        >>> to_base64(bytes("example", "utf-8"))
+        >>> _to_base64(bytes("example", "utf-8"))
         'ZXhhbXBsZQ'
     """
 
     # Convert str inputs to bytes
     if isinstance(msg, str):
         msg = msg.encode("utf-8")
 
@@ -480,57 +439,57 @@
 
     # Remove padding
     output = output.replace("=", "")
 
     return output
 
 
-def from_base64(msg: str) -> str:
+def _from_base64(msg: str) -> str:
     """Decode a base64uri encoded message defined by RFC 4648 into
     its binary contents. Decode a URI-safe RFC 4648 encoding.
 
     Args:
         msg (str): A base64uri message to be decoded.
 
     Returns:
         str: A decoded message
 
     Example:
-        >>> from_base64("ZXhhbXBsZQ")
+        >>> _from_base64("ZXhhbXBsZQ")
         'example'
     """
 
     # Decode base64uri
-    decoded_msg = urlsafe_b64decode(to_bytes(msg))
+    decoded_msg = urlsafe_b64decode(_to_bytes(msg))
 
     # Decode bytes obj as a str
     return decoded_msg.decode("utf-8")
 
 
-def to_bytes(s: str) -> bytes:
+def _to_bytes(s: str) -> bytes:
     """Convert a string to a bytes object.
 
     Prior to conversion to bytes the string object must have a length that is a
     multiple of 4.  If applicable, padding will be applied to extend the length
     of the string input.
 
     Args:
         s (str): A string object.
 
     Returns:
         bytes: A bytes object.
 
     Examples:
-        >>> to_bytes("abcd")
+        >>> _to_bytes("abcd")
         b'abcd'
-        >>> to_bytes("abcde")
+        >>> _to_bytes("abcde")
         b'abcde==='
-        >>> to_bytes("abcdef")
+        >>> _to_bytes("abcdef")
         b'abcdef=='
-        >>> to_bytes("abcdefg")
+        >>> _to_bytes("abcdefg")
         b'abcdefg='
     """
 
     r = len(s) % 4
     if r != 0:
         s += "=" * (4 - r)
```

### Comparing `phable-0.1.6/pyproject.toml` & `phable-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phable"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Rick Jennings <rjennings055@gmail.com>"]
 readme = "README.md"
 packages = [{include = "phable"}]
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `phable-0.1.6/PKG-INFO` & `phable-0.1.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: phable
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 License: MIT
 Author: Rick Jennings
 Author-email: rjennings055@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 About
 -----
-Phable provides a simple way to retrieve Haystack tagged JSON data from a file or Haystack server using Python.  The retrieved data is reformatted to integrate seamlessly with popular open source Python libraries including, Pandas, Numpy, Matplotlib, and more.
+Phable provides a simple way to retrieve and process JSON formatted [Project Haystack](https://project-haystack.org/) data from a flat file or Haystack server using modern Python.
 
-Python has evolved during the past few years, having introduced type hints, asyncio, and more.  These enhancements make it easier to read and debug Python code.  To that end Phable is designed using the latest Python features.
-
-Haystack in this context is a reference to [Project Haystack](https://project-haystack.org/), which is an open source initiative to streamline working with IoT Data.  Project Haystack standardizes semantic data models and web services with the goal of making it easier to unlock value from the vast quantity of data being generated by the smart devices that permeate our homes, buildings, factories, and cities.
+The initial focus of this project is to make it easy to work with a Jupyter Notebook connected to a Haystack server.
 
 Installation
 ------------
-Phable requires Python 3.11 or higher and has no other dependencies.  Phable will likely most often be used with other 3rd party libraries and built-in support is provided.  (TODO :  Explain more)
+Phable requires Python 3.11 or higher.  During the early stages of this project we will likely have several Python package dependencies, such as Pandas.  In the future we hope to remove these dependencies from Phable.
 
 Download Phable from Pypi:
 
 ```console
 $ pip install phable
 ```
 
@@ -39,43 +37,17 @@
 
 # define these settings specific for your use case
 # Reminder:  Probably secure your login credentials!!!
 uri = "http://localhost:8080/api/demo"
 username = "su"
 password = "su"
 
-# open a session, execute queries, and simply close
+# open a session, execute a query, and simply close
 # session with the context manager
 with Phable(uri, username, password) as ph:
-    ph.about()
+    about_grid = ph.about()
+
+print(f"Here are details about the Haystack Server:\n{about_grid}")
 ```
 
 **More examples coming soon!**
 
-Future
-------
-Today Phable formally supports read-only data operations.  As this project matures we would like to add more features.
-
-The near-term focus is on making this project easily understood by a Python developer - refactoring the code several times and improving the documentation.  We would love your feedback and contributions!
-
-License
--------
-To be defined
-
-TODO
-----
-- Support pandas without requiring pandas dependency
-- Improve docs
-- Improve tests
-- Add more tests
-- Factory for serializers
-- Explain in the docs that zoneinfo module is used for tz data and may require other dependencies
-- Validate the Haystack timezones
-- Only provide tests for what is exposed on the API
-- Test Coord, XStr, and other kinds over API
-- Improve parsing of singletons Marker, Remove, and NA
-- Setup some prod and test log settings
-
-Questions
----------
- - What version Haystack should I put in the Grid meta?
- - How do we validate the responses meet the Haystack requirements?
```

