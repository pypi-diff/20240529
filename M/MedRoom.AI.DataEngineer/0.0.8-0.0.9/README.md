# Comparing `tmp/medroom_ai_dataengineer-0.0.8.tar.gz` & `tmp/medroom_ai_dataengineer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medroom_ai_dataengineer-0.0.8.tar", last modified: Mon May 27 18:09:02 2024, max compression
+gzip compressed data, was "medroom_ai_dataengineer-0.0.9.tar", last modified: Mon May 27 19:23:31 2024, max compression
```

## Comparing `medroom_ai_dataengineer-0.0.8.tar` & `medroom_ai_dataengineer-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 18:09:02.237816 medroom_ai_dataengineer-0.0.8/
--rw-rw-rw-   0        0        0    11558 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.8/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-27 18:09:02.235760 medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/
--rw-rw-rw-   0        0        0    13823 2024-05-27 18:09:02.000000 medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2024-05-27 18:09:02.000000 medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      115 2024-05-27 18:09:02.000000 medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-12 17:49:13.000000 medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      151 2024-05-27 18:09:02.000000 medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-27 18:09:02.000000 medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13823 2024-05-27 18:09:02.236772 medroom_ai_dataengineer-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     8575 2024-05-27 17:56:40.000000 medroom_ai_dataengineer-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 18:09:02.191875 medroom_ai_dataengineer-0.0.8/medroom/
-drwxrwxrwx   0        0        0        0 2024-05-27 18:09:02.191875 medroom_ai_dataengineer-0.0.8/medroom/dna/
-drwxrwxrwx   0        0        0        0 2024-05-27 18:09:02.231059 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/
--rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/__init__.py
--rw-rw-rw-   0        0        0      663 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/config.py
--rw-rw-rw-   0        0        0      606 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/main.py
-drwxrwxrwx   0        0        0        0 2024-05-27 18:09:02.235013 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/
--rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/__init__.py
--rw-rw-rw-   0        0        0     4658 2024-05-27 18:07:11.000000 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/evalmetrics.py
--rw-rw-rw-   0        0        0     4949 2024-04-20 21:31:01.000000 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/mlflow_helper.py
--rw-rw-rw-   0        0        0     2908 2024-04-12 22:02:34.000000 medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/textclean.py
--rw-rw-rw-   0        0        0       42 2024-05-27 18:09:02.237939 medroom_ai_dataengineer-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1448 2024-05-27 17:56:40.000000 medroom_ai_dataengineer-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 19:23:31.052697 medroom_ai_dataengineer-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.9/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-27 19:23:31.050519 medroom_ai_dataengineer-0.0.9/MedRoom.AI.DataEngineer.egg-info/
+-rw-rw-rw-   0        0        0    13860 2024-05-27 19:23:30.000000 medroom_ai_dataengineer-0.0.9/MedRoom.AI.DataEngineer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2024-05-27 19:23:30.000000 medroom_ai_dataengineer-0.0.9/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      115 2024-05-27 19:23:30.000000 medroom_ai_dataengineer-0.0.9/MedRoom.AI.DataEngineer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 17:49:13.000000 medroom_ai_dataengineer-0.0.9/MedRoom.AI.DataEngineer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      172 2024-05-27 19:23:30.000000 medroom_ai_dataengineer-0.0.9/MedRoom.AI.DataEngineer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-27 19:23:30.000000 medroom_ai_dataengineer-0.0.9/MedRoom.AI.DataEngineer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13860 2024-05-27 19:23:31.052697 medroom_ai_dataengineer-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8575 2024-05-27 17:56:40.000000 medroom_ai_dataengineer-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 19:23:30.950602 medroom_ai_dataengineer-0.0.9/medroom/
+drwxrwxrwx   0        0        0        0 2024-05-27 19:23:30.950602 medroom_ai_dataengineer-0.0.9/medroom/dna/
+drwxrwxrwx   0        0        0        0 2024-05-27 19:23:31.027936 medroom_ai_dataengineer-0.0.9/medroom/dna/processors/
+-rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.9/medroom/dna/processors/__init__.py
+-rw-rw-rw-   0        0        0      663 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.9/medroom/dna/processors/config.py
+-rw-rw-rw-   0        0        0      606 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.9/medroom/dna/processors/main.py
+drwxrwxrwx   0        0        0        0 2024-05-27 19:23:31.050519 medroom_ai_dataengineer-0.0.9/medroom/dna/processors/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.9/medroom/dna/processors/utils/__init__.py
+-rw-rw-rw-   0        0        0     4658 2024-05-27 18:07:11.000000 medroom_ai_dataengineer-0.0.9/medroom/dna/processors/utils/evalmetrics.py
+-rw-rw-rw-   0        0        0     6051 2024-05-27 19:09:17.000000 medroom_ai_dataengineer-0.0.9/medroom/dna/processors/utils/mlflow_helper.py
+-rw-rw-rw-   0        0        0     2908 2024-04-12 22:02:34.000000 medroom_ai_dataengineer-0.0.9/medroom/dna/processors/utils/textclean.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 19:23:31.052697 medroom_ai_dataengineer-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1448 2024-05-27 17:56:40.000000 medroom_ai_dataengineer-0.0.9/setup.py
```

### Comparing `medroom_ai_dataengineer-0.0.8/LICENSE` & `medroom_ai_dataengineer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/PKG-INFO` & `medroom_ai_dataengineer-0.0.9/MedRoom.AI.DataEngineer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedRoom.AI.DataEngineer
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Natural Language Processing Data Engineer
 Home-page: https://github.com/MedRoomGitHub/MedRoom.AI.DataEngineer
 Author: Team IA
 Author-email: medroom@medroom.com.br
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -212,10 +212,11 @@
 Requires-Dist: nltk==3.8.1
 Requires-Dist: spacy==3.7.1
 Requires-Dist: unidecode==1.3.7
 Requires-Dist: pandas==2.1.1
 Requires-Dist: numpy==1.26.0
 Requires-Dist: scikit-learn==1.3.1
 Requires-Dist: mlflow==2.12.2
