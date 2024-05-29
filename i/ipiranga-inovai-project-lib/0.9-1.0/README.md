# Comparing `tmp/ipiranga-inovai-project-lib-0.9.tar.gz` & `tmp/ipiranga-inovai-project-lib-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipiranga-inovai-project-lib-0.9.tar", last modified: Wed May 29 19:10:34 2024, max compression
+gzip compressed data, was "ipiranga-inovai-project-lib-1.0.tar", last modified: Wed May 29 19:19:52 2024, max compression
```

## Comparing `ipiranga-inovai-project-lib-0.9.tar` & `ipiranga-inovai-project-lib-1.0.tar`

### file list

```diff
@@ -1,15 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 19:10:34.632332 ipiranga-inovai-project-lib-0.9/
--rw-rw-rw-   0        0        0      198 2024-04-05 19:57:15.000000 ipiranga-inovai-project-lib-0.9/LICENSE
--rw-rw-rw-   0        0        0      516 2024-05-29 19:10:34.629659 ipiranga-inovai-project-lib-0.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-05 19:18:28.000000 ipiranga-inovai-project-lib-0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 19:10:34.614928 ipiranga-inovai-project-lib-0.9/inovai/
--rw-rw-rw-   0        0        0        0 2024-04-05 20:33:51.000000 ipiranga-inovai-project-lib-0.9/inovai/__init__.py
--rw-rw-rw-   0        0        0    12749 2024-05-22 17:57:29.000000 ipiranga-inovai-project-lib-0.9/inovai/entities.py
--rw-rw-rw-   0        0        0      887 2024-05-27 20:47:20.000000 ipiranga-inovai-project-lib-0.9/inovai/enums.py
-drwxrwxrwx   0        0        0        0 2024-05-29 19:10:34.627660 ipiranga-inovai-project-lib-0.9/ipiranga_inovai_project_lib.egg-info/
--rw-rw-rw-   0        0        0      516 2024-05-29 19:10:34.000000 ipiranga-inovai-project-lib-0.9/ipiranga_inovai_project_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-05-29 19:10:34.000000 ipiranga-inovai-project-lib-0.9/ipiranga_inovai_project_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 19:10:34.000000 ipiranga-inovai-project-lib-0.9/ipiranga_inovai_project_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-29 19:10:34.000000 ipiranga-inovai-project-lib-0.9/ipiranga_inovai_project_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 19:10:34.632332 ipiranga-inovai-project-lib-0.9/setup.cfg
--rw-rw-rw-   0        0        0      689 2024-05-29 19:10:26.000000 ipiranga-inovai-project-lib-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 19:19:52.991609 ipiranga-inovai-project-lib-1.0/
+-rw-rw-rw-   0        0        0      198 2024-04-05 19:57:15.000000 ipiranga-inovai-project-lib-1.0/LICENSE
+-rw-rw-rw-   0        0        0      516 2024-05-29 19:19:52.989595 ipiranga-inovai-project-lib-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-05 19:18:28.000000 ipiranga-inovai-project-lib-1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 19:19:52.895072 ipiranga-inovai-project-lib-1.0/inovai/
+-rw-rw-rw-   0        0        0        0 2024-04-05 20:33:51.000000 ipiranga-inovai-project-lib-1.0/inovai/__init__.py
+-rw-rw-rw-   0        0        0    12749 2024-05-22 17:57:29.000000 ipiranga-inovai-project-lib-1.0/inovai/entities.py
+-rw-rw-rw-   0        0        0      887 2024-05-27 20:47:20.000000 ipiranga-inovai-project-lib-1.0/inovai/enums.py
+drwxrwxrwx   0        0        0        0 2024-05-29 19:19:52.975367 ipiranga-inovai-project-lib-1.0/inovai/models/
+-rw-rw-rw-   0        0        0     3519 2024-05-24 19:04:49.000000 ipiranga-inovai-project-lib-1.0/inovai/models/Endereco.py
+-rw-rw-rw-   0        0        0    13172 2024-05-29 14:47:31.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFe.py
+-rw-rw-rw-   0        0        0     5006 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeBoleto.py
+-rw-rw-rw-   0        0        0     1876 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeCartao.py
+-rw-rw-rw-   0        0        0     2021 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeDetalhePagamento.py
+-rw-rw-rw-   0        0        0     3291 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeDocImportacao.py
+-rw-rw-rw-   0        0        0     1899 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeDocImportacaoAdicao.py
+-rw-rw-rw-   0        0        0     2111 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeDocRef.py
+-rw-rw-rw-   0        0        0     1693 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeDuplicata.py
+-rw-rw-rw-   0        0        0     1826 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeEnvioXML.py
+-rw-rw-rw-   0        0        0     3548 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeEnvolvido.py
+-rw-rw-rw-   0        0        0     1716 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeExportacao.py
+-rw-rw-rw-   0        0        0     1801 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeFatura.py
+-rw-rw-rw-   0        0        0     5870 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeImposto.py
+-rw-rw-rw-   0        0        0     3707 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeImpostoRetido.py
+-rw-rw-rw-   0        0        0     1645 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeIntermediadorTransacao.py
+-rw-rw-rw-   0        0        0     5938 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeItem.py
+-rw-rw-rw-   0        0        0     2244 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeItemDadosCombustivel.py
+-rw-rw-rw-   0        0        0     2526 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeItemExportacao.py
+-rw-rw-rw-   0        0        0     1809 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeItemOrigemCombustivel.py
+-rw-rw-rw-   0        0        0     1665 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeObservacao.py
+-rw-rw-rw-   0        0        0     1669 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeObservacaoItem.py
+-rw-rw-rw-   0        0        0     1684 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeOrigem.py
+-rw-rw-rw-   0        0        0     1746 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFePagamento.py
+-rw-rw-rw-   0        0        0     1815 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeProcReferenciado.py
+-rw-rw-rw-   0        0        0     2251 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeTransporte.py
+-rw-rw-rw-   0        0        0     1736 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeVeiculo.py
+-rw-rw-rw-   0        0        0     1970 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeVolume.py
+-rw-rw-rw-   0        0        0        0 2024-04-05 20:33:51.000000 ipiranga-inovai-project-lib-1.0/inovai/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 19:19:52.987460 ipiranga-inovai-project-lib-1.0/ipiranga_inovai_project_lib.egg-info/
+-rw-rw-rw-   0        0        0      516 2024-05-29 19:19:52.000000 ipiranga-inovai-project-lib-1.0/ipiranga_inovai_project_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1190 2024-05-29 19:19:52.000000 ipiranga-inovai-project-lib-1.0/ipiranga_inovai_project_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 19:19:52.000000 ipiranga-inovai-project-lib-1.0/ipiranga_inovai_project_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-29 19:19:52.000000 ipiranga-inovai-project-lib-1.0/ipiranga_inovai_project_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 19:19:52.992608 ipiranga-inovai-project-lib-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      689 2024-05-29 19:19:00.000000 ipiranga-inovai-project-lib-1.0/setup.py
```

### Comparing `ipiranga-inovai-project-lib-0.9/PKG-INFO` & `ipiranga-inovai-project-lib-1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipiranga-inovai-project-lib
-Version: 0.9
+Version: 1.0
 Summary: Projeto criado para importação genérica de entidades
 Home-page: https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib
 Author: Clayton Sandes Monteiro
 Author-email: clayton.monteiro.ext@ipiranga.ipiranga
 License: MIT
 Keywords: inovai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipiranga-inovai-project-lib-0.9/inovai/entities.py` & `ipiranga-inovai-project-lib-1.0/inovai/entities.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-0.9/inovai/enums.py` & `ipiranga-inovai-project-lib-1.0/inovai/enums.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-0.9/ipiranga_inovai_project_lib.egg-info/PKG-INFO` & `ipiranga-inovai-project-lib-1.0/ipiranga_inovai_project_lib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipiranga-inovai-project-lib
-Version: 0.9
+Version: 1.0
 Summary: Projeto criado para importação genérica de entidades
 Home-page: https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib
 Author: Clayton Sandes Monteiro
 Author-email: clayton.monteiro.ext@ipiranga.ipiranga
 License: MIT
 Keywords: inovai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipiranga-inovai-project-lib-0.9/setup.py` & `ipiranga-inovai-project-lib-1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ipiranga-inovai-project-lib",
-    version="0.9",
+    version="1.0",
     packages=find_packages(),
     description="Projeto criado para importação genérica de entidades",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="Clayton Sandes Monteiro",
     author_email="clayton.monteiro.ext@ipiranga.ipiranga",
     url="https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib",
```

