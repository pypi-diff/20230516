# Comparing `tmp/pyshs-0.3.2.tar.gz` & `tmp/pyshs-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyshs-0.3.2.tar", last modified: Thu Jul 21 15:45:38 2022, max compression
+gzip compressed data, was "pyshs-0.3.3.tar", last modified: Tue Jul 26 08:35:53 2022, max compression
```

## Comparing `pyshs-0.3.2.tar` & `pyshs-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1207 2022-07-10 16:38:42.992671 pyshs-0.3.2/.github/workflows/test.yml
--rw-r--r--   0        0        0       33 2021-04-19 18:31:27.000000 pyshs-0.3.2/.gitignore
--rw-r--r--   0        0        0     1082 2021-07-28 16:57:50.603926 pyshs-0.3.2/LICENSE
--rw-r--r--   0        0        0     1740 2022-07-21 15:44:33.000000 pyshs-0.3.2/README.md
--rw-r--r--   0        0        0  3875214 2022-07-20 21:09:28.437466 pyshs-0.3.2/docs/Exemple PySHS.ipynb
--rwxr-xr-x   0        0        0   329030 2017-12-14 09:37:50.000000 pyshs-0.3.2/docs/bdd2011.sav
--rw-r--r--   0        0        0     6436 2022-07-20 21:02:06.300396 pyshs-0.3.2/docs/resultats.xlsx
--rw-r--r--   0        0        0      453 2022-07-21 13:40:24.000000 pyshs-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1659 2022-07-21 15:44:41.000000 pyshs-0.3.2/pyshs/__init__.py
--rw-r--r--   0        0        0    32569 2022-07-21 15:42:42.000000 pyshs-0.3.2/pyshs/_core.py
--rw-r--r--   0        0        0     1602 2022-07-10 16:54:22.415582 pyshs-0.3.2/test/test_pyshs.py
--rw-r--r--   0        0        0     2215 1970-01-01 00:00:00.000000 pyshs-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1207 2022-07-10 16:38:42.992671 pyshs-0.3.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0       33 2021-04-19 18:31:27.000000 pyshs-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1082 2021-07-28 16:57:50.603926 pyshs-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1740 2022-07-26 08:33:20.000000 pyshs-0.3.3/README.md
+-rw-r--r--   0        0        0  3875214 2022-07-20 21:09:28.437466 pyshs-0.3.3/docs/Exemple PySHS.ipynb
+-rwxr-xr-x   0        0        0   329030 2017-12-14 09:37:50.000000 pyshs-0.3.3/docs/bdd2011.sav
+-rw-r--r--   0        0        0     6436 2022-07-20 21:02:06.300396 pyshs-0.3.3/docs/resultats.xlsx
+-rw-r--r--   0        0        0      453 2022-07-21 13:40:24.000000 pyshs-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1659 2022-07-26 08:33:10.000000 pyshs-0.3.3/pyshs/__init__.py
+-rw-r--r--   0        0        0    32435 2022-07-26 08:32:27.000000 pyshs-0.3.3/pyshs/_core.py
+-rw-r--r--   0        0        0     1602 2022-07-10 16:54:22.415582 pyshs-0.3.3/test/test_pyshs.py
+-rw-r--r--   0        0        0     2215 1970-01-01 00:00:00.000000 pyshs-0.3.3/PKG-INFO
```

### Comparing `pyshs-0.3.2/.github/workflows/test.yml` & `pyshs-0.3.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyshs-0.3.2/LICENSE` & `pyshs-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyshs-0.3.2/README.md` & `pyshs-0.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Bibliothèque PySHS
 
 La bibliothèque PySHS a pour but de faciliter l'analyse de données de questionnaire en sciences humaines et sociales pour les francophones avec Python. 
 
 Elle a pour but de s'enrichir progressivement pour permettre à Python de devenir une alternative (réaliste) à R avec des fonctions facilement utilisables sur les opérations habituelles.
 
-La version actuelle est la **0.3.2**
+La version actuelle est la **0.3.3**
 
 ## Contenu
 
 ### Traiter des données issues d'enquêtes par questionnaires (avec pondération)
 
 - Description d'un tableau de données
 - Tri à plat et tableau(x) croisé(s) avec pondération
