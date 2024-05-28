# Comparing `tmp/getpaper-0.4.9.tar.gz` & `tmp/getpaper-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.4.9.tar", last modified: Sun Feb 25 12:28:13 2024, max compression
+gzip compressed data, was "getpaper-0.5.0.tar", last modified: Tue May 28 23:03:52 2024, max compression
```

## Comparing `getpaper-0.4.9.tar` & `getpaper-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2024-02-25 12:28:13.335152 getpaper-0.4.9/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.4.9/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4933 2024-02-25 12:28:13.335152 getpaper-0.4.9/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4240 2024-01-11 23:31:38.000000 getpaper-0.4.9/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2024-02-25 12:28:13.335152 getpaper-0.4.9/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.4.9/getpaper/__init__.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    20250 2024-02-25 11:54:25.000000 getpaper-0.4.9/getpaper/download.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    22594 2024-02-25 12:25:02.000000 getpaper-0.4.9/getpaper/parse.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4625 2023-11-21 00:14:33.000000 getpaper-0.4.9/getpaper/selenium_download.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      781 2023-11-20 21:07:40.000000 getpaper-0.4.9/getpaper/test.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2024-02-25 12:28:13.335152 getpaper-0.4.9/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4933 2024-02-25 12:28:13.000000 getpaper-0.4.9/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      327 2024-02-25 12:28:13.000000 getpaper-0.4.9/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2024-02-25 12:28:13.000000 getpaper-0.4.9/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       78 2024-02-25 12:28:13.000000 getpaper-0.4.9/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      415 2024-02-25 12:28:13.000000 getpaper-0.4.9/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2024-02-25 12:28:13.000000 getpaper-0.4.9/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2024-02-25 12:28:13.335152 getpaper-0.4.9/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     2044 2024-02-25 12:08:02.000000 getpaper-0.4.9/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2024-05-28 23:03:52.317352 getpaper-0.5.0/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.5.0/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5099 2024-05-28 23:03:52.317352 getpaper-0.5.0/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4406 2024-05-28 22:58:58.000000 getpaper-0.5.0/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2024-05-28 23:03:52.317352 getpaper-0.5.0/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.5.0/getpaper/__init__.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    23635 2024-05-28 22:55:22.000000 getpaper-0.5.0/getpaper/download.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    22594 2024-02-25 12:25:02.000000 getpaper-0.5.0/getpaper/parse.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4625 2024-05-28 22:53:46.000000 getpaper-0.5.0/getpaper/selenium_download.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      781 2023-11-20 21:07:40.000000 getpaper-0.5.0/getpaper/test.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2024-05-28 23:03:52.317352 getpaper-0.5.0/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5099 2024-05-28 23:03:52.000000 getpaper-0.5.0/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      327 2024-05-28 23:03:52.000000 getpaper-0.5.0/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2024-05-28 23:03:52.000000 getpaper-0.5.0/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       78 2024-05-28 23:03:52.000000 getpaper-0.5.0/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      413 2024-05-28 23:03:52.000000 getpaper-0.5.0/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2024-05-28 23:03:52.000000 getpaper-0.5.0/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2024-05-28 23:03:52.317352 getpaper-0.5.0/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     2042 2024-05-28 22:55:22.000000 getpaper-0.5.0/setup.py
```

### Comparing `getpaper-0.4.9/LICENSE` & `getpaper-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.4.9/PKG-INFO` & `getpaper-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.4.9
+Version: 0.5.0
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -45,19 +45,20 @@
 ## Downloading papers
 
 After the installation you can either import the library into your python code or you can use the console scripts.
 
 If you install from pip calling _download_ will mean calling getpaper/download.py , for _parse_ - getpaper/parse.py , for _index_ - getpaper/index.py
 
 ```bash
-download download_pubmed --pubmed 22266545 --folder "data/output/test/papers" --name pmid
+download download_pubmed --pubmed 22266545 --folder "data/output/test/papers" --name pmid --loglevel info  --scihub_on_fail True
 ```
 Downloads the paper with pubmed id into the folder 'papers' and uses the pubmed id as name
