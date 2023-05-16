# Comparing `tmp/upe-0.0.1.tar.gz` & `tmp/upe-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upe-0.0.1.tar", last modified: Tue May 16 19:33:18 2023, max compression
+gzip compressed data, was "upe-0.0.2.tar", last modified: Tue May 16 19:47:09 2023, max compression
```

## Comparing `upe-0.0.1.tar` & `upe-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 19:33:18.943542 upe-0.0.1/
--rw-rw-rw-   0        0        0      191 2023-05-16 19:33:18.943542 upe-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 19:33:18.927918 upe-0.0.1/libname/
--rw-rw-rw-   0        0        0       26 2023-05-16 18:56:14.000000 upe-0.0.1/libname/__init__.py
--rw-rw-rw-   0        0        0    26949 2023-05-16 19:29:03.000000 upe-0.0.1/libname/nqueen.py
--rw-rw-rw-   0        0        0       42 2023-05-16 19:33:18.943542 upe-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      428 2023-05-16 19:32:51.000000 upe-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:33:18.943542 upe-0.0.1/upe.egg-info/
--rw-rw-rw-   0        0        0      191 2023-05-16 19:33:18.000000 upe-0.0.1/upe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      154 2023-05-16 19:33:18.000000 upe-0.0.1/upe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 19:33:18.000000 upe-0.0.1/upe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 19:33:18.000000 upe-0.0.1/upe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 19:47:09.961661 upe-0.0.2/
+-rw-rw-rw-   0        0        0      191 2023-05-16 19:47:09.960695 upe-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 19:47:09.947660 upe-0.0.2/libname/
+-rw-rw-rw-   0        0        0       26 2023-05-16 18:56:14.000000 upe-0.0.2/libname/__init__.py
+-rw-rw-rw-   0        0        0    28541 2023-05-16 19:45:10.000000 upe-0.0.2/libname/nqueen.py
+-rw-rw-rw-   0        0        0       42 2023-05-16 19:47:09.961661 upe-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      428 2023-05-16 19:46:04.000000 upe-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 19:47:09.959660 upe-0.0.2/upe.egg-info/
+-rw-rw-rw-   0        0        0      191 2023-05-16 19:47:09.000000 upe-0.0.2/upe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2023-05-16 19:47:09.000000 upe-0.0.2/upe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 19:47:09.000000 upe-0.0.2/upe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 19:47:09.000000 upe-0.0.2/upe.egg-info/top_level.txt
```

### Comparing `upe-0.0.1/libname/nqueen.py` & `upe-0.0.2/libname/nqueen.py`

 * *Files 3% similar despite different names*

```diff
@@ -900,8 +900,62 @@
     # f2 = input('f2 : ')
 
     result = unify(f1, f2)
     if not result:
         print('The process of Unification failed!')
     else:
         print('The process of Unification successful!')
-        print(result)''')
+        print(result)''')
+    
+def dl():
+    print('''from numpy import loadtxt
+from tensorflow.keras.models import Sequential
+from tensorflow.keras.layers import Dense
+# load the dataset
+dataset = loadtxt('pima-indians-diabetes.csv', delimiter=',')
+# split into input (X) and output (y) variables
+X = dataset[:,0:8]
+y = dataset[:,8]
+model = Sequential()
+model.add(Dense(12, input_shape=(8,), activation='relu'))
+model.add(Dense(8, activation='relu'))
+model.add(Dense(1, activation='sigmoid'))
+model.compile(loss='binary_crossentropy', optimizer='adam', metrics=['accuracy'])
+model.fit(X, y, epochs=150, batch_size=10)
+accuracy = model.evaluate(X, y)
+print('Accuracy: %.2f' % (accuracy*100))''')
+    
+def montyhall():
+    print('''import random
+
+def monty_hall(choice):
+  prize=['goat','car','goat']
+  random.shuffle(prize)
+
+  while True:
+    opening_door=random.randrange(len(prize))
+    if prize[opening_door]!='car' and choice-1 !=opening_door:
+      break
+  
+  opening_door=opening_door+1
+  print('We are opening the door number-%d' % (opening_door))
+
+  options=[1,2,3]
+  options.remove(choice)
+  options.remove(opening_door)
+  switching_door=options[0]
+
+  print('Now, do you want to switch to door number-%d? (yes/no)' %(switching_door))
+
+  answer = input()
+  if answer == 'yes':
+      result = switching_door - 1
+  else:
+      result = choice - 1
+    
+    # Displaying the player's prize 
+  print('And your prize is ....', prize[result].upper())
+
+choice = int(input('Which door do you want to choose? (1,2,3): '))
+
+# Playing game
+play_monty_hall(choice)''')
```

