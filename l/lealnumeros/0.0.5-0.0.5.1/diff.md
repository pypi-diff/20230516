# Comparing `tmp/lealnumeros-0.0.5.tar.gz` & `tmp/lealnumeros-0.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lealnumeros-0.0.5.tar", last modified: Tue May 16 22:21:31 2023, max compression
+gzip compressed data, was "lealnumeros-0.0.5.1.tar", last modified: Tue May 16 22:26:17 2023, max compression
```

## Comparing `lealnumeros-0.0.5.tar` & `lealnumeros-0.0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 22:21:31.305223 lealnumeros-0.0.5/
--rw-rw-rw-   0        0        0     1098 2023-05-14 20:25:14.000000 lealnumeros-0.0.5/LICENCE
--rw-rw-rw-   0        0        0     1431 2023-05-16 22:21:31.304223 lealnumeros-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1081 2023-05-16 05:05:38.000000 lealnumeros-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 22:21:31.261248 lealnumeros-0.0.5/lealNumeros/
--rw-rw-rw-   0        0        0       32 2023-05-14 20:13:46.000000 lealnumeros-0.0.5/lealNumeros/__init__.py
--rw-rw-rw-   0        0        0     4021 2023-05-16 22:19:27.000000 lealnumeros-0.0.5/lealNumeros/main.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:21:31.302224 lealnumeros-0.0.5/lealnumeros.egg-info/
--rw-rw-rw-   0        0        0     1431 2023-05-16 22:21:31.000000 lealnumeros-0.0.5/lealnumeros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-16 22:21:31.000000 lealnumeros-0.0.5/lealnumeros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 22:21:31.000000 lealnumeros-0.0.5/lealnumeros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-16 22:21:31.000000 lealnumeros-0.0.5/lealnumeros.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-16 22:21:31.000000 lealnumeros-0.0.5/lealnumeros.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 22:21:31.305223 lealnumeros-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-05-16 22:20:54.000000 lealnumeros-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:26:17.745241 lealnumeros-0.0.5.1/
+-rw-rw-rw-   0        0        0     1098 2023-05-14 20:25:14.000000 lealnumeros-0.0.5.1/LICENCE
+-rw-rw-rw-   0        0        0     1628 2023-05-16 22:26:17.744226 lealnumeros-0.0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1272 2023-05-16 22:23:30.000000 lealnumeros-0.0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 22:26:17.722239 lealnumeros-0.0.5.1/lealNumeros/
+-rw-rw-rw-   0        0        0       32 2023-05-14 20:13:46.000000 lealnumeros-0.0.5.1/lealNumeros/__init__.py
+-rw-rw-rw-   0        0        0     4021 2023-05-16 22:19:27.000000 lealnumeros-0.0.5.1/lealNumeros/main.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:26:17.742228 lealnumeros-0.0.5.1/lealnumeros.egg-info/
+-rw-rw-rw-   0        0        0     1628 2023-05-16 22:26:17.000000 lealnumeros-0.0.5.1/lealnumeros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-16 22:26:17.000000 lealnumeros-0.0.5.1/lealnumeros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 22:26:17.000000 lealnumeros-0.0.5.1/lealnumeros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-16 22:26:17.000000 lealnumeros-0.0.5.1/lealnumeros.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-16 22:26:17.000000 lealnumeros-0.0.5.1/lealnumeros.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 22:26:17.746225 lealnumeros-0.0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      519 2023-05-16 22:25:57.000000 lealnumeros-0.0.5.1/setup.py
```

### Comparing `lealnumeros-0.0.5/LICENCE` & `lealnumeros-0.0.5.1/LICENCE`

 * *Files identical despite different names*

### Comparing `lealnumeros-0.0.5/PKG-INFO` & `lealnumeros-0.0.5.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 Metadata-Version: 2.1
 Name: lealnumeros
