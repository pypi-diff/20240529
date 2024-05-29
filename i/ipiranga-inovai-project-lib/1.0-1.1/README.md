# Comparing `tmp/ipiranga-inovai-project-lib-1.0.tar.gz` & `tmp/ipiranga-inovai-project-lib-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipiranga-inovai-project-lib-1.0.tar", last modified: Wed May 29 19:19:52 2024, max compression
+gzip compressed data, was "ipiranga-inovai-project-lib-1.1.tar", last modified: Wed May 29 19:27:28 2024, max compression
```

## Comparing `ipiranga-inovai-project-lib-1.0.tar` & `ipiranga-inovai-project-lib-1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 19:19:52.991609 ipiranga-inovai-project-lib-1.0/
--rw-rw-rw-   0        0        0      198 2024-04-05 19:57:15.000000 ipiranga-inovai-project-lib-1.0/LICENSE
--rw-rw-rw-   0        0        0      516 2024-05-29 19:19:52.989595 ipiranga-inovai-project-lib-1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-05 19:18:28.000000 ipiranga-inovai-project-lib-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 19:19:52.895072 ipiranga-inovai-project-lib-1.0/inovai/
--rw-rw-rw-   0        0        0        0 2024-04-05 20:33:51.000000 ipiranga-inovai-project-lib-1.0/inovai/__init__.py
--rw-rw-rw-   0        0        0    12749 2024-05-22 17:57:29.000000 ipiranga-inovai-project-lib-1.0/inovai/entities.py
--rw-rw-rw-   0        0        0      887 2024-05-27 20:47:20.000000 ipiranga-inovai-project-lib-1.0/inovai/enums.py
-drwxrwxrwx   0        0        0        0 2024-05-29 19:19:52.975367 ipiranga-inovai-project-lib-1.0/inovai/models/
--rw-rw-rw-   0        0        0     3519 2024-05-24 19:04:49.000000 ipiranga-inovai-project-lib-1.0/inovai/models/Endereco.py
--rw-rw-rw-   0        0        0    13172 2024-05-29 14:47:31.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFe.py
--rw-rw-rw-   0        0        0     5006 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeBoleto.py
--rw-rw-rw-   0        0        0     1876 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeCartao.py
--rw-rw-rw-   0        0        0     2021 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeDetalhePagamento.py
--rw-rw-rw-   0        0        0     3291 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeDocImportacao.py
--rw-rw-rw-   0        0        0     1899 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeDocImportacaoAdicao.py
--rw-rw-rw-   0        0        0     2111 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeDocRef.py
--rw-rw-rw-   0        0        0     1693 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeDuplicata.py
--rw-rw-rw-   0        0        0     1826 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeEnvioXML.py
--rw-rw-rw-   0        0        0     3548 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeEnvolvido.py
--rw-rw-rw-   0        0        0     1716 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeExportacao.py
--rw-rw-rw-   0        0        0     1801 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeFatura.py
--rw-rw-rw-   0        0        0     5870 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeImposto.py
--rw-rw-rw-   0        0        0     3707 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeImpostoRetido.py
--rw-rw-rw-   0        0        0     1645 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeIntermediadorTransacao.py
--rw-rw-rw-   0        0        0     5938 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeItem.py
--rw-rw-rw-   0        0        0     2244 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeItemDadosCombustivel.py
--rw-rw-rw-   0        0        0     2526 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeItemExportacao.py
--rw-rw-rw-   0        0        0     1809 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeItemOrigemCombustivel.py
--rw-rw-rw-   0        0        0     1665 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeObservacao.py
--rw-rw-rw-   0        0        0     1669 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeObservacaoItem.py
--rw-rw-rw-   0        0        0     1684 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeOrigem.py
--rw-rw-rw-   0        0        0     1746 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFePagamento.py
--rw-rw-rw-   0        0        0     1815 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeProcReferenciado.py
--rw-rw-rw-   0        0        0     2251 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeTransporte.py
--rw-rw-rw-   0        0        0     1736 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeVeiculo.py
--rw-rw-rw-   0        0        0     1970 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.0/inovai/models/NFeVolume.py
--rw-rw-rw-   0        0        0        0 2024-04-05 20:33:51.000000 ipiranga-inovai-project-lib-1.0/inovai/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 19:19:52.987460 ipiranga-inovai-project-lib-1.0/ipiranga_inovai_project_lib.egg-info/
--rw-rw-rw-   0        0        0      516 2024-05-29 19:19:52.000000 ipiranga-inovai-project-lib-1.0/ipiranga_inovai_project_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1190 2024-05-29 19:19:52.000000 ipiranga-inovai-project-lib-1.0/ipiranga_inovai_project_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 19:19:52.000000 ipiranga-inovai-project-lib-1.0/ipiranga_inovai_project_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-29 19:19:52.000000 ipiranga-inovai-project-lib-1.0/ipiranga_inovai_project_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 19:19:52.992608 ipiranga-inovai-project-lib-1.0/setup.cfg
--rw-rw-rw-   0        0        0      689 2024-05-29 19:19:00.000000 ipiranga-inovai-project-lib-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 19:27:28.361287 ipiranga-inovai-project-lib-1.1/
+-rw-rw-rw-   0        0        0      198 2024-04-05 19:57:15.000000 ipiranga-inovai-project-lib-1.1/LICENSE
+-rw-rw-rw-   0        0        0      516 2024-05-29 19:27:28.358566 ipiranga-inovai-project-lib-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-05 19:18:28.000000 ipiranga-inovai-project-lib-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 19:27:28.257376 ipiranga-inovai-project-lib-1.1/inovai/
+-rw-rw-rw-   0        0        0        0 2024-04-05 20:33:51.000000 ipiranga-inovai-project-lib-1.1/inovai/__init__.py
+-rw-rw-rw-   0        0        0    12749 2024-05-22 17:57:29.000000 ipiranga-inovai-project-lib-1.1/inovai/entities.py
+-rw-rw-rw-   0        0        0      887 2024-05-27 20:47:20.000000 ipiranga-inovai-project-lib-1.1/inovai/enums.py
+drwxrwxrwx   0        0        0        0 2024-05-29 19:27:28.346566 ipiranga-inovai-project-lib-1.1/inovai/models/
+-rw-rw-rw-   0        0        0     3519 2024-05-24 19:04:49.000000 ipiranga-inovai-project-lib-1.1/inovai/models/Endereco.py
+-rw-rw-rw-   0        0        0    13172 2024-05-29 19:26:54.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFe.py
+-rw-rw-rw-   0        0        0     5006 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeBoleto.py
+-rw-rw-rw-   0        0        0     1876 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeCartao.py
+-rw-rw-rw-   0        0        0     2021 2024-05-29 19:26:54.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeDetalhePagamento.py
+-rw-rw-rw-   0        0        0     3291 2024-05-29 19:26:54.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeDocImportacao.py
+-rw-rw-rw-   0        0        0     1899 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeDocImportacaoAdicao.py
+-rw-rw-rw-   0        0        0     2111 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeDocRef.py
+-rw-rw-rw-   0        0        0     1693 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeDuplicata.py
+-rw-rw-rw-   0        0        0     1826 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeEnvioXML.py
+-rw-rw-rw-   0        0        0     3548 2024-05-29 19:26:54.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeEnvolvido.py
+-rw-rw-rw-   0        0        0     1716 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeExportacao.py
+-rw-rw-rw-   0        0        0     1801 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeFatura.py
+-rw-rw-rw-   0        0        0     5870 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeImposto.py
+-rw-rw-rw-   0        0        0     3707 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeImpostoRetido.py
+-rw-rw-rw-   0        0        0     1645 2024-05-24 11:51:40.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeIntermediadorTransacao.py
+-rw-rw-rw-   0        0        0     5938 2024-05-29 19:26:54.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeItem.py
+-rw-rw-rw-   0        0        0     2244 2024-05-29 19:26:54.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeItemDadosCombustivel.py
+-rw-rw-rw-   0        0        0     2526 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeItemExportacao.py
+-rw-rw-rw-   0        0        0     1809 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeItemOrigemCombustivel.py
+-rw-rw-rw-   0        0        0     1665 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeObservacao.py
+-rw-rw-rw-   0        0        0     1669 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeObservacaoItem.py
+-rw-rw-rw-   0        0        0     1684 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeOrigem.py
+-rw-rw-rw-   0        0        0     1746 2024-05-29 19:26:54.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFePagamento.py
+-rw-rw-rw-   0        0        0     1815 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeProcReferenciado.py
+-rw-rw-rw-   0        0        0     2251 2024-05-29 19:26:54.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeTransporte.py
+-rw-rw-rw-   0        0        0     1736 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeVeiculo.py
+-rw-rw-rw-   0        0        0     1970 2024-05-24 11:51:41.000000 ipiranga-inovai-project-lib-1.1/inovai/models/NFeVolume.py
+-rw-rw-rw-   0        0        0        0 2024-04-05 20:33:51.000000 ipiranga-inovai-project-lib-1.1/inovai/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 19:27:28.356566 ipiranga-inovai-project-lib-1.1/ipiranga_inovai_project_lib.egg-info/
+-rw-rw-rw-   0        0        0      516 2024-05-29 19:27:28.000000 ipiranga-inovai-project-lib-1.1/ipiranga_inovai_project_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1190 2024-05-29 19:27:28.000000 ipiranga-inovai-project-lib-1.1/ipiranga_inovai_project_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 19:27:28.000000 ipiranga-inovai-project-lib-1.1/ipiranga_inovai_project_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-29 19:27:28.000000 ipiranga-inovai-project-lib-1.1/ipiranga_inovai_project_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 19:27:28.362286 ipiranga-inovai-project-lib-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      689 2024-05-29 19:27:16.000000 ipiranga-inovai-project-lib-1.1/setup.py
```

### Comparing `ipiranga-inovai-project-lib-1.0/PKG-INFO` & `ipiranga-inovai-project-lib-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipiranga-inovai-project-lib
-Version: 1.0
+Version: 1.1
 Summary: Projeto criado para importação genérica de entidades
 Home-page: https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib
 Author: Clayton Sandes Monteiro
 Author-email: clayton.monteiro.ext@ipiranga.ipiranga
 License: MIT
 Keywords: inovai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/entities.py` & `ipiranga-inovai-project-lib-1.1/inovai/entities.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/enums.py` & `ipiranga-inovai-project-lib-1.1/inovai/enums.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/Endereco.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/Endereco.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFe.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from config import context