+Requires-Dist: transformers==4.41.0
 Provides-Extra: plotting
 Requires-Dist: matplotlib==3.7.0; extra == "plotting"
 Requires-Dist: seaborn==0.13.0; extra == "plotting"
```

### Comparing `medroom_ai_dataengineer-0.0.8/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt` & `medroom_ai_dataengineer-0.0.9/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.8/PKG-INFO` & `medroom_ai_dataengineer-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedRoom.AI.DataEngineer
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Natural Language Processing Data Engineer
 Home-page: https://github.com/MedRoomGitHub/MedRoom.AI.DataEngineer
 Author: Team IA
 Author-email: medroom@medroom.com.br
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -212,10 +212,11 @@
 Requires-Dist: nltk==3.8.1
 Requires-Dist: spacy==3.7.1
 Requires-Dist: unidecode==1.3.7
 Requires-Dist: pandas==2.1.1
 Requires-Dist: numpy==1.26.0
 Requires-Dist: scikit-learn==1.3.1
 Requires-Dist: mlflow==2.12.2
+Requires-Dist: transformers==4.41.0
 Provides-Extra: plotting
 Requires-Dist: matplotlib==3.7.0; extra == "plotting"
 Requires-Dist: seaborn==0.13.0; extra == "plotting"
```

### Comparing `medroom_ai_dataengineer-0.0.8/README.md` & `medroom_ai_dataengineer-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.8/medroom/dna/processors/config.py` & `medroom_ai_dataengineer-0.0.9/medroom/dna/processors/config.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.8/medroom/dna/processors/main.py` & `medroom_ai_dataengineer-0.0.9/medroom/dna/processors/main.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/evalmetrics.py` & `medroom_ai_dataengineer-0.0.9/medroom/dna/processors/utils/evalmetrics.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/mlflow_helper.py` & `medroom_ai_dataengineer-0.0.9/medroom/dna/processors/utils/mlflow_helper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,52 @@
 # Importando Libs
 import json
 import pickle
 import tempfile