+
 ```bash
-download download_doi --doi 10.1038/s41597-020-00710-z --folder "data/output/test/papers"
+download download_doi --doi 10.1038/s41597-020-00710-z --folder "data/output/test/papers" --scihub_on_fail True
 ```
 Downloads the paper with DOI into the folder papers, as --name is not specified doi is used as name
 
 It is also possible to download many papers in parallel with download_papers(dois: List[str], destination: Path, threads: int) function, for example:
 ```python
 from pathlib import Path
 from typing import List
@@ -126,10 +127,11 @@
 ```
 
 Detectron2 is required for using models from the layoutparser model zoo but is not automatically installed with this package. 
 For macOS and Linux, build from source with:
 
 pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
 
-# Note
+# Notes
 
+Sometimes semantic-scholar change their APIs, so if the library stops working for you, open the issue.
 Since 0.3.0 version all indexing features were moved to indexpaper library
```

### Comparing `getpaper-0.4.9/README.md` & `getpaper-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,20 @@
 ## Downloading papers
 
 After the installation you can either import the library into your python code or you can use the console scripts.
 
 If you install from pip calling _download_ will mean calling getpaper/download.py , for _parse_ - getpaper/parse.py , for _index_ - getpaper/index.py
 
 ```bash
-download download_pubmed --pubmed 22266545 --folder "data/output/test/papers" --name pmid
+download download_pubmed --pubmed 22266545 --folder "data/output/test/papers" --name pmid --loglevel info  --scihub_on_fail True
 ```
 Downloads the paper with pubmed id into the folder 'papers' and uses the pubmed id as name
+
 ```bash
-download download_doi --doi 10.1038/s41597-020-00710-z --folder "data/output/test/papers"
+download download_doi --doi 10.1038/s41597-020-00710-z --folder "data/output/test/papers" --scihub_on_fail True
 ```
 Downloads the paper with DOI into the folder papers, as --name is not specified doi is used as name
 
 It is also possible to download many papers in parallel with download_papers(dois: List[str], destination: Path, threads: int) function, for example:
 ```python
 from pathlib import Path
 from typing import List
@@ -105,10 +106,11 @@
 ```
 
 Detectron2 is required for using models from the layoutparser model zoo but is not automatically installed with this package. 
 For macOS and Linux, build from source with:
 
 pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
 
-# Note
+# Notes
 
+Sometimes semantic-scholar change their APIs, so if the library stops working for you, open the issue.
 Since 0.3.0 version all indexing features were moved to indexpaper library
```

### Comparing `getpaper-0.4.9/getpaper/download.py` & `getpaper-0.5.0/getpaper/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 from __future__ import annotations
 import asyncio
 import json
 import os
+import pprint
 import xml.etree.ElementTree as ET
 from collections import OrderedDict
 from concurrent.futures import Executor
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 from typing import Optional, List
 import click
@@ -23,14 +24,94 @@
 import sys
 
 from pycomfort.config import LOG_LEVELS, configure_logger, LogLevel
 from unpywall import Unpywall
 from unpywall.utils import UnpywallCredentials
 import nest_asyncio
 