```

### Comparing `pyshs-0.3.2/docs/Exemple PySHS.ipynb` & `pyshs-0.3.3/docs/Exemple PySHS.ipynb`

 * *Files identical despite different names*

### Comparing `pyshs-0.3.2/docs/bdd2011.sav` & `pyshs-0.3.3/docs/bdd2011.sav`

 * *Files identical despite different names*

### Comparing `pyshs-0.3.2/docs/resultats.xlsx` & `pyshs-0.3.3/docs/resultats.xlsx`

 * *Files identical despite different names*

### Comparing `pyshs-0.3.2/pyshs/__init__.py` & `pyshs-0.3.3/pyshs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,8 +42,8 @@
     likelihood_ratio,
     vers_excel,
     moyenne_ponderee,
     ecart_type_pondere,
     catdes
 )
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
```

### Comparing `pyshs-0.3.2/pyshs/_core.py` & `pyshs-0.3.3/pyshs/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import warnings
 import math
+from typing import Optional, List
+
 
 import numpy as np
 import pandas as pd
 from pandas.api.types import is_numeric_dtype
 
 from scipy.stats import chi2_contingency
 from scipy.stats.distributions import chi2
@@ -800,35 +802,32 @@
     float : écart-type pondéré
     """
     average = np.average(colonne, weights=poids)
     variance = np.average((colonne - average) ** 2, weights=poids)
     return math.sqrt(variance)
 
 
-import warnings
-import math
-
-import numpy as np
-import pandas as pd
-from pandas.api.types import is_numeric_dtype
 
-from scipy.stats import chi2_contingency
-from scipy.stats.distributions import chi2
-from scipy.stats import hypergeom
-from scipy.stats import norm
-
-import statsmodels.api as sm
-import statsmodels.formula.api as smf
 
-import plotly.graph_objects as go
+def _escape_quotes(variable: str) -> str:
+    """ 
+    Complète la fonction Q() de patsy pour échapper les caractères problématiques
+    Parameters
+    ----------
+    variable : str
+        nom de variable
+        
+    Returns
+    -------
+    str
+        nom de variable modifiée
 
+    """
+    return variable.replace('"', '\\"')
 
-import statsmodels.api as sm
-from statsmodels.formula.api import ols
-from typing import Optional, List
 
 def catdes(df: pd.DataFrame, vardep: str, varindep: List[str] = None,
            proba: float = 0.05, weight: Optional[str] = False, mod: bool = False):
     """
     Calcule la relation entre une variable catégorielle et plusieurs variables.
     Implémentation de la fonction catdes de FactoMineR.
     Attention : encore en version BETA
@@ -924,26 +923,21 @@
                             ).set_index(vardep).sort_values("p")
     
 
     # Cas des variables numériques
     
     tableau_num_var = []
     var_num_corr = []
-
+    
     # Pour chaque variable numérique
-    for v in cols_num:
-        
-        # Gestion des espaces dans les noms pour la formule
-        v_m = v.replace(" ","_").replace(":","")
-        vardep_m = vardep.replace(" ","_").replace(":","")
-        df[v_m] = df[v]
-        df[vardep_m] = df[vardep]
-        
-        # Calcul d'un ANOVA
-        model = ols(f"{v_m} ~ C({vardep_m})", data=df).fit()
+    for v in cols_num:        
+        # Calcul d'une ANOVA
+        # Utilisation de Q() pour échapper les variables
+        #  See https://patsy.readthedocs.io/en/latest/builtins-reference.html#patsy.builtins.Q
+        model = ols(f"Q(\"{_escape_quotes(v)}\") ~ C(Q(\"{_escape_quotes(vardep)}\"))", data=df).fit()
         aov_table = sm.stats.anova_lm(model, typ=2)
         
         # Paramètre de l'association
         eta2 = aov_table.iloc[0,0]/aov_table.iloc[:,0].sum()
         p = aov_table.iloc[0,3]
 
         # Ajout aux résultats si significatif
```

### Comparing `pyshs-0.3.2/test/test_pyshs.py` & `pyshs-0.3.3/test/test_pyshs.py`

 * *Files identical despite different names*

### Comparing `pyshs-0.3.2/PKG-INFO` & `pyshs-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshs
-Version: 0.3.2
+Version: 0.3.3
 Summary: PySHS - Faciliter le traitement de données de questionnaires en SHS
 Home-page: https://github.com/emilienschultz/pyshs-bib
 Author: Emilien Schultz
 Author-email: emilien.schultz@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 
 # Bibliothèque PySHS
 
 La bibliothèque PySHS a pour but de faciliter l'analyse de données de questionnaire en sciences humaines et sociales pour les francophones avec Python. 
 
 Elle a pour but de s'enrichir progressivement pour permettre à Python de devenir une alternative (réaliste) à R avec des fonctions facilement utilisables sur les opérations habituelles.
 
-La version actuelle est la **0.3.2**
+La version actuelle est la **0.3.3**
 
 ## Contenu
 
 ### Traiter des données issues d'enquêtes par questionnaires (avec pondération)
 
 - Description d'un tableau de données
 - Tri à plat et tableau(x) croisé(s) avec pondération
```

