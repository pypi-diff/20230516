# Comparing `tmp/pyshs-0.3.3.tar.gz` & `tmp/pyshs-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyshs-0.3.3.tar", last modified: Tue Jul 26 08:35:53 2022, max compression
+gzip compressed data, was "pyshs-0.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyshs-0.3.3.tar` & `pyshs-0.3.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1207 2022-07-10 16:38:42.992671 pyshs-0.3.3/.github/workflows/test.yml
--rw-r--r--   0        0        0       33 2021-04-19 18:31:27.000000 pyshs-0.3.3/.gitignore
--rw-r--r--   0        0        0     1082 2021-07-28 16:57:50.603926 pyshs-0.3.3/LICENSE
--rw-r--r--   0        0        0     1740 2022-07-26 08:33:20.000000 pyshs-0.3.3/README.md
--rw-r--r--   0        0        0  3875214 2022-07-20 21:09:28.437466 pyshs-0.3.3/docs/Exemple PySHS.ipynb
--rwxr-xr-x   0        0        0   329030 2017-12-14 09:37:50.000000 pyshs-0.3.3/docs/bdd2011.sav
--rw-r--r--   0        0        0     6436 2022-07-20 21:02:06.300396 pyshs-0.3.3/docs/resultats.xlsx
--rw-r--r--   0        0        0      453 2022-07-21 13:40:24.000000 pyshs-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1659 2022-07-26 08:33:10.000000 pyshs-0.3.3/pyshs/__init__.py
--rw-r--r--   0        0        0    32435 2022-07-26 08:32:27.000000 pyshs-0.3.3/pyshs/_core.py
--rw-r--r--   0        0        0     1602 2022-07-10 16:54:22.415582 pyshs-0.3.3/test/test_pyshs.py
--rw-r--r--   0        0        0     2215 1970-01-01 00:00:00.000000 pyshs-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1207 2022-07-10 16:38:42.992671 pyshs-0.3.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0       33 2021-04-19 18:31:27.000000 pyshs-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1082 2021-07-28 16:57:50.603926 pyshs-0.3.4/LICENSE
+-rw-r--r--   0        0        0     1740 2022-07-26 08:33:20.000000 pyshs-0.3.4/README.md
+-rw-r--r--   0        0        0  3875214 2022-07-20 21:09:28.437466 pyshs-0.3.4/docs/Exemple PySHS.ipynb
+-rwxr-xr-x   0        0        0   329030 2017-12-14 09:37:50.000000 pyshs-0.3.4/docs/bdd2011.sav
+-rw-r--r--   0        0        0     6436 2022-07-20 21:02:06.300396 pyshs-0.3.4/docs/resultats.xlsx
+-rw-r--r--   0        0        0      453 2022-07-21 13:40:24.000000 pyshs-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1659 2023-05-16 15:22:54.834209 pyshs-0.3.4/pyshs/__init__.py
+-rw-r--r--   0        0        0    33397 2023-05-16 15:22:02.000000 pyshs-0.3.4/pyshs/_core.py
+-rw-r--r--   0        0        0     1602 2022-07-10 16:54:22.415582 pyshs-0.3.4/test/test_pyshs.py
+-rw-r--r--   0        0        0     2215 1970-01-01 00:00:00.000000 pyshs-0.3.4/PKG-INFO
```

### Comparing `pyshs-0.3.3/.github/workflows/test.yml` & `pyshs-0.3.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyshs-0.3.3/LICENSE` & `pyshs-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyshs-0.3.3/README.md` & `pyshs-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pyshs-0.3.3/docs/Exemple PySHS.ipynb` & `pyshs-0.3.4/docs/Exemple PySHS.ipynb`

 * *Files identical despite different names*

### Comparing `pyshs-0.3.3/docs/bdd2011.sav` & `pyshs-0.3.4/docs/bdd2011.sav`

 * *Files identical despite different names*

### Comparing `pyshs-0.3.3/docs/resultats.xlsx` & `pyshs-0.3.4/docs/resultats.xlsx`

 * *Files identical despite different names*

### Comparing `pyshs-0.3.3/pyshs/__init__.py` & `pyshs-0.3.4/pyshs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,8 +42,8 @@
     likelihood_ratio,
     vers_excel,
     moyenne_ponderee,
     ecart_type_pondere,
     catdes
 )
 
