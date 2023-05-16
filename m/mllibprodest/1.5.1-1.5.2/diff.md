# Comparing `tmp/mllibprodest-1.5.1.tar.gz` & `tmp/mllibprodest-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mllibprodest-1.5.1.tar", last modified: Sun Oct  9 15:18:11 2022, max compression
+gzip compressed data, was "mllibprodest-1.5.2.tar", last modified: Tue May 16 17:18:47 2023, max compression
```

## Comparing `mllibprodest-1.5.1.tar` & `mllibprodest-1.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2022-10-09 15:18:11.282676 mllibprodest-1.5.1/
--rw-rw-r--   0 messias   (1000) messias   (1000)    35150 2022-10-09 15:16:27.000000 mllibprodest-1.5.1/LICENSE
--rw-rw-r--   0 messias   (1000) messias   (1000)    25067 2022-10-09 15:18:11.282676 mllibprodest-1.5.1/PKG-INFO
--rw-rw-r--   0 messias   (1000) messias   (1000)    24073 2022-10-09 15:16:27.000000 mllibprodest-1.5.1/README.md
--rw-rw-r--   0 messias   (1000) messias   (1000)     1023 2022-10-09 15:16:27.000000 mllibprodest-1.5.1/pyproject.toml
--rw-rw-r--   0 messias   (1000) messias   (1000)      190 2022-10-09 15:18:11.282676 mllibprodest-1.5.1/setup.cfg
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2022-10-09 15:18:11.278676 mllibprodest-1.5.1/src/
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2022-10-09 15:18:11.282676 mllibprodest-1.5.1/src/mllibprodest/
--rw-rw-r--   0 messias   (1000) messias   (1000)        0 2022-10-09 15:16:27.000000 mllibprodest-1.5.1/src/mllibprodest/__init__.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     9117 2022-10-09 15:16:27.000000 mllibprodest-1.5.1/src/mllibprodest/interfaces.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     5308 2022-10-09 15:16:27.000000 mllibprodest-1.5.1/src/mllibprodest/provider.py
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2022-10-09 15:18:11.282676 mllibprodest-1.5.1/src/mllibprodest/providers_types/
--rw-rw-r--   0 messias   (1000) messias   (1000)        0 2022-10-09 15:16:27.000000 mllibprodest-1.5.1/src/mllibprodest/providers_types/__init__.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     2037 2022-10-09 15:16:27.000000 mllibprodest-1.5.1/src/mllibprodest/providers_types/local_provider.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     2303 2022-10-09 15:16:27.000000 mllibprodest-1.5.1/src/mllibprodest/providers_types/minio_provider.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     7927 2022-10-09 15:16:27.000000 mllibprodest-1.5.1/src/mllibprodest/providers_types/mlflow_provider.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     8476 2022-10-09 15:16:27.000000 mllibprodest-1.5.1/src/mllibprodest/shared_classes.py
--rw-rw-r--   0 messias   (1000) messias   (1000)     6772 2022-10-09 15:16:27.000000 mllibprodest-1.5.1/src/mllibprodest/utils.py
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2022-10-09 15:18:11.282676 mllibprodest-1.5.1/src/mllibprodest/validators/
--rw-rw-r--   0 messias   (1000) messias   (1000)        0 2022-10-09 15:16:27.000000 mllibprodest-1.5.1/src/mllibprodest/validators/__init__.py
--rw-rw-r--   0 messias   (1000) messias   (1000)    21483 2022-10-09 15:16:27.000000 mllibprodest-1.5.1/src/mllibprodest/validators/test.py
-drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2022-10-09 15:18:11.282676 mllibprodest-1.5.1/src/mllibprodest.egg-info/
--rw-rw-r--   0 messias   (1000) messias   (1000)    25067 2022-10-09 15:18:11.000000 mllibprodest-1.5.1/src/mllibprodest.egg-info/PKG-INFO
--rw-rw-r--   0 messias   (1000) messias   (1000)      666 2022-10-09 15:18:11.000000 mllibprodest-1.5.1/src/mllibprodest.egg-info/SOURCES.txt
--rw-rw-r--   0 messias   (1000) messias   (1000)        1 2022-10-09 15:18:11.000000 mllibprodest-1.5.1/src/mllibprodest.egg-info/dependency_links.txt
--rw-rw-r--   0 messias   (1000) messias   (1000)       66 2022-10-09 15:18:11.000000 mllibprodest-1.5.1/src/mllibprodest.egg-info/requires.txt
--rw-rw-r--   0 messias   (1000) messias   (1000)       13 2022-10-09 15:18:11.000000 mllibprodest-1.5.1/src/mllibprodest.egg-info/top_level.txt
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/
+-rw-rw-r--   0 messias   (1000) messias   (1000)    35150 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/LICENSE
+-rw-rw-r--   0 messias   (1000) messias   (1000)    25103 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/PKG-INFO
+-rw-rw-r--   0 messias   (1000) messias   (1000)    24109 2023-05-16 17:03:16.000000 mllibprodest-1.5.2/README.md
+-rw-rw-r--   0 messias   (1000) messias   (1000)     1024 2023-05-16 16:12:14.000000 mllibprodest-1.5.2/pyproject.toml
+-rw-rw-r--   0 messias   (1000) messias   (1000)      190 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/setup.cfg
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/src/
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/src/mllibprodest/
+-rw-rw-r--   0 messias   (1000) messias   (1000)        0 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/__init__.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     9117 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/interfaces.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     5308 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/provider.py
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/src/mllibprodest/providers_types/
+-rw-rw-r--   0 messias   (1000) messias   (1000)        0 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/providers_types/__init__.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     2037 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/providers_types/local_provider.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     2303 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/providers_types/minio_provider.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     7927 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/providers_types/mlflow_provider.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     8476 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/shared_classes.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)     6772 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/utils.py
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/src/mllibprodest/validators/
+-rw-rw-r--   0 messias   (1000) messias   (1000)        0 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/validators/__init__.py
+-rw-rw-r--   0 messias   (1000) messias   (1000)    21483 2023-05-15 18:22:04.000000 mllibprodest-1.5.2/src/mllibprodest/validators/test.py
+drwxrwxr-x   0 messias   (1000) messias   (1000)        0 2023-05-16 17:18:47.023238 mllibprodest-1.5.2/src/mllibprodest.egg-info/
+-rw-rw-r--   0 messias   (1000) messias   (1000)    25103 2023-05-16 17:18:47.000000 mllibprodest-1.5.2/src/mllibprodest.egg-info/PKG-INFO
+-rw-rw-r--   0 messias   (1000) messias   (1000)      666 2023-05-16 17:18:47.000000 mllibprodest-1.5.2/src/mllibprodest.egg-info/SOURCES.txt
+-rw-rw-r--   0 messias   (1000) messias   (1000)        1 2023-05-16 17:18:47.000000 mllibprodest-1.5.2/src/mllibprodest.egg-info/dependency_links.txt
+-rw-rw-r--   0 messias   (1000) messias   (1000)       65 2023-05-16 17:18:47.000000 mllibprodest-1.5.2/src/mllibprodest.egg-info/requires.txt
+-rw-rw-r--   0 messias   (1000) messias   (1000)       13 2023-05-16 17:18:47.000000 mllibprodest-1.5.2/src/mllibprodest.egg-info/top_level.txt
```

### Comparing `mllibprodest-1.5.1/LICENSE` & `mllibprodest-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.5.1/PKG-INFO` & `mllibprodest-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: mllibprodest
-Version: 1.5.1
+Version: 1.5.2
 Summary: Biblioteca de Machine Learning (ML) do Prodest.
 Home-page: https://github.com/prodest/mllibprodest
 Author: Instituto de Tecnologia da Informação e Comunicação do Espírito Santo (PRODEST)
 Author-email: "Instituto de Tecnologia da Informação e Comunicação do Espírito Santo (PRODEST)" <prodest@prodest.es.gov.br>
 License: GPLv3
 Project-URL: Homepage, https://github.com/prodest/mllibprodest
 Project-URL: Bug Tracker, https://github.com/prodest/mllibprodest/issues
 Project-URL: Documentation, https://prodest.github.io/mllibprodest
 Keywords: Prodest,ML,lib,stack
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: Portuguese (Brazilian)
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Biblioteca de ML (*Machine Learning*) - Prodest 
 A finalidade desta biblioteca é prover interfaces e funções que dão suporte ao provisionamento de modelos de ML na Stack 
 de ML do Prodest.
 
 Acesse a [documentação da lib](https://prodest.github.io/mllibprodest)!
 
 *Workflow* básico para construção, disponibilização e publicação de modelos:
 
 ![](https://github.com/prodest/mllibprodest/blob/main/docs/workflow.png?raw=true)
 
 ## Pré-requisitos
-* **Python >= 3.8.** Instruções: [Linux (Geralmente já vem instalado por padrão)](https://python.org.br/instalacao-linux) ou [Windows](https://www.python.org/downloads/windows).
+* **Python >= 3.9.** Instruções: [Linux (Geralmente já vem instalado por padrão)](https://python.org.br/instalacao-linux) ou [Windows](https://www.python.org/downloads/windows).
 * **Git.** Instruções: [Linux](https://git-scm.com/download/linux) ou [Windows](https://git-scm.com/download/win).
 * **Venv.** Gerenciador de ambiente virtual Python adotado no tutorial. Instruções: [Linux e Windows (escolha o sistema na página)](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment). 
 Ou qualquer outro gerenciador de ambiente Python que preferir.
 
 ## 1. Realize experimentos e escolha o modelo 
 
 Esta é uma das etapas iniciais de um projeto para o desenvolvimento de um modelo de *Machine Learning*. Neste momento é 
@@ -128,15 +128,15 @@
 - Crie uma pasta para testes;
 - Copie e cole o código acima em um editor de texto simples e salve com o nome 'testeml.py' dentro da pasta criada;
 - Abra um prompt de comando ou terminal e entre na pasta criada;
 - Crie e ative um ambiente virtual Python, conforme instruções: [Linux e Windows (escolha o sistema na página)](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment);
 - Instale os pacotes mlflow, sklearn, matplotlib e numpy;
 
 ```bash
-pip install mlflow sklearn matplotlib numpy
+pip install mlflow==2.3.2 scikit-learn==1.2.2 matplotlib==3.7.1 numpy==1.24.3
 ```
 - Rode o teste (ignore as mensagens do tipo 'INFO' de criação do banco de dados);
 ```bash
 python testeml.py
 ```
 Cabe observar que: depois de rodar o código de teste, foi criada uma pasta chamada '**mlruns**', dentro da pasta de 
 testes, que serve para armazenar os artefatos gerados pelo código e que são apresentados na interface do MLflow. 
@@ -164,15 +164,15 @@
 ```
 
 - Verifique se o experimento foi registrado. Acesse o MLFlow: [http://localhost:5000](http://localhost:5000) e procure 
 pelo experimento/execução '**Teste sklearn**' na seção **Experiments** (se o experimento não estiver listado, verifique 
 se o servidor foi iniciado de dentro da pasta correta);
 
 
-- Clique na execução do experimento que se encontra na coluna '**Created**' (destaque em verde);
+- Clique na execução do experimento que se encontra na coluna '**Run Name**' (destaque em verde);
 
 ![](https://github.com/prodest/mllibprodest/blob/main/docs/experiments-mlflow.png?raw=true)
 - Verifique se os artefatos foram gravados;
 
 ![](https://github.com/prodest/mllibprodest/blob/main/docs/artifacts-mlflow.png?raw=true)
 
 - Finalize o servidor do MLflow. Faça 'CTRL+c' no prompt de comando ou terminal onde ele foi iniciado;
@@ -199,15 +199,15 @@
 - Ative o ambiente virtual Python. Instruções: [Linux e Windows (escolha o sistema na página)](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment); 
 - Inicie o servidor do MLflow;
 ```bash
 mlflow server --backend-store-uri sqlite:///teste_mlflow.db --host 0.0.0.0 -p 5000 --default-artifact-root mlruns
 ```
 - Acesse o MLflow ([http://localhost:5000](http://localhost:5000)) e clique no experimento que foi criado por você (se 
 o experimento não estiver listado, verifique se o servidor do MLflow foi iniciado de dentro da pasta correta);
-- Clique no link (que está na coluna **'Created'**) para a rodada do experimento que deseja registrar;
+- Clique no link (que está na coluna **'Run Name'**) para a rodada do experimento que deseja registrar;
 - Clique no botão **'Register Model'** e escolha a opção **'Create New Model'**;
 - Dê um nome para o modelo e clique em **'Register'**;
 - Na barra superior clique em **'Models'**;
 - Clique no link para a última versão do modelo que está em **'Latest Version'**;
 - Na opção **'Stage'** troque de **'None'** para **'Production'** e clique em OK.
 
 Quando for testar a implementação dos *workers* (passo 3), lembre de deixar o servidor do MLflow rodando para que seja
```

### Comparing `mllibprodest-1.5.1/README.md` & `mllibprodest-1.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Acesse a [documentação da lib](https://prodest.github.io/mllibprodest)!
 
 *Workflow* básico para construção, disponibilização e publicação de modelos:
 
 ![](https://github.com/prodest/mllibprodest/blob/main/docs/workflow.png?raw=true)
 
 ## Pré-requisitos
-* **Python >= 3.8.** Instruções: [Linux (Geralmente já vem instalado por padrão)](https://python.org.br/instalacao-linux) ou [Windows](https://www.python.org/downloads/windows).
+* **Python >= 3.9.** Instruções: [Linux (Geralmente já vem instalado por padrão)](https://python.org.br/instalacao-linux) ou [Windows](https://www.python.org/downloads/windows).
 * **Git.** Instruções: [Linux](https://git-scm.com/download/linux) ou [Windows](https://git-scm.com/download/win).
 * **Venv.** Gerenciador de ambiente virtual Python adotado no tutorial. Instruções: [Linux e Windows (escolha o sistema na página)](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment). 
 Ou qualquer outro gerenciador de ambiente Python que preferir.
 
 ## 1. Realize experimentos e escolha o modelo 
 
 Esta é uma das etapas iniciais de um projeto para o desenvolvimento de um modelo de *Machine Learning*. Neste momento é 
@@ -107,15 +107,15 @@
 - Crie uma pasta para testes;
 - Copie e cole o código acima em um editor de texto simples e salve com o nome 'testeml.py' dentro da pasta criada;
 - Abra um prompt de comando ou terminal e entre na pasta criada;
 - Crie e ative um ambiente virtual Python, conforme instruções: [Linux e Windows (escolha o sistema na página)](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment);
 - Instale os pacotes mlflow, sklearn, matplotlib e numpy;
 
 ```bash
-pip install mlflow sklearn matplotlib numpy
+pip install mlflow==2.3.2 scikit-learn==1.2.2 matplotlib==3.7.1 numpy==1.24.3
 ```
 - Rode o teste (ignore as mensagens do tipo 'INFO' de criação do banco de dados);
 ```bash
 python testeml.py
 ```
 Cabe observar que: depois de rodar o código de teste, foi criada uma pasta chamada '**mlruns**', dentro da pasta de 
 testes, que serve para armazenar os artefatos gerados pelo código e que são apresentados na interface do MLflow. 
@@ -143,15 +143,15 @@
 ```
 
 - Verifique se o experimento foi registrado. Acesse o MLFlow: [http://localhost:5000](http://localhost:5000) e procure 
 pelo experimento/execução '**Teste sklearn**' na seção **Experiments** (se o experimento não estiver listado, verifique 
 se o servidor foi iniciado de dentro da pasta correta);
 
 
-- Clique na execução do experimento que se encontra na coluna '**Created**' (destaque em verde);
+- Clique na execução do experimento que se encontra na coluna '**Run Name**' (destaque em verde);
 
 ![](https://github.com/prodest/mllibprodest/blob/main/docs/experiments-mlflow.png?raw=true)
 - Verifique se os artefatos foram gravados;
 
 ![](https://github.com/prodest/mllibprodest/blob/main/docs/artifacts-mlflow.png?raw=true)
 
 - Finalize o servidor do MLflow. Faça 'CTRL+c' no prompt de comando ou terminal onde ele foi iniciado;
@@ -178,15 +178,15 @@
 - Ative o ambiente virtual Python. Instruções: [Linux e Windows (escolha o sistema na página)](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment); 
 - Inicie o servidor do MLflow;
 ```bash
 mlflow server --backend-store-uri sqlite:///teste_mlflow.db --host 0.0.0.0 -p 5000 --default-artifact-root mlruns
 ```
 - Acesse o MLflow ([http://localhost:5000](http://localhost:5000)) e clique no experimento que foi criado por você (se 
 o experimento não estiver listado, verifique se o servidor do MLflow foi iniciado de dentro da pasta correta);
-- Clique no link (que está na coluna **'Created'**) para a rodada do experimento que deseja registrar;
+- Clique no link (que está na coluna **'Run Name'**) para a rodada do experimento que deseja registrar;
 - Clique no botão **'Register Model'** e escolha a opção **'Create New Model'**;
 - Dê um nome para o modelo e clique em **'Register'**;
 - Na barra superior clique em **'Models'**;
 - Clique no link para a última versão do modelo que está em **'Latest Version'**;
 - Na opção **'Stage'** troque de **'None'** para **'Production'** e clique em OK.
 
 Quando for testar a implementação dos *workers* (passo 3), lembre de deixar o servidor do MLflow rodando para que seja
```

### Comparing `mllibprodest-1.5.1/pyproject.toml` & `mllibprodest-1.5.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
-requires = ['setuptools>=61.0']
+requires = ['setuptools>=66.0.0']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mllibprodest"
-version = "1.5.1"
+version = "1.5.2"
 license = {text = "GPLv3"}
 authors = [
   { name="Instituto de Tecnologia da Informação e Comunicação do Espírito Santo (PRODEST)", email="prodest@prodest.es.gov.br" },
 ]
 description = "Biblioteca de Machine Learning (ML) do Prodest."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
-    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: Portuguese (Brazilian)"
 ]
-dependencies = ['minio==7.1.12', 'python-dotenv==0.21.0', 'mlflow==1.29.0', 'boto3==1.24.89']
+dependencies = ['minio==7.1.14', 'python-dotenv==1.0.0', 'mlflow==2.3.2', 'boto3==1.26.134']
 keywords = ['Prodest', 'ML', 'lib', 'stack']
 
 [project.urls]
 "Homepage" = "https://github.com/prodest/mllibprodest"
 "Bug Tracker" = "https://github.com/prodest/mllibprodest/issues"
 "Documentation" = "https://prodest.github.io/mllibprodest"
```

### Comparing `mllibprodest-1.5.1/src/mllibprodest/interfaces.py` & `mllibprodest-1.5.2/src/mllibprodest/interfaces.py`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.5.1/src/mllibprodest/provider.py` & `mllibprodest-1.5.2/src/mllibprodest/provider.py`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.5.1/src/mllibprodest/providers_types/local_provider.py` & `mllibprodest-1.5.2/src/mllibprodest/providers_types/local_provider.py`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.5.1/src/mllibprodest/providers_types/minio_provider.py` & `mllibprodest-1.5.2/src/mllibprodest/providers_types/minio_provider.py`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.5.1/src/mllibprodest/providers_types/mlflow_provider.py` & `mllibprodest-1.5.2/src/mllibprodest/providers_types/mlflow_provider.py`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.5.1/src/mllibprodest/shared_classes.py` & `mllibprodest-1.5.2/src/mllibprodest/shared_classes.py`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.5.1/src/mllibprodest/utils.py` & `mllibprodest-1.5.2/src/mllibprodest/utils.py`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.5.1/src/mllibprodest/validators/test.py` & `mllibprodest-1.5.2/src/mllibprodest/validators/test.py`

 * *Files identical despite different names*

### Comparing `mllibprodest-1.5.1/src/mllibprodest.egg-info/PKG-INFO` & `mllibprodest-1.5.2/src/mllibprodest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: mllibprodest
-Version: 1.5.1
+Version: 1.5.2
 Summary: Biblioteca de Machine Learning (ML) do Prodest.
 Home-page: https://github.com/prodest/mllibprodest
 Author: Instituto de Tecnologia da Informação e Comunicação do Espírito Santo (PRODEST)
 Author-email: "Instituto de Tecnologia da Informação e Comunicação do Espírito Santo (PRODEST)" <prodest@prodest.es.gov.br>
 License: GPLv3
 Project-URL: Homepage, https://github.com/prodest/mllibprodest
 Project-URL: Bug Tracker, https://github.com/prodest/mllibprodest/issues
 Project-URL: Documentation, https://prodest.github.io/mllibprodest
 Keywords: Prodest,ML,lib,stack
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: Portuguese (Brazilian)
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Biblioteca de ML (*Machine Learning*) - Prodest 
 A finalidade desta biblioteca é prover interfaces e funções que dão suporte ao provisionamento de modelos de ML na Stack 
 de ML do Prodest.
 
 Acesse a [documentação da lib](https://prodest.github.io/mllibprodest)!
 
 *Workflow* básico para construção, disponibilização e publicação de modelos:
 
 ![](https://github.com/prodest/mllibprodest/blob/main/docs/workflow.png?raw=true)
 
 ## Pré-requisitos
-* **Python >= 3.8.** Instruções: [Linux (Geralmente já vem instalado por padrão)](https://python.org.br/instalacao-linux) ou [Windows](https://www.python.org/downloads/windows).
+* **Python >= 3.9.** Instruções: [Linux (Geralmente já vem instalado por padrão)](https://python.org.br/instalacao-linux) ou [Windows](https://www.python.org/downloads/windows).
 * **Git.** Instruções: [Linux](https://git-scm.com/download/linux) ou [Windows](https://git-scm.com/download/win).
 * **Venv.** Gerenciador de ambiente virtual Python adotado no tutorial. Instruções: [Linux e Windows (escolha o sistema na página)](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment). 
 Ou qualquer outro gerenciador de ambiente Python que preferir.
 
 ## 1. Realize experimentos e escolha o modelo 
 
 Esta é uma das etapas iniciais de um projeto para o desenvolvimento de um modelo de *Machine Learning*. Neste momento é 
@@ -128,15 +128,15 @@
 - Crie uma pasta para testes;
 - Copie e cole o código acima em um editor de texto simples e salve com o nome 'testeml.py' dentro da pasta criada;
 - Abra um prompt de comando ou terminal e entre na pasta criada;
 - Crie e ative um ambiente virtual Python, conforme instruções: [Linux e Windows (escolha o sistema na página)](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment);
 - Instale os pacotes mlflow, sklearn, matplotlib e numpy;
 
 ```bash
-pip install mlflow sklearn matplotlib numpy
+pip install mlflow==2.3.2 scikit-learn==1.2.2 matplotlib==3.7.1 numpy==1.24.3
 ```
 - Rode o teste (ignore as mensagens do tipo 'INFO' de criação do banco de dados);
 ```bash
 python testeml.py
 ```
 Cabe observar que: depois de rodar o código de teste, foi criada uma pasta chamada '**mlruns**', dentro da pasta de 
 testes, que serve para armazenar os artefatos gerados pelo código e que são apresentados na interface do MLflow. 
@@ -164,15 +164,15 @@
 ```
 
 - Verifique se o experimento foi registrado. Acesse o MLFlow: [http://localhost:5000](http://localhost:5000) e procure 
 pelo experimento/execução '**Teste sklearn**' na seção **Experiments** (se o experimento não estiver listado, verifique 
 se o servidor foi iniciado de dentro da pasta correta);
 
 
-- Clique na execução do experimento que se encontra na coluna '**Created**' (destaque em verde);
+- Clique na execução do experimento que se encontra na coluna '**Run Name**' (destaque em verde);
 
 ![](https://github.com/prodest/mllibprodest/blob/main/docs/experiments-mlflow.png?raw=true)
 - Verifique se os artefatos foram gravados;
 
 ![](https://github.com/prodest/mllibprodest/blob/main/docs/artifacts-mlflow.png?raw=true)
 
 - Finalize o servidor do MLflow. Faça 'CTRL+c' no prompt de comando ou terminal onde ele foi iniciado;
@@ -199,15 +199,15 @@
 - Ative o ambiente virtual Python. Instruções: [Linux e Windows (escolha o sistema na página)](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment); 
 - Inicie o servidor do MLflow;
 ```bash
 mlflow server --backend-store-uri sqlite:///teste_mlflow.db --host 0.0.0.0 -p 5000 --default-artifact-root mlruns
 ```
 - Acesse o MLflow ([http://localhost:5000](http://localhost:5000)) e clique no experimento que foi criado por você (se 
 o experimento não estiver listado, verifique se o servidor do MLflow foi iniciado de dentro da pasta correta);
-- Clique no link (que está na coluna **'Created'**) para a rodada do experimento que deseja registrar;
+- Clique no link (que está na coluna **'Run Name'**) para a rodada do experimento que deseja registrar;
 - Clique no botão **'Register Model'** e escolha a opção **'Create New Model'**;
 - Dê um nome para o modelo e clique em **'Register'**;
 - Na barra superior clique em **'Models'**;
 - Clique no link para a última versão do modelo que está em **'Latest Version'**;
 - Na opção **'Stage'** troque de **'None'** para **'Production'** e clique em OK.
 
 Quando for testar a implementação dos *workers* (passo 3), lembre de deixar o servidor do MLflow rodando para que seja
```

### Comparing `mllibprodest-1.5.1/src/mllibprodest.egg-info/SOURCES.txt` & `mllibprodest-1.5.2/src/mllibprodest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