-Version: 0.0.5
+Version: 0.0.5.1
 Summary: Trabalhe com formatação de números de uma maneira rápido e fácil.
 Author: José Rodolfo
 Author-email: silvaleal.ctt@gmail.com
 License: MIT License
 Keywords: lealnumeros
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 Trabalhe com formataÃ§Ã£o de nÃºmeros de uma maneira rÃ¡pido e fÃ¡cil.
 
 ```python
-
 from lealNumeros import LealNumerosAPI
 
 # Colocar pontuaÃ§Ã£o nos nÃºmeros
 print(LealNumerosAPI.numerosPontuados(10000))
 # Saida: 10.000
 
-# Colocar simbolos  
+# Colocar simbolos      
         # Formatos disponÃ­veis: (8) Mil
         #                           M (MilhÃ£o)
         #                           B (BilhÃ£o)
         #                           T (TrilhÃ£o)
         #                           Q (QuadrilhÃ£o)
         #                           Qi (QuintilhÃ£o)
         #                           Sx (SextilhÃ£o)
         #                           Sp (SeptilhÃ£o)
 print(LealNumerosAPI.numerosSimbolos(10000))
 # Saida: 10Mil
 
 # Escrever o nome do nÃºmero (PT-BR)
-print(LealNumerosAPI.numerosNome(10000))
+print(LealNumerosAPI.numerosNome(100))
 # Saida: Dez mil
 
 # Escrever diferenÃ§as entre nÃºmeros
-print(LealNumerosAPI.numerosDiferenca(10, 5))
-ou
-print(LealNumerosAPI.numerosDiferenca(5, 10))
+print(LealNumerosAPI.numerosDiferenca(5, 5))
 # Saida: 5
+
+# Escrever diferenÃ§as entre dias
+print(f'{LealNumerosAPI.dataDiferenca(1, 2, 2023)} Dias')
+
+# Calculadora
+conta = input('Qual a conta matemÃ¡tica? (ex.: 10 + 5)')
+resultado = LealNumerosAPI.numerosCalculadora(conta)
+print(resultado)
 ```
 
 ---
 
 Discord: silvaleal#7458
 Suporte: [https://discord.gg/394ChkbKrt](https://discord.gg/394ChkbKrt)
```

### Comparing `lealnumeros-0.0.5/lealNumeros/main.py` & `lealnumeros-0.0.5.1/lealNumeros/main.py`

 * *Files identical despite different names*

### Comparing `lealnumeros-0.0.5/lealnumeros.egg-info/PKG-INFO` & `lealnumeros-0.0.5.1/lealnumeros.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 Metadata-Version: 2.1
 Name: lealnumeros
-Version: 0.0.5
+Version: 0.0.5.1
 Summary: Trabalhe com formatação de números de uma maneira rápido e fácil.
 Author: José Rodolfo
 Author-email: silvaleal.ctt@gmail.com
 License: MIT License
 Keywords: lealnumeros
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 Trabalhe com formataÃ§Ã£o de nÃºmeros de uma maneira rÃ¡pido e fÃ¡cil.
 
 ```python
-
 from lealNumeros import LealNumerosAPI
 
 # Colocar pontuaÃ§Ã£o nos nÃºmeros
 print(LealNumerosAPI.numerosPontuados(10000))
 # Saida: 10.000
 
-# Colocar simbolos  
+# Colocar simbolos      
         # Formatos disponÃ­veis: (8) Mil
         #                           M (MilhÃ£o)
         #                           B (BilhÃ£o)
         #                           T (TrilhÃ£o)
         #                           Q (QuadrilhÃ£o)
         #                           Qi (QuintilhÃ£o)
         #                           Sx (SextilhÃ£o)
         #                           Sp (SeptilhÃ£o)
 print(LealNumerosAPI.numerosSimbolos(10000))
 # Saida: 10Mil
 
 # Escrever o nome do nÃºmero (PT-BR)
-print(LealNumerosAPI.numerosNome(10000))
+print(LealNumerosAPI.numerosNome(100))
 # Saida: Dez mil
 
 # Escrever diferenÃ§as entre nÃºmeros
-print(LealNumerosAPI.numerosDiferenca(10, 5))
-ou
-print(LealNumerosAPI.numerosDiferenca(5, 10))
+print(LealNumerosAPI.numerosDiferenca(5, 5))
 # Saida: 5
+
+# Escrever diferenÃ§as entre dias
+print(f'{LealNumerosAPI.dataDiferenca(1, 2, 2023)} Dias')
+
+# Calculadora
+conta = input('Qual a conta matemÃ¡tica? (ex.: 10 + 5)')
+resultado = LealNumerosAPI.numerosCalculadora(conta)
+print(resultado)
 ```
 
 ---
 
 Discord: silvaleal#7458
 Suporte: [https://discord.gg/394ChkbKrt](https://discord.gg/394ChkbKrt)
```

### Comparing `lealnumeros-0.0.5/setup.py` & `lealnumeros-0.0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='lealnumeros',
-    version='0.0.5',
+    version='0.0.5.1',
     license='MIT License',
     author='José Rodolfo',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='silvaleal.ctt@gmail.com',
     keywords='lealnumeros',
     description=u'Trabalhe com formatação de números de uma maneira rápido e fácil.',
```