+SEMANTIC_SCHOLAR_FIELDS = [
+    'abstract',
+    'authors',
+    'authors.affiliations',
+    #'authors.aliases',
+    'authors.authorId',
+    'authors.citationCount',
+    'authors.externalIds',
+    'authors.hIndex',
+    'authors.homepage',
+    'authors.name',
+    'authors.paperCount',
+    'authors.url',
+    'citationCount',
+    'citationStyles',
+    'citations',
+    'citations.abstract',
+    'citations.authors',
+    'citations.citationCount',
+    'citations.citationStyles',
+    'citations.corpusId',
+    'citations.externalIds',
+    'citations.fieldsOfStudy',
+    'citations.influentialCitationCount',
+    'citations.isOpenAccess',
+    'citations.journal',
+    'citations.openAccessPdf',
+    'citations.paperId',
+    'citations.publicationDate',
+    'citations.publicationTypes',
+    'citations.publicationVenue',
+    'citations.referenceCount',
+    'citations.s2FieldsOfStudy',
+    'citations.title',
+    'citations.url',
+    'citations.venue',
+    'citations.year',
+    'corpusId',
+    'embedding',
+    'externalIds',
+    'fieldsOfStudy',
+    'influentialCitationCount',
+    'isOpenAccess',
+    'journal',
+    'openAccessPdf',
+    'paperId',
+    'publicationDate',
+    'publicationTypes',
+    'publicationVenue',
+    'referenceCount',
+    'references',
+    'references.abstract',
+    'references.authors',
+    'references.citationCount',
+    'references.citationStyles',
+    'references.corpusId',
+    'references.externalIds',
+    'references.fieldsOfStudy',
+    'references.influentialCitationCount',
+    'references.isOpenAccess',
+    'references.journal',
+    'references.openAccessPdf',
+    'references.paperId',
+    'references.publicationDate',
+    'references.publicationTypes',
+    'references.publicationVenue',
+    'references.referenceCount',
+    'references.s2FieldsOfStudy',
+    'references.title',
+    'references.url',
+    'references.venue',
+    'references.year',
+    's2FieldsOfStudy',
+    'title',
+    'tldr',
+    'url',
+    'venue',
+    'year'
+]
+
 #DownloadedPaper = (str, Optional[Path], Optional[Path]) #type synonim for doi, Path, Path of the downloaded paper
 @dataclass
 class PaperDownload:
     id: str
     pdf: Optional[Path]
     metadata: Optional[Path]
     parsed: Optional[list[Path]] = None
@@ -118,28 +199,38 @@
     doi_from_pubmed wrapped in try
     :param pubmed:
     :return:
     """
     return Try.of(lambda: doi_from_pubmed(pubmed))
 
 
+def get_semantic_paper(paper_id: str, api_key: Optional[str] = None):
+    """
+    just a fix for non-working semantic-scholar
+    :param paper_id:
+    :param api_key:
+    :return:
+    """
+    sch = SemanticScholar(api_key=api_key)
+    return sch.get_paper(paper_id, fields=SEMANTIC_SCHOLAR_FIELDS)
+
 def resolve_semantic_scholar(paper_id: str,
                               metadata: Optional[Path] = None,
                               logger: Optional["loguru.Logger"] = None) -> PaperDownload:
     if logger is None:
         logger = loguru.logger
     logger.info(f"RESOLVING PAPER {paper_id} with meta and {metadata}")
-    sch = SemanticScholar()
-    paper: Paper = sch.get_paper(paper_id)
+    paper: Paper = get_semantic_paper(paper_id)
     if metadata is not None:
         json_data = json.dumps(paper.raw_data)
         metadata.touch(exist_ok=True)
         metadata.write_text(json_data)
         logger.info(f"metadata for {paper_id} successfully written to {metadata}")
     if paper.openAccessPdf is not None and "url" in paper.openAccessPdf:
+        logger.info(f"URL {paper.openAccessPdf}")
         url = paper.openAccessPdf["url"]
     else:
         url = None
     return PaperDownload(paper_id, None, metadata, None, url)
 
 #@logger.catch(reraise=False)
 def download_semantic_scholar(paper_id: str,
@@ -187,15 +278,17 @@
 def try_download(doi: str,
                  destination: Path,
                  skip_if_exist: bool = True,
                  name: Optional[str] = None,
                  scihub_on_fail: bool = False,
                  unpaywall_email: Optional[str] = None,
                  selenium_on_fail: bool = False,
-                 selenium_headless: bool=True, selenium_min_wait: int=12, selenium_max_wait: int=60,
+                 selenium_headless: bool = True,
+                 selenium_min_wait: int = 12,
+                 selenium_max_wait: int = 60,
                  logger: Optional["loguru.Logger"] = None
                  ) -> Try[PaperDownload]:
     """
     :param doi:
     :param destination:
     :param skip_if_exist:
     :param name:
@@ -217,45 +310,48 @@
     meta = paper.parent / paper.name.replace(".pdf", "_meta.json")
     if skip_if_exist and paper.exists():
         p = PaperDownload(doi, paper, meta)
         if p.parsed is None and p.get_paper_folder() is not None:
             p.parsed = [p.get_paper_folder()]
         logger.info(f"paper {paper} already exists, skipping!")
         return Try.of(lambda: p)
