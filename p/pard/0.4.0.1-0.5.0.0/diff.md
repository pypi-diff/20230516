# Comparing `tmp/pard-0.4.0.1.tar.gz` & `tmp/pard-0.5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pard-0.4.0.1.tar", max compression
+gzip compressed data, was "pard-0.5.0.0.tar", max compression
```

## Comparing `pard-0.4.0.1.tar` & `pard-0.5.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      182 2022-10-23 20:05:25.206355 pard-0.4.0.1/pard/__init__.py
--rw-r--r--   0        0        0     1430 2022-10-23 20:03:40.655460 pard-0.4.0.1/pard/_handling_3_letter_code_decorator.py
--rw-r--r--   0        0        0   248922 2023-04-04 13:01:29.603738 pard-0.4.0.1/pard/_raw_python_dictionaries.py
--rw-r--r--   0        0        0      845 2022-10-23 20:10:27.038271 pard-0.4.0.1/pard/epstein.py
--rw-r--r--   0        0        0     1731 2022-10-23 20:10:27.047831 pard-0.4.0.1/pard/experimental_exchangeability.py
--rw-r--r--   0        0        0      532 2022-10-23 20:10:27.034177 pard-0.4.0.1/pard/grantham.py
--rw-r--r--   0        0        0     5498 2023-02-27 17:05:25.237415 pard-0.4.0.1/pard/koshi_goldstein.py
--rw-r--r--   0        0        0      528 2022-10-23 20:10:27.053363 pard-0.4.0.1/pard/miyata.py
--rw-r--r--   0        0        0      526 2022-10-23 20:10:27.043726 pard-0.4.0.1/pard/sneath.py
--rw-r--r--   0        0        0      548 2023-04-04 13:03:41.129588 pard-0.4.0.1/pyproject.toml
--rw-r--r--   0        0        0     9182 2023-04-04 13:03:41.129588 pard-0.4.0.1/README.md
--rw-r--r--   0        0        0     9761 1970-01-01 00:00:00.000000 pard-0.4.0.1/setup.py
--rw-r--r--   0        0        0     9336 1970-01-01 00:00:00.000000 pard-0.4.0.1/PKG-INFO
+-rw-r--r--   0        0        0      182 2022-10-23 20:05:25.206355 pard-0.5.0.0/pard/__init__.py
+-rw-r--r--   0        0        0     1430 2022-10-23 20:03:40.655460 pard-0.5.0.0/pard/_handling_3_letter_code_decorator.py
+-rw-r--r--   0        0        0   260023 2023-05-16 13:19:45.789837 pard-0.5.0.0/pard/_raw_python_dictionaries.py
+-rw-r--r--   0        0        0      845 2022-10-23 20:10:27.038271 pard-0.5.0.0/pard/epstein.py
+-rw-r--r--   0        0        0     1722 2023-05-16 13:23:51.722407 pard-0.5.0.0/pard/experimental_exchangeability.py
+-rw-r--r--   0        0        0      532 2022-10-23 20:10:27.034177 pard-0.5.0.0/pard/grantham.py
+-rw-r--r--   0        0        0     1085 2023-05-16 13:25:23.144824 pard-0.5.0.0/pard/kolaskar.py
+-rw-r--r--   0        0        0     5498 2023-02-27 17:05:25.237415 pard-0.5.0.0/pard/koshi_goldstein.py
+-rw-r--r--   0        0        0      528 2022-10-23 20:10:27.053363 pard-0.5.0.0/pard/miyata.py
+-rw-r--r--   0        0        0      526 2022-10-23 20:10:27.043726 pard-0.5.0.0/pard/sneath.py
+-rw-r--r--   0        0        0      548 2023-05-16 13:32:58.000106 pard-0.5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9759 2023-05-16 13:43:06.172201 pard-0.5.0.0/README.md
+-rw-r--r--   0        0        0    10341 1970-01-01 00:00:00.000000 pard-0.5.0.0/setup.py
+-rw-r--r--   0        0        0     9906 1970-01-01 00:00:00.000000 pard-0.5.0.0/PKG-INFO
```

### Comparing `pard-0.4.0.1/pard/_handling_3_letter_code_decorator.py` & `pard-0.5.0.0/pard/_handling_3_letter_code_decorator.py`

 * *Files identical despite different names*

### Comparing `pard-0.4.0.1/pard/_raw_python_dictionaries.py` & `pard-0.5.0.0/pard/_raw_python_dictionaries.py`

 * *Files 4% similar despite different names*

```diff
@@ -1644,14 +1644,428 @@
         ("K", "K"): 0,
         ("R", "R"): 0,
     }
 
     return epstein_dict
 
 