-from domain.enum.document_type import DocumentType
+from inovai.enum.document_type import DocumentType
 from inovai.enums import TaxType
-from domain.models.NFeBoleto import NFeBoleto
-from domain.models.NFeDocRef import NFeDocRef
-from domain.models.NFeDuplicata import NFeDuplicata
-from domain.models.NFeEnvioXML import NFeEnvioXML
-from domain.models.NFeEnvolvido import NFeEnvolvido
-from domain.models.NFeExportacao import NFeExportacao
-from domain.models.NFeFatura import NFeFatura
-from domain.models.NFeImpostoRetido import NFeImpostoRetido
-from domain.models.NFeIntermediadorTransacao import NFeIntermediadorTransacao
-from domain.models.NFeItem import NFeItem
-from domain.models.NFeObservacao import NFeObservacao
-from domain.models.NFePagamento import NFePagamento
-from domain.models.NFeProcReferenciado import NFeProcReferenciado
-from domain.models.NFeTransporte import NFeTransporte
+from inovai.models.NFeBoleto import NFeBoleto
+from inovai.models.NFeDocRef import NFeDocRef
+from inovai.models.NFeDuplicata import NFeDuplicata
+from inovai.models.NFeEnvioXML import NFeEnvioXML
+from inovai.models.NFeEnvolvido import NFeEnvolvido
+from inovai.models.NFeExportacao import NFeExportacao
+from inovai.models.NFeFatura import NFeFatura
+from inovai.models.NFeImpostoRetido import NFeImpostoRetido
+from inovai.models.NFeIntermediadorTransacao import NFeIntermediadorTransacao
+from inovai.models.NFeItem import NFeItem
+from inovai.models.NFeObservacao import NFeObservacao
+from inovai.models.NFePagamento import NFePagamento
+from inovai.models.NFeProcReferenciado import NFeProcReferenciado
+from inovai.models.NFeTransporte import NFeTransporte
 import xml.etree.ElementTree as ET
 