-
     p: PaperDownload = resolve_semantic_scholar(doi, meta, logger)
     if unpaywall_email is not None:
         unpaywall_email = os.getenv("UNPAYWALL_EMAIL")
     if unpaywall_email is not None and p.url is None:
         UnpywallCredentials(unpaywall_email)
         p.url = Unpywall.get_pdf_link(doi)
+    if p.url is None:
+        logger.info(f"Semantic scholar and unpaywall could not found any openaccess URLs for the {p.id} paper")
     try_simple = Try.of(lambda: p.with_pdf(simple_download(p.url, paper, logger = logger)))
     if selenium_on_fail and p.url is not None:
         from getpaper.selenium_download import download_pdf_selenium
-        logger.trace(f"paper to download with selenium is {p}")
+        logger.debug(f"paper to download with selenium is {p}")
         before_last = try_simple.catch(lambda ex: p.with_pdf(download_pdf_selenium(p.url, destination, selenium_headless, selenium_min_wait, selenium_max_wait, final_path=paper, logger=logger)))
     else:
         before_last = try_simple
     before_last.on_failure(lambda e: logger.error(e))
     return before_last.catch(lambda _: schihub_doi(doi, paper, meta, logger)) if scihub_on_fail else before_last
 
 
-def download_pubmed(pubmed: str, destination: Path, skip_if_exist: bool = True, name: Optional[str] = None, scihub_on_fail: bool = False):
+def download_pubmed(pubmed: str, destination: Path, skip_if_exist: bool = True, name: Optional[str] = None, scihub_on_fail: bool = False, logger: Optional["loguru.Logger"] = None):
     """
     downloads paper by its pubmed id
     :param pubmed: pubmed id
     :param destination: where to store the result
     :param skip_if_exist:
     :param name:
     :param scihub_on_fail: if SciHub should be used as back up resolver. False by default. For paywalled articles it can be illegal in some of the countries, so use it at your own risk.
     :return:
     """
     try_resolve = try_doi_from_pubmed(pubmed)
