# Comparing `tmp/libgal-0.0.4.tar.gz` & `tmp/libgal-0.0.5.tar.gz`

## Comparing `libgal-0.0.4.tar` & `libgal-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 libgal-0.0.4/__init__.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 libgal-0.0.4/libgal.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 libgal-0.0.4/libgal.py.bak
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 libgal-0.0.4/pyproject.toml.bak
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 libgal-0.0.4/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libgal-0.0.4/libgal_package/libgal/__init__.py.bak
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 libgal-0.0.4/libgal_package/libgal/libgal.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 libgal-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0    12096 2020-02-02 00:00:00.000000 libgal-0.0.4/README.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 libgal-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    13724 2020-02-02 00:00:00.000000 libgal-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 libgal-0.0.5/__init__.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 libgal-0.0.5/libgal.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 libgal-0.0.5/libgal.py.bak
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 libgal-0.0.5/pyproject.toml.bak
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 libgal-0.0.5/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libgal-0.0.5/libgal_package/libgal/__init__.py.bak
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 libgal-0.0.5/libgal_package/libgal/libgal.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 libgal-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 libgal-0.0.5/README.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 libgal-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    13662 2020-02-02 00:00:00.000000 libgal-0.0.5/PKG-INFO
```

### Comparing `libgal-0.0.4/libgal.py` & `libgal-0.0.5/libgal.py`

 * *Files identical despite different names*

### Comparing `libgal-0.0.4/libgal.py.bak` & `libgal-0.0.5/libgal.py.bak`

 * *Files identical despite different names*

### Comparing `libgal-0.0.4/pyproject.toml.bak` & `libgal-0.0.5/pyproject.toml.bak`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "libgal"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Jean Manuel González Mejía", email="ebrainding@gmail.com" },
 ]
 
 license = { file = "LICENSE.txt" }
 
 description = "Librería para agilizar el desarrollo de nuestros programadores en el Banco Galicia"
```

### Comparing `libgal-0.0.4/libgal_package/libgal/libgal.py` & `libgal-0.0.5/libgal_package/libgal/libgal.py`

 * *Files identical despite different names*

### Comparing `libgal-0.0.4/LICENSE.txt` & `libgal-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libgal-0.0.4/README.md` & `libgal-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,16 @@
 
 ```sh
 #SECRETS
 USERNAME = usuario@correo.com
 PASSWORD = contraseña
 
 #CONFIGMAP
-API_PREDICT=https://dwos-dataanalytics.bancogalicia.com.ar/predict
-API_AUDIENCIAS=https://dwos-dataanalytics.bancogalicia.com.ar/audiencias
+API_PREDICT=https://url.com/predict
+API_AUDIENCIAS=https://url.com/audiencias
 CANT_POST=10 #Cantidad de últimos posts a descargar
 ```
 
 Es importante mencionar que al momento de desplegar nuestra aplicación no se debe subir este archivo “.env” ya que solo es para ejecuciones y pruebas en modo local que simula estar en openshift.  
 
 Ahora bien, para poder usar estas variables dentro de nuestro código solo será necesario importar la librería LIBGAL e instanciar en una variable la función VARIABLES_ENTORNO y así poder acceder a las variables de entorno mediante la misma, tal cómo se muestra en el siguiente ejemplo:
```

#### html2text {}

```diff
@@ -38,16 +38,15 @@
 serÃ¡ necesario crear un archivo de texto cuyo nombre y extensiÃ³n serÃ¡
 â.envâ. Por defecto esta librerÃ­a tomarÃ¡ el archivo â.envâ que se
 encuentra ubicado en la raÃ­z de nuestro ejecutable python. Dentro de este
 mismo archivo â.envâ podemos especificar todas las variables secrets y
 configmap que utilizarÃ¡ nuestra aplicaciÃ³n, tal como se muestra en el
 siguiente ejemplo:
 ```sh #SECRETS USERNAME = usuario@correo.com PASSWORD = contraseÃ±a #CONFIGMAP
-API_PREDICT=https://dwos-dataanalytics.bancogalicia.com.ar/predict
-API_AUDIENCIAS=https://dwos-dataanalytics.bancogalicia.com.ar/audiencias
+API_PREDICT=https://url.com/predict API_AUDIENCIAS=https://url.com/audiencias
 CANT_POST=10 #Cantidad de Ãºltimos posts a descargar ``` Es importante
 mencionar que al momento de desplegar nuestra aplicaciÃ³n no se debe subir este
 archivo â.envâ ya que solo es para ejecuciones y pruebas en modo local que
 simula estar en openshift. Ahora bien, para poder usar estas variables dentro
 de nuestro cÃ³digo solo serÃ¡ necesario importar la librerÃ­a LIBGAL e
 instanciar en una variable la funciÃ³n VARIABLES_ENTORNO y asÃ­ poder acceder a
 las variables de entorno mediante la misma, tal cÃ³mo se muestra en el