+import os
+import shutil
+from typing import Optional
 
 import mlflow
 from mlflow.entities import Experiment
+from mlflow.pyfunc import PythonModel
 from PIL import Image
+from transformers import pipeline
 
-
+class TransformersWrapper(PythonModel):
+    def __init__(self, model_path):
+        self.model_path = model_path
+        self.model = None
+        self.load_model()
+        
+    def load_model(self):
+        self.model = pipeline("sentiment-analysis", model=self.model_path)
+        
+    def predict(self, model_input):
+        return self.model(model_input)
+
+def delete_folder_or_file(path: str) -> Optional[str]:
+    if not os.path.exists(path):
+        return f"O caminho '{path}' não existe."
+    try:
+        if os.path.isfile(path) or os.path.islink(path):
+            os.unlink(path)  # Remove arquivos ou links
+        elif os.path.isdir(path):
+            shutil.rmtree(path)  # Remove diretórios e seus conteúdos
+    except Exception as e:
+        return f"Falha ao deletar {path}. Razão: {e}"
+    return None
 class MLFlowHelper:
     def __init__(self, server_url, experiment_name):
         mlflow.set_tracking_uri(f"{server_url}")  # Define o URI de rastreamento do MLflow
         self.experiment = self.create_or_get_experiment(experiment_name)  # Cria ou recupera um experimento
         self.artifact_handlers = {
             "img": self._process_image_artifact,  # Handler para imagens
             "df_example": self._process_dataframe_artifact,  # Handler para exemplos de DataFrame
-            "model": self._process_model_artifact,  # Handler para modelos
+            "model_pipeline": self._process_model_pipeline_artifact,  # Handler para pipelines de modelos
         }
 
     def load_data_pickle(self, nome_arquivo):
         with open(nome_arquivo, "rb") as arquivo:
             return pickle.load(arquivo)  # Carrega dados de um arquivo pickle
 
     def create_or_get_experiment(self, experiment_name: str) -> Experiment:
@@ -93,12 +120,15 @@
     def _process_dataframe_artifact(self, key, value):
         with tempfile.NamedTemporaryFile(mode="w", delete=False, suffix=".json") as tmp:
             json.dump(value, tmp)
             tmp.flush()
             mlflow.log_artifact(tmp.name, f"data/{key}")  # Registra o DataFrame no MLflow
             print(f"DataFrame '{key}' processado e logado com sucesso.")
 
-    def _process_model_artifact(self, key, value):
-        with tempfile.TemporaryDirectory() as tmpdirname:
-            value.save_pretrained(tmpdirname)
-            mlflow.pytorch.log_model(pytorch_model=value, artifact_path="model")  # Registra o modelo no MLflow
-            print(f"Modelo '{key}' processado e logado com sucesso.")
+    def _process_model_pipeline_artifact(self, key, value):
+        model_temp_path = "temp_model"
+        value.save_pretrained(model_temp_path)
+        mlflow.pyfunc.log_model(
+            artifact_path="model_pipeline",
+            python_model=TransformersWrapper(model_temp_path),)  # Registra o modelo no MLflow
+        print(f"Modelo '{key}' processado e logado com sucesso.")
+        delete_folder_or_file(model_temp_path)
```

### Comparing `medroom_ai_dataengineer-0.0.8/medroom/dna/processors/utils/textclean.py` & `medroom_ai_dataengineer-0.0.9/medroom/dna/processors/utils/textclean.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.8/setup.py` & `medroom_ai_dataengineer-0.0.9/setup.py`

 * *Files identical despite different names*

