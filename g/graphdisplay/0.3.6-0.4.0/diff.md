# Comparing `tmp/graphdisplay-0.3.6.tar.gz` & `tmp/graphdisplay-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdisplay-0.3.6.tar", last modified: Wed May 10 08:25:33 2023, max compression
+gzip compressed data, was "graphdisplay-0.4.0.tar", last modified: Tue May 16 18:18:49 2023, max compression
```

## Comparing `graphdisplay-0.3.6.tar` & `graphdisplay-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 08:25:33.328259 graphdisplay-0.3.6/
--rw-rw-rw-   0        0        0     5408 2023-05-10 08:25:33.328259 graphdisplay-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     4753 2023-05-06 17:15:34.000000 graphdisplay-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 08:25:33.312301 graphdisplay-0.3.6/graphdisplay/
--rw-rw-rw-   0        0        0       60 2023-05-03 20:40:03.000000 graphdisplay-0.3.6/graphdisplay/__init__.py
--rw-rw-rw-   0        0        0     4209 2023-05-09 05:43:15.000000 graphdisplay-0.3.6/graphdisplay/general_config.py
--rw-rw-rw-   0        0        0    17455 2023-05-07 10:31:30.000000 graphdisplay-0.3.6/graphdisplay/graph.py
--rw-rw-rw-   0        0        0    18618 2023-05-10 08:25:15.000000 graphdisplay-0.3.6/graphdisplay/graphdisplay.py
--rw-rw-rw-   0        0        0     7145 2023-05-09 06:25:44.000000 graphdisplay-0.3.6/graphdisplay/json_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:25:33.326264 graphdisplay-0.3.6/graphdisplay/store/
--rw-rw-rw-   0        0        0        0 2023-05-06 17:02:49.000000 graphdisplay-0.3.6/graphdisplay/store/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:25:33.324270 graphdisplay-0.3.6/graphdisplay.egg-info/
--rw-rw-rw-   0        0        0     5408 2023-05-10 08:25:33.000000 graphdisplay-0.3.6/graphdisplay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-05-10 08:25:33.000000 graphdisplay-0.3.6/graphdisplay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 08:25:33.000000 graphdisplay-0.3.6/graphdisplay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-10 08:25:33.000000 graphdisplay-0.3.6/graphdisplay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 08:25:33.329256 graphdisplay-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1322 2023-05-10 08:25:31.000000 graphdisplay-0.3.6/setup.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-16 18:18:49.782601 graphdisplay-0.4.0/
+-rw-rw-r--   0 beto      (1000) beto      (1000)     6167 2023-05-16 18:18:49.782601 graphdisplay-0.4.0/PKG-INFO
+-rw-rw-r--   0 beto      (1000) beto      (1000)     5529 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/README.md
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-16 18:18:49.778601 graphdisplay-0.4.0/graphdisplay/
+-rw-rw-r--   0 beto      (1000) beto      (1000)       98 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/graphdisplay/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     1856 2023-05-16 17:19:06.000000 graphdisplay-0.4.0/graphdisplay/about_win_manager.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     4154 2023-05-16 18:18:44.000000 graphdisplay-0.4.0/graphdisplay/general_config.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-16 18:18:49.778601 graphdisplay-0.4.0/graphdisplay/graphs/
+-rw-rw-r--   0 beto      (1000) beto      (1000)       24 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/graphdisplay/graphs/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)    17021 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/graphdisplay/graphs/graph.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     6977 2023-05-09 11:25:49.000000 graphdisplay-0.4.0/graphdisplay/json_manager.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)    27026 2023-05-16 15:34:14.000000 graphdisplay-0.4.0/graphdisplay/main.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-16 18:18:49.778601 graphdisplay-0.4.0/graphdisplay/store/
+-rw-rw-r--   0 beto      (1000) beto      (1000)        0 2023-05-06 20:46:34.000000 graphdisplay-0.4.0/graphdisplay/store/__init__.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-16 18:18:49.782601 graphdisplay-0.4.0/graphdisplay/trees/
+-rw-rw-r--   0 beto      (1000) beto      (1000)       87 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/graphdisplay/trees/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     3524 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/graphdisplay/trees/auto_balance_tree.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     3107 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/graphdisplay/trees/binary_search_tree.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     5510 2023-05-14 22:04:49.000000 graphdisplay-0.4.0/graphdisplay/trees/binary_tree.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-05-16 18:18:49.778601 graphdisplay-0.4.0/graphdisplay.egg-info/
+-rw-rw-r--   0 beto      (1000) beto      (1000)     6167 2023-05-16 18:18:49.000000 graphdisplay-0.4.0/graphdisplay.egg-info/PKG-INFO
+-rw-rw-r--   0 beto      (1000) beto      (1000)      540 2023-05-16 18:18:49.000000 graphdisplay-0.4.0/graphdisplay.egg-info/SOURCES.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)        1 2023-05-16 18:18:49.000000 graphdisplay-0.4.0/graphdisplay.egg-info/dependency_links.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)       13 2023-05-16 18:18:49.000000 graphdisplay-0.4.0/graphdisplay.egg-info/top_level.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)       38 2023-05-16 18:18:49.782601 graphdisplay-0.4.0/setup.cfg
+-rw-rw-r--   0 beto      (1000) beto      (1000)     1323 2023-05-16 16:42:51.000000 graphdisplay-0.4.0/setup.py
```

### Comparing `graphdisplay-0.3.6/PKG-INFO` & `graphdisplay-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,96 +1,86 @@
-Metadata-Version: 2.1
-Name: graphdisplay
-Version: 0.3.6
-Summary: Librería para representar visualmente grafos de tipo diccionario
-Home-page: https://github.com/seniorbeto
-Author: Alberto Penas Díaz
-Author-email: albertopenasdiaz@gmail.com
-License: MIT
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-
-# graphdisplay
-
-## Resumen
-
-graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos a los alumnos de Estructuras de Datos y Algoritmos. 
-Actualmente solo soporta la visualización de grafos implementados a través de un diccionario, tal y como se aportan como código base en la asignatura. 
-
-## ¿Quieres contribuir?
-
-Este es un proyecto de código abierto hecho por y para estudiantes así que cualquier ayuda, comentario o sugerencia es bienvenido. La mejor manera de contribuir es añadir los bugs que os encontréis 
-en el apartado de Issues pero también estoy completamente abierto a responder cualquier duda o ayuda desde mi correo personal (disponible en mi perfil de github). ¡Muchas gracias de antemano!
-
-## Método de uso 
-
-Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
-tkinter y math (que muchas veces vienen instaladas por defecto en python). 
-
-Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. Una vez hecho esto, se debe instanciar un grafo de tipo diccionario
-para finalmente introducirlo como argumento al instanciar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón 
-para una mejor visualización. **Al desplazar los vértices por la pantalla y fijar su posición, si se cierra la ventana y se vuelve a abrir, el grafo seguirá con la forma con la que se ha movido
-antes.**. Cabe destacar que, únicamente es necesario especificar como argumento el grafo que se quiere representar pero además hay otros ajustes que pueden ser útiles a la hora de mostrar 
-grafos grandes y complejos:
-+ graph: es el objeto de tipo grafo que se va a representar **ES MUY IMPORTANTE** que el grafo que se introduce como argumento sea el implementado en base al código base de la asignatura. Si alguno
-de los atributos cambiase de nombre, el programa no funcionaría correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA) o utilizar la 
-implementación de grafos que viene por defecto con el paquete.
-+ node_radius: el radio de cada vértice del grafo, por defecto es 40 y puede tomar cualquier valor entero entre 10 y 100
-+ scr_width: el tamaño en píxeles del ancho de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
-+ scr_width: el tamaño en píxeles de la altura de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
-
-Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
-```python
-g = Graph([1, 2, 3])
-g.addEdge(1, 2)
-g.addEdge(2, 3)
-
-# Para representar el grafo con todos los valores por defecto
-GraphGUI(g)
-
-# Para ajustar el radio de los nodos a 32, el ancho y largo de la pantalla a 700
-GraphGUI(g, 32, 700, 700)
-
-# Para ajustar únicamente el ancho de la pantalla a 200 píxeles
-GraphGUI(g, scr_width=200)
-```
-
-Además, también es posible generar este tipo de grafos a través de la librería. Importándolo con `from graphdisplay import Graph`, se puede instanciar un objeto de tipo Graph, pasándole como
-argumento una lista de los vértices del grafo para después, añadirle las aristas con el método `add_edge`, con los vértices que conecta la arista además del valor/coste de la arista.
-
-## Ejemplo de uso
-
-Para instanciar un grafo de tipo diccionario, se debe hacer de la siguiente manera: 
-
-```python
-labels = ['A', 'B', 'C', 'D', 'E']
-g = Graph(labels)
-
-# Now, we add the edges
-g.addEdge('A', 'C', 12)  # A->(12)C
-g.addEdge('A', 'D', 60)  # A->(60)D
-g.addEdge('B', 'A', 10)  # B->(10)A
-g.addEdge('C', 'B', 20)  # C->(20)B
-g.addEdge('C', 'D', 32)  # C->(32)D
-g.addEdge('E', 'A', 7)   # E->(7)A
-g.addEdge('A', 'E', 50)  # A->(50)E
-```
-
-Si queremos mostrar la pantalla, basta con instanciar un objeto de tipo GraphGUI, pasándole como argumento el grafo que queremos mostrar: 
-
-```python
-    GraphGUI(g)
-```
-Y nos mostrará la ventana:
-
-<img src="https://user-images.githubusercontent.com/94072018/236611009-de477dd9-d2dd-4247-80fa-dfc3e7a86a4b.png" width="400" height="400">
-
-Sabiendo cómo instanciar grafos, podemos ahora representar objetos algo más complicados ajustando un poco los parámetros de la instancia GraphGUI. En este caso: `GraphGUI(my_gragph, 30, 1000, 1000)`
-
-<img src="https://user-images.githubusercontent.com/94072018/236611227-2b812c07-7eac-4922-85a5-17cb6e13daea.png" width="550" height="550">
-
+# graphdisplay
+
+## Resumen
+
+graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos a los alumnos de Estructuras de Datos y Algoritmos. 
+Actualmente solo soporta la visualización de grafos implementados a través de un diccionario, tal y como se aportan como código base en la asignatura. 
+
+## ¿Quieres contribuir?
+
+Este es un proyecto de código abierto hecho por y para estudiantes así que cualquier ayuda, comentario o sugerencia es bienvenido. La mejor manera de contribuir es añadir los bugs que os encontréis 
+en el apartado de Issues pero también estoy completamente abierto a responder cualquier duda o ayuda desde mi correo personal (disponible en mi perfil de github). ¡Muchas gracias de antemano!
+
+## Método de uso 
+
+Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
+tkinter y math (que muchas veces vienen instaladas por defecto en python). 
+
+Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. Una vez hecho esto, se debe instanciar un grafo de tipo diccionario
+para finalmente introducirlo como argumento al instanciar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón 
+para una mejor visualización. Cabe destacar que, únicamente es necesario especificar como argumento el grafo que se quiere representar pero además hay otros ajustes que pueden ser útiles a la hora de mostrar 
+grafos grandes y complejos:
++ graph: es el objeto de tipo grafo que se va a representar **ES MUY IMPORTANTE** que el grafo que se introduce como argumento sea el implementado en base al código base de la asignatura. Si alguno
+de los atributos cambiase de nombre, el programa no funcionaría correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA) o utilizar la 
+implementación de grafos que viene por defecto con el paquete.
++ node_radius: el radio de cada vértice del grafo, por defecto es 40 y puede tomar cualquier valor entero entre 10 y 100
++ scr_width: el tamaño en píxeles del ancho de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
++ scr_width: el tamaño en píxeles de la altura de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
++ theme: el tema de la ventana, por defecto es 'brown' y no voy a mencionarlos todos porque hay muchos y me da pereza.
+
+Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
+```python
+g = Graph([1, 2, 3])
+g.addEdge(1, 2)
+g.addEdge(2, 3)
+
+# Para representar el grafo con todos los valores por defecto
+GraphGUI(g)
+
+# Para ajustar el radio de los nodos a 32, el ancho y largo de la pantalla a 700
+GraphGUI(g, 32, 700, 700)
+
+# Para ajustar únicamente el ancho de la pantalla a 200 píxeles
+GraphGUI(g, scr_width=200)
+```
+
+Además, también es posible generar este tipo de grafos a través de la librería. Importándolo con `from graphdisplay import Graph`, se puede instanciar un objeto de tipo Graph, pasándole como
+argumento una lista de los vértices del grafo para después, añadirle las aristas con el método `addEdge`, con los vértices que conecta la arista además del valor/coste de la arista.
+
+## Funcionalidades
+Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
+éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
+instaciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
+Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
+tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón save y nombrando el guardado) para
+después poder cargarlo en cualquier momento.
+## Ejemplo de uso
+
+Para instanciar un grafo de tipo diccionario, se debe hacer de la siguiente manera: 
+
+```python
+labels = ['A', 'B', 'C', 'D', 'E']
+g = Graph(labels)
+
+# Now, we add the edges
+g.addEdge('A', 'C', 12)  # A->(12)C
+g.addEdge('A', 'D', 60)  # A->(60)D
+g.addEdge('B', 'A', 10)  # B->(10)A
+g.addEdge('C', 'B', 20)  # C->(20)B
+g.addEdge('C', 'D', 32)  # C->(32)D
+g.addEdge('E', 'A', 7)   # E->(7)A
+g.addEdge('A', 'E', 50)  # A->(50)E
+```
+
+Si queremos mostrar la pantalla, basta con instanciar un objeto de tipo GraphGUI, pasándole como argumento el grafo que queremos mostrar: 
+
+```python
+    GraphGUI(g)
+```
+Y nos mostrará la ventana:
+
+<img src="https://user-images.githubusercontent.com/94072018/236611009-de477dd9-d2dd-4247-80fa-dfc3e7a86a4b.png" width="400" height="400">
+
+Sabiendo cómo instanciar grafos, podemos ahora representar objetos algo más complicados ajustando un poco los parámetros de la instancia GraphGUI. En este caso: `GraphGUI(my_gragph, 30, 1000, 1000)`
+
+<img src="https://user-images.githubusercontent.com/94072018/236611227-2b812c07-7eac-4922-85a5-17cb6e13daea.png" width="550" height="550">
+
```

### Comparing `graphdisplay-0.3.6/README.md` & `graphdisplay-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,103 @@
-# graphdisplay
-
-## Resumen
-
-graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos a los alumnos de Estructuras de Datos y Algoritmos. 
-Actualmente solo soporta la visualización de grafos implementados a través de un diccionario, tal y como se aportan como código base en la asignatura. 
-
-## ¿Quieres contribuir?
-
-Este es un proyecto de código abierto hecho por y para estudiantes así que cualquier ayuda, comentario o sugerencia es bienvenido. La mejor manera de contribuir es añadir los bugs que os encontréis 
-en el apartado de Issues pero también estoy completamente abierto a responder cualquier duda o ayuda desde mi correo personal (disponible en mi perfil de github). ¡Muchas gracias de antemano!
-
-## Método de uso 
-
-Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
-tkinter y math (que muchas veces vienen instaladas por defecto en python). 
-
-Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. Una vez hecho esto, se debe instanciar un grafo de tipo diccionario
-para finalmente introducirlo como argumento al instanciar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón 
-para una mejor visualización. **Al desplazar los vértices por la pantalla y fijar su posición, si se cierra la ventana y se vuelve a abrir, el grafo seguirá con la forma con la que se ha movido
-antes.**. Cabe destacar que, únicamente es necesario especificar como argumento el grafo que se quiere representar pero además hay otros ajustes que pueden ser útiles a la hora de mostrar 
-grafos grandes y complejos:
-+ graph: es el objeto de tipo grafo que se va a representar **ES MUY IMPORTANTE** que el grafo que se introduce como argumento sea el implementado en base al código base de la asignatura. Si alguno
-de los atributos cambiase de nombre, el programa no funcionaría correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA) o utilizar la 
-implementación de grafos que viene por defecto con el paquete.
-+ node_radius: el radio de cada vértice del grafo, por defecto es 40 y puede tomar cualquier valor entero entre 10 y 100
-+ scr_width: el tamaño en píxeles del ancho de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
-+ scr_width: el tamaño en píxeles de la altura de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
-
-Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
-```python
-g = Graph([1, 2, 3])
-g.addEdge(1, 2)
-g.addEdge(2, 3)
-
-# Para representar el grafo con todos los valores por defecto
-GraphGUI(g)
-
-# Para ajustar el radio de los nodos a 32, el ancho y largo de la pantalla a 700
-GraphGUI(g, 32, 700, 700)
-
-# Para ajustar únicamente el ancho de la pantalla a 200 píxeles
-GraphGUI(g, scr_width=200)
-```
-
-Además, también es posible generar este tipo de grafos a través de la librería. Importándolo con `from graphdisplay import Graph`, se puede instanciar un objeto de tipo Graph, pasándole como
-argumento una lista de los vértices del grafo para después, añadirle las aristas con el método `add_edge`, con los vértices que conecta la arista además del valor/coste de la arista.
-
-## Ejemplo de uso
-
-Para instanciar un grafo de tipo diccionario, se debe hacer de la siguiente manera: 
-
-```python
-labels = ['A', 'B', 'C', 'D', 'E']
-g = Graph(labels)
-
-# Now, we add the edges
-g.addEdge('A', 'C', 12)  # A->(12)C
-g.addEdge('A', 'D', 60)  # A->(60)D
-g.addEdge('B', 'A', 10)  # B->(10)A
-g.addEdge('C', 'B', 20)  # C->(20)B
-g.addEdge('C', 'D', 32)  # C->(32)D
-g.addEdge('E', 'A', 7)   # E->(7)A
-g.addEdge('A', 'E', 50)  # A->(50)E
-```
-
-Si queremos mostrar la pantalla, basta con instanciar un objeto de tipo GraphGUI, pasándole como argumento el grafo que queremos mostrar: 
-
-```python
-    GraphGUI(g)
-```
-Y nos mostrará la ventana:
-
-<img src="https://user-images.githubusercontent.com/94072018/236611009-de477dd9-d2dd-4247-80fa-dfc3e7a86a4b.png" width="400" height="400">
-
-Sabiendo cómo instanciar grafos, podemos ahora representar objetos algo más complicados ajustando un poco los parámetros de la instancia GraphGUI. En este caso: `GraphGUI(my_gragph, 30, 1000, 1000)`
-
-<img src="https://user-images.githubusercontent.com/94072018/236611227-2b812c07-7eac-4922-85a5-17cb6e13daea.png" width="550" height="550">
-
+Metadata-Version: 2.1
+Name: graphdisplay
+Version: 0.4.0
+Summary: Librería para representar visualmente grafos de tipo diccionario
+Home-page: https://github.com/seniorbeto
+Author: Alberto Penas Díaz
+Author-email: albertopenasdiaz@gmail.com
+License: MIT
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+
+# graphdisplay
+
+## Resumen
+
+graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos a los alumnos de Estructuras de Datos y Algoritmos. 
+Actualmente solo soporta la visualización de grafos implementados a través de un diccionario, tal y como se aportan como código base en la asignatura. 
+
+## ¿Quieres contribuir?
+
+Este es un proyecto de código abierto hecho por y para estudiantes así que cualquier ayuda, comentario o sugerencia es bienvenido. La mejor manera de contribuir es añadir los bugs que os encontréis 
+en el apartado de Issues pero también estoy completamente abierto a responder cualquier duda o ayuda desde mi correo personal (disponible en mi perfil de github). ¡Muchas gracias de antemano!
+
+## Método de uso 
+
+Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
+tkinter y math (que muchas veces vienen instaladas por defecto en python). 
+
+Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. Una vez hecho esto, se debe instanciar un grafo de tipo diccionario
+para finalmente introducirlo como argumento al instanciar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón 
+para una mejor visualización. Cabe destacar que, únicamente es necesario especificar como argumento el grafo que se quiere representar pero además hay otros ajustes que pueden ser útiles a la hora de mostrar 
+grafos grandes y complejos:
++ graph: es el objeto de tipo grafo que se va a representar **ES MUY IMPORTANTE** que el grafo que se introduce como argumento sea el implementado en base al código base de la asignatura. Si alguno
+de los atributos cambiase de nombre, el programa no funcionaría correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA) o utilizar la 
+implementación de grafos que viene por defecto con el paquete.
++ node_radius: el radio de cada vértice del grafo, por defecto es 40 y puede tomar cualquier valor entero entre 10 y 100
++ scr_width: el tamaño en píxeles del ancho de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
++ scr_width: el tamaño en píxeles de la altura de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
++ theme: el tema de la ventana, por defecto es 'brown' y no voy a mencionarlos todos porque hay muchos y me da pereza.
+
+Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
+```python
+g = Graph([1, 2, 3])
+g.addEdge(1, 2)
+g.addEdge(2, 3)
+
+# Para representar el grafo con todos los valores por defecto
+GraphGUI(g)
+
+# Para ajustar el radio de los nodos a 32, el ancho y largo de la pantalla a 700
+GraphGUI(g, 32, 700, 700)
+
+# Para ajustar únicamente el ancho de la pantalla a 200 píxeles
+GraphGUI(g, scr_width=200)
+```
+
+Además, también es posible generar este tipo de grafos a través de la librería. Importándolo con `from graphdisplay import Graph`, se puede instanciar un objeto de tipo Graph, pasándole como
+argumento una lista de los vértices del grafo para después, añadirle las aristas con el método `addEdge`, con los vértices que conecta la arista además del valor/coste de la arista.
+
+## Funcionalidades
+Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
+éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
+instaciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
+Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
+tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón save y nombrando el guardado) para
+después poder cargarlo en cualquier momento.
+## Ejemplo de uso
+
+Para instanciar un grafo de tipo diccionario, se debe hacer de la siguiente manera: 
+
+```python
+labels = ['A', 'B', 'C', 'D', 'E']
+g = Graph(labels)
+
+# Now, we add the edges
+g.addEdge('A', 'C', 12)  # A->(12)C
+g.addEdge('A', 'D', 60)  # A->(60)D
+g.addEdge('B', 'A', 10)  # B->(10)A
+g.addEdge('C', 'B', 20)  # C->(20)B
+g.addEdge('C', 'D', 32)  # C->(32)D
+g.addEdge('E', 'A', 7)   # E->(7)A
+g.addEdge('A', 'E', 50)  # A->(50)E
+```
+
+Si queremos mostrar la pantalla, basta con instanciar un objeto de tipo GraphGUI, pasándole como argumento el grafo que queremos mostrar: 
+
+```python
+    GraphGUI(g)
+```
+Y nos mostrará la ventana:
+
+<img src="https://user-images.githubusercontent.com/94072018/236611009-de477dd9-d2dd-4247-80fa-dfc3e7a86a4b.png" width="400" height="400">
+
+Sabiendo cómo instanciar grafos, podemos ahora representar objetos algo más complicados ajustando un poco los parámetros de la instancia GraphGUI. En este caso: `GraphGUI(my_gragph, 30, 1000, 1000)`
+
+<img src="https://user-images.githubusercontent.com/94072018/236611227-2b812c07-7eac-4922-85a5-17cb6e13daea.png" width="550" height="550">
+
```

### Comparing `graphdisplay-0.3.6/graphdisplay/general_config.py` & `graphdisplay-0.4.0/graphdisplay/general_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,135 +1,140 @@
-THEMES = {
-    "BROWN":{
-        "BUTTON_COLOR": "#ede4cc",
-        "VERTEX_COLOR": "#e3d7c5",
-        "BACKGROUND_CANVAS_COLOR": "#c7b9a5",
-        "FRAME_COLOR": "#87715f",
-        "AUTHOR_NAME_COLOR": "#301d05"
-    },
-    "BLUE":{
-        "BUTTON_COLOR": "#b7e7e8",
-        "VERTEX_COLOR": "#a7d6fc",
-        "BACKGROUND_CANVAS_COLOR": "#b5d9f7",
-        "FRAME_COLOR": "#6aaade",
-        "AUTHOR_NAME_COLOR": "#0b2d47"
-    },
-    "DARK":{
-        "BUTTON_COLOR": "#6a6a7d",
-        "VERTEX_COLOR": "#7d7d96",
-        "BACKGROUND_CANVAS_COLOR": "#404147",
-        "FRAME_COLOR": "#272729",
-        "AUTHOR_NAME_COLOR": "#c0c0f0"
-    },
-    "JESUSFUCKINGCHRIST":{
-        "BUTTON_COLOR": "#fffb00",
-        "VERTEX_COLOR": "#fffb00",
-        "BACKGROUND_CANVAS_COLOR": "#fffb00",
-        "FRAME_COLOR": "#fffb00",
-        "AUTHOR_NAME_COLOR": "#000000"
-    },
-    "PURPLE":{
-        "BUTTON_COLOR": "#f2c8fa",
-        "VERTEX_COLOR": "#e7cdf7",
-        "BACKGROUND_CANVAS_COLOR": "#e4c3fa",
-        "FRAME_COLOR": "#d899f7",
-        "AUTHOR_NAME_COLOR": "#6d1aa3"
-    },
-    "GREEN":{
-        "BUTTON_COLOR": "#B5FFC7",
-        "VERTEX_COLOR": "#A1FDB3",
-        "BACKGROUND_CANVAS_COLOR": "#BFFFCF",
-        "FRAME_COLOR": "#80FF99",
-        "AUTHOR_NAME_COLOR": "#05331F"
-    },
-    "DARKGREEN":{
-        "BUTTON_COLOR": "#173F2D",
-        "VERTEX_COLOR": "#215C41",
-        "BACKGROUND_CANVAS_COLOR": "#163623",
-        "FRAME_COLOR": "#0C2B1A",
-        "AUTHOR_NAME_COLOR": "#FFFFFF"
-    },
-    "UBUNTU":{
-        "BUTTON_COLOR": "#b35625",
-        "VERTEX_COLOR": "#d45102",
-        "BACKGROUND_CANVAS_COLOR": "#404040",
-        "FRAME_COLOR": "#303030",
-        "AUTHOR_NAME_COLOR": "#FFFFFF"
-    },
-    "LA NOCHE ESTRELLADA":{
-        "BUTTON_COLOR": "#9bafaa",
-        "VERTEX_COLOR": "#7b94a4",
-        "BACKGROUND_CANVAS_COLOR": "#557491",
-        "FRAME_COLOR": "#242d34",
-        "AUTHOR_NAME_COLOR": "#d5bc6a"
-    },
-    "LA GRAN OLA":{
-        "BUTTON_COLOR": "#a6a49b",
-        "VERTEX_COLOR": "#e7e2d2",
-        "BACKGROUND_CANVAS_COLOR": "#8599a4",
-        "FRAME_COLOR": "#4a5f79",
-        "AUTHOR_NAME_COLOR": "#d5bc6a"
-    },
-    "ANTARTICA":{
-        "BUTTON_COLOR": "#9BA4B5",
-        "VERTEX_COLOR": "#9BA4B5",
-        "BACKGROUND_CANVAS_COLOR": "#394867",
-        "FRAME_COLOR": "#212A3E",
-        "AUTHOR_NAME_COLOR": "#83764F"
-    },
-    "BREAKING BAD":{
-        "BUTTON_COLOR": "#F7E1AE",
-        "VERTEX_COLOR": "#F7E1AE",
-        "BACKGROUND_CANVAS_COLOR": "#617A55",
-        "FRAME_COLOR": "#3d4d36",
-        "AUTHOR_NAME_COLOR": "#F7E1AE"
-    },
-    "SOFT":{
-        "BUTTON_COLOR": "#E4D0D0",
-        "VERTEX_COLOR": "#E4D0D0",
-        "BACKGROUND_CANVAS_COLOR": "#D5B4B4",
-        "FRAME_COLOR": "#867070",
-        "AUTHOR_NAME_COLOR": "#000000"
-    },
-    "TURQUOISE": {
-        "BUTTON_COLOR": "#0E8388",
-        "VERTEX_COLOR": "#83918e",
-        "BACKGROUND_CANVAS_COLOR": "#2E4F4F",
-        "FRAME_COLOR": "#2C3333",
-        "AUTHOR_NAME_COLOR": "#CBE4DE"
-    },
-    "DEEP PURPLE":{
-        "BUTTON_COLOR": "#bdb8ac",
-        "VERTEX_COLOR": "#bdb8ac",
-        "BACKGROUND_CANVAS_COLOR": "#6D5D6E",
-        "FRAME_COLOR": "#4F4557",
-        "AUTHOR_NAME_COLOR": "#F4EEE0"
-    },
-    "THIS ONE IS UGLY":{
-        "BUTTON_COLOR": "#F67280",
-        "VERTEX_COLOR": "#C06C84",
-        "BACKGROUND_CANVAS_COLOR": "#6C5B7B",
-        "FRAME_COLOR": "#355C7D",
-        "AUTHOR_NAME_COLOR": "#F67280"
-    },
-    "FROST": {
-        "BUTTON_COLOR": "#00ADB5",
-        "VERTEX_COLOR": "#00ADB5",
-        "BACKGROUND_CANVAS_COLOR": "#393E46",
-        "FRAME_COLOR": "#222831",
-        "AUTHOR_NAME_COLOR": "#EEEEEE"
-    },
-    "NEKOS": {
-        "BUTTON_COLOR": "#DEFCF9",
-        "VERTEX_COLOR": "#CADEFC",
-        "BACKGROUND_CANVAS_COLOR": "#C3BEF0",
-        "FRAME_COLOR": "#CCA8E9",
-        "AUTHOR_NAME_COLOR": "#DEFCF9"
-    },
-    "VAMPIRE": {
-        "BUTTON_COLOR": "#FF0000",
-        "VERTEX_COLOR": "#FF0000",
-        "BACKGROUND_CANVAS_COLOR": "#950101",
-        "FRAME_COLOR": "#3D0000",
-        "AUTHOR_NAME_COLOR": "#FF0000"
-    }
+VERSION = '0.4.0'
+BUTTON_HEIGHT = 30
+BUTTON_WIDTH = 60
+XMARGEN = 7
+YMARGEN = 7
+THEMES = {
+    "BROWN":{
+        "BUTTON_COLOR": "#ede4cc",
+        "VERTEX_COLOR": "#e3d7c5",
+        "BACKGROUND_CANVAS_COLOR": "#c7b9a5",
+        "FRAME_COLOR": "#87715f",
+        "AUTHOR_NAME_COLOR": "#301d05"
+    },
+    "BLUE":{
+        "BUTTON_COLOR": "#b7e7e8",
+        "VERTEX_COLOR": "#a7d6fc",
+        "BACKGROUND_CANVAS_COLOR": "#b5d9f7",
+        "FRAME_COLOR": "#6aaade",
+        "AUTHOR_NAME_COLOR": "#0b2d47"
+    },
+    "DARK":{
+        "BUTTON_COLOR": "#6a6a7d",
+        "VERTEX_COLOR": "#7d7d96",
+        "BACKGROUND_CANVAS_COLOR": "#404147",
+        "FRAME_COLOR": "#272729",
+        "AUTHOR_NAME_COLOR": "#c0c0f0"
+    },
+    "JESUSFUCKINGCHRIST":{
+        "BUTTON_COLOR": "#fffb00",
+        "VERTEX_COLOR": "#fffb00",
+        "BACKGROUND_CANVAS_COLOR": "#fffb00",
+        "FRAME_COLOR": "#fffb00",
+        "AUTHOR_NAME_COLOR": "#000000"
+    },
+    "PURPLE":{
+        "BUTTON_COLOR": "#f2c8fa",
+        "VERTEX_COLOR": "#e7cdf7",
+        "BACKGROUND_CANVAS_COLOR": "#e4c3fa",
+        "FRAME_COLOR": "#d899f7",
+        "AUTHOR_NAME_COLOR": "#6d1aa3"
+    },
+    "GREEN":{
+        "BUTTON_COLOR": "#B5FFC7",
+        "VERTEX_COLOR": "#A1FDB3",
+        "BACKGROUND_CANVAS_COLOR": "#BFFFCF",
+        "FRAME_COLOR": "#80FF99",
+        "AUTHOR_NAME_COLOR": "#05331F"
+    },
+    "DARKGREEN":{
+        "BUTTON_COLOR": "#173F2D",
+        "VERTEX_COLOR": "#215C41",
+        "BACKGROUND_CANVAS_COLOR": "#163623",
+        "FRAME_COLOR": "#0C2B1A",
+        "AUTHOR_NAME_COLOR": "#FFFFFF"
+    },
+    "UBUNTU":{
+        "BUTTON_COLOR": "#b35625",
+        "VERTEX_COLOR": "#d45102",
+        "BACKGROUND_CANVAS_COLOR": "#404040",
+        "FRAME_COLOR": "#303030",
+        "AUTHOR_NAME_COLOR": "#FFFFFF"
+    },
+    "LA NOCHE ESTRELLADA":{
+        "BUTTON_COLOR": "#9bafaa",
+        "VERTEX_COLOR": "#7b94a4",
+        "BACKGROUND_CANVAS_COLOR": "#557491",
+        "FRAME_COLOR": "#242d34",
+        "AUTHOR_NAME_COLOR": "#d5bc6a"
+    },
+    "LA GRAN OLA":{
+        "BUTTON_COLOR": "#a6a49b",
+        "VERTEX_COLOR": "#e7e2d2",
+        "BACKGROUND_CANVAS_COLOR": "#8599a4",
+        "FRAME_COLOR": "#4a5f79",
+        "AUTHOR_NAME_COLOR": "#d5bc6a"
+    },
+    "ANTARTICA":{
+        "BUTTON_COLOR": "#9BA4B5",
+        "VERTEX_COLOR": "#9BA4B5",
+        "BACKGROUND_CANVAS_COLOR": "#394867",
+        "FRAME_COLOR": "#212A3E",
+        "AUTHOR_NAME_COLOR": "#83764F"
+    },
+    "BREAKING BAD":{
+        "BUTTON_COLOR": "#F7E1AE",
+        "VERTEX_COLOR": "#F7E1AE",
+        "BACKGROUND_CANVAS_COLOR": "#617A55",
+        "FRAME_COLOR": "#3d4d36",
+        "AUTHOR_NAME_COLOR": "#F7E1AE"
+    },
+    "SOFT":{
+        "BUTTON_COLOR": "#E4D0D0",
+        "VERTEX_COLOR": "#E4D0D0",
+        "BACKGROUND_CANVAS_COLOR": "#D5B4B4",
+        "FRAME_COLOR": "#867070",
+        "AUTHOR_NAME_COLOR": "#000000"
+    },
+    "TURQUOISE": {
+        "BUTTON_COLOR": "#0E8388",
+        "VERTEX_COLOR": "#83918e",
+        "BACKGROUND_CANVAS_COLOR": "#2E4F4F",
+        "FRAME_COLOR": "#2C3333",
+        "AUTHOR_NAME_COLOR": "#CBE4DE"
+    },
+    "DEEP PURPLE":{
+        "BUTTON_COLOR": "#bdb8ac",
+        "VERTEX_COLOR": "#bdb8ac",
+        "BACKGROUND_CANVAS_COLOR": "#6D5D6E",
+        "FRAME_COLOR": "#4F4557",
+        "AUTHOR_NAME_COLOR": "#F4EEE0"
+    },
+    "THIS ONE IS UGLY":{
+        "BUTTON_COLOR": "#F67280",
+        "VERTEX_COLOR": "#C06C84",
+        "BACKGROUND_CANVAS_COLOR": "#6C5B7B",
+        "FRAME_COLOR": "#355C7D",
+        "AUTHOR_NAME_COLOR": "#F67280"
+    },
+    "FROST": {
+        "BUTTON_COLOR": "#00ADB5",
+        "VERTEX_COLOR": "#00ADB5",
+        "BACKGROUND_CANVAS_COLOR": "#393E46",
+        "FRAME_COLOR": "#222831",
+        "AUTHOR_NAME_COLOR": "#EEEEEE"
+    },
+    "NEKOS": {
+        "BUTTON_COLOR": "#DEFCF9",
+        "VERTEX_COLOR": "#CADEFC",
+        "BACKGROUND_CANVAS_COLOR": "#C3BEF0",
+        "FRAME_COLOR": "#CCA8E9",
+        "AUTHOR_NAME_COLOR": "#DEFCF9"
+    },
+    "VAMPIRE": {
+        "BUTTON_COLOR": "#FF0000",
+        "VERTEX_COLOR": "#FF0000",
+        "BACKGROUND_CANVAS_COLOR": "#950101",
+        "FRAME_COLOR": "#3D0000",
+        "AUTHOR_NAME_COLOR": "#FF0000"
+    }
 }
```

### Comparing `graphdisplay-0.3.6/graphdisplay/graph.py` & `graphdisplay-0.4.0/graphdisplay/graphs/graph.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,434 +1,434 @@
-# -*- coding: utf-8 -*-
-import math
-
-class AdjacentVertex:
-    """This class allows us to represent a tuple with an adjacent vertex
-    and the weight associated (by default 1, for non-unweighted graphs)"""
-
-    def __init__(self, vertex, weight=None):
-        self._vertex = vertex
-        self._weight = weight
-
-    def __str__(self):
-        if self._weight != None:
-            return '(' + str(self._vertex) + ',' + str(self._weight) + ')'
-        else:
-            return str(self._vertex)
-
-
-class Graph():
-    def __init__(self, vertices, directed=True):
-        """We use a dictionary to represent the graph
-        the dictionary's keys are the vertices
-        The value associated for a given key will be the list of their neighbours.
-        Initially, the list of neighbours is empty"""
-        self._vertices = {}
-        for v in vertices:
-            self._vertices[v] = []
-        self._directed = directed
-
-    def addEdge(self, start, end, weight=None):
-        if start not in self._vertices.keys():
-            print(start, ' does not exist!')
-            return
-        if end not in self._vertices.keys():
-            print(end, ' does not exist!')
-            return
-
-        # adds to the end of the list of neigbours for start
-        self._vertices[start].append(AdjacentVertex(end, weight))
-
-        if self._directed == False:
-            # adds to the end of the list of neigbours for end
-            self._vertices[end].append(AdjacentVertex(start, weight))
-
-    def containsEdge(self, start, end):
-        if start not in self._vertices.keys():
-            print(start, ' does not exist!')
-            return 0
-        if end not in self._vertices.keys():
-            print(end, ' does not exist!')
-            return 0
-
-        # we search the AdjacentVertex whose v is end
-        for adj in self._vertices[start]:
-            if adj._vertex == end:
-                if adj._weight != None:
-                    return adj._weight
-                else:
-                    return 1  # unweighted graphs
-        return 0  # does not exist
-
-    def removeEdge(self, start, end):
-        if start not in self._vertices.keys():
-            print(start, ' does not exist!')
-            return
-        if end not in self._vertices.keys():
-            print(end, ' does not exist!')
-            return
-
-        # we must look for the adjacent AdjacentVertex (neighbour)  whose vertex is end, and then remove it
-        for adj in self._vertices[start]:
-            if adj._vertex == end:
-                self._vertices[start].remove(adj)
-        if self._directed == False:
-            # we must also look for the AdjacentVertex (neighbour)  whose vertex is end, and then remove it
-            for adj in self._vertices[end]:
-                if adj._vertex == start:
-                    self._vertices[end].remove(adj)
-
-    def __str__(self):
-        result = ''
-        for v in self._vertices:
-            result += '\n' + str(v) + ':'
-            for adj in self._vertices[v]:
-                result += str(adj) + "  "
-        return result
-
-    def add_vertex(self, vertex: str) -> None:
-        if vertex in self._vertices.keys():
-            print(vertex, ' already exists!')
-            return
-        self._vertices[vertex] = []
-
-    def _dfs(self, vertex: str, visited: dict) -> None:
-        visited[vertex] = True
-        for adj in self._vertices[vertex]:
-            # adj is an object of AdjacentVertex
-            adj_vertex = adj.vertex
-            if not visited[adj_vertex]:
-                self._dfs(adj_vertex, visited)
-
-    def _bfs(self, vertex: str, visited: dict) -> None:
-        queue = [vertex]
-        visited[vertex] = True
-        while len(queue) > 0:
-            u = queue.pop(0)
-            for adj in self._vertices[u]:
-                # remember that adj is an AdjacentVertex
-                if not visited[adj.vertex]:
-                    queue.append(adj.vertex)
-                    visited[adj.vertex] = True
-
-    def non_accessible(self, vertex: str) -> list:
-        """gets a vertex and returns the list of vertices
-        that cannot be reached from vertex, that is, there is no path
-        from vertex to these vertices"""
-        # First, we need to obtain all vertices that can be
-        # reached from vertex. To do this, we can apply
-        # the algorithms of dfs or bfs
-        visited = {}
-        for v1 in self._vertices:
-            visited[v1] = False
-        self._dfs(vertex, visited)
-        # The function _dfs will visit all vertices reachable
-        # from vertex. Therefore, the non-visited vertices
-        # will form the list of non-accessible vertices from vertex
-        result = []  # list with the non-accessible vertices
-        for v1 in self._vertices:
-            if not visited[v1]:
-                result.append(v1)
-
-        return result
-
-    def get_reachable(self, vertex: str, alg: str = '_dfs') -> list:
-        """gets a vertex and returns the list of vertices
-        that can be reached from vertex, that is, there is a path
-        from vertex to these vertices"""
-        # First, we need to obtain all vertices that can be
-        # reached from vertex. To do this, we can apply
-        # the algorithms of dfs or bfs
-        visited = {}
-        for v1 in self._vertices:
-            visited[v1] = False
-        if alg == '_dfs':
-            self._dfs(vertex, visited)
-        else:
-            self._bfs(vertex, visited)
-
-        # The function _dfs will visit all vertices reachable
-        # from vertex. Therefore, the visited vertices
-        # will form the list of accessible vertices from vertex
-        result = []  # list with the accessible vertices
-        for v1 in self._vertices:
-            if visited[v1]:
-                result.append(v1)
-
-        return result
-
-    def _check_bipartite(self, source: str, color: dict) -> bool:
-
-        # Assign first color to source
-        queue = [source]
-        color[source] = 1
-        # similar to bfs
-        while len(queue):
-            u = queue.pop(0)
-            for adj in self._vertices[u]:
-                adj_vertex = adj.vertex
-                if color[adj_vertex] is None:
-                    color[adj_vertex] = 1 - color[u]
-                    queue.append(adj_vertex)
-                elif color[adj_vertex] == color[u]:
-                    return False
-
-        # If we reach here, then all adjacent
-        # vertices can be colored with alternate
-        # color
-        return True
-
-    def check_bipartite(self) -> bool:
-        """ returns True if the graph is bipartite and False eoc
-        A graph is bipartite is a graph whose vertices can be divided
-        into two independent sets, U and V
-        such that every edge (u, v) either connects a vertex
-        from U to V or a vertex from V to U.
-        In other words, for every edge (u, v), either u belongs to U and v to V,
-         or u belongs to V and v to U. We can also say that there is no edge
-         that connects vertices of same set. """
-        color = {}
-        # We use a dictionary color to save the color
-        # assigned to each vertex: 1 means first color (origins)
-        # , 0 means second color (target)
-        for v1 in self._vertices:
-            color[v1] = None
-
-        for v1 in self._vertices:
-            if color[v1] is None:
-                if not self._check_bipartite(v1, color):
-                    return False
-
-        return True
-
-    def _has_cycles_bfs(self, vertex: str, visited: dict) -> bool:
-        """This is function is based on bfs to detect if there is
-        some cycle in the breadth traversal from vertex. It uses the dictionary
-        visited and the parent of the vertices to detect
-        cycle in subgraph reachable from vertex v."""
-
-        # Mark the current vertex as visited
-        queue = [vertex]
-        parents = {}
-        for v1 in self._vertices:
-            parents[v1] = None
-
-        while len(queue) > 0:
-            s = queue.pop(0)
-            visited[s] = True
-            for adj in self._vertices[s]:
-                adj_vertex = adj.vertex
-                if not visited[adj_vertex]:
-                    visited[adj_vertex] = True
-                    queue.append(adj_vertex)
-                    parents[adj_vertex] = s
-                elif parents[s] != adj_vertex:
-                    # if the ajd_vertex has been already visited,
-                    # and it is not the parent of current vertex,
-                    # then there is a cycle
-                    return True
-        return False
-
-    def _has_cycles_dfs(self, vertex: str, visited: dict, parent: str) -> bool:
-        """This is recursive function that uses the dictionary
-        visited and the parent of the vertices to detect
-        cycle in subgraph reachable from vertex v."""
-
-        # Mark the current vertex as visited
-        visited[vertex] = True
-        # Recur for all the vertices
-        # adjacent to this vertex
-        for adj in self._vertices[vertex]:
-            adj_vertex = adj.vertex
-            # If the node is not visited then recurse on it
-            if not visited[adj_vertex]:
-                if self._has_cycles_dfs(adj_vertex, visited, vertex):
-                    return True
-            elif parent != adj_vertex:
-                # if the ajd_vertex has been already visited,
-                # and it is not the parent of current vertex,
-                # then there is a cycle
-                return True
-        print()
-        return False
-
-    def _has_cycles_directed(self, vertex: str, visited: dict, rec_stack: dict) -> bool:
-        """detects a cycle in a directed graph using the
-        dfs alg. Moreover, visited and rec_stack allow us
-        to detect if a vertex has been previously visited."""
-
-        # Mark the current vertex as visited
-        visited[vertex] = True
-        rec_stack[vertex] = True
-        # Recur for all the vertices
-        # adjacent to this vertex
-        for adj in self._vertices[vertex]:
-            adj_vertex = adj.vertex
-            # If the node is not visited then recurse on it
-            if not visited[adj_vertex]:
-                if self._has_cycles_directed(adj_vertex, visited, rec_stack):
-                    return True
-            elif rec_stack[adj_vertex]:
-                return True
-        # The node needs to be popped from
-        # recursion stack before function ends
-        rec_stack[vertex] = False
-        return False
-
-    def has_cycles(self, alg: str = 'dfs') -> bool:
-        """returns True if the graph contains a cycle, False eoc"""
-        print(self._directed)
-        visited = {}
-        recursion_stack = {}
-
-        for v1 in self._vertices:
-            visited[v1] = False
-            # we will only use it for directed graphs
-            recursion_stack[v1] = False
-
-        # Call the recursive helper
-        # function to detect cycle in different
-        # DFS trees
-        for v1 in self._vertices:
-            if not visited[v1]:
-                if self._directed:
-                    result = self._has_cycles_directed(v1, visited, recursion_stack)
-                else:
-                    if alg == 'dfs':
-                        result = self._has_cycles_dfs(v1, visited, None)
-                    else:
-                        result = self._has_cycles_bfs(v1, visited)
-
-                if result:
-                    return True
-
-        return False
-
-    def min_distance(self, distances: dict, visited: dict) -> int:
-        """ This function is used from dijkstra.
-        It returns the vertex (index) whose associated value in
-        the dictionary distances is the smallest value. We
-        only consider the set of vertices that have not been visited"""
-        # Initialize minimum distance for next node
-        min_distance = math.inf
-        min_vertex = None
-
-        # returns the vertex with minimum distance from the non-visited vertices
-        for vertex in self._vertices.keys():
-            if distances[vertex] <= min_distance and not visited[vertex]:
-                min_distance = distances[vertex]  # update the new smallest
-                min_vertex = vertex  # update the index of the smallest
-
-        return min_vertex
-
-    def dijkstra(self, origin: object) -> None:
-        visited = {}  # for each vertex (key), the value is a boolean indicating if the vertex has been visited
-        previous = {}  # for each vertex (key), the value is the previous node in the minimum path from origin
-        distances = {}  # for each vertex (key), the value is minimum distance in the minimum path from origin
-
-        # initialize dictionaries
-        for v in self._vertices.keys():
-            visited[v] = False
-            previous[v] = None
-            distances[v] = math.inf
-
-        # The distance from origin to itself is 0
-        distances[origin] = 0
-
-        for _ in range(len(self._vertices)):
-            # pick the non-visited vertex with minimum distance
-            u = self.min_distance(distances, visited)
-            visited[u] = True
-            # get the adjacent vertices of u
-            for adj in self._vertices[u]:
-                i = adj._vertex
-                w = adj._weight
-                # for non-visited vertex, we have to check if its distance is greater than the distance from u
-                if not visited[i] and distances[i] > distances[u] + w:
-                    # we must update because its distance is greater than the new distance
-                    distances[i] = distances[u] + w
-                    previous[i] = u
-
-        # Finally, we print the minimum path from origin to the other vertices
-        self.print_solution(distances, previous, origin)
-
-        return distances, previous
-
-    def print_solution(self, distances: dict, previous: dict, origin: object):
-        """Both Dijkstra and Bellman-Ford algorithms use this function.
-        For each vertex, the function is able to rebuild the reverse path from i to origin.
-        To do this, the function only needs to read the value associated to the vertex in the dictionary
-        previous until to reach a vertex whouse associated value is None (origin)"""
-        print("Minimum path from ", origin)
-
-        for i in self._vertices.keys():
-            if distances[i] == math.inf:
-                print("There is not path from ", origin, ' to ', i)
-            else:
-                # minimum_path is the list which contains the minimum path from origin to i
-                minimum_path = []
-                prev = previous[i]
-                # this loop helps us to build the path
-                while prev is not None:
-                    minimum_path.insert(0, prev)
-                    prev = previous[prev]
-
-                # we append the last vertex, which is i
-                minimum_path.append(i)
-
-                # we print the path from v to i and the distance
-                print(origin, '->', i, ":", minimum_path, distances[i])
-
-    def bellmanford(self, origin: object) -> None:
-        """Bellman-Ford algorithm for minimum path"""
-        previous = {}
-        distances = {}
-        for v in self._vertices.keys():
-            previous[v] = None
-            distances[v] = math.inf
-        distances[origin] = 0
-
-        for _ in range(len(self._vertices) - 1):
-            for u in self._vertices.keys():
-                # get all adjacent vertices of u
-                for adj in self._vertices[u]:
-                    v = adj.vertex
-                    w = adj.weight
-                    if distances[v] > distances[u] + w:
-                        distances[v] = distances[u] + w
-                        previous[v] = u
-
-        # final review to check if there is a solution, or there is a negative cicle (therefore, there is no solution)
-        for u in self._vertices.keys():
-            for adj in self._vertices[u]:
-                v = adj._vertex
-                w = adj._weight
-                if distances[v] > distances[u] + w:
-                    # There is at least a negative cicle.
-                    print('There is no solution ', origin)
-                    return False
-
-        self.print_solution(distances, previous, origin)
-        return distances, previous
-
-    def minimum_path(self, start: object, end: object) -> list:
-        """ returns a list containing the path from star to end.
-        It also returns the distance of the path. If the path
-        does not exist, it returns an empty list and infinito"""
-        if start not in self._vertices.keys():
-            print(start, ' does not exist!!!')
-            return None, None
-        if end not in self._vertices.keys():
-            print(end, ' does not exist!!!')
-            return None, None
-
-        distances, previous = self.dijkstra(start)
-        if distances[end] == math.inf:
-            return [], math.inf
-
-        result = [end]
-        prev = previous[end]
-        while prev is not None:
-            result.insert(0, prev)
-            prev = previous[prev]
-
-        return result, distances[end]
+# -*- coding: utf-8 -*-
+import math
+
+class AdjacentVertex:
+    """This class allows us to represent a tuple with an adjacent vertex
+    and the weight associated (by default 1, for non-unweighted graphs)"""
+
+    def __init__(self, vertex, weight=None):
+        self._vertex = vertex
+        self._weight = weight
+
+    def __str__(self):
+        if self._weight != None:
+            return '(' + str(self._vertex) + ',' + str(self._weight) + ')'
+        else:
+            return str(self._vertex)
+
+
+class Graph():
+    def __init__(self, vertices, directed=True):
+        """We use a dictionary to represent the graph
+        the dictionary's keys are the vertices
+        The value associated for a given key will be the list of their neighbours.
+        Initially, the list of neighbours is empty"""
+        self._vertices = {}
+        for v in vertices:
+            self._vertices[v] = []
+        self._directed = directed
+
+    def addEdge(self, start, end, weight=None):
+        if start not in self._vertices.keys():
+            print(start, ' does not exist!')
+            return
+        if end not in self._vertices.keys():
+            print(end, ' does not exist!')
+            return
+
+        # adds to the end of the list of neigbours for start
+        self._vertices[start].append(AdjacentVertex(end, weight))
+
+        if self._directed == False:
+            # adds to the end of the list of neigbours for end
+            self._vertices[end].append(AdjacentVertex(start, weight))
+
+    def containsEdge(self, start, end):
+        if start not in self._vertices.keys():
+            print(start, ' does not exist!')
+            return 0
+        if end not in self._vertices.keys():
+            print(end, ' does not exist!')
+            return 0
+
+        # we search the AdjacentVertex whose v is end
+        for adj in self._vertices[start]:
+            if adj._vertex == end:
+                if adj._weight != None:
+                    return adj._weight
+                else:
+                    return 1  # unweighted graphs
+        return 0  # does not exist
+
+    def removeEdge(self, start, end):
+        if start not in self._vertices.keys():
+            print(start, ' does not exist!')
+            return
+        if end not in self._vertices.keys():
+            print(end, ' does not exist!')
+            return
+
+        # we must look for the adjacent AdjacentVertex (neighbour)  whose vertex is end, and then remove it
+        for adj in self._vertices[start]:
+            if adj._vertex == end:
+                self._vertices[start].remove(adj)
+        if self._directed == False:
+            # we must also look for the AdjacentVertex (neighbour)  whose vertex is end, and then remove it
+            for adj in self._vertices[end]:
+                if adj._vertex == start:
+                    self._vertices[end].remove(adj)
+
+    def __str__(self):
+        result = ''
+        for v in self._vertices:
+            result += '\n' + str(v) + ':'
+            for adj in self._vertices[v]:
+                result += str(adj) + "  "
+        return result
+
+    def add_vertex(self, vertex: str) -> None:
+        if vertex in self._vertices.keys():
+            print(vertex, ' already exists!')
+            return
+        self._vertices[vertex] = []
+
+    def _dfs(self, vertex: str, visited: dict) -> None:
+        visited[vertex] = True
+        for adj in self._vertices[vertex]:
+            # adj is an object of AdjacentVertex
+            adj_vertex = adj.vertex
+            if not visited[adj_vertex]:
+                self._dfs(adj_vertex, visited)
+
+    def _bfs(self, vertex: str, visited: dict) -> None:
+        queue = [vertex]
+        visited[vertex] = True
+        while len(queue) > 0:
+            u = queue.pop(0)
+            for adj in self._vertices[u]:
+                # remember that adj is an AdjacentVertex
+                if not visited[adj.vertex]:
+                    queue.append(adj.vertex)
+                    visited[adj.vertex] = True
+
+    def non_accessible(self, vertex: str) -> list:
+        """gets a vertex and returns the list of vertices
+        that cannot be reached from vertex, that is, there is no path
+        from vertex to these vertices"""
+        # First, we need to obtain all vertices that can be
+        # reached from vertex. To do this, we can apply
+        # the algorithms of dfs or bfs
+        visited = {}
+        for v1 in self._vertices:
+            visited[v1] = False
+        self._dfs(vertex, visited)
+        # The function _dfs will visit all vertices reachable
+        # from vertex. Therefore, the non-visited vertices
+        # will form the list of non-accessible vertices from vertex
+        result = []  # list with the non-accessible vertices
+        for v1 in self._vertices:
+            if not visited[v1]:
+                result.append(v1)
+
+        return result
+
+    def get_reachable(self, vertex: str, alg: str = '_dfs') -> list:
+        """gets a vertex and returns the list of vertices
+        that can be reached from vertex, that is, there is a path
+        from vertex to these vertices"""
+        # First, we need to obtain all vertices that can be
+        # reached from vertex. To do this, we can apply
+        # the algorithms of dfs or bfs
+        visited = {}
+        for v1 in self._vertices:
+            visited[v1] = False
+        if alg == '_dfs':
+            self._dfs(vertex, visited)
+        else:
+            self._bfs(vertex, visited)
+
+        # The function _dfs will visit all vertices reachable
+        # from vertex. Therefore, the visited vertices
+        # will form the list of accessible vertices from vertex
+        result = []  # list with the accessible vertices
+        for v1 in self._vertices:
+            if visited[v1]:
+                result.append(v1)
+
+        return result
+
+    def _check_bipartite(self, source: str, color: dict) -> bool:
+
+        # Assign first color to source
+        queue = [source]
+        color[source] = 1
+        # similar to bfs
+        while len(queue):
+            u = queue.pop(0)
+            for adj in self._vertices[u]:
+                adj_vertex = adj.vertex
+                if color[adj_vertex] is None:
+                    color[adj_vertex] = 1 - color[u]
+                    queue.append(adj_vertex)
+                elif color[adj_vertex] == color[u]:
+                    return False
+
+        # If we reach here, then all adjacent
+        # vertices can be colored with alternate
+        # color
+        return True
+
+    def check_bipartite(self) -> bool:
+        """ returns True if the graph is bipartite and False eoc
+        A graph is bipartite is a graph whose vertices can be divided
+        into two independent sets, U and V
+        such that every edge (u, v) either connects a vertex
+        from U to V or a vertex from V to U.
+        In other words, for every edge (u, v), either u belongs to U and v to V,
+         or u belongs to V and v to U. We can also say that there is no edge
+         that connects vertices of same set. """
+        color = {}
+        # We use a dictionary color to save the color
+        # assigned to each vertex: 1 means first color (origins)
+        # , 0 means second color (target)
+        for v1 in self._vertices:
+            color[v1] = None
+
+        for v1 in self._vertices:
+            if color[v1] is None:
+                if not self._check_bipartite(v1, color):
+                    return False
+
+        return True
+
+    def _has_cycles_bfs(self, vertex: str, visited: dict) -> bool:
+        """This is function is based on bfs to detect if there is
+        some cycle in the breadth traversal from vertex. It uses the dictionary
+        visited and the parent of the vertices to detect
+        cycle in subgraph reachable from vertex v."""
+
+        # Mark the current vertex as visited
+        queue = [vertex]
+        parents = {}
+        for v1 in self._vertices:
+            parents[v1] = None
+
+        while len(queue) > 0:
+            s = queue.pop(0)
+            visited[s] = True
+            for adj in self._vertices[s]:
+                adj_vertex = adj.vertex
+                if not visited[adj_vertex]:
+                    visited[adj_vertex] = True
+                    queue.append(adj_vertex)
+                    parents[adj_vertex] = s
+                elif parents[s] != adj_vertex:
+                    # if the ajd_vertex has been already visited,
+                    # and it is not the parent of current vertex,
+                    # then there is a cycle
+                    return True
+        return False
+
+    def _has_cycles_dfs(self, vertex: str, visited: dict, parent: str) -> bool:
+        """This is recursive function that uses the dictionary
+        visited and the parent of the vertices to detect
+        cycle in subgraph reachable from vertex v."""
+
+        # Mark the current vertex as visited
+        visited[vertex] = True
+        # Recur for all the vertices
+        # adjacent to this vertex
+        for adj in self._vertices[vertex]:
+            adj_vertex = adj.vertex
+            # If the node is not visited then recurse on it
+            if not visited[adj_vertex]:
+                if self._has_cycles_dfs(adj_vertex, visited, vertex):
+                    return True
+            elif parent != adj_vertex:
+                # if the ajd_vertex has been already visited,
+                # and it is not the parent of current vertex,
+                # then there is a cycle
+                return True
+        print()
+        return False
+
+    def _has_cycles_directed(self, vertex: str, visited: dict, rec_stack: dict) -> bool:
+        """detects a cycle in a directed graph using the
+        dfs alg. Moreover, visited and rec_stack allow us
+        to detect if a vertex has been previously visited."""
+
+        # Mark the current vertex as visited
+        visited[vertex] = True
+        rec_stack[vertex] = True
+        # Recur for all the vertices
+        # adjacent to this vertex
+        for adj in self._vertices[vertex]:
+            adj_vertex = adj.vertex
+            # If the node is not visited then recurse on it
+            if not visited[adj_vertex]:
+                if self._has_cycles_directed(adj_vertex, visited, rec_stack):
+                    return True
+            elif rec_stack[adj_vertex]:
+                return True
+        # The node needs to be popped from
+        # recursion stack before function ends
+        rec_stack[vertex] = False
+        return False
+
+    def has_cycles(self, alg: str = 'dfs') -> bool:
+        """returns True if the graph contains a cycle, False eoc"""
+        print(self._directed)
+        visited = {}
+        recursion_stack = {}
+
+        for v1 in self._vertices:
+            visited[v1] = False
+            # we will only use it for directed graphs
+            recursion_stack[v1] = False
+
+        # Call the recursive helper
+        # function to detect cycle in different
+        # DFS trees
+        for v1 in self._vertices:
+            if not visited[v1]:
+                if self._directed:
+                    result = self._has_cycles_directed(v1, visited, recursion_stack)
+                else:
+                    if alg == 'dfs':
+                        result = self._has_cycles_dfs(v1, visited, None)
+                    else:
+                        result = self._has_cycles_bfs(v1, visited)
+
+                if result:
+                    return True
+
+        return False
+
+    def min_distance(self, distances: dict, visited: dict) -> int:
+        """ This function is used from dijkstra.
+        It returns the vertex (index) whose associated value in
+        the dictionary distances is the smallest value. We
+        only consider the set of vertices that have not been visited"""
+        # Initialize minimum distance for next node
+        min_distance = math.inf
+        min_vertex = None
+
+        # returns the vertex with minimum distance from the non-visited vertices
+        for vertex in self._vertices.keys():
+            if distances[vertex] <= min_distance and not visited[vertex]:
+                min_distance = distances[vertex]  # update the new smallest
+                min_vertex = vertex  # update the index of the smallest
+
+        return min_vertex
+
+    def dijkstra(self, origin: object) -> None:
+        visited = {}  # for each vertex (key), the value is a boolean indicating if the vertex has been visited
+        previous = {}  # for each vertex (key), the value is the previous node in the minimum path from origin
+        distances = {}  # for each vertex (key), the value is minimum distance in the minimum path from origin
+
+        # initialize dictionaries
+        for v in self._vertices.keys():
+            visited[v] = False
+            previous[v] = None
+            distances[v] = math.inf
+
+        # The distance from origin to itself is 0
+        distances[origin] = 0
+
+        for _ in range(len(self._vertices)):
+            # pick the non-visited vertex with minimum distance
+            u = self.min_distance(distances, visited)
+            visited[u] = True
+            # get the adjacent vertices of u
+            for adj in self._vertices[u]:
+                i = adj._vertex
+                w = adj._weight
+                # for non-visited vertex, we have to check if its distance is greater than the distance from u
+                if not visited[i] and distances[i] > distances[u] + w:
+                    # we must update because its distance is greater than the new distance
+                    distances[i] = distances[u] + w
+                    previous[i] = u
+
+        # Finally, we print the minimum path from origin to the other vertices
+        self.print_solution(distances, previous, origin)
+
+        return distances, previous
+
+    def print_solution(self, distances: dict, previous: dict, origin: object):
+        """Both Dijkstra and Bellman-Ford algorithms use this function.
+        For each vertex, the function is able to rebuild the reverse path from i to origin.
+        To do this, the function only needs to read the value associated to the vertex in the dictionary
+        previous until to reach a vertex whouse associated value is None (origin)"""
+        print("Minimum path from ", origin)
+
+        for i in self._vertices.keys():
+            if distances[i] == math.inf:
+                print("There is not path from ", origin, ' to ', i)
+            else:
+                # minimum_path is the list which contains the minimum path from origin to i
+                minimum_path = []
+                prev = previous[i]
+                # this loop helps us to build the path
+                while prev is not None:
+                    minimum_path.insert(0, prev)
+                    prev = previous[prev]
+
+                # we append the last vertex, which is i
+                minimum_path.append(i)
+
+                # we print the path from v to i and the distance
+                print(origin, '->', i, ":", minimum_path, distances[i])
+
+    def bellmanford(self, origin: object) -> None:
+        """Bellman-Ford algorithm for minimum path"""
+        previous = {}
+        distances = {}
+        for v in self._vertices.keys():
+            previous[v] = None
+            distances[v] = math.inf
+        distances[origin] = 0
+
+        for _ in range(len(self._vertices) - 1):
+            for u in self._vertices.keys():
+                # get all adjacent vertices of u
+                for adj in self._vertices[u]:
+                    v = adj.vertex
+                    w = adj.weight
+                    if distances[v] > distances[u] + w:
+                        distances[v] = distances[u] + w
+                        previous[v] = u
+
+        # final review to check if there is a solution, or there is a negative cicle (therefore, there is no solution)
+        for u in self._vertices.keys():
+            for adj in self._vertices[u]:
+                v = adj._vertex
+                w = adj._weight
+                if distances[v] > distances[u] + w:
+                    # There is at least a negative cicle.
+                    print('There is no solution ', origin)
+                    return False
+
+        self.print_solution(distances, previous, origin)
+        return distances, previous
+
+    def minimum_path(self, start: object, end: object) -> list:
+        """ returns a list containing the path from star to end.
+        It also returns the distance of the path. If the path
+        does not exist, it returns an empty list and infinito"""
+        if start not in self._vertices.keys():
+            print(start, ' does not exist!!!')
+            return None, None
+        if end not in self._vertices.keys():
+            print(end, ' does not exist!!!')
+            return None, None
+
+        distances, previous = self.dijkstra(start)
+        if distances[end] == math.inf:
+            return [], math.inf
+
+        result = [end]
+        prev = previous[end]
+        while prev is not None:
+            result.insert(0, prev)
+            prev = previous[prev]
+
+        return result, distances[end]
```

### Comparing `graphdisplay-0.3.6/graphdisplay/json_manager.py` & `graphdisplay-0.4.0/graphdisplay/json_manager.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,169 +1,169 @@
-import os
-import json
-import tkinter as tk
-from tkinter import messagebox
-from datetime import datetime
-
-class JsonManager:
-    def __init__(self, parent, graphgui):
-        self.__JSON_SAVE_DIR = os.path.join(os.path.dirname(__file__), 'store/')
-
-        self.graphgui = graphgui
-        self.__parent = parent
-        self.current_data_id = None
-        self.current_data = None
-
-        try:
-            with open(self.__JSON_SAVE_DIR + '../permanent.json', "r", encoding="utf-8", newline="") as file:
-                self.__permanent = json.load(file)
-        except FileNotFoundError:
-            self.__permanent = {}
-
-    def update_permanent(self):
-        with open(self.__JSON_SAVE_DIR + '../permanent.json', "w", encoding="utf-8", newline="") as file:
-            json.dump(self.__permanent, file, indent=4)
-
-    def delete_permanent(self, name: str):
-        del self.__permanent[name]
-        os.remove(self.__JSON_SAVE_DIR + name + '.json')
-        self.update_permanent()
-
-    def add_permanent(self, name: str):
-        self.__permanent[name] = str(datetime.now())
-        self.update_permanent()
-
-    def get_data(self, file_name: str) -> dict:
-        try:
-            with open(self.__JSON_SAVE_DIR + file_name + '.json', "r", encoding="utf-8", newline="") as file:
-                data = json.load(file)
-        except FileNotFoundError:
-            data = None
-        self.current_data_id = file_name
-        self.current_data = data
-        return data
-
-    def save_data(self, file_name: str, data: dict):
-        with open(self.__JSON_SAVE_DIR + file_name + '.json', "w", encoding="utf-8", newline="") as file:
-            json.dump(data, file, indent=4)
-
-    def generate_save_window(self, current_position: dict):
-        SaveWindow(self.__parent, self, current_position)
-
-    def generate_load_window(self):
-        LoadWindow(self.__parent, self)
-
-    def generate_delete_window(self):
-        DeleteWindow(self.__parent, self)
-
-class DeleteWindow(tk.Toplevel):
-    def __init__(self, root, json_manager: JsonManager):
-        super().__init__(root)
-        self.title("Delete save")
-        self.geometry("200x100")
-        self.resizable(False, False)
-        self.__manager = json_manager
-        self.configure(background=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
-
-        self.__label = tk.Label(self, text="Select save:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
-        self.__label.pack(side=tk.TOP)
-
-        options = list(self.__manager._JsonManager__permanent.keys())
-        if len(options) > 0:
-            self.__selecion = tk.StringVar(self)
-            self.__selecion.set(options[0])
-            self.__option_menu = tk.OptionMenu(self, self.__selecion, *options)
-            self.__option_menu.config(bg=self.__manager.graphgui._BUTTON_COLOR)
-            self.__option_menu.pack(side=tk.TOP)
-
-            self.__button = tk.Button(self, text="Delete", command=self.__on_delete, bg=self.__manager.graphgui._BUTTON_COLOR)
-            self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
-
-            self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
-            self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
-
-    def __on_delete(self):
-        selection = self.__selecion.get()
-        if selection not in self.__manager._JsonManager__permanent:
-            messagebox.showerror("Error", "The selected save does not exist")
-            self.destroy()
-        self.__manager.delete_permanent(selection)
-        messagebox.showinfo("Confirm", f"Removed : {selection}")
-
-    def __on_cancel(self):
-        self.destroy()
-
-class LoadWindow(tk.Toplevel):
-    def __init__(self, root, json_manager: JsonManager):
-        super().__init__(root)
-        self.title("Load")
-        self.geometry("200x100")
-        self.resizable(False, False)
-        self.__manager = json_manager
-        self.configure(background=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
-
-        self.__label = tk.Label(self, text="Select save:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
-        self.__label.pack(side=tk.TOP)
-
-        options = list(self.__manager._JsonManager__permanent.keys())
-        if len(options) > 0:
-            self.__selecion = tk.StringVar(self)
-            self.__selecion.set(options[0])
-            self.__option_menu = tk.OptionMenu(self, self.__selecion, *options)
-            self.__option_menu.config(bg=self.__manager.graphgui._BUTTON_COLOR)
-            self.__option_menu.pack(side=tk.TOP)
-
-            self.__button = tk.Button(self, text="Load", command=self.__on_load, bg=self.__manager.graphgui._BUTTON_COLOR)
-            self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
-
-            self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
-            self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
-
-    def __on_load(self):
-        selection = self.__selecion.get()
-        if selection not in self.__manager._JsonManager__permanent:
-            messagebox.showerror("Error", "The selected save does not exist")
-            self.destroy()
-        self.new_position = self.__manager.get_data(selection)
-        self.__manager.graphgui.display_reset(self.new_position)
-
-    def __on_cancel(self):
-        self.destroy()
-
-class SaveWindow(tk.Toplevel):
-    def __init__(self, root, json_manager: JsonManager, graph_position: dict):
-        super().__init__(root)
-        self.title("Save")
-        self.geometry("200x100")
-        self.resizable(False, False)
-        self.__current_position = graph_position
-        self.__manager = json_manager
-        self.configure(bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
-        self.__root = root
-        self.bind("<Return>", self.__on_save)
-
-        self.__label = tk.Label(self, text="Save as:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
-        self.__label.pack(side=tk.TOP)
-
-        self.__entry = tk.Entry(self)
-        self.__entry.pack(side=tk.TOP)
-
-        self.__button = tk.Button(self, text="Save", command=self.__on_save, bg=self.__manager.graphgui._BUTTON_COLOR)
-        self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
-
-        self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
-        self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
-
-    def __on_save(self, event = None):
-        word = self.__entry.get()
-        word = word.strip()
-        word = word.replace(" ", "_")
-        if word:
-            self.__manager.save_data(word, self.__current_position)
-            self.__manager.add_permanent(word)
-            messagebox.showinfo("Confirmación", f"Guardado : {word}")
-        else:
-            messagebox.showerror("Error", "You must enter a name")
-        self.destroy()
-
-    def __on_cancel(self):
+import os
+import json
+import tkinter as tk
+from tkinter import messagebox
+from datetime import datetime
+
+class JsonManager:
+    def __init__(self, parent, graphgui):
+        self.__JSON_SAVE_DIR = os.path.join(os.path.dirname(__file__), 'store/')
+
+        self.graphgui = graphgui
+        self.__parent = parent
+        self.current_data_id = None
+        self.current_data = None
+
+        try:
+            with open(self.__JSON_SAVE_DIR + '../permanent.json', "r", encoding="utf-8", newline="") as file:
+                self.__permanent = json.load(file)
+        except FileNotFoundError:
+            self.__permanent = {}
+
+    def update_permanent(self):
+        with open(self.__JSON_SAVE_DIR + '../permanent.json', "w", encoding="utf-8", newline="") as file:
+            json.dump(self.__permanent, file, indent=4)
+
+    def delete_permanent(self, name: str):
+        del self.__permanent[name]
+        os.remove(self.__JSON_SAVE_DIR + name + '.json')
+        self.update_permanent()
+
+    def add_permanent(self, name: str):
+        self.__permanent[name] = str(datetime.now())
+        self.update_permanent()
+
+    def get_data(self, file_name: str) -> dict:
+        try:
+            with open(self.__JSON_SAVE_DIR + file_name + '.json', "r", encoding="utf-8", newline="") as file:
+                data = json.load(file)
+        except FileNotFoundError:
+            data = None
+        self.current_data_id = file_name
+        self.current_data = data
+        return data
+
+    def save_data(self, file_name: str, data: dict):
+        with open(self.__JSON_SAVE_DIR + file_name + '.json', "w", encoding="utf-8", newline="") as file:
+            json.dump(data, file, indent=4)
+
+    def generate_save_window(self, current_position: dict):
+        SaveWindow(self.__parent, self, current_position)
+
+    def generate_load_window(self):
+        LoadWindow(self.__parent, self)
+
+    def generate_delete_window(self):
+        DeleteWindow(self.__parent, self)
+
+class DeleteWindow(tk.Toplevel):
+    def __init__(self, root, json_manager: JsonManager):
+        super().__init__(root)
+        self.title("Delete save")
+        self.geometry("200x100")
+        self.resizable(False, False)
+        self.__manager = json_manager
+        self.configure(background=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
+
+        self.__label = tk.Label(self, text="Select save:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
+        self.__label.pack(side=tk.TOP)
+
+        options = list(self.__manager._JsonManager__permanent.keys())
+        if len(options) > 0:
+            self.__selecion = tk.StringVar(self)
+            self.__selecion.set(options[0])
+            self.__option_menu = tk.OptionMenu(self, self.__selecion, *options)
+            self.__option_menu.config(bg=self.__manager.graphgui._BUTTON_COLOR)
+            self.__option_menu.pack(side=tk.TOP)
+
+            self.__button = tk.Button(self, text="Delete", command=self.__on_delete, bg=self.__manager.graphgui._BUTTON_COLOR)
+            self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
+
+            self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
+            self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
+
+    def __on_delete(self):
+        selection = self.__selecion.get()
+        if selection not in self.__manager._JsonManager__permanent:
+            messagebox.showerror("Error", "The selected save does not exist")
+            self.destroy()
+        self.__manager.delete_permanent(selection)
+        messagebox.showinfo("Confirm", f"Removed : {selection}")
+
+    def __on_cancel(self):
+        self.destroy()
+
+class LoadWindow(tk.Toplevel):
+    def __init__(self, root, json_manager: JsonManager):
+        super().__init__(root)
+        self.title("Load")
+        self.geometry("200x100")
+        self.resizable(False, False)
+        self.__manager = json_manager
+        self.configure(background=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
+
+        self.__label = tk.Label(self, text="Select save:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
+        self.__label.pack(side=tk.TOP)
+
+        options = list(self.__manager._JsonManager__permanent.keys())
+        if len(options) > 0:
+            self.__selecion = tk.StringVar(self)
+            self.__selecion.set(options[0])
+            self.__option_menu = tk.OptionMenu(self, self.__selecion, *options)
+            self.__option_menu.config(bg=self.__manager.graphgui._BUTTON_COLOR)
+            self.__option_menu.pack(side=tk.TOP)
+
+            self.__button = tk.Button(self, text="Load", command=self.__on_load, bg=self.__manager.graphgui._BUTTON_COLOR)
+            self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
+
+            self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
+            self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
+
+    def __on_load(self):
+        selection = self.__selecion.get()
+        if selection not in self.__manager._JsonManager__permanent:
+            messagebox.showerror("Error", "The selected save does not exist")
+            self.destroy()
+        self.new_position = self.__manager.get_data(selection)
+        self.__manager.graphgui.display_reset(self.new_position)
+
+    def __on_cancel(self):
+        self.destroy()
+
+class SaveWindow(tk.Toplevel):
+    def __init__(self, root, json_manager: JsonManager, graph_position: dict):
+        super().__init__(root)
+        self.title("Save")
+        self.geometry("200x100")
+        self.resizable(False, False)
+        self.__current_position = graph_position
+        self.__manager = json_manager
+        self.configure(bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
+        self.__root = root
+        self.bind("<Return>", self.__on_save)
+
+        self.__label = tk.Label(self, text="Save as:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
+        self.__label.pack(side=tk.TOP)
+
+        self.__entry = tk.Entry(self)
+        self.__entry.pack(side=tk.TOP)
+
+        self.__button = tk.Button(self, text="Save", command=self.__on_save, bg=self.__manager.graphgui._BUTTON_COLOR)
+        self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
+
+        self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
+        self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
+
+    def __on_save(self, event = None):
+        word = self.__entry.get()
+        word = word.strip()
+        word = word.replace(" ", "_")
+        if word:
+            self.__manager.save_data(word, self.__current_position)
+            self.__manager.add_permanent(word)
+            messagebox.showinfo("Confirmación", f"Guardado : {word}")
+        else:
+            messagebox.showerror("Error", "You must enter a name")
+        self.destroy()
+
+    def __on_cancel(self):
         self.destroy()
```

### Comparing `graphdisplay-0.3.6/graphdisplay.egg-info/PKG-INFO` & `graphdisplay-0.4.0/graphdisplay.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,103 @@
-Metadata-Version: 2.1
-Name: graphdisplay
-Version: 0.3.6
-Summary: Librería para representar visualmente grafos de tipo diccionario
-Home-page: https://github.com/seniorbeto
-Author: Alberto Penas Díaz
-Author-email: albertopenasdiaz@gmail.com
-License: MIT
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-
-# graphdisplay
-
-## Resumen
-
-graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos a los alumnos de Estructuras de Datos y Algoritmos. 
-Actualmente solo soporta la visualización de grafos implementados a través de un diccionario, tal y como se aportan como código base en la asignatura. 
-
-## ¿Quieres contribuir?
-
-Este es un proyecto de código abierto hecho por y para estudiantes así que cualquier ayuda, comentario o sugerencia es bienvenido. La mejor manera de contribuir es añadir los bugs que os encontréis 
-en el apartado de Issues pero también estoy completamente abierto a responder cualquier duda o ayuda desde mi correo personal (disponible en mi perfil de github). ¡Muchas gracias de antemano!
-
-## Método de uso 
-
-Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
-tkinter y math (que muchas veces vienen instaladas por defecto en python). 
-
-Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. Una vez hecho esto, se debe instanciar un grafo de tipo diccionario
-para finalmente introducirlo como argumento al instanciar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón 
-para una mejor visualización. **Al desplazar los vértices por la pantalla y fijar su posición, si se cierra la ventana y se vuelve a abrir, el grafo seguirá con la forma con la que se ha movido
-antes.**. Cabe destacar que, únicamente es necesario especificar como argumento el grafo que se quiere representar pero además hay otros ajustes que pueden ser útiles a la hora de mostrar 
-grafos grandes y complejos:
-+ graph: es el objeto de tipo grafo que se va a representar **ES MUY IMPORTANTE** que el grafo que se introduce como argumento sea el implementado en base al código base de la asignatura. Si alguno
-de los atributos cambiase de nombre, el programa no funcionaría correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA) o utilizar la 
-implementación de grafos que viene por defecto con el paquete.
-+ node_radius: el radio de cada vértice del grafo, por defecto es 40 y puede tomar cualquier valor entero entre 10 y 100
-+ scr_width: el tamaño en píxeles del ancho de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
-+ scr_width: el tamaño en píxeles de la altura de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
-
-Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
-```python
-g = Graph([1, 2, 3])
-g.addEdge(1, 2)
-g.addEdge(2, 3)
-
-# Para representar el grafo con todos los valores por defecto
-GraphGUI(g)
-
-# Para ajustar el radio de los nodos a 32, el ancho y largo de la pantalla a 700
-GraphGUI(g, 32, 700, 700)
-
-# Para ajustar únicamente el ancho de la pantalla a 200 píxeles
-GraphGUI(g, scr_width=200)
-```
-
-Además, también es posible generar este tipo de grafos a través de la librería. Importándolo con `from graphdisplay import Graph`, se puede instanciar un objeto de tipo Graph, pasándole como
-argumento una lista de los vértices del grafo para después, añadirle las aristas con el método `add_edge`, con los vértices que conecta la arista además del valor/coste de la arista.
-
-## Ejemplo de uso
-
-Para instanciar un grafo de tipo diccionario, se debe hacer de la siguiente manera: 
-
-```python
-labels = ['A', 'B', 'C', 'D', 'E']
-g = Graph(labels)
-
-# Now, we add the edges
-g.addEdge('A', 'C', 12)  # A->(12)C
-g.addEdge('A', 'D', 60)  # A->(60)D
-g.addEdge('B', 'A', 10)  # B->(10)A
-g.addEdge('C', 'B', 20)  # C->(20)B
-g.addEdge('C', 'D', 32)  # C->(32)D
-g.addEdge('E', 'A', 7)   # E->(7)A
-g.addEdge('A', 'E', 50)  # A->(50)E
-```
-
-Si queremos mostrar la pantalla, basta con instanciar un objeto de tipo GraphGUI, pasándole como argumento el grafo que queremos mostrar: 
-
-```python
-    GraphGUI(g)
-```
-Y nos mostrará la ventana:
-
-<img src="https://user-images.githubusercontent.com/94072018/236611009-de477dd9-d2dd-4247-80fa-dfc3e7a86a4b.png" width="400" height="400">
-
-Sabiendo cómo instanciar grafos, podemos ahora representar objetos algo más complicados ajustando un poco los parámetros de la instancia GraphGUI. En este caso: `GraphGUI(my_gragph, 30, 1000, 1000)`
-
-<img src="https://user-images.githubusercontent.com/94072018/236611227-2b812c07-7eac-4922-85a5-17cb6e13daea.png" width="550" height="550">
-
+Metadata-Version: 2.1
+Name: graphdisplay
+Version: 0.4.0
+Summary: Librería para representar visualmente grafos de tipo diccionario
+Home-page: https://github.com/seniorbeto
+Author: Alberto Penas Díaz
+Author-email: albertopenasdiaz@gmail.com
+License: MIT
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+
+# graphdisplay
+
+## Resumen
+
+graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos a los alumnos de Estructuras de Datos y Algoritmos. 
+Actualmente solo soporta la visualización de grafos implementados a través de un diccionario, tal y como se aportan como código base en la asignatura. 
+
+## ¿Quieres contribuir?
+
+Este es un proyecto de código abierto hecho por y para estudiantes así que cualquier ayuda, comentario o sugerencia es bienvenido. La mejor manera de contribuir es añadir los bugs que os encontréis 
+en el apartado de Issues pero también estoy completamente abierto a responder cualquier duda o ayuda desde mi correo personal (disponible en mi perfil de github). ¡Muchas gracias de antemano!
+
+## Método de uso 
+
+Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
+tkinter y math (que muchas veces vienen instaladas por defecto en python). 
+
+Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. Una vez hecho esto, se debe instanciar un grafo de tipo diccionario
+para finalmente introducirlo como argumento al instanciar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón 
+para una mejor visualización. Cabe destacar que, únicamente es necesario especificar como argumento el grafo que se quiere representar pero además hay otros ajustes que pueden ser útiles a la hora de mostrar 
+grafos grandes y complejos:
++ graph: es el objeto de tipo grafo que se va a representar **ES MUY IMPORTANTE** que el grafo que se introduce como argumento sea el implementado en base al código base de la asignatura. Si alguno
+de los atributos cambiase de nombre, el programa no funcionaría correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA) o utilizar la 
+implementación de grafos que viene por defecto con el paquete.
++ node_radius: el radio de cada vértice del grafo, por defecto es 40 y puede tomar cualquier valor entero entre 10 y 100
++ scr_width: el tamaño en píxeles del ancho de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
++ scr_width: el tamaño en píxeles de la altura de la ventana, por defecto es 600 y puede tomar cualquier valor entero entre 200 y 1000
++ theme: el tema de la ventana, por defecto es 'brown' y no voy a mencionarlos todos porque hay muchos y me da pereza.
+
+Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
+```python
+g = Graph([1, 2, 3])
+g.addEdge(1, 2)
+g.addEdge(2, 3)
+
+# Para representar el grafo con todos los valores por defecto
+GraphGUI(g)
+
+# Para ajustar el radio de los nodos a 32, el ancho y largo de la pantalla a 700
+GraphGUI(g, 32, 700, 700)
+
+# Para ajustar únicamente el ancho de la pantalla a 200 píxeles
+GraphGUI(g, scr_width=200)
+```
+
+Además, también es posible generar este tipo de grafos a través de la librería. Importándolo con `from graphdisplay import Graph`, se puede instanciar un objeto de tipo Graph, pasándole como
+argumento una lista de los vértices del grafo para después, añadirle las aristas con el método `addEdge`, con los vértices que conecta la arista además del valor/coste de la arista.
+
+## Funcionalidades
+Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
+éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
+instaciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
+Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
+tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón save y nombrando el guardado) para
+después poder cargarlo en cualquier momento.
+## Ejemplo de uso
+
+Para instanciar un grafo de tipo diccionario, se debe hacer de la siguiente manera: 
+
+```python
+labels = ['A', 'B', 'C', 'D', 'E']
+g = Graph(labels)
+
+# Now, we add the edges
+g.addEdge('A', 'C', 12)  # A->(12)C
+g.addEdge('A', 'D', 60)  # A->(60)D
+g.addEdge('B', 'A', 10)  # B->(10)A
+g.addEdge('C', 'B', 20)  # C->(20)B
+g.addEdge('C', 'D', 32)  # C->(32)D
+g.addEdge('E', 'A', 7)   # E->(7)A
+g.addEdge('A', 'E', 50)  # A->(50)E
+```
+
+Si queremos mostrar la pantalla, basta con instanciar un objeto de tipo GraphGUI, pasándole como argumento el grafo que queremos mostrar: 
+
+```python
+    GraphGUI(g)
+```
+Y nos mostrará la ventana:
+
+<img src="https://user-images.githubusercontent.com/94072018/236611009-de477dd9-d2dd-4247-80fa-dfc3e7a86a4b.png" width="400" height="400">
+
+Sabiendo cómo instanciar grafos, podemos ahora representar objetos algo más complicados ajustando un poco los parámetros de la instancia GraphGUI. En este caso: `GraphGUI(my_gragph, 30, 1000, 1000)`
+
+<img src="https://user-images.githubusercontent.com/94072018/236611227-2b812c07-7eac-4922-85a5-17cb6e13daea.png" width="550" height="550">
+
```

### Comparing `graphdisplay-0.3.6/setup.py` & `graphdisplay-0.4.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-import pathlib
-from setuptools import find_packages, setup
-
-HERE = pathlib.Path(__file__).parent
-
-VERSION = '0.3.6'
-PACKAGE_NAME = 'graphdisplay'
-AUTHOR = 'Alberto Penas Díaz'
-AUTHOR_EMAIL = 'albertopenasdiaz@gmail.com'
-URL = 'https://github.com/seniorbeto'
-
-LICENSE = 'MIT' #Tipo de licencia
-DESCRIPTION = 'Librería para representar visualmente grafos de tipo diccionario'
-LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8')
-LONG_DESC_TYPE = "text/markdown"
-
-
-INSTALL_REQUIRES = [
-      'tk==0.1.1'
-      ]
-
-setup(
-    name=PACKAGE_NAME,
-    version=VERSION,
-    description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
-    long_description_content_type=LONG_DESC_TYPE,
-    author=AUTHOR,
-    author_email=AUTHOR_EMAIL,
-    url=URL,
-    #install_requires=INSTALL_REQUIRES,
-    license=LICENSE,
-    packages=find_packages(),
-    include_package_data=True,
-    classifiers=['Programming Language :: Python',
-                 'Programming Language :: Python :: 2.7',
-                 'Programming Language :: Python :: 3.3',
-                 'Programming Language :: Python :: 3.4',
-                 'Programming Language :: Python :: 3.5',
-                 'Programming Language :: Python :: 3.6',
-                 'Programming Language :: Python :: 3.7']
+import pathlib
+from setuptools import find_packages, setup
+from graphdisplay.general_config import *
+
+HERE = pathlib.Path(__file__).parent
+
+VERSION = VERSION
+PACKAGE_NAME = 'graphdisplay'
+AUTHOR = 'Alberto Penas Díaz'
+AUTHOR_EMAIL = 'albertopenasdiaz@gmail.com'
+URL = 'https://github.com/seniorbeto'
+
+LICENSE = 'MIT' #Tipo de licencia
+DESCRIPTION = 'Librería para representar visualmente grafos de tipo diccionario'
+LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8')
+LONG_DESC_TYPE = "text/markdown"
+
+
+INSTALL_REQUIRES = [
+      'tk==0.1.1'
+      ]
+
+setup(
+    name=PACKAGE_NAME,
+    version=VERSION,
+    description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    long_description_content_type=LONG_DESC_TYPE,
+    author=AUTHOR,
+    author_email=AUTHOR_EMAIL,
+    url=URL,
+    #install_requires=INSTALL_REQUIRES,
+    license=LICENSE,
+    packages=find_packages(),
+    include_package_data=True,
+    classifiers=['Programming Language :: Python',
+                 'Programming Language :: Python :: 2.7',
+                 'Programming Language :: Python :: 3.3',
+                 'Programming Language :: Python :: 3.4',
+                 'Programming Language :: Python :: 3.5',
+                 'Programming Language :: Python :: 3.6',
+                 'Programming Language :: Python :: 3.7']
 )
```

