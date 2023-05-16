# Comparing `tmp/ifd_python-10.0.1.tar.gz` & `tmp/ifd_python-10.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifd_python-10.0.1.tar", max compression
+gzip compressed data, was "ifd_python-10.1.tar", max compression
```

## Comparing `ifd_python-10.0.1.tar` & `ifd_python-10.1.tar`

### file list

```diff
@@ -1,31 +1,34 @@
--rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-10.0.1/LICENSE
--rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-10.0.1/README.md
--rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-10.0.1/ifd/__init__.py
--rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-10.0.1/ifd/entities/Abstract/ADetection.py
--rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-10.0.1/ifd/entities/Abstract/__init__.py
--rw-r--r--   0        0        0      734 2023-04-19 13:21:34.036921 ifd_python-10.0.1/ifd/entities/Classification.py
--rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-10.0.1/ifd/entities/Couleur.py
--rw-r--r--   0        0        0      707 2023-04-13 09:26:25.358120 ifd_python-10.0.1/ifd/entities/Detection.py
--rw-r--r--   0        0        0     2303 2023-04-19 08:19:41.294208 ifd_python-10.0.1/ifd/entities/Image.py
--rw-r--r--   0        0        0     1428 2023-05-05 12:08:36.910162 ifd_python-10.0.1/ifd/entities/LogResult.py
--rw-r--r--   0        0        0      477 2023-04-13 09:26:25.358120 ifd_python-10.0.1/ifd/entities/Modele.py
--rw-r--r--   0        0        0      794 2023-05-04 14:04:45.639232 ifd_python-10.0.1/ifd/entities/OCR.py
--rw-r--r--   0        0        0      529 2023-05-04 14:04:45.639232 ifd_python-10.0.1/ifd/entities/RabbitMqMessage.py
--rw-r--r--   0        0        0      709 2023-04-19 08:27:21.531854 ifd_python-10.0.1/ifd/entities/Tag.py
--rw-r--r--   0        0        0      423 2023-05-04 07:26:22.716168 ifd_python-10.0.1/ifd/entities/Ticket.py
--rw-r--r--   0        0        0      290 2023-05-03 16:41:43.255646 ifd_python-10.0.1/ifd/entities/__init__.py
--rw-r--r--   0        0        0      717 2023-04-13 09:26:25.358120 ifd_python-10.0.1/ifd/entities/bbox.py
--rw-r--r--   0        0        0     2161 2023-05-04 14:04:45.639232 ifd_python-10.0.1/ifd/repository/AmqpImageRepository.py
--rw-r--r--   0        0        0     2215 2023-05-05 14:06:59.670941 ifd_python-10.0.1/ifd/repository/RestTicketRepository.py
--rw-r--r--   0        0        0      986 2023-05-05 15:52:24.410579 ifd_python-10.0.1/ifd/repository/SqlLogRepository.py
--rw-r--r--   0        0        0     2009 2023-05-05 15:52:24.410579 ifd_python-10.0.1/ifd/repository/SqlTicketRepository.py
--rw-r--r--   0        0        0      210 2023-05-04 14:04:45.639232 ifd_python-10.0.1/ifd/repository/__init__.py
--rw-r--r--   0        0        0      940 2023-05-05 15:52:24.410579 ifd_python-10.0.1/ifd/repository/abstract/AbsSqlRepository.py
--rw-r--r--   0        0        0       46 2023-05-04 14:04:45.639232 ifd_python-10.0.1/ifd/repository/abstract/__init__.py
--rw-r--r--   0        0        0     1082 2023-05-05 15:52:24.410579 ifd_python-10.0.1/ifd/spec.py
--rw-r--r--   0        0        0      526 2023-04-19 08:19:41.298208 ifd_python-10.0.1/ifd/tools.py
--rw-r--r--   0        0        0      131 2023-04-14 12:36:19.030168 ifd_python-10.0.1/ifd/usecase/Interfaces/IFonction.py
--rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-10.0.1/ifd/usecase/Interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 15:07:22.275577 ifd_python-10.0.1/ifd/usecase/__init__.py
--rw-r--r--   0        0        0      407 2023-05-09 15:07:31.719698 ifd_python-10.0.1/pyproject.toml
--rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 ifd_python-10.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-10.1/LICENSE
+-rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-10.1/README.md
+-rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-10.1/ifd/__init__.py
+-rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-10.1/ifd/entities/Abstract/ADetection.py
+-rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-10.1/ifd/entities/Abstract/__init__.py
+-rw-r--r--   0        0        0      630 2023-05-16 09:20:45.247803 ifd_python-10.1/ifd/entities/BodyTicket.py
+-rw-r--r--   0        0        0      734 2023-04-19 13:21:34.036921 ifd_python-10.1/ifd/entities/Classification.py
+-rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-10.1/ifd/entities/Couleur.py
+-rw-r--r--   0        0        0      707 2023-04-13 09:26:25.358120 ifd_python-10.1/ifd/entities/Detection.py
+-rw-r--r--   0        0        0     2303 2023-04-19 08:19:41.294208 ifd_python-10.1/ifd/entities/Image.py
+-rw-r--r--   0        0        0      730 2023-05-16 09:20:45.247803 ifd_python-10.1/ifd/entities/Intervention.py
+-rw-r--r--   0        0        0     1428 2023-05-05 12:08:36.910162 ifd_python-10.1/ifd/entities/LogResult.py
+-rw-r--r--   0        0        0      741 2023-05-16 09:20:45.247803 ifd_python-10.1/ifd/entities/Malfacon.py
+-rw-r--r--   0        0        0      477 2023-04-13 09:26:25.358120 ifd_python-10.1/ifd/entities/Modele.py
+-rw-r--r--   0        0        0      794 2023-05-04 14:04:45.639232 ifd_python-10.1/ifd/entities/OCR.py
+-rw-r--r--   0        0        0      529 2023-05-04 14:04:45.639232 ifd_python-10.1/ifd/entities/RabbitMqMessage.py
+-rw-r--r--   0        0        0     1033 2023-05-16 09:20:45.247803 ifd_python-10.1/ifd/entities/Tag.py
+-rw-r--r--   0        0        0      423 2023-05-04 07:26:22.716168 ifd_python-10.1/ifd/entities/Ticket.py
+-rw-r--r--   0        0        0      290 2023-05-03 16:41:43.255646 ifd_python-10.1/ifd/entities/__init__.py
+-rw-r--r--   0        0        0      717 2023-04-13 09:26:25.358120 ifd_python-10.1/ifd/entities/bbox.py
+-rw-r--r--   0        0        0     2161 2023-05-04 14:04:45.639232 ifd_python-10.1/ifd/repository/AmqpImageRepository.py
+-rw-r--r--   0        0        0     2215 2023-05-05 14:06:59.670941 ifd_python-10.1/ifd/repository/RestTicketRepository.py
+-rw-r--r--   0        0        0      986 2023-05-05 15:52:24.410579 ifd_python-10.1/ifd/repository/SqlLogRepository.py
+-rw-r--r--   0        0        0     2009 2023-05-05 15:52:24.410579 ifd_python-10.1/ifd/repository/SqlTicketRepository.py
+-rw-r--r--   0        0        0      210 2023-05-04 14:04:45.639232 ifd_python-10.1/ifd/repository/__init__.py
+-rw-r--r--   0        0        0      940 2023-05-05 15:52:24.410579 ifd_python-10.1/ifd/repository/abstract/AbsSqlRepository.py
+-rw-r--r--   0        0        0       46 2023-05-04 14:04:45.639232 ifd_python-10.1/ifd/repository/abstract/__init__.py
+-rw-r--r--   0        0        0     1082 2023-05-05 15:52:24.410579 ifd_python-10.1/ifd/spec.py
+-rw-r--r--   0        0        0      526 2023-04-19 08:19:41.298208 ifd_python-10.1/ifd/tools.py
+-rw-r--r--   0        0        0      131 2023-04-14 12:36:19.030168 ifd_python-10.1/ifd/usecase/Interfaces/IFonction.py
+-rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-10.1/ifd/usecase/Interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 09:20:45.263804 ifd_python-10.1/ifd/usecase/__init__.py
+-rw-r--r--   0        0        0      405 2023-05-16 09:20:54.235916 ifd_python-10.1/pyproject.toml
+-rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 ifd_python-10.1/PKG-INFO
```

### Comparing `ifd_python-10.0.1/LICENSE` & `ifd_python-10.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/README.md` & `ifd_python-10.1/README.md`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/ifd/entities/Abstract/ADetection.py` & `ifd_python-10.1/ifd/entities/Abstract/ADetection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/ifd/entities/Classification.py` & `ifd_python-10.1/ifd/entities/Classification.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/ifd/entities/Detection.py` & `ifd_python-10.1/ifd/entities/Detection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/ifd/entities/Image.py` & `ifd_python-10.1/ifd/entities/Image.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/ifd/entities/LogResult.py` & `ifd_python-10.1/ifd/entities/LogResult.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/ifd/entities/OCR.py` & `ifd_python-10.1/ifd/entities/OCR.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/ifd/entities/RabbitMqMessage.py` & `ifd_python-10.1/ifd/entities/RabbitMqMessage.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/ifd/entities/bbox.py` & `ifd_python-10.1/ifd/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/ifd/repository/AmqpImageRepository.py` & `ifd_python-10.1/ifd/repository/AmqpImageRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/ifd/repository/RestTicketRepository.py` & `ifd_python-10.1/ifd/repository/RestTicketRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/ifd/repository/SqlLogRepository.py` & `ifd_python-10.1/ifd/repository/SqlLogRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/ifd/repository/SqlTicketRepository.py` & `ifd_python-10.1/ifd/repository/SqlTicketRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/ifd/repository/abstract/AbsSqlRepository.py` & `ifd_python-10.1/ifd/repository/abstract/AbsSqlRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/ifd/spec.py` & `ifd_python-10.1/ifd/spec.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/ifd/tools.py` & `ifd_python-10.1/ifd/tools.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.0.1/PKG-INFO` & `ifd_python-10.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifd-python
-Version: 10.0.1
+Version: 10.1
 Summary: 
 Author: Antonin Lemoine
 Author-email: antonin.lemoine@altitudeinfra.fr
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