```

### Comparing `libgal-0.0.4/pyproject.toml` & `libgal-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "libgal"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Jean Manuel González Mejía", email="ebrainding@gmail.com" },
 ]
 
 license = { file = "LICENSE.txt" }
 
 description = "Librería para agilizar el desarrollo de nuestros programadores en el Banco Galicia"
```

### Comparing `libgal-0.0.4/PKG-INFO` & `libgal-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libgal
-Version: 0.0.4
+Version: 0.0.5
 Summary: Librería para agilizar el desarrollo de nuestros programadores en el Banco Galicia
 Project-URL: Homepage, https://github.com/Banco-Galicia/libgal
 Project-URL: Bug Tracker, https://github.com/Banco-Galicia/libgal/issues
 Author-email: Jean Manuel González Mejía <ebrainding@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 JEAN MANUEL GONZÁLEZ MEJÍA
@@ -145,16 +145,16 @@
 
 ```sh
 #SECRETS
 USERNAME = usuario@correo.com
 PASSWORD = contraseña
 
 #CONFIGMAP
-API_PREDICT=https://dwos-dataanalytics.bancogalicia.com.ar/predict
-API_AUDIENCIAS=https://dwos-dataanalytics.bancogalicia.com.ar/audiencias
+API_PREDICT=https://url.com/predict
+API_AUDIENCIAS=https://url.com/audiencias
 CANT_POST=10 #Cantidad de últimos posts a descargar
 ```
 
 Es importante mencionar que al momento de desplegar nuestra aplicación no se debe subir este archivo “.env” ya que solo es para ejecuciones y pruebas en modo local que simula estar en openshift.  
 
 Ahora bien, para poder usar estas variables dentro de nuestro código solo será necesario importar la librería LIBGAL e instanciar en una variable la función VARIABLES_ENTORNO y así poder acceder a las variables de entorno mediante la misma, tal cómo se muestra en el siguiente ejemplo:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libgal Version: 0.0.4 Summary: LibrerÃ­a para
+Metadata-Version: 2.1 Name: libgal Version: 0.0.5 Summary: LibrerÃ­a para
 agilizar el desarrollo de nuestros programadores en el Banco Galicia Project-
 URL: Homepage, https://github.com/Banco-Galicia/libgal Project-URL: Bug
 Tracker, https://github.com/Banco-Galicia/libgal/issues Author-email: Jean
 Manuel GonzÃ¡lez MejÃ­a
 gmail.com> License: MIT License Copyright (c) 2022 JEAN MANUEL GONZÃLEZ MEJÃA
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
@@ -62,16 +62,15 @@
 serÃ¡ necesario crear un archivo de texto cuyo nombre y extensiÃ³n serÃ¡
 â.envâ. Por defecto esta librerÃ­a tomarÃ¡ el archivo â.envâ que se
 encuentra ubicado en la raÃ­z de nuestro ejecutable python. Dentro de este
 mismo archivo â.envâ podemos especificar todas las variables secrets y
 configmap que utilizarÃ¡ nuestra aplicaciÃ³n, tal como se muestra en el
 siguiente ejemplo:
 ```sh #SECRETS USERNAME = usuario@correo.com PASSWORD = contraseÃ±a #CONFIGMAP
-API_PREDICT=https://dwos-dataanalytics.bancogalicia.com.ar/predict
-API_AUDIENCIAS=https://dwos-dataanalytics.bancogalicia.com.ar/audiencias
+API_PREDICT=https://url.com/predict API_AUDIENCIAS=https://url.com/audiencias
 CANT_POST=10 #Cantidad de Ãºltimos posts a descargar ``` Es importante
 mencionar que al momento de desplegar nuestra aplicaciÃ³n no se debe subir este
 archivo â.envâ ya que solo es para ejecuciones y pruebas en modo local que
 simula estar en openshift. Ahora bien, para poder usar estas variables dentro
 de nuestro cÃ³digo solo serÃ¡ necesario importar la librerÃ­a LIBGAL e
 instanciar en una variable la funciÃ³n VARIABLES_ENTORNO y asÃ­ poder acceder a
 las variables de entorno mediante la misma, tal cÃ³mo se muestra en el
```