+def make_kolaskar_dict() -> dict[tuple[str, str], float]:
+    """
+    :return: Dictionary representative of TABLE 2 from 'Sequence alignment approach to pick up conformationally similar
+             protein fragments' by Kolaskar, AS and Kulkarni-Kale, Urmila. Keys are pairs of strings. Cf. scientific
+             paper for more details on how those scores are derived.
+             The matrix is also called the 'Conformational similarity weight matrix'.
+    """
+
+    kolaskar_dict: dict[tuple[str, str], float] = {
+        ("A", "A"): 10.0,
+        ("A", "R"): 6.6,
+        ("A", "N"): 0.0,
+        ("A", "D"): 0.0,
+        ("A", "C"): 0.0,
+        ("A", "Q"): 6.6,
+        ("A", "E"): 9.0,
+        ("A", "G"): 0.0,
+        ("A", "H"): 0.0,
+        ("A", "I"): 0.0,
+        ("A", "L"): 5.0,
+        ("A", "K"): 6.6,
+        ("A", "M"): 5.0,
+        ("A", "F"): 0.0,
+        ("A", "P"): 0.0,
+        ("A", "S"): 0.0,
+        ("A", "T"): 0.0,
+        ("A", "W"): 0.0,
+        ("A", "Y"): 0.0,
+        ("A", "V"): 0.0,
+        ("R", "A"): 6.6,
+        ("R", "R"): 10.0,
+        ("R", "N"): 0.0,
+        ("R", "D"): 0.0,
+        ("R", "C"): 0.0,
+        ("R", "Q"): 9.0,
+        ("R", "E"): 6.6,
+        ("R", "G"): 0.0,
+        ("R", "H"): 5.0,
+        ("R", "I"): 0.0,
+        ("R", "L"): 6.6,
+        ("R", "K"): 9.0,
+        ("R", "M"): 9.0,
+        ("R", "F"): 9.0,
+        ("R", "P"): 0.0,
+        ("R", "S"): 5.0,
+        ("R", "T"): 5.0,
+        ("R", "W"): 6.6,
+        ("R", "Y"): 5.0,
+        ("R", "V"): 0.0,
+        ("N", "A"): 0.0,
+        ("N", "R"): 0.0,
+        ("N", "N"): 10.0,
+        ("N", "D"): 9.0,
+        ("N", "C"): 0.0,
+        ("N", "Q"): 0.0,
+        ("N", "E"): 0.0,
+        ("N", "G"): 0.0,
+        ("N", "H"): 5.0,
+        ("N", "I"): 0.0,
+        ("N", "L"): 0.0,
+        ("N", "K"): 0.0,
+        ("N", "M"): 0.0,
+        ("N", "F"): 0.0,
+        ("N", "P"): 0.0,
+        ("N", "S"): 6.6,
+        ("N", "T"): 0.0,
+        ("N", "W"): 0.0,
+        ("N", "Y"): 0.0,
+        ("N", "V"): 0.0,
+        ("D", "A"): 0.0,
+        ("D", "R"): 0.0,
+        ("D", "N"): 9.0,
+        ("D", "D"): 10.0,
+        ("D", "C"): 0.0,
+        ("D", "Q"): 0.0,
+        ("D", "E"): 0.0,
+        ("D", "G"): 0.0,
+        ("D", "H"): 6.6,
+        ("D", "I"): 0.0,
+        ("D", "L"): 0.0,
+        ("D", "K"): 5.0,
+        ("D", "M"): 0.0,
+        ("D", "F"): 0.0,
+        ("D", "P"): 0.0,
+        ("D", "S"): 6.6,
+        ("D", "T"): 0.0,
+        ("D", "W"): 0.0,
+        ("D", "Y"): 0.0,
+        ("D", "V"): 0.0,
+        ("C", "A"): 0.0,
+        ("C", "R"): 0.0,
+        ("C", "N"): 0.0,
+        ("C", "D"): 0.0,
+        ("C", "C"): 10.0,
+        ("C", "Q"): 0.0,
+        ("C", "E"): 0.0,
+        ("C", "G"): 0.0,
+        ("C", "H"): 9.0,
+        ("C", "I"): 0.0,
+        ("C", "L"): 0.0,
+        ("C", "K"): 0.0,
+        ("C", "M"): 0.0,
+        ("C", "F"): 5.0,
+        ("C", "P"): 0.0,
+        ("C", "S"): 9.0,
+        ("C", "T"): 6.6,
+        ("C", "W"): 5.0,
+        ("C", "Y"): 5.0,
+        ("C", "V"): 0.0,
+        ("Q", "A"): 6.6,
+        ("Q", "R"): 9.0,
+        ("Q", "N"): 0.0,
+        ("Q", "D"): 0.0,
+        ("Q", "C"): 0.0,
+        ("Q", "Q"): 10.0,
+        ("Q", "E"): 6.6,
+        ("Q", "G"): 0.0,
+        ("Q", "H"): 5.0,
+        ("Q", "I"): 0.0,
+        ("Q", "L"): 9.0,
+        ("Q", "K"): 9.0,
+        ("Q", "M"): 5.0,
+        ("Q", "F"): 6.6,
+        ("Q", "P"): 0.0,
+        ("Q", "S"): 0.0,
+        ("Q", "T"): 5.0,
+        ("Q", "W"): 5.0,
+        ("Q", "Y"): 5.0,
+        ("Q", "V"): 0.0,
+        ("E", "A"): 9.0,
+        ("E", "R"): 6.6,
+        ("E", "N"): 0.0,
+        ("E", "D"): 0.0,
+        ("E", "C"): 0.0,
+        ("E", "Q"): 6.6,
+        ("E", "E"): 10.0,
+        ("E", "G"): 0.0,
+        ("E", "H"): 0.0,
+        ("E", "I"): 0.0,
+        ("E", "L"): 5.0,
+        ("E", "K"): 9.0,
+        ("E", "M"): 0.0,
+        ("E", "F"): 0.0,
+        ("E", "P"): 0.0,
+        ("E", "S"): 0.0,
+        ("E", "T"): 0.0,
+        ("E", "W"): 0.0,
+        ("E", "Y"): 0.0,
+        ("E", "V"): 0.0,
+        ("G", "A"): 0.0,
+        ("G", "R"): 0.0,
+        ("G", "N"): 0.0,
+        ("G", "D"): 0.0,
+        ("G", "C"): 0.0,
+        ("G", "Q"): 0.0,
+        ("G", "E"): 0.0,
+        ("G", "G"): 10.0,
+        ("G", "H"): 0.0,
+        ("G", "I"): 0.0,
+        ("G", "L"): 0.0,
+        ("G", "K"): 0.0,
+        ("G", "M"): 0.0,
+        ("G", "F"): 0.0,
+        ("G", "P"): 0.0,
+        ("G", "S"): 0.0,
+        ("G", "T"): 0.0,
+        ("G", "W"): 0.0,
+        ("G", "Y"): 0.0,
+        ("G", "V"): 0.0,
+        ("H", "A"): 0.0,
+        ("H", "R"): 5.0,
+        ("H", "N"): 5.0,
+        ("H", "D"): 6.6,
+        ("H", "C"): 9.0,
+        ("H", "Q"): 5.0,
+        ("H", "E"): 0.0,
+        ("H", "G"): 0.0,
+        ("H", "H"): 10.0,
+        ("H", "I"): 0.0,
+        ("H", "L"): 0.0,
+        ("H", "K"): 0.0,
+        ("H", "M"): 0.0,
+        ("H", "F"): 5.0,
+        ("H", "P"): 0.0,
+        ("H", "S"): 9.0,
+        ("H", "T"): 5.0,
+        ("H", "W"): 5.0,
+        ("H", "Y"): 6.6,
+        ("H", "V"): 0.0,
+        ("I", "A"): 0.0,
+        ("I", "R"): 0.0,
+        ("I", "N"): 0.0,
+        ("I", "D"): 0.0,
+        ("I", "C"): 0.0,
+        ("I", "Q"): 0.0,
+        ("I", "E"): 0.0,
+        ("I", "G"): 0.0,
+        ("I", "H"): 0.0,
+        ("I", "I"): 10.0,
+        ("I", "L"): 0.0,
+        ("I", "K"): 0.0,
+        ("I", "M"): 0.0,
+        ("I", "F"): 0.0,
+        ("I", "P"): 0.0,
+        ("I", "S"): 0.0,
+        ("I", "T"): 0.0,
+        ("I", "W"): 0.0,
+        ("I", "Y"): 0.0,
+        ("I", "V"): 9.0,
+        ("L", "A"): 5.0,
+        ("L", "R"): 6.6,
+        ("L", "N"): 0.0,
+        ("L", "D"): 0.0,
+        ("L", "C"): 0.0,
+        ("L", "Q"): 9.0,
+        ("L", "E"): 5.0,
+        ("L", "G"): 0.0,
+        ("L", "H"): 0.0,
+        ("L", "I"): 0.0,
+        ("L", "L"): 10.0,
+        ("L", "K"): 9.0,
+        ("L", "M"): 6.6,
+        ("L", "F"): 5.0,
+        ("L", "P"): 0.0,
+        ("L", "S"): 0.0,
+        ("L", "T"): 0.0,
+        ("L", "W"): 5.0,
+        ("L", "Y"): 0.0,
+        ("L", "V"): 0.0,
+        ("K", "A"): 6.6,
+        ("K", "R"): 9.0,
+        ("K", "N"): 0.0,
+        ("K", "D"): 5.0,
+        ("K", "C"): 0.0,
+        ("K", "Q"): 9.0,
+        ("K", "E"): 9.0,
+        ("K", "G"): 0.0,
+        ("K", "H"): 0.0,
+        ("K", "I"): 0.0,
+        ("K", "L"): 9.0,
+        ("K", "K"): 10.0,
+        ("K", "M"): 5.0,
+        ("K", "F"): 5.0,
+        ("K", "P"): 0.0,
+        ("K", "S"): 5.0,
+        ("K", "T"): 5.0,
+        ("K", "W"): 0.0,
+        ("K", "Y"): 0.0,
+        ("K", "V"): 0.0,
+        ("M", "A"): 5.0,
+        ("M", "R"): 9.0,
+        ("M", "N"): 0.0,
+        ("M", "D"): 0.0,
+        ("M", "C"): 0.0,
+        ("M", "Q"): 5.0,
+        ("M", "E"): 0.0,
+        ("M", "G"): 0.0,
+        ("M", "H"): 0.0,
+        ("M", "I"): 0.0,
+        ("M", "L"): 6.6,
+        ("M", "K"): 5.0,
+        ("M", "M"): 10.0,
+        ("M", "F"): 6.6,
+        ("M", "P"): 0.0,
+        ("M", "S"): 0.0,
+        ("M", "T"): 0.0,
+        ("M", "W"): 6.6,
+        ("M", "Y"): 0.0,
+        ("M", "V"): 0.0,
+        ("F", "A"): 0.0,
+        ("F", "R"): 9.0,
+        ("F", "N"): 0.0,
+        ("F", "D"): 0.0,
+        ("F", "C"): 5.0,
+        ("F", "Q"): 6.6,
+        ("F", "E"): 0.0,
+        ("F", "G"): 0.0,
+        ("F", "H"): 5.0,
+        ("F", "I"): 0.0,
+        ("F", "L"): 5.0,
+        ("F", "K"): 5.0,
+        ("F", "M"): 6.6,
+        ("F", "F"): 10.0,
+        ("F", "P"): 0.0,
+        ("F", "S"): 5.0,
+        ("F", "T"): 5.0,
+        ("F", "W"): 9.0,
+        ("F", "Y"): 9.0,
+        ("F", "V"): 0.0,
+        ("P", "A"): 0.0,
+        ("P", "R"): 0.0,
+        ("P", "N"): 0.0,
+        ("P", "D"): 0.0,
+        ("P", "C"): 0.0,
+        ("P", "Q"): 0.0,
+        ("P", "E"): 0.0,
+        ("P", "G"): 0.0,
+        ("P", "H"): 0.0,
+        ("P", "I"): 0.0,
+        ("P", "L"): 0.0,
+        ("P", "K"): 0.0,
+        ("P", "M"): 0.0,
+        ("P", "F"): 0.0,
+        ("P", "P"): 10.0,
+        ("P", "S"): 0.0,
+        ("P", "T"): 0.0,
+        ("P", "W"): 0.0,
+        ("P", "Y"): 0.0,
+        ("P", "V"): 0.0,
+        ("S", "A"): 0.0,
+        ("S", "R"): 5.0,
+        ("S", "N"): 6.6,
+        ("S", "D"): 6.6,
+        ("S", "C"): 9.0,
+        ("S", "Q"): 0.0,
+        ("S", "E"): 0.0,
+        ("S", "G"): 0.0,
+        ("S", "H"): 9.0,
+        ("S", "I"): 0.0,
+        ("S", "L"): 0.0,
+        ("S", "K"): 5.0,
+        ("S", "M"): 0.0,
+        ("S", "F"): 5.0,
+        ("S", "P"): 0.0,
+        ("S", "S"): 10.0,
+        ("S", "T"): 6.6,
+        ("S", "W"): 5.0,
+        ("S", "Y"): 6.6,
+        ("S", "V"): 0.0,
+        ("T", "A"): 0.0,
+        ("T", "R"): 5.0,
+        ("T", "N"): 0.0,
+        ("T", "D"): 0.0,
+        ("T", "C"): 6.6,
+        ("T", "Q"): 5.0,
+        ("T", "E"): 0.0,
+        ("T", "G"): 0.0,
+        ("T", "H"): 5.0,
+        ("T", "I"): 0.0,
+        ("T", "L"): 0.0,
+        ("T", "K"): 5.0,
+        ("T", "M"): 0.0,
+        ("T", "F"): 5.0,
+        ("T", "P"): 0.0,
+        ("T", "S"): 6.6,
+        ("T", "T"): 10.0,
+        ("T", "W"): 5.0,
+        ("T", "Y"): 9.0,
+        ("T", "V"): 0.0,
+        ("W", "A"): 0.0,
+        ("W", "R"): 6.6,
+        ("W", "N"): 0.0,
+        ("W", "D"): 0.0,
+        ("W", "C"): 5.0,
+        ("W", "Q"): 5.0,
+        ("W", "E"): 0.0,
+        ("W", "G"): 0.0,
+        ("W", "H"): 5.0,
+        ("W", "I"): 0.0,
+        ("W", "L"): 5.0,
+        ("W", "K"): 0.0,
+        ("W", "M"): 6.6,
+        ("W", "F"): 9.0,
+        ("W", "P"): 0.0,
+        ("W", "S"): 5.0,
+        ("W", "T"): 5.0,
+        ("W", "W"): 10.0,
+        ("W", "Y"): 5.0,
+        ("W", "V"): 0.0,
+        ("Y", "A"): 0.0,
+        ("Y", "R"): 5.0,
+        ("Y", "N"): 0.0,
+        ("Y", "D"): 0.0,
+        ("Y", "C"): 5.0,
+        ("Y", "Q"): 5.0,
+        ("Y", "E"): 0.0,
+        ("Y", "G"): 0.0,
+        ("Y", "H"): 6.6,
+        ("Y", "I"): 0.0,
+        ("Y", "L"): 0.0,
+        ("Y", "K"): 0.0,
+        ("Y", "M"): 0.0,
+        ("Y", "F"): 9.0,
+        ("Y", "P"): 0.0,
+        ("Y", "S"): 6.6,
+        ("Y", "T"): 9.0,
+        ("Y", "W"): 5.0,
+        ("Y", "Y"): 10.0,
+        ("Y", "V"): 0.0,
+        ("V", "A"): 0.0,
+        ("V", "R"): 0.0,
+        ("V", "N"): 0.0,
+        ("V", "D"): 0.0,
+        ("V", "C"): 0.0,
+        ("V", "Q"): 0.0,
+        ("V", "E"): 0.0,
+        ("V", "G"): 0.0,
+        ("V", "H"): 0.0,
+        ("V", "I"): 9.0,
+        ("V", "L"): 0.0,
+        ("V", "K"): 0.0,
+        ("V", "M"): 0.0,
+        ("V", "F"): 0.0,
+        ("V", "P"): 0.0,
+        ("V", "S"): 0.0,
+        ("V", "T"): 0.0,
+        ("V", "W"): 0.0,
+        ("V", "Y"): 0.0,
+        ("V", "V"): 10.0,
+    }
+
+    return kolaskar_dict
+
+
 def make_symmetric_experimental_exchangeability_dict() -> dict[tuple[str, str], float]:
     """
     :return: A dictionary representative of TABLE 2 & 3 from 'The Exchangeability of Amino Acids in Proteins' by Lev Y.
              Yampolsky and Arlin Stoltzfus. Keys are pairs of strings. Cf. scientific paper for more details on how
              those scores are derived. Cf. paper for formula used to infer the symmetrised version (weighted mean).
              It does not have any missing values like the asymmetrical verison does, cf. article:
              'The symmetric matrix EXSij has no missing values because exchange data are available for every possible
@@ -9145,14 +9559,15 @@
     )
 
 
 SNEATH_DICT: dict[tuple[str, str], int]
 MIYATA_DICT: dict[tuple[str, str], float]
 SYMMETRIC_EPSTEIN_DICT: dict[tuple[str, str], float]
 ASYMMETRIC_EPSTEIN_DICT: dict[tuple[str, str], float]
+KOLASKAR_DICT: dict[tuple[str, str], float]
 SYMMETRIC_EXPERIMENTAL_EXCHANGEABILITY_DICT: dict[tuple[str, str], float]
 ASYMMETRIC_EXPERIMENTAL_EXCHANGEABILITY_DICT: dict[tuple[str, str], int | None]
 GRANTHAM_DICT: dict[tuple[str, str], int]
 SYMMETRIC_KOSHI_GOLDSTEIN_ALL_RESIDUES_DICT: dict[tuple[str, str], float]
 ASYMMETRIC_KOSHI_GOLDSTEIN_ALL_RESIDUES_DICT: dict[tuple[str, str], float]
 SYMMETRIC_KOSHI_GOLDSTEIN_EXPOSED_RESIDUES_DICT: dict[tuple[str, str], float]
 ASYMMETRIC_KOSHI_GOLDSTEIN_EXPOSED_RESIDUES_DICT: dict[tuple[str, str], float]
@@ -9160,14 +9575,15 @@
 ASYMMETRIC_KOSHI_GOLDSTEIN_BURIED_RESIDUES_DICT: dict[tuple[str, str], float]
 
 
 SNEATH_DICT                                  = make_sneath_dict()
 MIYATA_DICT                                  = make_miyata_dict()
 SYMMETRIC_EPSTEIN_DICT                       = make_symmetric_epstein_dict()
 ASYMMETRIC_EPSTEIN_DICT                      = make_asymmetric_epstein_dict()
+KOLASKAR_DICT                                = make_kolaskar_dict()
 SYMMETRIC_EXPERIMENTAL_EXCHANGEABILITY_DICT  = make_symmetric_experimental_exchangeability_dict()
 ASYMMETRIC_EXPERIMENTAL_EXCHANGEABILITY_DICT = make_asymmetric_experimental_exchangeability_dict()
 GRANTHAM_DICT                                = make_grantham_dict()
 # Koshi-Goldstein dicts
 (
     SYMMETRIC_KOSHI_GOLDSTEIN_ALL_RESIDUES_DICT,
     SYMMETRIC_KOSHI_GOLDSTEIN_EXPOSED_RESIDUES_DICT,
```

### Comparing `pard-0.4.0.1/pard/epstein.py` & `pard-0.5.0.0/pard/epstein.py`

 * *Files identical despite different names*

### Comparing `pard-0.4.0.1/pard/experimental_exchangeability.py` & `pard-0.5.0.0/pard/experimental_exchangeability.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     :param amino_acid_1: 1 letter code of the first amino acid
     :param amino_acid_2: 1 letter code of the third amino acid
     :param symmetric: whether the symmetric version of the matrix is wanted or not (i.e. exchanges of known* or
                       unknown direction)
                       * amino_acid_1 -> amino_acid_2
     :param warning: Set warning to False to stop seeing the warning
 
-    :return: An integer / float / None representing the experimental exchangeability distance between amino_acid_1 and
+    :return: An integer / float / None representing the experimental exchangeability between amino_acid_1 and
              amino_acid_2 (x1000)
     """
     if warning:
         logging.warning(
             " Friendly reminder that exchangeability is not a distance. Rather, it is the mean activity of"
             " variants with an exchange from amino acid amino_acid_1 to amino_acid_2. Meaning, high"
             " exchangeability is likely to mean that the amino acids are similar, although this statement"
```

### Comparing `pard-0.4.0.1/pard/grantham.py` & `pard-0.5.0.0/pard/grantham.py`

 * *Files identical despite different names*

### Comparing `pard-0.4.0.1/pard/koshi_goldstein.py` & `pard-0.5.0.0/pard/koshi_goldstein.py`

 * *Files identical despite different names*

### Comparing `pard-0.4.0.1/pard/miyata.py` & `pard-0.5.0.0/pard/miyata.py`

 * *Files identical despite different names*

### Comparing `pard-0.4.0.1/pard/sneath.py` & `pard-0.5.0.0/pard/sneath.py`

 * *Files identical despite different names*

### Comparing `pard-0.4.0.1/pyproject.toml` & `pard-0.5.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pard"
-version = "0.4.0.1"
+version = "0.5.0.0"
 description = "Physicochemical Amino acid Replacement Distances"
 authors = ["JasonMendoza2008 <lhotteromain@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "pard"},
 ]
```

### Comparing `pard-0.4.0.1/README.md` & `pard-0.5.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,19 @@
 experimental protein activity and stability after exchanging one amino acid into another
 [[5]](https://pubmed.ncbi.nlm.nih.gov/15944362/),
 etc.
 
 `pard` is a package designed to make those **P**hysicochemical **A**mino acid **R**eplacement **D**istances calculations
 straightforward with Python.
 
-One typical use is to establish a 'distance' between a wild-type protein and its mutated version.
+One typical use is to establish a 'distance' between a wild-type protein and its mutated version. Sometimes, rather
+than a distance, a similarity is outputted (e.g. with `the Conformational similarity weight matrix`
+[[7]](https://www.sciencedirect.com/science/article/abs/pii/002228369290261H)). The higher the distance, the more
+different the two amino acids are. The higher the similarity, the more similar the two amino acids are. Whenever
+a distance is not outputted but rather a similarity, a warning (that the user can turn off) will be raised.
 
 
 ### Getting started
 #### Install from PyPI (recommended)
 To use `pard`, run `pip install pard` in your terminal.
 
 #### Usage
@@ -142,85 +146,88 @@
 #### Unit tests details
 Coverage
 ```
 Name                                         Stmts   Miss  Cover
 ----------------------------------------------------------------
 pard\__init__.py                                 3      0   100%
 pard\_handling_3_letter_code_decorator.py       18      2    89%
-pard\_raw_python_dictionaries.py                61     32    48%
+pard\_raw_python_dictionaries.py                66      0   100%
 pard\epstein.py                                  7      0   100%
 pard\experimental_exchangeability.py            10      0   100%
 pard\grantham.py                                 5      0   100%
-pard\koshi_goldstein.py                         55     24    56%
+pard\kolaskar.py                                 8      0   100%
+pard\koshi_goldstein.py                         55      2    96%
 pard\miyata.py                                   5      0   100%
 pard\sneath.py                                   5      0   100%
 tests\__init__.py                                0      0   100%
 tests\test_epstein.py                           46      0   100%
 tests\test_experimental_exchangeability.py      30      0   100%
 tests\test_grantham.py                          25      0   100%
-tests\test_koshi_goldstein.py                  108     50    54%
+tests\test_kolaskar.py                          26      0   100%
+tests\test_koshi_goldstein.py                  108      0   100%
 tests\test_miyata.py                            25      0   100%
 tests\test_pard.py                               3      0   100%
-tests\test_raw_python_dictionaries.py           20     11    45%
+tests\test_raw_python_dictionaries.py           22      0   100%
 tests\test_sneath.py                            21      0   100%
-unit_tests_mypy.py                               5      5     0%
-unit_tests_simple.py                             5      5     0%
+unit_tests_simple.py                             5      0   100%
 ----------------------------------------------------------------
-TOTAL                                          457    129    72%
+TOTAL                                          493      4    99%
 ```
 
 #### pytest
 ```
 platform win32 -- Python 3.11.1, pytest-7.2.0, pluggy-1.0.0
 plugins: anyio-3.6.2, mypy-0.10.3
-collected 14 items
+collected 15 items
 
-tests\test_epstein.py .                                                  [  7%]
-tests\test_experimental_exchangeability.py .                             [ 14%]
-tests\test_grantham.py .                                                 [ 21%]
-tests\test_koshi_goldstein.py .......                                    [ 71%]
-tests\test_miyata.py .                                                   [ 78%]
-tests\test_pard.py .                                                     [ 85%]
-tests\test_raw_python_dictionaries.py .                                  [ 92%]
-tests\test_sneath.py .                                                   [100%]
+tests\test_epstein.py .                                              [  6%] 
+tests\test_experimental_exchangeability.py .                         [ 13%] 
+tests\test_grantham.py .                                             [ 20%] 
+tests\test_kolaskar.py .                                             [ 26%] 
+tests\test_koshi_goldstein.py .......                                [ 73%]
+tests\test_miyata.py .                                               [ 80%] 
+tests\test_pard.py .                                                 [ 86%] 
+tests\test_raw_python_dictionaries.py .                              [ 93%]
+tests\test_sneath.py .                                               [100%]
+
+=========================== 15 passed in 0.06s ===========================
 
-============================= 14 passed in 0.06s ==============================
 ```
 
 #### mypy detail
 ```
-=============================== mypy ===============================
-Success: no issues found in 20 source files
+================================== mypy ==================================
+Success: no issues found in 22 source files
 ```
 
 ### Useful links:
 - [Corresponding GitHub repository](https://github.com/MICS-Lab/pard)
 - [Corresponding PyPI page](https://pypi.org/project/pard/)
 
 
 ### Citation
 If you use this software, please cite it as below.
 
 - APA:
 
 `
 Lhotte, R. & Taupin, J. (2022).
-Physicochemical Amino acid Replacement Distances (PARD) package (Version 0.4.0.1) [Computer software].
+Physicochemical Amino acid Replacement Distances (PARD) package (Version 0.5.0.0) [Computer software].
 https://doi.org/10.5281/zenodo.7013169
 `
 
 - BibTeX:
 
 ```
 @software{lhotte_pard_2022,
     author = {Lhotte, Romain and Taupin, Jean-Luc},
     doi = {10.5281/zenodo.7013169},
     month = {8},
     title = {{Physicochemical Amino acid Replacement Distances (PARD) package}},
-    version = {0.4.0.1},
+    version = {0.5.0.0},
     year = {2022}
 }
 ```
 
 
 ### References
 - [1] Grantham, R., 1974. Amino acid difference formula to help explain protein evolution. science, 185(4154),
```

### Comparing `pard-0.4.0.1/setup.py` & `pard-0.5.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['pard']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'pard',
-    'version': '0.4.0.1',
+    'version': '0.5.0.0',
     'description': 'Physicochemical Amino acid Replacement Distances',
-    'long_description': '## PARD (Physicochemical Amino acid Replacement Distances)\n[![DOI](https://zenodo.org/badge/526882024.svg)](https://zenodo.org/badge/latestdoi/526882024)\n![Coverage](\nreadme_resources/coverage.svg\n)\n[![Downloads](https://pepy.tech/badge/pard)](https://pepy.tech/project/pard)\n\n### Overview\nAmino acid replacements (also referred to as substitutions) are changes from one amino acid to a different one in a\nprotein - and there are different ways to assess the difference between the two amino acids that come into play in an\namino acid replacement.\n\nOne can look at one or several properties\' discrepancy between two amino acids.\nTo list only a few: polarity\n[[1]](https://www.science.org/doi/10.1126/science.185.4154.862) [[3]](https://www.nature.com/articles/215355a0) \n[[4]](https://link.springer.com/article/10.1007/BF01732340),\nmolecular volume / relative sizes of amino-acid side chains \n[[1]](https://www.science.org/doi/10.1126/science.185.4154.862) [[3]](https://www.nature.com/articles/215355a0)\n[[4]](https://link.springer.com/article/10.1007/BF01732340), \nmean number of lone pair electrons on the side-chain\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123),\nmaximum moment of inertia for rotation at the α―β bond\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123)\nor at the β―γ bond [[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123)\nor at the γ―δ bond [[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123), \npresence of a pyrrolidine ring (proline (P))\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123), \nexperimental protein activity and stability after exchanging one amino acid into another\n[[5]](https://pubmed.ncbi.nlm.nih.gov/15944362/),\netc.\n\n`pard` is a package designed to make those **P**hysicochemical **A**mino acid **R**eplacement **D**istances calculations\nstraightforward with Python.\n\nOne typical use is to establish a \'distance\' between a wild-type protein and its mutated version.\n\n\n### Getting started\n#### Install from PyPI (recommended)\nTo use `pard`, run `pip install pard` in your terminal.\n\n#### Usage\n```py\n## Imports\nfrom pard.grantham import grantham\nfrom pard.sneath import sneath\nfrom pard.experimental_exchangeability import experimental_exchangeability\nfrom pard.koshi_goldstein import koshi_goldstein, MatrixType\n\n\n## Basic examples\namino_acid_1: str = "W"  # Tryptophan\namino_acid_2: str = "L"  # Leucine\ndistance_grantham: int = grantham(amino_acid_1, amino_acid_2)\nprint(distance_grantham)\n\ndistance_sneath: int   = sneath(amino_acid_1, amino_acid_2)\nprint(distance_sneath)\n\ndistance_ee: float     = experimental_exchangeability(\n    amino_acid_1, \n    amino_acid_2, \n    False, \n    warning=True\n)\nprint(distance_ee)\n\n\n## More subtle examples\n# Koshi-Goldstein has several scores and can estimate the likelihood of InDels\ndistance_koshi_goldstein_all: float = koshi_goldstein(\n    "-",\n    "A",\n    MatrixType.ALL_RESIDUES,\n    False,\n    warning=True\n)\nprint(distance_koshi_goldstein_all)\n```\nor equivalently\n```py\n## Imports\nimport pard\n\n\n## Basic examples\namino_acid_1: str = "W"  # Tryptophan\namino_acid_2: str = "L"  # Leucine\ndistance_grantham: int = pard.grantham.grantham(amino_acid_1, amino_acid_2)\nprint(distance_grantham)\n\ndistance_sneath: int   = pard.sneath.sneath(amino_acid_1, amino_acid_2)\nprint(distance_sneath)\n\ndistance_ee: float     = pard.experimental_exchangeability.experimental_exchangeability(\n    amino_acid_1,\n    amino_acid_2,\n    False,\n    warning=True\n)\nprint(distance_ee)\n\n\n## More subtle examples\n# Koshi-Goldstein has several scores and can estimate the likelihood of InDels\ndistance_koshi_goldstein_all: float = pard.koshi_goldstein.koshi_goldstein(\n    "-",\n    "A",\n    pard.koshi_goldstein.MatrixType.ALL_RESIDUES,\n    False,\n    warning=True\n)\nprint(distance_koshi_goldstein_all)\n```\nwill output:\n```\n>>> 61\n>>> 30\n>>> 177\n>>> 1.6\n```\nwhich are the correct values \n[[1]](https://www.science.org/doi/10.1126/science.185.4154.862)\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123)\n[[5]](https://pubmed.ncbi.nlm.nih.gov/15944362/)\n[[6]](https://academic.oup.com/peds/article-abstract/8/7/641/1465446)\n.\n\n#### Exit codes:\n```\n- 1: Argument amino_acid_1 or amino_acid_2 is neither of length 1 nor length 3. See error message.\n```\n\n### About the source code\n- Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.\n- All functions are unit-tested with [pytest](https://docs.pytest.org/en/6.2.x/).\n- All variables are correctly type-hinted, reviewed with [static type checker](https://mypy.readthedocs.io/en/stable/)\n`mypy`.\n- All functions are documented with [docstrings](https://www.python.org/dev/peps/pep-0257/).\n\n\n#### Unit tests details\nCoverage\n```\nName                                         Stmts   Miss  Cover\n----------------------------------------------------------------\npard\\__init__.py                                 3      0   100%\npard\\_handling_3_letter_code_decorator.py       18      2    89%\npard\\_raw_python_dictionaries.py                61     32    48%\npard\\epstein.py                                  7      0   100%\npard\\experimental_exchangeability.py            10      0   100%\npard\\grantham.py                                 5      0   100%\npard\\koshi_goldstein.py                         55     24    56%\npard\\miyata.py                                   5      0   100%\npard\\sneath.py                                   5      0   100%\ntests\\__init__.py                                0      0   100%\ntests\\test_epstein.py                           46      0   100%\ntests\\test_experimental_exchangeability.py      30      0   100%\ntests\\test_grantham.py                          25      0   100%\ntests\\test_koshi_goldstein.py                  108     50    54%\ntests\\test_miyata.py                            25      0   100%\ntests\\test_pard.py                               3      0   100%\ntests\\test_raw_python_dictionaries.py           20     11    45%\ntests\\test_sneath.py                            21      0   100%\nunit_tests_mypy.py                               5      5     0%\nunit_tests_simple.py                             5      5     0%\n----------------------------------------------------------------\nTOTAL                                          457    129    72%\n```\n\n#### pytest\n```\nplatform win32 -- Python 3.11.1, pytest-7.2.0, pluggy-1.0.0\nplugins: anyio-3.6.2, mypy-0.10.3\ncollected 14 items\n\ntests\\test_epstein.py .                                                  [  7%]\ntests\\test_experimental_exchangeability.py .                             [ 14%]\ntests\\test_grantham.py .                                                 [ 21%]\ntests\\test_koshi_goldstein.py .......                                    [ 71%]\ntests\\test_miyata.py .                                                   [ 78%]\ntests\\test_pard.py .                                                     [ 85%]\ntests\\test_raw_python_dictionaries.py .                                  [ 92%]\ntests\\test_sneath.py .                                                   [100%]\n\n============================= 14 passed in 0.06s ==============================\n```\n\n#### mypy detail\n```\n=============================== mypy ===============================\nSuccess: no issues found in 20 source files\n```\n\n### Useful links:\n- [Corresponding GitHub repository](https://github.com/MICS-Lab/pard)\n- [Corresponding PyPI page](https://pypi.org/project/pard/)\n\n\n### Citation\nIf you use this software, please cite it as below.\n\n- APA:\n\n`\nLhotte, R. & Taupin, J. (2022).\nPhysicochemical Amino acid Replacement Distances (PARD) package (Version 0.4.0.1) [Computer software].\nhttps://doi.org/10.5281/zenodo.7013169\n`\n\n- BibTeX:\n\n```\n@software{lhotte_pard_2022,\n    author = {Lhotte, Romain and Taupin, Jean-Luc},\n    doi = {10.5281/zenodo.7013169},\n    month = {8},\n    title = {{Physicochemical Amino acid Replacement Distances (PARD) package}},\n    version = {0.4.0.1},\n    year = {2022}\n}\n```\n\n\n### References\n- [1] Grantham, R., 1974. Amino acid difference formula to help explain protein evolution. science, 185(4154), \npp.862-864.\n- [2] Sneath, P.H.A., 1966. Relations between chemical structure and biological activity in peptides. Journal of\ntheoretical biology, 12(2), pp.157-195.\n- [3] Epstein, C.J., 1967. Non-randomness of ammo-acid changes in the evolution of homologous proteins. Nature,\n215(5099), pp.355-359.\n- [4] Miyata, T., Miyazawa, S. and Yasunaga, T., 1979. Two types of amino acid substitutions in protein evolution. \nJournal of molecular evolution, 12(3), pp.219-236.\n- [5] Yampolsky, L.Y. and Stoltzfus, A., 2005. The exchangeability of amino acids in proteins. Genetics, 170(4), \npp.1459-1472.\n- [6] Koshi, J.M. and Goldstein, R.A., 1995. Context-dependent optimal substitution matrices. Protein Engineering,\nDesign and Selection, 8(7), pp.641-645.\n',
+    'long_description': '## PARD (Physicochemical Amino acid Replacement Distances)\n[![DOI](https://zenodo.org/badge/526882024.svg)](https://zenodo.org/badge/latestdoi/526882024)\n![Coverage](\nreadme_resources/coverage.svg\n)\n[![Downloads](https://pepy.tech/badge/pard)](https://pepy.tech/project/pard)\n\n### Overview\nAmino acid replacements (also referred to as substitutions) are changes from one amino acid to a different one in a\nprotein - and there are different ways to assess the difference between the two amino acids that come into play in an\namino acid replacement.\n\nOne can look at one or several properties\' discrepancy between two amino acids.\nTo list only a few: polarity\n[[1]](https://www.science.org/doi/10.1126/science.185.4154.862) [[3]](https://www.nature.com/articles/215355a0) \n[[4]](https://link.springer.com/article/10.1007/BF01732340),\nmolecular volume / relative sizes of amino-acid side chains \n[[1]](https://www.science.org/doi/10.1126/science.185.4154.862) [[3]](https://www.nature.com/articles/215355a0)\n[[4]](https://link.springer.com/article/10.1007/BF01732340), \nmean number of lone pair electrons on the side-chain\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123),\nmaximum moment of inertia for rotation at the α―β bond\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123)\nor at the β―γ bond [[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123)\nor at the γ―δ bond [[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123), \npresence of a pyrrolidine ring (proline (P))\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123), \nexperimental protein activity and stability after exchanging one amino acid into another\n[[5]](https://pubmed.ncbi.nlm.nih.gov/15944362/),\netc.\n\n`pard` is a package designed to make those **P**hysicochemical **A**mino acid **R**eplacement **D**istances calculations\nstraightforward with Python.\n\nOne typical use is to establish a \'distance\' between a wild-type protein and its mutated version. Sometimes, rather\nthan a distance, a similarity is outputted (e.g. with `the Conformational similarity weight matrix`\n[[7]](https://www.sciencedirect.com/science/article/abs/pii/002228369290261H)). The higher the distance, the more\ndifferent the two amino acids are. The higher the similarity, the more similar the two amino acids are. Whenever\na distance is not outputted but rather a similarity, a warning (that the user can turn off) will be raised.\n\n\n### Getting started\n#### Install from PyPI (recommended)\nTo use `pard`, run `pip install pard` in your terminal.\n\n#### Usage\n```py\n## Imports\nfrom pard.grantham import grantham\nfrom pard.sneath import sneath\nfrom pard.experimental_exchangeability import experimental_exchangeability\nfrom pard.koshi_goldstein import koshi_goldstein, MatrixType\n\n\n## Basic examples\namino_acid_1: str = "W"  # Tryptophan\namino_acid_2: str = "L"  # Leucine\ndistance_grantham: int = grantham(amino_acid_1, amino_acid_2)\nprint(distance_grantham)\n\ndistance_sneath: int   = sneath(amino_acid_1, amino_acid_2)\nprint(distance_sneath)\n\ndistance_ee: float     = experimental_exchangeability(\n    amino_acid_1, \n    amino_acid_2, \n    False, \n    warning=True\n)\nprint(distance_ee)\n\n\n## More subtle examples\n# Koshi-Goldstein has several scores and can estimate the likelihood of InDels\ndistance_koshi_goldstein_all: float = koshi_goldstein(\n    "-",\n    "A",\n    MatrixType.ALL_RESIDUES,\n    False,\n    warning=True\n)\nprint(distance_koshi_goldstein_all)\n```\nor equivalently\n```py\n## Imports\nimport pard\n\n\n## Basic examples\namino_acid_1: str = "W"  # Tryptophan\namino_acid_2: str = "L"  # Leucine\ndistance_grantham: int = pard.grantham.grantham(amino_acid_1, amino_acid_2)\nprint(distance_grantham)\n\ndistance_sneath: int   = pard.sneath.sneath(amino_acid_1, amino_acid_2)\nprint(distance_sneath)\n\ndistance_ee: float     = pard.experimental_exchangeability.experimental_exchangeability(\n    amino_acid_1,\n    amino_acid_2,\n    False,\n    warning=True\n)\nprint(distance_ee)\n\n\n## More subtle examples\n# Koshi-Goldstein has several scores and can estimate the likelihood of InDels\ndistance_koshi_goldstein_all: float = pard.koshi_goldstein.koshi_goldstein(\n    "-",\n    "A",\n    pard.koshi_goldstein.MatrixType.ALL_RESIDUES,\n    False,\n    warning=True\n)\nprint(distance_koshi_goldstein_all)\n```\nwill output:\n```\n>>> 61\n>>> 30\n>>> 177\n>>> 1.6\n```\nwhich are the correct values \n[[1]](https://www.science.org/doi/10.1126/science.185.4154.862)\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123)\n[[5]](https://pubmed.ncbi.nlm.nih.gov/15944362/)\n[[6]](https://academic.oup.com/peds/article-abstract/8/7/641/1465446)\n.\n\n#### Exit codes:\n```\n- 1: Argument amino_acid_1 or amino_acid_2 is neither of length 1 nor length 3. See error message.\n```\n\n### About the source code\n- Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.\n- All functions are unit-tested with [pytest](https://docs.pytest.org/en/6.2.x/).\n- All variables are correctly type-hinted, reviewed with [static type checker](https://mypy.readthedocs.io/en/stable/)\n`mypy`.\n- All functions are documented with [docstrings](https://www.python.org/dev/peps/pep-0257/).\n\n\n#### Unit tests details\nCoverage\n```\nName                                         Stmts   Miss  Cover\n----------------------------------------------------------------\npard\\__init__.py                                 3      0   100%\npard\\_handling_3_letter_code_decorator.py       18      2    89%\npard\\_raw_python_dictionaries.py                66      0   100%\npard\\epstein.py                                  7      0   100%\npard\\experimental_exchangeability.py            10      0   100%\npard\\grantham.py                                 5      0   100%\npard\\kolaskar.py                                 8      0   100%\npard\\koshi_goldstein.py                         55      2    96%\npard\\miyata.py                                   5      0   100%\npard\\sneath.py                                   5      0   100%\ntests\\__init__.py                                0      0   100%\ntests\\test_epstein.py                           46      0   100%\ntests\\test_experimental_exchangeability.py      30      0   100%\ntests\\test_grantham.py                          25      0   100%\ntests\\test_kolaskar.py                          26      0   100%\ntests\\test_koshi_goldstein.py                  108      0   100%\ntests\\test_miyata.py                            25      0   100%\ntests\\test_pard.py                               3      0   100%\ntests\\test_raw_python_dictionaries.py           22      0   100%\ntests\\test_sneath.py                            21      0   100%\nunit_tests_simple.py                             5      0   100%\n----------------------------------------------------------------\nTOTAL                                          493      4    99%\n```\n\n#### pytest\n```\nplatform win32 -- Python 3.11.1, pytest-7.2.0, pluggy-1.0.0\nplugins: anyio-3.6.2, mypy-0.10.3\ncollected 15 items\n\ntests\\test_epstein.py .                                              [  6%] \ntests\\test_experimental_exchangeability.py .                         [ 13%] \ntests\\test_grantham.py .                                             [ 20%] \ntests\\test_kolaskar.py .                                             [ 26%] \ntests\\test_koshi_goldstein.py .......                                [ 73%]\ntests\\test_miyata.py .                                               [ 80%] \ntests\\test_pard.py .                                                 [ 86%] \ntests\\test_raw_python_dictionaries.py .                              [ 93%]\ntests\\test_sneath.py .                                               [100%]\n\n=========================== 15 passed in 0.06s ===========================\n\n```\n\n#### mypy detail\n```\n================================== mypy ==================================\nSuccess: no issues found in 22 source files\n```\n\n### Useful links:\n- [Corresponding GitHub repository](https://github.com/MICS-Lab/pard)\n- [Corresponding PyPI page](https://pypi.org/project/pard/)\n\n\n### Citation\nIf you use this software, please cite it as below.\n\n- APA:\n\n`\nLhotte, R. & Taupin, J. (2022).\nPhysicochemical Amino acid Replacement Distances (PARD) package (Version 0.5.0.0) [Computer software].\nhttps://doi.org/10.5281/zenodo.7013169\n`\n\n- BibTeX:\n\n```\n@software{lhotte_pard_2022,\n    author = {Lhotte, Romain and Taupin, Jean-Luc},\n    doi = {10.5281/zenodo.7013169},\n    month = {8},\n    title = {{Physicochemical Amino acid Replacement Distances (PARD) package}},\n    version = {0.5.0.0},\n    year = {2022}\n}\n```\n\n\n### References\n- [1] Grantham, R., 1974. Amino acid difference formula to help explain protein evolution. science, 185(4154), \npp.862-864.\n- [2] Sneath, P.H.A., 1966. Relations between chemical structure and biological activity in peptides. Journal of\ntheoretical biology, 12(2), pp.157-195.\n- [3] Epstein, C.J., 1967. Non-randomness of ammo-acid changes in the evolution of homologous proteins. Nature,\n215(5099), pp.355-359.\n- [4] Miyata, T., Miyazawa, S. and Yasunaga, T., 1979. Two types of amino acid substitutions in protein evolution. \nJournal of molecular evolution, 12(3), pp.219-236.\n- [5] Yampolsky, L.Y. and Stoltzfus, A., 2005. The exchangeability of amino acids in proteins. Genetics, 170(4), \npp.1459-1472.\n- [6] Koshi, J.M. and Goldstein, R.A., 1995. Context-dependent optimal substitution matrices. Protein Engineering,\nDesign and Selection, 8(7), pp.641-645.\n',
     'author': 'JasonMendoza2008',
     'author_email': 'lhotteromain@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pard-0.4.0.1/PKG-INFO` & `pard-0.5.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pard
-Version: 0.4.0.1
+Version: 0.5.0.0
 Summary: Physicochemical Amino acid Replacement Distances
 Author: JasonMendoza2008
 Author-email: lhotteromain@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -40,15 +40,19 @@
 experimental protein activity and stability after exchanging one amino acid into another
 [[5]](https://pubmed.ncbi.nlm.nih.gov/15944362/),
 etc.
 
 `pard` is a package designed to make those **P**hysicochemical **A**mino acid **R**eplacement **D**istances calculations
 straightforward with Python.
 
-One typical use is to establish a 'distance' between a wild-type protein and its mutated version.
+One typical use is to establish a 'distance' between a wild-type protein and its mutated version. Sometimes, rather
+than a distance, a similarity is outputted (e.g. with `the Conformational similarity weight matrix`
+[[7]](https://www.sciencedirect.com/science/article/abs/pii/002228369290261H)). The higher the distance, the more
+different the two amino acids are. The higher the similarity, the more similar the two amino acids are. Whenever
+a distance is not outputted but rather a similarity, a warning (that the user can turn off) will be raised.
 
 
 ### Getting started
 #### Install from PyPI (recommended)
 To use `pard`, run `pip install pard` in your terminal.
 
 #### Usage
@@ -154,85 +158,88 @@
 #### Unit tests details
 Coverage
 ```
 Name                                         Stmts   Miss  Cover
 ----------------------------------------------------------------
 pard\__init__.py                                 3      0   100%
 pard\_handling_3_letter_code_decorator.py       18      2    89%
-pard\_raw_python_dictionaries.py                61     32    48%
+pard\_raw_python_dictionaries.py                66      0   100%
 pard\epstein.py                                  7      0   100%
 pard\experimental_exchangeability.py            10      0   100%
 pard\grantham.py                                 5      0   100%
-pard\koshi_goldstein.py                         55     24    56%
+pard\kolaskar.py                                 8      0   100%
+pard\koshi_goldstein.py                         55      2    96%
 pard\miyata.py                                   5      0   100%
 pard\sneath.py                                   5      0   100%
 tests\__init__.py                                0      0   100%
 tests\test_epstein.py                           46      0   100%
 tests\test_experimental_exchangeability.py      30      0   100%
 tests\test_grantham.py                          25      0   100%
-tests\test_koshi_goldstein.py                  108     50    54%
+tests\test_kolaskar.py                          26      0   100%
+tests\test_koshi_goldstein.py                  108      0   100%
 tests\test_miyata.py                            25      0   100%
 tests\test_pard.py                               3      0   100%
-tests\test_raw_python_dictionaries.py           20     11    45%
+tests\test_raw_python_dictionaries.py           22      0   100%
 tests\test_sneath.py                            21      0   100%
-unit_tests_mypy.py                               5      5     0%
-unit_tests_simple.py                             5      5     0%
+unit_tests_simple.py                             5      0   100%
 ----------------------------------------------------------------
-TOTAL                                          457    129    72%
+TOTAL                                          493      4    99%
 ```
 
 #### pytest
 ```
 platform win32 -- Python 3.11.1, pytest-7.2.0, pluggy-1.0.0
 plugins: anyio-3.6.2, mypy-0.10.3
-collected 14 items
+collected 15 items
 
-tests\test_epstein.py .                                                  [  7%]
-tests\test_experimental_exchangeability.py .                             [ 14%]
-tests\test_grantham.py .                                                 [ 21%]
-tests\test_koshi_goldstein.py .......                                    [ 71%]
-tests\test_miyata.py .                                                   [ 78%]
-tests\test_pard.py .                                                     [ 85%]
-tests\test_raw_python_dictionaries.py .                                  [ 92%]
-tests\test_sneath.py .                                                   [100%]
+tests\test_epstein.py .                                              [  6%] 
+tests\test_experimental_exchangeability.py .                         [ 13%] 
+tests\test_grantham.py .                                             [ 20%] 
+tests\test_kolaskar.py .                                             [ 26%] 
+tests\test_koshi_goldstein.py .......                                [ 73%]
+tests\test_miyata.py .                                               [ 80%] 
+tests\test_pard.py .                                                 [ 86%] 
+tests\test_raw_python_dictionaries.py .                              [ 93%]
+tests\test_sneath.py .                                               [100%]
+
+=========================== 15 passed in 0.06s ===========================
 
-============================= 14 passed in 0.06s ==============================
 ```
 
 #### mypy detail
 ```
-=============================== mypy ===============================
-Success: no issues found in 20 source files
+================================== mypy ==================================
+Success: no issues found in 22 source files
 ```
 
 ### Useful links:
 - [Corresponding GitHub repository](https://github.com/MICS-Lab/pard)
 - [Corresponding PyPI page](https://pypi.org/project/pard/)
 
 
 ### Citation
 If you use this software, please cite it as below.
 
 - APA:
 
 `
 Lhotte, R. & Taupin, J. (2022).
-Physicochemical Amino acid Replacement Distances (PARD) package (Version 0.4.0.1) [Computer software].
+Physicochemical Amino acid Replacement Distances (PARD) package (Version 0.5.0.0) [Computer software].
 https://doi.org/10.5281/zenodo.7013169
 `
 
 - BibTeX:
 
 ```
 @software{lhotte_pard_2022,
     author = {Lhotte, Romain and Taupin, Jean-Luc},
     doi = {10.5281/zenodo.7013169},
     month = {8},
     title = {{Physicochemical Amino acid Replacement Distances (PARD) package}},
-    version = {0.4.0.1},
+    version = {0.5.0.0},
     year = {2022}
 }
 ```
 
 
 ### References
 - [1] Grantham, R., 1974. Amino acid difference formula to help explain protein evolution. science, 185(4154),
```