-from domain.util.util import format_date
+from inovai.util.util import format_date
 
 
 class NFe:
     boletos: [NFeBoleto]
     chaveAcesso: str
     cnpjMovimentacao: str
     codFilial: str
```

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeBoleto.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeBoleto.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeCartao.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeCartao.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeDetalhePagamento.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeDetalhePagamento.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from domain.models.NFeCartao import NFeCartao
+from inovai.models.NFeCartao import NFeCartao
 class NFeDetalhePagamento:
 	descricaoMeioPagamento: str
 	formaPagamento: str
 	pagamentoCartao: NFeCartao
 	tipoFormaPagamento: int
 	valorPagamento: float
```

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeDocImportacao.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeDocImportacao.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from domain.models.NFeDocImportacaoAdicao import NFeDocImportacaoAdicao
-from domain.models.NFeEnvolvido import NFeEnvolvido
-from domain.models.NFeOrigem import NFeOrigem
+from inovai.models.NFeDocImportacaoAdicao import NFeDocImportacaoAdicao
+from inovai.models.NFeEnvolvido import NFeEnvolvido
+from inovai.models.NFeOrigem import NFeOrigem
 class NFeDocImportacao:
 	adicoes: [NFeDocImportacaoAdicao]
 	codigoExportador: str
 	dataRegistro: str
 	desembaracoData: str
 	desembaracoLocal: str
 	desembaracoUF: str