-__version__ = "0.3.3"
+__version__ = "0.3.4"
```

### Comparing `pyshs-0.3.3/pyshs/_core.py` & `pyshs-0.3.4/pyshs/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# modification du 16/05/2023
+
 import warnings
 import math
 from typing import Optional, List
 
 
 import numpy as np
 import pandas as pd
@@ -288,24 +290,29 @@
                 + "%)"
             )
 
     # Ajout des 100% pour la ligne colonne
     t["All"] = t["All"].apply(lambda x: "{} (100%)".format(x))
 
     # Traduire All par Total
-    t.columns = list(t.columns)[:-1] + ["Total"]
-    t.index = list(t.index)[:-1] + ["Total"]
+    t = t.rename(index={"All":"Total"},columns={"All":"Total"})
+    t_absolu = t_absolu.rename(index={"All":"Total"},columns={"All":"Total"})
+    t_pourcentage = t_pourcentage.rename(index={"All":"Total"},columns={"All":"Total"})
+    #t.columns = list(t.columns)[:-1] + ["Total"]
+    #t.index = list(t.index)[:-1] + ["Total"]
 
     # Retour des tableaux non mis en forme
     if debug:
-        return t, t_absolu, t_pourcentage
+        val_p = chi2_contingency(t_absolu.drop("Total").drop("Total", axis=1))[1]
+        return t, t_absolu, t_pourcentage, val_p
 
     # Retour du tableau avec la p-value
     if p:
-        return t, chi2_contingency(t_absolu.drop("All").drop("All", axis=1))[1]
+        val_p = chi2_contingency(t_absolu.drop("Total").drop("Total", axis=1))[1]
+        return t, val_p
 
     # Retour du tableau mis en forme
     return t
 
 
 def tableau_croise_controle(df, cont, c, r, weight=False, chi2=False):
     """
@@ -369,35 +376,38 @@
     tab.index.names = [cont, c]
 
     # Retour du tableau mis en forme
     return tab
 
 
 def tableau_croise_multiple(
-    df, dep, indeps, weight=False, chi2=True, axis=0, ss_total=True
+    df, dep, indeps, weight=False, chi2=True, axis=0, ss_total=True, contenu = "complet"
 ):
     """
-    Tableau croisé multiple.
-    Variable dépendantes vs. plusieurs indépendantes.
+    Tableau croisé multiples variables.
+    Variable dépendantes vs. plusieurs variables indépendantes.
 
     Parameters
     ----------
     df : DataFrame
         Tableau de données
     dep : str or dic
         Variable dépendante en colonne
         Pour les dictionnaires : {nom:label}
     indeps : dict or list
         dictionnaire des variables indépendantes
+        Pour les dictionnaires : {nom:label}
     weight : str, optionnal
         poids optionnel
     axis : int, optionnal
         sens des pourcentages,axis = 1 pour les colonnes
     ss_total : bool, optionnal
         présence de sous totaux
+    contenu : str, optionnal
+        données complètes, brutes ou pourcentages
 
     Returns
     -------
     DataFrame
         mise en forme du tableau croisé.
 
     Notes
@@ -436,18 +446,32 @@
     # Compteur des totaux par croisement
     check_total = []
 
     # Boucle sur les variables indépendantes
     for i in indeps:
         # Tableau croisé pondéré (deux orientations possibles)
         if axis == 0:
-            t, p = tableau_croise(df, i, dep, weight, p=True)
+            t_comp,t_ab,t_per,p = tableau_croise(df,i,dep,weight,debug=True)
+            
+        else:
+            t_comp,t_ab,t_per,p = tableau_croise(df,dep,weight,i,debug=True)
+            t_comp = t_comp.T
+            t_ab = t_ab.T
+            t_per = t_per.T
+            
+        # Sélection du contenu du tableau
+        if contenu == "complet":
+            t = t_comp
+        elif contenu  == "absolu":
+            t = t_ab
+        elif contenu == "pourcentage":
+            t = t_per
         else:
-            t, p = tableau_croise(df, dep, i, weight, p=True)
-            t = t.T
+            print("Erreur dans le format du tableau")
+            return None
 
         # Enlever les sous-totaux si besoin
         if not ss_total:
             t = t.drop("Total")
 
         dis = tri_a_plat(df, i, weight=weight)
 
@@ -458,25 +482,23 @@
         else:
             t_all[indeps[i]] = t
 
     # Création d'un DataFrame
     t_all = pd.concat(t_all)
     t_all.columns.name = ""
     t_all.index.names = ["Variable", "Modalités"]
-    t_all.columns.values[-2] = "Total"
 
     # Alerter sur les totaux différents
     if len(set(check_total)) != 1:
         warnings.warn(
             "Attention, les totaux par tableaux sont différents (valeurs manquantes, UserWarning)"
         )
 
     return t_all
 
-
 def significativite(x, digits=4):
     """
     Mettre en forme la p-value.
 
     Parameters
     ----------
     x : float
@@ -721,22 +743,22 @@
     p = chi2.sf(LR, diff_df)  # test de la significativité
     return p
 
 
 def vers_excel(tables, file):
     """
     Écriture d'un ensemble de tableaux.
-    Dans un fichier excel avec titres.
+    Dans un fichier libre office (xlsc) avec titres.
 
     Parameters
     ----------
     tables : list or dict or DataFrame
         Données à écrire dans un fichier
     file: str
-        chemin et nom du fichier de sortie
+        chemin et nom du fichier de sortie (.xlsx)
 
     Returns
     -------
     None
     """
 
     # Transformation de l'entrée en dictionnaire
@@ -749,24 +771,24 @@
         return None
 
     # Ouverture d'un fichier excel
     if (not ".xlsx" in file) or (not ".xls" in file):
         print("Le fichier a créer n'a pas la bonne extension")
         return None
 
-    writer = pd.ExcelWriter(file)
-    workbook = writer.book
-    worksheet = workbook.add_worksheet("Résultats")
+    writer = pd.ExcelWriter(file, engine='openpyxl', mode='w')
+    writer.book.create_sheet("Résultats")
+    worksheet = writer.book.worksheets[0]
     writer.sheets["Résultats"] = worksheet
     curseur = 0  # ligne d'écriture
     # Boucle sur les tableaux
     for title in tables:
-        worksheet.write_string(curseur, 0, title)  # écriture du titre
+        worksheet.cell(curseur + 1,1,title)
         tables[title].to_excel(writer, sheet_name="Résultats", startrow=curseur + 2)
-        curseur += 2 + tables[title].shape[0] + 3
+        curseur += 2 + tables[title].shape[0] + 4
     writer.save()
 
     return None
 
 
 def moyenne_ponderee(colonne, poids):
     """
@@ -811,15 +833,15 @@
 def _escape_quotes(variable: str) -> str:
     """ 
     Complète la fonction Q() de patsy pour échapper les caractères problématiques
     Parameters
     ----------
     variable : str
         nom de variable
-        
+
     Returns
     -------
     str
         nom de variable modifiée
 
     """
     return variable.replace('"', '\\"')
@@ -848,17 +870,17 @@
 
     Returns
     -------
     DataFrame
         Tableau des associations entre variables quanti
     DataFrame
         Tableau des associations entre variables quali
-    DataFrame (optionnal)
+    DataFrame (if mod = True)
         Tableau des associations entre modalités qualitatives.
-    DataFrame (optionnal)
+    DataFrame (if mod = True)
         Tableau des associations entre modalités quantitatives.
 
     Notes
     -----
     Participation de Ahmadou Dicko pour passage R vers Python.
     Code initial en R dans FactoMineR.
     Passage en Python initié avec Inno3.
```

### Comparing `pyshs-0.3.3/test/test_pyshs.py` & `pyshs-0.3.4/test/test_pyshs.py`

 * *Files identical despite different names*

### Comparing `pyshs-0.3.3/PKG-INFO` & `pyshs-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshs
-Version: 0.3.3
+Version: 0.3.4
 Summary: PySHS - Faciliter le traitement de données de questionnaires en SHS
 Home-page: https://github.com/emilienschultz/pyshs-bib
 Author: Emilien Schultz
 Author-email: emilien.schultz@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```