-    return try_resolve.flat_map(lambda doi: try_download(doi, destination, skip_if_exist, name, scihub_on_fail))
-
+    result =  try_resolve.flat_map(lambda doi: try_download(doi, destination, skip_if_exist, name, scihub_on_fail, logger=logger))
+    if logger is not None:
+        result.on_failure(lambda ex: logger.error(ex))
+    return result
 
 async def download_async(executor: Executor,
                              doi: str, destination: Path,
                              skip_if_exist: bool = True,
                              name: Optional[str] = None,
                              scihub_on_fail: bool = False,
                              logger: Optional["loguru.Logger"] = None
@@ -265,15 +361,17 @@
 
     Args:
         executor (Executor): The ThreadPoolExecutor to run blocking IO in.
         doi (str): The DOI of the paper to download.
         destination (Path): The directory where the downloaded paper should be stored.
         skip_if_exist (bool): If True, skip the download if the paper already exists in the destination. Default is True.
         name (Optional[str]): The name of the file to save the paper as. If not provided, use the DOI. Default is None.
-        param scihub_on_fail: if SciHub should be used as back up resolver. False by default. For paywalled articles it can be illegal in some of the countries, so use it at your own risk.
+        param scihub_on_fail: if SciHub should be used as back up resolver. False by default.
+            For paywalled articles it can be illegal in some of the countries, so use it at your own risk.
+        logger: Logger class, defaulted to loguru.logger
 
 
     Returns:
         (str, Path): A tuple containing the DOI of the paper and the path to the downloaded paper.
     """
     if logger is None:
         logger = loguru.logger
@@ -282,34 +380,61 @@
 
     paper = _pdf_path_for_doi(doi, destination, name, True)
     meta = paper.parent / paper.name.replace(".pdf", "_meta.json")
 
     # Get a reference to the current event loop
     loop = asyncio.get_event_loop()
 
-    _ = await loop.run_in_executor(executor, lambda: try_download(doi, destination, skip_if_exist, name, scihub_on_fail, logger))
+    _ = await loop.run_in_executor(
+        executor,
+        lambda: try_download(
+            doi,
+            destination,
+            skip_if_exist,
+            name,
+            scihub_on_fail,
+            logger=logger
+        )
+    )
 
     # Return the DOI and path to the downloaded paper
     return PaperDownload(doi, paper, meta)
 
 
-def download_papers(dois: List[str], destination: Path, threads: int, scihub_on_fail: bool = False, logger: Optional["loguru.Logger"] = None) -> (OrderedDict[str, PaperDownload], List[str]):
+def download_papers(
+        dois: List[str],
+        destination: Path,
+        threads: int,
+        scihub_on_fail: bool = False,
+        logger: Optional["loguru.Logger"] = None
+) -> (OrderedDict[str, PaperDownload], List[str]):
     """
     :param dois: List of DOIs of the papers to download
     :param destination: Directory where to put the downloaded papers
     :param threads: Maximum number of concurrent downloads
-    :param scihub_on_fail: if SciHub should be used as back up resolver. False by default. For paywalled articles it can be illegal in some of the countries, so use it at your own risk.
+    :param scihub_on_fail: if SciHub should be used as back up resolver. False by default.
+        For paywalled articles it can be illegal in some of the countries, so use it at your own risk.
+    :param logger: logger class to log stuff, probably compatible with logging.Logger, but use on your own risk.
     :return: tuple with OrderedDict of succeeded results and list of failed dois)
     """
+    if not logger:
+        logger = loguru.logger
     nest_asyncio.apply()
     # Create a ThreadPoolExecutor with desired number of threads
     with ThreadPoolExecutor(max_workers=threads) as executor:
         # Create a coroutine for each download
-        coroutines = [download_async(executor, doi, destination, scihub_on_fail=scihub_on_fail) for doi in dois]
-        #TODO: can be problematic
+        coroutines = [
+            download_async(
+                executor,
+                doi,
+                destination,
+                scihub_on_fail=scihub_on_fail,
+                logger=logger
+            ) for doi in dois]
+        # TODO: can be problematic
         # Get the current event loop, run the downloads, and wait for all of them to finish
         loop = asyncio.get_event_loop()
         results: List[PaperDownload | Exception] = loop.run_until_complete(asyncio.gather(*coroutines, return_exceptions=True))
         (failed, downloaded) = seq(results).partition(lambda r: isinstance(r, Exception))
         for f in failed:
             logger.error(f"FAILED TO DOWNLOAD: {f}")
     partitions: List[List[PaperDownload]] = seq(downloaded).partition(lambda kv: isinstance(kv.pdf, Path)).to_list()
@@ -374,19 +499,21 @@
 
 @app.command("download_pubmed")
 @click.option('--pubmed', type=click.STRING, help="download doi")
 @click.option('--folder', type=click.Path(), default=".", help="where to download the paper")
 @click.option('--skip_existing', type=click.BOOL, default=True, help="if it should skip downloading if the paper exists")
 @click.option('--scihub_on_fail', type=click.BOOL, default=False, help="if schihub should be used as backup resolver. Use it at your own risk and responsibility (false by default)")
 @click.option('--name', type=click.STRING, default=None, help="custom name, uses doi if none and pubmed id if pmid")
-def download_pubmed_command(pubmed: str, folder: str, skip_existing: bool, name: Optional[str], scihub_on_fail: bool = False):
+@click.option('--log_level', type=click.Choice(LOG_LEVELS, case_sensitive=False), default="debug", help="logging level")
+def download_pubmed_command(pubmed: str, folder: str, skip_existing: bool, name: Optional[str], scihub_on_fail: bool = False,  log_level: str = "debug"):
+    logger = configure_logger(log_level, add_stdout = True)
     where = Path(folder)
     where.mkdir(exist_ok=True, parents=True)
     custom_name = pubmed if name == "pmid" or name == "PMID" else name
-    return download_pubmed(pubmed, where, skip_existing, custom_name, scihub_on_fail=scihub_on_fail)
+    return download_pubmed(pubmed, where, skip_existing, custom_name, scihub_on_fail=scihub_on_fail, logger = logger)
 
 
 def get_access(
         sch: SemanticScholar,
         paper_ids: List[str],
         fields: Optional[List[str]] = None
 ) -> List[dict]:
```

### Comparing `getpaper-0.4.9/getpaper/parse.py` & `getpaper-0.5.0/getpaper/parse.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.4.9/getpaper/selenium_download.py` & `getpaper-0.5.0/getpaper/selenium_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import click
 from typing import Optional
 
 
 def download_pdf_selenium(url: str, download_dir: Path, headless: bool=True, min_wait_time: int=8, max_wait_time: int=60, final_path: Optional[Path] = None, logger: Optional["loguru.Logger"] = None) -> Path:
     if logger is None:
         logger = loguru.logger
-    logger.trace(f"selenium parameters url {url}, download_dir {download_dir}, headless {headless}, min_wait_time {min_wait_time}, max wait time {max_wait_time}, final path {final_path}")
+    logger.debug(f"selenium parameters url {url}, download_dir {download_dir}, headless {headless}, min_wait_time {min_wait_time}, max wait time {max_wait_time}, final path {final_path}")
 
     download_dir.mkdir(parents=True, exist_ok=True)
     absolute_download_dir = str(download_dir.resolve())
 
     options = FirefoxOptions()
     if headless:
         options.add_argument("--headless")
```

### Comparing `getpaper-0.4.9/getpaper/test.py` & `getpaper-0.5.0/getpaper/test.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.4.9/getpaper.egg-info/PKG-INFO` & `getpaper-0.5.0/getpaper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.4.9
+Version: 0.5.0
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -45,19 +45,20 @@
 ## Downloading papers
 
 After the installation you can either import the library into your python code or you can use the console scripts.
 
 If you install from pip calling _download_ will mean calling getpaper/download.py , for _parse_ - getpaper/parse.py , for _index_ - getpaper/index.py
 
 ```bash
-download download_pubmed --pubmed 22266545 --folder "data/output/test/papers" --name pmid
+download download_pubmed --pubmed 22266545 --folder "data/output/test/papers" --name pmid --loglevel info  --scihub_on_fail True
 ```
 Downloads the paper with pubmed id into the folder 'papers' and uses the pubmed id as name
+
 ```bash
-download download_doi --doi 10.1038/s41597-020-00710-z --folder "data/output/test/papers"
+download download_doi --doi 10.1038/s41597-020-00710-z --folder "data/output/test/papers" --scihub_on_fail True
 ```
 Downloads the paper with DOI into the folder papers, as --name is not specified doi is used as name
 
 It is also possible to download many papers in parallel with download_papers(dois: List[str], destination: Path, threads: int) function, for example:
 ```python
 from pathlib import Path
 from typing import List
@@ -126,10 +127,11 @@
 ```
 
 Detectron2 is required for using models from the layoutparser model zoo but is not automatically installed with this package. 
 For macOS and Linux, build from source with:
 
 pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
 
-# Note
+# Notes
 
+Sometimes semantic-scholar change their APIs, so if the library stops working for you, open the issue.
 Since 0.3.0 version all indexing features were moved to indexpaper library
```

### Comparing `getpaper-0.4.9/setup.py` & `getpaper-0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.4.9'
+VERSION = '0.5.0'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
@@ -21,21 +21,21 @@
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=[
         'pycomfort>=0.0.15',
         'click',
         'pynction',
-        'langchain>=0.1.9',
-        'langchain_community>=0.0.22',
+        'langchain>=0.2.1',
+        'langchain_community>=0.2.1',
         'scidownl>=1.0.2',
-        'semanticscholar>=0.7.0',
+        'semanticscholar>=0.8.1',
         'Deprecated',
-        'PyMuPDF>=1.23.25',
-        "unpywall>=0.2.2",
+        'PyMuPDF>=1.24.4',
+        "unpywall>=0.2.3",
         "nest_asyncio>=1.6.0",
         "chardet",
         "transformers"
     ],
     extras_require={
         'selenium': ['selenium', 'webdriver-manager'],
         'unstructured': [
```