```

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeDocImportacaoAdicao.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeDocImportacaoAdicao.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeDocRef.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeDocRef.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeDuplicata.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeDuplicata.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeEnvioXML.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeEnvioXML.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeEnvolvido.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeEnvolvido.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from domain.models.Endereco import Endereco
+from inovai.models.Endereco import Endereco
 
 
 class NFeEnvolvido:
     cnae: str
     cpfCNPJ: str
     email: str
     endereco: Endereco
```

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeExportacao.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeExportacao.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeFatura.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeFatura.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeImposto.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeImposto.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeImpostoRetido.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeImpostoRetido.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeIntermediadorTransacao.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeIntermediadorTransacao.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeItem.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeItem.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from domain.models.NFeDocImportacao import NFeDocImportacao
-from domain.models.NFeImposto import NFeImposto
-from domain.models.NFeItemDadosCombustivel import NFeItemDadosCombustivel
-from domain.models.NFeItemExportacao import NFeItemExportacao
-from domain.models.NFeObservacaoItem import NFeObservacaoItem
+from inovai.models.NFeDocImportacao import NFeDocImportacao
+from inovai.models.NFeImposto import NFeImposto
+from inovai.models.NFeItemDadosCombustivel import NFeItemDadosCombustivel
+from inovai.models.NFeItemExportacao import NFeItemExportacao
+from inovai.models.NFeObservacaoItem import NFeObservacaoItem
 import xml.etree.ElementTree as ET
 
 class NFeItem:
 	DIs: [NFeDocImportacao]
 	cBarra: str
 	cBarraTrib: str
 	cEAN: str
```

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeItemDadosCombustivel.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeItemDadosCombustivel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from domain.models.NFeItemOrigemCombustivel import NFeItemOrigemCombustivel
+from inovai.models.NFeItemOrigemCombustivel import NFeItemOrigemCombustivel
 class NFeItemDadosCombustivel:
 	cProdANP: str
 	codif: str
 	descANP: str
 	origemCombustivel: [NFeItemOrigemCombustivel]
 	percentualBioDiesel: float
 	percentualGLP: float
```

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeItemExportacao.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeItemExportacao.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeItemOrigemCombustivel.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeItemOrigemCombustivel.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeObservacao.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeObservacao.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeObservacaoItem.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeObservacaoItem.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeOrigem.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeOrigem.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFePagamento.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFePagamento.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from domain.models.NFeDetalhePagamento import NFeDetalhePagamento
+from inovai.models.NFeDetalhePagamento import NFeDetalhePagamento
 class NFePagamento:
 	detalhesPagamento: [NFeDetalhePagamento]
 	valorTroco: float
 
 	def __init__(self, **json):
 		if json:
 			for key, typeProp in self.__class__.__dict__['__annotations__'].items():
```

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeProcReferenciado.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeProcReferenciado.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeTransporte.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeTransporte.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from domain.models.NFeEnvolvido import NFeEnvolvido
-from domain.models.NFeImposto import NFeImposto
-from domain.models.NFeVeiculo import NFeVeiculo
-from domain.models.NFeVolume import NFeVolume
+from inovai.models.NFeEnvolvido import NFeEnvolvido
+from inovai.models.NFeImposto import NFeImposto
+from inovai.models.NFeVeiculo import NFeVeiculo
+from inovai.models.NFeVolume import NFeVolume
 class NFeTransporte:
 	contratoTransporte: str
 	icmsRetido: NFeImposto
 	modal: int
 	transportador: NFeEnvolvido
 	valorServico: float
 	veiculos: [NFeVeiculo]
```

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeVeiculo.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeVeiculo.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/inovai/models/NFeVolume.py` & `ipiranga-inovai-project-lib-1.1/inovai/models/NFeVolume.py`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/ipiranga_inovai_project_lib.egg-info/PKG-INFO` & `ipiranga-inovai-project-lib-1.1/ipiranga_inovai_project_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipiranga-inovai-project-lib
-Version: 1.0
+Version: 1.1
 Summary: Projeto criado para importação genérica de entidades
 Home-page: https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib
 Author: Clayton Sandes Monteiro
 Author-email: clayton.monteiro.ext@ipiranga.ipiranga
 License: MIT
 Keywords: inovai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipiranga-inovai-project-lib-1.0/ipiranga_inovai_project_lib.egg-info/SOURCES.txt` & `ipiranga-inovai-project-lib-1.1/ipiranga_inovai_project_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipiranga-inovai-project-lib-1.0/setup.py` & `ipiranga-inovai-project-lib-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ipiranga-inovai-project-lib",
-    version="1.0",
+    version="1.1",
     packages=find_packages(),
     description="Projeto criado para importação genérica de entidades",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="Clayton Sandes Monteiro",
     author_email="clayton.monteiro.ext@ipiranga.ipiranga",
     url="https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib",
```

