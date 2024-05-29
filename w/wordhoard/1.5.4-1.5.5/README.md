# Comparing `tmp/wordhoard-1.5.4.tar.gz` & `tmp/wordhoard-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordhoard-1.5.4.tar", last modified: Thu Jun  1 14:22:53 2023, max compression
+gzip compressed data, was "wordhoard-1.5.5.tar", last modified: Tue May 28 16:08:28 2024, max compression
```

## Comparing `wordhoard-1.5.4.tar` & `wordhoard-1.5.5.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-06-01 14:22:53.567582 wordhoard-1.5.4/
--rw-r--r--   0 bumgarner   (501) staff       (20)     1071 2020-10-20 22:26:04.000000 wordhoard-1.5.4/LICENSE
--rw-r--r--   0 bumgarner   (501) staff       (20)       73 2020-10-23 19:09:16.000000 wordhoard-1.5.4/MANIFEST.in
--rw-r--r--   0 bumgarner   (501) staff       (20)     5282 2023-06-01 14:22:53.567229 wordhoard-1.5.4/PKG-INFO
--rw-r--r--   0 bumgarner   (501) staff       (20)       38 2023-06-01 14:22:53.567684 wordhoard-1.5.4/setup.cfg
--rw-r--r--   0 bumgarner   (501) staff       (20)     2580 2023-06-01 14:21:27.000000 wordhoard-1.5.4/setup.py
-drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-06-01 14:22:53.543229 wordhoard-1.5.4/wordhoard/
--rw-r--r--   0 bumgarner   (501) staff       (20)    10244 2023-06-01 14:09:29.000000 wordhoard-1.5.4/wordhoard/.DS_Store
--rw-r--r--   0 bumgarner   (501) staff       (20)      828 2023-05-31 17:55:08.000000 wordhoard-1.5.4/wordhoard/__init__.py
-drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-06-01 14:22:53.548631 wordhoard-1.5.4/wordhoard/__pycache__/
--rw-r--r--   0 bumgarner   (501) staff       (20)     1106 2023-03-21 14:37:01.000000 wordhoard-1.5.4/wordhoard/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)    13558 2023-03-20 19:33:37.000000 wordhoard-1.5.4/wordhoard/__pycache__/antonyms.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)    18393 2023-03-20 19:33:37.000000 wordhoard-1.5.4/wordhoard/__pycache__/dictionary.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     5301 2023-03-21 14:37:01.000000 wordhoard-1.5.4/wordhoard/__pycache__/homophones.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)    10659 2023-03-20 19:33:37.000000 wordhoard-1.5.4/wordhoard/__pycache__/hypernyms.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)    11292 2023-03-20 19:33:37.000000 wordhoard-1.5.4/wordhoard/__pycache__/hyponyms.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)    21711 2023-03-20 19:33:37.000000 wordhoard-1.5.4/wordhoard/__pycache__/synonyms.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)    19670 2023-05-31 19:42:24.000000 wordhoard-1.5.4/wordhoard/antonyms.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    29507 2023-05-31 19:42:24.000000 wordhoard-1.5.4/wordhoard/dictionary.py
-drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-06-01 14:22:53.550023 wordhoard-1.5.4/wordhoard/files/
--rw-r--r--   0 bumgarner   (501) staff       (20)        1 2020-10-24 00:22:43.000000 wordhoard-1.5.4/wordhoard/files/__init__.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    29162 2021-06-09 14:56:46.000000 wordhoard-1.5.4/wordhoard/files/common_english_homophones.pkl
--rw-r--r--   0 bumgarner   (501) staff       (20)    35141 2021-09-12 12:42:32.000000 wordhoard-1.5.4/wordhoard/files/common_user_agents.pkl
--rw-r--r--   0 bumgarner   (501) staff       (20)   636545 2021-06-10 00:27:56.000000 wordhoard-1.5.4/wordhoard/files/no_homophones_english.pkl
--rw-r--r--   0 bumgarner   (501) staff       (20)     6478 2023-05-31 14:55:32.000000 wordhoard-1.5.4/wordhoard/homophones.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    16773 2023-05-31 18:07:54.000000 wordhoard-1.5.4/wordhoard/hypernyms.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    17057 2023-05-31 18:07:54.000000 wordhoard-1.5.4/wordhoard/hyponyms.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    33769 2023-06-01 13:11:41.000000 wordhoard-1.5.4/wordhoard/synonyms.py
-drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-06-01 14:22:53.554828 wordhoard-1.5.4/wordhoard/utilities/
--rw-r--r--   0 bumgarner   (501) staff       (20)        1 2020-10-24 00:22:43.000000 wordhoard-1.5.4/wordhoard/utilities/__init__.py
-drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-06-01 14:22:53.566415 wordhoard-1.5.4/wordhoard/utilities/__pycache__/
--rw-r--r--   0 bumgarner   (501) staff       (20)      177 2021-06-12 12:23:57.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     3198 2023-03-19 14:46:10.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/caching.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     3143 2022-03-05 18:28:10.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/captcha_checker.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     2122 2023-03-04 14:25:28.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/cleansing.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     2242 2023-02-25 19:31:27.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/cloudflare_bypass.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     3435 2023-03-08 15:41:26.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/cloudflare_checker.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     1024 2023-02-18 18:50:54.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/colorized_text.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     7860 2023-03-02 15:25:13.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/deep_translator.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)      879 2023-02-10 15:52:21.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/email_address_verification.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     2519 2023-03-02 15:16:31.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/exceptions.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     7783 2023-02-12 13:42:58.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/google_translator.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)    11237 2023-02-11 15:17:46.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/mymemory_translator.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     7425 2023-03-18 14:29:02.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/request_html.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     7081 2023-03-02 15:16:31.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/translator_languages.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     3088 2023-03-04 14:25:28.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/user_agents.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     1037 2023-03-04 15:22:37.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/word_verification.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)      812 2023-02-28 16:23:56.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/wordhoard_logger.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     5455 2023-04-14 14:54:35.000000 wordhoard-1.5.4/wordhoard/utilities/caching.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     4169 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/captcha_checker.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     2226 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/cleansing.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     3044 2023-04-10 13:56:10.000000 wordhoard-1.5.4/wordhoard/utilities/cloudflare_bypass.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     4244 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/cloudflare_checker.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     1632 2023-05-29 16:46:14.000000 wordhoard-1.5.4/wordhoard/utilities/colorized_text.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    13901 2023-05-31 14:04:31.000000 wordhoard-1.5.4/wordhoard/utilities/deep_translator.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     1712 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/email_address_verification.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     2507 2023-02-13 14:13:15.000000 wordhoard-1.5.4/wordhoard/utilities/exceptions.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    14793 2023-05-31 14:04:31.000000 wordhoard-1.5.4/wordhoard/utilities/google_translator.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    17428 2023-05-31 14:04:31.000000 wordhoard-1.5.4/wordhoard/utilities/mymemory_translator.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    13501 2023-05-31 14:55:32.000000 wordhoard-1.5.4/wordhoard/utilities/request_html.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    18164 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/translator_languages.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     4297 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/user_agents.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     1873 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/word_verification.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     1623 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/wordhoard_logger.py
-drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-06-01 14:22:53.544772 wordhoard-1.5.4/wordhoard.egg-info/
--rw-r--r--   0 bumgarner   (501) staff       (20)     5282 2023-06-01 14:22:53.000000 wordhoard-1.5.4/wordhoard.egg-info/PKG-INFO
--rw-r--r--   0 bumgarner   (501) staff       (20)     2579 2023-06-01 14:22:53.000000 wordhoard-1.5.4/wordhoard.egg-info/SOURCES.txt
--rw-r--r--   0 bumgarner   (501) staff       (20)        1 2023-06-01 14:22:53.000000 wordhoard-1.5.4/wordhoard.egg-info/dependency_links.txt
--rw-r--r--   0 bumgarner   (501) staff       (20)      258 2023-06-01 14:22:53.000000 wordhoard-1.5.4/wordhoard.egg-info/requires.txt
--rw-r--r--   0 bumgarner   (501) staff       (20)       10 2023-06-01 14:22:53.000000 wordhoard-1.5.4/wordhoard.egg-info/top_level.txt
+drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2024-05-28 16:08:28.396889 wordhoard-1.5.5/
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1071 2020-10-20 22:26:04.000000 wordhoard-1.5.5/LICENSE
+-rw-r--r--   0 bumgarner   (501) staff       (20)       73 2020-10-23 19:09:16.000000 wordhoard-1.5.5/MANIFEST.in
+-rw-r--r--   0 bumgarner   (501) staff       (20)     5580 2024-05-28 16:08:28.396220 wordhoard-1.5.5/PKG-INFO
+-rw-r--r--   0 bumgarner   (501) staff       (20)       38 2024-05-28 16:08:28.397042 wordhoard-1.5.5/setup.cfg
+-rw-r--r--   0 bumgarner   (501) staff       (20)     2386 2024-05-28 12:29:36.000000 wordhoard-1.5.5/setup.py
+drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2024-05-28 16:08:28.361026 wordhoard-1.5.5/wordhoard/
+-rw-r--r--   0 bumgarner   (501) staff       (20)    10244 2024-05-28 15:26:58.000000 wordhoard-1.5.5/wordhoard/.DS_Store
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1256 2024-05-28 12:30:34.000000 wordhoard-1.5.5/wordhoard/__init__.py
+drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2024-05-28 16:08:28.366182 wordhoard-1.5.5/wordhoard/__pycache__/
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1484 2024-05-28 12:34:24.000000 wordhoard-1.5.5/wordhoard/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)    25347 2024-05-28 12:34:24.000000 wordhoard-1.5.5/wordhoard/__pycache__/antonyms.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)    29919 2024-05-28 12:36:40.000000 wordhoard-1.5.5/wordhoard/__pycache__/dictionary.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     5966 2024-05-28 12:36:40.000000 wordhoard-1.5.5/wordhoard/__pycache__/homophones.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)    15754 2024-05-28 12:36:40.000000 wordhoard-1.5.5/wordhoard/__pycache__/hypernyms.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)    15866 2024-05-28 12:36:40.000000 wordhoard-1.5.5/wordhoard/__pycache__/hyponyms.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)    34612 2024-05-28 12:34:24.000000 wordhoard-1.5.5/wordhoard/__pycache__/synonyms.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)    31299 2024-05-25 14:23:57.000000 wordhoard-1.5.5/wordhoard/antonyms.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    38192 2024-05-25 14:23:57.000000 wordhoard-1.5.5/wordhoard/dictionary.py
+drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2024-05-28 16:08:28.368355 wordhoard-1.5.5/wordhoard/files/
+-rw-r--r--   0 bumgarner   (501) staff       (20)        1 2020-10-24 00:22:43.000000 wordhoard-1.5.5/wordhoard/files/__init__.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    29162 2021-06-09 14:56:46.000000 wordhoard-1.5.5/wordhoard/files/common_english_homophones.pkl
+-rw-r--r--   0 bumgarner   (501) staff       (20)    35141 2021-09-12 12:42:32.000000 wordhoard-1.5.5/wordhoard/files/common_user_agents.pkl
+-rw-r--r--   0 bumgarner   (501) staff       (20)   636545 2021-06-10 00:27:56.000000 wordhoard-1.5.5/wordhoard/files/no_homophones_english.pkl
+-rw-r--r--   0 bumgarner   (501) staff       (20)     6871 2024-05-09 16:35:47.000000 wordhoard-1.5.5/wordhoard/homophones.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    19418 2024-05-25 14:23:57.000000 wordhoard-1.5.5/wordhoard/hypernyms.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    18881 2024-05-25 14:23:57.000000 wordhoard-1.5.5/wordhoard/hyponyms.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    44299 2024-05-25 14:23:57.000000 wordhoard-1.5.5/wordhoard/synonyms.py
+drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2024-05-28 16:08:28.382822 wordhoard-1.5.5/wordhoard/utilities/
+-rw-r--r--   0 bumgarner   (501) staff       (20)        1 2020-10-24 00:22:43.000000 wordhoard-1.5.5/wordhoard/utilities/__init__.py
+drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2024-05-28 16:08:28.394676 wordhoard-1.5.5/wordhoard/utilities/__pycache__/
+-rw-r--r--   0 bumgarner   (501) staff       (20)      177 2021-06-12 12:23:57.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     6670 2024-05-28 15:28:11.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/caching.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     3143 2022-03-05 18:28:10.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/captcha_checker.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     2121 2024-05-28 12:34:24.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/cleansing.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     2564 2024-05-28 12:34:24.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/cloudflare_bypass.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     3547 2024-05-28 12:34:24.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/cloudflare_checker.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)      985 2024-05-28 12:34:24.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/colorized_text.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     7860 2023-03-02 15:25:13.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/deep_translator.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)      879 2023-02-10 15:52:21.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/email_address_verification.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     2519 2023-03-02 15:16:31.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/exceptions.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     7783 2023-02-12 13:42:58.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/google_translator.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)    11237 2023-02-11 15:17:46.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/mymemory_translator.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     9486 2024-05-28 12:34:24.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/request_html.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     7081 2023-03-02 15:16:31.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/translator_languages.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     3785 2024-05-28 12:34:24.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/user_agents.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1053 2024-05-28 12:34:24.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/word_verification.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1167 2024-05-28 12:36:40.000000 wordhoard-1.5.5/wordhoard/utilities/__pycache__/wordhoard_logger.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)    10009 2024-05-28 15:26:25.000000 wordhoard-1.5.5/wordhoard/utilities/caching.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     4061 2024-05-12 10:31:58.000000 wordhoard-1.5.5/wordhoard/utilities/captcha_checker.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     2225 2024-05-11 15:12:18.000000 wordhoard-1.5.5/wordhoard/utilities/cleansing.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     3907 2024-05-04 14:14:24.000000 wordhoard-1.5.5/wordhoard/utilities/cloudflare_bypass.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     4181 2024-05-25 15:32:58.000000 wordhoard-1.5.5/wordhoard/utilities/cloudflare_checker.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1630 2024-05-11 15:11:47.000000 wordhoard-1.5.5/wordhoard/utilities/colorized_text.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    14669 2024-05-26 14:34:06.000000 wordhoard-1.5.5/wordhoard/utilities/deep_translator.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1681 2024-05-12 11:02:29.000000 wordhoard-1.5.5/wordhoard/utilities/email_address_verification.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     2438 2024-05-13 13:20:27.000000 wordhoard-1.5.5/wordhoard/utilities/exceptions.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    16870 2024-05-25 15:11:37.000000 wordhoard-1.5.5/wordhoard/utilities/google_translator.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    18469 2024-05-25 15:11:37.000000 wordhoard-1.5.5/wordhoard/utilities/mymemory_translator.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    15767 2024-05-27 15:42:20.000000 wordhoard-1.5.5/wordhoard/utilities/request_html.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    18634 2024-05-12 11:06:41.000000 wordhoard-1.5.5/wordhoard/utilities/translator_languages.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     4963 2024-05-12 10:57:53.000000 wordhoard-1.5.5/wordhoard/utilities/user_agents.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1834 2024-05-11 15:11:09.000000 wordhoard-1.5.5/wordhoard/utilities/word_verification.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1973 2024-05-13 13:08:10.000000 wordhoard-1.5.5/wordhoard/utilities/wordhoard_logger.py
+drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2024-05-28 16:08:28.395298 wordhoard-1.5.5/wordhoard.egg-info/
+-rw-r--r--   0 bumgarner   (501) staff       (20)     5580 2024-05-28 16:08:28.000000 wordhoard-1.5.5/wordhoard.egg-info/PKG-INFO
+-rw-r--r--   0 bumgarner   (501) staff       (20)     2579 2024-05-28 16:08:28.000000 wordhoard-1.5.5/wordhoard.egg-info/SOURCES.txt
+-rw-r--r--   0 bumgarner   (501) staff       (20)        1 2024-05-28 16:08:28.000000 wordhoard-1.5.5/wordhoard.egg-info/dependency_links.txt
+-rw-r--r--   0 bumgarner   (501) staff       (20)      254 2024-05-28 16:08:28.000000 wordhoard-1.5.5/wordhoard.egg-info/requires.txt
+-rw-r--r--   0 bumgarner   (501) staff       (20)       10 2024-05-28 16:08:28.000000 wordhoard-1.5.5/wordhoard.egg-info/top_level.txt
```

### Comparing `wordhoard-1.5.4/LICENSE` & `wordhoard-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.4/PKG-INFO` & `wordhoard-1.5.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 Metadata-Version: 2.1
 Name: wordhoard
-Version: 1.5.4
+Version: 1.5.5
 Summary: A comprehensive lexical discovery application that is useful for finding semantic relationships such as, the antonyms, synonyms, hypernyms, hyponyms, homophones and definitions for a specific word.
 Home-page: https://github.com/johnbumgarner/wordhoard
 Author: John Bumgarner
 Author-email: wordhoardproject@gmail.com
 License: LICENSE.txt
 Keywords: antonyms,bag of words,definitions,hypernyms,hyponyms,homophones,information retrieval,lexicon,semantic relationships,synonyms,natural language processing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Processing :: General
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: backoff>=2.2.1
+Requires-Dist: beautifulsoup4>=4.12.3
+Requires-Dist: certifi>=2024.2.2
+Requires-Dist: charset-normalizer>=3.3.2
+Requires-Dist: cloudscraper>=1.2.71
+Requires-Dist: deckar01-ratelimit>=3.0.2
+Requires-Dist: deepl>=1.18.0
+Requires-Dist: idna>=3.7
+Requires-Dist: lxml>=5.2.2
+Requires-Dist: pyparsing>=3.1.2
+Requires-Dist: requests>=2.32.2
+Requires-Dist: requests-toolbelt>=1.0.0
+Requires-Dist: soupsieve>=2.5
+Requires-Dist: urllib3>=2.2.1
 
 # Primary Use Case
 <p align="justify"> 
 Textual analysis is a broad term for various research methodologies used to qualitatively describe, interpret and understand text data. These methodologies are mainly used in academic research to analyze content related to media and communication studies, popular culture, sociology, and philosophy. Textual analysis allows these researchers to quickly obtain relevant insights from unstructured data. All types of information can be gleaned from textual data, especially from social media posts or news articles. Some of this information includes the overall concept of the subtext, symbolism within the text, assumptions being made and potential relative value to a subject (e.g. data science). In some cases it is possible to deduce the relative historical and cultural context of a body of text using analysis techniques coupled with knowledge from different disciplines, like linguistics and semiotics.
    
 Word frequency is the technique used in textual analysis to measure the frequency of a specific word or word grouping within unstructured data. Measuring the number of word occurrences in a corpus allows a researcher to garner interesting insights about the text. A subset of word frequency is the correlation between a given word and that word's relationship to either antonyms and synonyms within the specific corpus being analyzed. Knowing these relationships is critical to improving word frequencies and topic modeling.
 
@@ -113,9 +124,9 @@
 The MIT License (MIT).  Please see <a href="https://wordhoard.readthedocs.io/en/latest/license" target="_blank">License File</a> for more information.
 </p>
 
 
 # Author
 
 <p align="justify">
-   Copyright (c) 2020 John Bumgarner 
+   Copyright (c) 2021 John Bumgarner 
 </p>
```

#### html2text {}

```diff
@@ -1,26 +1,30 @@
-Metadata-Version: 2.1 Name: wordhoard Version: 1.5.4 Summary: A comprehensive
+Metadata-Version: 2.1 Name: wordhoard Version: 1.5.5 Summary: A comprehensive
 lexical discovery application that is useful for finding semantic relationships
 such as, the antonyms, synonyms, hypernyms, hyponyms, homophones and
 definitions for a specific word. Home-page: https://github.com/johnbumgarner/
 wordhoard Author: John Bumgarner Author-email: wordhoardproject@gmail.com
 License: LICENSE.txt Keywords: antonyms,bag of
 words,definitions,hypernyms,hyponyms,homophones,information
 retrieval,lexicon,semantic relationships,synonyms,natural language processing
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Topic :: Text Processing
-:: General Classifier: Topic :: Text Processing :: Linguistic Classifier: Topic
-:: Utilities Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE # Primary Use Case
+Independent Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Text Processing :: Linguistic Classifier: Topic ::
+Utilities Requires-Python: >=3.8 Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: backoff>=2.2.1 Requires-Dist:
+beautifulsoup4>=4.12.3 Requires-Dist: certifi>=2024.2.2 Requires-Dist: charset-
+normalizer>=3.3.2 Requires-Dist: cloudscraper>=1.2.71 Requires-Dist: deckar01-
+ratelimit>=3.0.2 Requires-Dist: deepl>=1.18.0 Requires-Dist: idna>=3.7
+Requires-Dist: lxml>=5.2.2 Requires-Dist: pyparsing>=3.1.2 Requires-Dist:
+requests>=2.32.2 Requires-Dist: requests-toolbelt>=1.0.0 Requires-Dist:
+soupsieve>=2.5 Requires-Dist: urllib3>=2.2.1 # Primary Use Case
 Textual analysis is a broad term for various research methodologies used to
 qualitatively describe, interpret and understand text data. These methodologies
 are mainly used in academic research to analyze content related to media and
 communication studies, popular culture, sociology, and philosophy. Textual
 analysis allows these researchers to quickly obtain relevant insights from
 unstructured data. All types of information can be gleaned from textual data,
 especially from social media posts or news articles. Some of this information
@@ -64,8 +68,8 @@
 [GitHub]%20wordhoard%20project%20request) with any issues or enhancement
 requests.
 # Sponsorship If you would like to contribute financially to the development
 and maintenance of the WWoorrddhhooaarrdd project please read the _s_p_o_n_s_o_r_s_h_i_p
 _i_n_f_o_r_m_a_t_i_o_n. # License
 The MIT License (MIT). Please see _L_i_c_e_n_s_e_ _F_i_l_e for more information.
 # Author
-Copyright (c) 2020 John Bumgarner
+Copyright (c) 2021 John Bumgarner
```

### Comparing `wordhoard-1.5.4/setup.py` & `wordhoard-1.5.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import setuptools
 
-
 with open("PYPI_description.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wordhoard",
-    version="1.5.4",
+    version="1.5.5",
     author="John Bumgarner",
     author_email="wordhoardproject@gmail.com",
     description="A comprehensive lexical discovery application that is useful for finding semantic relationships "
                 "such as, the antonyms, synonyms, hypernyms, hyponyms, homophones and definitions for a specific word.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/johnbumgarner/wordhoard",
@@ -21,35 +20,32 @@
                             'files/no_homophones_english.pkl']},
     license='LICENSE.txt',
     classifiers=["Development Status :: 5 - Production/Stable",
                  "Intended Audience :: Developers",
                  "License :: OSI Approved :: MIT License",
                  "Natural Language :: English",
                  "Operating System :: OS Independent",
-                 "Programming Language :: Python :: 3.6",
-                 "Programming Language :: Python :: 3.7",
                  "Programming Language :: Python :: 3.8",
                  "Programming Language :: Python :: 3.9",
                  "Programming Language :: Python :: 3.10",
-                 "Topic :: Software Development :: Libraries :: Python Modules",
-                 "Topic :: Text Processing :: General",
+                 "Topic :: Software Development :: Libraries",
                  "Topic :: Text Processing :: Linguistic",
                  "Topic :: Utilities"],
-   keywords=['antonyms', 'bag of words', 'definitions', 'hypernyms', 'hyponyms', 'homophones',
+    keywords=['antonyms', 'bag of words', 'definitions', 'hypernyms', 'hyponyms', 'homophones',
               'information retrieval', 'lexicon', 'semantic relationships', 'synonyms',
               'natural language processing'],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     install_requires=['backoff>=2.2.1',
-                      'beautifulsoup4>=4.11.2',
-                      'certifi>=2022.12.7',
-                      'charset-normalizer>=3.1.0',
-                      'cloudscraper>=1.2.69',
+                      'beautifulsoup4>=4.12.3',
+                      'certifi>=2024.2.2',
+                      'charset-normalizer>=3.3.2',
+                      'cloudscraper>=1.2.71',
                       'deckar01-ratelimit>=3.0.2',
-                      'deepl>=1.14.0',
-                      'idna>=3.4',
-                      'lxml>=4.9.2',
-                      'pyparsing>=3.0.9',
-                      'requests>=2.28.2',
-                      'requests-toolbelt>=0.10.1',
-                      'soupsieve>=2.4',
-                      'urllib3>=1.26.15']
+                      'deepl>=1.18.0',
+                      'idna>=3.7',
+                      'lxml>=5.2.2',
+                      'pyparsing>=3.1.2',
+                      'requests>=2.32.2',
+                      'requests-toolbelt>=1.0.0',
+                      'soupsieve>=2.5',
+                      'urllib3>=2.2.1']
 )
```

### Comparing `wordhoard-1.5.4/wordhoard/.DS_Store` & `wordhoard-1.5.5/wordhoard/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -271,126 +271,126 @@
 000010e0: 0069 006c 0065 0073 6d6f 4444 626c 6f62  .i.l.e.smoDDblob
 000010f0: 0000 0008 2cfd d9ad 1677 c341 0000 0005  ....,....w.A....
 00001100: 0066 0069 006c 0065 0073 6d6f 6444 626c  .f.i.l.e.smodDbl
 00001110: 6f62 0000 0008 2cfd d9ad 1677 c341 0000  ob....,....w.A..
 00001120: 0005 0066 0069 006c 0065 0073 7068 3153  ...f.i.l.e.sph1S
 00001130: 636f 6d70 0000 0000 000a e000 0000 0009  comp............
 00001140: 0075 0074 0069 006c 0069 0074 0069 0065  .u.t.i.l.i.t.i.e
-00001150: 0073 6277 7370 626c 6f62 0000 00cc 6270  .sbwspblob....bp
-00001160: 6c69 7374 3030 d701 0203 0405 0607 0809  list00..........
-00001170: 0908 090d 095d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00001180: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
-00001190: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-000011a0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-000011b0: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-000011c0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-000011d0: 5369 6465 6261 7208 0909 0809 5f10 1b7b  Sidebar....._..{
-000011e0: 7b2d 3235 3030 2c20 3334 377d 2c20 7b31  {-2500, 347}, {1
-000011f0: 3430 322c 2037 3531 7d7d 0908 1725 313d  402, 751}}...%1=
-00001200: 4960 6d79 7a7b 7c7d 7e9c 0000 0000 0000  I`myz{|}~.......
-00001210: 0101 0000 0000 0000 000f 0000 0000 0000  ................
-00001220: 0000 0000 0000 0000 009d 0000 0009 0075  ...............u
-00001230: 0074 0069 006c 0069 0074 0069 0065 0073  .t.i.l.i.t.i.e.s
-00001240: 6473 636c 626f 6f6c 0000 0000 0900 7500  dsclbool......u.
-00001250: 7400 6900 6c00 6900 7400 6900 6500 736c  t.i.l.i.t.i.e.sl
-00001260: 6731 5363 6f6d 7000 0000 0000 02b6 2800  g1Scomp.......(.
-00001270: 0000 0900 7500 7400 6900 6c00 6900 7400  ....u.t.i.l.i.t.
-00001280: 6900 6500 736c 7376 4362 6c6f 6200 0002  i.e.slsvCblob...
-00001290: 9762 706c 6973 7430 30d8 0102 0304 0506  .bplist00.......
-000012a0: 0708 090a 0b19 494a 0a4c 5f10 1276 6965  ......IJ.L_..vie
-000012b0: 774f 7074 696f 6e73 5665 7273 696f 6e5f  wOptionsVersion_
-000012c0: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
-000012d0: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
-000012e0: 756c 6174 6541 6c6c 5369 7a65 7358 7465  ulateAllSizesXte
-000012f0: 7874 5369 7a65 5a73 6f72 7443 6f6c 756d  xtSizeZsortColum
-00001300: 6e5f 1010 7573 6552 656c 6174 6976 6544  n_..useRelativeD
-00001310: 6174 6573 5869 636f 6e53 697a 6510 0109  atesXiconSize...
-00001320: ab0c 151d 2226 2b30 353a 3f44 d40d 0e0f  ...."&+05:?D....
-00001330: 100a 0a13 1457 7669 7369 626c 6559 6173  .....WvisibleYas
-00001340: 6365 6e64 696e 6755 7769 6474 685a 6964  cendingUwidthZid
-00001350: 656e 7469 6669 6572 0909 1102 2b54 6e61  entifier....+Tna
-00001360: 6d65 d416 1718 1019 1a19 1c57 7669 7369  me.........Wvisi
-00001370: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
-00001380: 696e 6708 1023 0858 7562 6971 7569 7479  ing..#.Xubiquity
-00001390: d40d 0e0f 100a 1920 2109 0810 b55c 6461  ....... !....\da
-000013a0: 7465 4d6f 6469 6669 6564 d40d 0e0f 1019  teModified......
-000013b0: 1920 2508 085b 6461 7465 4372 6561 7465  . %..[dateCreate
-000013c0: 64d4 0d0e 0f10 0a19 292a 0908 1061 5473  d.......)*...aTs
-000013d0: 697a 65d4 0d0e 0f10 0a0a 2e2f 0909 1073  ize......../...s
-000013e0: 546b 696e 64d4 0d0e 0f10 190a 3334 0809  Tkind.......34..
-000013f0: 1064 556c 6162 656c d40d 0e0f 1019 0a38  .dUlabel.......8
-00001400: 3908 0910 4b57 7665 7273 696f 6ed4 0d0e  9...KWversion...
-00001410: 0f10 190a 3d3e 0809 1101 2c58 636f 6d6d  ....=>....,Xcomm
-00001420: 656e 7473 d40d 0e0f 1019 1942 4308 0810  ents.......BC...
-00001430: c85e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
-00001440: d416 1718 1019 2019 4708 0859 6461 7465  ...... .G..Ydate
-00001450: 4164 6465 6408 2340 2800 0000 0000 0054  Added.#@(......T
-00001460: 6e61 6d65 0923 4030 0000 0000 0000 0008  name.#@0........
-00001470: 0019 002e 0040 0048 005c 0065 0070 0083  .....@.H.\.e.p..
-00001480: 008c 008e 008f 009b 00a4 00ac 00b6 00bc  ................
-00001490: 00c7 00c8 00c9 00cc 00d1 00da 00e2 00e8  ................
-000014a0: 00f2 00f3 00f5 00f6 00ff 0108 0109 010a  ................
-000014b0: 010c 0119 0122 0123 0124 0130 0139 013a  .....".#.$.0.9.:
-000014c0: 013b 013d 0142 014b 014c 014d 014f 0154  .;.=.B.K.L.M.O.T
-000014d0: 015d 015e 015f 0161 0167 0170 0171 0172  .].^._.a.g.p.q.r
-000014e0: 0174 017c 0185 0186 0187 018a 0193 019c  .t.|............
-000014f0: 019d 019e 01a0 01af 01b8 01b9 01ba 01c4  ................
-00001500: 01c5 01ce 01d3 01d4 0000 0000 0000 0201  ................
-00001510: 0000 0000 0000 004d 0000 0000 0000 0000  .......M........
-00001520: 0000 0000 0000 01dd 0000 0009 0075 0074  .............u.t
-00001530: 0069 006c 0069 0074 0069 0065 0073 6c73  .i.l.i.t.i.e.sls
-00001540: 7670 626c 6f62 0000 025e 6270 6c69 7374  vpblob...^bplist
-00001550: 3030 d801 0203 0405 0607 0809 0a0b 1d45  00.............E
-00001560: 460a 485f 1012 7669 6577 4f70 7469 6f6e  F.H_..viewOption
-00001570: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-00001580: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00001590: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-000015a0: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
-000015b0: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
-000015c0: 5265 6c61 7469 7665 4461 7465 7358 6963  RelativeDatesXic
-000015d0: 6f6e 5369 7a65 1001 09d9 0c0d 0e0f 1011  onSize..........
-000015e0: 1213 1415 1e23 282d 3237 3c41 5863 6f6d  .....#(-27<AXcom
-000015f0: 6d65 6e74 735e 6461 7465 4c61 7374 4f70  ments^dateLastOp
-00001600: 656e 6564 5b64 6174 6543 7265 6174 6564  ened[dateCreated
-00001610: 5473 697a 6555 6c61 6265 6c54 6b69 6e64  TsizeUlabelTkind
-00001620: 5776 6572 7369 6f6e 546e 616d 655c 6461  WversionTname\da
-00001630: 7465 4d6f 6469 6669 6564 d416 1718 191a  teModified......
-00001640: 0a1c 1d55 696e 6465 7859 6173 6365 6e64  ...UindexYascend
-00001650: 696e 6755 7769 6474 6857 7669 7369 626c  ingUwidthWvisibl
-00001660: 6510 0709 1101 2c08 d416 1718 191f 1d21  e.....,........!
-00001670: 1d10 0808 10c8 08d4 1617 1819 241d 261d  ............$.&.
-00001680: 1002 0810 b508 d416 1718 1929 1d2b 0a10  ...........).+..
-00001690: 0308 1061 09d4 1617 1819 2e0a 301d 1005  ...a........0...
-000016a0: 0910 6408 d416 1718 1933 0a35 0a10 0409  ..d......3.5....
-000016b0: 1073 09d4 1617 1819 380a 3a1d 1006 0910  .s......8.:.....
-000016c0: 4b08 d416 1718 193d 0a3f 0a10 0009 1102  K......=.?......
-000016d0: 2b09 d416 1718 1909 1d26 0a08 0908 2340  +........&....#@
-000016e0: 2800 0000 0000 0054 6e61 6d65 0923 4030  (......Tname.#@0
-000016f0: 0000 0000 0000 0008 0019 002e 0040 0048  .............@.H
-00001700: 005c 0065 0070 0083 008c 008e 008f 00a2  .\.e.p..........
-00001710: 00ab 00ba 00c6 00cb 00d1 00d6 00de 00e3  ................
-00001720: 00f0 00f9 00ff 0109 010f 0117 0119 011a  ................
-00001730: 011d 011e 0127 0129 012a 012c 012d 0136  .....'.).*.,.-.6
-00001740: 0138 0139 013b 013c 0145 0147 0148 014a  .8.9.;.<.E.G.H.J
-00001750: 014b 0154 0156 0157 0159 015a 0163 0165  .K.T.V.W.Y.Z.c.e
-00001760: 0166 0168 0169 0172 0174 0175 0177 0178  .f.h.i.r.t.u.w.x
-00001770: 0181 0183 0184 0187 0188 0191 0192 0193  ................
-00001780: 0194 019d 01a2 01a3 0000 0000 0000 0201  ................
-00001790: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
-000017a0: 0000 0000 0000 01ac 0000 0009 0075 0074  .............u.t
-000017b0: 0069 006c 0069 0074 0069 0065 0073 6d6f  .i.l.i.t.i.e.smo
-000017c0: 4444 626c 6f62 0000 0008 38fe e678 02e5  DDblob....8..x..
-000017d0: c441 0000 0009 0075 0074 0069 006c 0069  .A.....u.t.i.l.i
-000017e0: 0074 0069 0065 0073 6d6f 6444 626c 6f62  .t.i.e.smodDblob
-000017f0: 0000 0008 38fe e678 02e5 c441 0000 0009  ....8..x...A....
-00001800: 0075 0074 0069 006c 0069 0074 0069 0065  .u.t.i.l.i.t.i.e
-00001810: 0073 7068 3153 636f 6d70 0000 0000 0003  .sph1Scomp......
-00001820: d000 0000 0009 0075 0074 0069 006c 0069  .......u.t.i.l.i
-00001830: 0074 0069 0065 0073 7653 726e 6c6f 6e67  .t.i.e.svSrnlong
-00001840: 0000 0001 0000 0000 0000 0000 0000 0000  ................
+00001150: 0073 6277 7370 626c 6f62 0000 00bb 6270  .sbwspblob....bp
+00001160: 6c69 7374 3030 d601 0203 0405 0607 0807  list00..........
+00001170: 080b 085d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
+00001180: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+00001190: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+000011a0: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+000011b0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+000011c0: 6f77 5369 6465 6261 7208 0908 095f 101b  owSidebar...._..
+000011d0: 7b7b 2d32 3533 362c 2033 3537 7d2c 207b  {{-2536, 357}, {
+000011e0: 3131 3538 2c20 3634 377d 7d09 0815 232f  1158, 647}}...#/
+000011f0: 3b52 5f6b 6c6d 6e6f 8d00 0000 0000 0001  ;R_klmno........
+00001200: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
+00001210: 0000 0000 0000 0000 8e00 0000 0900 7500  ..............u.
+00001220: 7400 6900 6c00 6900 7400 6900 6500 7364  t.i.l.i.t.i.e.sd
+00001230: 7363 6c62 6f6f 6c01 0000 0009 0075 0074  sclbool......u.t
+00001240: 0069 006c 0069 0074 0069 0065 0073 6c67  .i.l.i.t.i.e.slg
+00001250: 3153 636f 6d70 0000 0000 0002 b628 0000  1Scomp.......(..
+00001260: 0009 0075 0074 0069 006c 0069 0074 0069  ...u.t.i.l.i.t.i
+00001270: 0065 0073 6c73 7643 626c 6f62 0000 0297  .e.slsvCblob....
+00001280: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
+00001290: 0809 0a0b 1949 4a0a 4c5f 1012 7669 6577  .....IJ.L_..view
+000012a0: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
+000012b0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+000012c0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+000012d0: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
+000012e0: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
+000012f0: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00001300: 7465 7358 6963 6f6e 5369 7a65 1001 09ab  tesXiconSize....
+00001310: 0c15 1d22 262b 3035 3a3f 44d4 0d0e 0f10  ..."&+05:?D.....
+00001320: 0a0a 1314 5776 6973 6962 6c65 5961 7363  ....WvisibleYasc
+00001330: 656e 6469 6e67 5577 6964 7468 5a69 6465  endingUwidthZide
+00001340: 6e74 6966 6965 7209 0911 022b 546e 616d  ntifier....+Tnam
+00001350: 65d4 1617 1810 191a 191c 5776 6973 6962  e.........Wvisib
+00001360: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
+00001370: 6e67 0810 2308 5875 6269 7175 6974 79d4  ng..#.Xubiquity.
+00001380: 0d0e 0f10 0a19 2021 0908 10b5 5c64 6174  ...... !....\dat
+00001390: 654d 6f64 6966 6965 64d4 0d0e 0f10 1919  eModified.......
+000013a0: 2025 0808 5b64 6174 6543 7265 6174 6564   %..[dateCreated
+000013b0: d40d 0e0f 100a 1929 2a09 0810 6154 7369  .......)*...aTsi
+000013c0: 7a65 d40d 0e0f 100a 0a2e 2f09 0910 7354  ze......../...sT
+000013d0: 6b69 6e64 d40d 0e0f 1019 0a33 3408 0910  kind.......34...
+000013e0: 6455 6c61 6265 6cd4 0d0e 0f10 190a 3839  dUlabel.......89
+000013f0: 0809 104b 5776 6572 7369 6f6e d40d 0e0f  ...KWversion....
+00001400: 1019 0a3d 3e08 0911 012c 5863 6f6d 6d65  ...=>....,Xcomme
+00001410: 6e74 73d4 0d0e 0f10 1919 4243 0808 10c8  nts.......BC....
+00001420: 5e64 6174 654c 6173 744f 7065 6e65 64d4  ^dateLastOpened.
+00001430: 1617 1810 1920 1947 0808 5964 6174 6541  ..... .G..YdateA
+00001440: 6464 6564 0823 4028 0000 0000 0000 546e  dded.#@(......Tn
+00001450: 616d 6509 2340 3000 0000 0000 0000 0800  ame.#@0.........
+00001460: 1900 2e00 4000 4800 5c00 6500 7000 8300  ....@.H.\.e.p...
+00001470: 8c00 8e00 8f00 9b00 a400 ac00 b600 bc00  ................
+00001480: c700 c800 c900 cc00 d100 da00 e200 e800  ................
+00001490: f200 f300 f500 f600 ff01 0801 0901 0a01  ................
+000014a0: 0c01 1901 2201 2301 2401 3001 3901 3a01  ....".#.$.0.9.:.
+000014b0: 3b01 3d01 4201 4b01 4c01 4d01 4f01 5401  ;.=.B.K.L.M.O.T.
+000014c0: 5d01 5e01 5f01 6101 6701 7001 7101 7201  ].^._.a.g.p.q.r.
+000014d0: 7401 7c01 8501 8601 8701 8a01 9301 9c01  t.|.............
+000014e0: 9d01 9e01 a001 af01 b801 b901 ba01 c401  ................
+000014f0: c501 ce01 d301 d400 0000 0000 0002 0100  ................
+00001500: 0000 0000 0000 4d00 0000 0000 0000 0000  ......M.........
+00001510: 0000 0000 0001 dd00 0000 0900 7500 7400  ............u.t.
+00001520: 6900 6c00 6900 7400 6900 6500 736c 7376  i.l.i.t.i.e.slsv
+00001530: 7062 6c6f 6200 0002 5e62 706c 6973 7430  pblob...^bplist0
+00001540: 30d8 0102 0304 0506 0708 090a 0b1d 4546  0.............EF
+00001550: 0a48 5f10 1276 6965 774f 7074 696f 6e73  .H_..viewOptions
+00001560: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
+00001570: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
+00001580: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
+00001590: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
+000015a0: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
+000015b0: 656c 6174 6976 6544 6174 6573 5869 636f  elativeDatesXico
+000015c0: 6e53 697a 6510 0109 d90c 0d0e 0f10 1112  nSize...........
+000015d0: 1314 151e 2328 2d32 373c 4158 636f 6d6d  ....#(-27<AXcomm
+000015e0: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
+000015f0: 6e65 645b 6461 7465 4372 6561 7465 6454  ned[dateCreatedT
+00001600: 7369 7a65 556c 6162 656c 546b 696e 6457  sizeUlabelTkindW
+00001610: 7665 7273 696f 6e54 6e61 6d65 5c64 6174  versionTname\dat
+00001620: 654d 6f64 6966 6965 64d4 1617 1819 1a0a  eModified.......
+00001630: 1c1d 5569 6e64 6578 5961 7363 656e 6469  ..UindexYascendi
+00001640: 6e67 5577 6964 7468 5776 6973 6962 6c65  ngUwidthWvisible
+00001650: 1007 0911 012c 08d4 1617 1819 1f1d 211d  .....,........!.
+00001660: 1008 0810 c808 d416 1718 1924 1d26 1d10  ...........$.&..
+00001670: 0208 10b5 08d4 1617 1819 291d 2b0a 1003  ..........).+...
+00001680: 0810 6109 d416 1718 192e 0a30 1d10 0509  ..a........0....
+00001690: 1064 08d4 1617 1819 330a 350a 1004 0910  .d......3.5.....
+000016a0: 7309 d416 1718 1938 0a3a 1d10 0609 104b  s......8.:.....K
+000016b0: 08d4 1617 1819 3d0a 3f0a 1000 0911 022b  ......=.?......+
+000016c0: 09d4 1617 1819 091d 260a 0809 0823 4028  ........&....#@(
+000016d0: 0000 0000 0000 546e 616d 6509 2340 3000  ......Tname.#@0.
+000016e0: 0000 0000 0000 0800 1900 2e00 4000 4800  ............@.H.
+000016f0: 5c00 6500 7000 8300 8c00 8e00 8f00 a200  \.e.p...........
+00001700: ab00 ba00 c600 cb00 d100 d600 de00 e300  ................
+00001710: f000 f900 ff01 0901 0f01 1701 1901 1a01  ................
+00001720: 1d01 1e01 2701 2901 2a01 2c01 2d01 3601  ....'.).*.,.-.6.
+00001730: 3801 3901 3b01 3c01 4501 4701 4801 4a01  8.9.;.<.E.G.H.J.
+00001740: 4b01 5401 5601 5701 5901 5a01 6301 6501  K.T.V.W.Y.Z.c.e.
+00001750: 6601 6801 6901 7201 7401 7501 7701 7801  f.h.i.r.t.u.w.x.
+00001760: 8101 8301 8401 8701 8801 9101 9201 9301  ................
+00001770: 9401 9d01 a201 a300 0000 0000 0002 0100  ................
+00001780: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
+00001790: 0000 0000 0001 ac00 0000 0900 7500 7400  ............u.t.
+000017a0: 6900 6c00 6900 7400 6900 6500 736d 6f44  i.l.i.t.i.e.smoD
+000017b0: 4462 6c6f 6200 0000 0838 fee6 7802 e5c4  Dblob....8..x...
+000017c0: 4100 0000 0900 7500 7400 6900 6c00 6900  A.....u.t.i.l.i.
+000017d0: 7400 6900 6500 736d 6f64 4462 6c6f 6200  t.i.e.smodDblob.
+000017e0: 0000 0838 fee6 7802 e5c4 4100 0000 0900  ...8..x...A.....
+000017f0: 7500 7400 6900 6c00 6900 7400 6900 6500  u.t.i.l.i.t.i.e.
+00001800: 7370 6831 5363 6f6d 7000 0000 0000 03d0  sph1Scomp.......
+00001810: 0000 0000 0900 7500 7400 6900 6c00 6900  ......u.t.i.l.i.
+00001820: 7400 6900 6500 7376 5372 6e6c 6f6e 6700  t.i.e.svSrnlong.
+00001830: 0000 0100 0000 0000 0000 0000 0000 0000  ................
+00001840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000018a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000018b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -586,56 +586,56 @@
 00002490: 0100 0200 0000 0000 0100 0400 0000 0000  ................
 000024a0: 0100 0800 0000 0000 0100 1000 0000 0000  ................
 000024b0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
 000024c0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
 000024d0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
 000024e0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
 000024f0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00002500: 00c5 01ce 01d3 01d4 0000 0000 0000 0201  ................
-00002510: 0000 0000 0000 004d 0000 0000 0000 0000  .......M........
-00002520: 0000 0000 0000 01dd 0000 0009 0075 0074  .............u.t
-00002530: 0069 006c 0069 0074 0069 0065 0073 6c73  .i.l.i.t.i.e.sls
-00002540: 7670 626c 6f62 0000 025e 6270 6c69 7374  vpblob...^bplist
-00002550: 3030 d801 0203 0405 0607 0809 0a0b 1d45  00.............E
-00002560: 460a 485f 1012 7669 6577 4f70 7469 6f6e  F.H_..viewOption
-00002570: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-00002580: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00002590: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-000025a0: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
-000025b0: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
-000025c0: 5265 6c61 7469 7665 4461 7465 7358 6963  RelativeDatesXic
-000025d0: 6f6e 5369 7a65 1001 09d9 0c0d 0e0f 1011  onSize..........
-000025e0: 1213 1415 1e23 282d 3237 3c41 5863 6f6d  .....#(-27<AXcom
-000025f0: 6d65 6e74 735e 6461 7465 4c61 7374 4f70  ments^dateLastOp
-00002600: 656e 6564 5b64 6174 6543 7265 6174 6564  ened[dateCreated
-00002610: 5473 697a 6555 6c61 6265 6c54 6b69 6e64  TsizeUlabelTkind
-00002620: 5776 6572 7369 6f6e 546e 616d 655c 6461  WversionTname\da
-00002630: 7465 4d6f 6469 6669 6564 d416 1718 191a  teModified......
-00002640: 0a1c 1d55 696e 6465 7859 6173 6365 6e64  ...UindexYascend
-00002650: 696e 6755 7769 6474 6857 7669 7369 626c  ingUwidthWvisibl
-00002660: 6510 0709 1101 2c08 d416 1718 191f 1d21  e.....,........!
-00002670: 1d10 0808 10c8 08d4 1617 1819 241d 261d  ............$.&.
-00002680: 1002 0810 b508 d416 1718 1929 1d2b 0a10  ...........).+..
-00002690: 0308 1061 09d4 1617 1819 2e0a 301d 1005  ...a........0...
-000026a0: 0910 6408 d416 1718 1933 0a35 0a10 0409  ..d......3.5....
-000026b0: 1073 09d4 1617 1819 380a 3a1d 1006 0910  .s......8.:.....
-000026c0: 4b08 d416 1718 193d 0a3f 0a10 0009 1102  K......=.?......
-000026d0: 2b09 d416 1718 1909 1d26 0a08 0908 2340  +........&....#@
-000026e0: 2800 0000 0000 0054 6e61 6d65 0923 4030  (......Tname.#@0
-000026f0: 0000 0000 0000 0008 0019 002e 0040 0048  .............@.H
-00002700: 005c 0065 0070 0083 008c 008e 008f 00a2  .\.e.p..........
-00002710: 00ab 00ba 00c6 00cb 00d1 00d6 00de 00e3  ................
-00002720: 00f0 00f9 00ff 0109 010f 0117 0119 011a  ................
-00002730: 011d 011e 0127 0129 012a 012c 012d 0136  .....'.).*.,.-.6
-00002740: 0138 0139 013b 013c 0145 0147 0148 014a  .8.9.;.<.E.G.H.J
-00002750: 014b 0154 0156 0157 0159 015a 0163 0165  .K.T.V.W.Y.Z.c.e
-00002760: 0166 0168 0169 0172 0174 0175 0177 0178  .f.h.i.r.t.u.w.x
-00002770: 0181 0183 0184 0187 0188 0191 0192 0193  ................
-00002780: 0194 019d 01a2 01a3 0000 0000 0000 0201  ................
-00002790: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
-000027a0: 0000 0000 0000 01ac 0000 0009 0075 0074  .............u.t
-000027b0: 0069 006c 0069 0074 0069 0065 0073 6d6f  .i.l.i.t.i.e.smo
-000027c0: 4444 626c 6f62 0000 0008 38fe e678 02e5  DDblob....8..x..
-000027d0: c441 0000 0009 0075 0074 0069 006c 0069  .A.....u.t.i.l.i
-000027e0: 0074 0069 0065 0073 6d6f 6444 626c 6f62  .t.i.e.smodDblob
-000027f0: 0000 0008 38fe e678 02e5 c441 0000 0009  ....8..x...A....
-00002800: 0075 0074                                .u.t
+00002500: 0000 0000 0000 4d00 0000 0000 0000 0000  ......M.........
+00002510: 0000 0000 0001 dd00 0000 0900 7500 7400  ............u.t.
+00002520: 6900 6c00 6900 7400 6900 6500 736c 7376  i.l.i.t.i.e.slsv
+00002530: 7062 6c6f 6200 0002 5e62 706c 6973 7430  pblob...^bplist0
+00002540: 30d8 0102 0304 0506 0708 090a 0b1d 4546  0.............EF
+00002550: 0a48 5f10 1276 6965 774f 7074 696f 6e73  .H_..viewOptions
+00002560: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
+00002570: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
+00002580: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
+00002590: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
+000025a0: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
+000025b0: 656c 6174 6976 6544 6174 6573 5869 636f  elativeDatesXico
+000025c0: 6e53 697a 6510 0109 d90c 0d0e 0f10 1112  nSize...........
+000025d0: 1314 151e 2328 2d32 373c 4158 636f 6d6d  ....#(-27<AXcomm
+000025e0: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
+000025f0: 6e65 645b 6461 7465 4372 6561 7465 6454  ned[dateCreatedT
+00002600: 7369 7a65 556c 6162 656c 546b 696e 6457  sizeUlabelTkindW
+00002610: 7665 7273 696f 6e54 6e61 6d65 5c64 6174  versionTname\dat
+00002620: 654d 6f64 6966 6965 64d4 1617 1819 1a0a  eModified.......
+00002630: 1c1d 5569 6e64 6578 5961 7363 656e 6469  ..UindexYascendi
+00002640: 6e67 5577 6964 7468 5776 6973 6962 6c65  ngUwidthWvisible
+00002650: 1007 0911 012c 08d4 1617 1819 1f1d 211d  .....,........!.
+00002660: 1008 0810 c808 d416 1718 1924 1d26 1d10  ...........$.&..
+00002670: 0208 10b5 08d4 1617 1819 291d 2b0a 1003  ..........).+...
+00002680: 0810 6109 d416 1718 192e 0a30 1d10 0509  ..a........0....
+00002690: 1064 08d4 1617 1819 330a 350a 1004 0910  .d......3.5.....
+000026a0: 7309 d416 1718 1938 0a3a 1d10 0609 104b  s......8.:.....K
+000026b0: 08d4 1617 1819 3d0a 3f0a 1000 0911 022b  ......=.?......+
+000026c0: 09d4 1617 1819 091d 260a 0809 0823 4028  ........&....#@(
+000026d0: 0000 0000 0000 546e 616d 6509 2340 3000  ......Tname.#@0.
+000026e0: 0000 0000 0000 0800 1900 2e00 4000 4800  ............@.H.
+000026f0: 5c00 6500 7000 8300 8c00 8e00 8f00 a200  \.e.p...........
+00002700: ab00 ba00 c600 cb00 d100 d600 de00 e300  ................
+00002710: f000 f900 ff01 0901 0f01 1701 1901 1a01  ................
+00002720: 1d01 1e01 2701 2901 2a01 2c01 2d01 3601  ....'.).*.,.-.6.
+00002730: 3801 3901 3b01 3c01 4501 4701 4801 4a01  8.9.;.<.E.G.H.J.
+00002740: 4b01 5401 5601 5701 5901 5a01 6301 6501  K.T.V.W.Y.Z.c.e.
+00002750: 6601 6801 6901 7201 7401 7501 7701 7801  f.h.i.r.t.u.w.x.
+00002760: 8101 8301 8401 8701 8801 9101 9201 9301  ................
+00002770: 9401 9d01 a201 a300 0000 0000 0002 0100  ................
+00002780: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
+00002790: 0000 0000 0001 ac00 0000 0900 7500 7400  ............u.t.
+000027a0: 6900 6c00 6900 7400 6900 6500 736d 6f44  i.l.i.t.i.e.smoD
+000027b0: 4462 6c6f 6200 0000 0838 fee6 7802 e5c4  Dblob....8..x...
+000027c0: 4100 0000 0900 7500 7400 6900 6c00 6900  A.....u.t.i.l.i.
+000027d0: 7400 6900 6500 736d 6f64 4462 6c6f 6200  t.i.e.smodDblob.
+000027e0: 0000 0838 fee6 7802 e5c4 4100 0000 0900  ...8..x...A.....
+000027f0: 7500 7400 6900 6c00 6900 7400 6900 6500  u.t.i.l.i.t.i.e.
+00002800: 7370 6831                                sph1
```

### Comparing `wordhoard-1.5.4/wordhoard/__pycache__/homophones.cpython-39.pyc` & `wordhoard-1.5.5/wordhoard/__pycache__/homophones.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Mar 20 19:37:32 2023 UTC, .py size: 6443 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,332 +1,373 @@
-00000000: 610d 0d0a 0000 0000 fcb5 1864 2b19 0000  a..........d+...
+00000000: 610d 0d0a 0000 0000 63fb 3c66 d71a 0000  a.......c.<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000a 0000 0040 0000 0073 8002 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5a05 6406 6407 6c06 5a06 6406  Z.d.Z.d.d.l.Z.d.
 00000050: 6407 6c07 5a07 6406 6407 6c08 5a08 6406  d.l.Z.d.d.l.Z.d.
 00000060: 6407 6c09 5a09 6406 6407 6c0a 5a0a 6406  d.l.Z.d.d.l.Z.d.
 00000070: 6408 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6406  d.l.m.Z.m.Z...d.
 00000080: 6409 6c0e 6d0f 5a0f 0100 6406 640a 6c10  d.l.m.Z...d.d.l.
 00000090: 6d11 5a11 0100 6509 a012 6513 a101 5a14  m.Z...e...e...Z.
-000000a0: 6506 6a15 a016 6506 6a15 a017 6518 a101  e.j...e.j...e...
-000000b0: a101 5a19 7a4e 6506 6a15 a01a 6519 640b  ..Z.zNe.j...e.d.
-000000c0: a102 5a1b 651c 651b 640c 8302 8f22 5a1d  ..Z.e.e.d...."Z.
-000000d0: 6508 a01e 651d a101 611f 651d a020 a100  e...e...a.e.. ..
-000000e0: 0100 5700 6407 0400 0400 8303 0100 6e10  ..W.d.........n.
-000000f0: 3100 73c8 3000 0100 0100 0100 5900 0100  1.s.0.......Y...
-00000100: 5700 6ea2 0400 6521 9001 7926 0100 5a22  W.n...e!..y&..Z"
-00000110: 0100 7a38 6514 a022 640d a101 0100 6514  ..z8e.."d.....e.
-00000120: a022 640e a01a 650a a023 6522 6a24 a101  ."d...e..#e"j$..
-00000130: a101 a101 0100 6507 a025 640f a101 0100  ......e..%d.....
-00000140: 5700 5900 6407 5a22 5b22 6e5a 6407 5a22  W.Y.d.Z"["nZd.Z"
-00000150: 5b22 3000 0400 6526 9001 7976 0100 5a22  ["0...e&..yv..Z"
-00000160: 0100 7a38 6514 a022 6410 a101 0100 6514  ..z8e.."d.....e.
-00000170: a022 640e a01a 650a a023 6522 6a24 a101  ."d...e..#e"j$..
-00000180: a101 a101 0100 6507 a025 640f a101 0100  ......e..%d.....
-00000190: 5700 5900 6407 5a22 5b22 6e0a 6407 5a22  W.Y.d.Z"["n.d.Z"
-000001a0: 5b22 3000 3000 7a50 6506 6a15 a01a 6519  ["0.0.zPe.j...e.
-000001b0: 6411 a102 5a27 651c 6527 640c 8302 8f22  d...Z'e.e'd...."
-000001c0: 5a28 6508 a01e 6528 a101 6129 6528 a020  Z(e...e(..a)e(. 
-000001d0: a100 0100 5700 6407 0400 0400 8303 0100  ....W.d.........
-000001e0: 6e12 3100 9001 73bc 3000 0100 0100 0100  n.1...s.0.......
-000001f0: 5900 0100 5700 6ea2 0400 6521 9002 791a  Y...W.n...e!..y.
-00000200: 0100 5a22 0100 7a38 6514 a022 6412 a101  ..Z"..z8e.."d...
-00000210: 0100 6514 a022 640e a01a 650a a023 6522  ..e.."d...e..#e"
-00000220: 6a24 a101 a101 a101 0100 6507 a025 640f  j$........e..%d.
-00000230: a101 0100 5700 5900 6407 5a22 5b22 6e5a  ....W.Y.d.Z"["nZ
-00000240: 6407 5a22 5b22 3000 0400 6526 9002 796a  d.Z"["0...e&..yj
-00000250: 0100 5a22 0100 7a38 6514 a022 6413 a101  ..Z"..z8e.."d...
-00000260: 0100 6514 a022 640e a01a 650a a023 6522  ..e.."d...e..#e"
-00000270: 6a24 a101 a101 a101 0100 6507 a025 640f  j$........e..%d.
-00000280: a101 0100 5700 5900 6407 5a22 5b22 6e0a  ....W.Y.d.Z"["n.
-00000290: 6407 5a22 5b22 3000 3000 4700 6414 6415  d.Z"["0.0.G.d.d.
-000002a0: 8400 6415 652a 8303 5a2b 6407 5300 2916  ..d.e*..Z+d.S.).
-000002b0: 7a72 0a54 6869 7320 5079 7468 6f6e 2073  zr.This Python s
-000002c0: 6372 6970 7420 6973 2064 6573 6967 6e65  cript is designe
-000002d0: 6420 746f 2071 7565 7279 2069 6e74 6572  d to query inter
-000002e0: 6e61 6c20 7265 706f 7369 746f 7269 6573  nal repositories
-000002f0: 2066 6f72 2074 6865 0a68 6f6d 6f70 686f   for the.homopho
-00000300: 6e65 7320 6173 736f 6369 6174 6564 2077  nes associated w
-00000310: 6974 6820 7468 6520 6769 7665 6e20 776f  ith the given wo
-00000320: 7264 2e0a 7a0e 4a6f 686e 2042 756d 6761  rd..z.John Bumga
-00000330: 726e 6572 7a0d 4a75 6e65 2031 312c 2032  rnerz.June 11, 2
-00000340: 3032 31da 0a50 726f 6475 6374 696f 6eda  021..Production.
-00000350: 034d 4954 7a21 436f 7079 7269 6768 7420  .MITz!Copyright 
-00000360: 2843 2920 3230 3231 204a 6f68 6e20 4275  (C) 2021 John Bu
-00000370: 6d67 6172 6e65 72e9 0000 0000 4e29 02da  mgarner.....N)..
-00000380: 044c 6973 74da 0555 6e69 6f6e 2901 da11  .List..Union)...
-00000390: 776f 7264 5f76 6572 6966 6963 6174 696f  word_verificatio
-000003a0: 6e29 01da 0e63 6f6c 6f72 697a 6564 5f74  n)...colorized_t
-000003b0: 6578 747a 2366 696c 6573 2f63 6f6d 6d6f  extz#files/commo
-000003c0: 6e5f 656e 676c 6973 685f 686f 6d6f 7068  n_english_homoph
-000003d0: 6f6e 6573 2e70 6b6c da02 7262 7a49 5468  ones.pkl..rbzITh
-000003e0: 6520 636f 6d6d 6f6e 5f65 6e67 6c69 7368  e common_english
-000003f0: 5f68 6f6d 6f70 686f 6e65 732e 706b 6c20  _homophones.pkl 
-00000400: 6669 6c65 2077 6173 206e 6f74 2066 6f75  file was not fou
-00000410: 6e64 2e20 4162 6f72 7469 6e67 206f 7065  nd. Aborting ope
-00000420: 7261 7469 6f6e 2eda 00e9 0100 0000 7a4f  ration........zO
-00000430: 416e 204f 5320 6572 726f 7220 6f63 6375  An OS error occu
-00000440: 7272 6564 2077 6865 6e20 7472 7969 6e67  rred when trying
-00000450: 2074 6f20 6f70 656e 2074 6865 2066 696c   to open the fil
-00000460: 6520 636f 6d6d 6f6e 5f65 6e67 6c69 7368  e common_english
-00000470: 5f68 6f6d 6f70 686f 6e65 732e 706b 6c7a  _homophones.pklz
-00000480: 1f66 696c 6573 2f6e 6f5f 686f 6d6f 7068  .files/no_homoph
-00000490: 6f6e 6573 5f65 6e67 6c69 7368 2e70 6b6c  ones_english.pkl
-000004a0: 7a45 5468 6520 6e6f 5f68 6f6d 6f70 686f  zEThe no_homopho
-000004b0: 6e65 735f 656e 676c 6973 682e 706b 6c20  nes_english.pkl 
-000004c0: 6669 6c65 2077 6173 206e 6f74 2066 6f75  file was not fou
-000004d0: 6e64 2e20 4162 6f72 7469 6e67 206f 7065  nd. Aborting ope
-000004e0: 7261 7469 6f6e 2e7a 4b41 6e20 4f53 2065  ration.zKAn OS e
-000004f0: 7272 6f72 206f 6363 7572 7265 6420 7768  rror occurred wh
-00000500: 656e 2074 7279 696e 6720 746f 206f 7065  en trying to ope
-00000510: 6e20 7468 6520 6669 6c65 206e 6f5f 686f  n the file no_ho
-00000520: 6d6f 7068 6f6e 6573 5f65 6e67 6c69 7368  mophones_english
-00000530: 2e70 6b6c 6300 0000 0000 0000 0000 0000  .pklc...........
-00000540: 0000 0000 0004 0000 0040 0000 0073 6400  .........@...sd.
-00000550: 0000 6500 5a01 6400 5a02 640f 6503 6402  ..e.Z.d.Z.d.e.d.
-00000560: 9c01 6403 6404 8405 5a04 6505 6405 9c01  ..d.d...Z.e.d...
-00000570: 6406 6407 8404 5a06 6507 6503 1900 6405  d.d...Z.e.e...d.
-00000580: 9c01 6408 6409 8404 5a08 6503 6405 9c01  ..d.d...Z.e.d...
-00000590: 640a 640b 8404 5a09 650a 6507 6503 1900  d.d...Z.e.e.e...
-000005a0: 6503 6602 1900 6405 9c01 640c 640d 8404  e.f...d...d.d...
-000005b0: 5a0b 640e 5300 2910 da0a 486f 6d6f 7068  Z.d.S.)...Homoph
-000005c0: 6f6e 6573 7209 0000 0029 01da 0d73 6561  onesr....)...sea
-000005d0: 7263 685f 7374 7269 6e67 6302 0000 0000  rch_stringc.....
-000005e0: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-000005f0: 0000 0073 0a00 0000 7c01 7c00 5f00 6401  ...s....|.|._.d.
-00000600: 5300 2902 612e 0200 000a 2020 2020 2020  S.).a.....      
-00000610: 2020 5075 7270 6f73 650a 2020 2020 2020    Purpose.      
-00000620: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00000630: 2020 2020 2054 6869 7320 5079 7468 6f6e       This Python
-00000640: 2063 6c61 7373 2069 7320 7573 6564 2074   class is used t
-00000650: 6f20 7175 6572 7920 696e 7465 726e 616c  o query internal
-00000660: 2066 696c 6573 2063 6f6e 7461 696e 696e   files containin
-00000670: 670a 2020 2020 2020 2020 456e 676c 6973  g.        Englis
-00000680: 6820 6c61 6e67 7561 6765 2068 6f6d 6f70  h language homop
-00000690: 686f 6e65 7320 6173 736f 6369 6174 6564  hones associated
-000006a0: 2077 6974 6820 6120 7370 6563 6966 6963   with a specific
-000006b0: 2077 6f72 642e 0a0a 2020 2020 2020 2020   word...        
-000006c0: 5573 6167 6520 4578 616d 706c 6573 0a20  Usage Examples. 
-000006d0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-000006e0: 2d0a 0a20 2020 2020 2020 203e 3e3e 2068  -..        >>> h
-000006f0: 6f6d 6f70 686f 6e65 7320 3d20 486f 6d6f  omophones = Homo
-00000700: 7068 6f6e 6573 2827 686f 7273 6527 290a  phones('horse').
-00000710: 2020 2020 2020 2020 3e3e 3e20 7265 7375          >>> resu
-00000720: 6c74 7320 3d20 686f 6d6f 7068 6f6e 6573  lts = homophones
-00000730: 2e66 696e 645f 686f 6d6f 7068 6f6e 6573  .find_homophones
-00000740: 2829 0a0a 2020 2020 2020 2020 3e3e 3e20  ()..        >>> 
-00000750: 686f 6d6f 7068 6f6e 6573 203d 2048 6f6d  homophones = Hom
-00000760: 6f70 686f 6e65 7328 7365 6172 6368 5f73  ophones(search_s
-00000770: 7472 696e 673d 2768 6f72 7365 2729 0a20  tring='horse'). 
-00000780: 2020 2020 2020 203e 3e3e 2072 6573 756c         >>> resul
-00000790: 7473 203d 2068 6f6d 6f70 686f 6e65 732e  ts = homophones.
-000007a0: 6669 6e64 5f68 6f6d 6f70 686f 6e65 7328  find_homophones(
-000007b0: 290a 0a20 2020 2020 2020 2050 6172 616d  )..        Param
-000007c0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-000007d0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-000007e0: 203a 7061 7261 6d20 7365 6172 6368 5f73   :param search_s
-000007f0: 7472 696e 673a 2073 7472 696e 6720 636f  tring: string co
-00000800: 6e74 6169 6e69 6e67 2074 6865 2076 6172  ntaining the var
-00000810: 6961 626c 6520 746f 206f 6274 6169 6e20  iable to obtain 
-00000820: 686f 6d6f 7068 6f6e 6573 2066 6f72 0a20  homophones for. 
-00000830: 2020 2020 2020 204e a901 da05 5f77 6f72         N...._wor
-00000840: 6429 02da 0473 656c 6672 0c00 0000 a900  d)...selfr......
-00000850: 7210 0000 00fa 4e2f 5573 6572 732f 6275  r.....N/Users/bu
-00000860: 6d67 6172 6e65 722f 5079 7468 6f6e 5f50  mgarner/Python_P
-00000870: 726f 6a65 6374 732f 776f 7264 686f 6172  rojects/wordhoar
-00000880: 645f 6465 7665 6c6f 706d 656e 742f 776f  d_development/wo
-00000890: 7264 686f 6172 642f 686f 6d6f 7068 6f6e  rdhoard/homophon
-000008a0: 6573 2e70 79da 085f 5f69 6e69 745f 5f52  es.py..__init__R
-000008b0: 0000 0073 0200 0000 0017 7a13 486f 6d6f  ...s......z.Homo
-000008c0: 7068 6f6e 6573 2e5f 5f69 6e69 745f 5f29  phones.__init__)
-000008d0: 01da 0672 6574 7572 6e63 0100 0000 0000  ...returnc......
-000008e0: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
-000008f0: 0000 7344 0000 0074 00a0 017c 006a 02a1  ..sD...t...|.j..
-00000900: 017d 017c 0172 1464 0153 0074 03a0 0464  .}.|.r.d.S.t...d
-00000910: 027c 006a 029b 0064 039d 03a1 0101 0074  .|.j...d.......t
-00000920: 03a0 0464 047c 006a 029b 0064 059d 03a1  ...d.|.j...d....
-00000930: 0101 0064 0653 0064 0753 0029 087a b90a  ...d.S.d.S.).z..
-00000940: 2020 2020 2020 2020 5468 6973 2066 756e          This fun
-00000950: 6374 696f 6e20 6973 2064 6573 6967 6e65  ction is designe
-00000960: 6420 746f 2076 616c 6964 6174 6520 7468  d to validate th
-00000970: 6174 2074 6865 2073 796e 7461 7820 666f  at the syntax fo
-00000980: 720a 2020 2020 2020 2020 6120 7374 7269  r.        a stri
-00000990: 6e67 2076 6172 6961 626c 6520 6973 2069  ng variable is i
-000009a0: 6e20 616e 2061 6363 6570 7461 626c 6520  n an acceptable 
-000009b0: 666f 726d 6174 2e0a 0a20 2020 2020 2020  format...       
-000009c0: 203a 7265 7475 726e 3a20 5472 7565 206f   :return: True o
-000009d0: 7220 4661 6c73 650a 2020 2020 2020 2020  r False.        
-000009e0: 3a72 7479 7065 3a20 626f 6f6c 6561 6e0a  :rtype: boolean.
-000009f0: 2020 2020 2020 2020 547a 0954 6865 2077          Tz.The w
-00000a00: 6f72 6420 7a1b 2077 6173 206e 6f74 2069  ord z. was not i
-00000a10: 6e20 6120 7661 6c69 6420 666f 726d 6174  n a valid format
-00000a20: 2e7a 1c50 6c65 6173 6520 7665 7269 6679  .z.Please verify
-00000a30: 2074 6861 7420 7468 6520 776f 7264 207a   that the word z
-00000a40: 1620 6973 2073 7065 6c6c 6564 2063 6f72  . is spelled cor
-00000a50: 7265 6374 6c79 2e46 4e29 0572 0600 0000  rectly.FN).r....
-00000a60: da14 7661 6c69 6461 7465 5f77 6f72 645f  ..validate_word_
-00000a70: 7379 6e74 6178 720e 0000 00da 066c 6f67  syntaxr......log
-00000a80: 6765 72da 0565 7272 6f72 2902 720f 0000  ger..error).r...
-00000a90: 00da 0a76 616c 6964 5f77 6f72 6472 1000  ...valid_wordr..
-00000aa0: 0000 7210 0000 0072 1100 0000 da0e 5f76  ..r....r......_v
-00000ab0: 616c 6964 6174 655f 776f 7264 6b00 0000  alidate_wordk...
-00000ac0: 730c 0000 0000 080c 0104 0104 0214 0114  s...............
-00000ad0: 017a 1948 6f6d 6f70 686f 6e65 732e 5f76  .z.Homophones._v
-00000ae0: 616c 6964 6174 655f 776f 7264 6301 0000  alidate_wordc...
-00000af0: 0000 0000 0000 0000 0005 0000 0007 0000  ................
-00000b00: 0003 0000 0073 6e00 0000 6700 7d01 7400  .....sn...g.}.t.
-00000b10: 4400 5d48 7d02 7401 8700 6601 6401 6402  D.]H}.t...f.d.d.
-00000b20: 8408 7c02 4400 8301 8301 7d03 7c03 7208  ..|.D.....}.|.r.
-00000b30: 7c02 4400 5d24 7d04 7c04 8800 6a02 6b03  |.D.]$}.|...j.k.
-00000b40: 722a 7c01 a003 8800 6a02 9b00 6403 7c04  r*|.....j...d.|.
-00000b50: 9b00 9d03 a101 0100 712a 7108 7404 7c01  ........q*q.t.|.
-00000b60: 8301 6404 6b04 726a 7405 7406 7c01 8301  ..d.k.rjt.t.|...
-00000b70: 8301 5300 6405 5300 2906 7a9f 0a20 2020  ..S.d.S.).z..   
-00000b80: 2020 2020 2054 6869 7320 6675 6e63 7469       This functi
-00000b90: 6f6e 2069 7465 7261 7465 7320 7468 726f  on iterates thro
-00000ba0: 7567 6820 6120 6c69 7374 206f 6620 6b6e  ugh a list of kn
-00000bb0: 6f77 6e0a 2020 2020 2020 2020 456e 676c  own.        Engl
-00000bc0: 6973 6820 6c61 6e67 7561 6765 2068 6f6d  ish language hom
-00000bd0: 6f70 686f 6e65 732e 0a0a 2020 2020 2020  ophones...      
-00000be0: 2020 3a72 6574 7572 6e3a 206c 6973 7420    :return: list 
-00000bf0: 6f66 2068 6f6d 6f70 686f 6e65 730a 2020  of homophones.  
-00000c00: 2020 2020 2020 3a72 7479 7065 3a20 6c69        :rtype: li
-00000c10: 7374 0a20 2020 2020 2020 2063 0100 0000  st.        c....
-00000c20: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000c30: 1300 0000 731a 0000 0067 007c 005d 127d  ....s....g.|.].}
-00000c40: 017c 0188 006a 006b 0272 047c 0191 0271  .|...j.k.r.|...q
-00000c50: 0453 0072 1000 0000 720d 0000 0029 02da  .S.r....r....)..
-00000c60: 022e 30da 0477 6f72 64a9 0172 0f00 0000  ..0..word..r....
-00000c70: 7210 0000 0072 1100 0000 da0a 3c6c 6973  r....r......<lis
-00000c80: 7463 6f6d 703e 8600 0000 f300 0000 007a  tcomp>.........z
-00000c90: 3948 6f6d 6f70 686f 6e65 732e 5f63 6f6d  9Homophones._com
-00000ca0: 6d6f 6e5f 656e 676c 6973 685f 686f 6d6f  mon_english_homo
-00000cb0: 7068 6f6e 6573 2e3c 6c6f 6361 6c73 3e2e  phones.<locals>.
-00000cc0: 3c6c 6973 7463 6f6d 703e 7a13 2069 7320  <listcomp>z. is 
-00000cd0: 6120 686f 6d6f 7068 6f6e 6520 6f66 2072  a homophone of r
-00000ce0: 0300 0000 4e29 07da 165f 6b6e 6f77 6e5f  ....N)..._known_
-00000cf0: 686f 6d6f 7068 6f6e 6573 5f6c 6973 74da  homophones_list.
-00000d00: 0462 6f6f 6c72 0e00 0000 da06 6170 7065  .boolr......appe
-00000d10: 6e64 da03 6c65 6eda 046c 6973 74da 0373  nd..len..list..s
-00000d20: 6574 2905 720f 0000 005a 0872 746e 5f6c  et).r....Z.rtn_l
-00000d30: 6973 74da 0a68 6f6d 6f70 686f 6e65 73da  ist..homophones.
-00000d40: 056d 6174 6368 721a 0000 0072 1000 0000  .matchr....r....
-00000d50: 721b 0000 0072 1100 0000 da1a 5f63 6f6d  r....r......_com
-00000d60: 6d6f 6e5f 656e 676c 6973 685f 686f 6d6f  mon_english_homo
-00000d70: 7068 6f6e 6573 7b00 0000 7312 0000 0000  phones{...s.....
-00000d80: 0904 0108 0116 0104 0108 010a 011a 010c  ................
-00000d90: 017a 2548 6f6d 6f70 686f 6e65 732e 5f63  .z%Homophones._c
-00000da0: 6f6d 6d6f 6e5f 656e 676c 6973 685f 686f  ommon_english_ho
-00000db0: 6d6f 7068 6f6e 6573 6301 0000 0000 0000  mophonesc.......
-00000dc0: 0000 0000 0002 0000 0006 0000 0043 0000  .............C..
-00000dd0: 0073 2c00 0000 7400 7c00 6a01 7402 7600  .s,...t.|.j.t.v.
-00000de0: 8301 7d01 7c01 7228 7403 6401 6402 6401  ..}.|.r(t.d.d.d.
-00000df0: 6403 7c00 6a01 9b00 9d02 8304 5300 6404  d.|.j.......S.d.
-00000e00: 5300 2905 7ab0 0a20 2020 2020 2020 2054  S.).z..        T
-00000e10: 6869 7320 6675 6e63 7469 6f6e 2069 7465  his function ite
-00000e20: 7261 7465 7320 7468 726f 7567 6820 6120  rates through a 
-00000e30: 6c69 7374 206f 6620 456e 676c 6973 680a  list of English.
-00000e40: 2020 2020 2020 2020 6c61 6e67 7561 6765          language
-00000e50: 2077 6f72 6473 2077 6974 6820 6e6f 206b   words with no k
-00000e60: 6e6f 776e 2068 6f6d 6f70 686f 6e65 732e  nown homophones.
-00000e70: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00000e80: 6e3a 206e 6f20 686f 6d6f 7068 6f6e 6573  n: no homophones
-00000e90: 2066 6f72 2077 6f72 640a 2020 2020 2020   for word.      
-00000ea0: 2020 3a72 7479 7065 3a20 7374 720a 2020    :rtype: str.  
-00000eb0: 2020 2020 2020 e9ff 0000 0072 0300 0000        .....r....
-00000ec0: 7a12 4e6f 2068 6f6d 6f70 686f 6e65 7320  z.No homophones 
-00000ed0: 666f 7220 4e29 0472 1f00 0000 720e 0000  for N).r....r...
-00000ee0: 00da 135f 6e6f 5f68 6f6d 6f70 686f 6e65  ..._no_homophone
-00000ef0: 735f 6c69 7374 7207 0000 0029 0272 0f00  s_listr....).r..
-00000f00: 0000 7225 0000 0072 1000 0000 7210 0000  ..r%...r....r...
-00000f10: 0072 1100 0000 da21 5f65 6e67 6c69 7368  .r.....!_english
-00000f20: 5f77 6f72 6473 5f77 6974 686f 7574 5f68  _words_without_h
-00000f30: 6f6d 6f70 686f 6e65 738e 0000 0073 0a00  omophones....s..
-00000f40: 0000 0009 0e01 0401 0801 0aff 7a2c 486f  ............z,Ho
-00000f50: 6d6f 7068 6f6e 6573 2e5f 656e 676c 6973  mophones._englis
-00000f60: 685f 776f 7264 735f 7769 7468 6f75 745f  h_words_without_
-00000f70: 686f 6d6f 7068 6f6e 6573 6301 0000 0000  homophonesc.....
-00000f80: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
-00000f90: 0000 0073 2c00 0000 7c00 a000 a100 7d01  ...s,...|.....}.
-00000fa0: 7c01 7228 7c00 a001 a100 7d02 7c02 721c  |.r(|.....}.|.r.
-00000fb0: 7c02 5300 7c02 7328 7c00 a002 a100 5300  |.S.|.s(|.....S.
-00000fc0: 6401 5300 2902 617d 0100 000a 2020 2020  d.S.).a}....    
-00000fd0: 2020 2020 5075 7270 6f73 650a 2020 2020      Purpose.    
-00000fe0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00000ff0: 2020 2020 2020 2054 6869 7320 6675 6e63         This func
-00001000: 7469 6f6e 2071 7565 7269 6573 206d 756c  tion queries mul
-00001010: 7469 706c 6520 6c69 7374 7320 746f 2066  tiple lists to f
-00001020: 696e 640a 2020 2020 2020 2020 456e 676c  ind.        Engl
-00001030: 6973 6820 6c61 6e67 7561 6765 2068 6f6d  ish language hom
-00001040: 6f70 686f 6e65 7320 6173 736f 6369 6174  ophones associat
-00001050: 6564 2077 6974 6820 7468 650a 2020 2020  ed with the.    
-00001060: 2020 2020 7370 6563 6966 6963 2077 6f72      specific wor
-00001070: 6420 7072 6f76 6964 6564 2074 6f20 7468  d provided to th
-00001080: 6520 436c 6173 7320 486f 6d6f 7068 6f6e  e Class Homophon
-00001090: 6573 2e0a 0a20 2020 2020 2020 2052 6574  es...        Ret
-000010a0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-000010b0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-000010c0: 3a72 6574 7572 6e3a 0a20 2020 2020 2020  :return:.       
-000010d0: 2020 2020 2068 6f6d 6f70 686f 6e65 733a       homophones:
-000010e0: 206c 6973 7420 6f66 2068 6f6d 6f70 686f   list of homopho
-000010f0: 6e65 730a 2020 2020 2020 2020 2020 2020  nes.            
-00001100: 6e6f 5f68 6f6d 6f70 686f 6e65 733a 2073  no_homophones: s
-00001110: 7472 696e 670a 0a20 2020 2020 2020 203a  tring..        :
-00001120: 7274 7970 653a 206c 6973 740a 2020 2020  rtype: list.    
-00001130: 2020 2020 3a72 7479 7065 3a20 7374 720a      :rtype: str.
-00001140: 2020 2020 2020 2020 4e29 0372 1800 0000          N).r....
-00001150: 7226 0000 0072 2900 0000 2903 720f 0000  r&...r)...).r...
-00001160: 0072 1700 0000 5a18 6b6e 6f77 6e5f 656e  .r....Z.known_en
-00001170: 676c 6973 685f 686f 6d6f 7068 6f6e 6573  glish_homophones
-00001180: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
-00001190: 0f66 696e 645f 686f 6d6f 7068 6f6e 6573  .find_homophones
-000011a0: 9c00 0000 730e 0000 0000 1108 0104 0108  ....s...........
-000011b0: 0104 0104 0104 017a 1a48 6f6d 6f70 686f  .......z.Homopho
-000011c0: 6e65 732e 6669 6e64 5f68 6f6d 6f70 686f  nes.find_homopho
-000011d0: 6e65 734e 2901 7209 0000 0029 0cda 085f  nesN).r....)..._
-000011e0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-000011f0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00001200: 5fda 0373 7472 7212 0000 0072 1f00 0000  _..strr....r....
-00001210: 7218 0000 0072 0400 0000 7226 0000 0072  r....r....r&...r
-00001220: 2900 0000 7205 0000 0072 2a00 0000 7210  )...r....r*...r.
-00001230: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
-00001240: 0000 720b 0000 0050 0000 0073 1000 0000  ..r....P...s....
-00001250: 0803 00ff 0201 02ff 0c19 0e10 1213 0e0e  ................
-00001260: 720b 0000 0029 2cda 075f 5f64 6f63 5f5f  r....),..__doc__
-00001270: da0a 5f5f 6175 7468 6f72 5f5f da08 5f5f  ..__author__..__
-00001280: 6461 7465 5f5f da0a 5f5f 7374 6174 7573  date__..__status
-00001290: 5f5f da0b 5f5f 6c69 6365 6e73 655f 5fda  __..__license__.
-000012a0: 0d5f 5f63 6f70 7972 6967 6874 5f5f da02  .__copyright__..
-000012b0: 6f73 da03 7379 73da 0670 6963 6b6c 65da  os..sys..pickle.
-000012c0: 076c 6f67 6769 6e67 da09 7472 6163 6562  .logging..traceb
-000012d0: 6163 6bda 0674 7970 696e 6772 0400 0000  ack..typingr....
-000012e0: 7205 0000 005a 1377 6f72 6468 6f61 7264  r....Z.wordhoard
-000012f0: 2e75 7469 6c69 7469 6573 7206 0000 00da  .utilitiesr.....
-00001300: 2277 6f72 6468 6f61 7264 2e75 7469 6c69  "wordhoard.utili
-00001310: 7469 6573 2e63 6f6c 6f72 697a 6564 5f74  ties.colorized_t
-00001320: 6578 7472 0700 0000 da09 6765 744c 6f67  extr......getLog
-00001330: 6765 7272 2b00 0000 7215 0000 00da 0470  gerr+...r......p
-00001340: 6174 68da 0764 6972 6e61 6d65 da07 6162  ath..dirname..ab
-00001350: 7370 6174 68da 085f 5f66 696c 655f 5f5a  spath..__file__Z
-00001360: 1050 4152 454e 545f 4449 5245 4354 4f52  .PARENT_DIRECTOR
-00001370: 59da 046a 6f69 6e5a 165f 6669 6c65 5f6b  Y..joinZ._file_k
-00001380: 6e6f 776e 5f68 6f6d 6f70 686f 6e65 73da  nown_homophones.
-00001390: 046f 7065 6e5a 0f5f 656e 675f 686f 6d6f  .openZ._eng_homo
-000013a0: 7068 6f6e 6573 da04 6c6f 6164 721e 0000  phones..loadr...
-000013b0: 00da 0563 6c6f 7365 da11 4669 6c65 4e6f  ...close..FileNo
-000013c0: 7446 6f75 6e64 4572 726f 7272 1600 0000  tFoundErrorr....
-000013d0: da09 666f 726d 6174 5f74 62da 0d5f 5f74  ..format_tb..__t
-000013e0: 7261 6365 6261 636b 5f5f da04 6578 6974  raceback__..exit
-000013f0: da07 4f53 4572 726f 725a 195f 6669 6c65  ..OSErrorZ._file
-00001400: 5f6e 6f5f 6b6e 6f77 6e5f 686f 6d6f 7068  _no_known_homoph
-00001410: 6f6e 6573 5a12 5f6e 6f5f 656e 675f 686f  onesZ._no_eng_ho
-00001420: 6d6f 7068 6f6e 6573 7228 0000 00da 066f  mophonesr(.....o
-00001430: 626a 6563 7472 0b00 0000 7210 0000 0072  bjectr....r....r
-00001440: 1000 0000 7210 0000 0072 1100 0000 da08  ....r....r......
-00001450: 3c6d 6f64 756c 653e 0300 0000 7354 0000  <module>....sT..
-00001460: 0004 0404 0104 0104 0104 0104 1708 0108  ................
-00001470: 0108 0108 0108 0110 010c 010c 020a 0214  ................
-00001480: 0402 010e 010c 010a 012a 0110 010a 0118  .........*......
-00001490: 011e 0110 010a 0118 0120 0402 010e 010c  ......... ......
-000014a0: 010a 012c 0110 010a 0118 011e 0110 010a  ...,............
-000014b0: 0118 0120 03                             ... .
+000000a0: 6700 6115 6700 6116 4700 640b 640c 8400  g.a.g.a.G.d.d...
+000000b0: 640c 8302 5a17 6517 a018 a100 0100 4700  d...Z.e.......G.
+000000c0: 640d 640e 8400 640e 8302 5a19 6407 5300  d.d...d...Z.d.S.
+000000d0: 290f 7a72 0a54 6869 7320 5079 7468 6f6e  ).zr.This Python
+000000e0: 206d 6f64 756c 6520 6973 2064 6573 6967   module is desig
+000000f0: 6e65 6420 746f 2071 7565 7279 2069 6e74  ned to query int
+00000100: 6572 6e61 6c20 7265 706f 7369 746f 7269  ernal repositori
+00000110: 6573 2066 6f72 2074 6865 0a68 6f6d 6f70  es for the.homop
+00000120: 686f 6e65 7320 6173 736f 6369 6174 6564  hones associated
+00000130: 2077 6974 6820 7468 6520 6769 7665 6e20   with the given 
+00000140: 776f 7264 2e0a 7a0e 4a6f 686e 2042 756d  word..z.John Bum
+00000150: 6761 726e 6572 7a0d 4a75 6e65 2031 312c  garnerz.June 11,
+00000160: 2032 3032 31da 0a50 726f 6475 6374 696f   2021..Productio
+00000170: 6eda 034d 4954 7a21 436f 7079 7269 6768  n..MITz!Copyrigh
+00000180: 7420 2843 2920 3230 3231 204a 6f68 6e20  t (C) 2021 John 
+00000190: 4275 6d67 6172 6e65 72e9 0000 0000 4e29  Bumgarner.....N)
+000001a0: 02da 044c 6973 74da 0555 6e69 6f6e 2901  ...List..Union).
+000001b0: da11 776f 7264 5f76 6572 6966 6963 6174  ..word_verificat
+000001c0: 696f 6e29 01da 0e63 6f6c 6f72 697a 6564  ion)...colorized
+000001d0: 5f74 6578 7463 0000 0000 0000 0000 0000  _textc..........
+000001e0: 0000 0000 0000 0500 0000 4000 0000 7338  ..........@...s8
+000001f0: 0000 0065 005a 0164 005a 0264 015a 0365  ...e.Z.d.Z.d.Z.e
+00000200: 0464 0264 039c 0164 0464 0584 0483 015a  .d.d...d.d.....Z
+00000210: 0565 0465 0665 0764 0264 069c 0364 0764  .e.e.e.d.d...d.d
+00000220: 0884 0483 015a 0864 0253 0029 09da 0c50  .....Z.d.S.)...P
+00000230: 6963 6b6c 654c 6f61 6465 727a 880a 2020  ickleLoaderz..  
+00000240: 2020 2020 2020 4120 7574 696c 6974 7920        A utility 
+00000250: 636c 6173 7320 666f 7220 6c6f 6164 696e  class for loadin
+00000260: 6720 7069 636b 6c65 2066 696c 6573 2063  g pickle files c
+00000270: 6f6e 7461 696e 696e 6720 456e 676c 6973  ontaining Englis
+00000280: 6820 686f 6d6f 7068 6f6e 6573 2061 6e64  h homophones and
+00000290: 0a20 2020 2020 2020 2045 6e67 6c69 7368  .        English
+000002a0: 2077 6f72 6473 2077 6974 6820 6e6f 206b   words with no k
+000002b0: 6e6f 776e 2068 6f6d 6f70 686f 6e65 732e  nown homophones.
+000002c0: 0a20 2020 204e a901 da06 7265 7475 726e  .    N....return
+000002d0: 6300 0000 0000 0000 0000 0000 0006 0000  c...............
+000002e0: 000a 0000 0043 0000 0073 1a01 0000 7400  .....C...s....t.
+000002f0: 6a01 a002 7400 6a01 a003 7404 a101 a101  j...t.j...t.....
+00000300: 7d00 7400 6a01 a005 7c00 6401 a102 7d01  }.t.j...|.d...}.
+00000310: 7400 6a01 a005 7c00 6402 a102 7d02 7a3c  t.j...|.d...}.z<
+00000320: 7406 7c01 6403 6404 8d02 8f1c 7d03 7407  t.|.d.d.....}.t.
+00000330: 6a08 7c03 6405 8d01 6109 5700 6406 0400  j.|.d...a.W.d...
+00000340: 0400 8303 0100 6e10 3100 7360 3000 0100  ......n.1.s`0...
+00000350: 0100 0100 5900 0100 5700 6e34 0400 740a  ....Y...W.n4..t.
+00000360: 740b 6602 79a0 0100 7d04 0100 7a18 740c  t.f.y...}...z.t.
+00000370: a00d 7c01 7c04 a102 0100 5700 5900 6406  ..|.|.....W.Y.d.
+00000380: 7d04 7e04 6e0a 6406 7d04 7e04 3000 3000  }.~.n.d.}.~.0.0.
+00000390: 7a3c 7406 7c02 6403 6404 8d02 8f1c 7d05  z<t.|.d.d.....}.
+000003a0: 7407 6a08 7c05 6405 8d01 610e 5700 6406  t.j.|.d...a.W.d.
+000003b0: 0400 0400 8303 0100 6e10 3100 73d2 3000  ........n.1.s.0.
+000003c0: 0100 0100 0100 5900 0100 5700 6e36 0400  ......Y...W.n6..
+000003d0: 740a 740b 6602 9001 7914 0100 7d04 0100  t.t.f...y...}...
+000003e0: 7a18 740c a00d 7c02 7c04 a102 0100 5700  z.t...|.|.....W.
+000003f0: 5900 6406 7d04 7e04 6e0a 6406 7d04 7e04  Y.d.}.~.n.d.}.~.
+00000400: 3000 3000 6406 5300 2907 7aab 0a20 2020  0.0.d.S.).z..   
+00000410: 2020 2020 2020 2020 204c 6f61 6473 2070           Loads p
+00000420: 6963 6b6c 6520 6669 6c65 7320 636f 6e74  ickle files cont
+00000430: 6169 6e69 6e67 2045 6e67 6c69 7368 2068  aining English h
+00000440: 6f6d 6f70 686f 6e65 7320 616e 6420 456e  omophones and En
+00000450: 676c 6973 6820 776f 7264 7320 7769 7468  glish words with
+00000460: 206e 6f20 6b6e 6f77 6e20 686f 6d6f 7068   no known homoph
+00000470: 6f6e 6573 2e0a 0a20 2020 2020 2020 2020  ones...         
+00000480: 2020 203a 7265 7475 726e 733a 204e 6f6e     :returns: Non
+00000490: 650a 2020 2020 2020 2020 2020 2020 3a72  e.            :r
+000004a0: 7479 7065 3a20 4e6f 6e65 5479 7065 0a20  type: NoneType. 
+000004b0: 2020 2020 2020 207a 2366 696c 6573 2f63         z#files/c
+000004c0: 6f6d 6d6f 6e5f 656e 676c 6973 685f 686f  ommon_english_ho
+000004d0: 6d6f 7068 6f6e 6573 2e70 6b6c 7a1f 6669  mophones.pklz.fi
+000004e0: 6c65 732f 6e6f 5f68 6f6d 6f70 686f 6e65  les/no_homophone
+000004f0: 735f 656e 676c 6973 682e 706b 6cda 0272  s_english.pkl..r
+00000500: 6229 02da 0466 696c 65da 046d 6f64 6529  b)...file..mode)
+00000510: 0172 0c00 0000 4e29 0fda 026f 73da 0470  .r....N)...os..p
+00000520: 6174 68da 0764 6972 6e61 6d65 da07 6162  ath..dirname..ab
+00000530: 7370 6174 68da 085f 5f66 696c 655f 5fda  spath..__file__.
+00000540: 046a 6f69 6eda 046f 7065 6eda 0670 6963  .join..open..pic
+00000550: 6b6c 65da 046c 6f61 64da 165f 6b6e 6f77  kle..load.._know
+00000560: 6e5f 686f 6d6f 7068 6f6e 6573 5f6c 6973  n_homophones_lis
+00000570: 74da 1146 696c 654e 6f74 466f 756e 6445  t..FileNotFoundE
+00000580: 7272 6f72 da07 4f53 4572 726f 7272 0800  rror..OSErrorr..
+00000590: 0000 da18 6861 6e64 6c65 5f70 6963 6b6c  ....handle_pickl
+000005a0: 655f 6c6f 6164 5f65 7272 6f72 da13 5f6e  e_load_error.._n
+000005b0: 6f5f 686f 6d6f 7068 6f6e 6573 5f6c 6973  o_homophones_lis
+000005c0: 7429 065a 1070 6172 656e 745f 6469 7265  t).Z.parent_dire
+000005d0: 6374 6f72 795a 165f 6669 6c65 5f6b 6e6f  ctoryZ._file_kno
+000005e0: 776e 5f68 6f6d 6f70 686f 6e65 735a 195f  wn_homophonesZ._
+000005f0: 6669 6c65 5f6e 6f5f 6b6e 6f77 6e5f 686f  file_no_known_ho
+00000600: 6d6f 7068 6f6e 6573 5a0f 5f65 6e67 5f68  mophonesZ._eng_h
+00000610: 6f6d 6f70 686f 6e65 73da 0565 7272 6f72  omophones..error
+00000620: 5a12 5f6e 6f5f 656e 675f 686f 6d6f 7068  Z._no_eng_homoph
+00000630: 6f6e 6573 a900 721d 0000 00fa 4d2f 5573  ones..r.....M/Us
+00000640: 6572 732f 6275 6d67 6172 6e65 722f 5079  ers/bumgarner/Py
+00000650: 7468 6f6e 5f50 726f 6a65 6374 732f 776f  thon_Projects/wo
+00000660: 7264 686f 6172 645f 7072 6f64 7563 7469  rdhoard_producti
+00000670: 6f6e 2f77 6f72 6468 6f61 7264 2f68 6f6d  on/wordhoard/hom
+00000680: 6f70 686f 6e65 732e 7079 da11 6c6f 6164  ophones.py..load
+00000690: 5f70 6963 6b6c 655f 6669 6c65 733a 0000  _pickle_files:..
+000006a0: 0073 1a00 0000 0009 1401 0e01 0e02 0203  .s..............
+000006b0: 0e01 2e01 1201 2202 0203 0e01 2e01 1401  ......".........
+000006c0: 7a1e 5069 636b 6c65 4c6f 6164 6572 2e6c  z.PickleLoader.l
+000006d0: 6f61 645f 7069 636b 6c65 5f66 696c 6573  oad_pickle_files
+000006e0: 2903 da09 6669 6c65 5f70 6174 6872 1c00  )...file_pathr..
+000006f0: 0000 720a 0000 0063 0200 0000 0000 0000  ..r....c........
+00000700: 0000 0000 0200 0000 0700 0000 4300 0000  ............C...
+00000710: 7354 0000 0074 007c 0174 0183 0272 1e74  sT...t.|.t...r.t
+00000720: 02a0 0364 017c 009b 0064 029d 03a1 0101  ...d.|...d......
+00000730: 006e 1074 02a0 0364 037c 009b 009d 02a1  .n.t...d.|......
+00000740: 0101 0074 02a0 0364 04a0 0474 05a0 067c  ...t...d...t...|
+00000750: 016a 07a1 01a1 01a1 0101 0074 08a0 0964  .j.........t...d
+00000760: 05a1 0101 0064 0653 0029 0761 3b01 0000  .....d.S.).a;...
+00000770: 0a20 2020 2020 2020 2020 2020 2048 616e  .            Han
+00000780: 646c 6573 2065 7272 6f72 7320 7768 656e  dles errors when
+00000790: 206c 6f61 6469 6e67 2070 6963 6b6c 6520   loading pickle 
+000007a0: 6669 6c65 732e 0a0a 2020 2020 2020 2020  files...        
+000007b0: 2020 2020 3a61 7267 2066 696c 655f 7061      :arg file_pa
+000007c0: 7468 3a20 5468 6520 7061 7468 206f 6620  th: The path of 
+000007d0: 7468 6520 7069 636b 6c65 2066 696c 652e  the pickle file.
+000007e0: 0a20 2020 2020 2020 2020 2020 203a 6172  .            :ar
+000007f0: 6720 7479 7065 2066 696c 655f 7061 7468  g type file_path
+00000800: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
+00000810: 2020 3a61 7267 2065 7272 6f72 3a20 5468    :arg error: Th
+00000820: 6520 6572 726f 7220 7261 6973 6564 2064  e error raised d
+00000830: 7572 696e 6720 6669 6c65 206c 6f61 6469  uring file loadi
+00000840: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
+00000850: 3a61 7267 2074 7970 6520 6572 726f 723a  :arg type error:
+00000860: 2045 7863 6570 7469 6f6e 0a20 2020 2020   Exception.     
+00000870: 2020 2020 2020 203a 7265 7475 726e 733a         :returns:
+00000880: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00000890: 2020 3a72 7479 7065 3b20 4e6f 6e65 5479    :rtype; NoneTy
+000008a0: 7065 0a20 2020 2020 2020 207a 1054 6865  pe.        z.The
+000008b0: 2070 6963 6b6c 6520 6669 6c65 207a 2320   pickle file z# 
+000008c0: 7761 7320 6e6f 7420 666f 756e 642e 2041  was not found. A
+000008d0: 626f 7274 696e 6720 6f70 6572 6174 696f  borting operatio
+000008e0: 6e2e 7a39 416e 204f 5320 6572 726f 7220  n.z9An OS error 
+000008f0: 6f63 6375 7272 6564 2077 6865 6e20 7472  occurred when tr
+00000900: 7969 6e67 2074 6f20 6f70 656e 2074 6865  ying to open the
+00000910: 2070 6963 6b6c 6520 6669 6c65 20da 00e9   pickle file ...
+00000920: 0100 0000 4e29 0ada 0a69 7369 6e73 7461  ....N)...isinsta
+00000930: 6e63 6572 1800 0000 da06 6c6f 6767 6572  ncer......logger
+00000940: 721c 0000 0072 1300 0000 da09 7472 6163  r....r......trac
+00000950: 6562 6163 6bda 0966 6f72 6d61 745f 7462  eback..format_tb
+00000960: da0d 5f5f 7472 6163 6562 6163 6b5f 5fda  ..__traceback__.
+00000970: 0373 7973 da04 6578 6974 2902 7220 0000  .sys..exit).r ..
+00000980: 0072 1c00 0000 721d 0000 0072 1d00 0000  .r....r....r....
+00000990: 721e 0000 0072 1a00 0000 5700 0000 730a  r....r....W...s.
+000009a0: 0000 0000 0c0a 0114 0210 0118 017a 2550  .............z%P
+000009b0: 6963 6b6c 654c 6f61 6465 722e 6861 6e64  ickleLoader.hand
+000009c0: 6c65 5f70 6963 6b6c 655f 6c6f 6164 5f65  le_pickle_load_e
+000009d0: 7272 6f72 2909 da08 5f5f 6e61 6d65 5f5f  rror)...__name__
+000009e0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+000009f0: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+00000a00: 635f 5fda 0c73 7461 7469 636d 6574 686f  c__..staticmetho
+00000a10: 6472 1f00 0000 da03 7374 72da 0945 7863  dr......str..Exc
+00000a20: 6570 7469 6f6e 721a 0000 0072 1d00 0000  eptionr....r....
+00000a30: 721d 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
+00000a40: 0800 0000 3400 0000 730a 0000 0008 0104  ....4...s.......
+00000a50: 0502 0110 1c02 0172 0800 0000 6300 0000  .......r....c...
+00000a60: 0000 0000 0000 0000 0000 0000 0004 0000  ................
+00000a70: 0040 0000 0073 6800 0000 6500 5a01 6400  .@...sh...e.Z.d.
+00000a80: 5a02 6401 5a03 6410 6504 6403 9c01 6404  Z.d.Z.d.e.d...d.
+00000a90: 6405 8405 5a05 6506 6406 9c01 6407 6408  d...Z.e.d...d.d.
+00000aa0: 8404 5a07 6508 6504 1900 6406 9c01 6409  ..Z.e.e...d...d.
+00000ab0: 640a 8404 5a09 6506 6406 9c01 640b 640c  d...Z.e.d...d.d.
+00000ac0: 8404 5a0a 650b 6508 6504 1900 640d 6602  ..Z.e.e.e...d.f.
+00000ad0: 1900 6406 9c01 640e 640f 8404 5a0c 640d  ..d...d.d...Z.d.
+00000ae0: 5300 2911 da0a 486f 6d6f 7068 6f6e 6573  S.)...Homophones
+00000af0: 61be 0100 000a 2020 2020 2020 2020 5075  a.....        Pu
+00000b00: 7270 6f73 650a 2020 2020 2020 2020 2d2d  rpose.        --
+00000b10: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00000b20: 2054 6869 7320 5079 7468 6f6e 2063 6c61   This Python cla
+00000b30: 7373 2069 7320 7573 6564 2074 6f20 7175  ss is used to qu
+00000b40: 6572 7920 696e 7465 726e 616c 2066 696c  ery internal fil
+00000b50: 6573 2063 6f6e 7461 696e 696e 670a 2020  es containing.  
+00000b60: 2020 2020 2020 456e 676c 6973 6820 6c61        English la
+00000b70: 6e67 7561 6765 2068 6f6d 6f70 686f 6e65  nguage homophone
+00000b80: 7320 6173 736f 6369 6174 6564 2077 6974  s associated wit
+00000b90: 6820 6120 7370 6563 6966 6963 2077 6f72  h a specific wor
+00000ba0: 642e 0a0a 2020 2020 2020 2020 5573 6167  d...        Usag
+00000bb0: 6520 4578 616d 706c 6573 0a20 2020 2020  e Examples.     
+00000bc0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00000bd0: 2020 2020 2020 3e3e 3e20 686f 6d6f 7068        >>> homoph
+00000be0: 6f6e 6573 203d 2048 6f6d 6f70 686f 6e65  ones = Homophone
+00000bf0: 7328 2768 6f72 7365 2729 0a20 2020 2020  s('horse').     
+00000c00: 2020 203e 3e3e 2072 6573 756c 7473 203d     >>> results =
+00000c10: 2068 6f6d 6f70 686f 6e65 732e 6669 6e64   homophones.find
+00000c20: 5f68 6f6d 6f70 686f 6e65 7328 290a 0a20  _homophones().. 
+00000c30: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00000c40: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00000c50: 2d2d 2d2d 0a20 2020 2020 2020 203a 7061  ----.        :pa
+00000c60: 7261 6d20 7365 6172 6368 5f73 7472 696e  ram search_strin
+00000c70: 673a 2073 7472 696e 6720 636f 6e74 6169  g: string contai
+00000c80: 6e69 6e67 2074 6865 2076 6172 6961 626c  ning the variabl
+00000c90: 6520 746f 206f 6274 6169 6e20 686f 6d6f  e to obtain homo
+00000ca0: 7068 6f6e 6573 2066 6f72 0a20 2020 2020  phones for.     
+00000cb0: 2020 2072 2100 0000 2901 da0d 7365 6172     r!...)...sear
+00000cc0: 6368 5f73 7472 696e 6763 0200 0000 0000  ch_stringc......
+00000cd0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+00000ce0: 0000 730a 0000 007c 017c 005f 0064 0053  ..s....|.|._.d.S
+00000cf0: 00a9 014e a901 da05 5f77 6f72 6429 02da  ...N...._word)..
+00000d00: 0473 656c 6672 3200 0000 721d 0000 0072  .selfr2...r....r
+00000d10: 1d00 0000 721e 0000 00da 085f 5f69 6e69  ....r......__ini
+00000d20: 745f 5f7d 0000 0073 0200 0000 0003 7a13  t__}...s......z.
+00000d30: 486f 6d6f 7068 6f6e 6573 2e5f 5f69 6e69  Homophones.__ini
+00000d40: 745f 5f72 0900 0000 6301 0000 0000 0000  t__r....c.......
+00000d50: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
+00000d60: 0073 3c00 0000 7400 a001 7c00 6a02 a101  .s<...t...|.j...
+00000d70: 7d01 7c01 7338 7403 a004 6401 7c00 6a02  }.|.s8t...d.|.j.
+00000d80: 9b00 6402 9d03 a101 0100 7403 a004 6403  ..d.......t...d.
+00000d90: 7c00 6a02 9b00 6404 9d03 a101 0100 7c01  |.j...d.......|.
+00000da0: 5300 2905 7ab9 0a20 2020 2020 2020 2054  S.).z..        T
+00000db0: 6869 7320 6675 6e63 7469 6f6e 2069 7320  his function is 
+00000dc0: 6465 7369 676e 6564 2074 6f20 7661 6c69  designed to vali
+00000dd0: 6461 7465 2074 6861 7420 7468 6520 7379  date that the sy
+00000de0: 6e74 6178 2066 6f72 0a20 2020 2020 2020  ntax for.       
+00000df0: 2061 2073 7472 696e 6720 7661 7269 6162   a string variab
+00000e00: 6c65 2069 7320 696e 2061 6e20 6163 6365  le is in an acce
+00000e10: 7074 6162 6c65 2066 6f72 6d61 742e 0a0a  ptable format...
+00000e20: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00000e30: 2054 7275 6520 6f72 2046 616c 7365 0a20   True or False. 
+00000e40: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
+00000e50: 6f6f 6c65 616e 0a20 2020 2020 2020 207a  oolean.        z
+00000e60: 0954 6865 2077 6f72 6420 7a1b 2077 6173  .The word z. was
+00000e70: 206e 6f74 2069 6e20 6120 7661 6c69 6420   not in a valid 
+00000e80: 666f 726d 6174 2e7a 1c50 6c65 6173 6520  format.z.Please 
+00000e90: 7665 7269 6679 2074 6861 7420 7468 6520  verify that the 
+00000ea0: 776f 7264 207a 1620 6973 2073 7065 6c6c  word z. is spell
+00000eb0: 6564 2063 6f72 7265 6374 6c79 2e29 0572  ed correctly.).r
+00000ec0: 0600 0000 da14 7661 6c69 6461 7465 5f77  ......validate_w
+00000ed0: 6f72 645f 7379 6e74 6178 7235 0000 0072  ord_syntaxr5...r
+00000ee0: 2400 0000 721c 0000 0029 0272 3600 0000  $...r....).r6...
+00000ef0: da0a 7661 6c69 645f 776f 7264 721d 0000  ..valid_wordr...
+00000f00: 0072 1d00 0000 721e 0000 00da 0e5f 7661  .r....r......_va
+00000f10: 6c69 6461 7465 5f77 6f72 6482 0000 0073  lidate_word....s
+00000f20: 0a00 0000 0008 0c01 0401 1401 1401 7a19  ..............z.
+00000f30: 486f 6d6f 7068 6f6e 6573 2e5f 7661 6c69  Homophones._vali
+00000f40: 6461 7465 5f77 6f72 6463 0100 0000 0000  date_wordc......
+00000f50: 0000 0000 0000 0300 0000 0600 0000 0300  ................
+00000f60: 0000 7348 0000 0067 007d 0174 0044 005d  ..sH...g.}.t.D.]
+00000f70: 327d 0274 0187 0066 0164 0164 0284 087c  2}.t...f.d.d...|
+00000f80: 0244 0083 0183 0172 087c 01a0 0287 0066  .D.....r.|.....f
+00000f90: 0164 0364 0284 087c 0244 0083 01a1 0101  .d.d...|.D......
+00000fa0: 0071 0874 0374 047c 0183 0183 0153 0029  .q.t.t.|.....S.)
+00000fb0: 047a 9f0a 2020 2020 2020 2020 5468 6973  .z..        This
+00000fc0: 2066 756e 6374 696f 6e20 6974 6572 6174   function iterat
+00000fd0: 6573 2074 6872 6f75 6768 2061 206c 6973  es through a lis
+00000fe0: 7420 6f66 206b 6e6f 776e 0a20 2020 2020  t of known.     
+00000ff0: 2020 2045 6e67 6c69 7368 206c 616e 6775     English langu
+00001000: 6167 6520 686f 6d6f 7068 6f6e 6573 2e0a  age homophones..
+00001010: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00001020: 3a20 6c69 7374 206f 6620 686f 6d6f 7068  : list of homoph
+00001030: 6f6e 6573 0a20 2020 2020 2020 203a 7274  ones.        :rt
+00001040: 7970 653a 206c 6973 740a 2020 2020 2020  ype: list.      
+00001050: 2020 6301 0000 0000 0000 0000 0000 0002    c.............
+00001060: 0000 0003 0000 0033 0000 0073 1800 0000  .......3...s....
+00001070: 7c00 5d10 7d01 7c01 8800 6a00 6b02 5600  |.].}.|...j.k.V.
+00001080: 0100 7102 6400 5300 7233 0000 0072 3400  ..q.d.S.r3...r4.
+00001090: 0000 a902 da02 2e30 da04 776f 7264 a901  .......0..word..
+000010a0: 7236 0000 0072 1d00 0000 721e 0000 00da  r6...r....r.....
+000010b0: 093c 6765 6e65 7870 723e 9a00 0000 f300  .<genexpr>......
+000010c0: 0000 007a 3848 6f6d 6f70 686f 6e65 732e  ...z8Homophones.
+000010d0: 5f63 6f6d 6d6f 6e5f 656e 676c 6973 685f  _common_english_
+000010e0: 686f 6d6f 7068 6f6e 6573 2e3c 6c6f 6361  homophones.<loca
+000010f0: 6c73 3e2e 3c67 656e 6578 7072 3e63 0100  ls>.<genexpr>c..
+00001100: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00001110: 0000 3300 0000 7328 0000 007c 005d 207d  ..3...s(...|.] }
+00001120: 017c 0188 006a 006b 0372 0288 006a 009b  .|...j.k.r...j..
+00001130: 0064 007c 019b 009d 0356 0001 0071 0264  .d.|.....V...q.d
+00001140: 0153 0029 027a 1320 6973 2061 2068 6f6d  .S.).z. is a hom
+00001150: 6f70 686f 6e65 206f 6620 4e72 3400 0000  ophone of Nr4...
+00001160: 723b 0000 0072 3e00 0000 721d 0000 0072  r;...r>...r....r
+00001170: 1e00 0000 723f 0000 009b 0000 0073 0200  ....r?.......s..
+00001180: 0000 0401 2905 7217 0000 00da 0361 6e79  ....).r......any
+00001190: da06 6578 7465 6e64 da04 6c69 7374 da03  ..extend..list..
+000011a0: 7365 7429 0372 3600 0000 5a0f 686f 6d6f  set).r6...Z.homo
+000011b0: 7068 6f6e 6573 5f6c 6973 74da 0a68 6f6d  phones_list..hom
+000011c0: 6f70 686f 6e65 7372 1d00 0000 723e 0000  ophonesr....r>..
+000011d0: 0072 1e00 0000 da1a 5f63 6f6d 6d6f 6e5f  .r......_common_
+000011e0: 656e 676c 6973 685f 686f 6d6f 7068 6f6e  english_homophon
+000011f0: 6573 9000 0000 730e 0000 0000 0804 0108  es....s.........
+00001200: 0116 010e 0102 ff0a 027a 2548 6f6d 6f70  .........z%Homop
+00001210: 686f 6e65 732e 5f63 6f6d 6d6f 6e5f 656e  hones._common_en
+00001220: 676c 6973 685f 686f 6d6f 7068 6f6e 6573  glish_homophones
+00001230: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001240: 0002 0000 0043 0000 0073 0a00 0000 7c00  .....C...s....|.
+00001250: 6a00 7401 7600 5300 2901 7aa8 0a20 2020  j.t.v.S.).z..   
+00001260: 2020 2020 2054 6869 7320 6675 6e63 7469       This functi
+00001270: 6f6e 2069 7465 7261 7465 7320 7468 726f  on iterates thro
+00001280: 7567 6820 6120 6c69 7374 206f 6620 456e  ugh a list of En
+00001290: 676c 6973 680a 2020 2020 2020 2020 6c61  glish.        la
+000012a0: 6e67 7561 6765 2077 6f72 6473 2077 6974  nguage words wit
+000012b0: 6820 6e6f 206b 6e6f 776e 2068 6f6d 6f70  h no known homop
+000012c0: 686f 6e65 732e 0a0a 2020 2020 2020 2020  hones...        
+000012d0: 3a72 6574 7572 6e3a 2054 7275 6520 6f72  :return: True or
+000012e0: 2046 616c 7365 0a20 2020 2020 2020 203a   False.        :
+000012f0: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
+00001300: 2020 2020 2902 7235 0000 0072 1b00 0000      ).r5...r....
+00001310: 723e 0000 0072 1d00 0000 721d 0000 0072  r>...r....r....r
+00001320: 1e00 0000 da21 5f65 6e67 6c69 7368 5f77  .....!_english_w
+00001330: 6f72 6473 5f77 6974 686f 7574 5f68 6f6d  ords_without_hom
+00001340: 6f70 686f 6e65 739f 0000 0073 0200 0000  ophones....s....
+00001350: 0008 7a2c 486f 6d6f 7068 6f6e 6573 2e5f  ..z,Homophones._
+00001360: 656e 676c 6973 685f 776f 7264 735f 7769  english_words_wi
+00001370: 7468 6f75 745f 686f 6d6f 7068 6f6e 6573  thout_homophones
+00001380: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
+00001390: 0000 0400 0000 4300 0000 7340 0000 007c  ......C...s@...|
+000013a0: 00a0 00a1 0072 3c7c 00a0 01a1 007d 017c  .....r<|.....}.|
+000013b0: 0172 187c 0153 007c 00a0 02a1 0064 0175  .r.|.S.|.....d.u
+000013c0: 0072 3c74 0364 027c 006a 049b 009d 0264  .r<t.d.|.j.....d
+000013d0: 0364 048d 0201 0064 0553 0064 0553 0029  .d.....d.S.d.S.)
+000013e0: 067a eb0a 2020 2020 2020 2020 5468 6973  .z..        This
+000013f0: 2066 756e 6374 696f 6e20 7175 6572 6965   function querie
+00001400: 7320 6d75 6c74 6970 6c65 206c 6973 7473  s multiple lists
+00001410: 2074 6f20 6669 6e64 2045 6e67 6c69 7368   to find English
+00001420: 206c 616e 6775 6167 6520 686f 6d6f 7068   language homoph
+00001430: 6f6e 6573 2061 7373 6f63 6961 7465 640a  ones associated.
+00001440: 2020 2020 2020 2020 7769 7468 2074 6865          with the
+00001450: 2073 7065 6369 6669 6320 776f 7264 2070   specific word p
+00001460: 726f 7669 6465 6420 746f 2074 6865 2043  rovided to the C
+00001470: 6c61 7373 2048 6f6d 6f70 686f 6e65 732e  lass Homophones.
+00001480: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+00001490: 6e3a 206c 6973 7420 6f66 2068 6f6d 6f70  n: list of homop
+000014a0: 686f 6e65 730a 2020 2020 2020 2020 3a72  hones.        :r
+000014b0: 7479 7065 3a20 556e 696f 6e5b 4c69 7374  type: Union[List
+000014c0: 5b73 7472 5d0a 2020 2020 2020 2020 467a  [str].        Fz
+000014d0: 1d4e 6f20 686f 6d6f 7068 6f6e 6573 2066  .No homophones f
+000014e0: 6f72 2074 6865 2077 6f72 6420 2d20 da07  or the word - ..
+000014f0: 6d61 6765 6e74 6129 02da 0474 6578 74da  magenta)...text.
+00001500: 0563 6f6c 6f72 4e29 0572 3a00 0000 7246  .colorN).r:...rF
+00001510: 0000 0072 4700 0000 7207 0000 0072 3500  ...rG...r....r5.
+00001520: 0000 2902 7236 0000 005a 186b 6e6f 776e  ..).r6...Z.known
+00001530: 5f65 6e67 6c69 7368 5f68 6f6d 6f70 686f  _english_homopho
+00001540: 6e65 7372 1d00 0000 721d 0000 0072 1e00  nesr....r....r..
+00001550: 0000 da0f 6669 6e64 5f68 6f6d 6f70 686f  ....find_homopho
+00001560: 6e65 73a9 0000 0073 1000 0000 0008 0801  nes....s........
+00001570: 0801 0401 0401 0c01 1401 0401 7a1a 486f  ............z.Ho
+00001580: 6d6f 7068 6f6e 6573 2e66 696e 645f 686f  mophones.find_ho
+00001590: 6d6f 7068 6f6e 6573 2901 7221 0000 0029  mophones).r!...)
+000015a0: 0d72 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
+000015b0: 722d 0000 0072 2f00 0000 7237 0000 00da  r-...r/...r7....
+000015c0: 0462 6f6f 6c72 3a00 0000 7204 0000 0072  .boolr:...r....r
+000015d0: 4600 0000 7247 0000 0072 0500 0000 724b  F...rG...r....rK
+000015e0: 0000 0072 1d00 0000 721d 0000 0072 1d00  ...r....r....r..
+000015f0: 0000 721e 0000 0072 3100 0000 6c00 0000  ..r....r1...l...
+00001600: 7312 0000 0008 0104 1100 ff02 0102 ff0c  s...............
+00001610: 050e 0e12 0f0e 0a72 3100 0000 291a 722d  .......r1...).r-
+00001620: 0000 00da 0a5f 5f61 7574 686f 725f 5fda  .....__author__.
+00001630: 085f 5f64 6174 655f 5fda 0a5f 5f73 7461  .__date__..__sta
+00001640: 7475 735f 5fda 0b5f 5f6c 6963 656e 7365  tus__..__license
+00001650: 5f5f da0d 5f5f 636f 7079 7269 6768 745f  __..__copyright_
+00001660: 5f72 0e00 0000 7228 0000 0072 1500 0000  _r....r(...r....
+00001670: da07 6c6f 6767 696e 6772 2500 0000 da06  ..loggingr%.....
+00001680: 7479 7069 6e67 7204 0000 0072 0500 0000  typingr....r....
+00001690: 5a13 776f 7264 686f 6172 642e 7574 696c  Z.wordhoard.util
+000016a0: 6974 6965 7372 0600 0000 da22 776f 7264  itiesr....."word
+000016b0: 686f 6172 642e 7574 696c 6974 6965 732e  hoard.utilities.
+000016c0: 636f 6c6f 7269 7a65 645f 7465 7874 7207  colorized_textr.
+000016d0: 0000 00da 0967 6574 4c6f 6767 6572 722a  .....getLoggerr*
+000016e0: 0000 0072 2400 0000 7217 0000 0072 1b00  ...r$...r....r..
+000016f0: 0000 7208 0000 0072 1f00 0000 7231 0000  ..r....r....r1..
+00001700: 0072 1d00 0000 721d 0000 0072 1d00 0000  .r....r....r....
+00001710: 721e 0000 00da 083c 6d6f 6475 6c65 3e03  r......<module>.
+00001720: 0000 0073 2600 0000 0404 0401 0401 0401  ...s&...........
+00001730: 0401 0418 0801 0801 0801 0801 0801 1003  ................
+00001740: 0c01 0c02 0a03 0401 0402 0e36 0802       ...........6..
```

### Comparing `wordhoard-1.5.4/wordhoard/__pycache__/synonyms.cpython-39.pyc` & `wordhoard-1.5.5/wordhoard/__pycache__/antonyms.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Mar 20 19:25:24 2023 UTC, .py size: 33916 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,1357 +1,1585 @@
-00000000: 610d 0d0a 0000 0000 24b3 1864 7c84 0000  a.......$..d|...
+00000000: 610d 0d0a 0000 0000 7df4 5166 437a 0000  a.......}.QfCz..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 0a01 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 3801 0000 6400  .....@...s8...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5a05 6406 6407 6c06 5a06 6406  Z.d.Z.d.d.l.Z.d.
 00000050: 6407 6c07 5a07 6406 6407 6c08 5a08 6406  d.l.Z.d.d.l.Z.d.
-00000060: 6407 6c09 5a09 6406 6407 6c0a 5a0a 6406  d.l.Z.d.d.l.Z.d.
-00000070: 6407 6c0b 5a0c 6406 6408 6c06 6d0d 5a0d  d.l.Z.d.d.l.m.Z.
-00000080: 0100 6406 6409 6c0e 6d0f 5a0f 6d10 5a10  ..d.d.l.m.Z.m.Z.
-00000090: 0100 6406 640a 6c11 6d12 5a12 6d13 5a13  ..d.d.l.m.Z.m.Z.
-000000a0: 0100 6406 640b 6c14 6d15 5a15 0100 6406  ..d.d.l.m.Z...d.
-000000b0: 640c 6c16 6d17 5a17 0100 6406 640d 6c18  d.l.m.Z...d.d.l.
-000000c0: 6d19 5a19 0100 6406 640e 6c1a 6d1b 5a1b  m.Z...d.d.l.m.Z.
-000000d0: 6d1c 5a1c 0100 6406 640f 6c1d 6d1e 5a1e  m.Z...d.d.l.m.Z.
-000000e0: 6d1f 5a1f 6d20 5a20 6d21 5a21 6d22 5a22  m.Z.m Z m!Z!m"Z"
-000000f0: 6d23 5a23 6d24 5a24 0100 6406 6410 6c25  m#Z#m$Z$..d.d.l%
-00000100: 6d26 5a26 6d27 5a27 6d28 5a28 0100 6406  m&Z&m'Z'm(Z(..d.
-00000110: 6411 6c29 6d2a 5a2a 0100 6508 a02b 652c  d.l)m*Z*..e..+e,
-00000120: a101 5a2d 4700 6412 6413 8400 6413 652e  ..Z-G.d.d...d.e.
-00000130: 8303 5a2f 6407 5300 2914 7a77 0a54 6869  ..Z/d.S.).zw.Thi
-00000140: 7320 5079 7468 6f6e 2073 6372 6970 7420  s Python script 
-00000150: 6973 2064 6573 6967 6e65 6420 746f 2071  is designed to q
-00000160: 7565 7279 206d 756c 7469 706c 6520 6f6e  uery multiple on
-00000170: 6c69 6e65 2072 6570 6f73 6974 6f72 6965  line repositorie
-00000180: 7320 666f 7220 7468 650a 7379 6e6f 6e79  s for the.synony
-00000190: 6d73 2061 7373 6f63 6961 7465 6420 7769  ms associated wi
-000001a0: 7468 2074 6865 2067 6976 656e 2077 6f72  th the given wor
-000001b0: 642e 0a7a 0e4a 6f68 6e20 4275 6d67 6172  d..z.John Bumgar
-000001c0: 6e65 727a 104f 6374 6f62 6572 2031 352c  nerz.October 15,
-000001d0: 2032 3032 30da 0a50 726f 6475 6374 696f   2020..Productio
-000001e0: 6eda 034d 4954 7a21 436f 7079 7269 6768  n..MITz!Copyrigh
-000001f0: 7420 2843 2920 3230 3230 204a 6f68 6e20  t (C) 2020 John 
-00000200: 4275 6d67 6172 6e65 72e9 0000 0000 4e29  Bumgarner.....N)
-00000210: 01da 0d42 6561 7574 6966 756c 536f 7570  ...BeautifulSoup
-00000220: 2902 da0c 6f6e 5f65 7863 6570 7469 6f6e  )...on_exception
-00000230: da04 6578 706f 2902 da06 6c69 6d69 7473  ..expo)...limits
-00000240: da12 5261 7465 4c69 6d69 7445 7863 6570  ..RateLimitExcep
-00000250: 7469 6f6e 2901 da05 5175 6572 7929 01da  tion)...Query)..
-00000260: 0a43 6c6f 7564 666c 6172 6529 01da 0e63  .Cloudflare)...c
-00000270: 6f6c 6f72 697a 6564 5f74 6578 7429 02da  olorized_text)..
-00000280: 1254 6872 6561 6450 6f6f 6c45 7865 6375  .ThreadPoolExecu
-00000290: 746f 72da 0c61 735f 636f 6d70 6c65 7465  tor..as_complete
-000002a0: 6429 07da 0444 6963 74da 044c 6973 74da  d)...Dict..List.
-000002b0: 084f 7074 696f 6e61 6cda 0353 6574 da05  .Optional..Set..
-000002c0: 5369 7a65 64da 0554 7570 6c65 da05 556e  Sized..Tuple..Un
-000002d0: 696f 6e29 03da 0763 6163 6869 6e67 da09  ion)...caching..
-000002e0: 636c 6561 6e73 696e 67da 1177 6f72 645f  cleansing..word_
-000002f0: 7665 7269 6669 6361 7469 6f6e 2901 da16  verification)...
-00000300: 436c 6f75 6466 6c61 7265 5665 7269 6669  CloudflareVerifi
-00000310: 6361 7469 6f6e 6300 0000 0000 0000 0000  cationc.........
-00000320: 0000 0000 0000 000a 0000 0040 0000 0073  ...........@...s
-00000330: 9001 0000 6500 5a01 6400 5a02 6424 6503  ....e.Z.d.Z.d$e.
-00000340: 6503 6504 6504 6505 6503 1900 6505 6506  e.e.e.e.e...e.e.
-00000350: 6503 6503 6602 1900 1900 6406 9c06 6407  e.e.f.....d...d.
-00000360: 6408 8405 5a07 6409 640a 8400 5a08 6509  d...Z.d.d...Z.e.
-00000370: 640b 9c01 640c 640d 8404 5a0a 650b 6509  d...d.d...Z.e.e.
-00000380: 650c 6506 6503 650d 6503 1900 6602 1900  e.e.e.e.e...f...
-00000390: 6405 6602 1900 6602 1900 640b 9c01 640e  d.f...f...d...d.
-000003a0: 640f 8404 5a0e 6503 650c 650d 6503 1900  d...Z.e.e.e.e...
-000003b0: 650f 6503 1900 6602 1900 6405 6410 9c03  e.e...f...d.d...
-000003c0: 6411 6412 8404 5a10 6503 6511 6a12 6a13  d.d...Z.e.e.j.j.
-000003d0: 6413 9c02 6414 6415 8404 5a14 650d 6503  d...d.d...Z.e.e.
-000003e0: 1900 640b 9c01 6416 6417 8404 5a15 650c  ..d...d.d...Z.e.
-000003f0: 650d 6516 1900 6506 6503 650d 6503 1900  e.e...e.e.e.e...
-00000400: 6602 1900 6503 6603 1900 640b 9c01 6418  f...e.f...d...d.
-00000410: 6419 8404 5a17 650c 650b 650d 6503 1900  d...Z.e.e.e.e...
-00000420: 6503 6602 1900 6405 6602 1900 640b 9c01  e.f...d.f...d...
-00000430: 641a 641b 8404 5a18 650c 650b 650d 6503  d.d...Z.e.e.e.e.
-00000440: 1900 6503 6602 1900 6405 6602 1900 640b  ..e.f...d.f...d.
-00000450: 9c01 641c 641d 8404 5a19 650c 650b 650d  ..d.d...Z.e.e.e.
-00000460: 6503 1900 6503 6602 1900 6405 6602 1900  e...e.f...d.f...
-00000470: 640b 9c01 641e 641f 8404 5a1a 650c 650b  d...d.d...Z.e.e.
-00000480: 650d 6503 1900 6503 6602 1900 6405 6602  e.e...e.f...d.f.
-00000490: 1900 640b 9c01 6420 6421 8404 5a1b 650c  ..d...d d!..Z.e.
-000004a0: 650b 650d 6503 1900 6503 6602 1900 6405  e.e.e...e.f...d.
-000004b0: 6602 1900 640b 9c01 6422 6423 8404 5a1c  f...d...d"d#..Z.
-000004c0: 6405 5300 2925 da08 5379 6e6f 6e79 6d73  d.S.)%..Synonyms
-000004d0: da00 da04 6c69 7374 e91e 0000 00e9 3c00  ....list......<.
-000004e0: 0000 4e29 06da 0d73 6561 7263 685f 7374  ..N)...search_st
-000004f0: 7269 6e67 da0d 6f75 7470 7574 5f66 6f72  ring..output_for
-00000500: 6d61 74da 166d 6178 5f6e 756d 6265 725f  mat..max_number_
-00000510: 6f66 5f72 6571 7565 7374 73da 1972 6174  of_requests..rat
-00000520: 655f 6c69 6d69 745f 7469 6d65 6f75 745f  e_limit_timeout_
-00000530: 7065 7269 6f64 da0a 7573 6572 5f61 6765  period..user_age
-00000540: 6e74 da07 7072 6f78 6965 7363 0700 0000  nt..proxiesc....
-00000550: 0000 0000 0000 0000 0a00 0000 0600 0000  ................
-00000560: 4300 0000 735e 0000 007c 067c 005f 007c  C...s^...|.|._.|
-00000570: 017c 005f 017c 057c 005f 027c 027c 005f  .|._.|.|._.|.|._
-00000580: 0368 0064 01a3 017c 005f 0464 027d 077c  .h.d...|._.d.}.|
-00000590: 077c 005f 0574 0674 0774 0864 037c 006a  .|._.t.t.t.d.|.j
-000005a0: 0964 048d 047d 0874 0a7c 037c 0464 058d  .d...}.t.|.|.d..
-000005b0: 027d 097c 087c 097c 006a 0b83 0183 017c  .}.|.|.|.j.....|
-000005c0: 005f 0b64 0653 0029 0761 0504 0000 0a20  ._.d.S.).a..... 
-000005d0: 2020 2020 2020 2054 6869 7320 5079 7468         This Pyth
-000005e0: 6f6e 2063 6c61 7373 2069 7320 7573 6564  on class is used
-000005f0: 2074 6f20 7175 6572 7920 6d75 6c74 6970   to query multip
-00000600: 6c65 206f 6e6c 696e 6520 7265 706f 7369  le online reposi
-00000610: 746f 7269 6573 2066 6f72 2074 6865 2073  tories for the s
-00000620: 796e 6f6e 796d 730a 2020 2020 2020 2020  ynonyms.        
-00000630: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
-00000640: 6120 7370 6563 6966 6963 2077 6f72 642e  a specific word.
-00000650: 0a0a 2020 2020 2020 2020 5573 6167 6520  ..        Usage 
-00000660: 4578 616d 706c 6573 0a20 2020 2020 2020  Examples.       
-00000670: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020   ----------..   
-00000680: 2020 2020 203e 3e3e 2073 796e 6f6e 796d       >>> synonym
-00000690: 203d 2053 796e 6f6e 796d 7328 276d 6f74   = Synonyms('mot
-000006a0: 6865 7227 290a 2020 2020 2020 2020 3e3e  her').        >>
-000006b0: 3e20 7265 7375 6c74 7320 3d20 7379 6e6f  > results = syno
-000006c0: 6e79 6d2e 6669 6e64 5f73 796e 6f6e 796d  nym.find_synonym
-000006d0: 7328 290a 0a20 2020 2020 2020 203e 3e3e  s()..        >>>
-000006e0: 2073 796e 6f6e 796d 203d 2053 796e 6f6e   synonym = Synon
-000006f0: 796d 7328 7365 6172 6368 5f73 7472 696e  yms(search_strin
-00000700: 673d 276d 6f74 6865 7227 290a 2020 2020  g='mother').    
-00000710: 2020 2020 3e3e 3e20 7265 7375 6c74 7320      >>> results 
-00000720: 3d20 7379 6e6f 6e79 6d2e 6669 6e64 5f73  = synonym.find_s
-00000730: 796e 6f6e 796d 7328 290a 0a20 2020 2020  ynonyms()..     
-00000740: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00000750: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00000760: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000770: 7365 6172 6368 5f73 7472 696e 673a 2073  search_string: s
-00000780: 7472 696e 6720 636f 6e74 6169 6e69 6e67  tring containing
-00000790: 2074 6865 2076 6172 6961 626c 6520 746f   the variable to
-000007a0: 206f 6274 6169 6e20 7379 6e6f 6e79 6d73   obtain synonyms
-000007b0: 2066 6f72 0a0a 2020 2020 2020 2020 3a70   for..        :p
-000007c0: 6172 616d 206f 7574 7075 745f 666f 726d  aram output_form
-000007d0: 6174 3a20 466f 726d 6174 2074 6f20 7573  at: Format to us
-000007e0: 6520 666f 7220 7265 7475 726e 6564 2072  e for returned r
-000007f0: 6573 756c 7473 2e0a 2020 2020 2020 2020  esults..        
-00000800: 2020 2020 2020 2044 6566 6175 6c74 2076         Default v
-00000810: 616c 7565 3a20 6c69 7374 3b20 4163 6365  alue: list; Acce
-00000820: 7074 6162 6c65 2076 616c 7565 733a 2064  ptable values: d
-00000830: 6963 7469 6f6e 6172 7920 6f72 206c 6973  ictionary or lis
-00000840: 740a 0a20 2020 2020 2020 203a 7061 7261  t..        :para
-00000850: 6d20 6d61 785f 6e75 6d62 6572 5f6f 665f  m max_number_of_
-00000860: 7265 7175 6573 7473 3a20 6d61 7869 6d75  requests: maximu
-00000870: 6d20 6e75 6d62 6572 206f 6620 7265 7175  m number of requ
-00000880: 6573 7473 2066 6f72 2061 2073 7065 6369  ests for a speci
-00000890: 6669 6320 7469 6d65 6f75 745f 7065 7269  fic timeout_peri
-000008a0: 6f64 0a0a 2020 2020 2020 2020 3a70 6172  od..        :par
-000008b0: 616d 2072 6174 655f 6c69 6d69 745f 7469  am rate_limit_ti
-000008c0: 6d65 6f75 745f 7065 7269 6f64 3a20 7468  meout_period: th
-000008d0: 6520 7469 6d65 2070 6572 696f 6420 6265  e time period be
-000008e0: 666f 7265 2061 2073 6573 7369 6f6e 2069  fore a session i
-000008f0: 7320 706c 6163 6564 2069 6e20 6120 7465  s placed in a te
-00000900: 6d70 6f72 6172 7920 6869 6265 726e 6174  mporary hibernat
-00000910: 696f 6e20 6d6f 6465 0a0a 2020 2020 2020  ion mode..      
-00000920: 2020 3a70 6172 616d 2075 7365 725f 6167    :param user_ag
-00000930: 656e 743a 2073 7472 696e 6720 636f 6e74  ent: string cont
-00000940: 6169 6e69 6e67 2065 6974 6865 7220 6120  aining either a 
-00000950: 676c 6f62 616c 2075 7365 7220 6167 656e  global user agen
-00000960: 7420 7479 7065 206f 7220 6120 7370 6563  t type or a spec
-00000970: 6966 6963 2075 7365 7220 6167 656e 740a  ific user agent.
-00000980: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000990: 7072 6f78 6965 733a 2064 6963 7469 6f6e  proxies: diction
-000009a0: 6172 7920 6f66 2070 726f 7869 6573 2074  ary of proxies t
-000009b0: 6f20 7573 6520 7769 7468 2050 7974 686f  o use with Pytho
-000009c0: 6e20 5265 7175 6573 7473 0a20 2020 2020  n Requests.     
-000009d0: 2020 203e 0300 0000 da04 6a73 6f6e 721b     >......jsonr.
-000009e0: 0000 00da 0a64 6963 7469 6f6e 6172 7946  .....dictionaryF
-000009f0: 721d 0000 0029 02da 086d 6178 5f74 696d  r....)...max_tim
-00000a00: 65da 0a6f 6e5f 6261 636b 6f66 6629 02da  e..on_backoff)..
-00000a10: 0563 616c 6c73 da06 7065 7269 6f64 4e29  .calls..periodN)
-00000a20: 0cda 085f 7072 6f78 6965 73da 055f 776f  ..._proxies.._wo
-00000a30: 7264 da0b 5f75 7365 725f 6167 656e 74da  rd.._user_agent.
-00000a40: 0e5f 6f75 7470 7574 5f66 6f72 6d61 74da  ._output_format.
-00000a50: 155f 7661 6c69 645f 6f75 7470 7574 5f66  ._valid_output_f
-00000a60: 6f72 6d61 7473 da12 5f72 6174 655f 6c69  ormats.._rate_li
-00000a70: 6d69 745f 7374 6174 7573 7205 0000 0072  mit_statusr....r
-00000a80: 0600 0000 7208 0000 00da 105f 6261 636b  ....r......_back
-00000a90: 6f66 665f 6861 6e64 6c65 7272 0700 0000  off_handlerr....
-00000aa0: da0d 6669 6e64 5f73 796e 6f6e 796d 7329  ..find_synonyms)
-00000ab0: 0ada 0473 656c 6672 1e00 0000 721f 0000  ...selfr....r...
-00000ac0: 0072 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
-00000ad0: 7223 0000 00da 1172 6174 655f 6c69 6d69  r#.....rate_limi
-00000ae0: 745f 7374 6174 7573 da07 6861 6e64 6c65  t_status..handle
-00000af0: 72da 076c 696d 6974 6572 a900 7236 0000  r..limiter..r6..
-00000b00: 00fa 4c2f 5573 6572 732f 6275 6d67 6172  ..L/Users/bumgar
-00000b10: 6e65 722f 5079 7468 6f6e 5f50 726f 6a65  ner/Python_Proje
-00000b20: 6374 732f 776f 7264 686f 6172 645f 6465  cts/wordhoard_de
-00000b30: 7665 6c6f 706d 656e 742f 776f 7264 686f  velopment/wordho
-00000b40: 6172 642f 7379 6e6f 6e79 6d73 2e70 79da  ard/synonyms.py.
-00000b50: 085f 5f69 6e69 745f 5f37 0000 0073 1400  .__init__7...s..
-00000b60: 0000 0023 0601 0601 0601 0601 0a02 0401  ...#............
-00000b70: 0603 1202 0c01 7a11 5379 6e6f 6e79 6d73  ......z.Synonyms
-00000b80: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00000b90: 0000 0000 0000 0100 0000 0600 0000 4300  ..............C.
-00000ba0: 0000 7330 0000 007c 006a 0064 0175 0072  ..s0...|.j.d.u.r
-00000bb0: 2c74 0174 0264 0264 0364 0364 0483 0483  ,t.t.d.d.d.d....
-00000bc0: 0101 0074 03a0 0464 05a1 0101 0064 067c  ...t...d.....d.|
-00000bd0: 005f 0064 0053 0029 074e 46e9 ff00 0000  ._.d.S.).NF.....
-00000be0: 7203 0000 007a 6954 6865 2073 796e 6f6e  r....ziThe synon
-00000bf0: 796d 7320 7175 6572 7920 7261 7465 206c  yms query rate l
-00000c00: 696d 6974 2077 6173 2072 6561 6368 6564  imit was reached
-00000c10: 2e20 5468 6520 7175 6572 7969 6e67 2070  . The querying p
-00000c20: 726f 6365 7373 2069 7320 656e 7465 7269  rocess is enteri
-00000c30: 6e67 2061 2074 656d 706f 7261 7279 2068  ng a temporary h
-00000c40: 6962 6572 6e61 7469 6f6e 206d 6f64 652e  ibernation mode.
-00000c50: 7a2a 5468 6520 7379 6e6f 6e79 6d73 2071  z*The synonyms q
-00000c60: 7565 7279 2072 6174 6520 6c69 6d69 7420  uery rate limit 
-00000c70: 7761 7320 7265 6163 6865 642e 5429 0572  was reached.T).r
-00000c80: 2f00 0000 da05 7072 696e 7472 0b00 0000  /.....printr....
-00000c90: da06 6c6f 6767 6572 da04 696e 666f 2901  ..logger..info).
-00000ca0: 7232 0000 0072 3600 0000 7236 0000 0072  r2...r6...r6...r
-00000cb0: 3700 0000 7230 0000 0069 0000 0073 0c00  7...r0...i...s..
-00000cc0: 0000 0001 0a01 0a01 02ff 0603 0a01 7a19  ..............z.
-00000cd0: 5379 6e6f 6e79 6d73 2e5f 6261 636b 6f66  Synonyms._backof
-00000ce0: 665f 6861 6e64 6c65 7229 01da 0672 6574  f_handler)...ret
-00000cf0: 7572 6e63 0100 0000 0000 0000 0000 0000  urnc............
-00000d00: 0200 0000 0500 0000 4300 0000 7344 0000  ........C...sD..
-00000d10: 0074 00a0 017c 006a 02a1 017d 017c 0172  .t...|.j...}.|.r
-00000d20: 1464 0153 0074 03a0 0464 027c 006a 029b  .d.S.t...d.|.j..
-00000d30: 0064 039d 03a1 0101 0074 03a0 0464 047c  .d.......t...d.|
-00000d40: 006a 029b 0064 059d 03a1 0101 0064 0653  .j...d.......d.S
-00000d50: 0064 0753 0029 087a b60a 2020 2020 2020  .d.S.).z..      
-00000d60: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
-00000d70: 6973 2064 6573 6967 6e65 6420 746f 2076  is designed to v
-00000d80: 616c 6964 6174 6520 7468 6174 2074 6865  alidate that the
-00000d90: 2073 796e 7461 7820 666f 720a 2020 2020   syntax for.    
-00000da0: 2020 2020 6120 7374 7269 6e67 2076 6172      a string var
-00000db0: 6961 626c 6520 6973 2069 6e20 616e 2061  iable is in an a
-00000dc0: 6363 6570 7461 626c 6520 666f 726d 6174  cceptable format
-00000dd0: 2e0a 0a20 2020 2020 2020 203a 7265 7475  ...        :retu
-00000de0: 726e 3a20 5472 7565 206f 7220 4661 6c73  rn: True or Fals
-00000df0: 650a 2020 2020 2020 2020 3a72 7479 7065  e.        :rtype
-00000e00: 3a20 626f 6f6c 0a20 2020 2020 2020 2054  : bool.        T
-00000e10: 7a09 5468 6520 776f 7264 207a 1b20 7761  z.The word z. wa
-00000e20: 7320 6e6f 7420 696e 2061 2076 616c 6964  s not in a valid
-00000e30: 2066 6f72 6d61 742e fa1c 506c 6561 7365   format...Please
-00000e40: 2076 6572 6966 7920 7468 6174 2074 6865   verify that the
-00000e50: 2077 6f72 6420 fa16 2069 7320 7370 656c   word .. is spel
-00000e60: 6c65 6420 636f 7272 6563 746c 792e 464e  led correctly.FN
-00000e70: 2905 7217 0000 00da 1476 616c 6964 6174  ).r......validat
-00000e80: 655f 776f 7264 5f73 796e 7461 7872 2b00  e_word_syntaxr+.
-00000e90: 0000 723b 0000 00da 0565 7272 6f72 2902  ..r;.....error).
-00000ea0: 7232 0000 00da 0a76 616c 6964 5f77 6f72  r2.....valid_wor
-00000eb0: 6472 3600 0000 7236 0000 0072 3700 0000  dr6...r6...r7...
-00000ec0: da0e 5f76 616c 6964 6174 655f 776f 7264  .._validate_word
-00000ed0: 7100 0000 730c 0000 0000 080c 0104 0104  q...s...........
-00000ee0: 0214 0114 017a 1753 796e 6f6e 796d 732e  .....z.Synonyms.
-00000ef0: 5f76 616c 6964 6174 655f 776f 7264 6301  _validate_wordc.
-00000f00: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00000f10: 0000 0043 0000 0073 1000 0000 7400 a001  ...C...s....t...
-00000f20: 7c00 6a02 a101 7d01 7c01 5300 a901 4e29  |.j...}.|.S...N)
-00000f30: 0372 1500 0000 da0e 6361 6368 655f 7379  .r......cache_sy
-00000f40: 6e6f 6e79 6d73 722b 0000 0029 0272 3200  nonymsr+...).r2.
-00000f50: 0000 da0b 6368 6563 6b5f 6361 6368 6572  ....check_cacher
-00000f60: 3600 0000 7236 0000 0072 3700 0000 da0c  6...r6...r7.....
-00000f70: 5f63 6865 636b 5f63 6163 6865 8100 0000  _check_cache....
-00000f80: 7304 0000 0000 010c 017a 1553 796e 6f6e  s........z.Synon
-00000f90: 796d 732e 5f63 6865 636b 5f63 6163 6865  yms._check_cache
-00000fa0: 2903 da0c 706f 735f 6361 7465 676f 7279  )...pos_category
-00000fb0: da08 7379 6e6f 6e79 6d73 723d 0000 0063  ..synonymsr=...c
-00000fc0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00000fd0: 0500 0000 4300 0000 7314 0000 0074 00a0  ....C...s....t..
-00000fe0: 017c 006a 027c 017c 02a1 0301 0064 0053  .|.j.|.|.....d.S
-00000ff0: 0072 4400 0000 2903 7215 0000 00da 1a69  .rD...).r......i
-00001000: 6e73 6572 745f 776f 7264 5f63 6163 6865  nsert_word_cache
-00001010: 5f73 796e 6f6e 796d 7372 2b00 0000 2903  _synonymsr+...).
-00001020: 7232 0000 0072 4800 0000 7249 0000 0072  r2...rH...rI...r
-00001030: 3600 0000 7236 0000 0072 3700 0000 da0d  6...r6...r7.....
-00001040: 5f75 7064 6174 655f 6361 6368 6585 0000  _update_cache...
-00001050: 0073 0400 0000 0001 1001 7a16 5379 6e6f  .s........z.Syno
-00001060: 6e79 6d73 2e5f 7570 6461 7465 5f63 6163  nyms._update_cac
-00001070: 6865 2902 da03 7572 6c72 3d00 0000 6302  he)...urlr=...c.
-00001080: 0000 0000 0000 0000 0000 0003 0000 0005  ................
-00001090: 0000 0043 0000 0073 aa00 0000 7c00 6a00  ...C...s....|.j.
-000010a0: 6401 7500 7224 7c00 6a01 6401 7500 7224  d.u.r$|.j.d.u.r$
-000010b0: 7402 7c01 8301 a003 a100 7d02 7c02 5300  t.|.......}.|.S.
-000010c0: 7c00 6a00 6401 7500 724c 7c00 6a01 6401  |.j.d.u.rL|.j.d.
-000010d0: 7501 724c 7402 7c01 7c00 6a01 8302 a003  u.rLt.|.|.j.....
-000010e0: a100 7d02 7c02 5300 7c00 6a00 6401 7501  ..}.|.S.|.j.d.u.
-000010f0: 7278 7c00 6a01 6401 7500 7278 7402 7c01  rx|.j.d.u.rxt.|.
-00001100: 6401 7c00 6a00 6402 8d03 a003 a100 7d02  d.|.j.d.......}.
-00001110: 7c02 5300 7c00 6a00 6401 7501 72a6 7c00  |.S.|.j.d.u.r.|.
-00001120: 6a01 6401 7501 72a6 7402 7c01 7c00 6a01  j.d.u.r.t.|.|.j.
-00001130: 7c00 6a00 6402 8d03 a003 a100 7d02 7c02  |.j.d.......}.|.
-00001140: 5300 6401 5300 2903 6111 0100 000a 2020  S.d.S.).a.....  
-00001150: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
-00001160: 696f 6e20 7175 6572 6965 7320 7468 6520  ion queries the 
-00001170: 7265 7175 6573 7465 6420 6f6e 6c69 6e65  requested online
-00001180: 2072 6570 6f73 6974 6f72 7920 616e 6420   repository and 
-00001190: 7265 7475 726e 7320 7468 650a 2020 2020  returns the.    
-000011a0: 2020 2020 7265 7370 6f6e 7365 2066 6f72      response for
-000011b0: 2074 6869 7320 7370 6563 6966 6963 2071   this specific q
-000011c0: 7565 7279 2e0a 0a20 2020 2020 2020 203a  uery...        :
-000011d0: 7061 7261 6d20 7572 6c3a 2074 6865 2055  param url: the U
-000011e0: 524c 2066 6f72 2074 6865 206f 6e6c 696e  RL for the onlin
-000011f0: 6520 7265 706f 7369 746f 7279 2062 6569  e repository bei
-00001200: 6e67 2071 7565 7269 6564 0a20 2020 2020  ng queried.     
-00001210: 2020 203a 7265 7475 726e 3a20 7265 7370     :return: resp
-00001220: 6f6e 7365 2063 6f6e 7465 6e74 0a20 2020  onse content.   
-00001230: 2020 2020 203a 7274 7970 653a 2072 6571       :rtype: req
-00001240: 7565 7374 732e 6d6f 6465 6c73 2e52 6573  uests.models.Res
-00001250: 706f 6e73 650a 2020 2020 2020 2020 4e29  ponse.        N)
-00001260: 0272 2200 0000 7223 0000 0029 0472 2a00  .r"...r#...).r*.
-00001270: 0000 722c 0000 0072 0900 0000 da10 6765  ..r,...r......ge
-00001280: 745f 7765 6273 6974 655f 6874 6d6c 2903  t_website_html).
-00001290: 7232 0000 0072 4c00 0000 da08 7265 7370  r2...rL.....resp
-000012a0: 6f6e 7365 7236 0000 0072 3600 0000 7237  onser6...r6...r7
-000012b0: 0000 00da 165f 7265 7175 6573 745f 6874  ....._request_ht
-000012c0: 7470 5f72 6573 706f 6e73 6589 0000 0073  tp_response....s
-000012d0: 1800 0000 0009 1401 0c01 0401 1401 1001  ................
-000012e0: 0401 1401 1401 0401 1401 1601 7a1f 5379  ............z.Sy
-000012f0: 6e6f 6e79 6d73 2e5f 7265 7175 6573 745f  nonyms._request_
-00001300: 6874 7470 5f72 6573 706f 6e73 6563 0100  http_responsec..
-00001310: 0000 0000 0000 0000 0000 0900 0000 0b00  ................
-00001320: 0000 4300 0000 73e4 0000 007c 006a 007c  ..C...s....|.j.|
-00001330: 006a 017c 006a 027c 006a 037c 006a 0467  .j.|.j.|.j.|.j.g
-00001340: 057d 0174 0564 0164 028d 018f ae7d 0267  .}.t.d.d.....}.g
-00001350: 007d 0367 007d 047a 4e7c 0144 005d 187d  .}.g.}.zN|.D.].}
-00001360: 057c 02a0 067c 05a1 017d 067c 03a0 077c  .|...|...}.|...|
-00001370: 06a1 0101 0071 3274 087c 0383 0144 005d  .....q2t.|...D.]
-00001380: 127d 077c 04a0 077c 07a0 09a1 00a1 0101  .}.|...|........
-00001390: 0071 547c 0457 0057 0002 0064 0304 0004  .qT|.W.W...d....
-000013a0: 0083 0301 0053 0004 0074 0a79 c001 007d  .....S...t.y...}
-000013b0: 0801 007a 2e74 0ba0 0c64 04a1 0101 0074  ...z.t...d.....t
-000013c0: 0ba0 0c64 05a0 0d74 0ea0 0f7c 086a 10a1  ...d...t...|.j..
-000013d0: 01a1 01a1 0101 0057 0059 0064 037d 087e  .......W.Y.d.}.~
-000013e0: 086e 0a64 037d 087e 0830 0030 0057 0064  .n.d.}.~.0.0.W.d
-000013f0: 0304 0004 0083 0301 006e 1031 0073 d630  .........n.1.s.0
-00001400: 0001 0001 0001 0059 0001 0064 0353 0029  .......Y...d.S.)
-00001410: 067a 790a 2020 2020 2020 2020 5275 6e73  .zy.        Runs
-00001420: 2074 6865 2071 7565 7279 2074 6173 6b73   the query tasks
-00001430: 2069 6e20 7061 7261 6c6c 656c 2075 7369   in parallel usi
-00001440: 6e67 2061 2054 6872 6561 6450 6f6f 6c2e  ng a ThreadPool.
-00001450: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00001460: 6e3a 206c 6973 740a 2020 2020 2020 2020  n: list.        
-00001470: 3a72 7479 7065 3a20 6e65 7374 6564 206c  :rtype: nested l
-00001480: 6973 740a 2020 2020 2020 2020 e905 0000  ist.        ....
-00001490: 0029 01da 0b6d 6178 5f77 6f72 6b65 7273  .)...max_workers
-000014a0: 4e7a 3841 6e20 756e 6b6e 6f77 6e20 6572  Nz8An unknown er
-000014b0: 726f 7220 6f63 6375 7272 6564 2069 6e20  ror occurred in 
-000014c0: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-000014d0: 6465 2073 6567 6d65 6e74 3a72 1a00 0000  de segment:r....
-000014e0: 2911 da19 5f71 7565 7279 5f63 6f6c 6c69  )..._query_colli
-000014f0: 6e73 5f64 6963 7469 6f6e 6172 79da 165f  ns_dictionary.._
-00001500: 7175 6572 795f 6d65 7272 6961 6d5f 7765  query_merriam_we
-00001510: 6273 7465 72da 125f 7175 6572 795f 7379  bster.._query_sy
-00001520: 6e6f 6e79 6d5f 636f 6dda 145f 7175 6572  nonym_com.._quer
-00001530: 795f 7468 6573 6175 7275 735f 636f 6dda  y_thesaurus_com.
-00001540: 0e5f 7175 6572 795f 776f 7264 6e65 7472  ._query_wordnetr
-00001550: 0c00 0000 da06 7375 626d 6974 da06 6170  ......submit..ap
-00001560: 7065 6e64 720d 0000 00da 0672 6573 756c  pendr......resul
-00001570: 74da 0945 7863 6570 7469 6f6e 723b 0000  t..Exceptionr;..
-00001580: 0072 4100 0000 da04 6a6f 696e da09 7472  .rA.....join..tr
-00001590: 6163 6562 6163 6bda 0966 6f72 6d61 745f  aceback..format_
-000015a0: 7462 da0d 5f5f 7472 6163 6562 6163 6b5f  tb..__traceback_
-000015b0: 5f29 0972 3200 0000 da05 7461 736b 73da  _).r2.....tasks.
-000015c0: 0865 7865 6375 746f 72da 0d72 756e 6e69  .executor..runni
-000015d0: 6e67 5f74 6173 6b73 da0e 6669 6e69 7368  ng_tasks..finish
-000015e0: 6564 5f74 6173 6b73 da04 7461 736b da0e  ed_tasks..task..
-000015f0: 7375 626d 6974 7465 645f 7461 736b da0d  submitted_task..
-00001600: 6669 6e69 7368 6564 5f74 6173 6b72 4100  finished_taskrA.
-00001610: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
-00001620: 00da 1c5f 7275 6e5f 7175 6572 795f 7461  ..._run_query_ta
-00001630: 736b 735f 696e 5f70 6172 616c 6c65 6c9f  sks_in_parallel.
-00001640: 0000 0073 2000 0000 0007 0c01 08ff 0403  ...s ...........
-00001650: 0c01 0401 0401 0201 0801 0a01 0c01 0c01  ................
-00001660: 1001 1401 0e01 0a01 7a25 5379 6e6f 6e79  ........z%Synony
-00001670: 6d73 2e5f 7275 6e5f 7175 6572 795f 7461  ms._run_query_ta
-00001680: 736b 735f 696e 5f70 6172 616c 6c65 6c63  sks_in_parallelc
-00001690: 0100 0000 0000 0000 0000 0000 0900 0000  ................
-000016a0: 0800 0000 4300 0000 7332 0200 007c 006a  ....C...s2...|.j
-000016b0: 007c 006a 0176 0172 2c74 0274 0364 0164  .|.j.v.r,t.t.d.d
-000016c0: 0264 0264 037c 006a 009b 0064 049d 0383  .d.d.|.j...d....
-000016d0: 0483 0101 0090 026e 027c 00a0 04a1 007d  .......n.|.....}
-000016e0: 017c 0164 0575 0072 5c74 0274 0364 0164  .|.d.u.r\t.t.d.d
-000016f0: 0264 0164 067c 006a 059b 0064 079d 0383  .d.d.|.j...d....
-00001700: 0483 0101 0090 016e d27c 0164 0875 0090  .......n.|.d.u..
-00001710: 0272 2e7c 00a0 06a1 007d 027c 0264 0219  .r.|.....}.|.d..
-00001720: 0064 0875 0090 0172 3074 077c 0264 0919  .d.u...r0t.|.d..
-00001730: 00a0 08a1 0083 0164 0219 007d 0374 09a0  .......d...}.t..
-00001740: 0a74 077c 0264 0919 00a0 0ba1 0083 01a1  .t.|.d..........
-00001750: 017d 047c 006a 0064 0a6b 0272 ca74 0c74  .}.|.j.d.k.r.t.t
-00001760: 0d64 0b64 0c84 007c 0264 0919 0044 0083  .d.d...|.d...D..
-00001770: 0183 0183 0153 007c 006a 0064 0d6b 0272  .....S.|.j.d.k.r
-00001780: f47c 006a 057c 0374 0c74 0d7c 0483 0174  .|.j.|.t.t.|...t
-00001790: 0e64 0e8d 0264 0f9c 0269 017d 057c 0553  .d...d...i.}.|.S
-000017a0: 007c 006a 0064 106b 0290 0272 2e74 0f6a  .|.j.d.k...r.t.j
-000017b0: 107c 006a 057c 0374 0c74 0d7c 0483 0174  .|.j.|.t.t.|...t
-000017c0: 0e64 0e8d 0264 0f9c 0269 0164 1164 0564  .d...d...i.d.d.d
-000017d0: 128d 037d 067c 0653 0090 006e fe7c 0264  ...}.|.S...n.|.d
-000017e0: 0219 0064 0575 0090 0272 2e7c 00a0 11a1  ...d.u...r.|....
-000017f0: 007d 0764 13a0 1274 0d64 1464 0c84 007c  .}.d...t.d.d...|
-00001800: 0744 0083 0183 01a1 017d 0364 1564 0c84  .D.......}.d.d..
-00001810: 007c 0744 0083 017d 0474 09a0 0a7c 04a1  .|.D...}.t...|..
-00001820: 017d 0874 09a0 137c 08a1 017d 087c 0890  .}.t...|...}.|..
-00001830: 0173 a474 0274 0364 0164 0264 0164 167c  .s.t.t.d.d.d.d.|
-00001840: 006a 059b 0064 179d 0383 0483 0101 006e  .j...d.........n
-00001850: 8a7c 006a 0064 0a6b 0290 0172 ca74 0c74  .|.j.d.k...r.t.t
-00001860: 0d64 1864 0c84 007c 0844 0083 0183 0174  .d.d...|.D.....t
-00001870: 0e64 0e8d 0253 007c 006a 0064 0d6b 0290  .d...S.|.j.d.k..
-00001880: 0172 f67c 006a 057c 0374 0c74 0d7c 0883  .r.|.j.|.t.t.|..
-00001890: 0174 0e64 0e8d 0264 0f9c 0269 017d 057c  .t.d...d...i.}.|
-000018a0: 0553 007c 006a 0064 106b 0290 0272 2e74  .S.|.j.d.k...r.t
-000018b0: 0f6a 107c 006a 057c 0374 0c74 0d7c 0883  .j.|.j.|.t.t.|..
-000018c0: 0174 0e64 0e8d 0264 0f9c 0269 0164 1164  .t.d...d...i.d.d
-000018d0: 0564 128d 037d 067c 0653 0064 1953 0029  .d...}.|.S.d.S.)
-000018e0: 1a61 7a01 0000 0a20 2020 2020 2020 2050  .az....        P
-000018f0: 7572 706f 7365 0a20 2020 2020 2020 202d  urpose.        -
-00001900: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00001910: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
-00001920: 7175 6572 6965 7320 6d75 6c74 6970 6c65  queries multiple
-00001930: 206f 6e6c 696e 6520 7265 706f 7369 746f   online reposito
-00001940: 7269 6573 2074 6f20 6469 7363 6f76 6572  ries to discover
-00001950: 2073 796e 6f6e 796d 730a 2020 2020 2020   synonyms.      
-00001960: 2020 6173 736f 6369 6174 6564 2077 6974    associated wit
-00001970: 6820 7468 6520 7370 6563 6966 6963 2077  h the specific w
-00001980: 6f72 6420 7072 6f76 6964 6564 2074 6f20  ord provided to 
-00001990: 7468 6520 436c 6173 7320 5379 6e6f 6e79  the Class Synony
-000019a0: 6d73 2e0a 2020 2020 2020 2020 5468 6520  ms..        The 
-000019b0: 7379 6e6f 6e79 6d73 2061 7265 2064 6564  synonyms are ded
-000019c0: 7570 6c69 6361 7465 6420 616e 6420 736f  uplicated and so
-000019d0: 7274 6564 2061 6c70 6861 6265 7469 6361  rted alphabetica
-000019e0: 6c6c 792e 0a0a 2020 2020 2020 2020 5265  lly...        Re
-000019f0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-00001a00: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00001a10: 203a 7265 7475 726e 733a 0a20 2020 2020   :returns:.     
-00001a20: 2020 2020 2020 2073 796e 6f6e 796d 733a         synonyms:
-00001a30: 206c 6973 7420 6f66 2073 796e 6f6e 796d   list of synonym
-00001a40: 730a 0a20 2020 2020 2020 203a 7274 7970  s..        :rtyp
-00001a50: 653a 206c 6973 740a 2020 2020 2020 2020  e: list.        
-00001a60: 7239 0000 0072 0300 0000 7a1d 5468 6520  r9...r....z.The 
-00001a70: 7072 6f76 6964 6564 206f 7574 7075 7420  provided output 
-00001a80: 7479 7065 202d 2d3e 207a 4220 3c2d 2d20  type --> zB <-- 
-00001a90: 6973 206e 6f74 206f 6e65 206f 6620 7468  is not one of th
-00001aa0: 6520 6163 6365 7074 6162 6c65 2074 7970  e acceptable typ
-00001ab0: 6573 3a20 6469 6374 696f 6e61 7279 2c20  es: dictionary, 
-00001ac0: 6c69 7374 206f 7220 6a73 6f6e 2e46 723e  list or json.Fr>
-00001ad0: 0000 0072 3f00 0000 54e9 0100 0000 721b  ...r?...T.....r.
-00001ae0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001af0: 0200 0000 0400 0000 5300 0000 7314 0000  ........S...s...
-00001b00: 0067 007c 005d 0c7d 017c 01a0 00a1 0091  .g.|.].}.|......
-00001b10: 0271 0453 0072 3600 0000 a901 da05 6c6f  .q.S.r6.......lo
-00001b20: 7765 72a9 02da 022e 30da 0477 6f72 6472  wer.....0..wordr
-00001b30: 3600 0000 7236 0000 0072 3700 0000 da0a  6...r6...r7.....
-00001b40: 3c6c 6973 7463 6f6d 703e d500 0000 f300  <listcomp>......
-00001b50: 0000 007a 2a53 796e 6f6e 796d 732e 6669  ...z*Synonyms.fi
-00001b60: 6e64 5f73 796e 6f6e 796d 732e 3c6c 6f63  nd_synonyms.<loc
-00001b70: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
-00001b80: 2500 0000 2901 da03 6b65 7929 02da 0e70  %...)...key)...p
-00001b90: 6172 745f 6f66 5f73 7065 6563 6872 4900  art_of_speechrI.
-00001ba0: 0000 7224 0000 00e9 0400 0000 2902 da06  ..r$........)...
-00001bb0: 696e 6465 6e74 da0c 656e 7375 7265 5f61  indent..ensure_a
-00001bc0: 7363 6969 721a 0000 0063 0100 0000 0000  sciir....c......
-00001bd0: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00001be0: 0000 7320 0000 0067 007c 005d 187d 017c  ..s ...g.|.].}.|
-00001bf0: 0172 047c 0164 0075 0172 047c 0164 0119  .r.|.d.u.r.|.d..
-00001c00: 0091 0271 0453 0029 024e 7267 0000 0072  ...q.S.).Nrg...r
-00001c10: 3600 0000 a902 726b 0000 00da 0178 7236  6.....rk.....xr6
-00001c20: 0000 0072 3600 0000 7237 0000 0072 6d00  ...r6...r7...rm.
-00001c30: 0000 e300 0000 726e 0000 0063 0100 0000  ......rn...c....
-00001c40: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00001c50: 5300 0000 7320 0000 0067 007c 005d 187d  S...s ...g.|.].}
-00001c60: 017c 0172 047c 0164 0075 0172 047c 0164  .|.r.|.d.u.r.|.d
-00001c70: 0119 0091 0271 0453 0029 024e 7203 0000  .....q.S.).Nr...
-00001c80: 0072 3600 0000 7274 0000 0072 3600 0000  .r6...rt...r6...
-00001c90: 7236 0000 0072 3700 0000 726d 0000 00e5  r6...r7...rm....
-00001ca0: 0000 0072 6e00 0000 7a25 4e6f 2073 796e  ...rn...z%No syn
-00001cb0: 6f6e 796d 7320 7765 7265 2066 6f75 6e64  onyms were found
-00001cc0: 2066 6f72 2074 6865 2077 6f72 643a 207a   for the word: z
-00001cd0: 3320 0a50 6c65 6173 6520 7665 7269 6679  3 .Please verify
-00001ce0: 2074 6861 7420 7468 6520 776f 7264 2069   that the word i
-00001cf0: 7320 7370 656c 6c65 6420 636f 7272 6563  s spelled correc
-00001d00: 746c 792e 6301 0000 0000 0000 0000 0000  tly.c...........
-00001d10: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
-00001d20: 0000 6700 7c00 5d0c 7d01 7c01 a000 a100  ..g.|.].}.|.....
-00001d30: 9102 7104 5300 7236 0000 0072 6800 0000  ..q.S.r6...rh...
-00001d40: 726a 0000 0072 3600 0000 7236 0000 0072  rj...r6...r6...r
-00001d50: 3700 0000 726d 0000 00ef 0000 0072 6e00  7...rm.......rn.
-00001d60: 0000 4e29 1472 2d00 0000 722e 0000 0072  ..N).r-...r....r
-00001d70: 3a00 0000 720b 0000 0072 4300 0000 722b  :...r....rC...r+
-00001d80: 0000 0072 4700 0000 721b 0000 00da 046b  ...rG...r......k
-00001d90: 6579 7372 1600 0000 da1d 666c 6174 7465  eysr......flatte
-00001da0: 6e5f 6d75 6c74 6964 696d 656e 7369 6f6e  n_multidimension
-00001db0: 616c 5f6c 6973 74da 0676 616c 7565 73da  al_list..values.
-00001dc0: 0673 6f72 7465 64da 0373 6574 da03 6c65  .sorted..set..le
-00001dd0: 6e72 2400 0000 da05 6475 6d70 7372 6600  nr$.....dumpsrf.
-00001de0: 0000 725b 0000 00da 0f6e 6f72 6d61 6c69  ..r[.....normali
-00001df0: 7a65 5f73 7061 6365 2909 7232 0000 0072  ze_space).r2...r
-00001e00: 4200 0000 7246 0000 0072 7000 0000 7249  B...rF...rp...rI
-00001e10: 0000 00da 0b6f 7574 7075 745f 6469 6374  .....output_dict
-00001e20: da0b 6a73 6f6e 5f6f 626a 6563 74da 0d71  ..json_object..q
-00001e30: 7565 7279 5f72 6573 756c 7473 5a10 7379  uery_resultsZ.sy
-00001e40: 6e6f 6e79 6d73 5f72 6573 756c 7473 7236  nonyms_resultsr6
-00001e50: 0000 0072 3600 0000 7237 0000 0072 3100  ...r6...r7...r1.
-00001e60: 0000 b700 0000 7370 0000 0000 0f0c 010a  ......sp........
-00001e70: 010c ff0a 0408 0108 010a 010c ff0a 020a  ................
-00001e80: 0108 010e 0114 0116 010a 011a 010a 010a  ................
-00001e90: 0102 ff02 0102 ff0c 0204 010c 010a 010e  ................
-00001ea0: ff06 0204 fe06 0308 020e 0108 0218 020e  ................
-00001eb0: 010a 020a 0106 010a 010c ff08 040c 011a  ................
-00001ec0: 010c 010a 0102 ff02 0102 ff0c 0204 010c  ................
-00001ed0: 010a 010e ff06 0204 fe06 037a 1653 796e  ...........z.Syn
-00001ee0: 6f6e 796d 732e 6669 6e64 5f73 796e 6f6e  onyms.find_synon
-00001ef0: 796d 7363 0100 0000 0000 0000 0000 0000  ymsc............
-00001f00: 0e00 0000 0a00 0000 4300 0000 7396 0300  ........C...s...
-00001f10: 0090 027a 2a7c 00a0 0064 017c 006a 019b  ...z*|...d.|.j..
-00001f20: 009d 02a1 017d 017c 016a 0264 026b 0272  .....}.|.j.d.k.r
-00001f30: 3874 03a0 0464 037c 006a 019b 009d 02a1  8t...d.|.j......
-00001f40: 0101 0057 0064 0453 0074 057c 016a 0664  ...W.d.S.t.|.j.d
-00001f50: 0583 027d 0274 0764 067c 0283 02a0 08a1  ...}.t.d.|......
-00001f60: 007d 037c 0364 0775 0090 0172 4c7c 026a  .}.|.d.u...rL|.j
-00001f70: 0964 0864 097c 006a 019b 0064 0a9d 0364  .d.d.|.j...d...d
-00001f80: 0b8d 027d 047c 0472 9074 03a0 0464 037c  ...}.|.r.t...d.|
-00001f90: 006a 019b 009d 02a1 0101 0057 0064 0453  .j.........W.d.S
-00001fa0: 0064 0c7d 057c 02a0 0964 0d64 0e64 0f69  .d.}.|...d.d.d.i
-00001fb0: 01a1 0272 d47c 02a0 0964 0d64 0e64 0f69  ...r.|...d.d.d.i
-00001fc0: 01a1 027d 0674 0a7c 066a 0683 0164 106b  ...}.t.|.j...d.k
-00001fd0: 0372 d07c 066a 06a0 0b64 11a1 017d 056e  .r.|.j...d...}.n
-00001fe0: 0464 0c7d 0567 007d 077c 02a0 0964 1264  .d.}.g.}.|...d.d
-00001ff0: 0e64 1369 01a1 027d 087c 0890 0272 287c  .d.i...}.|...r(|
-00002000: 08a0 0c64 1264 0e64 1468 02a1 0244 005d  ...d.d.d.h...D.]
-00002010: 227d 097c 09a0 0d64 0d64 0e64 1569 01a1  "}.|...d.d.d.i..
-00002020: 027d 0a7c 07a0 0e7c 0a6a 06a1 0101 0090  .}.|...|.j......
-00002030: 0071 fe74 0f64 1664 1784 007c 0744 0083  .q.t.d.d...|.D..
-00002040: 0183 017d 0b7c 00a0 107c 057c 0ba1 0201  ...}.|...|.|....
-00002050: 007c 0b7c 0566 0257 0053 006e dc7c 0364  .|.|.f.W.S.n.|.d
-00002060: 1875 0090 0272 2864 0c7d 0574 1164 017c  .u...r(d.}.t.d.|
-00002070: 006a 019b 009d 0283 01a0 12a1 007d 0c7c  .j...........}.|
-00002080: 0ca0 0964 0d64 0e64 0f69 01a1 0290 0172  ...d.d.d.i.....r
-00002090: b27c 0ca0 0964 0d64 0e64 0f69 01a1 027d  .|...d.d.d.i...}
-000020a0: 0674 0a7c 066a 0683 0164 106b 0390 0172  .t.|.j...d.k...r
-000020b0: ae7c 066a 06a0 0b64 11a1 017d 056e 0464  .|.j...d...}.n.d
-000020c0: 0c7d 0567 007d 077c 0ca0 0964 1264 0e64  .}.g.}.|...d.d.d
-000020d0: 1369 01a1 027d 087c 0890 0272 287c 08a0  .i...}.|...r(|..
-000020e0: 0c64 1264 0e64 1468 02a1 0244 005d 227d  .d.d.d.h...D.]"}
-000020f0: 097c 09a0 0d64 0d64 0e64 1569 01a1 027d  .|...d.d.d.i...}
-00002100: 0a7c 07a0 0e7c 0a6a 06a1 0101 0090 0171  .|...|.j.......q
-00002110: dc74 0f64 1964 1784 007c 0744 0083 0183  .t.d.d...|.D....
-00002120: 017d 0b7c 00a0 107c 057c 0ba1 0201 007c  .}.|...|.|.....|
-00002130: 0b7c 0566 0257 0053 0057 0090 016e 6404  .|.f.W.S.W...nd.
-00002140: 0074 136a 1490 0279 7801 007d 0d01 007a  .t.j...yx..}...z
-00002150: 3074 03a0 1564 1aa1 0101 0074 03a0 1564  0t...d.....t...d
-00002160: 0ca0 1674 17a0 187c 0d6a 19a1 01a1 01a1  ...t...|.j......
-00002170: 0101 0057 0059 0064 047d 0d7e 0d90 016e  ...W.Y.d.}.~...n
-00002180: 2264 047d 0d7e 0d30 0004 0074 1a90 0279  "d.}.~.0...t...y
-00002190: be01 007d 0d01 007a 2e74 03a0 1564 1ba1  ...}...z.t...d..
-000021a0: 0101 0074 03a0 1564 0ca0 1674 17a0 187c  ...t...d...t...|
-000021b0: 0d6a 19a1 01a1 01a1 0101 0057 0059 0064  .j.........W.Y.d
-000021c0: 047d 0d7e 0d6e dc64 047d 0d7e 0d30 0004  .}.~.n.d.}.~.0..
-000021d0: 0074 1b90 0379 0401 007d 0d01 007a 2e74  .t...y...}...z.t
-000021e0: 03a0 1564 1ca1 0101 0074 03a0 1564 0ca0  ...d.....t...d..
-000021f0: 1674 17a0 187c 0d6a 19a1 01a1 01a1 0101  .t...|.j........
-00002200: 0057 0059 0064 047d 0d7e 0d6e 9664 047d  .W.Y.d.}.~.n.d.}
-00002210: 0d7e 0d30 0004 0074 1c90 0379 4a01 007d  .~.0...t...yJ..}
-00002220: 0d01 007a 2e74 03a0 1564 1da1 0101 0074  ...z.t...d.....t
-00002230: 03a0 1564 0ca0 1674 17a0 187c 0d6a 19a1  ...d...t...|.j..
-00002240: 01a1 01a1 0101 0057 0059 0064 047d 0d7e  .......W.Y.d.}.~
-00002250: 0d6e 5064 047d 0d7e 0d30 0004 0074 1d90  .nPd.}.~.0...t..
-00002260: 0379 9001 007d 0d01 007a 2e74 03a0 1564  .y...}...z.t...d
-00002270: 1ea1 0101 0074 03a0 1564 0ca0 1674 17a0  .....t...d...t..
-00002280: 187c 0d6a 19a1 01a1 01a1 0101 0057 0059  .|.j.........W.Y
-00002290: 0064 047d 0d7e 0d6e 0a64 047d 0d7e 0d30  .d.}.~.n.d.}.~.0
-000022a0: 0030 0064 0453 0029 1f61 ed02 0000 0a20  .0.d.S.).a..... 
-000022b0: 2020 2020 2020 2054 6869 7320 6675 6e63         This func
-000022c0: 7469 6f6e 2071 7565 7269 6573 2063 6f6c  tion queries col
-000022d0: 6c69 6e73 6469 6374 696f 6e61 7279 2e63  linsdictionary.c
-000022e0: 6f6d 2066 6f72 2073 796e 6f6e 796d 7320  om for synonyms 
-000022f0: 6173 736f 6369 6174 6564 0a20 2020 2020  associated.     
-00002300: 2020 2077 6974 6820 7468 6520 7370 6563     with the spec
-00002310: 6966 6963 2077 6f72 6420 7072 6f76 6964  ific word provid
-00002320: 6564 2074 6f20 7468 6520 436c 6173 7320  ed to the Class 
-00002330: 5379 6e6f 6e79 6d73 2e0a 0a20 2020 2020  Synonyms...     
-00002340: 2020 203a 7265 7475 726e 733a 0a20 2020     :returns:.   
-00002350: 2020 2020 2020 2020 2073 796e 6f6e 796d           synonym
-00002360: 733a 206c 6973 7420 6f66 2073 796e 6f6e  s: list of synon
-00002370: 796d 730a 0a20 2020 2020 2020 203a 7274  yms..        :rt
-00002380: 7970 653a 206c 6973 740a 0a20 2020 2020  ype: list..     
-00002390: 2020 203a 7261 6973 6573 3a0a 2020 2020     :raises:.    
-000023a0: 2020 2020 2020 2020 4174 7472 6962 7574          Attribut
-000023b0: 6545 7272 6f72 3a20 5261 6973 6564 2077  eError: Raised w
-000023c0: 6865 6e20 616e 2061 7474 7269 6275 7465  hen an attribute
-000023d0: 2072 6566 6572 656e 6365 206f 7220 6173   reference or as
-000023e0: 7369 676e 6d65 6e74 2066 6169 6c73 0a0a  signment fails..
-000023f0: 2020 2020 2020 2020 2020 2020 496e 6465              Inde
-00002400: 7845 7272 6f72 3a20 5261 6973 6564 2077  xError: Raised w
-00002410: 6865 6e20 6120 7365 7175 656e 6365 2073  hen a sequence s
-00002420: 7562 7363 7269 7074 2069 7320 6f75 7420  ubscript is out 
-00002430: 6f66 2072 616e 6765 0a0a 2020 2020 2020  of range..      
-00002440: 2020 2020 2020 4b65 7945 7272 6f72 3a20        KeyError: 
-00002450: 5261 6973 6564 2077 6865 6e20 6120 6d61  Raised when a ma
-00002460: 7070 696e 6720 2864 6963 7469 6f6e 6172  pping (dictionar
-00002470: 7929 206b 6579 2069 7320 6e6f 7420 666f  y) key is not fo
-00002480: 756e 6420 696e 2074 6865 2073 6574 206f  und in the set o
-00002490: 6620 6578 6973 7469 6e67 206b 6579 730a  f existing keys.
-000024a0: 0a20 2020 2020 2020 2020 2020 2054 7970  .            Typ
-000024b0: 6545 7272 6f72 3a20 5261 6973 6564 2077  eError: Raised w
-000024c0: 6865 6e20 616e 206f 7065 7261 7469 6f6e  hen an operation
-000024d0: 206f 7220 6675 6e63 7469 6f6e 2069 7320   or function is 
-000024e0: 6170 706c 6965 6420 746f 2061 6e20 6f62  applied to an ob
-000024f0: 6a65 6374 206f 6620 696e 6170 7072 6f70  ject of inapprop
-00002500: 7269 6174 6520 7479 7065 0a0a 2020 2020  riate type..    
-00002510: 2020 2020 2020 2020 6273 342e 4665 6174          bs4.Feat
-00002520: 7572 654e 6f74 466f 756e 643a 2072 6169  ureNotFound: rai
-00002530: 7365 6420 6279 2074 6865 2042 6561 7574  sed by the Beaut
-00002540: 6966 756c 536f 7570 2063 6f6e 7374 7275  ifulSoup constru
-00002550: 6374 6f72 2069 6620 6e6f 2070 6172 7365  ctor if no parse
-00002560: 7220 7769 7468 2074 6865 2072 6571 7565  r with the reque
-00002570: 7374 6564 2066 6561 7475 7265 730a 2020  sted features.  
-00002580: 2020 2020 2020 2020 2020 6973 2066 6f75            is fou
-00002590: 6e64 0a20 2020 2020 2020 207a 3f68 7474  nd.        z?htt
-000025a0: 7073 3a2f 2f77 7777 2e63 6f6c 6c69 6e73  ps://www.collins
-000025b0: 6469 6374 696f 6e61 7279 2e63 6f6d 2f64  dictionary.com/d
-000025c0: 6963 7469 6f6e 6172 792f 656e 676c 6973  ictionary/englis
-000025d0: 682d 7468 6573 6175 7275 732f e994 0100  h-thesaurus/....
-000025e0: 007a 3943 6f6c 6c69 6e73 2044 6963 7469  .z9Collins Dicti
-000025f0: 6f6e 6172 7920 6861 6420 6e6f 2073 796e  onary had no syn
-00002600: 6f6e 796d 2072 6566 6572 656e 6365 2066  onym reference f
-00002610: 6f72 2074 6865 2077 6f72 6420 4eda 046c  or the word N..l
-00002620: 786d 6c7a 2168 7474 7073 3a2f 2f77 7777  xmlz!https://www
-00002630: 2e63 6f6c 6c69 6e73 6469 6374 696f 6e61  .collinsdictiona
-00002640: 7279 2e63 6f6d 46da 0268 3175 1900 0000  ry.comF..h1u....
-00002650: 536f 7272 792c 206e 6f20 7265 7375 6c74  Sorry, no result
-00002660: 7320 666f 7220 e280 9c75 1d00 0000 e280  s for ...u......
-00002670: 9d20 696e 2074 6865 2045 6e67 6c69 7368  . in the English
-00002680: 2054 6865 7361 7572 7573 2ea9 01da 0474   Thesaurus.....t
-00002690: 6578 7472 1a00 0000 da04 7370 616e da05  extr......span..
-000026a0: 636c 6173 735a 0e68 6561 6465 7253 656e  classZ.headerSen
-000026b0: 7365 506f 7372 0300 0000 7a02 2829 da03  sePosr....z.()..
-000026c0: 6469 765a 0862 6c6f 636b 5379 6e7a 0d66  divZ.blockSynz.f
-000026d0: 6f72 6d20 7479 7065 2d73 796e 5a04 6f72  orm type-synZ.or
-000026e0: 7468 6301 0000 0000 0000 0000 0000 0002  thc.............
-000026f0: 0000 0004 0000 0053 0000 0073 1800 0000  .......S...s....
-00002700: 6700 7c00 5d10 7d01 7c01 a000 a100 a001  g.|.].}.|.......
-00002710: a100 9102 7104 5300 7236 0000 00a9 0272  ....q.S.r6.....r
-00002720: 6900 0000 da05 7374 7269 7072 7400 0000  i.....striprt...
-00002730: 7236 0000 0072 3600 0000 7237 0000 0072  r6...r6...r7...r
-00002740: 6d00 0000 3101 0000 726e 0000 007a 3653  m...1...rn...z6S
-00002750: 796e 6f6e 796d 732e 5f71 7565 7279 5f63  ynonyms._query_c
-00002760: 6f6c 6c69 6e73 5f64 6963 7469 6f6e 6172  ollins_dictionar
-00002770: 792e 3c6c 6f63 616c 733e 2e3c 6c69 7374  y.<locals>.<list
-00002780: 636f 6d70 3e54 6301 0000 0000 0000 0000  comp>Tc.........
-00002790: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
-000027a0: 1800 0000 6700 7c00 5d10 7d01 7c01 a000  ....g.|.].}.|...
-000027b0: a100 a001 a100 9102 7104 5300 7236 0000  ........q.S.r6..
-000027c0: 0072 8900 0000 7274 0000 0072 3600 0000  .r....rt...r6...
-000027d0: 7236 0000 0072 3700 0000 726d 0000 004a  r6...r7...rm...J
-000027e0: 0100 0072 6e00 0000 fa30 416e 2065 7272  ...rn....0An err
-000027f0: 6f72 206f 6363 7572 7265 6420 696e 2074  or occurred in t
-00002800: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f64  he following cod
-00002810: 6520 7365 676d 656e 743a fa39 416e 2041  e segment:.9An A
-00002820: 7474 7269 6275 7465 4572 726f 7220 6f63  ttributeError oc
-00002830: 6375 7272 6564 2069 6e20 7468 6520 666f  curred in the fo
-00002840: 6c6c 6f77 696e 6720 636f 6465 2073 6567  llowing code seg
-00002850: 6d65 6e74 3afa 3541 6e20 496e 6465 7845  ment:.5An IndexE
-00002860: 7272 6f72 206f 6363 7572 7265 6420 696e  rror occurred in
-00002870: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00002880: 6f64 6520 7365 676d 656e 743a fa32 4120  ode segment:.2A 
-00002890: 4b65 7945 7272 6f72 206f 6363 7572 7265  KeyError occurre
-000028a0: 6420 696e 2074 6865 2066 6f6c 6c6f 7769  d in the followi
-000028b0: 6e67 2063 6f64 6520 7365 676d 656e 743a  ng code segment:
-000028c0: fa33 4120 5479 7065 4572 726f 7220 6f63  .3A TypeError oc
-000028d0: 6375 7272 6564 2069 6e20 7468 6520 666f  curred in the fo
-000028e0: 6c6c 6f77 696e 6720 636f 6465 2073 6567  llowing code seg
-000028f0: 6d65 6e74 3a29 1e72 4f00 0000 722b 0000  ment:).rO...r+..
-00002900: 00da 0b73 7461 7475 735f 636f 6465 723b  ...status_coder;
-00002910: 0000 0072 3c00 0000 7204 0000 0072 8500  ...r<...r....r..
-00002920: 0000 7218 0000 00da 1863 6c6f 7564 666c  ..r......cloudfl
-00002930: 6172 655f 7072 6f74 6563 7465 645f 7572  are_protected_ur
-00002940: 6cda 0466 696e 6472 7b00 0000 728a 0000  l..findr{...r...
-00002950: 00da 0866 696e 645f 616c 6cda 0966 696e  ...find_all..fin
-00002960: 6443 6869 6c64 7258 0000 0072 7900 0000  dChildrX...ry...
-00002970: 724b 0000 0072 0a00 0000 da06 6279 7061  rK...r......bypa
-00002980: 7373 da03 6273 34da 0f46 6561 7475 7265  ss..bs4..Feature
-00002990: 4e6f 7446 6f75 6e64 7241 0000 0072 5b00  NotFoundrA...r[.
-000029a0: 0000 725c 0000 0072 5d00 0000 725e 0000  ..r\...r]...r^..
-000029b0: 00da 0e41 7474 7269 6275 7465 4572 726f  ...AttributeErro
-000029c0: 72da 0a49 6e64 6578 4572 726f 72da 084b  r..IndexError..K
-000029d0: 6579 4572 726f 72da 0954 7970 6545 7272  eyError..TypeErr
-000029e0: 6f72 290e 7232 0000 0072 4e00 0000 da04  or).r2...rN.....
-000029f0: 736f 7570 da15 636c 6f75 6466 6c61 7265  soup..cloudflare
-00002a00: 5f70 726f 7465 6374 696f 6e5a 0f6e 6f5f  _protectionZ.no_
-00002a10: 776f 7264 5f72 6573 756c 7473 da17 7061  word_results..pa
-00002a20: 7274 5f6f 665f 7370 6565 6368 5f63 6174  rt_of_speech_cat
-00002a30: 6567 6f72 795a 1274 6167 5f70 6172 745f  egoryZ.tag_part_
-00002a40: 6f66 5f73 7065 6563 6872 4900 0000 7280  of_speechrI...r.
-00002a50: 0000 005a 0773 7562 5f73 796e da05 6368  ...Z.sub_syn..ch
-00002a60: 696c 64da 0d73 796e 6f6e 796d 735f 6c69  ild..synonyms_li
-00002a70: 7374 5a0a 6672 6573 685f 736f 7570 7241  stZ.fresh_souprA
-00002a80: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
-00002a90: 0000 7252 0000 00fb 0000 0073 8200 0000  ..rR.......s....
-00002aa0: 0016 0401 1202 0a01 1201 0602 0c01 0401  ................
-00002ab0: 02ff 0802 0a01 0601 0cff 0602 0401 1201  ................
-00002ac0: 0602 0402 1001 1001 0e01 0e02 0402 0401  ................
-00002ad0: 1001 0601 1401 1001 1001 1201 0c01 0c02  ................
-00002ae0: 0a01 0402 0401 04ff 0c04 1201 1001 1001  ................
-00002af0: 0e02 0402 0401 1001 0601 1401 1001 1002  ................
-00002b00: 1201 0c01 1002 1201 0a01 2e01 1001 0a01  ................
-00002b10: 2c01 1001 0a01 2c01 1001 0a01 2c01 1001  ,.....,.....,...
-00002b20: 0a01 7a22 5379 6e6f 6e79 6d73 2e5f 7175  ..z"Synonyms._qu
-00002b30: 6572 795f 636f 6c6c 696e 735f 6469 6374  ery_collins_dict
-00002b40: 696f 6e61 7279 6301 0000 0000 0000 0000  ionaryc.........
-00002b50: 0000 000d 0000 000a 0000 0043 0000 0073  ...........C...s
-00002b60: 3203 0000 9001 7ac6 7c00 a000 6401 7c00  2.....z.|...d.|.
-00002b70: 6a01 9b00 9d02 a101 7d01 7c01 6a02 6402  j.......}.|.j.d.
-00002b80: 6b02 7238 7403 a004 6403 7c00 6a01 9b00  k.r8t...d.|.j...
-00002b90: 9d02 a101 0100 5700 6404 5300 7405 7c01  ......W.d.S.t.|.
-00002ba0: 6a06 6405 8302 7d02 7407 6406 7c02 8302  j.d...}.t.d.|...
-00002bb0: a008 a100 7d03 7c03 6407 7500 9001 72b4  ....}.|.d.u...r.
-00002bc0: 7409 a00a 6408 a101 7d04 7c02 6a0b 7c04  t...d...}.|.j.|.
-00002bd0: 6409 8d01 728a 7403 a004 6403 7c00 6a01  d...r.t...d.|.j.
-00002be0: 9b00 9d02 a101 0100 5700 6404 5300 7c02  ........W.d.S.|.
-00002bf0: a00b 640a 640b 640c 6901 a102 72b2 7403  ..d.d.d.i...r.t.
-00002c00: a004 6403 7c00 6a01 9b00 9d02 a101 0100  ..d.|.j.........
-00002c10: 5700 6404 5300 6700 7d05 640d 7d06 7c02  W.d.S.g.}.d.}.|.
-00002c20: a00c 640e a101 72f0 7c02 a00c 640e a101  ..d...r.|...d...
-00002c30: 7d07 740d 7c07 640f 1900 6a06 8301 640f  }.t.|.d...j...d.
-00002c40: 6b03 72ec 7c07 640f 1900 6a06 7d06 6e04  k.r.|.d...j.}.n.
-00002c50: 640d 7d06 7c02 a00b 6410 640b 6411 6901  d.}.|...d.d.d.i.
-00002c60: a102 9001 72c4 7c02 a00b 6410 640b 6411  ....r.|...d.d.d.
-00002c70: 6901 a102 7d08 7c08 6a06 a00e 6412 a101  i...}.|.j...d...
-00002c80: 9001 72a8 7c02 a00b 6413 640b 6414 6901  ..r.|...d.d.d.i.
-00002c90: a102 7d09 7c09 a00f 6415 640b 6416 6901  ..}.|...d.d.d.i.
-00002ca0: a102 4400 5d48 7d0a 7c0a a00b 6417 640b  ..D.]H}.|...d.d.
-00002cb0: 6418 6901 a102 9001 7368 7c0a a00b 6417  d.i.....sh|...d.
-00002cc0: 640b 6419 6901 a102 9001 7240 7c0a 6a0b  d.d.i.....r@|.j.
-00002cd0: 641a 641b 641c 8d02 7d0b 7c05 a010 7c0b  d.d.d...}.|...|.
-00002ce0: 6a06 a011 a100 a101 0100 9001 7140 7412  j...........q@t.
-00002cf0: 641d 641e 8400 7c05 4400 8301 8301 7d05  d.d...|.D.....}.
-00002d00: 7c00 a013 7c06 7c05 a102 0100 7c05 7c06  |...|.|.....|.|.
-00002d10: 6602 5700 5300 6e10 7c03 641b 7500 9001  f.W.S.n.|.d.u...
-00002d20: 72c4 5700 6404 5300 5700 9001 6e64 0400  r.W.d.S.W...nd..
-00002d30: 7414 6a15 9002 7914 0100 7d0c 0100 7a30  t.j...y...}...z0
-00002d40: 7403 a016 641f a101 0100 7403 a016 640d  t...d.....t...d.
-00002d50: a017 7418 a019 7c0c 6a1a a101 a101 a101  ..t...|.j.......
-00002d60: 0100 5700 5900 6404 7d0c 7e0c 9001 6e22  ..W.Y.d.}.~...n"
-00002d70: 6404 7d0c 7e0c 3000 0400 741b 9002 795a  d.}.~.0...t...yZ
-00002d80: 0100 7d0c 0100 7a2e 7403 a016 6420 a101  ..}...z.t...d ..
-00002d90: 0100 7403 a016 640d a017 7418 a019 7c0c  ..t...d...t...|.
-00002da0: 6a1a a101 a101 a101 0100 5700 5900 6404  j.........W.Y.d.
-00002db0: 7d0c 7e0c 6edc 6404 7d0c 7e0c 3000 0400  }.~.n.d.}.~.0...
-00002dc0: 741c 9002 79a0 0100 7d0c 0100 7a2e 7403  t...y...}...z.t.
-00002dd0: a016 6421 a101 0100 7403 a016 640d a017  ..d!....t...d...
-00002de0: 7418 a019 7c0c 6a1a a101 a101 a101 0100  t...|.j.........
-00002df0: 5700 5900 6404 7d0c 7e0c 6e96 6404 7d0c  W.Y.d.}.~.n.d.}.
-00002e00: 7e0c 3000 0400 741d 9002 79e6 0100 7d0c  ~.0...t...y...}.
-00002e10: 0100 7a2e 7403 a016 6422 a101 0100 7403  ..z.t...d"....t.
-00002e20: a016 640d a017 7418 a019 7c0c 6a1a a101  ..d...t...|.j...
-00002e30: a101 a101 0100 5700 5900 6404 7d0c 7e0c  ......W.Y.d.}.~.
-00002e40: 6e50 6404 7d0c 7e0c 3000 0400 741e 9003  nPd.}.~.0...t...
-00002e50: 792c 0100 7d0c 0100 7a2e 7403 a016 6423  y,..}...z.t...d#
-00002e60: a101 0100 7403 a016 640d a017 7418 a019  ....t...d...t...
-00002e70: 7c0c 6a1a a101 a101 a101 0100 5700 5900  |.j.........W.Y.
-00002e80: 6404 7d0c 7e0c 6e0a 6404 7d0c 7e0c 3000  d.}.~.n.d.}.~.0.
-00002e90: 3000 6404 5300 2924 61f2 0200 000a 2020  0.d.S.)$a.....  
-00002ea0: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
-00002eb0: 696f 6e20 7175 6572 6965 7320 6d65 7272  ion queries merr
-00002ec0: 6961 6d2d 7765 6273 7465 722e 636f 6d20  iam-webster.com 
-00002ed0: 666f 7220 7379 6e6f 6e79 6d73 2061 7373  for synonyms ass
-00002ee0: 6f63 6961 7465 640a 2020 2020 2020 2020  ociated.        
-00002ef0: 7769 7468 2074 6865 2073 7065 6369 6669  with the specifi
-00002f00: 6320 776f 7264 2070 726f 7669 6465 6420  c word provided 
-00002f10: 746f 2074 6865 2043 6c61 7373 2053 796e  to the Class Syn
-00002f20: 6f6e 796d 732e 0a0a 2020 2020 2020 2020  onyms...        
-00002f30: 3a72 6574 7572 6e73 3a0a 2020 2020 2020  :returns:.      
-00002f40: 2020 2020 2020 7379 6e6f 6e79 6d73 3a20        synonyms: 
-00002f50: 6c69 7374 206f 6620 7379 6e6f 6e79 6d73  list of synonyms
-00002f60: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-00002f70: 3a20 6c69 7374 206f 7220 4e6f 6e65 0a0a  : list or None..
-00002f80: 2020 2020 2020 2020 3a72 6169 7365 733a          :raises:
-00002f90: 0a20 2020 2020 2020 2020 2020 4174 7472  .           Attr
-00002fa0: 6962 7574 6545 7272 6f72 3a20 5261 6973  ibuteError: Rais
-00002fb0: 6564 2077 6865 6e20 616e 2061 7474 7269  ed when an attri
-00002fc0: 6275 7465 2072 6566 6572 656e 6365 206f  bute reference o
-00002fd0: 7220 6173 7369 676e 6d65 6e74 2066 6169  r assignment fai
-00002fe0: 6c73 0a0a 2020 2020 2020 2020 2020 2020  ls..            
-00002ff0: 496e 6465 7845 7272 6f72 3a20 5261 6973  IndexError: Rais
-00003000: 6564 2077 6865 6e20 6120 7365 7175 656e  ed when a sequen
-00003010: 6365 2073 7562 7363 7269 7074 2069 7320  ce subscript is 
-00003020: 6f75 7420 6f66 2072 616e 6765 0a0a 2020  out of range..  
-00003030: 2020 2020 2020 2020 2020 4b65 7945 7272            KeyErr
-00003040: 6f72 3a20 5261 6973 6564 2077 6865 6e20  or: Raised when 
-00003050: 6120 6d61 7070 696e 6720 2864 6963 7469  a mapping (dicti
-00003060: 6f6e 6172 7929 206b 6579 2069 7320 6e6f  onary) key is no
-00003070: 7420 666f 756e 6420 696e 2074 6865 2073  t found in the s
-00003080: 6574 206f 6620 6578 6973 7469 6e67 206b  et of existing k
-00003090: 6579 730a 0a20 2020 2020 2020 2020 2020  eys..           
-000030a0: 2054 7970 6545 7272 6f72 3a20 5261 6973   TypeError: Rais
-000030b0: 6564 2077 6865 6e20 616e 206f 7065 7261  ed when an opera
-000030c0: 7469 6f6e 206f 7220 6675 6e63 7469 6f6e  tion or function
-000030d0: 2069 7320 6170 706c 6965 6420 746f 2061   is applied to a
-000030e0: 6e20 6f62 6a65 6374 206f 6620 696e 6170  n object of inap
-000030f0: 7072 6f70 7269 6174 6520 7479 7065 0a0a  propriate type..
-00003100: 2020 2020 2020 2020 2020 2020 6273 342e              bs4.
-00003110: 4665 6174 7572 654e 6f74 466f 756e 643a  FeatureNotFound:
-00003120: 2072 6169 7365 6420 6279 2074 6865 2042   raised by the B
-00003130: 6561 7574 6966 756c 536f 7570 2063 6f6e  eautifulSoup con
-00003140: 7374 7275 6374 6f72 2069 6620 6e6f 2070  structor if no p
-00003150: 6172 7365 7220 7769 7468 2074 6865 2072  arser with the r
-00003160: 6571 7565 7374 6564 2066 6561 7475 7265  equested feature
-00003170: 730a 2020 2020 2020 2020 2020 2020 6973  s.            is
-00003180: 2066 6f75 6e64 0a20 2020 2020 2020 207a   found.        z
-00003190: 2a68 7474 7073 3a2f 2f77 7777 2e6d 6572  *https://www.mer
-000031a0: 7269 616d 2d77 6562 7374 6572 2e63 6f6d  riam-webster.com
-000031b0: 2f74 6865 7361 7572 7573 2f72 8100 0000  /thesaurus/r....
-000031c0: 7a3a 4d65 7272 6961 6d2d 7765 6273 7465  z:Merriam-webste
-000031d0: 722e 636f 6d20 6861 6420 6e6f 2073 796e  r.com had no syn
-000031e0: 6f6e 796d 2072 6566 6572 656e 6365 2066  onym reference f
-000031f0: 6f72 2074 6865 2077 6f72 6420 4e72 8200  or the word Nr..
-00003200: 0000 7a1f 6874 7470 733a 2f2f 7777 772e  ..z.https://www.
-00003210: 6d65 7272 6961 6d2d 7765 6273 7465 722e  merriam-webster.
-00003220: 636f 6d46 7a0d 576f 7264 7320 6661 696c  comFz.Words fail
-00003230: 2075 7372 8400 0000 7283 0000 0072 8700   usr....r....r..
-00003240: 0000 7a0e 6d69 7370 656c 6c65 642d 776f  ..z.mispelled-wo
-00003250: 7264 721a 0000 007a 6e23 7468 6573 6175  rdr....zn#thesau
-00003260: 7275 732d 656e 7472 792d 312d 3120 3e20  rus-entry-1-1 > 
-00003270: 6469 762e 726f 772e 656e 7472 792d 6865  div.row.entry-he
-00003280: 6164 6572 203e 2064 6976 203e 2064 6976  ader > div > div
-00003290: 203e 2064 6976 2e61 6c69 676e 2d69 7465   > div.align-ite
-000032a0: 6d73 2d62 6173 656c 696e 652e 642d 666c  ms-baseline.d-fl
-000032b0: 6578 2e66 6c65 782d 6772 6f77 2d31 203e  ex.flex-grow-1 >
-000032c0: 2068 3220 3e20 6172 0300 0000 da01 707a   h2 > ar......pz
-000032d0: 0e66 756e 6374 696f 6e2d 6c61 6265 6c72  .function-labelr
-000032e0: 1900 0000 7288 0000 007a 1f74 6865 732d  ....r....z.thes-
-000032f0: 6c69 7374 2d63 6f6e 7465 6e74 2073 796e  list-content syn
-00003300: 6f6e 796d 735f 6c69 7374 da02 6c69 7a13  onyms_list..liz.
-00003310: 7468 6573 2d77 6f72 642d 6c69 7374 2d69  thes-word-list-i
-00003320: 7465 6d72 8600 0000 7a0f 6c6f 7a65 6e67  temr....z.lozeng
-00003330: 6520 636f 6c6f 722d 347a 0f6c 6f7a 656e  e color-4z.lozen
-00003340: 6765 2063 6f6c 6f72 2d33 da01 6154 a901  ge color-3..aT..
-00003350: da04 6872 6566 6301 0000 0000 0000 0000  ..hrefc.........
-00003360: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
-00003370: 1800 0000 6700 7c00 5d10 7d01 7c01 a000  ....g.|.].}.|...
-00003380: a100 a001 a100 9102 7104 5300 7236 0000  ........q.S.r6..
-00003390: 0072 8900 0000 7274 0000 0072 3600 0000  .r....rt...r6...
-000033a0: 7236 0000 0072 3700 0000 726d 0000 009d  r6...r7...rm....
-000033b0: 0100 0072 6e00 0000 7a33 5379 6e6f 6e79  ...rn...z3Synony
-000033c0: 6d73 2e5f 7175 6572 795f 6d65 7272 6961  ms._query_merria
-000033d0: 6d5f 7765 6273 7465 722e 3c6c 6f63 616c  m_webster.<local
-000033e0: 733e 2e3c 6c69 7374 636f 6d70 3e72 8b00  s>.<listcomp>r..
-000033f0: 0000 728c 0000 0072 8d00 0000 728e 0000  ..r....r....r...
-00003400: 0072 8f00 0000 291f 724f 0000 0072 2b00  .r....).rO...r+.
-00003410: 0000 7290 0000 0072 3b00 0000 723c 0000  ..r....r;...r<..
-00003420: 0072 0400 0000 7285 0000 0072 1800 0000  .r....r....r....
-00003430: 7291 0000 00da 0572 6567 6578 da07 636f  r......regex..co
-00003440: 6d70 696c 6572 9200 0000 da06 7365 6c65  mpiler......sele
-00003450: 6374 727b 0000 00da 0a73 7461 7274 7377  ctr{.....startsw
-00003460: 6974 6872 9300 0000 7258 0000 0072 8a00  ithr....rX...r..
-00003470: 0000 7279 0000 0072 4b00 0000 7296 0000  ..ry...rK...r...
-00003480: 0072 9700 0000 7241 0000 0072 5b00 0000  .r....rA...r[...
-00003490: 725c 0000 0072 5d00 0000 725e 0000 0072  r\...r]...r^...r
-000034a0: 9800 0000 7299 0000 0072 9a00 0000 729b  ....r....r....r.
-000034b0: 0000 0029 0d72 3200 0000 724e 0000 0072  ...).r2...rN...r
-000034c0: 9c00 0000 729d 0000 00da 0770 6174 7465  ....r......patte
-000034d0: 726e 72a0 0000 0072 9e00 0000 da12 6373  rnr....r......cs
-000034e0: 735f 7061 7274 5f6f 665f 7370 6565 6368  s_part_of_speech
-000034f0: da05 6c61 6265 6cda 0e77 6f72 645f 636f  ..label..word_co
-00003500: 6e74 6169 6e65 72da 096c 6973 745f 6974  ntainer..list_it
-00003510: 656d da04 6c69 6e6b 7241 0000 0072 3600  em..linkrA...r6.
-00003520: 0000 7236 0000 0072 3700 0000 7253 0000  ..r6...r7...rS..
-00003530: 005f 0100 0073 7000 0000 0016 0401 1202  ._...sp.........
-00003540: 0a01 1201 0602 0c01 0401 02ff 0802 0a01  ................
-00003550: 0a01 0c01 1201 0601 1001 1201 0602 0401  ................
-00003560: 0403 0a01 0401 02ff 0402 1201 0c02 0402  ................
-00003570: 1201 1001 0e01 1001 1401 1201 0eff 0402  ................
-00003580: 0e01 1401 1201 0c01 0c01 0a01 0c02 1201  ................
-00003590: 0a01 2e01 1001 0a01 2c01 1001 0a01 2c01  ........,.....,.
-000035a0: 1001 0a01 2c01 1001 0a01 7a1f 5379 6e6f  ....,.....z.Syno
-000035b0: 6e79 6d73 2e5f 7175 6572 795f 6d65 7272  nyms._query_merr
-000035c0: 6961 6d5f 7765 6273 7465 7263 0100 0000  iam_websterc....
-000035d0: 0000 0000 0000 0000 0c00 0000 0a00 0000  ................
-000035e0: 4300 0000 73f0 0200 0090 017a 847c 00a0  C...s......z.|..
-000035f0: 0064 017c 006a 019b 009d 02a1 017d 017c  .d.|.j.......}.|
-00003600: 016a 0264 026b 0272 3874 03a0 0464 037c  .j.d.k.r8t...d.|
-00003610: 006a 019b 009d 02a1 0101 0057 0064 0453  .j.........W.d.S
-00003620: 0074 057c 016a 0664 0583 027d 0274 0764  .t.|.j.d...}.t.d
-00003630: 067c 0283 02a0 08a1 007d 037c 0364 0775  .|.......}.|.d.u
-00003640: 0090 0172 727c 02a0 0964 0864 0964 0a69  ...rr|...d.d.d.i
-00003650: 01a1 027d 0474 0aa0 0b64 0ba1 017d 057c  ...}.t...d...}.|
-00003660: 026a 097c 0564 0c8d 0172 9a74 03a0 0464  .j.|.d...r.t...d
-00003670: 037c 006a 019b 009d 02a1 0101 0057 0064  .|.j.........W.d
-00003680: 0453 007c 046a 0c64 0d19 0064 0e6b 0290  .S.|.j.d...d.k..
-00003690: 0172 8264 0f7d 067c 02a0 0964 1064 1164  .r.d.}.|...d.d.d
-000036a0: 1269 01a1 0290 0172 587c 02a0 0964 1064  .i.....rX|...d.d
-000036b0: 1164 1269 01a1 027d 0764 1364 1484 007c  .d.i...}.d.d...|
-000036c0: 07a0 0964 1564 1664 1769 01a1 02a0 0d64  ...d.d.d.i.....d
-000036d0: 18a1 0144 0083 017d 0874 0e64 1964 1484  ...D...}.t.d.d..
-000036e0: 007c 0844 0083 0183 017d 097c 02a0 0f64  .|.D.....}.|...d
-000036f0: 1aa1 0190 0172 427c 02a0 0f64 1aa1 017d  .....rB|...d...}
-00003700: 0a74 107c 0a64 1b19 006a 0683 0164 1b6b  .t.|.d...j...d.k
-00003710: 0390 0172 3e7c 0a64 1b19 006a 06a0 1164  ...r>|.d...j...d
-00003720: 1ca1 017d 066e 0464 0f7d 067c 00a0 127c  ...}.n.d.}.|...|
-00003730: 067c 09a1 0201 007c 097c 0666 0257 0053  .|.....|.|.f.W.S
-00003740: 0074 03a0 0464 037c 006a 019b 009d 02a1  .t...d.|.j......
-00003750: 0101 0057 0064 0453 006e 107c 0364 1d75  ...W.d.S.n.|.d.u
-00003760: 0090 0172 8257 0064 0453 0057 0090 016e  ...r.W.d.S.W...n
-00003770: 6404 0074 136a 1490 0179 d201 007d 0b01  d..t.j...y...}..
-00003780: 007a 3074 03a0 1564 1ea1 0101 0074 03a0  .z0t...d.....t..
-00003790: 1564 0fa0 1674 17a0 187c 0b6a 19a1 01a1  .d...t...|.j....
-000037a0: 01a1 0101 0057 0059 0064 047d 0b7e 0b90  .....W.Y.d.}.~..
-000037b0: 016e 2264 047d 0b7e 0b30 0004 0074 1a90  .n"d.}.~.0...t..
-000037c0: 0279 1801 007d 0b01 007a 2e74 03a0 1564  .y...}...z.t...d
-000037d0: 1fa1 0101 0074 03a0 1564 0fa0 1674 17a0  .....t...d...t..
-000037e0: 187c 0b6a 19a1 01a1 01a1 0101 0057 0059  .|.j.........W.Y
-000037f0: 0064 047d 0b7e 0b6e dc64 047d 0b7e 0b30  .d.}.~.n.d.}.~.0
-00003800: 0004 0074 1b90 0279 5e01 007d 0b01 007a  ...t...y^..}...z
-00003810: 2e74 03a0 1564 20a1 0101 0074 03a0 1564  .t...d ....t...d
-00003820: 0fa0 1674 17a0 187c 0b6a 19a1 01a1 01a1  ...t...|.j......
-00003830: 0101 0057 0059 0064 047d 0b7e 0b6e 9664  ...W.Y.d.}.~.n.d
-00003840: 047d 0b7e 0b30 0004 0074 1c90 0279 a401  .}.~.0...t...y..
-00003850: 007d 0b01 007a 2e74 03a0 1564 21a1 0101  .}...z.t...d!...
-00003860: 0074 03a0 1564 0fa0 1674 17a0 187c 0b6a  .t...d...t...|.j
-00003870: 19a1 01a1 01a1 0101 0057 0059 0064 047d  .........W.Y.d.}
-00003880: 0b7e 0b6e 5064 047d 0b7e 0b30 0004 0074  .~.nPd.}.~.0...t
-00003890: 1d90 0279 ea01 007d 0b01 007a 2e74 03a0  ...y...}...z.t..
-000038a0: 1564 22a1 0101 0074 03a0 1564 0fa0 1674  .d"....t...d...t
-000038b0: 17a0 187c 0b6a 19a1 01a1 01a1 0101 0057  ...|.j.........W
-000038c0: 0059 0064 047d 0b7e 0b6e 0a64 047d 0b7e  .Y.d.}.~.n.d.}.~
-000038d0: 0b30 0030 0064 0453 0029 2361 ec02 0000  .0.0.d.S.)#a....
-000038e0: 0a20 2020 2020 2020 2054 6869 7320 6675  .        This fu
-000038f0: 6e63 7469 6f6e 2071 7565 7269 6573 2073  nction queries s
-00003900: 796e 6f6e 796d 2e63 6f6d 2066 6f72 2073  ynonym.com for s
-00003910: 796e 6f6e 796d 7320 6173 736f 6369 6174  ynonyms associat
-00003920: 6564 0a20 2020 2020 2020 2077 6974 6820  ed.        with 
-00003930: 7468 6520 7370 6563 6966 6963 2077 6f72  the specific wor
-00003940: 6420 7072 6f76 6964 6564 2074 6f20 7468  d provided to th
-00003950: 6520 436c 6173 7320 5379 6e6f 6e79 6d73  e Class Synonyms
-00003960: 2e0a 0a20 2020 2020 2020 2020 3a72 6574  ...         :ret
-00003970: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00003980: 2020 7379 6e6f 6e79 6d73 3a20 6c69 7374    synonyms: list
-00003990: 206f 6620 7379 6e6f 6e79 6d73 0a0a 2020   of synonyms..  
-000039a0: 2020 2020 2020 3a72 7479 7065 3a20 6c69        :rtype: li
-000039b0: 7374 206f 7220 4e6f 6e65 0a0a 2020 2020  st or None..    
-000039c0: 2020 2020 3a72 6169 7365 733a 0a20 2020      :raises:.   
-000039d0: 2020 2020 2020 2020 2041 7474 7269 6275           Attribu
-000039e0: 7465 4572 726f 723a 2052 6169 7365 6420  teError: Raised 
-000039f0: 7768 656e 2061 6e20 6174 7472 6962 7574  when an attribut
-00003a00: 6520 7265 6665 7265 6e63 6520 6f72 2061  e reference or a
-00003a10: 7373 6967 6e6d 656e 7420 6661 696c 730a  ssignment fails.
-00003a20: 0a20 2020 2020 2020 2020 2020 2049 6e64  .            Ind
-00003a30: 6578 4572 726f 723a 2052 6169 7365 6420  exError: Raised 
-00003a40: 7768 656e 2061 2073 6571 7565 6e63 6520  when a sequence 
-00003a50: 7375 6273 6372 6970 7420 6973 206f 7574  subscript is out
-00003a60: 206f 6620 7261 6e67 650a 0a20 2020 2020   of range..     
-00003a70: 2020 2020 2020 204b 6579 4572 726f 723a         KeyError:
-00003a80: 2052 6169 7365 6420 7768 656e 2061 206d   Raised when a m
-00003a90: 6170 7069 6e67 2028 6469 6374 696f 6e61  apping (dictiona
-00003aa0: 7279 2920 6b65 7920 6973 206e 6f74 2066  ry) key is not f
-00003ab0: 6f75 6e64 2069 6e20 7468 6520 7365 7420  ound in the set 
-00003ac0: 6f66 2065 7869 7374 696e 6720 6b65 7973  of existing keys
-00003ad0: 0a0a 2020 2020 2020 2020 2020 2020 5479  ..            Ty
-00003ae0: 7065 4572 726f 723a 2052 6169 7365 6420  peError: Raised 
-00003af0: 7768 656e 2061 6e20 6f70 6572 6174 696f  when an operatio
-00003b00: 6e20 6f72 2066 756e 6374 696f 6e20 6973  n or function is
-00003b10: 2061 7070 6c69 6564 2074 6f20 616e 206f   applied to an o
-00003b20: 626a 6563 7420 6f66 2069 6e61 7070 726f  bject of inappro
-00003b30: 7072 6961 7465 2074 7970 650a 0a20 2020  priate type..   
-00003b40: 2020 2020 2020 2020 2062 7334 2e46 6561           bs4.Fea
-00003b50: 7475 7265 4e6f 7446 6f75 6e64 3a20 7261  tureNotFound: ra
-00003b60: 6973 6564 2062 7920 7468 6520 4265 6175  ised by the Beau
-00003b70: 7469 6675 6c53 6f75 7020 636f 6e73 7472  tifulSoup constr
-00003b80: 7563 746f 7220 6966 206e 6f20 7061 7273  uctor if no pars
-00003b90: 6572 2077 6974 6820 7468 6520 7265 7175  er with the requ
-00003ba0: 6573 7465 6420 6665 6174 7572 6573 0a20  ested features. 
-00003bb0: 2020 2020 2020 2020 2020 2069 7320 666f             is fo
-00003bc0: 756e 640a 2020 2020 2020 2020 7a21 6874  und.        z!ht
-00003bd0: 7470 733a 2f2f 7777 772e 7379 6e6f 6e79  tps://www.synony
-00003be0: 6d2e 636f 6d2f 7379 6e6f 6e79 6d73 2f72  m.com/synonyms/r
-00003bf0: 8100 0000 7a32 5379 6e6f 6e79 6d2e 636f  ....z2Synonym.co
-00003c00: 6d20 6861 6420 6e6f 2073 796e 6f6e 796d  m had no synonym
-00003c10: 2072 6566 6572 656e 6365 2066 6f72 2074   reference for t
-00003c20: 6865 2077 6f72 6420 4e72 8200 0000 7a17  he word Nr....z.
-00003c30: 6874 7470 733a 2f2f 7777 772e 7379 6e6f  https://www.syno
-00003c40: 6e79 6d2e 636f 6d46 da04 6d65 7461 da04  nym.comF..meta..
-00003c50: 6e61 6d65 5a08 7061 6765 7479 7065 7a0a  nameZ.pagetypez.
-00003c60: 4f6f 7073 2c20 3430 3421 7284 0000 00da  Oops, 404!r.....
-00003c70: 0763 6f6e 7465 6e74 5a04 5465 726d 721a  .contentZ.Termr.
-00003c80: 0000 0072 8800 0000 7a0c 6461 7461 2d73  ...r....z.data-s
-00003c90: 6563 7469 6f6e 7249 0000 0063 0100 0000  ectionrI...c....
-00003ca0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00003cb0: 5300 0000 7312 0000 0067 007c 005d 0a7d  S...s....g.|.].}
-00003cc0: 017c 016a 0091 0271 0453 0072 3600 0000  .|.j...q.S.r6...
-00003cd0: 7284 0000 0072 6a00 0000 7236 0000 0072  r....rj...r6...r
-00003ce0: 3600 0000 7237 0000 0072 6d00 0000 df01  6...r7...rm.....
-00003cf0: 0000 726e 0000 007a 2f53 796e 6f6e 796d  ..rn...z/Synonym
-00003d00: 732e 5f71 7565 7279 5f73 796e 6f6e 796d  s._query_synonym
-00003d10: 5f63 6f6d 2e3c 6c6f 6361 6c73 3e2e 3c6c  _com.<locals>.<l
-00003d20: 6973 7463 6f6d 703e da02 756c 7287 0000  istcomp>..ulr...
-00003d30: 007a 0c73 6563 7469 6f6e 2d6c 6973 7472  .z.section-listr
-00003d40: a200 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00003d50: 0002 0000 0004 0000 0053 0000 0073 1800  .........S...s..
-00003d60: 0000 6700 7c00 5d10 7d01 7c01 a000 a100  ..g.|.].}.|.....
-00003d70: a001 a100 9102 7104 5300 7236 0000 0072  ......q.S.r6...r
-00003d80: 8900 0000 7274 0000 0072 3600 0000 7236  ....rt...r6...r6
-00003d90: 0000 0072 3700 0000 726d 0000 00e1 0100  ...r7...rm......
-00003da0: 0072 6e00 0000 7a7a 626f 6479 203e 2064  .rn...zzbody > d
-00003db0: 6976 2e70 6167 652d 636f 6e74 6169 6e65  iv.page-containe
-00003dc0: 7220 3e20 6469 762e 636f 6e74 656e 742d  r > div.content-
-00003dd0: 636f 6e74 6169 6e65 7220 3e20 6469 762e  container > div.
-00003de0: 6d61 696e 2d63 6f6c 756d 6e20 3e20 6469  main-column > di
-00003df0: 762e 7365 6374 696f 6e73 2d77 7261 7070  v.sections-wrapp
-00003e00: 6572 203e 2064 6976 3a6e 7468 2d63 6869  er > div:nth-chi
-00003e10: 6c64 2831 2920 3e20 7020 3e20 7374 726f  ld(1) > p > stro
-00003e20: 6e67 7203 0000 00da 012e 5472 8b00 0000  ngr.......Tr....
-00003e30: 728c 0000 0072 8d00 0000 728e 0000 0072  r....r....r....r
-00003e40: 8f00 0000 291e 724f 0000 0072 2b00 0000  ....).rO...r+...
-00003e50: 7290 0000 0072 3b00 0000 723c 0000 0072  r....r;...r<...r
-00003e60: 0400 0000 7285 0000 0072 1800 0000 7291  ....r....r....r.
-00003e70: 0000 0072 9200 0000 72a6 0000 0072 a700  ...r....r....r..
-00003e80: 0000 da05 6174 7472 7372 9300 0000 7279  ....attrsr....ry
-00003e90: 0000 0072 a800 0000 727b 0000 0072 8a00  ...r....r{...r..
-00003ea0: 0000 724b 0000 0072 9600 0000 7297 0000  ..rK...r....r...
-00003eb0: 0072 4100 0000 725b 0000 0072 5c00 0000  .rA...r[...r\...
-00003ec0: 725d 0000 0072 5e00 0000 7298 0000 0072  r]...r^...r....r
-00003ed0: 9900 0000 729a 0000 0072 9b00 0000 290c  ....r....r....).
-00003ee0: 7232 0000 0072 4e00 0000 729c 0000 0072  r2...rN...r....r
-00003ef0: 9d00 0000 da0a 7374 6174 7573 5f74 6167  ......status_tag
-00003f00: 72aa 0000 0072 9e00 0000 5a0e 7379 6e6f  r....r....Z.syno
-00003f10: 6e79 6d73 5f63 6c61 7373 7249 0000 0072  nyms_classrI...r
-00003f20: a000 0000 72ab 0000 0072 4100 0000 7236  ....r....rA...r6
-00003f30: 0000 0072 3600 0000 7237 0000 0072 5400  ...r6...r7...rT.
-00003f40: 0000 b401 0000 7366 0000 0000 1604 0112  ......sf........
-00003f50: 020a 0112 0106 020c 0104 0102 ff08 020a  ................
-00003f60: 0110 010a 010c 0112 0106 0110 0104 0212  ................
-00003f70: 0110 0106 0114 ff06 0212 030c 0104 0102  ................
-00003f80: ff04 0214 0112 0204 020c 010a 0212 0108  ................
-00003f90: 010a 010c 0212 010a 012e 0110 010a 012c  ...............,
-00003fa0: 0110 010a 012c 0110 010a 012c 0110 010a  .....,.....,....
-00003fb0: 017a 1b53 796e 6f6e 796d 732e 5f71 7565  .z.Synonyms._que
-00003fc0: 7279 5f73 796e 6f6e 796d 5f63 6f6d 6301  ry_synonym_comc.
-00003fd0: 0000 0000 0000 0000 0000 000c 0000 000a  ................
-00003fe0: 0000 0043 0000 0073 be02 0000 9001 7a52  ...C...s......zR
-00003ff0: 7c00 a000 6401 7c00 6a01 9b00 9d02 a101  |...d.|.j.......
-00004000: 7d01 7c01 6a02 6402 6b02 7238 7403 a004  }.|.j.d.k.r8t...
-00004010: 6403 7c00 6a01 9b00 9d02 a101 0100 5700  d.|.j.........W.
-00004020: 6404 5300 7405 7c01 6a06 6405 8302 7d02  d.S.t.|.j.d...}.
-00004030: 7407 6406 7c02 8302 a008 a100 7d03 7c03  t.d.|.......}.|.
-00004040: 6407 7500 9001 7240 7c02 a009 6408 a101  d.u...r@|...d...
-00004050: 7d04 7c04 6a06 a00a 6409 a101 728a 7403  }.|.j...d...r.t.
-00004060: a004 6403 7c00 6a01 9b00 9d02 a101 0100  ..d.|.j.........
-00004070: 5700 6404 5300 6700 7d05 640a 7d06 7c02  W.d.S.g.}.d.}.|.
-00004080: a00b 640b a101 72c8 7c02 a00b 640b a101  ..d...r.|...d...
-00004090: 7d07 740c 7c07 640c 1900 6a06 8301 640c  }.t.|.d...j...d.
-000040a0: 6b03 72c4 7c07 640c 1900 6a06 7d06 6e04  k.r.|.d...j.}.n.
-000040b0: 640a 7d06 7c02 a009 640d 640e 640f 6901  d.}.|...d.d.d.i.
-000040c0: a102 7d08 7c08 a009 6410 a101 a00d 6411  ..}.|...d.....d.
-000040d0: a101 4400 5d3e 7d09 7c09 a00d 6412 6413  ..D.]>}.|...d.d.
-000040e0: 6414 6901 a102 4400 5d16 7d0a 7c05 a00e  d.i...D.].}.|...
-000040f0: 7c0a 6a06 a00f a100 a101 0100 9000 71fc  |.j...........q.
-00004100: 7410 6415 6416 8400 7c05 4400 8301 8301  t.d.d...|.D.....
-00004110: 7d05 71e8 7c00 a011 7c06 7c05 a102 0100  }.q.|...|.|.....
-00004120: 7c05 7c06 6602 5700 5300 6e10 7c03 6417  |.|.f.W.S.n.|.d.
-00004130: 7500 9001 7250 5700 6404 5300 5700 9001  u...rPW.d.S.W...
-00004140: 6e64 0400 7412 6a13 9001 79a0 0100 7d0b  nd..t.j...y...}.
-00004150: 0100 7a30 7403 a014 6418 a101 0100 7403  ..z0t...d.....t.
-00004160: a014 640a a015 7416 a017 7c0b 6a18 a101  ..d...t...|.j...
-00004170: a101 a101 0100 5700 5900 6404 7d0b 7e0b  ......W.Y.d.}.~.
-00004180: 9001 6e22 6404 7d0b 7e0b 3000 0400 7419  ..n"d.}.~.0...t.
-00004190: 9001 79e6 0100 7d0b 0100 7a2e 7403 a014  ..y...}...z.t...
-000041a0: 6419 a101 0100 7403 a014 640a a015 7416  d.....t...d...t.
-000041b0: a017 7c0b 6a18 a101 a101 a101 0100 5700  ..|.j.........W.
-000041c0: 5900 6404 7d0b 7e0b 6edc 6404 7d0b 7e0b  Y.d.}.~.n.d.}.~.
-000041d0: 3000 0400 741a 9002 792c 0100 7d0b 0100  0...t...y,..}...
-000041e0: 7a2e 7403 a014 641a a101 0100 7403 a014  z.t...d.....t...
-000041f0: 640a a015 7416 a017 7c0b 6a18 a101 a101  d...t...|.j.....
-00004200: a101 0100 5700 5900 6404 7d0b 7e0b 6e96  ....W.Y.d.}.~.n.
-00004210: 6404 7d0b 7e0b 3000 0400 741b 9002 7972  d.}.~.0...t...yr
-00004220: 0100 7d0b 0100 7a2e 7403 a014 641b a101  ..}...z.t...d...
-00004230: 0100 7403 a014 640a a015 7416 a017 7c0b  ..t...d...t...|.
-00004240: 6a18 a101 a101 a101 0100 5700 5900 6404  j.........W.Y.d.
-00004250: 7d0b 7e0b 6e50 6404 7d0b 7e0b 3000 0400  }.~.nPd.}.~.0...
-00004260: 741c 9002 79b8 0100 7d0b 0100 7a2e 7403  t...y...}...z.t.
-00004270: a014 641c a101 0100 7403 a014 640a a015  ..d.....t...d...
-00004280: 7416 a017 7c0b 6a18 a101 a101 a101 0100  t...|.j.........
-00004290: 5700 5900 6404 7d0b 7e0b 6e0a 6404 7d0b  W.Y.d.}.~.n.d.}.
-000042a0: 7e0b 3000 3000 6404 5300 291d 61ed 0200  ~.0.0.d.S.).a...
-000042b0: 000a 2020 2020 2020 2020 5468 6973 2066  ..        This f
-000042c0: 756e 6374 696f 6e20 7175 6572 6965 7320  unction queries 
-000042d0: 7468 6573 6175 7275 732e 636f 6d20 666f  thesaurus.com fo
-000042e0: 7220 7379 6e6f 6e79 6d73 2061 7373 6f63  r synonyms assoc
-000042f0: 6961 7465 640a 2020 2020 2020 2020 7769  iated.        wi
-00004300: 7468 2074 6865 2073 7065 6369 6669 6320  th the specific 
-00004310: 776f 7264 2070 726f 7669 6465 6420 746f  word provided to
-00004320: 2074 6865 2043 6c61 7373 2053 796e 6f6e   the Class Synon
-00004330: 796d 732e 0a0a 2020 2020 2020 2020 3a72  yms...        :r
-00004340: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00004350: 2020 2020 7379 6e6f 6e79 6d73 3a20 6c69      synonyms: li
-00004360: 7374 206f 6620 7379 6e6f 6e79 6d73 0a0a  st of synonyms..
-00004370: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00004380: 6c69 7374 206f 7220 4e6f 6e65 0a0a 2020  list or None..  
-00004390: 2020 2020 2020 3a72 6169 7365 733a 0a20        :raises:. 
-000043a0: 2020 2020 2020 2020 2020 2041 7474 7269             Attri
-000043b0: 6275 7465 4572 726f 723a 2052 6169 7365  buteError: Raise
-000043c0: 6420 7768 656e 2061 6e20 6174 7472 6962  d when an attrib
-000043d0: 7574 6520 7265 6665 7265 6e63 6520 6f72  ute reference or
-000043e0: 2061 7373 6967 6e6d 656e 7420 6661 696c   assignment fail
-000043f0: 730a 0a20 2020 2020 2020 2020 2020 2049  s..            I
-00004400: 6e64 6578 4572 726f 723a 2052 6169 7365  ndexError: Raise
-00004410: 6420 7768 656e 2061 2073 6571 7565 6e63  d when a sequenc
-00004420: 6520 7375 6273 6372 6970 7420 6973 206f  e subscript is o
-00004430: 7574 206f 6620 7261 6e67 650a 0a20 2020  ut of range..   
-00004440: 2020 2020 2020 2020 204b 6579 4572 726f           KeyErro
-00004450: 723a 2052 6169 7365 6420 7768 656e 2061  r: Raised when a
-00004460: 206d 6170 7069 6e67 2028 6469 6374 696f   mapping (dictio
-00004470: 6e61 7279 2920 6b65 7920 6973 206e 6f74  nary) key is not
-00004480: 2066 6f75 6e64 2069 6e20 7468 6520 7365   found in the se
-00004490: 7420 6f66 2065 7869 7374 696e 6720 6b65  t of existing ke
-000044a0: 7973 0a0a 2020 2020 2020 2020 2020 2020  ys..            
-000044b0: 5479 7065 4572 726f 723a 2052 6169 7365  TypeError: Raise
-000044c0: 6420 7768 656e 2061 6e20 6f70 6572 6174  d when an operat
-000044d0: 696f 6e20 6f72 2066 756e 6374 696f 6e20  ion or function 
-000044e0: 6973 2061 7070 6c69 6564 2074 6f20 616e  is applied to an
-000044f0: 206f 626a 6563 7420 6f66 2069 6e61 7070   object of inapp
-00004500: 726f 7072 6961 7465 2074 7970 650a 0a20  ropriate type.. 
-00004510: 2020 2020 2020 2020 2020 2062 7334 2e46             bs4.F
-00004520: 6561 7475 7265 4e6f 7446 6f75 6e64 3a20  eatureNotFound: 
-00004530: 7261 6973 6564 2062 7920 7468 6520 4265  raised by the Be
-00004540: 6175 7469 6675 6c53 6f75 7020 636f 6e73  autifulSoup cons
-00004550: 7472 7563 746f 7220 6966 206e 6f20 7061  tructor if no pa
-00004560: 7273 6572 2077 6974 6820 7468 6520 7265  rser with the re
-00004570: 7175 6573 7465 6420 6665 6174 7572 6573  quested features
-00004580: 0a20 2020 2020 2020 2020 2020 2069 7320  .            is 
-00004590: 666f 756e 640a 2020 2020 2020 2020 7a21  found.        z!
-000045a0: 6874 7470 733a 2f2f 7777 772e 7468 6573  https://www.thes
-000045b0: 6175 7275 732e 636f 6d2f 6272 6f77 7365  aurus.com/browse
-000045c0: 2f72 8100 0000 7a34 5468 6573 6175 7275  /r....z4Thesauru
-000045d0: 732e 636f 6d20 6861 6420 6e6f 2073 796e  s.com had no syn
-000045e0: 6f6e 796d 2072 6566 6572 656e 6365 2066  onym reference f
-000045f0: 6f72 2074 6865 2077 6f72 6420 4e72 8200  or the word Nr..
-00004600: 0000 7a19 6874 7470 733a 2f2f 7777 772e  ..z.https://www.
-00004610: 7468 6573 6175 7275 732e 636f 6d46 7283  thesaurus.comFr.
-00004620: 0000 007a 0d30 2072 6573 756c 7473 2066  ...z.0 results f
-00004630: 6f72 721a 0000 007a 3d23 6865 6164 776f  orr....z=#headwo
-00004640: 7264 203e 2064 6976 2e63 7373 2d62 6a6e  rd > div.css-bjn
-00004650: 3877 682e 6531 6272 3861 3170 3020 3e20  8wh.e1br8a1p0 > 
-00004660: 6469 7620 3e20 756c 203e 206c 6920 3e20  div > ul > li > 
-00004670: 6120 3e20 656d 7203 0000 0072 8800 0000  a > emr....r....
-00004680: 7a0b 6461 7461 2d74 6573 7469 647a 1377  z.data-testidz.w
-00004690: 6f72 642d 6772 6964 2d63 6f6e 7461 696e  ord-grid-contain
-000046a0: 6572 72b3 0000 0072 a200 0000 72a3 0000  err....r....r...
-000046b0: 0072 8700 0000 7a14 6373 732d 316b 6731  .r....z.css-1kg1
-000046c0: 7976 3820 6568 3437 3562 6e30 6301 0000  yv8 eh475bn0c...
-000046d0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-000046e0: 0053 0000 0073 1800 0000 6700 7c00 5d10  .S...s....g.|.].
-000046f0: 7d01 7c01 a000 a100 a001 a100 9102 7104  }.|...........q.
-00004700: 5300 7236 0000 0072 8900 0000 7274 0000  S.r6...r....rt..
-00004710: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
-00004720: 726d 0000 003a 0200 0072 6e00 0000 7a31  rm...:...rn...z1
-00004730: 5379 6e6f 6e79 6d73 2e5f 7175 6572 795f  Synonyms._query_
-00004740: 7468 6573 6175 7275 735f 636f 6d2e 3c6c  thesaurus_com.<l
-00004750: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00004760: 3e54 728b 0000 0072 8c00 0000 728d 0000  >Tr....r....r...
-00004770: 0072 8e00 0000 728f 0000 0029 1d72 4f00  .r....r....).rO.
-00004780: 0000 722b 0000 0072 9000 0000 723b 0000  ..r+...r....r;..
-00004790: 0072 3c00 0000 7204 0000 0072 8500 0000  .r<...r....r....
-000047a0: 7218 0000 0072 9100 0000 7292 0000 0072  r....r....r....r
-000047b0: a900 0000 72a8 0000 0072 7b00 0000 7293  ....r....r{...r.
-000047c0: 0000 0072 5800 0000 728a 0000 0072 7900  ...rX...r....ry.
-000047d0: 0000 724b 0000 0072 9600 0000 7297 0000  ..rK...r....r...
-000047e0: 0072 4100 0000 725b 0000 0072 5c00 0000  .rA...r[...r\...
-000047f0: 725d 0000 0072 5e00 0000 7298 0000 0072  r]...r^...r....r
-00004800: 9900 0000 729a 0000 0072 9b00 0000 290c  ....r....r....).
-00004810: 7232 0000 0072 4e00 0000 729c 0000 0072  r2...rN...r....r
-00004820: 9d00 0000 72b6 0000 0072 a000 0000 729e  ....r....r....r.
-00004830: 0000 0072 ab00 0000 72ad 0000 0072 ae00  ...r....r....r..
-00004840: 0000 72af 0000 0072 4100 0000 7236 0000  ..r....rA...r6..
-00004850: 0072 3600 0000 7237 0000 0072 5500 0000  .r6...r7...rU...
-00004860: 0502 0000 735e 0000 0000 1604 0112 020a  ....s^..........
-00004870: 0112 0106 020c 0104 0102 ff08 020a 010a  ................
-00004880: 010c 0112 0106 0204 0104 020a 0104 0102  ................
-00004890: ff04 0212 010c 0204 0110 0114 0114 0114  ................
-000048a0: 0214 010c 010c 010a 010c 0212 010a 012e  ................
-000048b0: 0110 010a 012c 0110 010a 012c 0110 010a  .....,.....,....
-000048c0: 012c 0110 010a 017a 1d53 796e 6f6e 796d  .,.....z.Synonym
-000048d0: 732e 5f71 7565 7279 5f74 6865 7361 7572  s._query_thesaur
-000048e0: 7573 5f63 6f6d 6301 0000 0000 0000 0000  us_comc.........
-000048f0: 0000 000b 0000 000a 0000 0043 0000 0073  ...........C...s
-00004900: 9802 0000 9001 7a2c 7c00 a000 6401 7c00  ......z,|...d.|.
-00004910: 6a01 9b00 9d02 a101 7d01 7c01 6a02 6402  j.......}.|.j.d.
-00004920: 6b02 7238 7403 a004 6403 7c00 6a01 9b00  k.r8t...d.|.j...
-00004930: 9d02 a101 0100 5700 6404 5300 7405 7c01  ......W.d.S.t.|.
-00004940: 6a06 6405 8302 7d02 7407 6406 7c02 8302  j.d...}.t.d.|...
-00004950: a008 a100 7d03 7c03 6407 7500 9001 721a  ....}.|.d.u...r.
-00004960: 7409 a00a 6408 a101 7d04 7c02 6a0b 7c04  t...d...}.|.j.|.
-00004970: 6409 8d01 728a 7403 a004 6403 7c00 6a01  d...r.t...d.|.j.
-00004980: 9b00 9d02 a101 0100 5700 6404 5300 6700  ........W.d.S.g.
-00004990: 7d05 7c02 6a0c 640a 640b 6409 8d02 9001  }.|.j.d.d.d.....
-000049a0: 722a 640c 7d06 7c02 a00c 640d a101 640e  r*d.}.|...d...d.
-000049b0: 1900 a00c 640f a101 7d07 7c07 4400 5d34  ....d...}.|.D.]4
-000049c0: 7d08 7c08 6a0d 6410 6411 8d01 4400 5d22  }.|.j.d.d...D.]"
-000049d0: 7d09 6412 7c09 6a0e 640e 1900 7601 72ca  }.d.|.j.d...v.r.
-000049e0: 7c05 a00f 7c09 6a0e 640e 1900 a101 0100  |...|.j.d.......
-000049f0: 71ca 71ba 7410 6413 6414 8400 7c05 4400  q.q.t.d.d...|.D.
-00004a00: 8301 8301 7d05 7c00 a011 7c06 7c05 a102  ....}.|...|.|...
-00004a10: 0100 7c05 7c06 6602 5700 5300 6e10 7c03  ..|.|.f.W.S.n.|.
-00004a20: 6410 7500 9001 722a 5700 6404 5300 5700  d.u...r*W.d.S.W.
-00004a30: 9001 6e64 0400 7412 6a13 9001 797a 0100  ..nd..t.j...yz..
-00004a40: 7d0a 0100 7a30 7403 a014 6415 a101 0100  }...z0t...d.....
-00004a50: 7403 a014 6416 a015 7416 a017 7c0a 6a18  t...d...t...|.j.
-00004a60: a101 a101 a101 0100 5700 5900 6404 7d0a  ........W.Y.d.}.
-00004a70: 7e0a 9001 6e22 6404 7d0a 7e0a 3000 0400  ~...n"d.}.~.0...
-00004a80: 7419 9001 79c0 0100 7d0a 0100 7a2e 7403  t...y...}...z.t.
-00004a90: a014 6417 a101 0100 7403 a014 6416 a015  ..d.....t...d...
-00004aa0: 7416 a017 7c0a 6a18 a101 a101 a101 0100  t...|.j.........
-00004ab0: 5700 5900 6404 7d0a 7e0a 6edc 6404 7d0a  W.Y.d.}.~.n.d.}.
-00004ac0: 7e0a 3000 0400 741a 9002 7906 0100 7d0a  ~.0...t...y...}.
-00004ad0: 0100 7a2e 7403 a014 6418 a101 0100 7403  ..z.t...d.....t.
-00004ae0: a014 6416 a015 7416 a017 7c0a 6a18 a101  ..d...t...|.j...
-00004af0: a101 a101 0100 5700 5900 6404 7d0a 7e0a  ......W.Y.d.}.~.
-00004b00: 6e96 6404 7d0a 7e0a 3000 0400 741b 9002  n.d.}.~.0...t...
-00004b10: 794c 0100 7d0a 0100 7a2e 7403 a014 6419  yL..}...z.t...d.
-00004b20: a101 0100 7403 a014 6416 a015 7416 a017  ....t...d...t...
-00004b30: 7c0a 6a18 a101 a101 a101 0100 5700 5900  |.j.........W.Y.
-00004b40: 6404 7d0a 7e0a 6e50 6404 7d0a 7e0a 3000  d.}.~.nPd.}.~.0.
-00004b50: 0400 741c 9002 7992 0100 7d0a 0100 7a2e  ..t...y...}...z.
-00004b60: 7403 a014 641a a101 0100 7403 a014 6416  t...d.....t...d.
-00004b70: a015 7416 a017 7c0a 6a18 a101 a101 a101  ..t...|.j.......
-00004b80: 0100 5700 5900 6404 7d0a 7e0a 6e0a 6404  ..W.Y.d.}.~.n.d.
-00004b90: 7d0a 7e0a 3000 3000 6404 5300 291b 61df  }.~.0.0.d.S.).a.
-00004ba0: 0200 000a 2020 2020 2020 2020 5468 6973  ....        This
-00004bb0: 2066 756e 6374 696f 6e20 7175 6572 6965   function querie
-00004bc0: 7320 776f 7264 6e65 7420 666f 7220 7379  s wordnet for sy
-00004bd0: 6e6f 6e79 6d73 2061 7373 6f63 6961 7465  nonyms associate
-00004be0: 640a 2020 2020 2020 2020 7769 7468 2074  d.        with t
-00004bf0: 6865 2073 7065 6369 6669 6320 776f 7264  he specific word
-00004c00: 2070 726f 7669 6465 6420 746f 2074 6865   provided to the
-00004c10: 2043 6c61 7373 2053 796e 6f6e 796d 732e   Class Synonyms.
-00004c20: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00004c30: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00004c40: 7379 6e6f 6e79 6d73 3a20 6c69 7374 206f  synonyms: list o
-00004c50: 6620 7379 6e6f 6e79 6d73 0a0a 2020 2020  f synonyms..    
-00004c60: 2020 2020 3a72 7479 7065 3a20 6c69 7374      :rtype: list
-00004c70: 0a0a 2020 2020 2020 2020 3a72 6169 7365  ..        :raise
-00004c80: 733a 0a20 2020 2020 2020 2020 2020 2041  s:.            A
-00004c90: 7474 7269 6275 7465 4572 726f 723a 2052  ttributeError: R
-00004ca0: 6169 7365 6420 7768 656e 2061 6e20 6174  aised when an at
-00004cb0: 7472 6962 7574 6520 7265 6665 7265 6e63  tribute referenc
-00004cc0: 6520 6f72 2061 7373 6967 6e6d 656e 7420  e or assignment 
-00004cd0: 6661 696c 730a 0a20 2020 2020 2020 2020  fails..         
-00004ce0: 2020 2049 6e64 6578 4572 726f 723a 2052     IndexError: R
-00004cf0: 6169 7365 6420 7768 656e 2061 2073 6571  aised when a seq
-00004d00: 7565 6e63 6520 7375 6273 6372 6970 7420  uence subscript 
-00004d10: 6973 206f 7574 206f 6620 7261 6e67 650a  is out of range.
-00004d20: 0a20 2020 2020 2020 2020 2020 204b 6579  .            Key
-00004d30: 4572 726f 723a 2052 6169 7365 6420 7768  Error: Raised wh
-00004d40: 656e 2061 206d 6170 7069 6e67 2028 6469  en a mapping (di
-00004d50: 6374 696f 6e61 7279 2920 6b65 7920 6973  ctionary) key is
-00004d60: 206e 6f74 2066 6f75 6e64 2069 6e20 7468   not found in th
-00004d70: 6520 7365 7420 6f66 2065 7869 7374 696e  e set of existin
-00004d80: 6720 6b65 7973 0a0a 2020 2020 2020 2020  g keys..        
-00004d90: 2020 2020 5479 7065 4572 726f 723a 2052      TypeError: R
-00004da0: 6169 7365 6420 7768 656e 2061 6e20 6f70  aised when an op
-00004db0: 6572 6174 696f 6e20 6f72 2066 756e 6374  eration or funct
-00004dc0: 696f 6e20 6973 2061 7070 6c69 6564 2074  ion is applied t
-00004dd0: 6f20 616e 206f 626a 6563 7420 6f66 2069  o an object of i
-00004de0: 6e61 7070 726f 7072 6961 7465 2074 7970  nappropriate typ
-00004df0: 650a 0a20 2020 2020 2020 2020 2020 2062  e..            b
-00004e00: 7334 2e46 6561 7475 7265 4e6f 7446 6f75  s4.FeatureNotFou
-00004e10: 6e64 3a20 7261 6973 6564 2062 7920 7468  nd: raised by th
-00004e20: 6520 4265 6175 7469 6675 6c53 6f75 7020  e BeautifulSoup 
-00004e30: 636f 6e73 7472 7563 746f 7220 6966 206e  constructor if n
-00004e40: 6f20 7061 7273 6572 2077 6974 6820 7468  o parser with th
-00004e50: 6520 7265 7175 6573 7465 6420 6665 6174  e requested feat
-00004e60: 7572 6573 0a20 2020 2020 2020 2020 2020  ures.           
-00004e70: 2069 7320 666f 756e 640a 2020 2020 2020   is found.      
-00004e80: 2020 7a2d 6874 7470 3a2f 2f77 6f72 646e    z-http://wordn
-00004e90: 6574 7765 622e 7072 696e 6365 746f 6e2e  etweb.princeton.
-00004ea0: 6564 752f 7065 726c 2f77 6562 776e 3f73  edu/perl/webwn?s
-00004eb0: 3d72 8100 0000 7a2e 576f 7264 6e65 7420  =r....z.Wordnet 
-00004ec0: 6861 6420 6e6f 2073 796e 6f6e 796d 2072  had no synonym r
-00004ed0: 6566 6572 656e 6365 2066 6f72 2074 6865  eference for the
-00004ee0: 2077 6f72 6420 4e72 8200 0000 7a1f 6874   word Nr....z.ht
-00004ef0: 7470 3a2f 2f77 6f72 646e 6574 7765 622e  tp://wordnetweb.
-00004f00: 7072 696e 6365 746f 6e2e 6564 7546 7a26  princeton.eduFz&
-00004f10: 596f 7572 2073 6561 7263 6820 6469 6420  Your search did 
-00004f20: 6e6f 7420 7265 7475 726e 2061 6e79 2072  not return any r
-00004f30: 6573 756c 7473 7284 0000 00da 0268 335a  esultsr......h3Z
-00004f40: 044e 6f75 6e5a 046e 6f75 6e72 b300 0000  .NounZ.nounr....
-00004f50: 7203 0000 0072 a200 0000 5472 a400 0000  r....r....Tr....
-00004f60: 7a02 533a 6301 0000 0000 0000 0000 0000  z.S:c...........
-00004f70: 0002 0000 0004 0000 0053 0000 0073 1800  .........S...s..
-00004f80: 0000 6700 7c00 5d10 7d01 7c01 a000 a100  ..g.|.].}.|.....
-00004f90: a001 a100 9102 7104 5300 7236 0000 0072  ......q.S.r6...r
-00004fa0: 8900 0000 7274 0000 0072 3600 0000 7236  ....rt...r6...r6
-00004fb0: 0000 0072 3700 0000 726d 0000 007f 0200  ...r7...rm......
-00004fc0: 0072 6e00 0000 7a2b 5379 6e6f 6e79 6d73  .rn...z+Synonyms
-00004fd0: 2e5f 7175 6572 795f 776f 7264 6e65 742e  ._query_wordnet.
-00004fe0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00004ff0: 6d70 3e72 8b00 0000 721a 0000 0072 8c00  mp>r....r....r..
-00005000: 0000 728d 0000 0072 8e00 0000 728f 0000  ..r....r....r...
-00005010: 0029 1d72 4f00 0000 722b 0000 0072 9000  .).rO...r+...r..
-00005020: 0000 723b 0000 0072 3c00 0000 7204 0000  ..r;...r<...r...
-00005030: 0072 8500 0000 7218 0000 0072 9100 0000  .r....r....r....
-00005040: 72a6 0000 0072 a700 0000 7292 0000 00da  r....r....r.....
-00005050: 0766 696e 6441 6c6c 7293 0000 00da 0863  .findAllr......c
-00005060: 6f6e 7465 6e74 7372 5800 0000 7279 0000  ontentsrX...ry..
-00005070: 0072 4b00 0000 7296 0000 0072 9700 0000  .rK...r....r....
-00005080: 7241 0000 0072 5b00 0000 725c 0000 0072  rA...r[...r\...r
-00005090: 5d00 0000 725e 0000 0072 9800 0000 7299  ]...r^...r....r.
-000050a0: 0000 0072 9a00 0000 729b 0000 0029 0b72  ...r....r....).r
-000050b0: 3200 0000 724e 0000 0072 9c00 0000 729d  2...rN...r....r.
-000050c0: 0000 0072 aa00 0000 72a0 0000 0072 9e00  ...r....r....r..
-000050d0: 0000 5a0b 7061 7265 6e74 5f6e 6f64 65da  ..Z.parent_node.
-000050e0: 0863 6869 6c64 7265 6e72 9f00 0000 7241  .childrenr....rA
-000050f0: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
-00005100: 0000 7256 0000 0051 0200 0073 5400 0000  ..rV...Q...sT...
-00005110: 0016 0401 1202 0a01 1201 0602 0c01 0401  ................
-00005120: 02ff 0802 0a01 0a01 0c01 1201 0602 0401  ................
-00005130: 1001 0401 1401 0801 1001 0e01 1401 1201  ................
-00005140: 0c01 0c01 0a01 0c02 1201 0a01 2e01 1001  ................
-00005150: 0a01 2c01 1001 0a01 2c01 1001 0a01 2c01  ..,.....,.....,.
-00005160: 1001 0a01 7a17 5379 6e6f 6e79 6d73 2e5f  ....z.Synonyms._
-00005170: 7175 6572 795f 776f 7264 6e65 7429 0672  query_wordnet).r
-00005180: 1a00 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
-00005190: 0000 004e 4e29 1dda 085f 5f6e 616d 655f  ...NN)...__name_
-000051a0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000051b0: 5f71 7561 6c6e 616d 655f 5fda 0373 7472  _qualname__..str
-000051c0: da03 696e 7472 1000 0000 720e 0000 0072  ..intr....r....r
-000051d0: 3800 0000 7230 0000 00da 0462 6f6f 6c72  8...r0.....boolr
-000051e0: 4300 0000 7213 0000 0072 1400 0000 720f  C...r....r....r.
-000051f0: 0000 0072 4700 0000 7211 0000 0072 4b00  ...rG...r....rK.
-00005200: 0000 da08 7265 7175 6573 7473 da06 6d6f  ....requests..mo
-00005210: 6465 6c73 da08 5265 7370 6f6e 7365 724f  dels..ResponserO
-00005220: 0000 0072 6600 0000 7212 0000 0072 3100  ...rf...r....r1.
-00005230: 0000 7252 0000 0072 5300 0000 7254 0000  ..rR...rS...rT..
-00005240: 0072 5500 0000 7256 0000 0072 3600 0000  .rU...rV...r6...
-00005250: 7236 0000 0072 3600 0000 7237 0000 0072  r6...r6...r7...r
-00005260: 1900 0000 3500 0000 7334 0000 0008 0300  ....5...s4......
-00005270: 0100 0100 0100 0100 0100 fa02 0102 0102  ................
-00005280: 0102 0102 0106 010e fa0c 3208 080e 102a  ..........2....*
-00005290: 0422 0414 1612 1828 4422 6422 5522 5122  .".....(D"d"U"Q"
-000052a0: 4c72 1900 0000 2930 da07 5f5f 646f 635f  Lr....)0..__doc_
-000052b0: 5fda 0a5f 5f61 7574 686f 725f 5fda 085f  _..__author__.._
-000052c0: 5f64 6174 655f 5fda 0a5f 5f73 7461 7475  _date__..__statu
-000052d0: 735f 5fda 0b5f 5f6c 6963 656e 7365 5f5f  s__..__license__
-000052e0: da0d 5f5f 636f 7079 7269 6768 745f 5f72  ..__copyright__r
-000052f0: 9600 0000 7224 0000 00da 076c 6f67 6769  ....r$.....loggi
-00005300: 6e67 72c1 0000 0072 5c00 0000 da02 7265  ngr....r\.....re
-00005310: 72a6 0000 0072 0400 0000 da07 6261 636b  r....r......back
-00005320: 6f66 6672 0500 0000 7206 0000 00da 0972  offr....r......r
-00005330: 6174 656c 696d 6974 7207 0000 0072 0800  atelimitr....r..
-00005340: 0000 da20 776f 7264 686f 6172 642e 7574  ... wordhoard.ut
-00005350: 696c 6974 6965 732e 7265 7175 6573 745f  ilities.request_
-00005360: 6874 6d6c 7209 0000 005a 2577 6f72 6468  htmlr....Z%wordh
-00005370: 6f61 7264 2e75 7469 6c69 7469 6573 2e63  oard.utilities.c
-00005380: 6c6f 7564 666c 6172 655f 6279 7061 7373  loudflare_bypass
-00005390: 720a 0000 00da 2277 6f72 6468 6f61 7264  r....."wordhoard
-000053a0: 2e75 7469 6c69 7469 6573 2e63 6f6c 6f72  .utilities.color
-000053b0: 697a 6564 5f74 6578 7472 0b00 0000 da12  ized_textr......
-000053c0: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
-000053d0: 6573 720c 0000 0072 0d00 0000 da06 7479  esr....r......ty
-000053e0: 7069 6e67 720e 0000 0072 0f00 0000 7210  pingr....r....r.
-000053f0: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
-00005400: 0000 7214 0000 005a 1377 6f72 6468 6f61  ..r....Z.wordhoa
-00005410: 7264 2e75 7469 6c69 7469 6573 7215 0000  rd.utilitiesr...
-00005420: 0072 1600 0000 7217 0000 00da 2677 6f72  .r....r.....&wor
-00005430: 6468 6f61 7264 2e75 7469 6c69 7469 6573  dhoard.utilities
-00005440: 2e63 6c6f 7564 666c 6172 655f 6368 6563  .cloudflare_chec
-00005450: 6b65 7272 1800 0000 da09 6765 744c 6f67  kerr......getLog
-00005460: 6765 7272 bb00 0000 723b 0000 00da 066f  gerr....r;.....o
-00005470: 626a 6563 7472 1900 0000 7236 0000 0072  bjectr....r6...r
-00005480: 3600 0000 7236 0000 0072 3700 0000 da08  6...r6...r7.....
-00005490: 3c6d 6f64 756c 653e 0300 0000 732e 0000  <module>....s...
-000054a0: 0004 0404 0104 0104 0104 0104 1708 0108  ................
-000054b0: 0108 0108 0108 0108 010c 0110 0110 010c  ................
-000054c0: 010c 010c 0110 0124 0114 010c 020a 02    .......$.......
+00000060: 6407 6c09 5a09 6406 6407 6c0a 5a0b 6406  d.l.Z.d.d.l.Z.d.
+00000070: 6408 6c0c 6d0d 5a0d 0100 6406 6409 6c0e  d.l.m.Z...d.d.l.
+00000080: 6d0f 5a0f 0100 6406 640a 6c10 6d11 5a11  m.Z...d.d.l.m.Z.
+00000090: 6d12 5a12 6d13 5a13 0100 6406 640b 6c14  m.Z.m.Z...d.d.l.
+000000a0: 6d15 5a15 6d16 5a16 6d17 5a17 6d18 5a18  m.Z.m.Z.m.Z.m.Z.
+000000b0: 6d19 5a19 6d1a 5a1a 0100 6406 6407 6c1b  m.Z.m.Z...d.d.l.
+000000c0: 5a1b 6406 6407 6c1c 5a1c 6406 640c 6c1b  Z.d.d.l.Z.d.d.l.
+000000d0: 6d1d 5a1d 0100 6406 640d 6c1e 6d1f 5a1f  m.Z...d.d.l.m.Z.
+000000e0: 6d20 5a20 0100 6406 640e 6c21 6d22 5a22  m Z ..d.d.l!m"Z"
+000000f0: 6d23 5a23 0100 6406 640f 6c24 6d25 5a25  m#Z#..d.d.l$m%Z%
+00000100: 0100 6406 6410 6c26 6d27 5a27 0100 6406  ..d.d.l&m'Z'..d.
+00000110: 6411 6c28 6d29 5a29 6d2a 5a2a 6d2b 5a2b  d.l(m)Z)m*Z*m+Z+
+00000120: 0100 6406 6412 6c2c 6d2d 5a2d 0100 6508  ..d.d.l,m-Z-..e.
+00000130: a02e 652f a101 5a30 4700 6413 6414 8400  ..e/..Z0G.d.d...
+00000140: 6414 8302 5a31 4700 6415 6416 8400 6416  d...Z1G.d.d...d.
+00000150: 8302 5a32 4700 6417 6418 8400 6418 8302  ..Z2G.d.d...d...
+00000160: 5a33 6407 5300 2919 7a78 0a54 6869 7320  Z3d.S.).zx.This 
+00000170: 5079 7468 6f6e 206d 6f64 756c 6520 6973  Python module is
+00000180: 2064 6573 6967 6e65 6420 746f 2071 7565   designed to que
+00000190: 7279 206d 756c 7469 706c 6520 6f6e 6c69  ry multiple onli
+000001a0: 6e65 2072 6570 6f73 6974 6f72 6965 7320  ne repositories 
+000001b0: 666f 7220 7468 650a 616e 746f 6e79 6d73  for the.antonyms
+000001c0: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
+000001d0: 2061 2073 7065 6369 6669 6320 776f 7264   a specific word
+000001e0: 2e0a 7a0e 4a6f 686e 2042 756d 6761 726e  ..z.John Bumgarn
+000001f0: 6572 7a10 4f63 746f 6265 7220 3135 2c20  erz.October 15, 
+00000200: 3230 3230 da0a 5072 6f64 7563 7469 6f6e  2020..Production
+00000210: da03 4d49 547a 2143 6f70 7972 6967 6874  ..MITz!Copyright
+00000220: 2028 4329 2032 3032 3020 4a6f 686e 2042   (C) 2020 John B
+00000230: 756d 6761 726e 6572 e900 0000 004e 2901  umgarner.....N).
+00000240: da05 5369 7a65 6429 01da 1042 726f 6b65  ..Sized)...Broke
+00000250: 6e54 6872 6561 6450 6f6f 6c29 03da 1254  nThreadPool)...T
+00000260: 6872 6561 6450 6f6f 6c45 7865 6375 746f  hreadPoolExecuto
+00000270: 72da 0c61 735f 636f 6d70 6c65 7465 64da  r..as_completed.
+00000280: 0e42 726f 6b65 6e45 7865 6375 746f 7229  .BrokenExecutor)
+00000290: 06da 0444 6963 74da 044c 6973 74da 084f  ...Dict..List..O
+000002a0: 7074 696f 6e61 6cda 0353 6574 da05 5475  ptional..Set..Tu
+000002b0: 706c 65da 0555 6e69 6f6e 2901 da0d 4265  ple..Union)...Be
+000002c0: 6175 7469 6675 6c53 6f75 7029 02da 0c6f  autifulSoup)...o
+000002d0: 6e5f 6578 6365 7074 696f 6eda 0465 7870  n_exception..exp
+000002e0: 6f29 02da 066c 696d 6974 73da 1252 6174  o)...limits..Rat
+000002f0: 654c 696d 6974 4578 6365 7074 696f 6e29  eLimitException)
+00000300: 01da 0551 7565 7279 2901 da0e 636f 6c6f  ...Query)...colo
+00000310: 7269 7a65 645f 7465 7874 2903 da07 6361  rized_text)...ca
+00000320: 6368 696e 67da 0963 6c65 616e 7369 6e67  ching..cleansing
+00000330: da11 776f 7264 5f76 6572 6966 6963 6174  ..word_verificat
+00000340: 696f 6e29 01da 1643 6c6f 7564 666c 6172  ion)...Cloudflar
+00000350: 6556 6572 6966 6963 6174 696f 6e63 0000  eVerificationc..
+00000360: 0000 0000 0000 0000 0000 0000 0000 0400  ................
+00000370: 0000 4000 0000 7344 0000 0065 005a 0164  ..@...sD...e.Z.d
+00000380: 005a 0264 015a 0365 0464 0264 0384 0083  .Z.d.Z.e.d.d....
+00000390: 015a 0565 0465 0665 0764 049c 0264 0564  .Z.e.e.e.d...d.d
+000003a0: 0684 0483 015a 0865 0465 0665 0764 049c  .....Z.e.e.e.d..
+000003b0: 0264 0764 0884 0483 015a 0964 0953 0029  .d.d.....Z.d.S.)
+000003c0: 0ada 0c50 6172 744f 6653 7065 6563 6861  ...PartOfSpeecha
+000003d0: 9d02 0000 0a20 2020 2020 2020 2054 6869  .....        Thi
+000003e0: 7320 7574 696c 6974 7920 636c 6173 7320  s utility class 
+000003f0: 636f 6e74 6169 6e73 2073 7461 7469 6320  contains static 
+00000400: 6d65 7468 6f64 7320 746f 2065 7874 7261  methods to extra
+00000410: 6374 2070 6172 7420 6f66 2073 7065 6563  ct part of speec
+00000420: 6820 6361 7465 676f 7269 6573 0a20 2020  h categories.   
+00000430: 2020 2020 2066 726f 6d20 4854 4d4c 2072       from HTML r
+00000440: 6573 706f 6e73 6573 206f 6620 7661 7269  esponses of vari
+00000450: 6f75 7320 736f 7572 6365 732c 2077 6869  ous sources, whi
+00000460: 6368 2061 7265 2054 6865 7361 7572 7573  ch are Thesaurus
+00000470: 2e63 6f6d 2c20 616e 6420 576f 7264 4869  .com, and WordHi
+00000480: 7070 6f2e 0a0a 2020 2020 2020 2020 5374  ppo...        St
+00000490: 6174 6963 204d 6574 686f 6473 0a20 2020  atic Methods.   
+000004a0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
+000004b0: 2d2d 2d0a 2020 2020 2020 2020 5f68 616e  ---.        _han
+000004c0: 646c 655f 7175 6572 795f 6578 6365 7074  dle_query_except
+000004d0: 696f 6e73 2865 7272 6f72 293a 0a20 2020  ions(error):.   
+000004e0: 2020 2020 2020 2020 2048 656c 7065 7220           Helper 
+000004f0: 6d65 7468 6f64 2074 6f20 6861 6e64 6c65  method to handle
+00000500: 2063 6f6d 6d6f 6e20 6578 6365 7074 696f   common exceptio
+00000510: 6e73 2069 6e20 7175 6572 7920 6d65 7468  ns in query meth
+00000520: 6f64 732e 0a0a 2020 2020 2020 2020 7061  ods...        pa
+00000530: 7274 5f6f 665f 7370 6565 6368 5f63 6174  rt_of_speech_cat
+00000540: 6567 6f72 795f 7468 6573 6175 7275 735f  egory_thesaurus_
+00000550: 636f 6d28 736f 7570 3a20 4265 6175 7469  com(soup: Beauti
+00000560: 6675 6c53 6f75 7029 202d 3e20 7374 723a  fulSoup) -> str:
+00000570: 0a20 2020 2020 2020 2020 2020 2045 7874  .            Ext
+00000580: 7261 6374 7320 7468 6520 7061 7274 206f  racts the part o
+00000590: 6620 7370 6565 6368 2063 6174 6567 6f72  f speech categor
+000005a0: 7920 6672 6f6d 2074 6865 2048 544d 4c20  y from the HTML 
+000005b0: 7265 7370 6f6e 7365 206f 6620 5468 6573  response of Thes
+000005c0: 6175 7275 732e 636f 6d2e 0a0a 2020 2020  aurus.com...    
+000005d0: 2020 2020 7061 7274 5f6f 665f 7370 6565      part_of_spee
+000005e0: 6368 5f63 6174 6567 6f72 795f 776f 7264  ch_category_word
+000005f0: 6869 7070 6f28 736f 7570 3a20 4265 6175  hippo(soup: Beau
+00000600: 7469 6675 6c53 6f75 7029 202d 3e20 7374  tifulSoup) -> st
+00000610: 723a 0a20 2020 2020 2020 2020 2020 2045  r:.            E
+00000620: 7874 7261 6374 7320 7468 6520 7061 7274  xtracts the part
+00000630: 206f 6620 7370 6565 6368 2063 6174 6567   of speech categ
+00000640: 6f72 7920 6672 6f6d 2074 6865 2048 544d  ory from the HTM
+00000650: 4c20 7265 7370 6f6e 7365 206f 6620 576f  L response of Wo
+00000660: 7264 4869 7070 6f2e 0a20 2020 2020 2020  rdHippo..       
+00000670: 2063 0100 0000 0000 0000 0000 0000 0100   c..............
+00000680: 0000 0700 0000 4300 0000 7326 0000 0074  ......C...s&...t
+00000690: 00a0 0164 01a1 0101 0074 00a0 0164 02a0  ...d.....t...d..
+000006a0: 0274 03a0 047c 006a 05a1 01a1 01a1 0101  .t...|.j........
+000006b0: 0064 0353 00a9 047a 4d0a 2020 2020 2020  .d.S...zM.      
+000006c0: 2020 4865 6c70 6572 206d 6574 686f 6420    Helper method 
+000006d0: 746f 2068 616e 646c 6520 636f 6d6d 6f6e  to handle common
+000006e0: 2065 7863 6570 7469 6f6e 7320 696e 2071   exceptions in q
+000006f0: 7565 7279 206d 6574 686f 6473 2e0a 2020  uery methods..  
+00000700: 2020 2020 2020 7a30 416e 2065 7272 6f72        z0An error
+00000710: 206f 6363 7572 7265 6420 696e 2074 6865   occurred in the
+00000720: 2066 6f6c 6c6f 7769 6e67 2063 6f64 6520   following code 
+00000730: 7365 676d 656e 743a da00 4ea9 06da 066c  segment:..N....l
+00000740: 6f67 6765 72da 0565 7272 6f72 da04 6a6f  ogger..error..jo
+00000750: 696e da09 7472 6163 6562 6163 6bda 0966  in..traceback..f
+00000760: 6f72 6d61 745f 7462 da0d 5f5f 7472 6163  ormat_tb..__trac
+00000770: 6562 6163 6b5f 5fa9 0172 1f00 0000 a900  eback__..r......
+00000780: 7225 0000 00fa 4b2f 5573 6572 732f 6275  r%....K/Users/bu
+00000790: 6d67 6172 6e65 722f 5079 7468 6f6e 5f50  mgarner/Python_P
+000007a0: 726f 6a65 6374 732f 776f 7264 686f 6172  rojects/wordhoar
+000007b0: 645f 7072 6f64 7563 7469 6f6e 2f77 6f72  d_production/wor
+000007c0: 6468 6f61 7264 2f61 6e74 6f6e 796d 732e  dhoard/antonyms.
+000007d0: 7079 da18 5f68 616e 646c 655f 7175 6572  py.._handle_quer
+000007e0: 795f 6578 6365 7074 696f 6e73 4d00 0000  y_exceptionsM...
+000007f0: 7304 0000 0000 050a 017a 2550 6172 744f  s........z%PartO
+00000800: 6653 7065 6563 682e 5f68 616e 646c 655f  fSpeech._handle_
+00000810: 7175 6572 795f 6578 6365 7074 696f 6e73  query_exceptions
+00000820: a902 da04 736f 7570 da06 7265 7475 726e  ....soup..return
+00000830: 6301 0000 0000 0000 0000 0000 000a 0000  c...............
+00000840: 000c 0000 0043 0000 0073 c600 0000 6401  .....C...s....d.
+00000850: 7d01 7a82 6402 7d02 6403 7d03 7c00 6a00  }.z.d.}.d.}.|.j.
+00000860: 6404 7401 a002 7c02 a101 6405 8d02 7d04  d.t...|...d...}.
+00000870: 7c04 7284 7401 6a03 7c02 9b00 6406 7c03  |.r.t.j.|...d.|.
+00000880: 9b00 9d03 7c04 6a04 6407 8d02 7d05 7c05  ....|.j.d...}.|.
+00000890: 7284 7c05 a005 6408 a101 a006 6409 a101  r.|...d.....d...
+000008a0: 7d06 7c06 a007 640a 640b a102 7d06 640c  }.|...d.d...}.d.
+000008b0: 7d07 7401 6a03 7c07 7c06 6407 8d02 7d08  }.t.j.|.|.d...}.
+000008c0: 7c08 7284 7c08 a005 6408 a101 a006 a100  |.r.|...d.......
+000008d0: 7d01 5700 6e3a 0400 7408 6a09 740a 740b  }.W.n:..t.j.t.t.
+000008e0: 740c 740d 6605 79c0 0100 7d09 0100 7a16  t.t.f.y...}...z.
+000008f0: 740e a00f 7c09 a101 0100 5700 5900 640d  t...|.....W.Y.d.
+00000900: 7d09 7e09 6e0a 640d 7d09 7e09 3000 3000  }.~.n.d.}.~.0.0.
+00000910: 7c01 5300 290e 6110 0100 000a 2020 2020  |.S.).a.....    
+00000920: 2020 2020 4578 7472 6163 7473 2074 6865      Extracts the
+00000930: 2070 6172 7420 6f66 2073 7065 6563 6820   part of speech 
+00000940: 6361 7465 676f 7279 2066 726f 6d20 7468  category from th
+00000950: 6520 4854 4d4c 2072 6573 706f 6e73 6520  e HTML response 
+00000960: 6f66 2054 6865 7361 7572 7573 2e63 6f6d  of Thesaurus.com
+00000970: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+00000980: 6d20 736f 7570 3a20 4265 6175 7469 6675  m soup: Beautifu
+00000990: 6c53 6f75 7020 6f62 6a65 6374 2063 6f6e  lSoup object con
+000009a0: 7461 696e 696e 6720 7468 6520 4854 4d4c  taining the HTML
+000009b0: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
+000009c0: 2020 3a70 6172 616d 2074 7970 6520 736f    :param type so
+000009d0: 7570 3a20 6273 342e 4265 6175 7469 6675  up: bs4.Beautifu
+000009e0: 6c53 6f75 700a 2020 2020 2020 2020 3a72  lSoup.        :r
+000009f0: 6574 7572 6e3a 2050 6172 7420 6f66 2073  eturn: Part of s
+00000a00: 7065 6563 6820 6361 7465 676f 7279 0a20  peech category. 
+00000a10: 2020 2020 2020 203a 7274 7970 653a 2073         :rtype: s
+00000a20: 7472 0a20 2020 2020 2020 2072 1c00 0000  tr.        r....
+00000a30: fa37 7769 6e64 6f77 5c2e 5f5f 7374 6174  .7window\.__stat
+00000a40: 6963 526f 7574 6572 4879 6472 6174 696f  icRouterHydratio
+00000a50: 6e44 6174 615c 732a 3d5c 732a 4a53 4f4e  nData\s*=\s*JSON
+00000a60: 5c2e 7061 7273 655c 28fa 035c 293b da06  \.parse\(..\);..
+00000a70: 7363 7269 7074 2902 da04 6e61 6d65 da04  script)...name..
+00000a80: 7465 7874 fa05 282e 2a3f 29a9 02da 0770  text..(.*?)....p
+00000a90: 6174 7465 726e da06 7374 7269 6e67 e901  attern..string..
+00000aa0: 0000 00fa 0222 27fa 025c 22fa 0122 7a2b  ....."'..\".."z+
+00000ab0: 2270 6172 744f 6653 7065 6563 6822 3a22  "partOfSpeech":"
+00000ac0: 285b 5e22 5d2a 2922 2c22 7368 6f72 7444  ([^"]*)","shortD
+00000ad0: 6566 696e 6974 696f 6e73 224e 2910 da04  efinitions"N)...
+00000ae0: 6669 6e64 da05 7265 6765 78da 0763 6f6d  find..regex..com
+00000af0: 7069 6c65 da06 7365 6172 6368 7233 0000  pile..searchr3..
+00000b00: 00da 0567 726f 7570 da05 7374 7269 70da  ...group..strip.
+00000b10: 0772 6570 6c61 6365 da03 6273 34da 0f46  .replace..bs4..F
+00000b20: 6561 7475 7265 4e6f 7446 6f75 6e64 da0e  eatureNotFound..
+00000b30: 4174 7472 6962 7574 6545 7272 6f72 da0a  AttributeError..
+00000b40: 496e 6465 7845 7272 6f72 da08 4b65 7945  IndexError..KeyE
+00000b50: 7272 6f72 da09 5479 7065 4572 726f 7272  rror..TypeErrorr
+00000b60: 1a00 0000 7227 0000 0029 0a72 2900 0000  ....r'...).r)...
+00000b70: da17 7061 7274 5f6f 665f 7370 6565 6368  ..part_of_speech
+00000b80: 5f63 6174 6567 6f72 79da 0d73 7461 7274  _category..start
+00000b90: 5f70 6174 7465 726e da0b 656e 645f 7061  _pattern..end_pa
+00000ba0: 7474 6572 6eda 0a73 6372 6970 745f 7461  ttern..script_ta
+00000bb0: 67da 056d 6174 6368 da0d 6a73 6f6e 5f64  g..match..json_d
+00000bc0: 6174 615f 7374 725a 0b70 6f73 5f70 6174  ata_strZ.pos_pat
+00000bd0: 7465 726e 5a09 706f 735f 6d61 7463 6872  ternZ.pos_matchr
+00000be0: 1f00 0000 7225 0000 0072 2500 0000 7226  ....r%...r%...r&
+00000bf0: 0000 00da 2570 6172 745f 6f66 5f73 7065  ....%part_of_spe
+00000c00: 6563 685f 6361 7465 676f 7279 5f74 6865  ech_category_the
+00000c10: 7361 7572 7573 5f63 6f6d 5500 0000 7322  saurus_comU...s"
+00000c20: 0000 0000 0a04 0102 0104 0104 0114 0104  ................
+00000c30: 011a 0104 0110 010c 0104 010e 0104 0112  ................
+00000c40: 011a 0120 017a 3250 6172 744f 6653 7065  ... .z2PartOfSpe
+00000c50: 6563 682e 7061 7274 5f6f 665f 7370 6565  ech.part_of_spee
+00000c60: 6368 5f63 6174 6567 6f72 795f 7468 6573  ch_category_thes
+00000c70: 6175 7275 735f 636f 6d63 0100 0000 0000  aurus_comc......
+00000c80: 0000 0000 0000 0400 0000 0c00 0000 4300  ..............C.
+00000c90: 0000 7394 0000 0064 017d 017a 507c 006a  ..s....d.}.zP|.j
+00000ca0: 0064 0264 0364 0469 0164 058d 0272 527c  .d.d.d.i.d...rR|
+00000cb0: 006a 0064 0264 0364 0469 0164 058d 027d  .j.d.d.d.i.d...}
+00000cc0: 0274 017c 026a 0283 0164 066b 0372 5264  .t.|.j...d.k.rRd
+00000cd0: 01a0 0374 0464 0764 0884 007c 026a 0283  ...t.d.d...|.j..
+00000ce0: 02a1 01a0 05a1 007d 0157 006e 3a04 0074  .......}.W.n:..t
+00000cf0: 066a 0774 0874 0974 0a74 0b66 0579 8e01  .j.t.t.t.t.f.y..
+00000d00: 007d 0301 007a 1674 0ca0 0d7c 03a1 0101  .}...z.t...|....
+00000d10: 0057 0059 0064 097d 037e 036e 0a64 097d  .W.Y.d.}.~.n.d.}
+00000d20: 037e 0330 0030 007c 0153 0029 0a61 0c01  .~.0.0.|.S.).a..
+00000d30: 0000 0a20 2020 2020 2020 2045 7874 7261  ...        Extra
+00000d40: 6374 7320 7468 6520 7061 7274 206f 6620  cts the part of 
+00000d50: 7370 6565 6368 2063 6174 6567 6f72 7920  speech category 
+00000d60: 6672 6f6d 2074 6865 2048 544d 4c20 7265  from the HTML re
+00000d70: 7370 6f6e 7365 206f 6620 576f 7264 4869  sponse of WordHi
+00000d80: 7070 6f2e 0a0a 2020 2020 2020 2020 3a70  ppo...        :p
+00000d90: 6172 616d 2073 6f75 703a 2042 6561 7574  aram soup: Beaut
+00000da0: 6966 756c 536f 7570 206f 626a 6563 7420  ifulSoup object 
+00000db0: 636f 6e74 6169 6e69 6e67 2074 6865 2048  containing the H
+00000dc0: 544d 4c20 7265 7370 6f6e 7365 0a20 2020  TML response.   
+00000dd0: 2020 2020 203a 7061 7261 6d20 7479 7065       :param type
+00000de0: 2073 6f75 703a 2062 7334 2e42 6561 7574   soup: bs4.Beaut
+00000df0: 6966 756c 536f 7570 0a20 2020 2020 2020  ifulSoup.       
+00000e00: 203a 7265 7475 726e 3a20 5061 7274 206f   :return: Part o
+00000e10: 6620 7370 6565 6368 2063 6174 6567 6f72  f speech categor
+00000e20: 790a 2020 2020 2020 2020 3a72 7479 7065  y.        :rtype
+00000e30: 3a20 7374 720a 2020 2020 2020 2020 721c  : str.        r.
+00000e40: 0000 00da 0364 6976 da05 636c 6173 735a  .....div..classZ
+00000e50: 0877 6f72 6474 7970 65a9 0272 2e00 0000  .wordtype..r....
+00000e60: 5a05 6174 7472 7372 0300 0000 6301 0000  Z.attrsr....c...
+00000e70: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00000e80: 0053 0000 0073 0800 0000 7c00 a000 a100  .S...s....|.....
+00000e90: 5300 a901 4e29 01da 0769 7361 6c70 6861  S...N)...isalpha
+00000ea0: 2901 da01 7872 2500 0000 7225 0000 0072  )...xr%...r%...r
+00000eb0: 2600 0000 da08 3c6c 616d 6264 613e 8000  &.....<lambda>..
+00000ec0: 0000 f300 0000 007a 4050 6172 744f 6653  .......z@PartOfS
+00000ed0: 7065 6563 682e 7061 7274 5f6f 665f 7370  peech.part_of_sp
+00000ee0: 6565 6368 5f63 6174 6567 6f72 795f 776f  eech_category_wo
+00000ef0: 7264 6869 7070 6f2e 3c6c 6f63 616c 733e  rdhippo.<locals>
+00000f00: 2e3c 6c61 6d62 6461 3e4e 290e 7238 0000  .<lambda>N).r8..
+00000f10: 00da 036c 656e 722f 0000 0072 2000 0000  ...lenr/...r ...
+00000f20: da06 6669 6c74 6572 da05 6c6f 7765 7272  ..filter..lowerr
+00000f30: 3f00 0000 7240 0000 0072 4100 0000 7242  ?...r@...rA...rB
+00000f40: 0000 0072 4300 0000 7244 0000 0072 1a00  ...rC...rD...r..
+00000f50: 0000 7227 0000 0029 0472 2900 0000 7245  ..r'...).r)...rE
+00000f60: 0000 005a 1270 6172 745f 6f66 5f73 7065  ...Z.part_of_spe
+00000f70: 6563 685f 7461 6772 1f00 0000 7225 0000  ech_tagr....r%..
+00000f80: 0072 2500 0000 7226 0000 00da 2170 6172  .r%...r&....!par
+00000f90: 745f 6f66 5f73 7065 6563 685f 6361 7465  t_of_speech_cate
+00000fa0: 676f 7279 5f77 6f72 6468 6970 706f 7100  gory_wordhippoq.
+00000fb0: 0000 7312 0000 0000 0a04 0102 0112 0112  ..s.............
+00000fc0: 010e 011e 011a 0120 017a 2e50 6172 744f  ....... .z.PartO
+00000fd0: 6653 7065 6563 682e 7061 7274 5f6f 665f  fSpeech.part_of_
+00000fe0: 7370 6565 6368 5f63 6174 6567 6f72 795f  speech_category_
+00000ff0: 776f 7264 6869 7070 6f4e 290a da08 5f5f  wordhippoN)...__
+00001000: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00001010: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00001020: da07 5f5f 646f 635f 5fda 0c73 7461 7469  ..__doc__..stati
+00001030: 636d 6574 686f 6472 2700 0000 720f 0000  cmethodr'...r...
+00001040: 00da 0373 7472 724b 0000 0072 5700 0000  ...strrK...rW...
+00001050: 7225 0000 0072 2500 0000 7225 0000 0072  r%...r%...r%...r
+00001060: 2600 0000 721a 0000 003c 0000 0073 0e00  &...r....<...s..
+00001070: 0000 0801 0410 0201 0a07 0201 121b 0201  ................
+00001080: 721a 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00001090: 0000 0000 0000 0500 0000 4000 0000 735a  ..........@...sZ
+000010a0: 0000 0065 005a 0164 005a 0264 015a 0365  ...e.Z.d.Z.d.Z.e
+000010b0: 0464 0264 0384 0083 015a 0565 0465 0665  .d.d.....Z.e.e.e
+000010c0: 0765 0864 049c 0364 0564 0684 0483 015a  .e.d...d.d.....Z
+000010d0: 0965 0465 0665 0864 079c 0264 0864 0984  .e.e.e.d...d.d..
+000010e0: 0483 015a 0a65 0465 0665 0864 079c 0264  ...Z.e.e.e.d...d
+000010f0: 0a64 0b84 0483 015a 0b64 0c53 0029 0dda  .d.....Z.d.S.)..
+00001100: 0a50 6172 7365 576f 7264 7361 7202 0000  .ParseWordsar...
+00001110: 0a20 2020 2020 2020 2041 2075 7469 6c69  .        A utili
+00001120: 7479 2063 6c61 7373 2066 6f72 2070 6172  ty class for par
+00001130: 7369 6e67 2061 6e74 6f6e 796d 7320 6672  sing antonyms fr
+00001140: 6f6d 2076 6172 696f 7573 206f 6e6c 696e  om various onlin
+00001150: 6520 736f 7572 6365 732e 0a0a 2020 2020  e sources...    
+00001160: 2020 2020 5468 6973 2063 6c61 7373 2063      This class c
+00001170: 6f6e 7461 696e 7320 7374 6174 6963 206d  ontains static m
+00001180: 6574 686f 6473 2074 6f20 7061 7273 6520  ethods to parse 
+00001190: 616e 746f 6e79 6d73 2066 726f 6d20 4854  antonyms from HT
+000011a0: 4d4c 2072 6573 706f 6e73 6573 206f 6620  ML responses of 
+000011b0: 7661 7269 6f75 7320 736f 7572 6365 732c  various sources,
+000011c0: 0a20 2020 2020 2020 2077 6869 6368 2061  .        which a
+000011d0: 7265 2054 6865 7361 7572 7573 2e63 6f6d  re Thesaurus.com
+000011e0: 2061 6e64 2057 6f72 6448 6970 706f 2e0a   and WordHippo..
+000011f0: 0a20 2020 2020 2020 204d 6574 686f 6473  .        Methods
+00001200: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00001210: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
+00001220: 5f71 7565 7279 5f65 7863 6570 7469 6f6e  _query_exception
+00001230: 7328 6572 726f 7229 3a0a 2020 2020 2020  s(error):.      
+00001240: 2020 2020 2020 4865 6c70 6572 206d 6574        Helper met
+00001250: 686f 6420 746f 2068 616e 646c 6520 636f  hod to handle co
+00001260: 6d6d 6f6e 2065 7863 6570 7469 6f6e 7320  mmon exceptions 
+00001270: 696e 2071 7565 7279 206d 6574 686f 6473  in query methods
+00001280: 2e0a 0a20 2020 2020 2020 2070 6172 7365  ...        parse
+00001290: 5f74 6865 7361 7572 7573 5f63 6f6d 2873  _thesaurus_com(s
+000012a0: 6f75 703a 2042 6561 7574 6966 756c 536f  oup: BeautifulSo
+000012b0: 7570 2920 2d3e 206c 6973 743a 0a20 2020  up) -> list:.   
+000012c0: 2020 2020 2020 2020 2050 6172 7365 7320           Parses 
+000012d0: 616e 746f 6e79 6d73 2066 726f 6d20 7468  antonyms from th
+000012e0: 6520 4854 4d4c 2072 6573 706f 6e73 6520  e HTML response 
+000012f0: 6f66 2054 6865 7361 7572 7573 2e63 6f6d  of Thesaurus.com
+00001300: 2e0a 0a20 2020 2020 2020 2070 6172 7365  ...        parse
+00001310: 5f77 6f72 6468 6970 706f 2873 6f75 703a  _wordhippo(soup:
+00001320: 2042 6561 7574 6966 756c 536f 7570 2920   BeautifulSoup) 
+00001330: 2d3e 206c 6973 743a 0a20 2020 2020 2020  -> list:.       
+00001340: 2020 2020 2050 6172 7365 7320 616e 746f       Parses anto
+00001350: 6e79 6d73 2066 726f 6d20 7468 6520 4854  nyms from the HT
+00001360: 4d4c 2072 6573 706f 6e73 6520 6f66 2057  ML response of W
+00001370: 6f72 6448 6970 706f 2e0a 2020 2020 2020  ordHippo..      
+00001380: 2020 6301 0000 0000 0000 0000 0000 0001    c.............
+00001390: 0000 0007 0000 0043 0000 0073 2600 0000  .......C...s&...
+000013a0: 7400 a001 6401 a101 0100 7400 a001 6402  t...d.....t...d.
+000013b0: a002 7403 a004 7c00 6a05 a101 a101 a101  ..t...|.j.......
+000013c0: 0100 6403 5300 721b 0000 0072 1d00 0000  ..d.S.r....r....
+000013d0: 7224 0000 0072 2500 0000 7225 0000 0072  r$...r%...r%...r
+000013e0: 2600 0000 7227 0000 0098 0000 0073 0400  &...r'.......s..
+000013f0: 0000 0005 0a01 7a23 5061 7273 6557 6f72  ......z#ParseWor
+00001400: 6473 2e5f 6861 6e64 6c65 5f71 7565 7279  ds._handle_query
+00001410: 5f65 7863 6570 7469 6f6e 7329 0372 2900  _exceptions).r).
+00001420: 0000 da04 776f 7264 722a 0000 0063 0200  ....wordr*...c..
+00001430: 0000 0000 0000 0000 0000 0900 0000 0c00  ................
+00001440: 0000 4300 0000 73a0 0000 0067 007d 027a  ..C...s....g.}.z
+00001450: 5c7c 006a 0064 0164 027c 019b 0064 039d  \|.j.d.d.|...d..
+00001460: 0364 048d 027d 037c 0372 5e7c 036a 0164  .d...}.|.r^|.j.d
+00001470: 0164 058d 017d 047c 046a 0064 0664 058d  .d...}.|.j.d.d..
+00001480: 017d 057c 0572 5e7c 056a 0264 0764 058d  .}.|.r^|.j.d.d..
+00001490: 017d 067c 0644 005d 107d 077c 02a0 037c  .}.|.D.].}.|...|
+000014a0: 076a 04a1 0101 0071 4c57 006e 3a04 0074  .j.....qLW.n:..t
+000014b0: 056a 0674 0774 0874 0974 0a66 0579 9a01  .j.t.t.t.t.f.y..
+000014c0: 007d 0801 007a 1674 0ba0 0c7c 08a1 0101  .}...z.t...|....
+000014d0: 0057 0059 0064 087d 087e 086e 0a64 087d  .W.Y.d.}.~.n.d.}
+000014e0: 087e 0830 0030 007c 0253 0029 0961 5b01  .~.0.0.|.S.).a[.
+000014f0: 0000 0a20 2020 2020 2020 2050 6172 7365  ...        Parse
+00001500: 7320 7379 6e6f 6e79 6d73 2066 726f 6d20  s synonyms from 
+00001510: 7468 6520 4854 4d4c 2072 6573 706f 6e73  the HTML respons
+00001520: 6520 6f66 2054 6865 7361 7572 7573 2e63  e of Thesaurus.c
+00001530: 6f6d 2e0a 0a20 2020 2020 2020 203a 7061  om...        :pa
+00001540: 7261 6d20 736f 7570 3a20 4265 6175 7469  ram soup: Beauti
+00001550: 6675 6c53 6f75 7020 6f62 6a65 6374 2063  fulSoup object c
+00001560: 6f6e 7461 696e 696e 6720 7468 6520 4854  ontaining the HT
+00001570: 4d4c 2072 6573 706f 6e73 650a 2020 2020  ML response.    
+00001580: 2020 2020 3a70 6172 616d 2074 7970 6520      :param type 
+00001590: 736f 7570 3a20 6273 342e 4265 6175 7469  soup: bs4.Beauti
+000015a0: 6675 6c53 6f75 700a 2020 2020 2020 2020  fulSoup.        
+000015b0: 3a70 6172 616d 2077 6f72 643a 2077 6f72  :param word: wor
+000015c0: 6420 746f 2073 6561 7263 680a 2020 2020  d to search.    
+000015d0: 2020 2020 3a70 6172 616d 2074 7970 6520      :param type 
+000015e0: 776f 7264 3a20 7374 7269 6e67 0a20 2020  word: string.   
+000015f0: 2020 2020 203a 7265 7475 726e 3a20 4c69       :return: Li
+00001600: 7374 206f 6620 7379 6e6f 6e79 6d73 2065  st of synonyms e
+00001610: 7874 7261 6374 6564 2066 726f 6d20 7468  xtracted from th
+00001620: 6520 4854 4d4c 2072 6573 706f 6e73 650a  e HTML response.
+00001630: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00001640: 6c69 7374 0a20 2020 2020 2020 2072 4c00  list.        rL.
+00001650: 0000 7a18 5768 6174 2069 7320 7468 6520  ..z.What is the 
+00001660: 6f70 706f 7369 7465 206f 6620 fa01 3fa9  opposite of ..?.
+00001670: 0272 2e00 0000 7233 0000 00a9 0172 2e00  .r....r3.....r..
+00001680: 0000 da05 7461 626c 65da 0274 644e 290d  ....table..tdN).
+00001690: 7238 0000 005a 1166 696e 645f 6e65 7874  r8...Z.find_next
+000016a0: 5f73 6962 6c69 6e67 da08 6669 6e64 5f61  _sibling..find_a
+000016b0: 6c6c da06 6170 7065 6e64 722f 0000 0072  ll..appendr/...r
+000016c0: 3f00 0000 7240 0000 0072 4100 0000 7242  ?...r@...rA...rB
+000016d0: 0000 0072 4300 0000 7244 0000 0072 5e00  ...rC...rD...r^.
+000016e0: 0000 7227 0000 0029 0972 2900 0000 725f  ..r'...).r)...r_
+000016f0: 0000 00da 0d61 6e74 6f6e 796d 735f 6c69  .....antonyms_li
+00001700: 7374 5a0b 6469 765f 656c 656d 656e 745a  stZ.div_elementZ
+00001710: 086e 6578 745f 6469 765a 0974 6162 6c65  .next_divZ.table
+00001720: 5f74 6167 5a0b 7464 5f65 6c65 6d65 6e74  _tagZ.td_element
+00001730: 735a 0a74 645f 656c 656d 656e 7472 1f00  sZ.td_elementr..
+00001740: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
+00001750: 00da 1070 6172 7365 5f67 6f6f 676c 655f  ...parse_google_
+00001760: 636f 6da0 0000 0073 1a00 0000 000c 0401  com....s........
+00001770: 0201 1601 0401 0c01 0c01 0401 0c01 0801  ................
+00001780: 1201 1a01 2001 7a1b 5061 7273 6557 6f72  .... .z.ParseWor
+00001790: 6473 2e70 6172 7365 5f67 6f6f 676c 655f  ds.parse_google_
+000017a0: 636f 6d72 2800 0000 6301 0000 0000 0000  comr(...c.......
+000017b0: 0000 0000 000c 0000 000c 0000 0043 0000  .............C..
+000017c0: 0073 f800 0000 6700 7d01 7ab4 6401 7d02  .s....g.}.z.d.}.
+000017d0: 6402 7d03 7c00 6a00 6403 7401 a002 7c02  d.}.|.j.d.t...|.
+000017e0: a101 6404 8d02 7d04 7c04 72b6 7401 6a03  ..d...}.|.r.t.j.
+000017f0: 7c02 9b00 6405 7c03 9b00 9d03 7c04 6a04  |...d.|.....|.j.
+00001800: 6406 8d02 7d05 7c05 72b6 7c05 a005 6407  d...}.|.r.|...d.
+00001810: a101 a006 6408 a101 7d06 7c06 a007 6409  ....d...}.|...d.
+00001820: 640a a102 7d06 7401 6a03 640b 7c06 6406  d...}.t.j.d.|.d.
+00001830: 8d02 7d07 7c07 72b6 7401 6a03 640c 7c07  ..}.|.r.t.j.d.|.
+00001840: a005 640d a101 6406 8d02 7d08 7c08 72b6  ..d...d...}.|.r.
+00001850: 640e 7d09 7401 6a03 7c09 7c08 a005 640d  d.}.t.j.|.|...d.
+00001860: a101 6406 8d02 7d0a 7c0a 72b6 7c01 a008  ..d...}.|.r.|...
+00001870: 7c0a a005 6407 a101 a101 0100 5700 6e3a  |...d.......W.n:
+00001880: 0400 7409 6a0a 740b 740c 740d 740e 6605  ..t.j.t.t.t.t.f.
+00001890: 79f2 0100 7d0b 0100 7a16 740f a010 7c0b  y...}...z.t...|.
+000018a0: a101 0100 5700 5900 640f 7d0b 7e0b 6e0a  ....W.Y.d.}.~.n.
+000018b0: 640f 7d0b 7e0b 3000 3000 7c01 5300 2910  d.}.~.0.0.|.S.).
+000018c0: 6116 0100 000a 2020 2020 2020 2020 5061  a.....        Pa
+000018d0: 7273 6573 2073 796e 6f6e 796d 7320 6672  rses synonyms fr
+000018e0: 6f6d 2074 6865 2048 544d 4c20 7265 7370  om the HTML resp
+000018f0: 6f6e 7365 206f 6620 5468 6573 6175 7275  onse of Thesauru
+00001900: 732e 636f 6d2e 0a0a 2020 2020 2020 2020  s.com...        
+00001910: 3a70 6172 616d 2073 6f75 703a 2042 6561  :param soup: Bea
+00001920: 7574 6966 756c 536f 7570 206f 626a 6563  utifulSoup objec
+00001930: 7420 636f 6e74 6169 6e69 6e67 2074 6865  t containing the
+00001940: 2048 544d 4c20 7265 7370 6f6e 7365 0a20   HTML response. 
+00001950: 2020 2020 2020 203a 7061 7261 6d20 7479         :param ty
+00001960: 7065 2073 6f75 703a 2062 7334 2e42 6561  pe soup: bs4.Bea
+00001970: 7574 6966 756c 536f 7570 0a20 2020 2020  utifulSoup.     
+00001980: 2020 203a 7265 7475 726e 3a20 4c69 7374     :return: List
+00001990: 206f 6620 7379 6e6f 6e79 6d73 2065 7874   of synonyms ext
+000019a0: 7261 6374 6564 2066 726f 6d20 7468 6520  racted from the 
+000019b0: 4854 4d4c 2072 6573 706f 6e73 650a 2020  HTML response.  
+000019c0: 2020 2020 2020 3a72 7479 7065 3a20 6c69        :rtype: li
+000019d0: 7374 0a20 2020 2020 2020 2072 2b00 0000  st.        r+...
+000019e0: 722c 0000 0072 2d00 0000 7261 0000 0072  r,...r-...ra...r
+000019f0: 3000 0000 7231 0000 0072 3400 0000 7235  0...r1...r4...r5
+00001a00: 0000 0072 3600 0000 7237 0000 007a 145c  ...r6...r7...z.\
+00001a10: 5b7b 2261 6e74 6f6e 796d 7322 3a2e 2a3f  [{"antonyms":.*?
+00001a20: 7d5c 5d7a 1c5c 7b22 7369 6d69 6c61 7269  }\]z.\{"similari
+00001a30: 7479 223a 2d31 302c 5b5e 7d5d 2a5c 7d5c  ty":-10,[^}]*\}\
+00001a40: 5d72 0300 0000 7a1c 2274 6172 6765 7457  ]r....z."targetW
+00001a50: 6f72 6422 5c73 2a3a 5c73 2a22 285b 5e22  ord"\s*:\s*"([^"
+00001a60: 5d2b 2922 4e29 1172 3800 0000 7239 0000  ]+)"N).r8...r9..
+00001a70: 0072 3a00 0000 723b 0000 0072 3300 0000  .r:...r;...r3...
+00001a80: 723c 0000 0072 3d00 0000 723e 0000 0072  r<...r=...r>...r
+00001a90: 6600 0000 723f 0000 0072 4000 0000 7241  f...r?...r@...rA
+00001aa0: 0000 0072 4200 0000 7243 0000 0072 4400  ...rB...rC...rD.
+00001ab0: 0000 725e 0000 0072 2700 0000 290c 7229  ..r^...r'...).r)
+00001ac0: 0000 0072 6700 0000 7246 0000 0072 4700  ...rg...rF...rG.
+00001ad0: 0000 7248 0000 0072 4900 0000 724a 0000  ..rH...rI...rJ..
+00001ae0: 005a 0f61 6e74 6f6e 796d 5f73 6563 7469  .Z.antonym_secti
+00001af0: 6f6e 5a1b 616e 746f 6e79 6d73 5f73 696d  onZ.antonyms_sim
+00001b00: 696c 6172 6974 795f 7365 6374 696f 6e5a  ilarity_sectionZ
+00001b10: 0e74 6172 6765 745f 7061 7474 6572 6e5a  .target_patternZ
+00001b20: 0e74 6172 6765 745f 616e 746f 6e79 6d72  .target_antonymr
+00001b30: 1f00 0000 7225 0000 0072 2500 0000 7226  ....r%...r%...r&
+00001b40: 0000 00da 1370 6172 7365 5f74 6865 7361  .....parse_thesa
+00001b50: 7572 7573 5f63 6f6d ba00 0000 7332 0000  urus_com....s2..
+00001b60: 0000 0a04 0102 0104 0104 0114 0104 011a  ................
+00001b70: 0104 0110 010c 010e 0104 0106 0108 ff06  ................
+00001b80: 0204 0104 0106 0108 ff06 0204 0114 011a  ................
+00001b90: 0120 017a 1e50 6172 7365 576f 7264 732e  . .z.ParseWords.
+00001ba0: 7061 7273 655f 7468 6573 6175 7275 735f  parse_thesaurus_
+00001bb0: 636f 6d63 0100 0000 0000 0000 0000 0000  comc............
+00001bc0: 0800 0000 0c00 0000 4300 0000 73ea 0000  ........C...s...
+00001bd0: 0067 007d 017a 987c 006a 0064 0164 0264  .g.}.z.|.j.d.d.d
+00001be0: 0369 0164 048d 027d 027c 026a 0064 0164  .i.d...}.|.j.d.d
+00001bf0: 0264 0569 0164 048d 0264 0675 0172 687c  .d.i.d...d.u.rh|
+00001c00: 026a 0164 0164 0264 0569 0164 048d 0244  .j.d.d.d.i.d...D
+00001c10: 005d 247d 037c 036a 0164 0764 0864 098d  .]$}.|.j.d.d.d..
+00001c20: 0244 005d 107d 047c 01a0 027c 046a 03a1  .D.].}.|...|.j..
+00001c30: 0101 0071 5271 406e 327c 026a 0164 0a64  ...qRq@n2|.j.d.d
+00001c40: 0b8d 0144 005d 247d 057c 056a 0064 0764  ...D.]$}.|.j.d.d
+00001c50: 0864 098d 0244 005d 107d 067c 01a0 027c  .d...D.].}.|...|
+00001c60: 066a 03a1 0101 0071 8671 7457 006e 3a04  .j.....q.qtW.n:.
+00001c70: 0074 046a 0574 0674 0774 0874 0966 0579  .t.j.t.t.t.t.f.y
+00001c80: d601 007d 0701 007a 1674 0aa0 0b7c 07a1  ...}...z.t...|..
+00001c90: 0101 0057 0059 0064 067d 077e 076e 0a64  ...W.Y.d.}.~.n.d
+00001ca0: 067d 077e 0730 0030 0074 0c64 0c64 0d84  .}.~.0.0.t.d.d..
+00001cb0: 007c 0144 0083 0183 0153 0029 0e61 1201  .|.D.....S.).a..
+00001cc0: 0000 0a20 2020 2020 2020 2050 6172 7365  ...        Parse
+00001cd0: 7320 7379 6e6f 6e79 6d73 2066 726f 6d20  s synonyms from 
+00001ce0: 7468 6520 4854 4d4c 2072 6573 706f 6e73  the HTML respons
+00001cf0: 6520 6f66 2057 6f72 6468 6970 706f 2e0a  e of Wordhippo..
+00001d00: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001d10: 736f 7570 3a20 4265 6175 7469 6675 6c53  soup: BeautifulS
+00001d20: 6f75 7020 6f62 6a65 6374 2063 6f6e 7461  oup object conta
+00001d30: 696e 696e 6720 7468 6520 4854 4d4c 2072  ining the HTML r
+00001d40: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
+00001d50: 3a70 6172 616d 2074 7970 6520 736f 7570  :param type soup
+00001d60: 3a20 6273 342e 4265 6175 7469 6675 6c53  : bs4.BeautifulS
+00001d70: 6f75 700a 2020 2020 2020 2020 3a72 6574  oup.        :ret
+00001d80: 7572 6e3a 204c 6973 7420 6f66 2061 6e74  urn: List of ant
+00001d90: 6f6e 796d 7320 6578 7472 6163 7465 6420  onyms extracted 
+00001da0: 6672 6f6d 2074 6865 2048 544d 4c20 7265  from the HTML re
+00001db0: 7370 6f6e 7365 0a20 2020 2020 2020 203a  sponse.        :
+00001dc0: 7274 7970 653a 206c 6973 740a 2020 2020  rtype: list.    
+00001dd0: 2020 2020 724c 0000 0072 4d00 0000 5a0c      rL...rM...Z.
+00001de0: 7265 6c61 7465 6477 6f72 6473 724e 0000  relatedwordsrN..
+00001df0: 00da 0277 624e da01 6154 2902 722e 0000  ...wbN..aT).r...
+00001e00: 005a 0468 7265 6672 6400 0000 7262 0000  .Z.hrefrd...rb..
+00001e10: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00001e20: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
+00001e30: 007c 005d 0c7d 017c 01a0 00a1 0091 0271  .|.].}.|.......q
+00001e40: 0453 0072 2500 0000 a901 7256 0000 00a9  .S.r%.....rV....
+00001e50: 02da 022e 3072 5100 0000 7225 0000 0072  ....0rQ...r%...r
+00001e60: 2500 0000 7226 0000 00da 0a3c 6c69 7374  %...r&.....<list
+00001e70: 636f 6d70 3ef3 0000 0072 5300 0000 7a2e  comp>....rS...z.
+00001e80: 5061 7273 6557 6f72 6473 2e70 6172 7365  ParseWords.parse
+00001e90: 5f77 6f72 6468 6970 706f 2e3c 6c6f 6361  _wordhippo.<loca
+00001ea0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 290d  ls>.<listcomp>).
+00001eb0: 7238 0000 0072 6500 0000 7266 0000 0072  r8...re...rf...r
+00001ec0: 2f00 0000 723f 0000 0072 4000 0000 7241  /...r?...r@...rA
+00001ed0: 0000 0072 4200 0000 7243 0000 0072 4400  ...rB...rC...rD.
+00001ee0: 0000 725e 0000 0072 2700 0000 da06 736f  ..r^...r'.....so
+00001ef0: 7274 6564 2908 7229 0000 0072 6700 0000  rted).r)...rg...
+00001f00: 5a0b 7265 6c61 7465 645f 7461 675a 096c  Z.related_tagZ.l
+00001f10: 6973 745f 6974 656d da04 6c69 6e6b 5a09  ist_item..linkZ.
+00001f20: 7461 626c 655f 726f 775a 0968 7265 665f  table_rowZ.href_
+00001f30: 6c69 6e6b 721f 0000 0072 2500 0000 7225  linkr....r%...r%
+00001f40: 0000 0072 2600 0000 da0f 7061 7273 655f  ...r&.....parse_
+00001f50: 776f 7264 6869 7070 6fdc 0000 0073 1a00  wordhippo....s..
+00001f60: 0000 000a 0401 0201 1201 1601 1601 1201  ................
+00001f70: 1202 1001 1201 1401 1a01 2001 7a1a 5061  .......... .z.Pa
+00001f80: 7273 6557 6f72 6473 2e70 6172 7365 5f77  rseWords.parse_w
+00001f90: 6f72 6468 6970 706f 4e29 0c72 5800 0000  ordhippoN).rX...
+00001fa0: 7259 0000 0072 5a00 0000 725b 0000 0072  rY...rZ...r[...r
+00001fb0: 5c00 0000 7227 0000 0072 0f00 0000 725d  \...r'...r....r]
+00001fc0: 0000 00da 046c 6973 7472 6800 0000 7269  .....listrh...ri
+00001fd0: 0000 0072 7200 0000 7225 0000 0072 2500  ...rr...r%...r%.
+00001fe0: 0000 7225 0000 0072 2600 0000 725e 0000  ..r%...r&...r^..
+00001ff0: 0085 0000 0073 1200 0000 0801 0412 0201  .....s..........
+00002000: 0a07 0201 1419 0201 1221 0201 725e 0000  .........!..r^..
+00002010: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00002020: 0000 0b00 0000 4000 0000 73a0 0100 0065  ......@...s....e
+00002030: 005a 0164 005a 0264 015a 0364 2665 0465  .Z.d.Z.d.Z.d&e.e
+00002040: 0565 0665 0419 0019 0065 0465 0765 0765  .e.e.....e.e.e.e
+00002050: 0565 0419 0065 0565 0865 0465 0466 0219  .e...e.e.e.e.f..
+00002060: 0019 0064 079c 0764 0864 0984 055a 0964  ...d...d.d...Z.d
+00002070: 0364 0a9c 0164 0b64 0c84 045a 0a65 0b64  .d...d.d...Z.e.d
+00002080: 0a9c 0164 0d64 0e84 045a 0c65 0d65 0b65  ...d.d...Z.e.e.e
+00002090: 0e65 0865 0465 0665 0419 0066 0219 0064  .e.e.e.e...f...d
+000020a0: 0366 0219 0066 0219 0064 0a9c 0164 0f64  .f...f...d...d.d
+000020b0: 1084 045a 0f65 0465 0e65 0665 0419 0065  ...Z.e.e.e.e...e
+000020c0: 1065 0419 0066 0219 0064 0364 119c 0364  .e...f...d.d...d
+000020d0: 1264 1384 045a 1165 0465 126a 136a 1464  .d...Z.e.e.j.j.d
+000020e0: 149c 0264 1564 1684 045a 1565 0665 1665  ...d.d...Z.e.e.e
+000020f0: 0665 0419 0065 0466 0219 0019 0064 0a9c  .e...e.f.....d..
+00002100: 0164 1764 1884 045a 1765 1865 0e65 1965  .d.d...Z.e.e.e.e
+00002110: 0419 0065 0466 0219 0065 0e65 1865 1a65  ...e.f...e.e.e.e
+00002120: 0466 0319 0064 199c 0364 1a64 1b84 045a  .f...d...d.d...Z
+00002130: 1b65 0e65 0665 1c19 0065 0865 0465 0665  .e.e.e...e.e.e.e
+00002140: 0419 0066 0219 0065 0466 0319 0064 0a9c  ...f...e.f...d..
+00002150: 0164 1c64 1d84 045a 1d65 1e64 1e64 1f84  .d.d...Z.e.d.d..
+00002160: 0083 015a 1f65 0e65 0d65 0665 0419 0065  ...Z.e.e.e.e...e
+00002170: 0466 0219 0064 0366 0219 0064 0a9c 0164  .f...d.f...d...d
+00002180: 2064 2184 045a 2065 0e65 0d65 0665 0419   d!..Z e.e.e.e..
+00002190: 0065 0466 0219 0064 0366 0219 0064 0a9c  .e.f...d.f...d..
+000021a0: 0164 2264 2384 045a 2165 0e65 0d65 0665  .d"d#..Z!e.e.e.e
+000021b0: 0419 0065 0466 0219 0064 0366 0219 0064  ...e.f...d.f...d
+000021c0: 0a9c 0164 2464 2584 045a 2264 0353 0029  ...d$d%..Z"d.S.)
+000021d0: 27da 0841 6e74 6f6e 796d 7361 be0b 0000  '..Antonymsa....
+000021e0: 0a20 2020 2020 2020 2041 2050 7974 686f  .        A Pytho
+000021f0: 6e20 636c 6173 7320 666f 7220 7175 6572  n class for quer
+00002200: 7969 6e67 206d 756c 7469 706c 6520 6f6e  ying multiple on
+00002210: 6c69 6e65 2072 6570 6f73 6974 6f72 6965  line repositorie
+00002220: 7320 746f 2066 696e 6420 616e 746f 6e79  s to find antony
+00002230: 6d73 2066 6f72 2061 2073 7065 6369 6669  ms for a specifi
+00002240: 6320 776f 7264 2e0a 0a20 2020 2020 2020  c word...       
+00002250: 2055 7361 6765 2045 7861 6d70 6c65 730a   Usage Examples.
+00002260: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00002270: 2d2d 0a20 2020 2020 2020 203e 3e3e 2061  --.        >>> a
+00002280: 6e74 6f6e 796d 203d 2041 6e74 6f6e 796d  ntonym = Antonym
+00002290: 7328 276d 6f74 6865 7227 290a 2020 2020  s('mother').    
+000022a0: 2020 2020 3e3e 3e20 7265 7375 6c74 7320      >>> results 
+000022b0: 3d20 616e 746f 6e79 6d2e 6669 6e64 5f61  = antonym.find_a
+000022c0: 6e74 6f6e 796d 7328 290a 0a20 2020 2020  ntonyms()..     
+000022d0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+000022e0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+000022f0: 0a20 2020 2020 2020 2073 6561 7263 685f  .        search_
+00002300: 7374 7269 6e67 203a 2073 7472 2c20 6f70  string : str, op
+00002310: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+00002320: 2020 2054 6865 2077 6f72 6420 666f 7220     The word for 
+00002330: 7768 6963 6820 616e 746f 6e79 6d73 2061  which antonyms a
+00002340: 7265 2074 6f20 6265 2066 6f75 6e64 2e0a  re to be found..
+00002350: 2020 2020 2020 2020 736f 7572 6365 733a          sources:
+00002360: 204f 7074 696f 6e61 6c5b 4c69 7374 5b73   Optional[List[s
+00002370: 7472 5d5d 0a20 2020 2020 2020 2020 2020  tr]].           
+00002380: 2054 6865 2073 6f75 7263 6573 2074 6f20   The sources to 
+00002390: 7365 6172 6368 2066 6f72 2061 6e74 6f6e  search for anton
+000023a0: 796d 732e 0a20 2020 2020 2020 206f 7574  yms..        out
+000023b0: 7075 745f 666f 726d 6174 203a 2073 7472  put_format : str
+000023c0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+000023d0: 2020 2020 2020 2046 6f72 6d61 7420 666f         Format fo
+000023e0: 7220 7265 7475 726e 6564 2072 6573 756c  r returned resul
+000023f0: 7473 2e20 4465 6661 756c 7420 6973 2027  ts. Default is '
+00002400: 6c69 7374 272e 2041 6363 6570 7461 626c  list'. Acceptabl
+00002410: 6520 7661 6c75 6573 2061 7265 2027 6469  e values are 'di
+00002420: 6374 696f 6e61 7279 272c 2027 6c69 7374  ctionary', 'list
+00002430: 272c 206f 7220 276a 736f 6e27 2e0a 2020  ', or 'json'..  
+00002440: 2020 2020 2020 6d61 785f 6e75 6d62 6572        max_number
+00002450: 5f6f 665f 7265 7175 6573 7473 203a 2069  _of_requests : i
+00002460: 6e74 2c20 6f70 7469 6f6e 616c 0a20 2020  nt, optional.   
+00002470: 2020 2020 2020 2020 204d 6178 696d 756d           Maximum
+00002480: 206e 756d 6265 7220 6f66 2072 6571 7565   number of reque
+00002490: 7374 7320 7769 7468 696e 2061 2073 7065  sts within a spe
+000024a0: 6369 6669 6564 2074 696d 6520 7065 7269  cified time peri
+000024b0: 6f64 2e0a 2020 2020 2020 2020 7261 7465  od..        rate
+000024c0: 5f6c 696d 6974 5f74 696d 656f 7574 5f70  _limit_timeout_p
+000024d0: 6572 696f 6420 3a20 696e 742c 206f 7074  eriod : int, opt
+000024e0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+000024f0: 2020 5469 6d65 2070 6572 696f 6420 6265    Time period be
+00002500: 666f 7265 2074 656d 706f 7261 7279 2068  fore temporary h
+00002510: 6962 6572 6e61 7469 6f6e 2064 7565 2074  ibernation due t
+00002520: 6f20 7261 7465 206c 696d 6974 696e 672e  o rate limiting.
+00002530: 0a20 2020 2020 2020 2075 7365 725f 6167  .        user_ag
+00002540: 656e 7420 3a20 7374 722c 206f 7074 696f  ent : str, optio
+00002550: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+00002560: 5573 6572 2061 6765 6e74 2073 7472 696e  User agent strin
+00002570: 6720 666f 7220 4854 5450 2072 6571 7565  g for HTTP reque
+00002580: 7374 732e 0a20 2020 2020 2020 2070 726f  sts..        pro
+00002590: 7869 6573 203a 2064 6963 742c 206f 7074  xies : dict, opt
+000025a0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+000025b0: 2020 4469 6374 696f 6e61 7279 206f 6620    Dictionary of 
+000025c0: 7072 6f78 6965 7320 666f 7220 5079 7468  proxies for Pyth
+000025d0: 6f6e 2052 6571 7565 7374 732e 0a0a 2020  on Requests...  
+000025e0: 2020 2020 2020 4174 7472 6962 7574 6573        Attributes
+000025f0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00002600: 2d2d 2d0a 2020 2020 2020 2020 5f70 726f  ---.        _pro
+00002610: 7869 6573 203a 204f 7074 696f 6e61 6c5b  xies : Optional[
+00002620: 4469 6374 5b73 7472 2c20 7374 725d 5d0a  Dict[str, str]].
+00002630: 2020 2020 2020 2020 2020 2020 5072 6f78              Prox
+00002640: 6965 7320 746f 2075 7365 2077 6974 6820  ies to use with 
+00002650: 5079 7468 6f6e 2052 6571 7565 7374 732e  Python Requests.
+00002660: 0a20 2020 2020 2020 205f 776f 7264 203a  .        _word :
+00002670: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
+00002680: 2054 6865 2077 6f72 6420 746f 2066 696e   The word to fin
+00002690: 6420 616e 746f 6e79 6d73 2066 6f72 2e0a  d antonyms for..
+000026a0: 2020 2020 2020 2020 205f 736f 7572 6365           _source
+000026b0: 7320 3a20 4f70 7469 6f6e 616c 5b4c 6973  s : Optional[Lis
+000026c0: 745b 7374 725d 5d0a 2020 2020 2020 2020  t[str]].        
+000026d0: 2020 2020 5468 6520 736f 7572 6365 7320      The sources 
+000026e0: 746f 2073 6561 7263 6820 666f 7220 616e  to search for an
+000026f0: 746f 6e79 6d73 2e0a 2020 2020 2020 2020  tonyms..        
+00002700: 5f75 7365 725f 6167 656e 7420 3a20 4f70  _user_agent : Op
+00002710: 7469 6f6e 616c 5b73 7472 5d0a 2020 2020  tional[str].    
+00002720: 2020 2020 2020 2020 5573 6572 2061 6765          User age
+00002730: 6e74 2066 6f72 2048 5454 5020 7265 7175  nt for HTTP requ
+00002740: 6573 7473 2e0a 2020 2020 2020 2020 5f6f  ests..        _o
+00002750: 7574 7075 745f 666f 726d 6174 203a 2073  utput_format : s
+00002760: 7472 0a20 2020 2020 2020 2020 2020 2046  tr.            F
+00002770: 6f72 6d61 7420 666f 7220 7265 7475 726e  ormat for return
+00002780: 6564 2072 6573 756c 7473 2e0a 2020 2020  ed results..    
+00002790: 2020 2020 5f76 616c 6964 5f6f 7574 7075      _valid_outpu
+000027a0: 745f 666f 726d 6174 7320 3a20 5365 745b  t_formats : Set[
+000027b0: 7374 725d 0a20 2020 2020 2020 2020 2020  str].           
+000027c0: 2053 6574 206f 6620 7661 6c69 6420 6f75   Set of valid ou
+000027d0: 7470 7574 2066 6f72 6d61 7473 2e0a 2020  tput formats..  
+000027e0: 2020 2020 2020 5f72 6174 655f 6c69 6d69        _rate_limi
+000027f0: 745f 7374 6174 7573 203a 2062 6f6f 6c0a  t_status : bool.
+00002800: 2020 2020 2020 2020 2020 2020 5374 6174              Stat
+00002810: 7573 2069 6e64 6963 6174 696e 6720 7768  us indicating wh
+00002820: 6574 6865 7220 7261 7465 206c 696d 6974  ether rate limit
+00002830: 2069 7320 7265 6163 6865 642e 0a0a 2020   is reached...  
+00002840: 2020 2020 2020 4d65 7468 6f64 730a 2020        Methods.  
+00002850: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+00002860: 2020 2020 2020 6669 6e64 5f61 6e74 6f6e        find_anton
+00002870: 796d 7328 2920 2d3e 2055 6e69 6f6e 5b4c  yms() -> Union[L
+00002880: 6973 745b 5369 7a65 645d 2c20 4469 6374  ist[Sized], Dict
+00002890: 5b73 7472 2c20 4c69 7374 5b73 7472 5d5d  [str, List[str]]
+000028a0: 2c20 7374 725d 3a0a 2020 2020 2020 2020  , str]:.        
+000028b0: 2020 2020 4669 6e64 7320 616e 746f 6e79      Finds antony
+000028c0: 6d73 2066 6f72 2074 6865 2073 7065 6369  ms for the speci
+000028d0: 6669 6564 2077 6f72 642e 0a20 2020 2020  fied word..     
+000028e0: 2020 205f 7661 6c69 6461 7465 5f77 6f72     _validate_wor
+000028f0: 6428 2920 2d3e 2062 6f6f 6c3a 0a20 2020  d() -> bool:.   
+00002900: 2020 2020 2020 2020 2056 616c 6964 6174           Validat
+00002910: 6573 2074 6865 2073 796e 7461 7820 6f66  es the syntax of
+00002920: 2074 6865 2077 6f72 642e 0a20 2020 2020   the word..     
+00002930: 2020 205f 6368 6563 6b5f 6361 6368 6528     _check_cache(
+00002940: 2920 2d3e 2054 7570 6c65 5b62 6f6f 6c2c  ) -> Tuple[bool,
+00002950: 2055 6e69 6f6e 5b44 6963 745b 7374 722c   Union[Dict[str,
+00002960: 204c 6973 745b 7374 725d 5d2c 204e 6f6e   List[str]], Non
+00002970: 655d 5d3a 0a20 2020 2020 2020 2020 2020  e]]:.           
+00002980: 2043 6865 636b 7320 6966 2061 6e74 6f6e   Checks if anton
+00002990: 796d 7320 6172 6520 6361 6368 6564 2e0a  yms are cached..
+000029a0: 2020 2020 2020 2020 5f75 7064 6174 655f          _update_
+000029b0: 6361 6368 6528 706f 735f 6361 7465 676f  cache(pos_catego
+000029c0: 7279 3a20 7374 722c 2061 6e74 6f6e 796d  ry: str, antonym
+000029d0: 733a 2055 6e69 6f6e 5b4c 6973 745b 7374  s: Union[List[st
+000029e0: 725d 2c20 5365 745b 7374 725d 5d29 202d  r], Set[str]]) -
+000029f0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00002a00: 2020 2020 5570 6461 7465 7320 7468 6520      Updates the 
+00002a10: 6361 6368 6520 7769 7468 206e 6577 2061  cache with new a
+00002a20: 6e74 6f6e 796d 732e 0a20 2020 2020 2020  ntonyms..       
+00002a30: 205f 7265 7175 6573 745f 6874 7470 5f72   _request_http_r
+00002a40: 6573 706f 6e73 6528 7572 6c3a 2073 7472  esponse(url: str
+00002a50: 2920 2d3e 2072 6571 7565 7374 732e 6d6f  ) -> requests.mo
+00002a60: 6465 6c73 2e52 6573 706f 6e73 653a 0a20  dels.Response:. 
+00002a70: 2020 2020 2020 2020 2020 204d 616b 6573             Makes
+00002a80: 2061 6e20 4854 5450 2072 6571 7565 7374   an HTTP request
+00002a90: 2061 6e64 2072 6574 7572 6e73 2074 6865   and returns the
+00002aa0: 2072 6573 706f 6e73 652e 0a20 2020 2020   response..     
+00002ab0: 2020 205f 7275 6e5f 7175 6572 795f 7461     _run_query_ta
+00002ac0: 736b 735f 696e 5f70 6172 616c 6c65 6c28  sks_in_parallel(
+00002ad0: 2920 2d3e 204c 6973 745b 7475 706c 655b  ) -> List[tuple[
+00002ae0: 4c69 7374 5b73 7472 5d2c 2073 7472 5d5d  List[str], str]]
+00002af0: 3a0a 2020 2020 2020 2020 2020 2020 5275  :.            Ru
+00002b00: 6e73 2071 7565 7279 2074 6173 6b73 2069  ns query tasks i
+00002b10: 6e20 7061 7261 6c6c 656c 2075 7369 6e67  n parallel using
+00002b20: 2061 2054 6872 6561 6450 6f6f 6c2e 0a20   a ThreadPool.. 
+00002b30: 2020 2020 2020 205f 7175 6572 795f 6f75         _query_ou
+00002b40: 7470 7574 2873 656c 662c 2061 6e74 6f6e  tput(self, anton
+00002b50: 796d 733a 206c 6973 742c 2070 6172 745f  yms: list, part_
+00002b60: 6f66 5f73 7065 6563 683a 2055 6e69 6f6e  of_speech: Union
+00002b70: 5b73 6574 5b73 7472 5d2c 2073 7472 5d29  [set[str], str])
+00002b80: 202d 3e20 556e 696f 6e5b 6c69 7374 2c20   -> Union[list, 
+00002b90: 6469 6374 2c20 7374 725d 3a0a 2020 2020  dict, str]:.    
+00002ba0: 2020 2020 2020 2020 5072 6f63 6573 7320          Process 
+00002bb0: 7468 6520 6f75 7470 7574 2066 6f72 6d61  the output forma
+00002bc0: 7420 6261 7365 6420 6f6e 2074 6865 2073  t based on the s
+00002bd0: 7065 6369 6669 6564 2066 6f72 6d61 742e  pecified format.
+00002be0: 0a20 2020 2020 2020 205f 6861 6e64 6c65  .        _handle
+00002bf0: 5f71 7565 7279 5f65 7863 6570 7469 6f6e  _query_exception
+00002c00: 7328 6572 726f 7229 3a0a 2020 2020 2020  s(error):.      
+00002c10: 2020 2020 2020 4861 6e64 6c65 7320 636f        Handles co
+00002c20: 6d6d 6f6e 2065 7863 6570 7469 6f6e 7320  mmon exceptions 
+00002c30: 696e 2071 7565 7279 206d 6574 686f 6473  in query methods
+00002c40: 2e0a 2020 2020 2020 2020 5f71 7565 7279  ..        _query
+00002c50: 5f67 6f6f 676c 655f 636f 6d28 2920 2d3e  _google_com() ->
+00002c60: 2055 6e69 6f6e 5b54 7570 6c65 5b4c 6973   Union[Tuple[Lis
+00002c70: 745b 7374 725d 2c20 7374 725d 2c20 4e6f  t[str], str], No
+00002c80: 6e65 5d3a 0a20 2020 2020 2020 2020 2020  ne]:.           
+00002c90: 2051 7565 7269 6573 2067 6f6f 676c 652e   Queries google.
+00002ca0: 636f 6d20 666f 7220 616e 746f 6e79 6d73  com for antonyms
+00002cb0: 2e0a 2020 2020 2020 2020 5f71 7565 7279  ..        _query
+00002cc0: 5f74 6865 7361 7572 7573 5f63 6f6d 2829  _thesaurus_com()
+00002cd0: 202d 3e20 556e 696f 6e5b 5475 706c 655b   -> Union[Tuple[
+00002ce0: 4c69 7374 5b73 7472 5d2c 2073 7472 5d2c  List[str], str],
+00002cf0: 204e 6f6e 655d 3a0a 2020 2020 2020 2020   None]:.        
+00002d00: 2020 2020 5175 6572 6965 7320 7468 6573      Queries thes
+00002d10: 6175 7275 732e 636f 6d20 666f 7220 616e  aurus.com for an
+00002d20: 746f 6e79 6d73 2e0a 2020 2020 2020 2020  tonyms..        
+00002d30: 5f71 7565 7279 5f77 6f72 6468 6970 706f  _query_wordhippo
+00002d40: 2829 202d 3e20 556e 696f 6e5b 5475 706c  () -> Union[Tupl
+00002d50: 655b 4c69 7374 5b73 7472 5d2c 2073 7472  e[List[str], str
+00002d60: 5d2c 204e 6f6e 655d 3a0a 2020 2020 2020  ], None]:.      
+00002d70: 2020 2020 2020 5175 6572 6965 7320 776f        Queries wo
+00002d80: 7264 6869 7070 6f20 666f 7220 616e 746f  rdhippo for anto
+00002d90: 6e79 6d73 2e0a 2020 2020 2020 2020 721c  nyms..        r.
+00002da0: 0000 004e 7273 0000 00e9 1e00 0000 e93c  ...Nrs.........<
+00002db0: 0000 0029 07da 0d73 6561 7263 685f 7374  ...)...search_st
+00002dc0: 7269 6e67 da07 736f 7572 6365 73da 0d6f  ring..sources..o
+00002dd0: 7574 7075 745f 666f 726d 6174 da16 6d61  utput_format..ma
+00002de0: 785f 6e75 6d62 6572 5f6f 665f 7265 7175  x_number_of_requ
+00002df0: 6573 7473 da19 7261 7465 5f6c 696d 6974  ests..rate_limit
+00002e00: 5f74 696d 656f 7574 5f70 6572 696f 64da  _timeout_period.
+00002e10: 0a75 7365 725f 6167 656e 74da 0770 726f  .user_agent..pro
+00002e20: 7869 6573 6308 0000 0000 0000 0000 0000  xiesc...........
+00002e30: 000b 0000 0006 0000 0043 0000 0073 6400  .........C...sd.
+00002e40: 0000 7c07 7c00 5f00 7c01 7c00 5f01 7c06  ..|.|._.|.|._.|.
+00002e50: 7c00 5f02 7c03 7c00 5f03 6800 6401 a301  |._.|.|._.h.d...
+00002e60: 7c00 5f04 7c02 7c00 5f05 6402 7d08 7c08  |._.|.|._.d.}.|.
+00002e70: 7c00 5f06 7407 7408 7409 6403 7c00 6a0a  |._.t.t.t.d.|.j.
+00002e80: 6404 8d04 7d09 740b 7c04 7c05 6405 8d02  d...}.t.|.|.d...
+00002e90: 7d0a 7c09 7c0a 7c00 6a0c 8301 8301 7c00  }.|.|.|.j.....|.
+00002ea0: 5f0c 6400 5300 2906 4e3e 0300 0000 7273  _.d.S.).N>....rs
+00002eb0: 0000 00da 046a 736f 6eda 0a64 6963 7469  .....json..dicti
+00002ec0: 6f6e 6172 7946 7276 0000 0029 045a 0877  onaryFrv...).Z.w
+00002ed0: 6169 745f 6765 6eda 0965 7863 6570 7469  ait_gen..excepti
+00002ee0: 6f6e 5a08 6d61 785f 7469 6d65 5a0a 6f6e  onZ.max_timeZ.on
+00002ef0: 5f62 6163 6b6f 6666 2902 5a05 6361 6c6c  _backoff).Z.call
+00002f00: 735a 0670 6572 696f 6429 0dda 085f 7072  sZ.period)..._pr
+00002f10: 6f78 6965 73da 055f 776f 7264 da0b 5f75  oxies.._word.._u
+00002f20: 7365 725f 6167 656e 74da 0e5f 6f75 7470  ser_agent.._outp
+00002f30: 7574 5f66 6f72 6d61 74da 155f 7661 6c69  ut_format.._vali
+00002f40: 645f 6f75 7470 7574 5f66 6f72 6d61 7473  d_output_formats
+00002f50: da08 5f73 6f75 7263 6573 da12 5f72 6174  .._sources.._rat
+00002f60: 655f 6c69 6d69 745f 7374 6174 7573 7210  e_limit_statusr.
+00002f70: 0000 0072 1100 0000 7213 0000 00da 105f  ...r....r......_
+00002f80: 6261 636b 6f66 665f 6861 6e64 6c65 7272  backoff_handlerr
+00002f90: 1200 0000 da1c 5f72 756e 5f71 7565 7279  ......_run_query
+00002fa0: 5f74 6173 6b73 5f69 6e5f 7061 7261 6c6c  _tasks_in_parall
+00002fb0: 656c 290b da04 7365 6c66 7277 0000 0072  el)...selfrw...r
+00002fc0: 7800 0000 7279 0000 0072 7a00 0000 727b  x...ry...rz...r{
+00002fd0: 0000 0072 7c00 0000 727d 0000 005a 1172  ...r|...r}...Z.r
+00002fe0: 6174 655f 6c69 6d69 745f 7374 6174 7573  ate_limit_status
+00002ff0: da07 6861 6e64 6c65 725a 076c 696d 6974  ..handlerZ.limit
+00003000: 6572 7225 0000 0072 2500 0000 7226 0000  err%...r%...r&..
+00003010: 00da 085f 5f69 6e69 745f 5f3a 0100 0073  ...__init__:...s
+00003020: 1e00 0000 0009 0601 0601 0601 0601 0a01  ................
+00003030: 0602 0401 0603 0401 0201 0201 04fd 0605  ................
+00003040: 0c01 7a11 416e 746f 6e79 6d73 2e5f 5f69  ..z.Antonyms.__i
+00003050: 6e69 745f 5f29 0172 2a00 0000 6302 0000  nit__).r*...c...
+00003060: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+00003070: 0043 0000 0073 7e00 0000 7c00 6a00 6401  .C...s~...|.j.d.
+00003080: 7500 724c 7401 6402 6403 6404 8d02 0100  u.rLt.d.d.d.....
+00003090: 7401 6405 7c01 6406 1900 6407 9b04 6408  t.d.|.d...d...d.
+000030a0: 7c01 6409 1900 9b00 640a 9d05 640b 6404  |.d.....d...d.d.
+000030b0: 8d02 0100 7402 a003 640c a101 0100 640d  ....t...d.....d.
+000030c0: 7c00 5f00 6e2e 7c00 6a00 640d 7500 727a  |._.n.|.j.d.u.rz
+000030d0: 7401 6405 7c01 6406 1900 6407 9b04 6408  t.d.|.d...d...d.
+000030e0: 7c01 6409 1900 9b00 640a 9d05 640b 6404  |.d.....d...d.d.
+000030f0: 8d02 0100 640e 5300 290f 6110 0500 000a  ....d.S.).a.....
+00003100: 2020 2020 2020 2020 4861 6e64 6c65 7320          Handles 
+00003110: 7468 6520 6261 636b 6f66 6620 6d65 6368  the backoff mech
+00003120: 616e 6973 6d20 7768 656e 2074 6865 2072  anism when the r
+00003130: 6174 6520 6c69 6d69 7420 666f 7220 7175  ate limit for qu
+00003140: 6572 7969 6e67 2061 6e74 6f6e 796d 7320  erying antonyms 
+00003150: 6973 2072 6561 6368 6564 2e0a 0a20 2020  is reached...   
+00003160: 2020 2020 2054 6869 7320 6d65 7468 6f64       This method
+00003170: 2069 7320 7472 6967 6765 7265 6420 7768   is triggered wh
+00003180: 656e 2074 6865 2072 6174 6520 6c69 6d69  en the rate limi
+00003190: 7420 6973 2065 6e63 6f75 6e74 6572 6564  t is encountered
+000031a0: 2e20 4974 206c 6f67 7320 7468 6520 7261  . It logs the ra
+000031b0: 7465 206c 696d 6974 2065 7665 6e74 2061  te limit event a
+000031c0: 6e64 2064 6973 706c 6179 730a 2020 2020  nd displays.    
+000031d0: 2020 2020 636f 6c6f 7269 7a65 6420 6d65      colorized me
+000031e0: 7373 6167 6573 2069 6e64 6963 6174 696e  ssages indicatin
+000031f0: 6720 7468 6174 2074 6865 2070 726f 6365  g that the proce
+00003200: 7373 2069 7320 656e 7465 7269 6e67 2061  ss is entering a
+00003210: 2074 656d 706f 7261 7279 2068 6962 6572   temporary hiber
+00003220: 6e61 7469 6f6e 206d 6f64 652e 2049 6620  nation mode. If 
+00003230: 7468 6520 7261 7465 0a20 2020 2020 2020  the rate.       
+00003240: 206c 696d 6974 2068 6173 2061 6c72 6561   limit has alrea
+00003250: 6479 2062 6565 6e20 7265 6163 6865 642c  dy been reached,
+00003260: 2069 7420 636f 6e74 696e 7565 7320 746f   it continues to
+00003270: 2064 6973 706c 6179 2063 6f6c 6f72 697a   display coloriz
+00003280: 6564 2062 6163 6b6f 6666 206d 6573 7361  ed backoff messa
+00003290: 6765 7320 666f 7220 7375 6273 6571 7565  ges for subseque
+000032a0: 6e74 0a20 2020 2020 2020 2072 6574 7269  nt.        retri
+000032b0: 6573 2e0a 0a20 2020 2020 2020 203a 7061  es...        :pa
+000032c0: 7261 6d20 6465 7461 696c 733a 2041 2064  ram details: A d
+000032d0: 6963 7469 6f6e 6172 7920 636f 6e74 6169  ictionary contai
+000032e0: 6e69 6e67 2069 6e66 6f72 6d61 7469 6f6e  ning information
+000032f0: 2061 626f 7574 2074 6865 2062 6163 6b6f   about the backo
+00003300: 6666 2065 7665 6e74 2c20 696e 636c 7564  ff event, includ
+00003310: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
+00003320: 2020 2020 2020 2020 2020 2020 202d 2027               - '
+00003330: 7761 6974 2720 2866 6c6f 6174 293a 2054  wait' (float): T
+00003340: 6865 206e 756d 6265 7220 6f66 2073 6563  he number of sec
+00003350: 6f6e 6473 2074 6f20 7761 6974 2062 6566  onds to wait bef
+00003360: 6f72 6520 7265 7472 7969 6e67 2e0a 2020  ore retrying..  
+00003370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003380: 2020 2020 2020 2d20 2774 7269 6573 2720        - 'tries' 
+00003390: 2869 6e74 293a 2054 6865 206e 756d 6265  (int): The numbe
+000033a0: 7220 6f66 2072 6574 7279 2061 7474 656d  r of retry attem
+000033b0: 7074 7320 6d61 6465 2073 6f20 6661 722e  pts made so far.
+000033c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000033d0: 2020 2020 2020 2020 202d 2041 6464 6974           - Addit
+000033e0: 696f 6e61 6c20 6465 7461 696c 7320 7375  ional details su
+000033f0: 6368 2061 7320 2774 6172 6765 7427 2c20  ch as 'target', 
+00003400: 2761 7267 7327 2c20 276b 7761 7267 7327  'args', 'kwargs'
+00003410: 2c20 2765 6c61 7073 6564 272c 2061 6e64  , 'elapsed', and
+00003420: 2027 6578 6365 7074 696f 6e27 2077 6869   'exception' whi
+00003430: 6368 2070 726f 7669 6465 0a20 2020 2020  ch provide.     
+00003440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003450: 2020 2020 2063 6f6e 7465 7874 2061 626f       context abo
+00003460: 7574 2074 6865 2065 7665 6e74 2028 6e6f  ut the event (no
+00003470: 7420 7573 6564 2069 6e20 7468 6973 206d  t used in this m
+00003480: 6574 686f 6420 6275 7420 7061 7274 206f  ethod but part o
+00003490: 6620 7468 6520 6465 7461 696c 7320 6469  f the details di
+000034a0: 6374 696f 6e61 7279 292e 0a0a 2020 2020  ctionary)...    
+000034b0: 2020 2020 7479 7065 2064 6574 6169 6c73      type details
+000034c0: 3a20 4469 6374 0a0a 2020 2020 2020 2020  : Dict..        
+000034d0: 5369 6465 2045 6666 6563 7473 3a0a 2020  Side Effects:.  
+000034e0: 2020 2020 2020 2d20 4469 7370 6c61 7973        - Displays
+000034f0: 2063 6f6c 6f72 697a 6564 2074 6578 7420   colorized text 
+00003500: 6d65 7373 6167 6573 2074 6f20 696e 6469  messages to indi
+00003510: 6361 7465 2074 6865 2062 6163 6b6f 6666  cate the backoff
+00003520: 2073 7461 7475 732e 0a20 2020 2020 2020   status..       
+00003530: 202d 204c 6f67 7320 616e 2069 6e66 6f20   - Logs an info 
+00003540: 6d65 7373 6167 6520 7768 656e 2074 6865  message when the
+00003550: 2072 6174 6520 6c69 6d69 7420 6973 2069   rate limit is i
+00003560: 6e69 7469 616c 6c79 2072 6561 6368 6564  nitially reached
+00003570: 2e0a 2020 2020 2020 2020 2d20 5365 7473  ..        - Sets
+00003580: 2074 6865 2060 5f72 6174 655f 6c69 6d69   the `_rate_limi
+00003590: 745f 7374 6174 7573 6020 6174 7472 6962  t_status` attrib
+000035a0: 7574 6520 746f 2054 7275 6520 7768 656e  ute to True when
+000035b0: 2074 6865 2072 6174 6520 6c69 6d69 7420   the rate limit 
+000035c0: 6973 2066 6972 7374 2065 6e63 6f75 6e74  is first encount
+000035d0: 6572 6564 2e0a 0a20 2020 2020 2020 203a  ered...        :
+000035e0: 7265 7475 726e 733a 204e 6f6e 650a 2020  returns: None.  
+000035f0: 2020 2020 2020 3a72 7479 7065 3a20 4e6f        :rtype: No
+00003600: 6e65 5479 7065 0a20 2020 2020 2020 2046  neType.        F
+00003610: 7a69 5468 6520 616e 746f 6e79 6d73 2071  ziThe antonyms q
+00003620: 7565 7279 2072 6174 6520 6c69 6d69 7420  uery rate limit 
+00003630: 7761 7320 7265 6163 6865 642e 2054 6865  was reached. The
+00003640: 2071 7565 7279 696e 6720 7072 6f63 6573   querying proces
+00003650: 7320 6973 2065 6e74 6572 696e 6720 6120  s is entering a 
+00003660: 7465 6d70 6f72 6172 7920 6869 6265 726e  temporary hibern
+00003670: 6174 696f 6e20 6d6f 6465 2eda 0372 6564  ation mode...red
+00003680: a902 722f 0000 005a 0563 6f6c 6f72 7a0c  ..r/...Z.colorz.
+00003690: 4261 636b 696e 6720 6f66 6620 da04 7761  Backing off ..wa
+000036a0: 6974 7a03 2e31 667a 1020 7365 636f 6e64  itz..1fz. second
+000036b0: 7320 6166 7465 7273 205a 0574 7269 6573  s afters Z.tries
+000036c0: 7a07 2074 7269 6573 2eda 0462 6c75 657a  z. tries...bluez
+000036d0: 2a54 6865 2061 6e74 6f6e 796d 7320 7175  *The antonyms qu
+000036e0: 6572 7920 7261 7465 206c 696d 6974 2077  ery rate limit w
+000036f0: 6173 2072 6561 6368 6564 2e54 4e29 0472  as reached.TN).r
+00003700: 8700 0000 7215 0000 0072 1e00 0000 da04  ....r....r......
+00003710: 696e 666f 2902 728a 0000 005a 0764 6574  info).r....Z.det
+00003720: 6169 6c73 7225 0000 0072 2500 0000 7226  ailsr%...r%...r&
+00003730: 0000 0072 8800 0000 5601 0000 731a 0000  ...r....V...s...
+00003740: 0000 190a 0104 0102 ff06 021c 0102 ff06  ................
+00003750: 020a 0108 010a 011c 0102 ff7a 1941 6e74  ...........z.Ant
+00003760: 6f6e 796d 732e 5f62 6163 6b6f 6666 5f68  onyms._backoff_h
+00003770: 616e 646c 6572 6301 0000 0000 0000 0000  andlerc.........
+00003780: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
+00003790: 3c00 0000 7400 a001 7c00 6a02 a101 7d01  <...t...|.j...}.
+000037a0: 7c01 7338 7403 a004 6401 7c00 6a02 9b00  |.s8t...d.|.j...
+000037b0: 6402 9d03 a101 0100 7403 a004 6403 7c00  d.......t...d.|.
+000037c0: 6a02 9b00 6404 9d03 a101 0100 7c01 5300  j...d.......|.S.
+000037d0: 2905 7ab1 0a20 2020 2020 2020 2054 6869  ).z..        Thi
+000037e0: 7320 6675 6e63 7469 6f6e 2069 7320 6465  s function is de
+000037f0: 7369 676e 6564 2074 6f20 7661 6c69 6461  signed to valida
+00003800: 7465 2074 6861 7420 7468 6520 7379 6e74  te that the synt
+00003810: 6178 2066 6f72 2061 2073 7472 696e 6720  ax for a string 
+00003820: 7661 7269 6162 6c65 2069 7320 696e 2061  variable is in a
+00003830: 6e20 6163 6365 7074 6162 6c65 2066 6f72  n acceptable for
+00003840: 6d61 742e 0a0a 2020 2020 2020 2020 3a72  mat...        :r
+00003850: 6574 7572 6e3a 2054 7275 6520 6f72 2046  eturn: True or F
+00003860: 616c 7365 0a20 2020 2020 2020 203a 7274  alse.        :rt
+00003870: 7970 653a 2062 6f6f 6c65 616e 0a20 2020  ype: boolean.   
+00003880: 2020 2020 207a 0954 6865 2077 6f72 6420       z.The word 
+00003890: 7a1b 2077 6173 206e 6f74 2069 6e20 6120  z. was not in a 
+000038a0: 7661 6c69 6420 666f 726d 6174 2e7a 1c50  valid format.z.P
+000038b0: 6c65 6173 6520 7665 7269 6679 2074 6861  lease verify tha
+000038c0: 7420 7468 6520 776f 7264 207a 1620 6973  t the word z. is
+000038d0: 2073 7065 6c6c 6564 2063 6f72 7265 6374   spelled correct
+000038e0: 6c79 2e29 0572 1800 0000 5a14 7661 6c69  ly.).r....Z.vali
+000038f0: 6461 7465 5f77 6f72 645f 7379 6e74 6178  date_word_syntax
+00003900: 7282 0000 0072 1e00 0000 721f 0000 0029  r....r....r....)
+00003910: 0272 8a00 0000 da0a 7661 6c69 645f 776f  .r......valid_wo
+00003920: 7264 7225 0000 0072 2500 0000 7226 0000  rdr%...r%...r&..
+00003930: 00da 0e5f 7661 6c69 6461 7465 5f77 6f72  ..._validate_wor
+00003940: 647a 0100 0073 0a00 0000 0007 0c01 0401  dz...s..........
+00003950: 1401 1401 7a17 416e 746f 6e79 6d73 2e5f  ....z.Antonyms._
+00003960: 7661 6c69 6461 7465 5f77 6f72 6463 0100  validate_wordc..
+00003970: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00003980: 0000 4300 0000 7310 0000 0074 00a0 017c  ..C...s....t...|
+00003990: 006a 02a1 017d 017c 0153 0072 4f00 0000  .j...}.|.S.rO...
+000039a0: 2903 7216 0000 005a 0e63 6163 6865 5f61  ).r....Z.cache_a
+000039b0: 6e74 6f6e 796d 7372 8200 0000 2902 728a  ntonymsr....).r.
+000039c0: 0000 00da 0b63 6865 636b 5f63 6163 6865  .....check_cache
+000039d0: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
+000039e0: 0c5f 6368 6563 6b5f 6361 6368 6587 0100  ._check_cache...
+000039f0: 0073 0400 0000 0001 0c01 7a15 416e 746f  .s........z.Anto
+00003a00: 6e79 6d73 2e5f 6368 6563 6b5f 6361 6368  nyms._check_cach
+00003a10: 6529 03da 0c70 6f73 5f63 6174 6567 6f72  e)...pos_categor
+00003a20: 79da 0861 6e74 6f6e 796d 7372 2a00 0000  y..antonymsr*...
+00003a30: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00003a40: 0005 0000 0043 0000 0073 1400 0000 7400  .....C...s....t.
+00003a50: a001 7c00 6a02 7c01 7c02 a103 0100 6400  ..|.j.|.|.....d.
+00003a60: 5300 724f 0000 0029 0372 1600 0000 5a1a  S.rO...).r....Z.
+00003a70: 696e 7365 7274 5f77 6f72 645f 6361 6368  insert_word_cach
+00003a80: 655f 616e 746f 6e79 6d73 7282 0000 0029  e_antonymsr....)
+00003a90: 0372 8a00 0000 7296 0000 0072 9700 0000  .r....r....r....
+00003aa0: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
+00003ab0: 0d5f 7570 6461 7465 5f63 6163 6865 8b01  ._update_cache..
+00003ac0: 0000 7302 0000 0000 017a 1641 6e74 6f6e  ..s......z.Anton
+00003ad0: 796d 732e 5f75 7064 6174 655f 6361 6368  yms._update_cach
+00003ae0: 6529 02da 0375 726c 722a 0000 0063 0200  e)...urlr*...c..
+00003af0: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+00003b00: 0000 4300 0000 73a8 0000 0064 017d 027c  ..C...s....d.}.|
+00003b10: 006a 0064 0175 0072 287c 006a 0164 0175  .j.d.u.r(|.j.d.u
+00003b20: 0072 2874 027c 0164 028d 01a0 03a1 007d  .r(t.|.d.......}
+00003b30: 026e 7c7c 006a 0064 0175 0072 507c 006a  .n||.j.d.u.rP|.j
+00003b40: 0164 0175 0172 5074 027c 017c 006a 0164  .d.u.rPt.|.|.j.d
+00003b50: 038d 02a0 03a1 007d 026e 547c 006a 0064  .......}.nT|.j.d
+00003b60: 0175 0172 7a7c 006a 0164 0175 0072 7a74  .u.rz|.j.d.u.rzt
+00003b70: 027c 0164 017c 006a 0064 048d 03a0 03a1  .|.d.|.j.d......
+00003b80: 007d 026e 2a7c 006a 0064 0175 0172 a47c  .}.n*|.j.d.u.r.|
+00003b90: 006a 0164 0175 0172 a474 027c 017c 006a  .j.d.u.r.t.|.|.j
+00003ba0: 017c 006a 0064 048d 03a0 03a1 007d 027c  .|.j.d.......}.|
+00003bb0: 0253 0029 0561 1101 0000 0a20 2020 2020  .S.).a.....     
+00003bc0: 2020 2054 6869 7320 6675 6e63 7469 6f6e     This function
+00003bd0: 2071 7565 7269 6573 2074 6865 2072 6571   queries the req
+00003be0: 7565 7374 6564 206f 6e6c 696e 6520 7265  uested online re
+00003bf0: 706f 7369 746f 7279 2061 6e64 2072 6574  pository and ret
+00003c00: 7572 6e73 2074 6865 0a20 2020 2020 2020  urns the.       
+00003c10: 2072 6573 706f 6e73 6520 666f 7220 7468   response for th
+00003c20: 6973 2073 7065 6369 6669 6320 7175 6572  is specific quer
+00003c30: 792e 0a0a 2020 2020 2020 2020 3a70 6172  y...        :par
+00003c40: 616d 2075 726c 3a20 7468 6520 5552 4c20  am url: the URL 
+00003c50: 666f 7220 7468 6520 6f6e 6c69 6e65 2072  for the online r
+00003c60: 6570 6f73 6974 6f72 7920 6265 696e 6720  epository being 
+00003c70: 7175 6572 6965 640a 2020 2020 2020 2020  queried.        
+00003c80: 3a72 6574 7572 6e3a 2072 6573 706f 6e73  :return: respons
+00003c90: 6520 636f 6e74 656e 740a 2020 2020 2020  e content.      
+00003ca0: 2020 3a72 7479 7065 3a20 7265 7175 6573    :rtype: reques
+00003cb0: 7473 2e6d 6f64 656c 732e 5265 7370 6f6e  ts.models.Respon
+00003cc0: 7365 0a20 2020 2020 2020 204e 2901 da0d  se.        N)...
+00003cd0: 7572 6c5f 746f 5f73 6372 6170 6529 0272  url_to_scrape).r
+00003ce0: 9a00 0000 727c 0000 0029 0372 9a00 0000  ....r|...).r....
+00003cf0: 727c 0000 0072 7d00 0000 2904 7281 0000  r|...r}...).r...
+00003d00: 0072 8300 0000 7214 0000 005a 1067 6574  .r....r....Z.get
+00003d10: 5f77 6562 7369 7465 5f68 746d 6c29 0372  _website_html).r
+00003d20: 8a00 0000 7299 0000 00da 0872 6573 706f  ....r......respo
+00003d30: 6e73 6572 2500 0000 7225 0000 0072 2600  nser%...r%...r&.
+00003d40: 0000 da16 5f72 6571 7565 7374 5f68 7474  ...._request_htt
+00003d50: 705f 7265 7370 6f6e 7365 8e01 0000 7314  p_response....s.
+00003d60: 0000 0000 0904 0114 0110 0114 0114 0114  ................
+00003d70: 0116 0114 0116 017a 1f41 6e74 6f6e 796d  .......z.Antonym
+00003d80: 732e 5f72 6571 7565 7374 5f68 7474 705f  s._request_http_
+00003d90: 7265 7370 6f6e 7365 6301 0000 0000 0000  responsec.......
+00003da0: 0000 0000 000a 0000 000b 0000 0003 0000  ................
+00003db0: 0073 0e01 0000 6700 8900 7c00 6a00 6401  .s....g...|.j.d.
+00003dc0: 7500 7218 6700 6402 a201 8900 6e1e 7c00  u.r.g.d.....n.|.
+00003dd0: 6a00 6401 7501 722a 7c00 6a00 8900 6e0c  j.d.u.r*|.j...n.
+00003de0: 7401 6403 6404 6405 8d02 0100 7c00 6a02  t.d.d.d.....|.j.
+00003df0: 7c00 6a03 7c00 6a04 6402 9c03 7d01 8700  |.j.|.j.d...}...
+00003e00: 6601 6406 6407 8408 7c01 a005 a100 4400  f.d.d...|.....D.
+00003e10: 8301 7d02 7406 6408 6409 8d01 8f90 7d03  ..}.t.d.d.....}.
+00003e20: 6700 7d04 6700 7d05 7a3e 7c02 4400 5d18  g.}.g.}.z>|.D.].
+00003e30: 7d06 7c03 a007 7c06 a101 7d07 7c04 a008  }.|...|...}.|...
+00003e40: 7c07 a101 0100 7178 7409 7c04 8301 4400  |.....qxt.|...D.
+00003e50: 5d12 7d08 7c05 a008 7c08 a00a a100 a101  ].}.|...|.......
+00003e60: 0100 719a 5700 6e34 0400 740b 740c 740d  ..q.W.n4..t.t.t.
+00003e70: 6603 79e4 0100 7d09 0100 7a16 7c00 a00e  f.y...}...z.|...
+00003e80: 7c09 a101 0100 5700 5900 6401 7d09 7e09  |.....W.Y.d.}.~.
+00003e90: 6e0a 6401 7d09 7e09 3000 3000 7c05 5700  n.d.}.~.0.0.|.W.
+00003ea0: 0200 6401 0400 0400 8303 0100 5300 3100  ..d.........S.1.
+00003eb0: 9001 7300 3000 0100 0100 0100 5900 0100  ..s.0.......Y...
+00003ec0: 6401 5300 290a 7a79 0a20 2020 2020 2020  d.S.).zy.       
+00003ed0: 2052 756e 7320 7468 6520 7175 6572 7920   Runs the query 
+00003ee0: 7461 736b 7320 696e 2070 6172 616c 6c65  tasks in paralle
+00003ef0: 6c20 7573 696e 6720 6120 5468 7265 6164  l using a Thread
+00003f00: 506f 6f6c 2e0a 0a20 2020 2020 2020 203a  Pool...        :
+00003f10: 7265 7475 726e 3a20 6c69 7374 0a20 2020  return: list.   
+00003f20: 2020 2020 203a 7274 7970 653a 206e 6573       :rtype: nes
+00003f30: 7465 6420 6c69 7374 0a20 2020 2020 2020  ted list.       
+00003f40: 204e 2903 5a06 676f 6f67 6c65 7a0d 7468   N).Z.googlez.th
+00003f50: 6573 6175 7275 732e 636f 6d5a 0977 6f72  esaurus.comZ.wor
+00003f60: 6468 6970 706f 7a74 506c 6561 7365 2076  dhippoztPlease v
+00003f70: 6572 6966 7920 7468 6174 2074 6865 2073  erify that the s
+00003f80: 6f75 7263 6573 2074 6861 7420 7765 7265  ources that were
+00003f90: 2070 726f 7669 6465 6420 6172 6520 7661   provided are va
+00003fa0: 6c69 642e 200a 5661 6c69 6420 536f 7572  lid. .Valid Sour
+00003fb0: 6365 733a 200a 2d20 676f 6f67 6c65 200a  ces: .- google .
+00003fc0: 2d20 7468 6573 6175 7275 732e 636f 6d20  - thesaurus.com 
+00003fd0: 0a2d 2077 6f72 6468 6970 706f 728d 0000  .- wordhippor...
+00003fe0: 0072 8e00 0000 6301 0000 0000 0000 0000  .r....c.........
+00003ff0: 0000 0003 0000 0004 0000 0013 0000 0073  ...............s
+00004000: 1c00 0000 6700 7c00 5d14 5c02 7d01 7d02  ....g.|.].\.}.}.
+00004010: 7c01 8800 7600 7204 7c02 9102 7104 5300  |...v.r.|...q.S.
+00004020: 7225 0000 0072 2500 0000 2903 726e 0000  r%...r%...).rn..
+00004030: 00da 016b da01 76a9 0172 7800 0000 7225  ...k..v..rx...r%
+00004040: 0000 0072 2600 0000 726f 0000 00b9 0100  ...r&...ro......
+00004050: 0072 5300 0000 7a39 416e 746f 6e79 6d73  .rS...z9Antonyms
+00004060: 2e5f 7275 6e5f 7175 6572 795f 7461 736b  ._run_query_task
+00004070: 735f 696e 5f70 6172 616c 6c65 6c2e 3c6c  s_in_parallel.<l
+00004080: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00004090: 3ee9 0500 0000 2901 5a0b 6d61 785f 776f  >.....).Z.max_wo
+000040a0: 726b 6572 7329 0f72 8600 0000 7215 0000  rkers).r....r...
+000040b0: 00da 0d5f 7175 6572 795f 676f 6f67 6c65  ..._query_google
+000040c0: da14 5f71 7565 7279 5f74 6865 7361 7572  .._query_thesaur
+000040d0: 7573 5f63 6f6d da10 5f71 7565 7279 5f77  us_com.._query_w
+000040e0: 6f72 6468 6970 706f da05 6974 656d 7372  ordhippo..itemsr
+000040f0: 0600 0000 5a06 7375 626d 6974 7266 0000  ....Z.submitrf..
+00004100: 0072 0700 0000 da06 7265 7375 6c74 7208  .r......resultr.
+00004110: 0000 0072 0500 0000 da0c 5469 6d65 6f75  ...r......Timeou
+00004120: 7445 7272 6f72 7227 0000 0029 0a72 8a00  tErrorr'...).r..
+00004130: 0000 5a0f 7072 696d 6172 795f 736f 7572  ..Z.primary_sour
+00004140: 6365 735a 0574 6173 6b73 5a08 6578 6563  cesZ.tasksZ.exec
+00004150: 7574 6f72 5a0d 7275 6e6e 696e 675f 7461  utorZ.running_ta
+00004160: 736b 735a 0e66 696e 6973 6865 645f 7461  sksZ.finished_ta
+00004170: 736b 735a 0474 6173 6b5a 0e73 7562 6d69  sksZ.taskZ.submi
+00004180: 7474 6564 5f74 6173 6b5a 0d66 696e 6973  tted_taskZ.finis
+00004190: 6865 645f 7461 736b 721f 0000 0072 2500  hed_taskr....r%.
+000041a0: 0000 729f 0000 0072 2600 0000 7289 0000  ..r....r&...r...
+000041b0: 00a2 0100 0073 3200 0000 0007 0401 0a01  .....s2.........
+000041c0: 0a01 0a01 0802 0404 02fc 0606 0401 0401  ................
+000041d0: 04fe 0604 1602 0c01 0401 0401 0201 0801  ................
+000041e0: 0a01 0c01 0c01 1401 1401 2001 7a25 416e  .......... .z%An
+000041f0: 746f 6e79 6d73 2e5f 7275 6e5f 7175 6572  tonyms._run_quer
+00004200: 795f 7461 736b 735f 696e 5f70 6172 616c  y_tasks_in_paral
+00004210: 6c65 6c29 0372 9700 0000 da0e 7061 7274  lel).r......part
+00004220: 5f6f 665f 7370 6565 6368 722a 0000 0063  _of_speechr*...c
+00004230: 0300 0000 0000 0000 0000 0000 0400 0000  ................
+00004240: 0700 0000 4300 0000 7388 0000 0064 017d  ....C...s....d.}
+00004250: 037c 006a 0064 026b 0272 2274 0164 0364  .|.j.d.k.r"t.d.d
+00004260: 0484 007c 0144 0083 0183 017d 036e 627c  ...|.D.....}.nb|
+00004270: 006a 0064 056b 0272 4c7c 006a 0264 06a0  .j.d.k.rL|.j.d..
+00004280: 037c 02a1 0174 0174 047c 0183 0183 0164  .|...t.t.|.....d
+00004290: 079c 0269 017d 036e 387c 006a 0064 086b  ...i.}.n8|.j.d.k
+000042a0: 0272 8474 056a 067c 006a 0264 06a0 037c  .r.t.j.|.j.d...|
+000042b0: 02a1 0174 0174 047c 0183 0174 0764 098d  ...t.t.|...t.d..
+000042c0: 0264 079c 0269 0164 0a64 0b64 0c8d 037d  .d...i.d.d.d...}
+000042d0: 037c 0353 0029 0d61 2903 0000 0a20 2020  .|.S.).a)....   
+000042e0: 2020 2020 2020 2020 2050 726f 6365 7373           Process
+000042f0: 2074 6865 206f 7574 7075 7420 666f 726d   the output form
+00004300: 6174 2062 6173 6564 206f 6e20 7468 6520  at based on the 
+00004310: 7370 6563 6966 6965 6420 666f 726d 6174  specified format
+00004320: 2e0a 0a20 2020 2020 2020 2020 2020 203a  ...            :
+00004330: 7061 7261 6d20 616e 746f 6e79 6d73 3a20  param antonyms: 
+00004340: 4c69 7374 206f 6620 7379 6e6f 6e79 6d73  List of synonyms
+00004350: 2074 6f20 7072 6f63 6573 732e 0a20 2020   to process..   
+00004360: 2020 2020 2020 2020 203a 7061 7261 6d20           :param 
+00004370: 7479 7065 2061 6e74 6f6e 796d 733a 206c  type antonyms: l
+00004380: 6973 740a 2020 2020 2020 2020 2020 2020  ist.            
+00004390: 3a70 6172 616d 2070 6172 745f 6f66 5f73  :param part_of_s
+000043a0: 7065 6563 683a 2050 6172 7420 6f66 2073  peech: Part of s
+000043b0: 7065 6563 6820 6173 736f 6369 6174 6564  peech associated
+000043c0: 2077 6974 6820 7468 6520 616e 746f 6e79   with the antony
+000043d0: 6d73 2e0a 2020 2020 2020 2020 2020 2020  ms..            
+000043e0: 3a70 6172 616d 2070 6172 745f 6f66 5f73  :param part_of_s
+000043f0: 7065 6563 683a 2055 6e69 6f6e 5b73 6574  peech: Union[set
+00004400: 5b73 7472 5d2c 2073 7472 5d0a 0a20 2020  [str], str]..   
+00004410: 2020 2020 2020 2020 203a 7265 7475 726e           :return
+00004420: 733a 2050 726f 6365 7373 6564 206f 7574  s: Processed out
+00004430: 7075 7420 6261 7365 6420 6f6e 2074 6865  put based on the
+00004440: 2073 7065 6369 6669 6564 206f 7574 7075   specified outpu
+00004450: 7420 666f 726d 6174 3a0a 2020 2020 2020  t format:.      
+00004460: 2020 2020 2020 2020 2020 2d20 4966 206f            - If o
+00004470: 7574 7075 7420 666f 726d 6174 2069 7320  utput format is 
+00004480: 276c 6973 7427 2c20 7265 7475 726e 7320  'list', returns 
+00004490: 6120 736f 7274 6564 206c 6973 7420 6f66  a sorted list of
+000044a0: 206c 6f77 6572 6361 7365 2061 6e74 6f6e   lowercase anton
+000044b0: 796d 732e 0a20 2020 2020 2020 2020 2020  yms..           
+000044c0: 2020 2020 202d 2049 6620 6f75 7470 7574       - If output
+000044d0: 2066 6f72 6d61 7420 6973 2027 6469 6374   format is 'dict
+000044e0: 696f 6e61 7279 272c 2072 6574 7572 6e73  ionary', returns
+000044f0: 2061 2064 6963 7469 6f6e 6172 7920 7769   a dictionary wi
+00004500: 7468 2074 6865 2077 6f72 642c 0a20 2020  th the word,.   
+00004510: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00004520: 6172 7420 6f66 2073 7065 6563 682c 2061  art of speech, a
+00004530: 6e64 2073 6f72 7465 6420 616e 746f 6e79  nd sorted antony
+00004540: 6d73 2e0a 2020 2020 2020 2020 2020 2020  ms..            
+00004550: 2020 2020 2d20 4966 206f 7574 7075 7420      - If output 
+00004560: 666f 726d 6174 2069 7320 276a 736f 6e27  format is 'json'
+00004570: 2c20 7265 7475 726e 7320 6120 4a53 4f4e  , returns a JSON
+00004580: 206f 626a 6563 7420 7769 7468 2074 6865   object with the
+00004590: 2077 6f72 642c 0a20 2020 2020 2020 2020   word,.         
+000045a0: 2020 2020 2020 2020 2070 6172 7420 6f66           part of
+000045b0: 2073 7065 6563 682c 2061 6e64 2073 6f72   speech, and sor
+000045c0: 7465 6420 616e 746f 6e79 6d73 2e0a 2020  ted antonyms..  
+000045d0: 2020 2020 2020 2020 2020 3a72 7479 7065            :rtype
+000045e0: 3a20 556e 696f 6e5b 6c69 7374 2c20 6469  : Union[list, di
+000045f0: 6374 2c20 7374 725d 0a20 2020 2020 2020  ct, str].       
+00004600: 2020 2020 204e 7273 0000 0063 0100 0000       Nrs...c....
+00004610: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00004620: 5300 0000 7314 0000 0068 007c 005d 0c7d  S...s....h.|.].}
+00004630: 017c 01a0 00a1 0092 0271 0453 0072 2500  .|.......q.S.r%.
+00004640: 0000 726c 0000 0029 0272 6e00 0000 725f  ..rl...).rn...r_
+00004650: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
+00004660: 0000 da09 3c73 6574 636f 6d70 3edb 0100  ....<setcomp>...
+00004670: 0072 5300 0000 7a29 416e 746f 6e79 6d73  .rS...z)Antonyms
+00004680: 2e5f 7175 6572 795f 6f75 7470 7574 2e3c  ._query_output.<
+00004690: 6c6f 6361 6c73 3e2e 3c73 6574 636f 6d70  locals>.<setcomp
+000046a0: 3e72 7f00 0000 721c 0000 0029 0272 a700  >r....r....).r..
+000046b0: 0000 7297 0000 0072 7e00 0000 2901 da03  ..r....r~...)...
+000046c0: 6b65 79e9 0400 0000 4629 02da 0669 6e64  key.....F)...ind
+000046d0: 656e 745a 0c65 6e73 7572 655f 6173 6369  entZ.ensure_asci
+000046e0: 6929 0872 8400 0000 7270 0000 0072 8200  i).r....rp...r..
+000046f0: 0000 7220 0000 00da 0373 6574 727e 0000  ..r .....setr~..
+00004700: 00da 0564 756d 7073 7254 0000 0029 0472  ...dumpsrT...).r
+00004710: 8a00 0000 7297 0000 0072 a700 0000 5a10  ....r....r....Z.
+00004720: 7072 6f63 6573 7365 645f 6f75 7470 7574  processed_output
+00004730: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
+00004740: 0d5f 7175 6572 795f 6f75 7470 7574 c801  ._query_output..
+00004750: 0000 7320 0000 0000 1104 010a 0114 010a  ..s ............
+00004760: 010c 010a ff0a 020a 0108 0108 010e ff04  ................
+00004770: ff02 0204 fe06 037a 1641 6e74 6f6e 796d  .......z.Antonym
+00004780: 732e 5f71 7565 7279 5f6f 7574 7075 7463  s._query_outputc
+00004790: 0100 0000 0000 0000 0000 0000 0700 0000  ................
+000047a0: 0500 0000 4300 0000 7326 0100 007c 006a  ....C...s&...|.j
+000047b0: 007c 006a 0176 0172 2e74 0264 017c 006a  .|.j.v.r.t.d.|.j
+000047c0: 009b 0064 029d 0364 0364 048d 0201 0074  ...d...d.d.....t
+000047d0: 03a0 0464 05a1 0101 006e f47c 00a0 05a1  ...d.....n.|....
+000047e0: 007d 017c 0164 0675 0072 5674 0264 077c  .}.|.d.u.rVt.d.|
+000047f0: 006a 069b 0064 089d 0364 0964 048d 0201  .j...d...d.d....
+00004800: 006e cc7c 0164 0a75 0090 0172 227c 00a0  .n.|.d.u...r"|..
+00004810: 07a1 007d 027c 0264 0b19 0064 0a75 0072  ...}.|.d...d.u.r
+00004820: aa74 087c 0264 0519 00a0 09a1 0083 0164  .t.|.d.........d
+00004830: 0b19 007d 0374 0aa0 0b74 087c 0264 0519  ...}.t...t.|.d..
+00004840: 00a0 0ca1 0083 01a1 017d 047c 00a0 0d7c  .........}.|...|
+00004850: 047c 03a1 0253 007c 0264 0b19 0064 0675  .|...S.|.d...d.u
+00004860: 0090 0172 227c 00a0 0ea1 007d 0564 0c64  ...r"|.....}.d.d
+00004870: 0d84 007c 0544 0083 017d 0364 0e64 0f84  ...|.D...}.d.d..
+00004880: 007c 0544 0083 017d 0474 0aa0 0b74 0f7c  .|.D...}.t...t.|
+00004890: 0483 01a1 017d 0674 0aa0 1074 0f7c 0683  .....}.t...t.|..
+000048a0: 01a1 017d 067c 0690 0173 1674 0264 107c  ...}.|...s.t.d.|
+000048b0: 006a 069b 0064 119d 0364 1264 048d 0201  .j...d...d.d....
+000048c0: 006e 0c7c 00a0 0d7c 067c 03a1 0253 0064  .n.|...|.|...S.d
+000048d0: 1353 0029 1461 5301 0000 0a20 2020 2020  .S.).aS....     
+000048e0: 2020 2054 6869 7320 6675 6e63 7469 6f6e     This function
+000048f0: 2071 7565 7269 6573 206d 756c 7469 706c   queries multipl
+00004900: 6520 6f6e 6c69 6e65 2072 6570 6f73 6974  e online reposit
+00004910: 6f72 6965 7320 746f 2064 6973 636f 7665  ories to discove
+00004920: 7220 616e 746f 6e79 6d73 0a20 2020 2020  r antonyms.     
+00004930: 2020 2061 7373 6f63 6961 7465 6420 7769     associated wi
+00004940: 7468 2074 6865 2073 7065 6369 6669 6320  th the specific 
+00004950: 776f 7264 2070 726f 7669 6465 6420 746f  word provided to
+00004960: 2074 6865 2043 6c61 7373 2041 6e74 6f6e   the Class Anton
+00004970: 796d 732e 0a20 2020 2020 2020 2054 6865  yms..        The
+00004980: 2061 6e74 6f6e 796d 7320 6172 6520 6465   antonyms are de
+00004990: 6475 706c 6963 6174 6564 2061 6e64 2073  duplicated and s
+000049a0: 6f72 7465 6420 616c 7068 6162 6574 6963  orted alphabetic
+000049b0: 616c 6c79 2e0a 0a20 2020 2020 2020 203a  ally...        :
+000049c0: 7265 7475 726e 733a 2061 6e74 6f6e 796d  returns: antonym
+000049d0: 7320 7769 7468 2070 6172 7473 206f 6620  s with parts of 
+000049e0: 7370 6565 6368 0a20 2020 2020 2020 203a  speech.        :
+000049f0: 7274 7970 653a 2055 6e69 6f6e 5b4c 6973  rtype: Union[Lis
+00004a00: 745b 5369 7a65 645d 2c20 4469 6374 5b73  t[Sized], Dict[s
+00004a10: 7472 2c20 4c69 7374 5b73 7472 5d5d 2c20  tr, List[str]], 
+00004a20: 7374 725d 0a20 2020 2020 2020 207a 1d54  str].        z.T
+00004a30: 6865 2070 726f 7669 6465 6420 6f75 7470  he provided outp
+00004a40: 7574 2074 7970 6520 2d2d 3e20 7a42 203c  ut type --> zB <
+00004a50: 2d2d 2069 7320 6e6f 7420 6f6e 6520 6f66  -- is not one of
+00004a60: 2074 6865 2061 6363 6570 7461 626c 6520   the acceptable 
+00004a70: 7479 7065 733a 2064 6963 7469 6f6e 6172  types: dictionar
+00004a80: 792c 206c 6973 7420 6f72 206a 736f 6e2e  y, list or json.
+00004a90: 728d 0000 0072 8e00 0000 7234 0000 0046  r....r....r4...F
+00004aa0: 7a20 506c 6561 7365 2076 6572 6966 7920  z Please verify 
+00004ab0: 7468 6174 2074 6865 2077 6f72 6420 2d2d  that the word --
+00004ac0: 3e20 7a1a 203c 2d2d 2069 7320 7370 656c  > z. <-- is spel
+00004ad0: 6c65 6420 636f 7272 6563 746c 792e 5a07  led correctly.Z.
+00004ae0: 6d61 6765 6e74 6154 7203 0000 0063 0100  magentaTr....c..
+00004af0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00004b00: 0000 5300 0000 7320 0000 0068 007c 005d  ..S...s ...h.|.]
+00004b10: 187d 017c 0172 047c 0164 0075 0172 047c  .}.|.r.|.d.u.r.|
+00004b20: 0164 0119 0092 0271 0453 0029 024e 7234  .d.....q.S.).Nr4
+00004b30: 0000 0072 2500 0000 726d 0000 0072 2500  ...r%...rm...r%.
+00004b40: 0000 7225 0000 0072 2600 0000 72a8 0000  ..r%...r&...r...
+00004b50: 00ff 0100 0072 5300 0000 7a29 416e 746f  .....rS...z)Anto
+00004b60: 6e79 6d73 2e66 696e 645f 616e 746f 6e79  nyms.find_antony
+00004b70: 6d73 2e3c 6c6f 6361 6c73 3e2e 3c73 6574  ms.<locals>.<set
+00004b80: 636f 6d70 3e63 0100 0000 0000 0000 0000  comp>c..........
+00004b90: 0000 0200 0000 0400 0000 5300 0000 7320  ..........S...s 
+00004ba0: 0000 0067 007c 005d 187d 017c 0172 047c  ...g.|.].}.|.r.|
+00004bb0: 0164 0075 0172 047c 0164 0119 0091 0271  .d.u.r.|.d.....q
+00004bc0: 0453 0029 024e 7203 0000 0072 2500 0000  .S.).Nr....r%...
+00004bd0: 726d 0000 0072 2500 0000 7225 0000 0072  rm...r%...r%...r
+00004be0: 2600 0000 726f 0000 0000 0200 0072 5300  &...ro.......rS.
+00004bf0: 0000 7a2a 416e 746f 6e79 6d73 2e66 696e  ..z*Antonyms.fin
+00004c00: 645f 616e 746f 6e79 6d73 2e3c 6c6f 6361  d_antonyms.<loca
+00004c10: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7a25  ls>.<listcomp>z%
+00004c20: 4e6f 2061 6e74 6f6e 796d 7320 7765 7265  No antonyms were
+00004c30: 2066 6f75 6e64 2066 6f72 2074 6865 2077   found for the w
+00004c40: 6f72 643a 207a 3320 0a50 6c65 6173 6520  ord: z3 .Please 
+00004c50: 7665 7269 6679 2074 6861 7420 7468 6520  verify that the 
+00004c60: 776f 7264 2069 7320 7370 656c 6c65 6420  word is spelled 
+00004c70: 636f 7272 6563 746c 792e 7290 0000 004e  correctly.r....N
+00004c80: 2911 7284 0000 0072 8500 0000 7215 0000  ).r....r....r...
+00004c90: 00da 0373 7973 da04 6578 6974 7293 0000  ...sys..exitr...
+00004ca0: 0072 8200 0000 7295 0000 0072 7300 0000  .r....r....rs...
+00004cb0: da04 6b65 7973 7217 0000 005a 1d66 6c61  ..keysr....Z.fla
+00004cc0: 7474 656e 5f6d 756c 7469 6469 6d65 6e73  tten_multidimens
+00004cd0: 696f 6e61 6c5f 6c69 7374 da06 7661 6c75  ional_list..valu
+00004ce0: 6573 72ae 0000 0072 8900 0000 7270 0000  esr....r....rp..
+00004cf0: 005a 0f6e 6f72 6d61 6c69 7a65 5f73 7061  .Z.normalize_spa
+00004d00: 6365 2907 728a 0000 0072 9200 0000 7294  ce).r....r....r.
+00004d10: 0000 0072 a700 0000 7297 0000 005a 0d71  ...r....r....Z.q
+00004d20: 7565 7279 5f72 6573 756c 7473 5a10 616e  uery_resultsZ.an
+00004d30: 746f 6e79 6d73 5f72 6573 756c 7473 7225  tonyms_resultsr%
+00004d40: 0000 0072 2500 0000 7226 0000 00da 0d66  ...r%...r&.....f
+00004d50: 696e 645f 616e 746f 6e79 6d73 e501 0000  ind_antonyms....
+00004d60: 7336 0000 0000 090c 010e 0102 ff06 020c  s6..............
+00004d70: 0208 0108 010e 0102 ff08 020a 0108 010c  ................
+00004d80: 0114 0116 010c 010e 0108 010e 010e 020e  ................
+00004d90: 020e 0106 010e 0102 ff08 037a 1641 6e74  ...........z.Ant
+00004da0: 6f6e 796d 732e 6669 6e64 5f61 6e74 6f6e  onyms.find_anton
+00004db0: 796d 7363 0100 0000 0000 0000 0000 0000  ymsc............
+00004dc0: 0100 0000 0700 0000 4300 0000 7326 0000  ........C...s&..
+00004dd0: 0074 00a0 0164 01a1 0101 0074 00a0 0164  .t...d.....t...d
+00004de0: 02a0 0274 03a0 047c 006a 05a1 01a1 01a1  ...t...|.j......
+00004df0: 0101 0064 0353 0072 1b00 0000 721d 0000  ...d.S.r....r...
+00004e00: 0072 2400 0000 7225 0000 0072 2500 0000  .r$...r%...r%...
+00004e10: 7226 0000 0072 2700 0000 0b02 0000 7304  r&...r'.......s.
+00004e20: 0000 0000 050a 017a 2141 6e74 6f6e 796d  .......z!Antonym
+00004e30: 732e 5f68 616e 646c 655f 7175 6572 795f  s._handle_query_
+00004e40: 6578 6365 7074 696f 6e73 6301 0000 0000  exceptionsc.....
+00004e50: 0000 0000 0000 0005 0000 000c 0000 0043  ...............C
+00004e60: 0000 0073 d000 0000 7a90 7c00 6a00 6401  ...s....z.|.j.d.
+00004e70: 7c00 6a01 9b00 9d02 6402 8d01 7d01 7c01  |.j.....d...}.|.
+00004e80: 6a02 6403 6b02 7238 7403 a004 6404 7c00  j.d.k.r8t...d.|.
+00004e90: 6a01 9b00 9d02 a101 0100 5700 6405 5300  j.........W.d.S.
+00004ea0: 7405 7c01 6a06 6406 6407 8d02 7d02 7407  t.|.j.d.d...}.t.
+00004eb0: 6a08 7c02 7c00 6a01 6408 8d02 7d03 7c03  j.|.|.j.d...}.|.
+00004ec0: 7276 7c00 6a09 6409 740a 7c03 8301 640a  rv|.j.d.t.|...d.
+00004ed0: 8d02 0100 7c03 6409 6602 5700 5300 7403  ....|.d.f.W.S.t.
+00004ee0: a004 6404 7c00 6a01 9b00 9d02 a101 0100  ..d.|.j.........
+00004ef0: 5700 6405 5300 5700 6e3a 0400 740b 6a0c  W.d.S.W.n:..t.j.
+00004f00: 740d 740e 740f 7410 6605 79ca 0100 7d04  t.t.t.t.f.y...}.
+00004f10: 0100 7a16 7c00 a011 7c04 a101 0100 5700  ..z.|...|.....W.
+00004f20: 5900 6405 7d04 7e04 6e0a 6405 7d04 7e04  Y.d.}.~.n.d.}.~.
+00004f30: 3000 3000 6405 5300 290b 61bd 0200 000a  0.0.d.S.).a.....
+00004f40: 2020 2020 2020 2020 5468 6973 2066 756e          This fun
+00004f50: 6374 696f 6e20 7175 6572 6965 7320 676f  ction queries go
+00004f60: 6f67 6c65 2e63 6f6d 2066 6f72 2061 6e74  ogle.com for ant
+00004f70: 6f6e 796d 7320 6173 736f 6369 6174 6564  onyms associated
+00004f80: 2077 6974 6820 7468 6520 7370 6563 6966   with the specif
+00004f90: 6963 2077 6f72 6420 7072 6f76 6964 6564  ic word provided
+00004fa0: 2074 6f20 7468 6520 436c 6173 7320 416e   to the Class An
+00004fb0: 746f 6e79 6d73 2e0a 0a20 2020 2020 2020  tonyms...       
+00004fc0: 203a 7265 7475 726e 733a 206c 6973 7420   :returns: list 
+00004fd0: 6f66 2061 6e74 6f6e 796d 7320 616e 6420  of antonyms and 
+00004fe0: 7061 7274 7320 6f66 2073 7065 6563 6820  parts of speech 
+00004ff0: 7374 720a 2020 2020 2020 2020 3a72 7479  str.        :rty
+00005000: 7065 3a20 556e 696f 6e5b 5475 706c 655b  pe: Union[Tuple[
+00005010: 4c69 7374 5b73 7472 5d2c 2073 7472 5d0a  List[str], str].
+00005020: 2020 2020 2020 2020 3a72 6169 7365 733a          :raises:
+00005030: 0a20 2020 2020 2020 2020 2020 202d 2041  .            - A
+00005040: 7474 7269 6275 7465 4572 726f 723a 2057  ttributeError: W
+00005050: 6865 6e20 616e 2061 7474 7269 6275 7465  hen an attribute
+00005060: 2072 6566 6572 656e 6365 206f 7220 6173   reference or as
+00005070: 7369 676e 6d65 6e74 2066 6169 6c73 2e0a  signment fails..
+00005080: 2020 2020 2020 2020 2020 2020 2d20 496e              - In
+00005090: 6465 7845 7272 6f72 3a20 5768 656e 2061  dexError: When a
+000050a0: 2073 6571 7565 6e63 6520 7375 6273 6372   sequence subscr
+000050b0: 6970 7420 6973 206f 7574 206f 6620 7261  ipt is out of ra
+000050c0: 6e67 652e 0a20 2020 2020 2020 2020 2020  nge..           
+000050d0: 202d 204b 6579 4572 726f 723a 2057 6865   - KeyError: Whe
+000050e0: 6e20 6120 6d61 7070 696e 6720 6b65 7920  n a mapping key 
+000050f0: 6973 206e 6f74 2066 6f75 6e64 2069 6e20  is not found in 
+00005100: 7468 6520 7365 7420 6f66 2065 7869 7374  the set of exist
+00005110: 696e 6720 6b65 7973 2e0a 2020 2020 2020  ing keys..      
+00005120: 2020 2020 2020 2d20 5479 7065 4572 726f        - TypeErro
+00005130: 723a 2057 6865 6e20 616e 206f 7065 7261  r: When an opera
+00005140: 7469 6f6e 206f 7220 6675 6e63 7469 6f6e  tion or function
+00005150: 2069 7320 6170 706c 6965 6420 746f 2061   is applied to a
+00005160: 6e20 696e 6170 7072 6f70 7269 6174 6520  n inappropriate 
+00005170: 7479 7065 2e0a 2020 2020 2020 2020 2020  type..          
+00005180: 2020 2d20 6273 342e 4665 6174 7572 654e    - bs4.FeatureN
+00005190: 6f74 466f 756e 643a 2052 6169 7365 6420  otFound: Raised 
+000051a0: 6279 2074 6865 2042 6561 7574 6966 756c  by the Beautiful
+000051b0: 536f 7570 2063 6f6e 7374 7275 6374 6f72  Soup constructor
+000051c0: 2069 6620 6e6f 2070 6172 7365 7220 7769   if no parser wi
+000051d0: 7468 2074 6865 2072 6571 7565 7374 6564  th the requested
+000051e0: 2066 6561 7475 7265 7320 6973 2066 6f75   features is fou
+000051f0: 6e64 2e0a 2020 2020 2020 2020 7a2d 6874  nd..        z-ht
+00005200: 7470 733a 2f2f 7777 772e 676f 6f67 6c65  tps://www.google
+00005210: 2e63 6f6d 2f73 6561 7263 683f 713d 616e  .com/search?q=an
+00005220: 746f 6e79 6d2b 666f 722b 2fa9 0172 9900  tonym+for+/..r..
+00005230: 0000 e994 0100 007a 2d47 6f6f 676c 6520  .......z-Google 
+00005240: 6861 6420 6e6f 2061 6e74 6f6e 796d 2072  had no antonym r
+00005250: 6566 6572 656e 6365 2066 6f72 2074 6865  eference for the
+00005260: 2077 6f72 6420 4eda 046c 786d 6ca9 025a   word N..lxml..Z
+00005270: 066d 6172 6b75 705a 0866 6561 7475 7265  .markupZ.feature
+00005280: 7329 0272 2900 0000 725f 0000 005a 046e  s).r)...r_...Z.n
+00005290: 6f75 6ea9 0272 9600 0000 7297 0000 0029  oun..r....r....)
+000052a0: 1272 9c00 0000 7282 0000 00da 0b73 7461  .r....r......sta
+000052b0: 7475 735f 636f 6465 721e 0000 0072 9100  tus_coder....r..
+000052c0: 0000 720f 0000 0072 2f00 0000 725e 0000  ..r....r/...r^..
+000052d0: 0072 6800 0000 7298 0000 0072 7000 0000  .rh...r....rp...
+000052e0: 723f 0000 0072 4000 0000 7241 0000 0072  r?...r@...rA...r
+000052f0: 4200 0000 7243 0000 0072 4400 0000 7227  B...rC...rD...r'
+00005300: 0000 0029 0572 8a00 0000 729b 0000 00da  ...).r....r.....
+00005310: 0b73 6f75 705f 6f62 6a65 6374 7267 0000  .soup_objectrg..
+00005320: 0072 1f00 0000 7225 0000 0072 2500 0000  .r....r%...r%...
+00005330: 7226 0000 0072 a100 0000 1302 0000 731c  r&...r........s.
+00005340: 0000 0000 0d02 0114 020a 0112 0106 020e  ................
+00005350: 0110 0104 0112 010a 0212 010a 011a 017a  ...............z
+00005360: 1641 6e74 6f6e 796d 732e 5f71 7565 7279  .Antonyms._query
+00005370: 5f67 6f6f 676c 6563 0100 0000 0000 0000  _googlec........
+00005380: 0000 0000 0800 0000 0c00 0000 4300 0000  ............C...
+00005390: 7314 0100 007a d27c 006a 0064 017c 006a  s....z.|.j.d.|.j
+000053a0: 019b 009d 0264 028d 017d 017c 016a 0264  .....d...}.|.j.d
+000053b0: 036b 0272 3874 03a0 0464 047c 006a 019b  .k.r8t...d.|.j..
+000053c0: 009d 02a1 0101 0057 0064 0553 0074 057c  .......W.d.S.t.|
+000053d0: 016a 0664 0664 078d 027d 0274 0764 087c  .j.d.d...}.t.d.|
+000053e0: 0264 098d 02a0 08a1 007d 037c 0364 0a75  .d.......}.|.d.u
+000053f0: 0072 c27c 026a 0964 0b64 0c64 0d69 0164  .r.|.j.d.d.d.i.d
+00005400: 0e8d 027d 047c 0472 a874 0a6a 0b7c 0264  ...}.|.r.t.j.|.d
+00005410: 0f8d 017d 0574 0c6a 0d7c 0264 0f8d 017d  ...}.t.j.|.d...}
+00005420: 067c 006a 0e7c 0674 0f7c 0583 0164 108d  .|.j.|.t.|...d..
+00005430: 0201 007c 057c 0666 0257 0053 0074 03a0  ...|.|.f.W.S.t..
+00005440: 0464 047c 006a 019b 009d 02a1 0101 0057  .d.|.j.........W
+00005450: 0064 0553 006e 0e7c 0364 1175 0072 d057  .d.S.n.|.d.u.r.W
+00005460: 0064 0553 0057 006e 3c04 0074 106a 1174  .d.S.W.n<..t.j.t
+00005470: 1274 1374 1474 1566 0590 0179 0e01 007d  .t.t.t.f...y...}
+00005480: 0701 007a 167c 00a0 167c 07a1 0101 0057  ...z.|...|.....W
+00005490: 0059 0064 057d 077e 076e 0a64 057d 077e  .Y.d.}.~.n.d.}.~
+000054a0: 0730 0030 0064 0553 0029 1261 c802 0000  .0.0.d.S.).a....
+000054b0: 0a20 2020 2020 2020 2054 6869 7320 6675  .        This fu
+000054c0: 6e63 7469 6f6e 2071 7565 7269 6573 2074  nction queries t
+000054d0: 6865 7361 7572 7573 2e63 6f6d 2066 6f72  hesaurus.com for
+000054e0: 2061 6e74 6f6e 796d 7320 6173 736f 6369   antonyms associ
+000054f0: 6174 6564 2077 6974 6820 7468 6520 7370  ated with the sp
+00005500: 6563 6966 6963 2077 6f72 6420 7072 6f76  ecific word prov
+00005510: 6964 6564 2074 6f20 7468 6520 436c 6173  ided to the Clas
+00005520: 730a 2020 2020 2020 2020 416e 746f 6e79  s.        Antony
+00005530: 6d73 2e0a 0a20 2020 2020 2020 203a 7265  ms...        :re
+00005540: 7475 726e 733a 206c 6973 7420 6f66 2061  turns: list of a
+00005550: 6e74 6f6e 796d 7320 616e 6420 7061 7274  ntonyms and part
+00005560: 7320 6f66 2073 7065 6563 6820 7374 720a  s of speech str.
+00005570: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00005580: 556e 696f 6e5b 5475 706c 655b 4c69 7374  Union[Tuple[List
+00005590: 5b73 7472 5d2c 2073 7472 5d0a 2020 2020  [str], str].    
+000055a0: 2020 2020 3a72 6169 7365 733a 0a20 2020      :raises:.   
+000055b0: 2020 2020 2020 2020 202d 2041 7474 7269           - Attri
+000055c0: 6275 7465 4572 726f 723a 2057 6865 6e20  buteError: When 
+000055d0: 616e 2061 7474 7269 6275 7465 2072 6566  an attribute ref
+000055e0: 6572 656e 6365 206f 7220 6173 7369 676e  erence or assign
+000055f0: 6d65 6e74 2066 6169 6c73 2e0a 2020 2020  ment fails..    
+00005600: 2020 2020 2020 2020 2d20 496e 6465 7845          - IndexE
+00005610: 7272 6f72 3a20 5768 656e 2061 2073 6571  rror: When a seq
+00005620: 7565 6e63 6520 7375 6273 6372 6970 7420  uence subscript 
+00005630: 6973 206f 7574 206f 6620 7261 6e67 652e  is out of range.
+00005640: 0a20 2020 2020 2020 2020 2020 202d 204b  .            - K
+00005650: 6579 4572 726f 723a 2057 6865 6e20 6120  eyError: When a 
+00005660: 6d61 7070 696e 6720 6b65 7920 6973 206e  mapping key is n
+00005670: 6f74 2066 6f75 6e64 2069 6e20 7468 6520  ot found in the 
+00005680: 7365 7420 6f66 2065 7869 7374 696e 6720  set of existing 
+00005690: 6b65 7973 2e0a 2020 2020 2020 2020 2020  keys..          
+000056a0: 2020 2d20 5479 7065 4572 726f 723a 2057    - TypeError: W
+000056b0: 6865 6e20 616e 206f 7065 7261 7469 6f6e  hen an operation
+000056c0: 206f 7220 6675 6e63 7469 6f6e 2069 7320   or function is 
+000056d0: 6170 706c 6965 6420 746f 2061 6e20 696e  applied to an in
+000056e0: 6170 7072 6f70 7269 6174 6520 7479 7065  appropriate type
+000056f0: 2e0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
+00005700: 6273 342e 4665 6174 7572 654e 6f74 466f  bs4.FeatureNotFo
+00005710: 756e 643a 2052 6169 7365 6420 6279 2074  und: Raised by t
+00005720: 6865 2042 6561 7574 6966 756c 536f 7570  he BeautifulSoup
+00005730: 2063 6f6e 7374 7275 6374 6f72 2069 6620   constructor if 
+00005740: 6e6f 2070 6172 7365 7220 7769 7468 2074  no parser with t
+00005750: 6865 2072 6571 7565 7374 6564 2066 6561  he requested fea
+00005760: 7475 7265 7320 6973 2066 6f75 6e64 2e0a  tures is found..
+00005770: 2020 2020 2020 2020 7a21 6874 7470 733a          z!https:
+00005780: 2f2f 7777 772e 7468 6573 6175 7275 732e  //www.thesaurus.
+00005790: 636f 6d2f 6272 6f77 7365 2f72 b400 0000  com/browse/r....
+000057a0: 72b5 0000 007a 3454 6865 7361 7572 7573  r....z4Thesaurus
+000057b0: 2e63 6f6d 2068 6164 206e 6f20 616e 746f  .com had no anto
+000057c0: 6e79 6d20 7265 6665 7265 6e63 6520 666f  nym reference fo
+000057d0: 7220 7468 6520 776f 7264 204e 72b6 0000  r the word Nr...
+000057e0: 0072 b700 0000 7a19 6874 7470 733a 2f2f  .r....z.https://
+000057f0: 7777 772e 7468 6573 6175 7275 732e 636f  www.thesaurus.co
+00005800: 6da9 0272 9900 0000 7229 0000 0046 5a06  m..r....r)...FZ.
+00005810: 6275 7474 6f6e 7a0f 6461 7461 2d6c 696e  buttonz.data-lin
+00005820: 6b6d 6f64 756c 657a 0e61 6e74 6f6e 796d  kmodulez.antonym
+00005830: 2d6d 6f64 756c 6572 4e00 0000 a901 7229  -modulerN.....r)
+00005840: 0000 0072 b800 0000 5429 1772 9c00 0000  ...r....T).r....
+00005850: 7282 0000 0072 b900 0000 721e 0000 0072  r....r....r....r
+00005860: 9100 0000 720f 0000 0072 2f00 0000 7219  ....r....r/...r.
+00005870: 0000 00da 1863 6c6f 7564 666c 6172 655f  .....cloudflare_
+00005880: 7072 6f74 6563 7465 645f 7572 6c72 3800  protected_urlr8.
+00005890: 0000 725e 0000 0072 6900 0000 721a 0000  ..r^...ri...r...
+000058a0: 0072 4b00 0000 7298 0000 0072 7000 0000  .rK...r....rp...
+000058b0: 723f 0000 0072 4000 0000 7241 0000 0072  r?...r@...rA...r
+000058c0: 4200 0000 7243 0000 0072 4400 0000 7227  B...rC...rD...r'
+000058d0: 0000 0029 0872 8a00 0000 729b 0000 0072  ...).r....r....r
+000058e0: ba00 0000 da15 636c 6f75 6466 6c61 7265  ......cloudflare
+000058f0: 5f70 726f 7465 6374 696f 6e5a 1261 6e74  _protectionZ.ant
+00005900: 6f6e 796d 5f62 7574 746f 6e5f 7461 6772  onym_button_tagr
+00005910: 6700 0000 7245 0000 0072 1f00 0000 7225  g...rE...r....r%
+00005920: 0000 0072 2500 0000 7226 0000 0072 a200  ...r%...r&...r..
+00005930: 0000 3202 0000 7328 0000 0000 0e02 0114  ..2...s(........
+00005940: 020a 0112 0106 020e 0110 0108 0112 0104  ................
+00005950: 010c 010c 0112 010a 0212 0108 0108 010a  ................
+00005960: 021c 017a 1d41 6e74 6f6e 796d 732e 5f71  ...z.Antonyms._q
+00005970: 7565 7279 5f74 6865 7361 7572 7573 5f63  uery_thesaurus_c
+00005980: 6f6d 6301 0000 0000 0000 0000 0000 0008  omc.............
+00005990: 0000 000c 0000 0043 0000 0073 1801 0000  .......C...s....
+000059a0: 7ad6 7c00 6a00 6401 7c00 6a01 9b00 6402  z.|.j.d.|.j...d.
+000059b0: 9d03 6403 8d01 7d01 7c01 6a02 6404 6b02  ..d...}.|.j.d.k.
+000059c0: 723a 7403 a004 6405 7c00 6a01 9b00 9d02  r:t...d.|.j.....
+000059d0: a101 0100 5700 6406 5300 7405 7c01 6a06  ....W.d.S.t.|.j.
+000059e0: 6407 6408 8d02 7d02 7407 6409 7c02 640a  d.d...}.t.d.|.d.
+000059f0: 8d02 a008 a100 7d03 7c03 640b 7500 72c6  ......}.|.d.u.r.
+00005a00: 7409 6a0a 640c 640d 8d01 7d04 7c02 6a0b  t.j.d.d...}.|.j.
+00005a10: 7c04 640e 8d01 7290 7403 a004 6405 7c00  |.d...r.t...d.|.
+00005a20: 6a01 9b00 9d02 a101 0100 5700 6406 5300  j.........W.d.S.
+00005a30: 740c 6a0d 7c02 640f 8d01 7d05 740e 6a0f  t.j.|.d...}.t.j.
+00005a40: 7c02 640f 8d01 7d06 7c00 6a10 7c05 7411  |.d...}.|.j.|.t.
+00005a50: 7c06 8301 6410 8d02 0100 7c06 7c05 6602  |...d.....|.|.f.
+00005a60: 5700 5300 6e0e 7c03 6411 7500 72d4 5700  W.S.n.|.d.u.r.W.
+00005a70: 6406 5300 5700 6e3c 0400 7412 6a13 7414  d.S.W.n<..t.j.t.
+00005a80: 7415 7416 7417 6605 9001 7912 0100 7d07  t.t.t.f...y...}.
+00005a90: 0100 7a16 7c00 a018 7c07 a101 0100 5700  ..z.|...|.....W.
+00005aa0: 5900 6406 7d07 7e07 6e0a 6406 7d07 7e07  Y.d.}.~.n.d.}.~.
+00005ab0: 3000 3000 6406 5300 2912 61d1 0200 000a  0.0.d.S.).a.....
+00005ac0: 2020 2020 2020 2020 5468 6973 2066 756e          This fun
+00005ad0: 6374 696f 6e20 7175 6572 6965 7320 776f  ction queries wo
+00005ae0: 7264 6869 7070 6f2e 636f 6d20 666f 7220  rdhippo.com for 
+00005af0: 616e 746f 6e79 6d73 2061 7373 6f63 6961  antonyms associa
+00005b00: 7465 6420 7769 7468 2074 6865 0a20 2020  ted with the.   
+00005b10: 2020 2020 2073 7065 6369 6669 6320 776f       specific wo
+00005b20: 7264 2070 726f 7669 6465 6420 746f 2074  rd provided to t
+00005b30: 6865 2043 6c61 7373 2041 6e74 6f6e 796d  he Class Antonym
+00005b40: 732e 0a0a 2020 2020 2020 2020 3a72 6574  s...        :ret
+00005b50: 7572 6e73 3a20 6c69 7374 206f 6620 616e  urns: list of an
+00005b60: 746f 6e79 6d73 2061 6e64 2070 6172 7420  tonyms and part 
+00005b70: 6f66 2073 7065 6563 6820 7374 7269 6e67  of speech string
+00005b80: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00005b90: 2055 6e69 6f6e 5b54 7570 6c65 5b4c 6973   Union[Tuple[Lis
+00005ba0: 745b 7374 725d 2c20 7374 725d 2c20 4e6f  t[str], str], No
+00005bb0: 6e65 5d0a 2020 2020 2020 2020 3a72 6169  ne].        :rai
+00005bc0: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
+00005bd0: 202d 2041 7474 7269 6275 7465 4572 726f   - AttributeErro
+00005be0: 723a 2057 6865 6e20 616e 2061 7474 7269  r: When an attri
+00005bf0: 6275 7465 2072 6566 6572 656e 6365 206f  bute reference o
+00005c00: 7220 6173 7369 676e 6d65 6e74 2066 6169  r assignment fai
+00005c10: 6c73 2e0a 2020 2020 2020 2020 2020 2020  ls..            
+00005c20: 2d20 496e 6465 7845 7272 6f72 3a20 5768  - IndexError: Wh
+00005c30: 656e 2061 2073 6571 7565 6e63 6520 7375  en a sequence su
+00005c40: 6273 6372 6970 7420 6973 206f 7574 206f  bscript is out o
+00005c50: 6620 7261 6e67 652e 0a20 2020 2020 2020  f range..       
+00005c60: 2020 2020 202d 204b 6579 4572 726f 723a       - KeyError:
+00005c70: 2057 6865 6e20 6120 6d61 7070 696e 6720   When a mapping 
+00005c80: 6b65 7920 6973 206e 6f74 2066 6f75 6e64  key is not found
+00005c90: 2069 6e20 7468 6520 7365 7420 6f66 2065   in the set of e
+00005ca0: 7869 7374 696e 6720 6b65 7973 2e0a 2020  xisting keys..  
+00005cb0: 2020 2020 2020 2020 2020 2d20 5479 7065            - Type
+00005cc0: 4572 726f 723a 2057 6865 6e20 616e 206f  Error: When an o
+00005cd0: 7065 7261 7469 6f6e 206f 7220 6675 6e63  peration or func
+00005ce0: 7469 6f6e 2069 7320 6170 706c 6965 6420  tion is applied 
+00005cf0: 746f 2061 6e20 696e 6170 7072 6f70 7269  to an inappropri
+00005d00: 6174 6520 7479 7065 2e0a 2020 2020 2020  ate type..      
+00005d10: 2020 2020 2020 2d20 6273 342e 4665 6174        - bs4.Feat
+00005d20: 7572 654e 6f74 466f 756e 643a 2052 6169  ureNotFound: Rai
+00005d30: 7365 6420 6279 2074 6865 2042 6561 7574  sed by the Beaut
+00005d40: 6966 756c 536f 7570 2063 6f6e 7374 7275  ifulSoup constru
+00005d50: 6374 6f72 2069 6620 6e6f 2070 6172 7365  ctor if no parse
+00005d60: 7220 7769 7468 2074 6865 2072 6571 7565  r with the reque
+00005d70: 7374 6564 2066 6561 7475 7265 7320 6973  sted features is
+00005d80: 2066 6f75 6e64 2e0a 2020 2020 2020 2020   found..        
+00005d90: 7a32 6874 7470 733a 2f2f 7777 772e 776f  z2https://www.wo
+00005da0: 7264 6869 7070 6f2e 636f 6d2f 7768 6174  rdhippo.com/what
+00005db0: 2d69 732f 7468 652d 6f70 706f 7369 7465  -is/the-opposite
+00005dc0: 2d6f 662f 7a05 2e68 746d 6c72 b400 0000  -of/z..htmlr....
+00005dd0: 72b5 0000 007a 3457 6f72 6468 6970 706f  r....z4Wordhippo
+00005de0: 2e63 6f6d 2068 6164 206e 6f20 616e 746f  .com had no anto
+00005df0: 6e79 6d20 7265 6665 7265 6e63 6520 666f  nym reference fo
+00005e00: 7220 7468 6520 776f 7264 204e 72b6 0000  r the word Nr...
+00005e10: 0072 b700 0000 7a19 6874 7470 733a 2f2f  .r....z.https://
+00005e20: 7777 772e 776f 7264 6869 7070 6f2e 636f  www.wordhippo.co
+00005e30: 6d72 bb00 0000 467a 2c57 6520 646f 206e  mr....Fz,We do n
+00005e40: 6f74 2063 7572 7265 6e74 6c79 206b 6e6f  ot currently kno
+00005e50: 7720 6f66 2061 6e79 2061 6e74 6f6e 796d  w of any antonym
+00005e60: 7320 666f 7229 0172 3200 0000 2901 722f  s for).r2...).r/
+00005e70: 0000 0072 bc00 0000 72b8 0000 0054 2919  ...r....r....T).
+00005e80: 729c 0000 0072 8200 0000 72b9 0000 0072  r....r....r....r
+00005e90: 1e00 0000 7291 0000 0072 0f00 0000 722f  ....r....r....r/
+00005ea0: 0000 0072 1900 0000 72bd 0000 0072 3900  ...r....r....r9.
+00005eb0: 0000 723a 0000 0072 3800 0000 721a 0000  ..r:...r8...r...
+00005ec0: 0072 5700 0000 725e 0000 0072 7200 0000  .rW...r^...rr...
+00005ed0: 7298 0000 0072 7000 0000 723f 0000 0072  r....rp...r?...r
+00005ee0: 4000 0000 7241 0000 0072 4200 0000 7243  @...rA...rB...rC
+00005ef0: 0000 0072 4400 0000 7227 0000 0029 0872  ...rD...r'...).r
+00005f00: 8a00 0000 729b 0000 0072 ba00 0000 72be  ....r....r....r.
+00005f10: 0000 0072 3200 0000 7245 0000 0072 6700  ...r2...rE...rg.
+00005f20: 0000 721f 0000 0072 2500 0000 7225 0000  ..r....r%...r%..
+00005f30: 0072 2600 0000 72a3 0000 0059 0200 0073  .r&...r....Y...s
+00005f40: 2800 0000 000e 0201 1602 0a01 1201 0602  (...............
+00005f50: 0e01 1001 0801 0c01 0c01 1201 0602 0c01  ................
+00005f60: 0c01 1201 0c01 0801 0a01 1c01 7a19 416e  ............z.An
+00005f70: 746f 6e79 6d73 2e5f 7175 6572 795f 776f  tonyms._query_wo
+00005f80: 7264 6869 7070 6f29 0772 1c00 0000 4e72  rdhippo).r....Nr
+00005f90: 7300 0000 7275 0000 0072 7600 0000 4e4e  s...ru...rv...NN
+00005fa0: 2923 7258 0000 0072 5900 0000 725a 0000  )#rX...rY...rZ..
+00005fb0: 0072 5b00 0000 725d 0000 0072 0b00 0000  .r[...r]...r....
+00005fc0: 720a 0000 00da 0369 6e74 7209 0000 0072  r......intr....r
+00005fd0: 8c00 0000 7288 0000 00da 0462 6f6f 6c72  ....r......boolr
+00005fe0: 9300 0000 720d 0000 0072 0e00 0000 7295  ....r....r....r.
+00005ff0: 0000 0072 0c00 0000 7298 0000 00da 0872  ...r....r......r
+00006000: 6571 7565 7374 735a 066d 6f64 656c 735a  equestsZ.modelsZ
+00006010: 0852 6573 706f 6e73 6572 9c00 0000 da05  .Responser......
+00006020: 7475 706c 6572 8900 0000 7273 0000 0072  tupler....rs...r
+00006030: ac00 0000 da04 6469 6374 72ae 0000 0072  ......dictr....r
+00006040: 0400 0000 72b3 0000 0072 5c00 0000 7227  ....r....r\...r'
+00006050: 0000 0072 a100 0000 72a2 0000 0072 a300  ...r....r....r..
+00006060: 0000 7225 0000 0072 2500 0000 7225 0000  ..r%...r%...r%..
+00006070: 0072 2600 0000 7274 0000 00f5 0000 0073  .r&...rt.......s
+00006080: 3c00 0000 0801 0445 0001 0001 0001 0001  <......E........
+00006090: 0001 0001 00f9 0201 0201 0a01 0201 0201  ................
+000060a0: 0201 0601 0ef9 0c1c 0e24 0e0d 2a04 2203  .........$..*.".
+000060b0: 1414 1e26 281d 2826 0201 0a07 221f 2227  ...&(.(&...."."'
+000060c0: 7274 0000 0029 3472 5b00 0000 da0a 5f5f  rt...)4r[.....__
+000060d0: 6175 7468 6f72 5f5f da08 5f5f 6461 7465  author__..__date
+000060e0: 5f5f da0a 5f5f 7374 6174 7573 5f5f da0b  __..__status__..
+000060f0: 5f5f 6c69 6365 6e73 655f 5fda 0d5f 5f63  __license__..__c
+00006100: 6f70 7972 6967 6874 5f5f 72af 0000 0072  opyright__r....r
+00006110: 7e00 0000 da07 6c6f 6767 696e 6772 2100  ~.....loggingr!.
+00006120: 0000 da02 7265 7239 0000 00da 0f63 6f6c  ....rer9.....col
+00006130: 6c65 6374 696f 6e73 2e61 6263 7204 0000  lections.abcr...
+00006140: 005a 1963 6f6e 6375 7272 656e 742e 6675  .Z.concurrent.fu
+00006150: 7475 7265 732e 7468 7265 6164 7205 0000  tures.threadr...
+00006160: 005a 1263 6f6e 6375 7272 656e 742e 6675  .Z.concurrent.fu
+00006170: 7475 7265 7372 0600 0000 7207 0000 0072  turesr....r....r
+00006180: 0800 0000 da06 7479 7069 6e67 7209 0000  ......typingr...
+00006190: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+000061a0: 720d 0000 0072 0e00 0000 723f 0000 0072  r....r....r?...r
+000061b0: c100 0000 720f 0000 005a 0762 6163 6b6f  ....r....Z.backo
+000061c0: 6666 7210 0000 0072 1100 0000 5a09 7261  ffr....r....Z.ra
+000061d0: 7465 6c69 6d69 7472 1200 0000 7213 0000  telimitr....r...
+000061e0: 005a 2077 6f72 6468 6f61 7264 2e75 7469  .Z wordhoard.uti
+000061f0: 6c69 7469 6573 2e72 6571 7565 7374 5f68  lities.request_h
+00006200: 746d 6c72 1400 0000 5a22 776f 7264 686f  tmlr....Z"wordho
+00006210: 6172 642e 7574 696c 6974 6965 732e 636f  ard.utilities.co
+00006220: 6c6f 7269 7a65 645f 7465 7874 7215 0000  lorized_textr...
+00006230: 005a 1377 6f72 6468 6f61 7264 2e75 7469  .Z.wordhoard.uti
+00006240: 6c69 7469 6573 7216 0000 0072 1700 0000  litiesr....r....
+00006250: 7218 0000 005a 2677 6f72 6468 6f61 7264  r....Z&wordhoard
+00006260: 2e75 7469 6c69 7469 6573 2e63 6c6f 7564  .utilities.cloud
+00006270: 666c 6172 655f 6368 6563 6b65 7272 1900  flare_checkerr..
+00006280: 0000 da09 6765 744c 6f67 6765 7272 5800  ....getLoggerrX.
+00006290: 0000 721e 0000 0072 1a00 0000 725e 0000  ..r....r....r^..
+000062a0: 0072 7400 0000 7225 0000 0072 2500 0000  .rt...r%...r%...
+000062b0: 7225 0000 0072 2600 0000 da08 3c6d 6f64  r%...r&.....<mod
+000062c0: 756c 653e 0300 0000 7336 0000 0004 0404  ule>....s6......
+000062d0: 0104 0104 0104 0104 1808 0108 0108 0108  ................
+000062e0: 0108 010c 010c 0114 0120 0308 0108 010c  ......... ......
+000062f0: 0110 0110 030c 010c 0114 010c 020a 020e  ................
+00006300: 490e 70                                  I.p
```

### Comparing `wordhoard-1.5.4/wordhoard/antonyms.py` & `wordhoard-1.5.5/wordhoard/hyponyms.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,407 +1,389 @@
 #!/usr/bin/env python3
 
 """
-This Python script is designed to query multiple online repositories for the
-antonyms associated with a specific word.
+This Python script is designed to query an online repository for the
+hyponyms associated with a specific word.
 """
 __author__ = 'John Bumgarner'
-__date__ = 'October 15, 2020'
+__date__ = 'June 12, 2021'
 __status__ = 'Production'
 __license__ = 'MIT'
-__copyright__ = "Copyright (C) 2020 John Bumgarner"
+__copyright__ = "Copyright (C) 2021 John Bumgarner"
 
 ##################################################################################
-# Date Completed: October 15, 2020
+# Date Initially Completed: June 12, 2021
 # Author: John Bumgarner
 #
-# Date Last Revised: May 31, 2023
+# Date Last Revised: May 10, 2024
 # Revised by: John Bumgarner
-##################################################################################
+###################################################################################
 
 ##################################################################################
 # “AS-IS” Clause
 #
 # Except as represented in this agreement, all work produced by Developer is
 # provided “AS IS”. Other than as provided in this agreement, Developer makes no
 # other warranties, express or implied, and hereby disclaims all implied warranties,
 # including any warranty of merchantability and warranty of fitness for a particular
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
-import bs4
+# Standard library imports
 import sys
 import json
 import logging
-import requests
 import traceback
-import re as regex
+from typing import List, Dict, Optional, Set, Tuple, Union
+
+# Third-party imports
+import bs4
+import requests
 from bs4 import BeautifulSoup
 from backoff import on_exception, expo
 from ratelimit import limits, RateLimitException
+
+# Local or project-specific imports
 from wordhoard.utilities.request_html import Query
 from wordhoard.utilities.colorized_text import colorized_text
-from concurrent.futures import ThreadPoolExecutor, as_completed
-from typing import Dict, List, Optional, Set, Sized, Tuple, Union
 from wordhoard.utilities import caching, cleansing, word_verification
 from wordhoard.utilities.cloudflare_checker import CloudflareVerification
 
 logger = logging.getLogger(__name__)
 
+class SoupParser:
+    """
+        Utility class for parsing HTML content using BeautifulSoup.
 
-class Antonyms(object):
+        This class provides static methods to handle common exceptions during HTML parsing and extract specific elements
+        such as the number of pages containing hyponyms and hyponyms themselves.
 
-    def __init__(self,
-                 search_string: str = '',
-                 output_format: str = 'list',
-                 max_number_of_requests: int = 30,
-                 rate_limit_timeout_period: int = 60,
-                 user_agent: Optional[str] = None,
-                 proxies: Optional[Dict[str, str]] = None):
-        """
-        Purpose
+        Methods
         ----------
+        - _handle_query_exceptions(error):
+            Helper method to handle common exceptions in query methods.
 
-        This Python class is used to query multiple online repositories for the antonyms
-        associated with a specific word.
+        - get_number_of_pages(soup: BeautifulSoup) -> int:
+            Determines the number of pages containing hyponyms for a specific word.
 
-        Usage Examples
-        ----------
-
-        >>> antonym = Antonyms('mother')
-        >>> results = antonym.find_antonyms()
+        - get_hyponyms(soup: BeautifulSoup) -> Set[str]:
+            Parses hyponyms from the HTML response of classicthesaurus_com.
+    """
+    @staticmethod
+    def _handle_query_exceptions(error):
+        """
+        Helper method to handle common exceptions in query methods.
+        """
+        logger.error('An error occurred in the following code segment:')
+        logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
-        >>> antonym = Antonyms(search_string='mother')
-        >>> results = antonym.find_antonyms()
+    @staticmethod
+    def get_number_of_pages(soup: BeautifulSoup) -> int:
+        """
+        This function determines the number of pages that contain hyponyms for a specific word.
 
-        Parameters
-        ----------
-        :param search_string: String containing the variable to obtain antonyms for
+        :param soup: BeautifulSoup object containing the HTML response
+        :param type soup: bs4.BeautifulSoup
+        :return: number of pages
+        :rtype: int
 
-        :param output_format: Format to use for returned results.
-               Default value: list; Acceptable values: dictionary or list
+        :raises:
+            - AttributeError: When an attribute reference or assignment fails.
+            - IndexError: When a sequence subscript is out of range.
+            - KeyError: When a mapping key is not found in the set of existing keys.
+            - TypeError: When an operation or function is applied to an inappropriate type.
+            - bs4.FeatureNotFound: Raised by the BeautifulSoup constructor if no parser with the requested features is found.
+        """
+        number_of_pages = 0
+        try:
+            pages = soup.find(name='div', attrs={'id': 'pages'})
+            if pages is not None:
+                list_of_pages = [num for page in pages for num in page if num.isdigit()]
+                if len(list_of_pages) != 0:
+                    number_of_pages = int(list_of_pages[-1]) + 1
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            SoupParser._handle_query_exceptions(error)
+        return number_of_pages
+
+    @staticmethod
+    def get_hyponyms(soup: BeautifulSoup) -> Set[str]:
+        """
+        Parses hyponyms from the HTML response of classicthesaurus_com.
+
+        :param soup: BeautifulSoup object containing the HTML response
+        :param type soup: bs4.BeautifulSoup
+        :return: set of hyponyms
+        :rtype: Set[str]
 
-        :param max_number_of_requests: Maximum number of requests for a specific timeout_period
+        :raises:
+            - AttributeError: When an attribute reference or assignment fails.
+            - IndexError: When a sequence subscript is out of range.
+            - KeyError: When a mapping key is not found in the set of existing keys.
+            - TypeError: When an operation or function is applied to an inappropriate type.
+            - bs4.FeatureNotFound: Raised by the BeautifulSoup constructor if no parser with the requested features is found.
+        """
+        sub_set: set = set()
+        try:
+            table = soup.find(name='table')
+            if table:
+                rows = table.find_all(name='tr', attrs={'class': 'theentry'})
+                if rows is not None:
+                    for row in rows:
+                        cols = row.find(name='td', attrs={'class': 'abbdef'}).find(name='a')
+                        if cols and cols.text != '»':
+                            sub_set.add(str(cols.text).lower())
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            SoupParser._handle_query_exceptions(error)
+        return sub_set
+
+class Hyponyms:
+    """
+        This Python class is used to query online repositories for the hyponyms associated with a specific word.
 
-        :param rate_limit_timeout_period: The time period before a session is placed in a temporary hibernation mode
+        Usage Examples
+        ----------
+        >>> hyponyms = Hyponyms('horse')
+        >>> results = hyponyms.find_hyponyms()
 
-        :param user_agent: string containing either a global user agent type or a specific user agent
+        Parameters
+        ----------
+        search_string : str, optional
+            The word for which hyponyms are to be found.
+        output_format : str, optional
+            Format for returned results. Default is 'list'. Acceptable values are 'dictionary', 'list', or 'json'.
+        max_number_of_requests : int, optional
+            Maximum number of requests within a specified time period.
+        rate_limit_timeout_period : int, optional
+            Time period before temporary hibernation due to rate limiting.
+        user_agent : str, optional
+            User agent string for HTTP requests.
+        proxies : dict, optional
+            Dictionary of proxies for Python Requests.
 
-        :param proxies: Dictionary of proxies to use with Python Requests
-        """
+        Attributes
+        ----------
+        _proxies : Optional[Dict[str, str]]
+            Proxies to use with Python Requests.
+        _word : str
+            The word to find hyponymsfor.
+        _user_agent : Optional[str]
+            User agent for HTTP requests.
+        _output_format : str
+            Format for returned results.
+        _valid_output_formats : Set[str]
+            Set of valid output formats.
+        _rate_limit_status : bool
+            Status indicating whether rate limit is reached.
+
+        Methods
+        -------
+        find_hyponyms() -> Union[List[Sized], Dict[str, List[str]], str]:
+            Finds hyponyms for the specified word.
+        _validate_word() -> bool:
+            Validates the syntax of the word.
+        _check_cache() -> Tuple[bool, Union[Dict[str, List[str]], None]]:
+            Checks if hyponyms are cached.
+        _update_cache(hyponyms: List[str]) -> None:
+            Updates the cache with new hyponyms.
+        _request_http_response(url: str) -> requests.models.Response:
+            Makes an HTTP request and returns the response.
+        _run_query_tasks_in_parallel() -> List[tuple[List[str], str]]:
+            Runs query tasks in parallel using a ThreadPool.
+        _query_output(self, hyponyms: list) -> Union[list, dict, str]:
+            Process the output format based on the specified format.
+        _handle_query_exceptions(error):
+            Handles common exceptions in query methods.
+    """
+    def __init__(self,
+                 search_string: str = '',
+                 output_format: str = 'list',
+                 max_number_of_requests: int = 30,
+                 rate_limit_timeout_period: int = 60,
+                 user_agent: Optional[str] = None,
+                 proxies: Optional[Dict[str, str]] = None):
 
         self._proxies = proxies
         self._word = search_string
         self._user_agent = user_agent
         self._output_format = output_format
         self._valid_output_formats = {'dictionary', 'list', 'json'}
 
         rate_limit_status = False
         self._rate_limit_status = rate_limit_status
 
         # Retries the requests after a certain time period has elapsed
-        handler = on_exception(expo, RateLimitException, max_time=60, on_backoff=self._backoff_handler)
-        # Establishes a rate limit for making requests to the antonyms repositories
+        handler = on_exception(wait_gen=expo,
+                               exception=RateLimitException,
+                               max_time=60,
+                               on_backoff=self._backoff_handler)
+        # Establishes a rate limit for making requests to the hyponyms repositories
         limiter = limits(calls=max_number_of_requests, period=rate_limit_timeout_period)
-        self.find_antonyms = handler(limiter(self.find_antonyms))
+        self.find_hyponyms = handler(limiter(self.find_hyponyms))
+
+    def _backoff_handler(self, details) -> None:
+        """
+        Handles the backoff mechanism when the rate limit for querying hyponyms is reached.
+
+        This method is triggered when the rate limit is encountered. It logs the rate limit event and displays
+        colorized messages indicating that the process is entering a temporary hibernation mode. If the rate
+        limit has already been reached, it continues to display colorized backoff messages for subsequent
+        retries.
 
-    def _backoff_handler(self):
+        :param details: A dictionary containing information about the backoff event, including:
+                        - 'wait' (float): The number of seconds to wait before retrying.
+                        - 'tries' (int): The number of retry attempts made so far.
+                        - Additional details such as 'target', 'args', 'kwargs', 'elapsed', and 'exception' which provide
+                          context about the event (not used in this method but part of the details dictionary).
+
+        type details: Dict
+
+        Side Effects:
+        - Displays colorized text messages to indicate the backoff status.
+        - Logs an info message when the rate limit is initially reached.
+        - Sets the `_rate_limit_status` attribute to True when the rate limit is first encountered.
+
+        :returns: None
+        :rtype: NoneType
+        """
         if self._rate_limit_status is False:
-            colorized_text('The antonyms query rate limit was reached. The querying process is entering '
-                           'a temporary hibernation mode.', 'red')
-            logger.info('The antonyms query rate limit was reached.')
+            colorized_text(text='The hyponyms query rate limit was reached. The querying process is '
+                                'entering a temporary hibernation mode.', color='red')
+            colorized_text(text=f"Backing off {details['wait']:.1f} seconds afters {details['tries']} tries.",
+                           color='blue')
+            logger.info('The hyponyms query rate limit was reached.')
             self._rate_limit_status = True
+        elif self._rate_limit_status is True:
+            colorized_text(text=f"Backing off {details['wait']:.1f} seconds afters {details['tries']} tries.",
+                           color='blue')
 
     def _validate_word(self) -> bool:
         """
         This function is designed to validate that the syntax for a string variable is in an acceptable format.
 
         :return: True or False
         :rtype: boolean
         """
         valid_word = word_verification.validate_word_syntax(self._word)
-        if valid_word:
-            return True
-        else:
+        if not valid_word:
             logger.error(f'The word {self._word} was not in a valid format.')
             logger.error(f'Please verify that the word {self._word} is spelled correctly.')
-            return False
+        return valid_word
 
-    def _check_cache(self) -> Tuple[bool, Union[Dict[str, List[str]], None]]:
-        check_cache = caching.cache_antonyms(self._word)
+    def _check_cache(self) -> Tuple[bool, Union[List[str], None]]:
+        check_cache = caching.cache_hyponyms(self._word)
         return check_cache
 
-    def _update_cache(self, pos_category: str, antonyms: Union[List[str], Set[str]]) -> None:
-        caching.insert_word_cache_antonyms(self._word, pos_category, antonyms)
-        return
+    def _update_cache(self, hyponyms: List[str]) -> None:
+        caching.insert_word_cache_hyponyms(self._word, hyponyms)
 
     def _request_http_response(self, url: str) -> requests.models.Response:
         """
         This function queries the requested online repository and returns the
         response for this specific query.
 
         :param url: the URL for the online repository being queried
         :return: response content
         :rtype: requests.models.Response
         """
+        response = None
         if self._proxies is None and self._user_agent is None:
-            response = Query(url).get_website_html()
-            return response
+            response = Query(url_to_scrape=url).get_website_html()
         elif self._proxies is None and self._user_agent is not None:
-            response = Query(url, self._user_agent).get_website_html()
-            return response
+            response = Query(url_to_scrape=url, user_agent=self._user_agent).get_website_html()
         elif self._proxies is not None and self._user_agent is None:
-            response = Query(url, user_agent=None, proxies=self._proxies).get_website_html()
-            return response
+            response = Query(url_to_scrape=url, user_agent=None, proxies=self._proxies).get_website_html()
         elif self._proxies is not None and self._user_agent is not None:
-            response = Query(url, user_agent=self._user_agent, proxies=self._proxies).get_website_html()
-            return response
+            response = Query(url_to_scrape=url, user_agent=self._user_agent, proxies=self._proxies).get_website_html()
+        return response
 
-    def _run_query_tasks_in_parallel(self) -> List[tuple[List[str], str]]:
+    @staticmethod
+    def _handle_query_exceptions(error):
         """
-        Runs the query tasks in parallel using a ThreadPool.
-
-        :return: list
-        :rtype: nested list
-        """
-        tasks = [self._query_thesaurus_com, self._query_wordhippo]
-
-        with ThreadPoolExecutor(max_workers=5) as executor:
-            running_tasks = []
-            finished_tasks = []
-            try:
-                for task in tasks:
-                    submitted_task = executor.submit(task)
-                    running_tasks.append(submitted_task)
-                for finished_task in as_completed(running_tasks):
-                    finished_tasks.append(finished_task.result())
-                return finished_tasks
-            except Exception as error:
-                logger.error('An unknown error occurred in the following code segment:')
-                logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        Helper method to handle common exceptions in query methods.
+        """
+        logger.error('An error occurred in the following code segment:')
+        logger.error(''.join(traceback.format_tb(error.__traceback__)))
+
+    def _query_output(self, hyponyms: list) -> Union[list, dict, str]:
+        """
+            Process the output format based on the specified format.
+
+            :param hyponyms: List of synonyms to process.
+            :param type hyponyms: list
+
+            :returns: Processed output based on the specified output format:
+                - If output format is 'list', returns a sorted list of lowercase hyponyms.
+                - If output format is 'dictionary', returns a dictionary with the word and sorted hyponyms.
+                - If output format is 'json', returns a JSON object with the word and sorted hyponyms.
+            :rtype: Union[list, dict, str]
+            """
+        processed_output = None
+        if self._output_format == 'list':
+            processed_output = [word.lower() for word in hyponyms]
+        elif self._output_format == 'dictionary':
+            processed_output = {self._word: [word.lower() for word in hyponyms]}
+        elif self._output_format == 'json':
+            processed_output = json.dumps({'hyponyms': {self._word: [word.lower() for word in hyponyms]}},
+                                          indent=4, ensure_ascii=False)
+        return processed_output
 
-    def find_antonyms(self) -> Union[List[Sized], Dict[str, List[str]], str]:
+    def find_hyponyms(self) -> Union[List[str], Dict[str, List[str]], str, None]:
         """
-        Purpose
-        ----------
-        This function queries multiple online repositories to discover antonyms
-        associated with the specific word provided to the Class Antonyms.
-        The antonyms are deduplicated and sorted alphabetically.
+        This function queries classicthesaurus_com for hyponyms associated
+        with the specific word provided to the Class Hyponyms.
 
-        Returns
-        ----------
-        :returns:
-            antonyms: list of antonyms
+        :returns: list of hyponyms
+        :rtype: Union[Tuple[List[str], str]
 
-        :rtype: list
+        :raises:
+            - AttributeError: When an attribute reference or assignment fails.
+            - IndexError: When a sequence subscript is out of range.
+            - KeyError: When a mapping key is not found in the set of existing keys.
+            - TypeError: When an operation or function is applied to an inappropriate type.
+            - bs4.FeatureNotFound: Raised by the BeautifulSoup constructor if no parser with the requested features is found.
         """
         if self._output_format not in self._valid_output_formats:
-            colorized_text(f'The provided output type --> {self._output_format} <-- is not one of the '
-                           f'acceptable types: dictionary, list or json.', 'red')
+            colorized_text(text=f'The provided output type --> {self._output_format} <-- is not one of the '
+                           f'acceptable types: dictionary, list or json.', color='red')
             sys.exit(1)
         else:
             valid_word = self._validate_word()
             if valid_word is False:
-                colorized_text(f'Please verify that the word --> {self._word} <-- is spelled correctly.', 'magenta')
+                colorized_text(text=f'Please verify that the word {self._word} is spelled correctly.', color='magenta')
             elif valid_word is True:
                 check_cache = self._check_cache()
                 if check_cache[0] is True:
-                    part_of_speech = list(check_cache[1].keys())[0]
-                    antonyms = cleansing.flatten_multidimensional_list(list(check_cache[1].values()))
-                    if self._output_format == 'list':
-                        return sorted(set(antonyms))
-                    elif self._output_format == 'dictionary':
-                        output_dict = {self._word: {'part_of_speech': part_of_speech,
-                                                    'antonyms': sorted(set(antonyms), key=len)}}
-                        return output_dict
-                    elif self._output_format == 'json':
-                        json_object = json.dumps({self._word: {'part_of_speech': part_of_speech,
-                                                               'antonyms': sorted(set(antonyms), key=len)}},
-                                                 indent=4, ensure_ascii=False)
-                        return json_object
-
+                    hyponyms = cleansing.flatten_multidimensional_list(check_cache[1])
+                    return self._query_output(hyponyms)
                 elif check_cache[0] is False:
-                    query_results = self._run_query_tasks_in_parallel()
-                    part_of_speech = ''.join(set([x[1] for x in query_results if x and x is not None]))
-                    antonyms = ([x[0] for x in query_results if x and x is not None])
-                    # flatten antonyms list
-                    antonyms_results = cleansing.flatten_multidimensional_list(antonyms)
-                    # remove excess white spaces from the strings in the list
-                    antonyms_results = cleansing.normalize_space(antonyms_results)
-
-                    if len(antonyms_results) != 0:
-                        if self._output_format == 'list':
-                            return sorted(set(antonyms_results))
-                        elif self._output_format == 'dictionary':
-                            output_dict = {self._word: {'part_of_speech': part_of_speech,
-                                                        'antonyms': sorted(set(antonyms_results), key=len)}}
-                            return output_dict
-                        elif self._output_format == 'json':
-                            json_object = json.dumps({self._word: {'part_of_speech': part_of_speech,
-                                                                   'antonyms': sorted(set(antonyms_results), key=len)}},
-                                                     indent=4, ensure_ascii=False)
-
-                            return json_object
-                    else:
-                        colorized_text(f'No antonyms were found for the word: {self._word} \n'
-                                       f'Please verify that the word is spelled correctly.', 'blue')
-
-    def _query_thesaurus_com(self) -> Union[Tuple[List[str], str], None]:
-        """
-        This function queries thesaurus.com for antonyms associated
-        with the specific word provided to the Class Antonyms.
-
-        :returns:
-            antonyms: list of antonyms
-
-        :rtype: list
-
-        :raises:
-            AttributeError: Raised when an attribute reference or assignment fails
-
-            IndexError: Raised when a sequence subscript is out of range
-
-            KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys
-
-            TypeError: Raised when an operation or function is applied to an object of inappropriate type
-
-            bs4.FeatureNotFound: raised by the BeautifulSoup constructor if no parser with the requested features
-            is found
-        """
-        try:
-            response = self._request_http_response(f'https://www.thesaurus.com/browse/{self._word}')
-
-            if response.status_code == 404:
-                logger.info(f'Thesaurus.com had no antonym reference for the word {self._word}')
-                return None
-            else:
-                soup = BeautifulSoup(response.text, "lxml")
-                cloudflare_protection = CloudflareVerification('https://www.thesaurus.com',
-                                                               soup).cloudflare_protected_url()
-                if cloudflare_protection is False:
-                    antonyms_list = []
-                    part_of_speech_category = ''
-
-                    if soup.find("div", {'id': 'antonyms'}):
-                        parent_tag = soup.find_all("div", {'data-testid': 'word-grid-container'})[1]
-                        for link in parent_tag.find_all('a', {'class': 'css-pc0050'}):
-                            antonyms_list.append(link.text.strip())
-                        antonyms = sorted([x.lower() for x in antonyms_list])
-
-                        # obtain the part of speech category for the specific word
-                        if soup.select('#headword > div.css-bjn8wh.e1br8a1p0 > div > ul > li > a > em'):
-                            css_part_of_speech = soup.select(
-                                '#headword > div.css-bjn8wh.e1br8a1p0 > div > ul > li > a > em')
-                            if len(css_part_of_speech[0].text) != 0:
-                                part_of_speech_category = css_part_of_speech[0].text.rstrip('.')
-                            else:
-                                part_of_speech_category = ''
-
-                        self._update_cache(part_of_speech_category, antonyms)
-                        return antonyms_list, part_of_speech_category
-                    else:
-                        logger.info(f'Thesaurus.com had no antonym reference for the word {self._word}')
-                        return None
-                elif cloudflare_protection is True:
-                    return None
-
-        except bs4.FeatureNotFound as error:
-            logger.error('An error occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except AttributeError as error:
-            logger.error('An AttributeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except IndexError as error:
-            logger.error('An IndexError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except KeyError as error:
-            logger.error('A KeyError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except TypeError as error:
-            logger.error('A TypeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-
-    def _query_wordhippo(self) -> Union[Tuple[List[str], str], None]:
-        """
-        This function queries wordhippo.com for antonyms associated with the specific word provided
-        to the Class Antonyms.
-
-        :returns:
-            antonyms: list of antonyms
-
-        :rtype: list
-
-        :raises:
-            AttributeError: Raised when an attribute reference or assignment fails
-
-            IndexError: Raised when a sequence subscript is out of range
-
-            KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys
-
-            TypeError: Raised when an operation or function is applied to an object of inappropriate type
-
-            bs4.FeatureNotFound: raised by the BeautifulSoup constructor if no parser with the requested features
-            is found
-        """
-        try:
-            response = self._request_http_response(f'https://www.wordhippo.com/what-is/the-opposite-of/{self._word}.html')
-
-            if response.status_code == 404:
-                logger.info(f'Wordhippo.com had no antonym reference for the word {self._word}')
-                return None
-            else:
-                soup = BeautifulSoup(response.text, "lxml")
-                cloudflare_protection = CloudflareVerification('https://www.wordhippo.com',
-                                                               soup).cloudflare_protected_url()
-                if cloudflare_protection is False:
-                    pattern = regex.compile(r'We do not currently know of any antonyms for')
-                    if soup.find(text=pattern):
-                        logger.info(f'Wordhippo.com had no antonym reference for the word {self._word}')
-                        return None
-                    else:
-                        antonyms_list = []
-                        part_of_speech_category = ''
-
-                        # obtain the part of speech category for the specific word
-                        if soup.find("div", {'class': 'wordtype'}):
-                            part_of_speech_tag = soup.find("div", {'class': 'wordtype'})
-                            if len(part_of_speech_tag.text) != 0:
-                                part_of_speech_category = ''.join(filter(str.isalpha, part_of_speech_tag.text)).lower()
-                            else:
-                                part_of_speech_category = ''
-
-                        related_tag = soup.find("div", {'class': 'relatedwords'})
-                        if related_tag.find("div", {'class': 'wb'}) is not None:
-                            for list_item in related_tag.find_all("div", {'class': 'wb'}):
-                                for link in list_item.find_all('a', href=True):
-                                    antonyms_list.append(link.text)
-                            antonyms = sorted([x.lower() for x in antonyms_list])
-                            self._update_cache(part_of_speech_category, antonyms)
-                            return antonyms, part_of_speech_category
+                    try:
+                        response = self._request_http_response(url=f'https://www.classicthesaurus.com/{self._word}/narrower')
+                        if response.status_code == 404:
+                            logger.info(f'Classic Thesaurus had no hyponyms reference for the word {self._word}')
+                            return None
                         else:
-                            for table_row in related_tag.find_all('td'):
-                                for href_link in table_row.find('a', href=True):
-                                    antonyms_list.append(href_link.text)
-                            antonyms = sorted([x.lower() for x in antonyms_list])
-                            self._update_cache(part_of_speech_category, antonyms)
-                            return antonyms, part_of_speech_category
-                elif cloudflare_protection is True:
-                    return None
-
-        except bs4.FeatureNotFound as error:
-            logger.error('An error occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except AttributeError as error:
-            logger.error('An AttributeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except IndexError as error:
-            logger.error('An IndexError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except KeyError as error:
-            logger.error('A KeyError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except TypeError as error:
-            logger.error('A TypeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+                            soup_object = BeautifulSoup(markup=response.text, features="lxml")
+                            cloudflare_protection = CloudflareVerification(url='https://www.classicthesaurus.com',
+                                                                           soup=soup_object).cloudflare_protected_url()
+                            if cloudflare_protection is False:
+                                hyponym = SoupParser.get_hyponyms(soup=soup_object)
+                                if 'no hyponyms found' in hyponym:
+                                    colorized_text(text=f'No hyponyms were found for the word: {self._word} \n'
+                                                   f'Please verify that the word is spelled correctly.', color='blue')
+                                    return None
+                                else:
+                                    number_of_pages = SoupParser.get_number_of_pages(soup=soup_object)
+                                    if number_of_pages >= 2:
+                                        for page in range(2, number_of_pages):
+                                            sub_html = self._request_http_response(url=f'https://www.classicthesaurus.com/{self._word}/narrower/{page}')
+                                            sub_soup = BeautifulSoup(markup=sub_html.text, features='lxml')
+                                            additional_hyponym = SoupParser.get_hyponyms(soup=sub_soup)
+                                            hyponym.union(additional_hyponym)
+                                    self._update_cache(sorted(hyponym))
+                                    return self._query_output(list(sorted(hyponym)))
+                            elif cloudflare_protection is True:
+                                return None
+                    except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+                        self._handle_query_exceptions(error)
```

### Comparing `wordhoard-1.5.4/wordhoard/dictionary.py` & `wordhoard-1.5.5/wordhoard/dictionary.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python3
 
 """
-This Python script is designed to query multiple online repositories for the
+This Python module is designed to query multiple online repositories for the
 definition associated with a given word.
 """
 __author__ = 'John Bumgarner'
 __date__ = 'October 15, 2020'
 __status__ = 'Production'
 __license__ = 'MIT'
 __copyright__ = "Copyright (C) 2021 John Bumgarner"
 
 ##################################################################################
 # Date Completed: October 15, 2020
 # Author: John Bumgarner
 #
-# Date Last Revised: May 31, 2023
+# Date Last Revised: May 25, 2024
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # “AS-IS” Clause
 #
 # Except as represented in this agreement, all work produced by Developer is
@@ -27,550 +27,719 @@
 # including any warranty of merchantability and warranty of fitness for a particular
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
-import bs4
+# Standard library imports
 import sys
 import json
 import logging
-import requests
 import traceback
 import re as regex
+from collections.abc import Sized
+from concurrent.futures.thread import BrokenThreadPool
+from concurrent.futures import ThreadPoolExecutor, as_completed, BrokenExecutor
+from typing import Dict, List, Optional, Set, Tuple, Union
+
+# Third-party imports
+import bs4
+import requests
 from bs4 import BeautifulSoup
 from backoff import on_exception, expo
 from ratelimit import limits, RateLimitException
+
+# Local or project-specific imports
 from wordhoard.utilities.request_html import Query
 from wordhoard.utilities.cloudflare_bypass import Cloudflare
 from wordhoard.utilities.colorized_text import colorized_text
-from concurrent.futures import ThreadPoolExecutor, as_completed
-from typing import Dict, List, Optional, Set, Sized, Tuple, Union
 from wordhoard.utilities import caching, cleansing, word_verification
 from wordhoard.utilities.cloudflare_checker import CloudflareVerification
 
 logger = logging.getLogger(__name__)
 
+class PartOfSpeech:
+    """
+        This utility class contains static methods to extract part of speech categories
+        from HTML responses of various sources, which are Collins Dictionary, Merriam-Webster,
+        Synonym.com and Thesaurus.com.
 
-class Definitions(object):
+        Static Methods
+        --------------
+        _handle_query_exceptions(error):
+            Helper method to handle common exceptions in query methods.
+
+        part_of_speech_category_collins_dictionary(soup: BeautifulSoup) -> str:
+            Extracts the part of speech category from the HTML response of Collins Dictionary.
+
+        part_of_speech_category_merriam_webster(soup: BeautifulSoup) -> str:
+            Extracts the part of speech category from the HTML response of Merriam-Webster.
+
+        part_of_speech_category_synonym_com(soup: BeautifulSoup) -> str:
+            Extracts the part of speech category from the HTML response of Synonym.com.
+
+        part_of_speech_category_thesaurus_com(soup: BeautifulSoup) -> str:
+            Extracts the part of speech category from the HTML response of Thesaurus.com.
 
-    def __init__(self,
-                 search_string: str = '',
-                 output_format: str = 'list',
-                 max_number_of_requests: int = 30,
-                 rate_limit_timeout_period: int = 60,
-                 user_agent: Optional[str] = None,
-                 proxies: Optional[Dict[str, str]] = None):
         """
-        Purpose
-        ----------
+    @staticmethod
+    def _handle_query_exceptions(error):
+        """
+        Helper method to handle common exceptions in query methods.
+        """
+        logger.error('An error occurred in the following code segment:')
+        logger.error(''.join(traceback.format_tb(error.__traceback__)))
+
+    @staticmethod
+    def part_of_speech_category_collins_dictionary(soup: BeautifulSoup) -> str:
+        """
+        Extracts the part of speech category from the HTML response of Collins Dictionary.
+
+        :param soup: BeautifulSoup object containing the HTML response
+        :param type soup: bs4.BeautifulSoup
+        :return: Part of speech category
+        :rtype: str
+        """
+        part_of_speech_category: str = ''
+        try:
+            if soup.find(name='span', attrs={'class': 'headerSensePos'}):
+                tag_part_of_speech = soup.find(name='span', attrs={'class': 'headerSensePos'})
+                if tag_part_of_speech and len(tag_part_of_speech.text) != 0:
+                    part_of_speech_category = tag_part_of_speech.text.strip('()')
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            PartOfSpeech._handle_query_exceptions(error)
+        return part_of_speech_category
+
+    @staticmethod
+    def part_of_speech_category_merriam_webster(soup: BeautifulSoup) -> str:
+        """
+        Extracts the part of speech category from the HTML response of Merriam-Webster.
+
+        :param soup: BeautifulSoup object containing the HTML response
+        :param type soup: bs4.BeautifulSoup
+        :return: Part of speech category
+        :rtype: str
+        """
+        part_of_speech_category: str = ''
+        try:
+            if soup.select(selector='#dictionary-entry-1 > div.row.entry-header > div > '
+                                    'div.entry-header-content.d-flex.flex-wrap.align-items-baseline.flex-row.mb-0 > '
+                                    'h2 > a'):
+                css_part_of_speech = soup.select(selector= '#dictionary-entry-1 > div.row.entry-header > div > '
+                                                           'div.entry-header-content.d-flex.flex-wrap.align-items-baseline.flex-row.mb-0 > h2 > a')
+                if len(css_part_of_speech[0].text) != 0:
+                    part_of_speech_category = css_part_of_speech[0].text.split()[0]
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            PartOfSpeech._handle_query_exceptions(error)
+        return part_of_speech_category.strip()
+
+    @staticmethod
+    def part_of_speech_category_synonym_com(soup: BeautifulSoup) -> str:
+        """
+        Extracts the part of speech category from the HTML response of Synonym.com.
+
+        :param soup: BeautifulSoup object containing the HTML response
+        :param type soup: bs4.BeautifulSoup
+        :return: Part of speech category
+        :rtype: str
+        """
+        part_of_speech_category: str = ''
+        try:
+            if soup.select(selector= 'body > div.page-container > div.content-container > div.main-column > '
+                                     'div.sections-wrapper > div:nth-child(1) > p > strong'):
+                css_part_of_speech = soup.select(selector= 'body > div.page-container > div.content-container > '
+                                                           'div.main-column > div.sections-wrapper > div:nth-child(1) > '
+                                                           'p > strong')
+                if len(css_part_of_speech[0].text) != 0:
+                    part_of_speech_category = css_part_of_speech[0].text.rstrip('.')
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            PartOfSpeech._handle_query_exceptions(error)
+        return part_of_speech_category.strip()
+
+    @staticmethod
+    def part_of_speech_category_thesaurus_com(soup: BeautifulSoup) -> str:
+        """
+        Extracts the part of speech category from the HTML response of Thesaurus.com.
+
+        :param soup: BeautifulSoup object containing the HTML response
+        :param type soup: bs4.BeautifulSoup
+        :return: Part of speech category
+        :rtype: str
+        """
+        part_of_speech_category: str = ''
+        try:
+            synonym_section = soup.find(name='section', attrs={'data-type': 'synonym-antonym-module'})
+            synonym_div_tags = synonym_section.find_all(name='div',
+                                                        attrs={'data-type': 'synonym-and-antonym-card'})
+            if synonym_div_tags:
+                part_of_speech_category = synonym_div_tags[0].find('p').text.split(' ', 1)[0]
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            PartOfSpeech._handle_query_exceptions(error)
+        return part_of_speech_category.strip()
+
+class ParseDefinitions:
+    """
+        This utility class contains static methods to parse definitions from HTML responses of various sources,
+        which are Merriam_Webster, Synonym.com and Thesaurus.com.
+
+        Static Methods
+        --------------
+        _handle_query_exceptions(error):
+            Helper method to handle common exceptions in query methods.
+
+        parse_merriam_webster(soup: BeautifulSoup) -> list:
+            Parses definitions from the HTML response of Merriam_Webster.
+
+        parse_synonym_com(soup: BeautifulSoup) -> list:
+            Parses definitions from the HTML response of Synonym.com.
+
+        parse_thesaurus_com(soup: BeautifulSoup) -> list:
+            Parses definitions from the HTML response of Thesaurus.com.
+        """
+
+    @staticmethod
+    def _handle_query_exceptions(error):
+        """
+        Helper method to handle common exceptions in query methods.
+        """
+        logger.error('An error occurred in the following code segment:')
+        logger.error(''.join(traceback.format_tb(error.__traceback__)))
+
+    @staticmethod
+    def parse_collins_dictionary(soup: BeautifulSoup, word: str) -> list:
+        """
+        Parses definitions from the HTML response of Collins Dictionary.
+
+        :param soup: BeautifulSoup object containing the HTML response
+        :param type soup: bs4.BeautifulSoup
+        :param word: word to search
+        :param type word: string
+        :return: List of definitions extracted from the HTML response
+        :rtype: list
+        """
+        definition_list: list = []
+        try:
+            query_results = soup.find(name='div', attrs={'class': 'form type-def titleTypeSubContainer'})
+            if query_results is not None:
+                definition = query_results.findNext(name='div', attrs={'class': 'def'})
+                definition_list.append(definition.text.strip())
+            elif query_results is None:
+                logger.error(f'Collins Dictionary had no definition reference for the word {word}')
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            ParseDefinitions._handle_query_exceptions(error)
+        return definition_list
+
+    @staticmethod
+    def parse_merriam_webster(soup: BeautifulSoup) -> list:
+        """
+        Parses definitions from the HTML response of Merriam-Webster.
+
+        :param soup: BeautifulSoup object containing the HTML response
+        :param type soup: bs4.BeautifulSoup
+        :return: List of definitions extracted from the HTML response
+        :rtype: list
+        """
+        definition_list: list = []
+        try:
+            dictionary_entry = soup.find(name='div', attrs={'id': 'dictionary-entry-1'})
+            definition_container = dictionary_entry.find(name='div', attrs={'class': 'vg'})
+            definition_entries = definition_container.find(name='div', attrs={'class': 'sb-0 sb-entry'})
+            for definition_entry in definition_entries.find_all(name='span', attrs={'class': 'dtText'}):
+                definition_list.append(definition_entry.text.lower().replace(':', '').strip())
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            ParseDefinitions._handle_query_exceptions(error)
+        return definition_list
+
+    @staticmethod
+    def parse_synonym_com(soup: BeautifulSoup) -> list:
+        """
+        Parses definitions from the HTML response of synonym.com.
+
+        :param soup: BeautifulSoup object containing the HTML response
+        :param type soup: bs4.BeautifulSoup
+        :return: List of definitions extracted from the HTML response
+        :rtype: list
+        """
+        definition_list: list = []
+        try:
+            dictionary_entries = soup.find(name='h3', attrs={'class': 'section-title'})
+            dictionary_entry = dictionary_entries.find_next(name='p').text
+            remove_brackets = regex.sub(pattern=r'.*?\[.*?\]', repl='', string=dictionary_entry)
+            remove_spaces = cleansing.remove_excess_whitespace(remove_brackets)
+            definition_list.append(remove_spaces)
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            ParseDefinitions._handle_query_exceptions(error)
+        return definition_list
+
+    @staticmethod
+    def parse_thesaurus_com(soup: BeautifulSoup) -> list:
+        """
+        Parses definitions from the HTML response of Thesaurus.com.
+
+        :param soup: BeautifulSoup object containing the HTML response
+        :param type soup: bs4.BeautifulSoup
+        :return: List of definitions extracted from the HTML response
+        :rtype: list
+        """
+        definition_list: list = []
+        try:
+            synonym_section = soup.find(name='section', attrs={'data-type': 'synonym-antonym-module'})
+            synonym_div_tags = synonym_section.find_all(name='div',
+                                                    attrs={'data-type': 'synonym-and-antonym-card'})
+            if synonym_div_tags:
+                definition = synonym_div_tags[0].find(name='p').text.split(' ', 1)[1]
+                definition_list.append(definition.strip())
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            ParseDefinitions._handle_query_exceptions(error)
+        return definition_list
+
+class Definitions:
+    """
         This Python class is used to query multiple online repositories for the definition
         associated with a specific word.
 
         Usage Examples
         ----------
-
         >>> definition = Definitions('mother')
         >>> results = definition.find_definitions()
 
-        >>> definition = Definitions(search_string='mother')
-        >>> results = definition.find_definitions()
-
         Parameters
         ----------
-        :param search_string: string containing the variable to obtain definition for
-
-        :param output_format: Format to use for returned results.
-               Default value: list; Acceptable values: dictionary or list
-
-        :param max_number_of_requests: maximum number of requests for a specific timeout_period
-
-        :param rate_limit_timeout_period: the time period before a session is placed in a temporary hibernation mode
+        search_string : str, optional
+            The word for which definitions are to be found.
+        sources: Optional[List[str]]
+            The sources to search for definitions.
+        output_format : str, optional
+            Format for returned results. Default is 'list'. Acceptable values are 'dictionary', 'list', or 'json'.
+        max_number_of_requests : int, optional
+            Maximum number of requests within a specified time period.
+        rate_limit_timeout_period : int, optional
+            Time period before temporary hibernation due to rate limiting.
+        user_agent : str, optional
+            User agent string for HTTP requests.
+        proxies : dict, optional
+            Dictionary of proxies for Python Requests.
 
-        :param user_agent: string containing either a global user agent type or a specific user agent
-
-        :param proxies: dictionary of proxies to use with Python Requests
+        Attributes
+        ----------
+        _proxies : Optional[Dict[str, str]]
+            Proxies to use with Python Requests.
+        _word : str
+            The word to find definitions for.
+        _sources : Optional[List[str]]
+            The sources to search for definitions.
+        _user_agent : Optional[str]
+            User agent for HTTP requests.
+        _output_format : str
+            Format for returned results.
+        _valid_output_formats : Set[str]
+            Set of valid output formats.
+        _rate_limit_status : bool
+            Status indicating whether rate limit is reached.
+
+        Methods
+        -------
+        find_definitions() -> Union[List[Sized], Dict[str, List[str]], str]:
+            Finds definitions for the specified word.
+        _validate_word() -> bool:
+            Validates the syntax of the word.
+        _check_cache() -> Tuple[bool, Union[Dict[str, List[str]], None]]:
+            Checks if definitions are cached.
+        _update_cache(pos_category: str, synonyms: Union[List[str], Set[str]]) -> None:
+            Updates the cache with new definitions.
+        _request_http_response(url: str) -> requests.models.Response:
+            Makes an HTTP request and returns the response.
+        _run_query_tasks_in_parallel() -> List[tuple[List[str], str]]:
+            Runs query tasks in parallel using a ThreadPool.
+        _query_output(self, antonyms: list, part_of_speech: Union[set[str], str]) -> Union[list, dict, str]:
+            Process the output format based on the specified format.
+        _handle_query_exceptions(error):
+            Handles common exceptions in query methods.
+        _query_collins_dictionary() -> Union[Tuple[List[str], str], None]:
+            Queries collinsdictionary.com for definitions.
+        _query_merriam_webster() -> Union[Tuple[List[str], str], None]:
+            Queries merriam-webster.com for definitions.
+        _query_synonym_com() -> Union[Tuple[List[str], str], None]:
+            Queries synonym.com for definitions.
+        _query_thesaurus_com() -> Union[Tuple[List[str], str], None]:
+            Queries thesaurus.com for definitions.
         """
+    def __init__(self,
+                 search_string: str = '',
+                 sources: Optional[List[str]] = None,
+                 output_format: str = 'list',
+                 max_number_of_requests: int = 30,
+                 rate_limit_timeout_period: int = 60,
+                 user_agent: Optional[str] = None,
+                 proxies: Optional[Dict[str, str]] = None):
 
         self._proxies = proxies
         self._word = search_string
         self._user_agent = user_agent
         self._output_format = output_format
         self._valid_output_formats = {'dictionary', 'list', 'json'}
+        self._sources = sources
 
         rate_limit_status = False
         self._rate_limit_status = rate_limit_status
 
         # Retries the requests after a certain time period has elapsed
-        handler = on_exception(expo, RateLimitException, max_time=60, on_backoff=self._backoff_handler)
+        handler = on_exception(wait_gen=expo,
+                               exception=RateLimitException,
+                               max_time=60,
+                               on_backoff=self._backoff_handler)
         # Establishes a rate limit for making requests to the definition repositories
         limiter = limits(calls=max_number_of_requests, period=rate_limit_timeout_period)
-        self.find_definitions = handler(limiter(self.find_definitions))
+        self._run_query_tasks_in_parallel = handler(limiter(self._run_query_tasks_in_parallel))
+
+    def _backoff_handler(self, details) -> None:
+        """
+        Handles the backoff mechanism when the rate limit for querying definition is reached.
+
+        This method is triggered when the rate limit is encountered. It logs the rate limit event and displays
+        colorized messages indicating that the process is entering a temporary hibernation mode. If the rate
+        limit has already been reached, it continues to display colorized backoff messages for subsequent
+        retries.
+
+        :param details: A dictionary containing information about the backoff event, including:
+                        - 'wait' (float): The number of seconds to wait before retrying.
+                        - 'tries' (int): The number of retry attempts made so far.
+                        - Additional details such as 'target', 'args', 'kwargs', 'elapsed', and 'exception' which provide
+                          context about the event (not used in this method but part of the details dictionary).
 
-    def _backoff_handler(self):
+        type details: Dict
+
+        Side Effects:
+        - Displays colorized text messages to indicate the backoff status.
+        - Logs an info message when the rate limit is initially reached.
+        - Sets the `_rate_limit_status` attribute to True when the rate limit is first encountered.
+
+        :returns: None
+        :rtype: NoneType
+        """
         if self._rate_limit_status is False:
-            colorized_text('The definition query rate limit was reached. The querying process is entering '
-                           'a temporary hibernation mode.', 'red')
+            colorized_text(text='The definition query rate limit was reached. The querying process is '
+                                'entering a temporary hibernation mode.', color='red')
+            colorized_text(text=f"Backing off {details['wait']:.1f} seconds afters {details['tries']} tries.",
+                           color='blue')
             logger.info('The definition query rate limit was reached.')
             self._rate_limit_status = True
+        elif self._rate_limit_status is True:
+            colorized_text(text=f"Backing off {details['wait']:.1f} seconds afters {details['tries']} tries.",
+                           color='blue')
 
     def _validate_word(self) -> bool:
         """
         This function is designed to validate that the syntax for a string variable is in an acceptable format.
 
         :return: True or False
         :rtype: bool
         """
         valid_word = word_verification.validate_word_syntax(self._word)
-        if valid_word:
-            return True
-        else:
+        if not valid_word:
             logger.error(f'The word {self._word} was not in a valid format.')
             logger.error(f'Please verify that the word {self._word} is spelled correctly.')
-            return False
+        return valid_word
 
     def _check_cache(self) -> Tuple[bool, Union[Dict[str, List[str]], None]]:
         check_cache = caching.cache_definition(self._word)
         return check_cache
 
     def _update_cache(self, pos_category: str, definition: Union[List[str], Set[str]]) -> None:
         caching.insert_word_cache_definition(self._word, pos_category, definition)
-        return
 
     def _request_http_response(self, url: str) -> requests.models.Response:
         """
         This function queries the requested online repository and returns the
         response for this specific query.
 
         :param url: the URL for the online repository being queried
         :return: response content
         :rtype: requests.models.Response
         """
+        response = None
         if self._proxies is None and self._user_agent is None:
-            response = Query(url).get_website_html()
-            return response
+            response = Query(url_to_scrape=url).get_website_html()
         elif self._proxies is None and self._user_agent is not None:
-            response = Query(url, self._user_agent).get_website_html()
-            return response
+            response = Query(url_to_scrape=url, user_agent=self._user_agent).get_website_html()
         elif self._proxies is not None and self._user_agent is None:
-            response = Query(url, user_agent=None, proxies=self._proxies).get_website_html()
-            return response
+            response = Query(url_to_scrape=url, user_agent=None, proxies=self._proxies).get_website_html()
         elif self._proxies is not None and self._user_agent is not None:
-            response = Query(url, user_agent=self._user_agent, proxies=self._proxies).get_website_html()
-            return response
+            response = Query(url_to_scrape=url, user_agent=self._user_agent, proxies=self._proxies).get_website_html()
+        return response
 
     def _run_query_tasks_in_parallel(self) -> List[tuple[List[str], str]]:
         """
         Runs the query tasks in parallel using a ThreadPool.
 
         :return: list
         :rtype: nested list
         """
-        tasks = [self._query_collins_dictionary, self._query_merriam_webster,
-                 self._query_synonym_com, self._query_thesaurus_com]
+        sources: list = []
+        if self._sources is None:
+            sources = ['collins', 'merriam-webster', 'synonym.com', 'thesaurus.com']
+        elif self._sources is not None:
+            sources = self._sources
+        else:
+            colorized_text(text='Please verify that the sources that were provided are valid. \n'
+                                'Valid Sources: \n'
+                                '- collins \n'
+                                '- merriam-webster \n'
+                                '- synonym.com \n'
+                                '- thesaurus.com', color='red')
+
+        primary_sources = {'collins': self._query_collins_dictionary,
+                           'merriam-webster': self._query_merriam_webster,
+                           'synonym.com': self._query_synonym_com,
+                           'thesaurus.com': self._query_thesaurus_com,}
+
+        tasks = [v for k, v in primary_sources.items() if k in sources]
 
         with ThreadPoolExecutor(max_workers=5) as executor:
             running_tasks = []
             finished_tasks = []
             try:
                 for task in tasks:
                     submitted_task = executor.submit(task)
                     running_tasks.append(submitted_task)
                 for finished_task in as_completed(running_tasks):
                     finished_tasks.append(finished_task.result())
-                return finished_tasks
-            except Exception as error:
-                logger.error('An unknown error occurred in the following code segment:')
-                logger.error(''.join(traceback.format_tb(error.__traceback__)))
+            except (BrokenExecutor, BrokenThreadPool, TimeoutError) as error:
+                self._handle_query_exceptions(error)
+            return finished_tasks
+
+    def _query_output(self, definitions: list, part_of_speech: Union[set[str], str]) -> Union[list, dict, str]:
+        """
+            Process the output format based on the specified format.
+
+            :param definitions: List of synonyms to process.
+            :param type definitions: list
+            :param part_of_speech: Part of speech associated with the definitions.
+            :param part_of_speech: Union[set[str], str]
+
+            :returns: Processed output based on the specified output format:
+                - If output format is 'list', returns a sorted list of lowercase definitions.
+                - If output format is 'dictionary', returns a dictionary with the word,
+                  part of speech, and sorted definitions.
+                - If output format is 'json', returns a JSON object with the word,
+                  part of speech, and sorted definitions.
+            :rtype: Union[list, dict, str]
+            """
+        processed_output = None
+        if self._output_format == 'list':
+            processed_output = sorted({word.lower() for word in definitions})
+        elif self._output_format == 'dictionary':
+            processed_output = {self._word: {'part_of_speech': ''.join(part_of_speech),
+                                             'definitions': sorted(set(definitions))}}
+        elif self._output_format == 'json':
+            processed_output = json.dumps({self._word:
+                                               {'part_of_speech': ''.join(part_of_speech),
+                                                'definitions': sorted(set(definitions), key=len)}}, indent=4, ensure_ascii=False)
+        return processed_output
 
     def find_definitions(self) -> Union[List[Sized], Dict[str, List[str]], str]:
         """
-        Purpose
-        ----------
-        This function queries multiple online repositories to discover
-        definitions related with the specific word provided to the
-        Class Definitions.
+        This function queries multiple online repositories to discover definitions related
+        with the specific word provided to the Class Definitions.
 
-        Returns
-        ----------
         :return: list of definitions
-
         :rtype: list
+
         """
         if self._output_format not in self._valid_output_formats:
             colorized_text(f'The provided output type --> {self._output_format} <-- is not one of the '
                            f'acceptable types: dictionary, list or json.', 'red')
             sys.exit(1)
         else:
             valid_word = self._validate_word()
             if valid_word is False:
                 colorized_text(f'Please verify that the word {self._word} is spelled correctly.', 'magenta')
             elif valid_word is True:
                 check_cache = self._check_cache()
                 if check_cache[0] is True:
                     part_of_speech = list(check_cache[1].keys())[0]
                     definitions = cleansing.flatten_multidimensional_list(list(check_cache[1].values()))
-                    if self._output_format == 'list':
-                        return sorted(set(definitions))
-                    elif self._output_format == 'dictionary':
-                        output_dict = {self._word: {'part_of_speech': part_of_speech,
-                                                    'definitions': sorted(set(definitions), key=len)}}
-                        return output_dict
-                    elif self._output_format == 'json':
-                        json_object = json.dumps({self._word: {'part_of_speech': part_of_speech,
-                                                               'definitions': sorted(set(definitions), key=len)}},
-                                                 indent=4, ensure_ascii=False)
-                        return json_object
-
+                    return self._query_output(definitions, part_of_speech)
                 elif check_cache[0] is False:
                     query_results = self._run_query_tasks_in_parallel()
-                    part_of_speech = ''.join(set([x[1] for x in query_results if x and x is not None]))
+                    part_of_speech = {x[1] for x in query_results if x and x is not None}
                     definitions = ([x[0] for x in query_results if x and x is not None])
                     # flatten definitions list
                     definitions = cleansing.flatten_multidimensional_list(definitions)
                     # remove excess white spaces from the strings in the list
                     definitions = [regex.sub(' +', " ", x) for x in definitions]
                     if not definitions:
-                        colorized_text(f'No definitions were found for the word: {self._word} \n'
-                                       f'Please verify that the word is spelled correctly.', 'blue')
+                        colorized_text(text=f'No definitions were found for the word: {self._word} \n'
+                                       f'Please verify that the word is spelled correctly.', color='blue')
                     else:
-                        if self._output_format == 'list':
-                            return sorted(set(definitions))
-                        elif self._output_format == 'dictionary':
-                            output_dict = {self._word: {'part_of_speech': part_of_speech, 'definitions': sorted(set(
-                                definitions), key=len)}}
-                            return output_dict
-                        elif self._output_format == 'json':
-                            json_object = json.dumps({self._word: {'part_of_speech': part_of_speech,
-                                                                   'definitions': sorted(set(definitions), key=len)}},
-                                                     indent=4, ensure_ascii=False)
-                            return json_object
+                        return self._query_output(definitions, part_of_speech)
+
+    @staticmethod
+    def _handle_query_exceptions(error):
+        """
+        Helper method to handle common exceptions in query methods.
+        """
+        logger.error('An error occurred in the following code segment:')
+        logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
     def _query_collins_dictionary(self) -> Union[Tuple[List[str], str], None]:
         """
         This function queries collinsdictionary.com for a definition associated
         with the specific word provided to the Class Definitions.
 
-         :returns:
-            definition: definition for a word
-
-        :rtype: str
-
+        :returns:definition for a word
+        :rtype: Union[Tuple[List[str], str], None]
         :raises:
-            AttributeError: Raised when an attribute reference or assignment fails
-
-            IndexError: Raised when a sequence subscript is out of range
-
-            KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys
-
-            TypeError: Raised when an operation or function is applied to an object of inappropriate type
-
-            bs4.FeatureNotFound: raised by the BeautifulSoup constructor if no parser with the requested features
-            is found
+            - AttributeError: When an attribute reference or assignment fails.
+            - IndexError: When a sequence subscript is out of range.
+            - KeyError: When a mapping key is not found in the set of existing keys.
+            - TypeError: When an operation or function is applied to an inappropriate type.
+            - bs4.FeatureNotFound: Raised by the BeautifulSoup constructor if no parser with the requested features is found.
         """
         try:
-            response = self._request_http_response(f'https://www.collinsdictionary.com/dictionary/english-thesaurus/{self._word}')
+            response = self._request_http_response(url=f'https://www.collinsdictionary.com/dictionary/english-thesaurus/{self._word}')
 
             if response.status_code == 404:
                 logger.error(f'Collins Dictionary had no definition reference for the word {self._word}')
                 return None
             else:
-                soup = BeautifulSoup(response.text, "lxml")
-                cloudflare_protection = CloudflareVerification('https://www.collinsdictionary.com',
-                                                               soup).cloudflare_protected_url()
-                if cloudflare_protection is False:
-                    definition_list = []
-                    part_of_speech_category = ''
+                soup_object = BeautifulSoup(markup=response.text, features="lxml")
+                cloudflare_protection = CloudflareVerification(url='https://www.collinsdictionary.com',
+                                                               soup=soup_object).cloudflare_protected_url()
 
-                    # obtain the part of speech category for the specific word
-                    if soup.find('span', {'class': 'headerSensePos'}):
-                        tag_part_of_speech = soup.find('span', {'class': 'headerSensePos'})
-                        if len(tag_part_of_speech.text) != 0:
-                            part_of_speech_category = tag_part_of_speech.text.strip('()')
-                        else:
-                            part_of_speech_category = ''
-
-                    query_results = soup.find('div', {'class': 'form type-def titleTypeSubContainer'})
-                    if query_results is not None:
-                        definition = query_results.findNext('div', {'class': 'def'})
-                        definition_list.append(definition.text.strip())
-                        self._update_cache(part_of_speech_category, definition_list)
-                        return definition_list, part_of_speech_category
-                    elif query_results is None:
-                        logger.error(f'Collins Dictionary had no definition reference for the word {self._word}')
-                        return None
+                if cloudflare_protection is False:
+                    definition_list = ParseDefinitions.parse_collins_dictionary(soup=soup_object, word=self._word)
+                    part_of_speech_category = PartOfSpeech.part_of_speech_category_collins_dictionary(soup=soup_object)
+                    self._update_cache(pos_category=part_of_speech_category, definition=definition_list)
+                    return definition_list, part_of_speech_category
                 elif cloudflare_protection is True:
-                    fresh_soup = Cloudflare(
-                        f'https://www.collinsdictionary.com/dictionary/english-thesaurus/{self._word}').bypass()
-
-                    definition_list = []
-                    part_of_speech_category = ''
-
-                    # obtain the part of speech category for the specific word
-                    if fresh_soup.find('span', {'class': 'headerSensePos'}):
-                        tag_part_of_speech = fresh_soup.find('span', {'class': 'headerSensePos'})
-                        if len(tag_part_of_speech.text) != 0:
-                            part_of_speech_category = tag_part_of_speech.text.strip('()')
-                        else:
-                            part_of_speech_category = ''
-
-                    query_results = fresh_soup.find('div', {'class': 'form type-def titleTypeSubContainer'})
-                    if query_results is not None:
-                        definition = query_results.findNext('div', {'class': 'def'})
-                        definition_list.append(definition.text.strip())
-                        self._update_cache(part_of_speech_category, definition_list)
-                        return definition_list, part_of_speech_category
-                    elif query_results is None:
-                        logger.error(f'Collins Dictionary had no definition reference for the word {self._word}')
+                    soup_object = Cloudflare(url=f'https://www.collinsdictionary.com/dictionary/english-thesaurus/{self._word}').bypass()
+                    if soup_object:
+                        definition_list = ParseDefinitions.parse_collins_dictionary(soup=soup_object, word=self._word)
+                        part_of_speech_category = PartOfSpeech.part_of_speech_category_collins_dictionary(soup_object)
+                        self._update_cache(pos_category=part_of_speech_category, definition=definition_list)
                         return definition_list, part_of_speech_category
-
-        except bs4.FeatureNotFound as error:
-            logger.error('An error occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except AttributeError as error:
-            logger.error('An AttributeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except IndexError as error:
-            logger.error('An IndexError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except KeyError as error:
-            logger.error('A KeyError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except TypeError as error:
-            logger.error('A TypeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            self._handle_query_exceptions(error)
 
     def _query_merriam_webster(self) -> Union[Tuple[List[str], str], None]:
         """
         This function queries merriam-webster.com for a definition associated
         with the specific word provided to the Class Definitions
 
-        :returns:
-            definitions: definition for a word
-
-        :rtype: list
-
+        :returns:definition for a word
+        :rtype: Union[Tuple[List[str], str], None]
         :raises:
-            AttributeError: Raised when an attribute reference or assignment fails
-
-            IndexError: Raised when a sequence subscript is out of range
-
-            KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys
-
-            TypeError: Raised when an operation or function is applied to an object of inappropriate type
-
-            bs4.FeatureNotFound: raised by the BeautifulSoup constructor if no parser with the requested features
-            is found
+            - AttributeError: When an attribute reference or assignment fails.
+            - IndexError: When a sequence subscript is out of range.
+            - KeyError: When a mapping key is not found in the set of existing keys.
+            - TypeError: When an operation or function is applied to an inappropriate type.
+            - bs4.FeatureNotFound: Raised by the BeautifulSoup constructor if no parser with the requested features is found.
         """
         try:
-            response = self._request_http_response(f'https://www.merriam-webster.com/dictionary/{self._word}')
+            response = self._request_http_response(url=f'https://www.merriam-webster.com/dictionary/{self._word}')
 
             if response.status_code == 404:
                 logger.info(f'Merriam-webster.com has no definition reference for the word {self._word}')
                 return None
             else:
-                soup = BeautifulSoup(response.text, "lxml")
-                cloudflare_protection = CloudflareVerification('https://www.merriam-webster.com',
-                                                               soup).cloudflare_protected_url()
+                soup_object = BeautifulSoup(markup=response.text, features="lxml")
+                cloudflare_protection = CloudflareVerification(url='https://www.merriam-webster.com',
+                                                               soup=soup_object).cloudflare_protected_url()
 
                 if cloudflare_protection is False:
-                    pattern = regex.compile(r'Words fail us')
-                    if soup.find(text=pattern):
+                    pattern = regex.compile(pattern=r'Words fail us')
+                    if soup_object.find(text=pattern):
                         logger.info(f'Merriam-webster.com has no reference for the word {self._word}')
                         return None
-                    elif soup.find('h1', {'class': 'mispelled-word'}):
+                    elif soup_object.find(name='h1', attrs={'class': 'mispelled-word'}):
                         logger.info(f'Merriam-webster.com has no definition reference for the word {self._word}')
                         return None
                     else:
-                        definition_list = []
-                        part_of_speech_category = ''
-                        # obtain the part of speech category for the specific word
-                        if soup.select(
-                            '#dictionary-entry-1 > div.row.entry-header > div > '
-                            'div.entry-header-content.d-flex.flex-wrap.align-items-baseline.flex-row.mb-0 > h2 > a'):
-                            css_part_of_speech = soup.select(
-                                '#dictionary-entry-1 > div.row.entry-header > div > div.entry-header-content.d-flex.flex-wrap.align-items-baseline.flex-row.mb-0 > h2 > a')
-                            if len(css_part_of_speech[0].text) != 0:
-                                part_of_speech_category = css_part_of_speech[0].text.split()[0]
-                            else:
-                                part_of_speech_category = ''
-
-                        dictionary_entry = soup.find('div', {'id': 'dictionary-entry-1'})
-                        definition_container = dictionary_entry.find('div', {'class': 'vg'})
-                        definition_entries = definition_container.find('div', {'class': 'sb-0 sb-entry'})
-                        for definition_entry in definition_entries.find_all('span', {'class': 'dtText'}):
-                            definition_list.append(definition_entry.text.lower().replace(':', '').strip())
-                        self._update_cache(part_of_speech_category, definition_list)
+                        definition_list = ParseDefinitions.parse_merriam_webster(soup=soup_object)
+                        part_of_speech_category = PartOfSpeech.part_of_speech_category_merriam_webster(soup=soup_object)
+                        self._update_cache(pos_category=part_of_speech_category, definition=definition_list)
                         return definition_list, part_of_speech_category
                 elif cloudflare_protection is True:
                     return None
-
-        except bs4.FeatureNotFound as error:
-            logger.error('An error occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except AttributeError as error:
-            logger.error('An AttributeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except IndexError as error:
-            logger.error('An IndexError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except KeyError as error:
-            logger.error('A KeyError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except TypeError as error:
-            logger.error('A TypeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            self._handle_query_exceptions(error)
 
     def _query_synonym_com(self) -> Union[Tuple[List[str], str], None]:
         """
         This function queries synonym.com for a definition associated
         with the specific word provided to the Class Definitions
 
-        :returns:
-            definitions: definition for a word
-
-        :rtype: list
-
+        :returns:definition for a word
+        :rtype: Union[Tuple[List[str], str], None]
         :raises:
-            AttributeError: Raised when an attribute reference or assignment fails
-
-            IndexError: Raised when a sequence subscript is out of range
-
-            KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys
-
-            TypeError: Raised when an operation or function is applied to an object of inappropriate type
-
-            bs4.FeatureNotFound: raised by the BeautifulSoup constructor if no parser with the requested features
-            is found
+            - AttributeError: When an attribute reference or assignment fails.
+            - IndexError: When a sequence subscript is out of range.
+            - KeyError: When a mapping key is not found in the set of existing keys.
+            - TypeError: When an operation or function is applied to an inappropriate type.
+            - bs4.FeatureNotFound: Raised by the BeautifulSoup constructor if no parser with the requested features is found.
         """
         try:
-            response = self._request_http_response(f'https://www.synonym.com/synonyms/{self._word}')
+            response = self._request_http_response(url=f'https://www.synonym.com/synonyms/{self._word}')
 
             if response.status_code == 404:
                 logger.info(f'Synonym.com had no definition reference for the word {self._word}')
                 return None
             else:
-
-                soup = BeautifulSoup(response.text, "lxml")
-                cloudflare_protection = CloudflareVerification('https://www.synonym.com',
-                                                               soup).cloudflare_protected_url()
+                soup_object = BeautifulSoup(markup=response.text, features="lxml")
+                cloudflare_protection = CloudflareVerification(url='https://www.synonym.com',
+                                                               soup= soup_object).cloudflare_protected_url()
                 if cloudflare_protection is False:
-                    definition_list = []
-                    part_of_speech_category = ''
-
-                    status_tag = soup.find("meta", {"name": "pagetype"})
-                    pattern = regex.compile(r'Oops, 404!')
-                    if soup.find(text=pattern):
+                    status_tag =  soup_object.find(name="meta", attrs={"name": "pagetype"})
+                    pattern = regex.compile(pattern=r'Oops, 404!')
+                    if  soup_object.find(text=pattern):
                         logger.info(f'Synonym.com had no definition reference for the word {self._word}')
-                        return definition_list, part_of_speech_category
+                        return None
                     elif status_tag.attrs['content'] == 'Term':
-                        # obtain the part of speech category for the specific word
-                        if soup.select(
-                            'body > div.page-container > div.content-container > div.main-column > '
-                            'div.sections-wrapper > div:nth-child(1) > p > strong'):
-                            css_part_of_speech = soup.select(
-                                'body > div.page-container > div.content-container > div.main-column > div.sections-wrapper > div:nth-child(1) > p > strong')
-                            if len(css_part_of_speech[0].text) != 0:
-                                part_of_speech_category = css_part_of_speech[0].text.rstrip('.')
-                            else:
-                                part_of_speech_category = ''
-
-                        dictionary_entries = soup.find('h3', {'class': 'section-title'})
-                        dictionary_entry = dictionary_entries.find_next('p').text
-                        remove_brackets = regex.sub(r'.*?\[.*?\]', '', dictionary_entry)
-                        remove_spaces = cleansing.remove_excess_whitespace(remove_brackets)
-                        definition_list.append(remove_spaces)
-                        self._update_cache(part_of_speech_category, definition_list)
+                        definition_list = ParseDefinitions.parse_synonym_com(soup=soup_object)
+                        part_of_speech_category = PartOfSpeech.part_of_speech_category_synonym_com(soup=soup_object)
+                        self._update_cache(pos_category=part_of_speech_category, definition=definition_list)
                         return definition_list, part_of_speech_category
                 elif cloudflare_protection is True:
                     return None
-
-        except bs4.FeatureNotFound as error:
-            logger.error('An error occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except AttributeError as error:
-            logger.error('An AttributeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except IndexError as error:
-            logger.error('An IndexError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except KeyError as error:
-            logger.error('A KeyError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except TypeError as error:
-            logger.error('A TypeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            self._handle_query_exceptions(error)
 
     def _query_thesaurus_com(self) -> Union[Tuple[List[str], str], None]:
         """
         This function queries thesaurus.com for a definition associated
-        with the specific word provided to the Class Synonyms.
-
-        :returns:
-            definitions: definition for a word
-
-        :rtype: list
+        with the specific word provided to the Class Definitions.
 
+        :returns:definition for a word
+        :rtype: Union[Tuple[List[str], str], None]
         :raises:
-            AttributeError: Raised when an attribute reference or assignment fails
-
-            IndexError: Raised when a sequence subscript is out of range
-
-            KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys
-
-            TypeError: Raised when an operation or function is applied to an object of inappropriate type
-
-            bs4.FeatureNotFound: raised by the BeautifulSoup constructor if no parser with the requested features
-            is found
+            - AttributeError: When an attribute reference or assignment fails.
+            - IndexError: When a sequence subscript is out of range.
+            - KeyError: When a mapping key is not found in the set of existing keys.
+            - TypeError: When an operation or function is applied to an inappropriate type.
+            - bs4.FeatureNotFound: Raised by the BeautifulSoup constructor if no parser with the requested features is found.
         """
         try:
-            response = self._request_http_response(f'https://www.thesaurus.com/browse/{self._word}')
+            response = self._request_http_response(url=f'https://www.thesaurus.com/browse/{self._word}')
 
             if response.status_code == 404:
                 logger.info(f'Thesaurus.com had no definition reference for the word {self._word}')
                 return None
             else:
-                soup = BeautifulSoup(response.text, "lxml")
-                cloudflare_protection = CloudflareVerification('https://www.thesaurus.com',
-                                                               soup).cloudflare_protected_url()
+                soup_object = BeautifulSoup(markup=response.text, features="lxml")
+                cloudflare_protection = CloudflareVerification(url='https://www.thesaurus.com',
+                                                               soup=soup_object).cloudflare_protected_url()
                 if cloudflare_protection is False:
-                    status_tag = soup.find("h1")
+                    status_tag = soup_object.find(name="h1")
                     if status_tag.text.startswith('0 results for'):
                         logger.info(f'Thesaurus.com had no definition reference for the word {self._word}')
                         return None
                     else:
-                        definition_list = []
-                        part_of_speech_category = ''
-
-                        # obtain the part of speech category for the specific word
-                        if soup.select('#headword > div.css-bjn8wh.e1br8a1p0 > div > ul > li > a > em'):
-                            css_part_of_speech = soup.select('#headword > div.css-bjn8wh.e1br8a1p0 > div > ul > li > a > em')
-                            if len(css_part_of_speech[0].text) != 0:
-                                part_of_speech_category = css_part_of_speech[0].text.rstrip('.')
-                            else:
-                                part_of_speech_category = ''
-
-                        if soup.select('#headword > div.css-bjn8wh.e1br8a1p0 > div > ul > li > a > strong'):
-                            css_definition = soup.select('#headword > div.css-bjn8wh.e1br8a1p0 > div > ul > li > a > strong')
-                            if len(css_definition[0].text) != 0:
-                                definition_list.append(css_definition[0].text)
-                        self._update_cache(part_of_speech_category, definition_list)
+                        definition_list = ParseDefinitions.parse_thesaurus_com(soup=soup_object)
+                        part_of_speech_category = PartOfSpeech.part_of_speech_category_thesaurus_com(soup=soup_object)
+                        self._update_cache(pos_category=part_of_speech_category, definition=definition_list)
                         return definition_list, part_of_speech_category
                 elif cloudflare_protection is True:
                     return None
-
-        except bs4.FeatureNotFound as error:
-            logger.error('An error occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except AttributeError as error:
-            logger.error('An AttributeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except IndexError as error:
-            logger.error('An IndexError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except KeyError as error:
-            logger.error('A KeyError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except TypeError as error:
-            logger.error('A TypeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            self._handle_query_exceptions(error)
```

### Comparing `wordhoard-1.5.4/wordhoard/files/common_english_homophones.pkl` & `wordhoard-1.5.5/wordhoard/files/common_english_homophones.pkl`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.4/wordhoard/files/common_user_agents.pkl` & `wordhoard-1.5.5/wordhoard/files/common_user_agents.pkl`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.4/wordhoard/files/no_homophones_english.pkl` & `wordhoard-1.5.5/wordhoard/files/no_homophones_english.pkl`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.4/wordhoard/homophones.py` & `wordhoard-1.5.5/wordhoard/homophones.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python3
 
 """
-This Python script is designed to query internal repositories for the
+This Python module is designed to query internal repositories for the
 homophones associated with the given word.
 """
 __author__ = 'John Bumgarner'
 __date__ = 'June 11, 2021'
 __status__ = 'Production'
 __license__ = 'MIT'
 __copyright__ = "Copyright (C) 2021 John Bumgarner"
 
 ##################################################################################
 # Date Completed: June 11, 2021
 # Author: John Bumgarner
 #
-# Date Last Revised: May 31, 2023
+# Date Last Revised: May 09, 2024
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # “AS-IS” Clause
 #
 # Except as represented in this agreement, all work produced by Developer is
@@ -27,155 +27,158 @@
 # including any warranty of merchantability and warranty of fitness for a particular
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
+# Standard library imports
 import os
 import sys
 import pickle
 import logging
 import traceback
 from typing import List, Union
+
+# Local or project-specific imports
 from wordhoard.utilities import word_verification
 from wordhoard.utilities.colorized_text import colorized_text
 
 logger = logging.getLogger(__name__)
 
-PARENT_DIRECTORY = os.path.dirname(os.path.abspath(__file__))
-
-# Opening the pickle file that contains a nested list of common
-# English language homophones.
-try:
-    _file_known_homophones = os.path.join(PARENT_DIRECTORY, 'files/common_english_homophones.pkl')
-    with open(_file_known_homophones, 'rb') as _eng_homophones:
-        _known_homophones_list = pickle.load(_eng_homophones)
-        _eng_homophones.close()
-except FileNotFoundError as error:
-    logger.error('The common_english_homophones.pkl file was not found. Aborting operation.')
-    logger.error(''.join(traceback.format_tb(error.__traceback__)))
-    sys.exit(1)
-except OSError as error:
-    logger.error(f"An OS error occurred when trying to open the file common_english_homophones.pkl")
-    logger.error(''.join(traceback.format_tb(error.__traceback__)))
-    sys.exit(1)
-
-# Opening the pickle file that contains a nested list of English
-# language words that have no known homophones.
-try:
-    _file_no_known_homophones = os.path.join(PARENT_DIRECTORY, 'files/no_homophones_english.pkl')
-    with open(_file_no_known_homophones, 'rb') as _no_eng_homophones:
-        _no_homophones_list = pickle.load(_no_eng_homophones)
-        _no_eng_homophones.close()
-except FileNotFoundError as error:
-    logger.error('The no_homophones_english.pkl file was not found. Aborting operation.')
-    logger.error(''.join(traceback.format_tb(error.__traceback__)))
-    sys.exit(1)
-except OSError as error:
-    logger.error(f"An OS error occurred when trying to open the file no_homophones_english.pkl")
-    logger.error(''.join(traceback.format_tb(error.__traceback__)))
-    sys.exit(1)
-
-
-class Homophones(object):
+# Define module-level variables to store loaded data
+_known_homophones_list = []
+_no_homophones_list = []
+
+class PickleLoader:
+    """
+        A utility class for loading pickle files containing English homophones and
+        English words with no known homophones.
+    """
+
+    @staticmethod
+    def load_pickle_files() -> None:
+        """
+            Loads pickle files containing English homophones and English words with no known homophones.
+
+            :returns: None
+            :rtype: NoneType
+        """
+        global _known_homophones_list, _no_homophones_list
+        parent_directory = os.path.dirname(os.path.abspath(__file__))
+        _file_known_homophones = os.path.join(parent_directory, 'files/common_english_homophones.pkl')
+        _file_no_known_homophones = os.path.join(parent_directory, 'files/no_homophones_english.pkl')
+
+        try:
+                # Opening the pickle file that contains a nested list of common
+                # English language homophones.
+            with open(file=_file_known_homophones, mode='rb') as _eng_homophones:
+                _known_homophones_list = pickle.load(file=_eng_homophones)
+        except (FileNotFoundError, OSError) as error:
+            PickleLoader.handle_pickle_load_error(_file_known_homophones, error)
+
+        try:
+            # Opening the pickle file that contains a nested list of English
+            # language words that have no known homophones.
+            with open(file=_file_no_known_homophones, mode='rb') as _no_eng_homophones:
+                _no_homophones_list = pickle.load(file=_no_eng_homophones)
+        except (FileNotFoundError, OSError) as error:
+            PickleLoader.handle_pickle_load_error(_file_no_known_homophones, error)
+
+    @staticmethod
+    def handle_pickle_load_error(file_path: str, error: Exception) -> None:
+        """
+            Handles errors when loading pickle files.
+
+            :arg file_path: The path of the pickle file.
+            :arg type file_path: str
+            :arg error: The error raised during file loading.
+            :arg type error: Exception
+            :returns: None
+            :rtype; NoneType
+        """
+        if isinstance(error, FileNotFoundError):
+            logger.error(f'The pickle file {file_path} was not found. Aborting operation.')
+        else:
+            logger.error(f"An OS error occurred when trying to open the pickle file {file_path}")
+        logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        sys.exit(1)
 
-    def __init__(self,
-                 search_string: str = ''):
+PickleLoader.load_pickle_files()
 
-        """
+class Homophones:
+    """
         Purpose
         ----------
         This Python class is used to query internal files containing
         English language homophones associated with a specific word.
 
         Usage Examples
         ----------
-
         >>> homophones = Homophones('horse')
         >>> results = homophones.find_homophones()
 
-        >>> homophones = Homophones(search_string='horse')
-        >>> results = homophones.find_homophones()
-
         Parameters
         ----------
         :param search_string: string containing the variable to obtain homophones for
         """
 
+    def __init__(self,
+                 search_string: str = ''):
+
         self._word = search_string
 
     def _validate_word(self) -> bool:
         """
         This function is designed to validate that the syntax for
         a string variable is in an acceptable format.
 
         :return: True or False
         :rtype: boolean
         """
         valid_word = word_verification.validate_word_syntax(self._word)
-        if valid_word:
-            return True
-        else:
+        if not valid_word:
             logger.error(f'The word {self._word} was not in a valid format.')
             logger.error(f'Please verify that the word {self._word} is spelled correctly.')
-            return False
+        return valid_word
 
     def _common_english_homophones(self) -> List[str]:
         """
         This function iterates through a list of known
         English language homophones.
 
         :return: list of homophones
         :rtype: list
         """
-        global _known_homophones_list
-        rtn_list = []
+        homophones_list = []
         for homophones in _known_homophones_list:
-            match = bool([word for word in homophones if word == self._word])
-            if match:
-                for word in homophones:
-                    if word != self._word:
-                        rtn_list.append(f'{self._word} is a homophone of {word}')
-        if len(rtn_list) > 0:
-            return list(set(rtn_list))
+            if any(word == self._word for word in homophones):
+                homophones_list.extend(
+                    f'{self._word} is a homophone of {word}' for word in homophones if word != self._word)
+        return list(set(homophones_list))
 
-    def _english_words_without_homophones(self) -> None:
+    def _english_words_without_homophones(self) -> bool:
         """
         This function iterates through a list of English
         language words with no known homophones.
 
-        :return: no homophones for word
-        :rtype: str
+        :return: True or False
+        :rtype: bool
         """
-        global _no_homophones_list
-        match = bool(self._word in _no_homophones_list)
-        if match:
-            return None
+        return self._word in _no_homophones_list
 
     def find_homophones(self) -> Union[List[str], None]:
         """
-        Purpose
-        ----------
-        This function queries multiple lists to find
-        English language homophones associated with the
-        specific word provided to the Class Homophones.
-
-        Returns
-        ----------
-        :return:
-            homophones: list of homophones
-            no_homophones: string
+        This function queries multiple lists to find English language homophones associated
+        with the specific word provided to the Class Homophones.
 
-        :rtype: list
-        :rtype: str
+        :return: list of homophones
+        :rtype: Union[List[str]
         """
-        valid_word = self._validate_word()
-        if valid_word:
+        if self._validate_word():
             known_english_homophones = self._common_english_homophones()
             if known_english_homophones:
                 return known_english_homophones
-            elif not known_english_homophones:
-                if self._english_words_without_homophones() is None:
-                    colorized_text(f'No homophones for the word - {self._word}', 'magenta')
-                    return None
-
+            elif self._english_words_without_homophones() is False:
+                colorized_text(text=f'No homophones for the word - {self._word}', color='magenta')
+                return None
+        return None
```

### Comparing `wordhoard-1.5.4/wordhoard/hypernyms.py` & `wordhoard-1.5.5/wordhoard/utilities/request_html.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,342 +1,294 @@
 #!/usr/bin/env python3
 
 """
-This Python script is designed to query an online repository for the
-hypernyms associated with a specific word.
+This Python script provide basic requests.get function and BeautifulSoup parent tag extraction.
 """
 __author__ = 'John Bumgarner'
-__date__ = 'June 12, 2021'
+__date__ = 'October 15, 2020'
 __status__ = 'Production'
 __license__ = 'MIT'
-__copyright__ = "Copyright (C) 2021 John Bumgarner"
-
-##################################################################################
-# Date Initially Completed: June 12, 2021
-# Author: John Bumgarner
-#
-# Date Last Revised: May 31, 2023
-# Revised by: John Bumgarner
-##################################################################################
+__copyright__ = "Copyright (C) 2020 John Bumgarner"
 
 ##################################################################################
 # “AS-IS” Clause
 #
 # Except as represented in this agreement, all work produced by Developer is
 # provided “AS IS”. Other than as provided in this agreement, Developer makes no
 # other warranties, express or implied, and hereby disclaims all implied warranties,
 # including any warranty of merchantability and warranty of fitness for a particular
 # purpose.
 ##################################################################################
 
 ##################################################################################
+# Date Completed: October 15, 2020
+# Author: John Bumgarner
+#
+# Date Last Revised: May 12, 2024
+# Revised by: John Bumgarner
+##################################################################################
+
+##################################################################################
 # Python imports required for basic operations
 ##################################################################################
-import bs4
+# Standard library imports
 import sys
-import json
 import logging
+import warnings
 import traceback
-from bs4 import BeautifulSoup
-from backoff import on_exception, expo
-from ratelimit import limits, RateLimitException
-from wordhoard.utilities.request_html import Query
-from typing import List, Dict, Optional, Set, Tuple, Union
-from wordhoard.utilities.colorized_text import colorized_text
-from wordhoard.utilities import caching, cleansing, word_verification
-from wordhoard.utilities.cloudflare_checker import CloudflareVerification
+from typing import Dict, Optional, Tuple
 
-logger = logging.getLogger(__name__)
-
-
-def _get_number_of_pages(soup: BeautifulSoup) -> int:
-    """
-    This function determines the number of pages that
-    contain hypernyms and hyperonyms for a specific word.
+# Third-party imports
+import requests
+from requests.adapters import Retry
+from requests.adapters import HTTPAdapter
+from urllib3.exceptions import MaxRetryError
 
-    :param soup: BeautifulSoup lxml
-    :return: number of pages
-    :rtype: int
+# Local or project-specific imports
+from wordhoard.utilities.colorized_text import colorized_text
+from wordhoard.utilities.user_agents import get_random_user_agent
 
-    :raises:
-        AttributeError: Raised when an attribute reference or assignment fails.
+warnings.filterwarnings('ignore', message='Unverified HTTPS request')
 
-        KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys.
+logger = logging.getLogger(__name__)
 
-        TypeError: Raised when an operation or function is applied to an object of inappropriate type.
-    """
-    try:
-        number_of_pages = 0
-        pages = soup.find('div', {'id': 'pages'})
-        if pages is not None:
-            list_of_pages = [num for page in pages for num in page if num.isdigit()]
-            if len(list_of_pages) != 0:
-                number_of_pages = int(list_of_pages[-1]) + 1
-        return number_of_pages
-
-    except AttributeError as e:
-        logger.error('An AttributeError occurred in the following code segment:')
-        logger.error(''.join(traceback.format_tb(e.__traceback__)))
-    except KeyError as e:
-        logger.error('A KeyError occurred in the following code segment:')
-        logger.error(''.join(traceback.format_tb(e.__traceback__)))
-    except TypeError as e:
-        logger.error('A TypeError occurred in the following code segment:')
-        logger.error(''.join(traceback.format_tb(e.__traceback__)))
+##################################################################
+# Select a random user agent from the array of user agent choices
+##################################################################
+rand_user_agent = get_random_user_agent()
+
+############################################
+# Create http request for harvest operation
+############################################
+http_headers = {'user-agent': rand_user_agent}
 
 
-def _get_hypernyms(soup: BeautifulSoup) -> Set[str]:
+class Query:
     """
-    This function queries an HTML table for hypernyms.
-
-    :param soup: BeautifulSoup lxml
-    :return: set of hypernyms and hyperonyms
-    :rtype: set
+        A class for querying and scraping data from a specified URL.
 
-    :raises:
-        AttributeError: Raised when an attribute reference or assignment fails.
+        Args:
+            url_to_scrape (str): The URL to scrape data from.
+            user_agent (Optional[str]): The user agent string to use in the request headers.
+            proxies (Optional[Dict[str, str]]): Dictionary of proxies to use for the request.
 
-        KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys.
+        Methods:
+            get_website_html(): Open an HTTP connection and harvest HTML from the initial source URL.
 
-        TypeError: Raised when an operation or function is applied to an object of inappropriate type.
+        This class provides methods to perform HTTP requests, handle response codes, and log relevant information
+        about the request process. It also handles exceptions related to HTTP requests, proxies, and connection errors.
     """
-    try:
-        sub_set = set()
-        table = soup.find('table')
-        if table:
-            rows = table.find_all('tr', {'class': 'theentry'})
-            if rows is not None:
-                for row in rows:
-                    cols = row.find('td', {'class': 'abbdef'}).find('a')
-                    if cols is not None:
-                        if cols.text != '»':
-                            sub_set.add(str(cols.text).lower())
-                        else:
-                            sub_set.add('no hypernyms found')
-            return sub_set
-
-    except AttributeError as e:
-        logger.error('An AttributeError occurred in the following code segment:')
-        logger.error(''.join(traceback.format_tb(e.__traceback__)))
-    except KeyError as e:
-        logger.error('A KeyError occurred in the following code segment:')
-        logger.error(''.join(traceback.format_tb(e.__traceback__)))
-    except TypeError as e:
-        logger.error('A TypeError occurred in the following code segment:')
-        logger.error(''.join(traceback.format_tb(e.__traceback__)))
-
-
-class Hypernyms(object):
-
     def __init__(self,
-                 search_string: str = '',
-                 output_format: str = 'list',
-                 max_number_of_requests: int = 30,
-                 rate_limit_timeout_period: int = 60,
+                 url_to_scrape: str = '',
                  user_agent: Optional[str] = None,
                  proxies: Optional[Dict[str, str]] = None):
 
-        """
-        Purpose
-        ----------
-        This Python class is used to query online repositories for the hypernyms
-        associated with a specific word.
-
-        Usage Examples
-        ----------
-
-        >>> hypernym = Hypernyms('red')
-        >>> results = hypernym.find_hypernyms()
-
-        >>> hypernym = Hypernyms(search_string='red')
-        >>> results = hypernym.find_hypernyms()
-
-        Parameters
-        ----------
-        :param search_string: string containing the variable to obtain hypernyms for
-
-        :param max_number_of_requests: maximum number of requests for a specific timeout_period
-
-        :param rate_limit_timeout_period: the time period before a session is placed in a temporary hibernation mode
-
-        :param user_agent: string containing either a global user agent type or a specific user agent
-
-        :param proxies: dictionary of proxies to use with Python Requests
-        """
+        # Reformat complex words, such as 'artificial intelligence' contained in a URL
+        # with a string.replace. The new format is 'artificial%20intelligence', which
+        # can be passed Python Requests as a quoted string
+        self._url_to_scrape = url_to_scrape.replace(" ", "%20")
 
         self._proxies = proxies
-        self._word = search_string
         self._user_agent = user_agent
-        self._output_format = output_format
-        self._valid_output_formats = {'dictionary', 'list', 'json'}
 
-        rate_limit_status = False
-        self._rate_limit_status = rate_limit_status
+    def _handle_http_status_codes(self, status_code: int):
+        """
+        Handle specific HTTP status codes and log appropriate messages.
 
-        # Retries the requests after a certain time period has elapsed
-        handler = on_exception(expo, RateLimitException, max_time=60, on_backoff=self._backoff_handler)
-        # Establishes a rate limit for making requests to the hypernyms repositories
-        limiter = limits(calls=max_number_of_requests, period=rate_limit_timeout_period)
-        self.find_hypernyms = handler(limiter(self.find_hypernyms))
-
-    def _backoff_handler(self):
-        if self._rate_limit_status is False:
-            colorized_text('The hypernym query rate limit was reached. The querying process is entering '
-                           'a temporary hibernation mode.', 'red')
-            logger.info('The hypernym query rate limit was reached.')
-            self._rate_limit_status = True
+        This method checks the provided HTTP status code and logs detailed
+        information for certain status codes, including 404, 500, 503, 504, and 521.
+        It also outputs colorized text for some of these status codes.
 
-    def _validate_word(self) -> bool:
+        :param status_code: The HTTP status code to handle.
+        :type status_code: int
         """
-        This function is designed to validate that the syntax for a string variable is in an acceptable format.
+        if status_code == 404:
+            logger.info('-' * 80)
+            logger.error(f'Response Status Code: {status_code}')
+            logger.info(
+                'The HTTP 404 Not Found status code means that the file or page that the was requested '
+                'was not found on the server')
+            logger.info(f'Requested URL: {self._url_to_scrape}')
+            logger.info('-' * 80)
+        elif status_code == 500:
+            colorized_text(text='An HTTP 500 Internal Server Error has occurred.'
+                           '\nPlease review the WordHoard logs for additional information.', color='red')
+            logger.info('-' * 80)
+            logger.error(f'Response Status Code: {status_code}')
+            logger.info(
+                "The HTTP 500 Internal Server Error status code indicates that the server encountered "
+                "an unexpected condition that prevented it from fulfilling the request.")
+            logger.info(f'Requested URL: {self._url_to_scrape}')
+            logger.info('-' * 80)
+        elif status_code == 503:
+            colorized_text(text='A 503 Service Unavailable status code has been detected.'
+                                '\nPlease review the WordHoard logs for additional information.', color='red')
+            logger.info('-' * 80)
+            logger.error(f'Response Status Code: {status_code}')
+            logger.info(
+                "The 503 Service Unavailable status code indicates that the server is temporarily unable "
+                "to handle the request")
+            logger.error(f'Requested URL: {self._url_to_scrape}')
+            logger.info('-' * 80)
+        elif status_code == 504:
+            colorized_text(text='An HTTP 504 Gateway Timeout Error status code has been detected.'
+                                '\nPlease review the WordHoard logs for additional information.', color='red')
+            logger.info('-' * 80)
+            logger.error(f'Response Status Code: {status_code}')
+            logger.info(
+                "The HTTP 504 Gateway Timeout Error status code indicating that a server, which is "
+                "currently acting as a gateway or proxy, did not receive a timely response "
+                "from another server")
+            logger.error(f'Requested URL: {self._url_to_scrape}')
+            logger.info('-' * 80)
+        elif status_code == 521:
+            colorized_text(text='A 521 status code has been detected. This code is often used by CloudFlare.'
+                                '\nPlease review the WordHoard logs for additional information.', color='red')
+            logger.info('-' * 80)
+            logger.error(f'Response Status Code: {status_code}')
+            logger.info("This status code is not specified in any RFCs, but is used by CloudFlare's"
+                        "reverse proxies to indicate that the origin webserver refused the connection")
+            logger.info(f'Requested URL: {self._url_to_scrape}')
+            logger.info('-' * 80)
 
-        :return: True or False
-        :rtype bool
+    def _handle_exceptions(self, error):
         """
-        valid_word = word_verification.validate_word_syntax(self._word)
-        if valid_word:
-            return True
-        else:
-            logger.error(f'The word {self._word} was not in a valid format.')
-            logger.error(f'Please verify that the word {self._word} is spelled correctly.')
-            return False
-
-    def _check_cache(self)-> Tuple[bool, Union[List[str], None]]:
-        check_cache = caching.cache_hypernyms(self._word)
-        return check_cache
-
-    def _update_cache(self, hypernym: List[str]) -> None:
-        caching.insert_word_cache_hypernyms(self._word, hypernym)
-        return
-
-    def find_hypernyms(self) -> Union[List[str], Dict[str, List[str]], str, None]:
+        Helper method to handle Python Request exceptions
         """
-        Purpose
-        ----------
-        This function queries classicthesaurus_com for hypernyms associated
-        with the specific word provided to the Class Hypernyms.
-
-        Returns
-        ----------
-        :returns:
-            hypernym: list of hypernyms
-
-        :rtype: list
-
-        Raises
-        ----------
-        :raises
-            AttributeError: Raised when an attribute reference or assignment fails
-
-            IndexError: Raised when a sequence subscript is out of range
+        if isinstance(error, requests.HTTPError):
+            colorized_text(text='A HTTPError has occurred.'
+                                '\nPlease review the WordHoard logs for additional information.', color='red')
+            logger.error(f'A HTTPError has occurred when requesting {self._url_to_scrape}')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+            sys.exit(1)
+        elif isinstance(error, requests.URLRequired):
+            logger.error(f'A URLRequired has occurred when requesting {self._url_to_scrape}')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+            sys.exit(1)
+        elif isinstance(error, requests.exceptions.ProxyError):
+            colorized_text(text='A unknown type of Proxy Error has occurred.'
+                                '\nPlease verify that your proxies are working.', color='red')
+            logger.error(f'A ProxyError has occurred when requesting {self._url_to_scrape}')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+            sys.exit(1)
+        elif isinstance(error, MaxRetryError):
+            colorized_text(text='The max number of connection retries was exceeded.'
+                                '\nPlease review the WordHoard logs for additional information.', color='red')
+            logger.error(f'A MaxRetryError has occurred when requesting {self._url_to_scrape}')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+            sys.exit(1)
+        elif isinstance(error, requests.ConnectionError):
+            colorized_text(text='A ConnectionError has occurred.'
+                                '\nPlease review the WordHoard logs for additional information.', color='red')
+            logger.error(f'A ConnectionError has occurred when requesting {self._url_to_scrape}')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+            sys.exit(1)
+        elif isinstance(error, requests.Timeout):
+            colorized_text(text='A connection timeout has occurred.'
+                           '\nPlease review the WordHoard logs for additional information.', color='red')
+            logger.error(f'A Timeout has occurred when requesting {self._url_to_scrape}')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+            sys.exit(1)
+        elif isinstance(error, requests.RequestException):
+            colorized_text(text='A RequestException has occurred.'
+                           '\nPlease review the WordHoard logs for additional information.', color='red')
+            logger.error(f'A RequestException has occurred when requesting {self._url_to_scrape}')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+            sys.exit(1)
 
-            KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys
+    # reference: https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#module-urllib3.util.retry
+    @staticmethod
+    def _requests_retry_session(retries: int = 5,
+                                backoff_factor: float = 0.5,
+                                status_forcelist: Tuple[int] = (500, 502, 503, 504),
+                                session: requests.sessions.Session = None,
+                                ):
+        session = session or requests.Session()
+        retry = Retry(
+            total=retries,
+            read=retries,
+            connect=retries,
+            backoff_factor=backoff_factor,
+            status_forcelist=status_forcelist,
+        )
+        http_adapter = HTTPAdapter(max_retries=retry)
+        session.mount('http://', http_adapter)
+        session.mount('https://', http_adapter)
+        return session
+
+    ###################################################################
+    # Open a HTTP connection and harvest HTML from initial source URL
+    ###################################################################
+    def get_website_html(self) -> requests.models.Response:
+        """
+            Open an HTTP connection and harvest HTML from the initial source URL.
 
-            TypeError: Raised when an operation or function is applied to an object of inappropriate type
+            Returns:
+                requests.models.Response: The response object containing the HTML content of the website.
 
-            bs4.FeatureNotFound: raised by the BeautifulSoup constructor if no parser with the requested features
-            is found
+            This method performs an HTTP GET request to the specified URL, handling various scenarios such as proxy usage,
+            user-agent headers, and response status codes. It logs relevant information about the request and response,
+            including any encountered errors or status codes outside the norm.
         """
-        if self._output_format not in self._valid_output_formats:
-            colorized_text(f'The provided output type --> {self._output_format} <-- is not one of the '
-                           f'acceptable types: dictionary, list or json.', 'red')
-            sys.exit(1)
-        else:
-            valid_word = self._validate_word()
-            if valid_word is False:
-                colorized_text(f'Please verify that the word {self._word} is spelled correctly.', 'magenta')
-            elif valid_word is True:
-                check_cache = self._check_cache()
-                if check_cache[0] is True:
-                    hypernym = cleansing.flatten_multidimensional_list(list(check_cache[1]))
-                    if self._output_format == 'list':
-                        return hypernym
-                    elif self._output_format == 'dictionary':
-                        output_dict = {self._word: hypernym}
-                        return output_dict
-                    elif self._output_format == 'json':
-                        json_object = json.dumps({'hypernyms': {self._word: hypernym}},
-                                                 indent=4, ensure_ascii=False)
-                        return json_object
-
-                elif check_cache[0] is False:
-                    try:
-                        response = ''
-                        if self._proxies is None and self._user_agent is None:
-                                response = Query(
-                                    f'https://www.classicthesaurus.com/{self._word}/broader').get_website_html()
-                        elif self._proxies is None and self._user_agent is not None:
-                                response = Query(f'https://www.classicthesaurus.com/{self._word}/broader',
-                                                 user_agent=self._user_agent).get_website_html()
-                        elif self._proxies is not None and self._user_agent is None:
-                                response = Query(f'https://www.classicthesaurus.com/{self._word}/broader',
-                                                 proxies=self._proxies).get_website_html()
-                        elif self._proxies is not None and self._user_agent is not None:
-                                response = Query(f'https://www.classicthesaurus.com/{self._word}/broader',
-                                                 user_agent=self._user_agent, proxies=self._proxies).get_website_html()
-
-                        if response.status_code == 404:
-                            logger.info(f'Classic Thesaurus had no hypernyms reference for the word {self._word}')
-                            return None
-                        else:
-                            soup = BeautifulSoup(response.text, "lxml")
-                            cloudflare_protection = CloudflareVerification('https://www.classicthesaurus.com',
-                                                                           soup).cloudflare_protected_url()
-                            if cloudflare_protection is False:
-                                hypernym = _get_hypernyms(soup)
-                                if 'no hypernyms found' in hypernym:
-                                    colorized_text(f'No hypernyms were found for the word: {self._word} \n'
-                                                   f'Please verify that the word is spelled correctly.', 'blue')
-                                else:
-                                    number_of_pages = _get_number_of_pages(soup)
-                                    if number_of_pages >= 2:
-                                        for page in range(2, number_of_pages):
-                                            sub_html = ''
-                                            if self._proxies is None and self._user_agent is None:
-                                                    sub_html = Query(
-                                                        f'https://www.classicthesaurus.com/{self._word}/broader/{page}').get_website_html()
-                                            elif self._proxies is None and self._user_agent is not None:
-                                                    sub_html = Query(
-                                                        f'https://www.classicthesaurus.com/{self._word}/broader/{page}',
-                                                        user_agent=self._user_agent).get_website_html()
-                                            elif self._proxies is not None and self._user_agent is None:
-                                                    sub_html = Query(
-                                                        f'https://www.classicthesaurus.com/{self._word}/broader/{page}',
-                                                        proxies=self._proxies).get_website_html()
-                                            elif self._proxies is not None and self._user_agent is not None:
-                                                    sub_html = Query(
-                                                        f'https://www.classicthesaurus.com/{self._word}/broader/{page}',
-                                                        user_agent=self._user_agent,
-                                                        proxies=self._proxies).get_website_html()
-
-                                            sub_soup = BeautifulSoup(sub_html.text, 'lxml')
-                                            additional_hypernym = _get_hypernyms(sub_soup)
-                                            if additional_hypernym:
-                                                hypernym.union(additional_hypernym)
-                                    self._update_cache(sorted(hypernym))
-                                    if self._output_format == 'list':
-                                        return sorted(hypernym)
-                                    elif self._output_format == 'dictionary':
-                                        output_dict = {self._word: sorted(hypernym)}
-                                        return output_dict
-                                    elif self._output_format == 'json':
-                                        json_object = json.dumps({'hypernyms': {self._word: sorted(hypernym)}},
-                                                                 indent=4, ensure_ascii=False)
-                                        return json_object
-                            elif cloudflare_protection is True:
-                                return None
-
-                    except bs4.FeatureNotFound as error:
-                        logger.error('An error occurred in the following code segment:')
-                        logger.error(''.join(traceback.format_tb(error.__traceback__)))
-                    except AttributeError as error:
-                        logger.error('An AttributeError occurred in the following code segment:')
-                        logger.error(''.join(traceback.format_tb(error.__traceback__)))
-                    except IndexError as error:
-                        logger.error('An IndexError occurred in the following code segment:')
-                        logger.error(''.join(traceback.format_tb(error.__traceback__)))
-                    except KeyError as error:
-                        logger.error('A KeyError occurred in the following code segment:')
-                        logger.error(''.join(traceback.format_tb(error.__traceback__)))
-                    except TypeError as error:
-                        logger.error('A TypeError occurred in the following code segment:')
-                        logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        response = ''
+        try:
+            if self._proxies is None and self._user_agent is None:
+                response = self._requests_retry_session().get(self._url_to_scrape,
+                                                              headers=http_headers,
+                                                              allow_redirects=True,
+                                                              verify=True,
+                                                              timeout=(30, 45))
+
+            elif self._proxies is None and self._user_agent is not None:
+                response = self._requests_retry_session().get(self._url_to_scrape,
+                                                              headers={'user-agent': self._user_agent},
+                                                              allow_redirects=True,
+                                                              verify=True,
+                                                              timeout=(30, 45))
+
+            elif self._proxies is not None and self._user_agent is None:
+                response = self._requests_retry_session().get(self._url_to_scrape,
+                                                              headers=http_headers,
+                                                              allow_redirects=True,
+                                                              verify=True,
+                                                              timeout=(30, 45),
+                                                              proxies=self._proxies)
+
+            elif self._proxies is not None and self._user_agent is not None:
+                response = self._requests_retry_session().get(self._url_to_scrape,
+                                                              headers={'user-agent': self._user_agent},
+                                                              allow_redirects=True,
+                                                              verify=True,
+                                                              timeout=(30, 45),
+                                                              proxies=self._proxies)
+
+            cloudflare_protected = bool([value for (key, value) in response.headers.items()
+                                         if key == 'Server'
+                                         and value == 'cloudflare'])
+
+            if response.status_code in {404, 500, 503, 504, 521}:
+                self._handle_http_status_codes(response.status_code)
+            elif response.status_code == 403:
+                if cloudflare_protected is True:
+                    logger.info('-' * 80)
+                    logger.info("The requested URL is protected by Cloudflare's DDoS mitigation service.")
+                    logger.info(f'Requested URL: {self._url_to_scrape}')
+                    logger.info('-' * 80)
+                elif cloudflare_protected is False:
+                    logger.info('-' * 80)
+                    logger.error(f'Response Status Code: {response.status_code}')
+                    logger.info('HTTP 403 is an HTTP status code meaning access to the requested '
+                                'resource is forbidden.')
+                    logger.info(f'Requested URL: {self._url_to_scrape}')
+                    logger.info('-' * 80)
+            else:
+                if response.status_code != 200:
+                    colorized_text(text=f'The Status Code: {response.status_code} has been detected.'
+                                   '\nPlease review the WordHoard logs for additional information.', color='red')
+                    logger.error(f'Response Status Code: {response.status_code}')
+                    logger.info(f'Requested URL: {self._url_to_scrape}')
+                    logger.info('-' * 80)
+
+        except (requests.HTTPError, requests.URLRequired, requests.exceptions.ProxyError, MaxRetryError,
+                requests.ConnectionError, requests.Timeout, requests.RequestException) as error:
+            self._handle_exceptions(error)
+        return response
```

### Comparing `wordhoard-1.5.4/wordhoard/hyponyms.py` & `wordhoard-1.5.5/wordhoard/utilities/mymemory_translator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,351 +1,354 @@
 #!/usr/bin/env python3
 
 """
-This Python script is designed to query an online repository for the
-hyponyms associated with a specific word.
+This Python module is used to translate a specific word from it source language,
+such as Spanish into American English using the MyMemory Translation service.
 """
 __author__ = 'John Bumgarner'
-__date__ = 'June 12, 2021'
+__date__ = 'September 24, 2021'
 __status__ = 'Production'
 __license__ = 'MIT'
 __copyright__ = "Copyright (C) 2021 John Bumgarner"
 
 ##################################################################################
-# Date Initially Completed: June 12, 2021
-# Author: John Bumgarner
-#
-# Date Last Revised: May 31, 2023
-# Revised by: John Bumgarner
-###################################################################################
-
-##################################################################################
 # “AS-IS” Clause
 #
 # Except as represented in this agreement, all work produced by Developer is
 # provided “AS IS”. Other than as provided in this agreement, Developer makes no
 # other warranties, express or implied, and hereby disclaims all implied warranties,
 # including any warranty of merchantability and warranty of fitness for a particular
 # purpose.
 ##################################################################################
 
 ##################################################################################
+# Date Completed: September 24, 2021
+# Author: John Bumgarner
+#
+# Date Last Revised: May 25, 2024
+# Revised by: John Bumgarner
+##################################################################################
+
+##################################################################################
 # Python imports required for basic operations
 ##################################################################################
-import bs4
+# Standard library imports
+import ast
 import sys
-import json
 import logging
 import traceback
-from bs4 import BeautifulSoup
+from string import punctuation
+from typing import Dict, Optional, Tuple, Union
+
+# Third-party imports
+import requests
+from requests.adapters import Retry
+from requests.adapters import HTTPAdapter
 from backoff import on_exception, expo
 from ratelimit import limits, RateLimitException
-from wordhoard.utilities.request_html import Query
-from typing import List, Dict, Optional, Set, Tuple, Union
+
+# Local or project-specific imports
+from wordhoard.utilities.exceptions import RequestException
 from wordhoard.utilities.colorized_text import colorized_text
-from wordhoard.utilities import caching, cleansing, word_verification
-from wordhoard.utilities.cloudflare_checker import CloudflareVerification
+from wordhoard.utilities.translator_languages import Languages
+from wordhoard.utilities.user_agents import get_random_user_agent
+from wordhoard.utilities.exceptions import InvalidLengthException
+from wordhoard.utilities.exceptions import TooManyRequestsException
+from wordhoard.utilities.exceptions import InvalidEmailAddressException
+from wordhoard.utilities.exceptions import LanguageNotSupportedException
+from wordhoard.utilities.email_address_verification import validate_address
 
 logger = logging.getLogger(__name__)
 
-
-def _get_number_of_pages(soup: BeautifulSoup) -> int:
+class Translator:
     """
-    This function determines the number of pages that contain hyponyms for a specific word.
-
-    :param soup: BeautifulSoup lxml
-
-    :return: number of pages
-
-    :rtype: int
-
-    :raises:
-        AttributeError: Raised when an attribute reference or assignment fails
-
-        KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys
-
-        TypeError: Raised when an operation or function is applied to an object of inappropriate type
-
-    """
-    try:
-        number_of_pages = 0
-        pages = soup.find('div', {'id': 'pages'})
-        if pages is not None:
-            list_of_pages = [num for page in pages for num in page if num.isdigit()]
-            if len(list_of_pages) != 0:
-                number_of_pages = int(list_of_pages[-1]) + 1
-        return number_of_pages
-
-    except AttributeError as error:
-        logger.error('An AttributeError occurred in the following code segment:')
-        logger.error(''.join(traceback.format_tb(error.__traceback__)))
-    except KeyError as error:
-        logger.error('A KeyError occurred in the following code segment:')
-        logger.error(''.join(traceback.format_tb(error.__traceback__)))
-    except TypeError as error:
-        logger.error('A TypeError occurred in the following code segment:')
-        logger.error(''.join(traceback.format_tb(error.__traceback__)))
-
-
-def _get_hyponyms(soup: BeautifulSoup) -> Set[str]:
-    """
-    This function queries an HTML table for hyponyms.
-
-    :param soup: BeautifulSoup lxml
-
-    :return:
-        hyponyms: set of hyponyms
-
-    :rtype: set
+        This class provides translation capabilities using the MyMemory Translation service.
+        It supports translating words from one language to another and handling various exceptions
+        that may occur during translation requests.
+
+        Args:
+            source_language (str): The source language for translation. Defaults to an empty string.
+            str_to_translate (str): The text to translate. Defaults to an empty string.
+            email_address (str): The email address for authentication. Defaults to an empty string.
+            proxies (Optional[Dict[str, str]]): Dictionary of proxy servers. Defaults to None.
+
+        Attributes:
+            _source_language (str): The source language for translation.
+            _str_to_translate (str): The text to translate.
+            _url_to_query (str): The API endpoint for translation requests.
+            _email_address (str): The email address for authentication.
+            _proxies (Optional[Dict[str, str]]): Dictionary of proxy servers.
+            _headers (Dict[str, str]): HTTP headers for requests.
+            _rate_limit_status (bool): A flag indicating the rate limit status for translation requests.
+
+        Methods:
+            __init__: Initializes the Translator object with source language, text to translate, email address, and proxies.
+            _backoff_handler: Handles rate limit exceeded situations by logging and setting rate_limit_status.
+            _mymemory_supported_languages: Checks if the source language is supported by MyMemory Translation service.
+            _requests_retry_session: Configures a retry session for handling HTTP request retries.
+            _handle_custom_exceptions: Handles custom exceptions specific to MyMemory Translation service.
+            _mymemory_translate: Translates text from the source language to English using MyMemory Translation service.
+            _mymemory_translate_reverse: Translates text from English to the source language using MyMemory Translation service.
+            translate_word: Translates text from the source language to English, handling unsupported languages.
+            reverse_translate: Translates text from English to the source language.
+
+        Note:
+            This class requires the 'requests', 'backoff', and 'ratelimit' modules for handling HTTP requests
+            and rate limiting. Ensure these modules are installed and configured correctly for translation operations.
+        """
+    def __init__(self,
+                 source_language: str = '',
+                 str_to_translate: str = '',
+                 email_address: str = '',
+                 max_number_of_requests: int = 30,
+                 rate_limit_timeout_period: int = 60,
+                 proxies: Optional[Dict[str, str]] = None
+                 ):
 
-    :raises:
-        AttributeError: Raised when an attribute reference or assignment fails.
+        self._source_language = source_language
+        self._str_to_translate = str_to_translate
+        self._url_to_query = 'http://api.mymemory.translated.net/get'
+        self._email_address = email_address
+        self._proxies = proxies
 
-        KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys.
+        rand_user_agent = get_random_user_agent()
+        http_headers = {'user-agent': rand_user_agent}
+        self._headers = http_headers
 
-        TypeError: Raised when an operation or function is applied to an object of inappropriate type.
-    """
-    try:
-        sub_set = set()
-        table = soup.find('table')
-        if table:
-            rows = table.find_all('tr', {'class': 'theentry'})
-            if rows is not None:
-                for row in rows:
-                    cols = row.find('td', {'class': 'abbdef'}).find('a')
-                    if cols is not None:
-                        if cols.text != '»':
-                            sub_set.add(str(cols.text).lower())
-                        else:
-                            sub_set.add('no hyponyms found')
-        return sub_set
-
-    except AttributeError as error:
-        logger.error('An AttributeError occurred in the following code segment:')
-        logger.error(''.join(traceback.format_tb(error.__traceback__)))
-    except KeyError as error:
-        logger.error('A KeyError occurred in the following code segment:')
-        logger.error(''.join(traceback.format_tb(error.__traceback__)))
-    except TypeError as error:
-        logger.error('A TypeError occurred in the following code segment:')
-        logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        ratelimit_status = False
+        self._rate_limit_status = ratelimit_status
 
+        # Retries the requests after a certain time period has elapsed
+        handler = on_exception(wait_gen=expo,
+                               exception=RateLimitException,
+                               max_time=60,
+                               on_backoff=self._backoff_handler)
+        # Establishes a rate limit for making requests to the MyMemory translation service
+        limiter = limits(calls=max_number_of_requests, period=rate_limit_timeout_period)
+        self.translate_word = handler(limiter(self.translate_word))
+        self.reverse_translate = handler(limiter(self.reverse_translate))
 
-class Hyponyms(object):
+    def _backoff_handler(self, details) -> None:
+        """
+        Handles the backoff mechanism when the rate limit for querying the MyMemory translation service is reached.
 
-    def __init__(self,
-                 search_string: str = '',
-                 output_format: str = 'list',
-                 max_number_of_requests: int = 30,
-                 rate_limit_timeout_period: int = 60,
-                 user_agent: Optional[str] = None,
-                 proxies: Optional[Dict[str, str]] = None):
+        This method is triggered when the rate limit is encountered. It logs the rate limit event and displays
+        colorized messages indicating that the process is entering a temporary hibernation mode. If the rate
+        limit has already been reached, it continues to display colorized backoff messages for subsequent
+        retries.
+
+        :param details: A dictionary containing information about the backoff event, including:
+                        - 'wait' (float): The number of seconds to wait before retrying.
+                        - 'tries' (int): The number of retry attempts made so far.
+                        - Additional details such as 'target', 'args', 'kwargs', 'elapsed', and 'exception' which provide
+                          context about the event (not used in this method but part of the details dictionary).
+
+        type details: Dict
+
+        Side Effects:
+        - Displays colorized text messages to indicate the backoff status.
+        - Logs an info message when the rate limit is initially reached.
+        - Sets the `_rate_limit_status` attribute to True when the rate limit is first encountered.
 
+        :returns: None
+        :rtype: NoneType
         """
-        Purpose
-        ----------
-        This Python class is used to query online repositories for the hyponyms associated with a specific word.
+        if self._rate_limit_status is False:
+            colorized_text(text='The MyMemory translation service query rate limit was reached. '
+                                'The querying process is entering a temporary hibernation mode.', color='red')
+            colorized_text(text=f"Backing off {details['wait']:.1f} seconds afters {details['tries']} tries.",
+                           color='blue')
+            logger.info('The MyMemory translation service query rate limit was reached.')
+            self._rate_limit_status = True
+        elif self._rate_limit_status is True:
+            colorized_text(text=f"Backing off {details['wait']:.1f} seconds afters {details['tries']} tries.",
+                           color='blue')
 
-        Usage Examples
-        ----------
+    def _mymemory_supported_languages(self) -> Union[str, None]:
+        """
+        This function determines if the requested source language is
+        one supported languages for the MyMemory Translator.
 
-        >>> hyponyms = Hyponyms('horse')
-        >>> results = hyponyms.find_hyponyms()
+        :return: language
+        :rtype: string
+        """
+        languages = Languages()
+        mymemory_languages = languages.mymemory_supported_languages()
+        mymemory_languages_str = str(mymemory_languages)
+        supported_languages = ast.literal_eval(mymemory_languages_str)
+        try:
+            if self._source_language in supported_languages.keys():
+                return self._source_language
+            elif self._source_language in supported_languages.values():
+                return self._source_language
+            else:
+                return None
+        except LanguageNotSupportedException as error:
+            logger.info('The language provided is not one of the supported languages of the MyMemory Translation service.')
+            logger.info(f'Requested language: {self._source_language}')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+
+    # reference: https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#module-urllib3.util.retry
+    @staticmethod
+    def _requests_retry_session(retries: int = 5,
+                                backoff_factor: float = 0.5,
+                                status_forcelist: Tuple[int] = (500, 502, 503, 504),
+                                session: requests.sessions.Session = None,
+                                ):
+        session = session or requests.Session()
+        retry = Retry(
+            total=retries,
+            read=retries,
+            connect=retries,
+            backoff_factor=backoff_factor,
+            status_forcelist=status_forcelist,
+        )
+        http_adapter = HTTPAdapter(max_retries=retry)
+        session.mount(prefix='http://', adapter=http_adapter)
+        session.mount(prefix='https://', adapter=http_adapter)
+        return session
 
-        >>> hyponyms = Hyponyms(search_string='horse')
-        >>> results = hyponyms.find_hyponyms()
+    def _handle_custom_exceptions(self, error):
+        """
+        Helper method to handle custom exceptions
+        """
+        if isinstance(error, InvalidEmailAddressException):
+            colorized_text(text='The email address provided for authentication to the MyMemory Translation service '
+                                'is invalid.', color='red')
+            logger.error('Invalid Email Address Error:')
+            logger.error('The email address provided for authentication to the MyMemory Translation service '
+                         'is invalid.')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        elif isinstance(error, InvalidLengthException):
+            colorized_text(text=f'The text length for the word: "{self._str_to_translate}" exceed the length limit '
+                                f'of MyMemory translation service.', color='red')
+            logger.error(f'The text length for the word: "{self._str_to_translate}" exceed the length limit of '
+                         f'MyMemory Translation service.')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        elif isinstance(error, RequestException):
+            colorized_text(text='An ambiguous connection exception has occurred when contacting the MyMemory Translation '
+                     'service. Please check the WordHoard log file for additional information.', color='red')
+            logger.error('Connection Exception:')
+            logger.error('An ambiguous connection exception has occurred when communicating with the '
+                         'MyMemory Translation service.')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        elif isinstance(error, TooManyRequestsException):
+            colorized_text(text='There has been too many connection requests to the MyMemory Translation service.',
+                           color='red')
+            logger.error('Connection Request Error:')
+            logger.error('There has been too many connection requests to the MyMemory Translation service.')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
-        Parameters
-        ----------
-        :param search_string: string variable used to find hyponyms for
+    def _mymemory_translate(self, original_language: str) -> Union[str, None]:
+        """
+        This function is used to translate a word from it source language, such as Spanish into American English.
 
-        :param max_number_of_requests: maximum number of requests for a specific timeout_period
+        :param original_language: language to translated from
+        :return: translated word
+        :rtype: string or None
+        """
+        try:
+            if not validate_address(email_address=self._email_address):
+                colorized_text(text='A valid email address is required to use the MyMemory Translation service.',
+                               color='red')
+                sys.exit(1)
+
+            response = self._requests_retry_session().get(self._url_to_query,
+                                                          params={'langpair': f'{original_language}|en-us',
+                                                                  'q': self._str_to_translate,
+                                                                  'de': self._email_address},
+                                                          headers=self._headers,
+                                                          proxies=self._proxies)
+
+            if response.status_code == 429:
+                # HTTP 429 -- Too Many Requests response status code indicates the user has
+                # sent too many requests in a given amount of time ("rate limiting")
+                raise TooManyRequestsException()
+            if response.status_code not in (200, 429):
+                raise RequestException()
+
+            data = response.json()
+            if not data:
+                colorized_text(text=f'MyMemory could not translate the word "{self._str_to_translate}".',
+                               color='magenta')
+                return None
+
+            translation = data.get('responseData').get('translatedText')
+            if translation != 'INVALID EMAIL PROVIDED':
+                return str(translation).lower().rstrip(punctuation)
+            elif translation == 'INVALID EMAIL PROVIDED':
+                raise InvalidEmailAddressException()
 
-        :param rate_limit_timeout_period: the time period before a session is placed in a temporary hibernation mode
+        except (InvalidEmailAddressException, InvalidLengthException, TooManyRequestsException, RequestException) as error:
+            self._handle_custom_exceptions(error)
 
-        :param user_agent: string containing either a global user agent type or a specific user agent
+    def _mymemory_translate_reverse(self) -> Union[str, None]:
+        """
+        This function is used to translate a word from it source language, such as Spanish into American English.
 
-        :param proxies: dictionary of proxies to use with Python Requests
+        :return: translated word
+        :rtype: string or None
         """
+        try:
+            if not validate_address(email_address=self._email_address):
+                colorized_text(text='A valid email address is required to use the MyMemory Translation service.',
+                               color='red')
+                sys.exit(1)
+
+            response = self._requests_retry_session().get(url=self._url_to_query,
+                                                          params={'langpair': f'en-us|{self._source_language}',
+                                                                  'q': self._str_to_translate,
+                                                                  'de': self._email_address},
+                                                          headers=self._headers,
+                                                          proxies=self._proxies
+                                                          )
+
+            if response.status_code == 429:
+                # HTTP 429 -- Too Many Requests response status code indicates the user has
+                # sent too many requests in a given amount of time ("rate limiting")
+                raise TooManyRequestsException()
+            if response.status_code not in (200, 429):
+                raise RequestException()
+
+            data = response.json()
+            if not data:
+                colorized_text(text=f'MyMemory could not translate the word "{self._str_to_translate}".',
+                               color='magenta')
+                return None
+
+            translation = data.get('responseData').get('translatedText')
+            if translation != 'INVALID EMAIL PROVIDED':
+                return str(translation).lower().rstrip(punctuation)
+            elif translation == 'INVALID EMAIL PROVIDED':
+                raise InvalidEmailAddressException()
 
-        self._proxies = proxies
-        self._word = search_string
-        self._user_agent = user_agent
-        self._output_format = output_format
-        self._valid_output_formats = {'dictionary', 'list', 'json'}
+        except (InvalidEmailAddressException, InvalidLengthException, TooManyRequestsException, RequestException) as error:
+            self._handle_custom_exceptions(error)
 
-        rate_limit_status = False
-        self._rate_limit_status = rate_limit_status
+    def translate_word(self) -> Union[str, None]:
+        """
+        This function is used to translate a word from it source language, such as Spanish into American English.
 
-        # Retries the requests after a certain time period has elapsed
-        handler = on_exception(expo, RateLimitException, max_time=60, on_backoff=self._backoff_handler)
-        # Establishes a rate limit for making requests to the hyponyms repositories
-        limiter = limits(calls=max_number_of_requests, period=rate_limit_timeout_period)
-        self.find_hyponyms = handler(limiter(self.find_hyponyms))
+        :return: translated word
+        :rtype: string
+        """
+        supported_language = self._mymemory_supported_languages()
+        if supported_language:
+            return self._mymemory_translate(supported_language)
+        elif not supported_language:
+            colorized_text(text='The language provided is not one of the supported languages for the MyMemory '
+                           'Translation service.', color='red')
+            colorized_text(text=f'Requested language: {self._source_language}', color='red')
+            colorized_text(text='Please review the languages supported by the MyMemory Translate service\n'
+                           'https://wordhoard.readthedocs.io/en/latest/translations'
+                           '/mymemory_supported_translation_languages/', color='green')
 
-    def _backoff_handler(self):
-        if self._rate_limit_status is False:
-            colorized_text('The hyponyms query rate limit was reached. The querying process is entering '
-                           'a temporary hibernation mode.', 'red')
-            logger.info('The hyponyms query rate limit was reached.')
-            self._rate_limit_status = True
+            return None
 
-    def _validate_word(self) -> bool:
+    def reverse_translate(self) -> Union[str, None]:
         """
-        This function is designed to validate that the syntax for a string variable is in an acceptable format.
+        This function is used to translate a word from American English into another language, such as Spanish.
 
-        :return: True or False
-        :rtype: bool
+        :return: translated word
+        :rtype: string or None
         """
-        valid_word = word_verification.validate_word_syntax(self._word)
-        if valid_word:
-            return True
-        else:
-            logger.error(f'The word {self._word} was not in a valid format.')
-            logger.error(f'Please verify that the word {self._word} is spelled correctly.')
-            return False
-
-    def _check_cache(self) -> Tuple[bool, Union[List[str], None]]:
-        check_cache = caching.cache_hyponyms(self._word)
-        return check_cache
-
-    def _update_cache(self, hyponyms: List[str]) -> None:
-        caching.insert_word_cache_hyponyms(self._word, hyponyms)
-        return
-
-    def find_hyponyms(self) -> Union[List[str], Dict[str, List[str]], str, None]:
-        """
-        Purpose
-        ----------
-        This function queries classicthesaurus_com for hyponyms associated
-        with the specific word provided to the Class Hyponyms.
-
-        Returns
-        ----------
-         :returns:
-             hyponyms: list of hyponyms
-
-        :rtype: list
-
-        Raises
-        ----------
-        :raises:
-            AttributeError: Raised when an attribute reference or assignment fails
-
-            IndexError: Raised when a sequence subscript is out of range
-
-            KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys
-
-            TypeError: Raised when an operation or function is applied to an object of inappropriate type
-
-            bs4.FeatureNotFound: raised by the BeautifulSoup constructor if no parser with the requested features
-            is found
-        """
-        if self._output_format not in self._valid_output_formats:
-            colorized_text(f'The provided output type --> {self._output_format} <-- is not one of the '
-                           f'acceptable types: dictionary, list or json.', 'red')
-            sys.exit(1)
-        else:
-            valid_word = self._validate_word()
-            if valid_word is False:
-                colorized_text(f'Please verify that the word {self._word} is spelled correctly.', 'magenta')
-            elif valid_word is True:
-                check_cache = self._check_cache()
-                if check_cache[0] is True:
-                    hyponym = cleansing.flatten_multidimensional_list(check_cache[1])
-                    if self._output_format == 'list':
-                        return [word.lower() for word in hyponym]
-                    elif self._output_format == 'dictionary':
-                        output_dict = {self._word: [word.lower() for word in hyponym]}
-                        return output_dict
-                    elif self._output_format == 'json':
-                        json_object = json.dumps({'hyponyms': {self._word: [word.lower() for word in hyponym]}},
-                                                 indent=4, ensure_ascii=False)
-                        return json_object
-
-                elif check_cache[0] is False:
-                    try:
-                        response = ''
-                        if self._proxies is None and self._user_agent is None:
-                            response = Query(
-                                f'https://www.classicthesaurus.com/{self._word}/narrower').get_website_html()
-                        elif self._proxies is None and self._user_agent is not None:
-                            response = Query(
-                                f'https://www.classicthesaurus.com/{self._word}/narrower',
-                                user_agent=self._user_agent).get_website_html()
-                        elif self._proxies is not None and self._user_agent is None:
-                            response = Query(f'https://www.classicthesaurus.com/{self._word}/narrower',
-                                             proxies=self._proxies).get_website_html()
-                        elif self._proxies is not None and self._user_agent is not None:
-                            response = Query(f'https://www.classicthesaurus.com/{self._word}/narrower',
-                                             user_agent=self._user_agent,
-                                             proxies=self._proxies).get_website_html()
-
-                        if response.status_code == 404:
-                            logger.info(f'Classic Thesaurus had no hyponyms reference for the word {self._word}')
-                            return None
-                        else:
-                            soup = BeautifulSoup(response.text, "lxml")
-                            cloudflare_protection = CloudflareVerification('https://www.classicthesaurus.com',
-                                                                           soup).cloudflare_protected_url()
-                            if cloudflare_protection is False:
-                                hyponym = _get_hyponyms(soup)
-                                if 'no hyponyms found' in hyponym:
-                                    colorized_text(f'No hyponyms were found for the word: {self._word} \n'
-                                                   f'Please verify that the word is spelled correctly.', 'blue')
-                                    return None
-                                else:
-                                    number_of_pages = _get_number_of_pages(soup)
-                                    if number_of_pages >= 2:
-                                        for page in range(2, number_of_pages):
-                                            sub_html = ''
-                                            if self._proxies is None and self._user_agent is None:
-                                                sub_html = Query(
-                                                    f'https://www.classicthesaurus.com/{self._word}/narrower/'
-                                                    f'{page}').get_website_html()
-                                            elif self._proxies is None and self._user_agent is not None:
-                                                sub_html = Query(
-                                                    f'https://www.classicthesaurus.com/{self._word}/narrower/'
-                                                    f'{page}', user_agent=self._user_agent).get_website_html()
-                                            elif self._proxies is not None and self._user_agent is None:
-                                                sub_html = Query(
-                                                    f'https://www.classicthesaurus.com/{self._word}/narrower/'
-                                                    f'{page}', proxies=self._proxies).get_website_html()
-                                            elif self._proxies is not None and self._user_agent is not None:
-                                                sub_html = Query(
-                                                    f'https://www.classicthesaurus.com/{self._word}/narrower/'
-                                                    f'{page}', proxies=self._proxies,
-                                                    user_agent=self._user_agent).get_website_html()
-
-                                            sub_soup = BeautifulSoup(sub_html.text, 'lxml')
-                                            additional_hyponym = _get_hyponyms(sub_soup)
-                                            hyponym.union(additional_hyponym)
-                                    self._update_cache(sorted(hyponym))
-                                    if self._output_format == 'list':
-                                        return [word.lower() for word in hyponym]
-                                    elif self._output_format == 'dictionary':
-                                        output_dict = {
-                                            self._word: [word.lower() for word in hyponym]}
-                                        return output_dict
-                                    elif self._output_format == 'json':
-                                        json_object = json.dumps({'hyponyms': {self._word: [word.lower() for word in
-                                                                                            hyponym]}},
-                                                                 indent=4, ensure_ascii=False)
-                                        return json_object
-                            elif cloudflare_protection is True:
-                                return None
-
-                    except bs4.FeatureNotFound as error:
-                        logger.error('An error occurred in the following code segment:')
-                        logger.error(''.join(traceback.format_tb(error.__traceback__)))
-                    except AttributeError as error:
-                        logger.error('An AttributeError occurred in the following code segment:')
-                        logger.error(''.join(traceback.format_tb(error.__traceback__)))
-                    except IndexError as error:
-                        logger.error('An IndexError occurred in the following code segment:')
-                        logger.error(''.join(traceback.format_tb(error.__traceback__)))
-                    except KeyError as error:
-                        logger.error('A KeyError occurred in the following code segment:')
-                        logger.error(''.join(traceback.format_tb(error.__traceback__)))
-                    except TypeError as error:
-                        logger.error('A TypeError occurred in the following code segment:')
-                        logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        return self._mymemory_translate_reverse()
```

### Comparing `wordhoard-1.5.4/wordhoard/synonyms.py` & `wordhoard-1.5.5/wordhoard/antonyms.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python3
 
 """
-This Python script is designed to query multiple online repositories for the
-synonyms associated with the given word.
+This Python module is designed to query multiple online repositories for the
+antonyms associated with a specific word.
 """
 __author__ = 'John Bumgarner'
 __date__ = 'October 15, 2020'
 __status__ = 'Production'
 __license__ = 'MIT'
 __copyright__ = "Copyright (C) 2020 John Bumgarner"
 
 ##################################################################################
 # Date Completed: October 15, 2020
 # Author: John Bumgarner
 #
-# Date Last Revised: May 31, 2023
+# Date Last Revised: May 25, 2024
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # “AS-IS” Clause
 #
 # Except as represented in this agreement, all work produced by Developer is
@@ -27,632 +27,611 @@
 # including any warranty of merchantability and warranty of fitness for a particular
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
-import bs4
+# Standard library imports
 import sys
 import json
 import logging
-import requests
 import traceback
 import re as regex
+from collections.abc import Sized
+from concurrent.futures.thread import BrokenThreadPool
+from concurrent.futures import ThreadPoolExecutor, as_completed, BrokenExecutor
+from typing import Dict, List, Optional, Set, Tuple, Union
+
+# Third-party imports
+import bs4
+import requests
 from bs4 import BeautifulSoup
 from backoff import on_exception, expo
 from ratelimit import limits, RateLimitException
+
+# Local or project-specific imports
 from wordhoard.utilities.request_html import Query
-from wordhoard.utilities.cloudflare_bypass import Cloudflare
 from wordhoard.utilities.colorized_text import colorized_text
-from concurrent.futures import ThreadPoolExecutor, as_completed
-from typing import Dict, List, Optional, Set, Sized, Tuple, Union
 from wordhoard.utilities import caching, cleansing, word_verification
 from wordhoard.utilities.cloudflare_checker import CloudflareVerification
 
-
 logger = logging.getLogger(__name__)
 
-class Synonyms(object):
+class PartOfSpeech:
+    """
+        This utility class contains static methods to extract part of speech categories
+        from HTML responses of various sources, which are Thesaurus.com, and WordHippo.
 
-    def __init__(self,
-                 search_string: str = '',
-                 output_format: str = 'list',
-                 max_number_of_requests: int = 30,
-                 rate_limit_timeout_period: int = 60,
-                 user_agent: Optional[str] = None,
-                 proxies: Optional[Dict[str, str]] = None):
+        Static Methods
+        --------------
+        _handle_query_exceptions(error):
+            Helper method to handle common exceptions in query methods.
+
+        part_of_speech_category_thesaurus_com(soup: BeautifulSoup) -> str:
+            Extracts the part of speech category from the HTML response of Thesaurus.com.
+
+        part_of_speech_category_wordhippo(soup: BeautifulSoup) -> str:
+            Extracts the part of speech category from the HTML response of WordHippo.
         """
-        This Python class is used to query multiple online repositories for the synonyms
-        associated with a specific word.
 
-        Usage Examples
-        ----------
+    @staticmethod
+    def _handle_query_exceptions(error):
+        """
+        Helper method to handle common exceptions in query methods.
+        """
+        logger.error('An error occurred in the following code segment:')
+        logger.error(''.join(traceback.format_tb(error.__traceback__)))
+
+    @staticmethod
+    def part_of_speech_category_thesaurus_com(soup: BeautifulSoup) -> str:
+        """
+        Extracts the part of speech category from the HTML response of Thesaurus.com.
+
+        :param soup: BeautifulSoup object containing the HTML response
+        :param type soup: bs4.BeautifulSoup
+        :return: Part of speech category
+        :rtype: str
+        """
+        part_of_speech_category: str = ''
+        try:
+            start_pattern = r'window\.__staticRouterHydrationData\s*=\s*JSON\.parse\('
+            end_pattern = r'\);'
+            script_tag = soup.find(name='script', text=regex.compile(start_pattern))
+            if script_tag:
+                match = regex.search(pattern=f'{start_pattern}(.*?){end_pattern}', string=script_tag.string)
+                if match:
+                    json_data_str = match.group(1).strip('"\'')
+                    json_data_str = json_data_str.replace('\\"', '"')
+                    pos_pattern = r'"partOfSpeech":"([^"]*)","shortDefinitions"'
+                    pos_match = regex.search(pattern=pos_pattern, string=json_data_str)
+                    if pos_match:
+                        part_of_speech_category = pos_match.group(1).strip()
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            PartOfSpeech._handle_query_exceptions(error)
+        return part_of_speech_category
+
+    @staticmethod
+    def part_of_speech_category_wordhippo(soup: BeautifulSoup) -> str:
+        """
+        Extracts the part of speech category from the HTML response of WordHippo.
+
+        :param soup: BeautifulSoup object containing the HTML response
+        :param type soup: bs4.BeautifulSoup
+        :return: Part of speech category
+        :rtype: str
+        """
+        part_of_speech_category: str = ''
+        try:
+            if soup.find(name="div", attrs={'class': 'wordtype'}):
+                part_of_speech_tag = soup.find(name="div", attrs={'class': 'wordtype'})
+                if len(part_of_speech_tag.text) != 0:
+                    part_of_speech_category = ''.join(filter(lambda x: x.isalpha(), part_of_speech_tag.text)).lower()
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            PartOfSpeech._handle_query_exceptions(error)
+        return part_of_speech_category
 
-        >>> synonym = Synonyms('mother')
-        >>> results = synonym.find_synonyms()
+class ParseWords:
+    """
+        A utility class for parsing antonyms from various online sources.
 
-        >>> synonym = Synonyms(search_string='mother')
-        >>> results = synonym.find_synonyms()
+        This class contains static methods to parse antonyms from HTML responses of various sources,
+        which are Thesaurus.com and WordHippo.
 
-        Parameters
-        ----------
-        :param search_string: string containing the variable to obtain synonyms for
+        Methods
+        -------
+        _handle_query_exceptions(error):
+            Helper method to handle common exceptions in query methods.
 
-        :param output_format: Format to use for returned results.
-               Default value: list; Acceptable values: dictionary or list
+        parse_thesaurus_com(soup: BeautifulSoup) -> list:
+            Parses antonyms from the HTML response of Thesaurus.com.
 
-        :param max_number_of_requests: maximum number of requests for a specific timeout_period
+        parse_wordhippo(soup: BeautifulSoup) -> list:
+            Parses antonyms from the HTML response of WordHippo.
+        """
+
+    @staticmethod
+    def _handle_query_exceptions(error):
+        """
+        Helper method to handle common exceptions in query methods.
+        """
+        logger.error('An error occurred in the following code segment:')
+        logger.error(''.join(traceback.format_tb(error.__traceback__)))
+
+    @staticmethod
+    def parse_google_com(soup: BeautifulSoup, word: str) -> list:
+        """
+        Parses synonyms from the HTML response of Thesaurus.com.
+
+        :param soup: BeautifulSoup object containing the HTML response
+        :param type soup: bs4.BeautifulSoup
+        :param word: word to search
+        :param type word: string
+        :return: List of synonyms extracted from the HTML response
+        :rtype: list
+        """
+        antonyms_list: list = []
+        try:
+            div_element = soup.find(name='div', string=f'What is the opposite of {word}?')
+            if div_element:
+                next_div = div_element.find_next_sibling(name='div')
+                table_tag = next_div.find(name='table')
+                if table_tag:
+                    td_elements = table_tag.find_all(name='td')
+                    for td_element in td_elements:
+                        antonyms_list.append(td_element.text)
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            ParseWords._handle_query_exceptions(error)
+        return antonyms_list
+
+    @staticmethod
+    def parse_thesaurus_com(soup: BeautifulSoup) -> list:
+        """
+        Parses synonyms from the HTML response of Thesaurus.com.
+
+        :param soup: BeautifulSoup object containing the HTML response
+        :param type soup: bs4.BeautifulSoup
+        :return: List of synonyms extracted from the HTML response
+        :rtype: list
+        """
+        antonyms_list: list = []
+        try:
+            start_pattern = r'window\.__staticRouterHydrationData\s*=\s*JSON\.parse\('
+            end_pattern = r'\);'
+            script_tag = soup.find(name='script', string=regex.compile(start_pattern))
+            if script_tag:
+                match = regex.search(pattern=f'{start_pattern}(.*?){end_pattern}', string=script_tag.string)
+                if match:
+                    json_data_str = match.group(1).strip('"\'')
+                    json_data_str = json_data_str.replace('\\"', '"')
+                    antonym_section = regex.search(pattern=r'\[{"antonyms":.*?}\]', string=json_data_str)
+                    if antonym_section:
+                        antonyms_similarity_section = regex.search(pattern=r'\{"similarity":-10,[^}]*\}\]',
+                                                                   string=antonym_section.group(0))
+                        if antonyms_similarity_section:
+                            target_pattern = r'"targetWord"\s*:\s*"([^"]+)"'
+                            target_antonym = regex.search(pattern=target_pattern,
+                                                          string=antonyms_similarity_section.group(0))
+                            if target_antonym:
+                                antonyms_list.append(target_antonym.group(1))
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            ParseWords._handle_query_exceptions(error)
+        return antonyms_list
+
+    @staticmethod
+    def parse_wordhippo(soup: BeautifulSoup) -> list:
+        """
+        Parses synonyms from the HTML response of Wordhippo.
+
+        :param soup: BeautifulSoup object containing the HTML response
+        :param type soup: bs4.BeautifulSoup
+        :return: List of antonyms extracted from the HTML response
+        :rtype: list
+        """
+        antonyms_list: list = []
+        try:
+            related_tag = soup.find(name="div", attrs={'class': 'relatedwords'})
+            if related_tag.find(name="div", attrs={'class': 'wb'}) is not None:
+                for list_item in related_tag.find_all(name="div", attrs={'class': 'wb'}):
+                    for link in list_item.find_all(name='a', href=True):
+                        antonyms_list.append(link.text)
+            else:
+                for table_row in related_tag.find_all(name='td'):
+                    for href_link in table_row.find(name='a', href=True):
+                        antonyms_list.append(href_link.text)
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            ParseWords._handle_query_exceptions(error)
+        return sorted([x.lower() for x in antonyms_list])
+
+class Antonyms:
+    """
+        A Python class for querying multiple online repositories to find antonyms for a specific word.
 
-        :param rate_limit_timeout_period: the time period before a session is placed in a temporary hibernation mode
+        Usage Examples
+        ----------
+        >>> antonym = Antonyms('mother')
+        >>> results = antonym.find_antonyms()
 
-        :param user_agent: string containing either a global user agent type or a specific user agent
+        Parameters
+        ----------
+        search_string : str, optional
+            The word for which antonyms are to be found.
+        sources: Optional[List[str]]
+            The sources to search for antonyms.
+        output_format : str, optional
+            Format for returned results. Default is 'list'. Acceptable values are 'dictionary', 'list', or 'json'.
+        max_number_of_requests : int, optional
+            Maximum number of requests within a specified time period.
+        rate_limit_timeout_period : int, optional
+            Time period before temporary hibernation due to rate limiting.
+        user_agent : str, optional
+            User agent string for HTTP requests.
+        proxies : dict, optional
+            Dictionary of proxies for Python Requests.
 
-        :param proxies: dictionary of proxies to use with Python Requests
+        Attributes
+        ----------
+        _proxies : Optional[Dict[str, str]]
+            Proxies to use with Python Requests.
+        _word : str
+            The word to find antonyms for.
+         _sources : Optional[List[str]]
+            The sources to search for antonyms.
+        _user_agent : Optional[str]
+            User agent for HTTP requests.
+        _output_format : str
+            Format for returned results.
+        _valid_output_formats : Set[str]
+            Set of valid output formats.
+        _rate_limit_status : bool
+            Status indicating whether rate limit is reached.
+
+        Methods
+        -------
+        find_antonyms() -> Union[List[Sized], Dict[str, List[str]], str]:
+            Finds antonyms for the specified word.
+        _validate_word() -> bool:
+            Validates the syntax of the word.
+        _check_cache() -> Tuple[bool, Union[Dict[str, List[str]], None]]:
+            Checks if antonyms are cached.
+        _update_cache(pos_category: str, antonyms: Union[List[str], Set[str]]) -> None:
+            Updates the cache with new antonyms.
+        _request_http_response(url: str) -> requests.models.Response:
+            Makes an HTTP request and returns the response.
+        _run_query_tasks_in_parallel() -> List[tuple[List[str], str]]:
+            Runs query tasks in parallel using a ThreadPool.
+        _query_output(self, antonyms: list, part_of_speech: Union[set[str], str]) -> Union[list, dict, str]:
+            Process the output format based on the specified format.
+        _handle_query_exceptions(error):
+            Handles common exceptions in query methods.
+        _query_google_com() -> Union[Tuple[List[str], str], None]:
+            Queries google.com for antonyms.
+        _query_thesaurus_com() -> Union[Tuple[List[str], str], None]:
+            Queries thesaurus.com for antonyms.
+        _query_wordhippo() -> Union[Tuple[List[str], str], None]:
+            Queries wordhippo for antonyms.
         """
+
+    def __init__(self,
+                 search_string: str = '',
+                 sources: Optional[List[str]] = None,
+                 output_format: str = 'list',
+                 max_number_of_requests: int = 30,
+                 rate_limit_timeout_period: int = 60,
+                 user_agent: Optional[str] = None,
+                 proxies: Optional[Dict[str, str]] = None):
+
         self._proxies = proxies
         self._word = search_string
         self._user_agent = user_agent
         self._output_format = output_format
         self._valid_output_formats = {'dictionary', 'list', 'json'}
+        self._sources = sources
 
         rate_limit_status = False
         self._rate_limit_status = rate_limit_status
 
         # Retries the requests after a certain time period has elapsed
-        handler = on_exception(expo, RateLimitException, max_time=60, on_backoff=self._backoff_handler)
-        # Establishes a rate limit for making requests to the synonyms repositories
+        handler = on_exception(wait_gen=expo,
+                               exception=RateLimitException,
+                               max_time=60,
+                               on_backoff=self._backoff_handler)
+        # Establishes a rate limit for making requests to the antonyms repositories
         limiter = limits(calls=max_number_of_requests, period=rate_limit_timeout_period)
-        self.find_synonyms = handler(limiter(self.find_synonyms))
+        self._run_query_tasks_in_parallel = handler(limiter(self._run_query_tasks_in_parallel))
+
+    def _backoff_handler(self, details) -> None:
+        """
+        Handles the backoff mechanism when the rate limit for querying antonyms is reached.
 
-    def _backoff_handler(self):
+        This method is triggered when the rate limit is encountered. It logs the rate limit event and displays
+        colorized messages indicating that the process is entering a temporary hibernation mode. If the rate
+        limit has already been reached, it continues to display colorized backoff messages for subsequent
+        retries.
+
+        :param details: A dictionary containing information about the backoff event, including:
+                        - 'wait' (float): The number of seconds to wait before retrying.
+                        - 'tries' (int): The number of retry attempts made so far.
+                        - Additional details such as 'target', 'args', 'kwargs', 'elapsed', and 'exception' which provide
+                          context about the event (not used in this method but part of the details dictionary).
+
+        type details: Dict
+
+        Side Effects:
+        - Displays colorized text messages to indicate the backoff status.
+        - Logs an info message when the rate limit is initially reached.
+        - Sets the `_rate_limit_status` attribute to True when the rate limit is first encountered.
+
+        :returns: None
+        :rtype: NoneType
+        """
         if self._rate_limit_status is False:
-            colorized_text('The synonyms query rate limit was reached. The querying process is '
-                                 'entering a temporary hibernation mode.', 'red')
-            logger.info('The synonyms query rate limit was reached.')
+            colorized_text(text='The antonyms query rate limit was reached. The querying process is '
+                                'entering a temporary hibernation mode.', color='red')
+            colorized_text(text=f"Backing off {details['wait']:.1f} seconds afters {details['tries']} tries.",
+                           color='blue')
+            logger.info('The antonyms query rate limit was reached.')
             self._rate_limit_status = True
+        elif self._rate_limit_status is True:
+            colorized_text(text=f"Backing off {details['wait']:.1f} seconds afters {details['tries']} tries.",
+                           color='blue')
 
     def _validate_word(self) -> bool:
         """
-        This function is designed to validate that the syntax for
-        a string variable is in an acceptable format.
+        This function is designed to validate that the syntax for a string variable is in an acceptable format.
 
         :return: True or False
-        :rtype: bool
+        :rtype: boolean
         """
         valid_word = word_verification.validate_word_syntax(self._word)
-        if valid_word:
-            return True
-        else:
+        if not valid_word:
             logger.error(f'The word {self._word} was not in a valid format.')
             logger.error(f'Please verify that the word {self._word} is spelled correctly.')
-            return False
+        return valid_word
 
     def _check_cache(self) -> Tuple[bool, Union[Dict[str, List[str]], None]]:
-        check_cache = caching.cache_synonyms(self._word)
+        check_cache = caching.cache_antonyms(self._word)
         return check_cache
 
-    def _update_cache(self, pos_category: str, synonyms: Union[List[str], Set[str]]) -> None:
-        caching.insert_word_cache_synonyms(self._word, pos_category, synonyms)
-        return
+    def _update_cache(self, pos_category: str, antonyms: Union[List[str], Set[str]]) -> None:
+        caching.insert_word_cache_antonyms(self._word, pos_category, antonyms)
 
     def _request_http_response(self, url: str) -> requests.models.Response:
         """
         This function queries the requested online repository and returns the
         response for this specific query.
 
         :param url: the URL for the online repository being queried
         :return: response content
         :rtype: requests.models.Response
         """
+        response = None
         if self._proxies is None and self._user_agent is None:
-            response = Query(url).get_website_html()
-            return response
+            response = Query(url_to_scrape=url).get_website_html()
         elif self._proxies is None and self._user_agent is not None:
-            response = Query(url, self._user_agent).get_website_html()
-            return response
+            response = Query(url_to_scrape=url, user_agent=self._user_agent).get_website_html()
         elif self._proxies is not None and self._user_agent is None:
-            response = Query(url, user_agent=None, proxies=self._proxies).get_website_html()
-            return response
+            response = Query(url_to_scrape=url, user_agent=None, proxies=self._proxies).get_website_html()
         elif self._proxies is not None and self._user_agent is not None:
-            response = Query(url, user_agent=self._user_agent, proxies=self._proxies).get_website_html()
-            return response
+            response = Query(url_to_scrape=url, user_agent=self._user_agent, proxies=self._proxies).get_website_html()
+        return response
 
     def _run_query_tasks_in_parallel(self) -> List[tuple[List[str], str]]:
         """
         Runs the query tasks in parallel using a ThreadPool.
 
         :return: list
         :rtype: nested list
         """
-        tasks = [self._query_collins_dictionary, self._query_merriam_webster, self._query_synonym_com,
-                 self._query_thesaurus_com, self._query_wordnet]
+        sources: list = []
+        if self._sources is None:
+            sources = ['google', 'thesaurus.com', 'wordhippo']
+        elif self._sources is not None:
+            sources = self._sources
+        else:
+            colorized_text(text='Please verify that the sources that were provided are valid. \n'
+                                'Valid Sources: \n'
+                                '- google \n'
+                                '- thesaurus.com \n'
+                                '- wordhippo', color='red')
+
+        primary_sources = {'google': self._query_google,
+                           'thesaurus.com': self._query_thesaurus_com,
+                           'wordhippo': self._query_wordhippo}
+
+        tasks = [v for k, v in primary_sources.items() if k in sources]
 
         with ThreadPoolExecutor(max_workers=5) as executor:
             running_tasks = []
             finished_tasks = []
             try:
                 for task in tasks:
                     submitted_task = executor.submit(task)
                     running_tasks.append(submitted_task)
                 for finished_task in as_completed(running_tasks):
                     finished_tasks.append(finished_task.result())
-                return finished_tasks
-            except Exception as error:
-                logger.error('An unknown error occurred in the following code segment:')
-                logger.error(''.join(traceback.format_tb(error.__traceback__)))
+            except (BrokenExecutor, BrokenThreadPool, TimeoutError) as error:
+                self._handle_query_exceptions(error)
+            return finished_tasks
+
+    def _query_output(self, antonyms: list, part_of_speech: Union[set[str], str]) -> Union[list, dict, str]:
+        """
+            Process the output format based on the specified format.
+
+            :param antonyms: List of synonyms to process.
+            :param type antonyms: list
+            :param part_of_speech: Part of speech associated with the antonyms.
+            :param part_of_speech: Union[set[str], str]
+
+            :returns: Processed output based on the specified output format:
+                - If output format is 'list', returns a sorted list of lowercase antonyms.
+                - If output format is 'dictionary', returns a dictionary with the word,
+                  part of speech, and sorted antonyms.
+                - If output format is 'json', returns a JSON object with the word,
+                  part of speech, and sorted antonyms.
+            :rtype: Union[list, dict, str]
+            """
+        processed_output = None
+        if self._output_format == 'list':
+            processed_output = sorted({word.lower() for word in antonyms})
+        elif self._output_format == 'dictionary':
+            processed_output = {self._word: {'part_of_speech': ''.join(part_of_speech),
+                                             'antonyms': sorted(set(antonyms))}}
+        elif self._output_format == 'json':
+            processed_output = json.dumps({self._word:
+                                               {'part_of_speech': ''.join(part_of_speech),
+                                                'antonyms': sorted(set(antonyms), key=len)}}, indent=4, ensure_ascii=False)
+        return processed_output
+
+    def find_antonyms(self) -> Union[List[Sized], Dict[str, List[str]], str]:
+        """
+        This function queries multiple online repositories to discover antonyms
+        associated with the specific word provided to the Class Antonyms.
+        The antonyms are deduplicated and sorted alphabetically.
 
-    def find_synonyms(self) -> Union[List[Sized], Dict[str, List[str]], str]:
-        """
-        Purpose
-        ----------
-        This function queries multiple online repositories to discover synonyms
-        associated with the specific word provided to the Class Synonyms.
-        The synonyms are deduplicated and sorted alphabetically.
-
-        Returns
-        ----------
-        :returns:
-            synonyms: list of synonyms
-
-        :rtype: list
+        :returns: antonyms with parts of speech
+        :rtype: Union[List[Sized], Dict[str, List[str]], str]
         """
         if self._output_format not in self._valid_output_formats:
-            colorized_text(f'The provided output type --> {self._output_format} <-- is not one of the '
-                           f'acceptable types: dictionary, list or json.', 'red')
+            colorized_text(text=f'The provided output type --> {self._output_format} <-- is not one of the '
+                                f'acceptable types: dictionary, list or json.', color='red')
             sys.exit(1)
         else:
             valid_word = self._validate_word()
             if valid_word is False:
-                colorized_text(f'Please verify that the word {self._word} is spelled correctly.', 'magenta')
+                colorized_text(text=f'Please verify that the word --> {self._word} <-- is spelled correctly.',
+                               color='magenta')
             elif valid_word is True:
                 check_cache = self._check_cache()
                 if check_cache[0] is True:
                     part_of_speech = list(check_cache[1].keys())[0]
-                    synonyms = cleansing.flatten_multidimensional_list(list(check_cache[1].values()))
-                    if self._output_format == 'list':
-                        return sorted(set(synonyms))
-                    elif self._output_format == 'dictionary':
-                        output_dict = {self._word: {'part_of_speech': part_of_speech, 'synonyms': sorted(set(
-                            synonyms), key=len)}}
-                        return output_dict
-                    elif self._output_format == 'json':
-                        json_object = json.dumps({self._word: {'part_of_speech': part_of_speech,
-                                                               'synonyms': sorted(set(synonyms), key=len)}},
-                                                 indent=4, ensure_ascii=False)
-                        return json_object
-
+                    antonyms = cleansing.flatten_multidimensional_list(list(check_cache[1].values()))
+                    return self._query_output(antonyms, part_of_speech)
                 elif check_cache[0] is False:
                     query_results = self._run_query_tasks_in_parallel()
-                    part_of_speech = ''.join(set([x[1] for x in query_results if x and x is not None]))
-                    synonyms = ([x[0] for x in query_results if x and x is not None])
-                    # flatten synonyms list
-                    synonyms_results =  cleansing.flatten_multidimensional_list(synonyms)
+                    part_of_speech = {x[1] for x in query_results if x and x is not None}
+                    antonyms = ([x[0] for x in query_results if x and x is not None])
+                    # flatten antonyms list
+                    antonyms_results = cleansing.flatten_multidimensional_list(sorted(antonyms))
                     # remove excess white spaces from the strings in the list
-                    synonyms_results = cleansing.normalize_space(synonyms_results)
-                    if not synonyms_results:
-                        colorized_text(f'No synonyms were found for the word: {self._word} \n'
-                                       f'Please verify that the word is spelled correctly.', 'blue')
+                    antonyms_results = cleansing.normalize_space(sorted(antonyms_results))
+                    if not antonyms_results:
+                        colorized_text(text=f'No antonyms were found for the word: {self._word} \n'
+                                       f'Please verify that the word is spelled correctly.', color='blue')
                     else:
-                        if self._output_format == 'list':
-                            return sorted(set([word.lower() for word in synonyms_results]))
-                        elif self._output_format == 'dictionary':
-                            output_dict = {self._word: {'part_of_speech': part_of_speech, 'synonyms': sorted(set(
-                                synonyms_results), key=len)}}
-                            return output_dict
-                        elif self._output_format == 'json':
-                            json_object = json.dumps({self._word: {'part_of_speech': part_of_speech,
-                                                                   'synonyms': sorted(set(synonyms_results), key=len)}},
-                                                     indent=4, ensure_ascii=False)
-                            return json_object
-
+                        return self._query_output(antonyms_results, part_of_speech)
 
-    def _query_collins_dictionary(self) -> Union[Tuple[List[str], str], None]:
+    @staticmethod
+    def _handle_query_exceptions(error):
         """
-        This function queries collinsdictionary.com for synonyms associated
-        with the specific word provided to the Class Synonyms.
-
-        :returns:
-            synonyms: list of synonyms
-
-        :rtype: list
-
-        :raises:
-            AttributeError: Raised when an attribute reference or assignment fails
-
-            IndexError: Raised when a sequence subscript is out of range
-
-            KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys
-
-            TypeError: Raised when an operation or function is applied to an object of inappropriate type
-
-            bs4.FeatureNotFound: raised by the BeautifulSoup constructor if no parser with the requested features
-            is found
+        Helper method to handle common exceptions in query methods.
         """
-        try:
-            response = self._request_http_response(f'https://www.collinsdictionary.com/dictionary/english-thesaurus/{self._word}')
-
-            if response.status_code == 404:
-                logger.info(f'Collins Dictionary had no synonym reference for the word {self._word}')
-                return None
-            else:
-                soup = BeautifulSoup(response.text, 'lxml')
-                cloudflare_protection = CloudflareVerification('https://www.collinsdictionary.com',
-                                                               soup).cloudflare_protected_url()
-                if cloudflare_protection is False:
-                    no_word_results = soup.find('h1',
-                                           text=f'Sorry, no results for “{self._word}” in the English Thesaurus.')
-                    if no_word_results:
-                        logger.info(f'Collins Dictionary had no synonym reference for the word {self._word}')
-                        return None
-                    else:
-                        part_of_speech_category = ''
-                        # obtain the part of speech category for the specific word
-                        if soup.find('span', {'class': 'headerSensePos'}):
-                            tag_part_of_speech = soup.find('span', {'class': 'headerSensePos'})
-                            if len(tag_part_of_speech.text) != 0:
-                                part_of_speech_category = tag_part_of_speech.text.strip('()')
-                            else:
-                                part_of_speech_category = ''
-
-                        synonyms = []
-                        query_results = soup.find('div', {'class': 'blockSyn'})
-                        if query_results:
-                            for sub_syn in query_results.find_all('div', {'class', 'form type-syn'}):
-                                child = sub_syn.findChild('span', {'class': 'orth'})
-                                synonyms.append(child.text)
-                            synonyms_list = sorted([x.lower().strip() for x in synonyms])
-                            self._update_cache(part_of_speech_category, synonyms_list)
-                            return synonyms_list, part_of_speech_category
+        logger.error('An error occurred in the following code segment:')
+        logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
-                elif cloudflare_protection is True:
-                    part_of_speech_category = ''
-
-                    fresh_soup = Cloudflare(f'https://www.collinsdictionary.com/dictionary/english-thesaurus'
-                                            f'/{self._word}').bypass()
-
-                    # obtain the part of speech category for the specific word
-                    if fresh_soup.find('span', {'class': 'headerSensePos'}):
-                        tag_part_of_speech = fresh_soup.find('span', {'class': 'headerSensePos'})
-                        if len(tag_part_of_speech.text) != 0:
-                            part_of_speech_category = tag_part_of_speech.text.strip('()')
-                        else:
-                            part_of_speech_category = ''
-
-                    synonyms = []
-                    query_results = fresh_soup.find('div', {'class': 'blockSyn'})
-                    if query_results:
-                        for sub_syn in query_results.find_all('div', {'class', 'form type-syn'}):
-                            child = sub_syn.findChild('span', {'class': 'orth'})
-                            synonyms.append(child.text)
-
-                        synonyms_list = sorted([x.lower().strip() for x in synonyms])
-                        self._update_cache(part_of_speech_category, synonyms_list)
-                        return synonyms_list, part_of_speech_category
-
-        except bs4.FeatureNotFound as error:
-            logger.error('An error occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except AttributeError as error:
-            logger.error('An AttributeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except IndexError as error:
-            logger.error('An IndexError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except KeyError as error:
-            logger.error('A KeyError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except TypeError as error:
-            logger.error('A TypeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-
-
-    def _query_merriam_webster(self) -> Union[Tuple[List[str], str], None]:
+    def _query_google(self) -> Union[Tuple[List[str], str], None]:
         """
-        This function queries merriam-webster.com for synonyms associated
-        with the specific word provided to the Class Synonyms.
-
-        :returns:
-            synonyms: list of synonyms
-
-        :rtype: list or None
+        This function queries google.com for antonyms associated with the specific word provided to the Class Antonyms.
 
+        :returns: list of antonyms and parts of speech str
+        :rtype: Union[Tuple[List[str], str]
         :raises:
-           AttributeError: Raised when an attribute reference or assignment fails
-
-            IndexError: Raised when a sequence subscript is out of range
-
-            KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys
-
-            TypeError: Raised when an operation or function is applied to an object of inappropriate type
-
-            bs4.FeatureNotFound: raised by the BeautifulSoup constructor if no parser with the requested features
-            is found
+            - AttributeError: When an attribute reference or assignment fails.
+            - IndexError: When a sequence subscript is out of range.
+            - KeyError: When a mapping key is not found in the set of existing keys.
+            - TypeError: When an operation or function is applied to an inappropriate type.
+            - bs4.FeatureNotFound: Raised by the BeautifulSoup constructor if no parser with the requested features is found.
         """
         try:
-            response = self._request_http_response(f'https://www.merriam-webster.com/thesaurus/{self._word}')
+            response = self._request_http_response(url=f'https://www.google.com/search?q=antonym+for+/{self._word}')
 
             if response.status_code == 404:
-                logger.info(f'Merriam-webster.com had no synonym reference for the word {self._word}')
+                logger.info(f'Google had no antonym reference for the word {self._word}')
                 return None
             else:
-                soup = BeautifulSoup(response.text, "lxml")
-                cloudflare_protection = CloudflareVerification('https://www.merriam-webster.com',
-                                                               soup).cloudflare_protected_url()
-                if cloudflare_protection is False:
-                    pattern = regex.compile(r'Words fail us')
-                    if soup.find(text=pattern):
-                        logger.info(f'Merriam-webster.com had no synonym reference for the word {self._word}')
-                        return None
-                    elif soup.find('h1', {'class': 'mispelled-word'}):
-                        logger.info(f'Merriam-webster.com had no synonym reference for the word {self._word}')
-                        return None
-                    else:
-                        synonyms_list = []
-                        part_of_speech_category = ''
-
-                        # obtain the part of speech category for the specific word
-                        if soup.select('#thesaurus-entry-1-1 > div.row.entry-header > div > div > div.align-items-baseline.d-flex.flex-grow-1 > h2 > a'):
-                            css_part_of_speech = soup.select(
-                                '#thesaurus-entry-1-1 > div.row.entry-header > div > div > div.align-items-baseline.d-flex.flex-grow-1 > h2 > a')
-                            if len(css_part_of_speech[0].text) != 0:
-                                part_of_speech_category = css_part_of_speech[0].text
-                            else:
-                                part_of_speech_category = ''
-
-                        if soup.find('p', {'class': 'function-label'}):
-                            label = soup.find('p', {'class': 'function-label'})
-                            if label.text.startswith('Synonyms'):
-                                word_container = soup.find('div', {'class': 'thes-list-content synonyms_list'})
-                                for list_item in word_container.find_all("li", {'class': 'thes-word-list-item'}):
-                                    if list_item.find('span', {'class': 'lozenge color-4'}) or \
-                                        list_item.find('span', {'class': 'lozenge color-3'}):
-                                        link = list_item.find('a', href=True)
-                                        synonyms_list.append(link.text.strip())
-                                synonyms_list = sorted([x.lower().strip() for x in synonyms_list])
-                                self._update_cache(part_of_speech_category, synonyms_list)
-                            return synonyms_list, part_of_speech_category
-                elif cloudflare_protection is True:
+                soup_object = BeautifulSoup(markup=response.text, features="lxml")
+                antonyms_list = ParseWords.parse_google_com(soup= soup_object, word=self._word)
+                if antonyms_list:
+                    self._update_cache(pos_category='noun', antonyms=sorted(antonyms_list))
+                    return antonyms_list, 'noun'
+                else:
+                    logger.info(f'Google had no antonym reference for the word {self._word}')
                     return None
-
-        except bs4.FeatureNotFound as error:
-            logger.error('An error occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except AttributeError as error:
-            logger.error('An AttributeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except IndexError as error:
-            logger.error('An IndexError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except KeyError as error:
-            logger.error('A KeyError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except TypeError as error:
-            logger.error('A TypeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-
-
-    def _query_synonym_com(self) -> Union[Tuple[List[str], str], None]:
-        """
-        This function queries synonym.com for synonyms associated
-        with the specific word provided to the Class Synonyms.
-
-         :returns:
-            synonyms: list of synonyms
-
-        :rtype: list or None
-
-        :raises:
-            AttributeError: Raised when an attribute reference or assignment fails
-
-            IndexError: Raised when a sequence subscript is out of range
-
-            KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys
-
-            TypeError: Raised when an operation or function is applied to an object of inappropriate type
-
-            bs4.FeatureNotFound: raised by the BeautifulSoup constructor if no parser with the requested features
-            is found
-        """
-        try:
-            response = self._request_http_response(f'https://www.synonym.com/synonyms/{self._word}')
-
-            if response.status_code == 404:
-                logger.info(f'Synonym.com had no synonym reference for the word {self._word}')
-                return None
-            else:
-                soup = BeautifulSoup(response.text, "lxml")
-                cloudflare_protection = CloudflareVerification('https://www.synonym.com',
-                                                               soup).cloudflare_protected_url()
-                if cloudflare_protection is False:
-                    status_tag = soup.find("meta", {"name": "pagetype"})
-                    pattern = regex.compile(r'Oops, 404!')
-                    if soup.find(text=pattern):
-                        logger.info(f'Synonym.com had no synonym reference for the word {self._word}')
-                        return None
-                    elif status_tag.attrs['content'] == 'Term':
-                        part_of_speech_category = ''
-
-                        if soup.find('div', {'data-section': 'synonyms'}):
-                            synonyms_class = soup.find('div', {'data-section': 'synonyms'})
-                            synonyms = [word.text for word in
-                                        synonyms_class.find('ul', {'class': 'section-list'}).find_all('li')]
-                            synonyms_list = sorted([x.lower().strip() for x in synonyms])
-
-                            # obtain the part of speech category for the specific word
-                            if soup.select('body > div.page-container > div.content-container > div.main-column > div.sections-wrapper > div:nth-child(1) > p > strong'):
-                                css_part_of_speech = soup.select(
-                                    'body > div.page-container > div.content-container > div.main-column > div.sections-wrapper > div:nth-child(1) > p > strong')
-                                if len(css_part_of_speech[0].text) != 0:
-                                    part_of_speech_category = css_part_of_speech[0].text.strip('.')
-                                else:
-                                    part_of_speech_category = ''
-
-                            self._update_cache(part_of_speech_category, synonyms_list)
-                            return synonyms_list, part_of_speech_category
-                        else:
-                            logger.info(f'Synonym.com had no synonym reference for the word {self._word}')
-                            return None
-                elif cloudflare_protection is True:
-                    return None
-
-        except bs4.FeatureNotFound as error:
-            logger.error('An error occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except AttributeError as error:
-            logger.error('An AttributeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except IndexError as error:
-            logger.error('An IndexError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except KeyError as error:
-            logger.error('A KeyError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except TypeError as error:
-            logger.error('A TypeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            self._handle_query_exceptions(error)
 
     def _query_thesaurus_com(self) -> Union[Tuple[List[str], str], None]:
         """
-        This function queries thesaurus.com for synonyms associated
-        with the specific word provided to the Class Synonyms.
-
-        :returns:
-            synonyms: list of synonyms
-
-        :rtype: list or None
+        This function queries thesaurus.com for antonyms associated with the specific word provided to the Class
+        Antonyms.
 
+        :returns: list of antonyms and parts of speech str
+        :rtype: Union[Tuple[List[str], str]
         :raises:
-            AttributeError: Raised when an attribute reference or assignment fails
-
-            IndexError: Raised when a sequence subscript is out of range
-
-            KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys
-
-            TypeError: Raised when an operation or function is applied to an object of inappropriate type
-
-            bs4.FeatureNotFound: raised by the BeautifulSoup constructor if no parser with the requested features
-            is found
+            - AttributeError: When an attribute reference or assignment fails.
+            - IndexError: When a sequence subscript is out of range.
+            - KeyError: When a mapping key is not found in the set of existing keys.
+            - TypeError: When an operation or function is applied to an inappropriate type.
+            - bs4.FeatureNotFound: Raised by the BeautifulSoup constructor if no parser with the requested features is found.
         """
         try:
-            response = self._request_http_response(f'https://www.thesaurus.com/browse/{self._word}')
+            response = self._request_http_response(url=f'https://www.thesaurus.com/browse/{self._word}')
 
             if response.status_code == 404:
-                logger.info(f'Thesaurus.com had no synonym reference for the word {self._word}')
+                logger.info(f'Thesaurus.com had no antonym reference for the word {self._word}')
                 return None
             else:
-                soup = BeautifulSoup(response.text, "lxml")
-                cloudflare_protection = CloudflareVerification('https://www.thesaurus.com',
-                                                               soup).cloudflare_protected_url()
+                soup_object = BeautifulSoup(markup=response.text, features="lxml")
+                cloudflare_protection = CloudflareVerification(url='https://www.thesaurus.com', soup=soup_object).cloudflare_protected_url()
                 if cloudflare_protection is False:
-                    status_tag = soup.find("h1")
-                    if status_tag.text.startswith('0 results for'):
-                        logger.info(f'Thesaurus.com had no synonym reference for the word {self._word}')
-                        return None
+                    antonym_button_tag = soup_object.find(name='button', attrs={'data-linkmodule': 'antonym-module'})
+                    if antonym_button_tag:
+                        antonyms_list = ParseWords.parse_thesaurus_com(soup=soup_object)
+                        part_of_speech_category = PartOfSpeech.part_of_speech_category_thesaurus_com(soup=soup_object)
+                        self._update_cache(pos_category=part_of_speech_category, antonyms=sorted(antonyms_list))
+                        return antonyms_list, part_of_speech_category
                     else:
-                        synonyms_list = []
-                        part_of_speech_category = ''
-                        # obtain the part of speech category for the specific word
-                        if soup.select('#headword > div.css-bjn8wh.e1br8a1p0 > div > ul > li > a > em'):
-                            css_part_of_speech = soup.select(
-                            '#headword > div.css-bjn8wh.e1br8a1p0 > div > ul > li > a > em')
-                            if len(css_part_of_speech[0].text) != 0:
-                                part_of_speech_category = css_part_of_speech[0].text
-                            else:
-                                part_of_speech_category = ''
-                        word_container = soup.find('div', {'data-testid': 'word-grid-container'})
-                        for list_item in word_container.find('ul').find_all('li'):
-                            for link in list_item.find_all('a', {'class': 'css-1kg1yv8 eh475bn0'}):
-                                synonyms_list.append(link.text.strip())
-
-                            synonyms_list = sorted([x.lower().strip() for x in  synonyms_list])
-                        self._update_cache(part_of_speech_category, synonyms_list)
-                        return synonyms_list, part_of_speech_category
+                        logger.info(f'Thesaurus.com had no antonym reference for the word {self._word}')
+                        return None
                 elif cloudflare_protection is True:
                     return None
 
-        except bs4.FeatureNotFound as error:
-            logger.error('An error occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except AttributeError as error:
-            logger.error('An AttributeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except IndexError as error:
-            logger.error('An IndexError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except KeyError as error:
-            logger.error('A KeyError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except TypeError as error:
-            logger.error('A TypeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            self._handle_query_exceptions(error)
 
-    def _query_wordnet(self) -> Union[Tuple[List[str], str], None]:
+    def _query_wordhippo(self) -> Union[Tuple[List[str], str], None]:
         """
-        This function queries wordnet for synonyms associated
-        with the specific word provided to the Class Synonyms.
-
-        :returns:
-            synonyms: list of synonyms
-
-        :rtype: list
+        This function queries wordhippo.com for antonyms associated with the
+        specific word provided to the Class Antonyms.
 
+        :returns: list of antonyms and part of speech string
+        :rtype: Union[Tuple[List[str], str], None]
         :raises:
-            AttributeError: Raised when an attribute reference or assignment fails
-
-            IndexError: Raised when a sequence subscript is out of range
-
-            KeyError: Raised when a mapping (dictionary) key is not found in the set of existing keys
-
-            TypeError: Raised when an operation or function is applied to an object of inappropriate type
-
-            bs4.FeatureNotFound: raised by the BeautifulSoup constructor if no parser with the requested features
-            is found
+            - AttributeError: When an attribute reference or assignment fails.
+            - IndexError: When a sequence subscript is out of range.
+            - KeyError: When a mapping key is not found in the set of existing keys.
+            - TypeError: When an operation or function is applied to an inappropriate type.
+            - bs4.FeatureNotFound: Raised by the BeautifulSoup constructor if no parser with the requested features is found.
         """
         try:
-            response = self._request_http_response(f'http://wordnetweb.princeton.edu/perl/webwn?s={self._word}')
+            response = self._request_http_response(url=f'https://www.wordhippo.com/what-is/the-opposite-of/{self._word}.html')
 
             if response.status_code == 404:
-                logger.info(f'Wordnet had no synonym reference for the word {self._word}')
+                logger.info(f'Wordhippo.com had no antonym reference for the word {self._word}')
                 return None
             else:
-                soup = BeautifulSoup(response.text, "lxml")
-                cloudflare_protection = CloudflareVerification('http://wordnetweb.princeton.edu',
-                                                               soup).cloudflare_protected_url()
+                soup_object = BeautifulSoup(markup=response.text, features="lxml")
+                cloudflare_protection = CloudflareVerification(url='https://www.wordhippo.com', soup=soup_object).cloudflare_protected_url()
                 if cloudflare_protection is False:
-                    pattern = regex.compile(r'Your search did not return any results')
-                    if soup.find(text=pattern):
-                        logger.info(f'Wordnet had no synonym reference for the word {self._word}')
+                    pattern = regex.compile(pattern=r'We do not currently know of any antonyms for')
+                    if soup_object.find(text=pattern):
+                        logger.info(f'Wordhippo.com had no antonym reference for the word {self._word}')
                         return None
                     else:
-                        synonyms_list = []
-                        if soup.findAll('h3', text='Noun'):
-                            part_of_speech_category = 'noun'
-                            parent_node = soup.findAll("ul")[0].findAll('li')
-                            for children in parent_node:
-                                for child in children.find_all(href=True):
-                                    if 'S:' not in child.contents[0]:
-                                        synonyms_list.append(child.contents[0])
-                            synonyms_list = sorted([x.lower().strip() for x in synonyms_list])
-                            self._update_cache(part_of_speech_category, synonyms_list)
-                            return synonyms_list, part_of_speech_category
+                        part_of_speech_category = PartOfSpeech.part_of_speech_category_wordhippo(soup=soup_object)
+                        antonyms_list = ParseWords.parse_wordhippo(soup=soup_object)
+                        self._update_cache(pos_category=part_of_speech_category, antonyms=sorted(antonyms_list))
+                        return antonyms_list, part_of_speech_category
                 elif cloudflare_protection is True:
                     return None
-
-        except bs4.FeatureNotFound as error:
-            logger.error('An error occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except AttributeError as error:
-            logger.error('An AttributeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except IndexError as error:
-            logger.error('An IndexError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except KeyError as error:
-            logger.error('A KeyError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-        except TypeError as error:
-            logger.error('A TypeError occurred in the following code segment:')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-
+        except (bs4.FeatureNotFound, AttributeError, IndexError, KeyError, TypeError) as error:
+            self._handle_query_exceptions(error)
```

### Comparing `wordhoard-1.5.4/wordhoard/utilities/__pycache__/captcha_checker.cpython-39.pyc` & `wordhoard-1.5.5/wordhoard/utilities/__pycache__/captcha_checker.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.4/wordhoard/utilities/__pycache__/cleansing.cpython-39.pyc` & `wordhoard-1.5.5/wordhoard/utilities/__pycache__/cleansing.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Mar  4 13:53:23 2023 UTC, .py size: 2226 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 534d 0364 b208 0000  a.......SM.d....
+00000000: 610d 0d0a 0000 0000 d28a 3f66 b108 0000  a.........?f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5a05 6406 6407 6c06 6d07 5a07  Z.d.Z.d.d.l.m.Z.
 00000050: 6d08 5a08 0100 6507 6507 6408 9c02 6409  m.Z...e.e.d...d.
 00000060: 640a 8404 5a09 650a 650a 640b 9c02 640c  d...Z.e.e.d...d.
 00000070: 640d 8404 5a0b 6508 6507 650a 1900 6507  d...Z.e.e.e...e.
@@ -37,97 +37,97 @@
 00000240: 6473 0a20 2020 203a 7265 7475 726e 3a20  ds.    :return: 
 00000250: 6c69 7374 206f 6620 776f 7264 730a 2020  list of words.  
 00000260: 2020 6301 0000 0000 0000 0000 0000 0002    c.............
 00000270: 0000 0004 0000 0053 0000 0073 1400 0000  .......S...s....
 00000280: 6700 7c00 5d0c 7d01 7c01 a000 a100 9102  g.|.].}.|.......
 00000290: 7104 5300 a900 2901 da05 7374 7269 7029  q.S...)...strip)
 000002a0: 02da 022e 30da 0178 7208 0000 0072 0800  ....0..xr....r..
-000002b0: 0000 fa57 2f55 7365 7273 2f62 756d 6761  ...W/Users/bumga
+000002b0: 0000 fa56 2f55 7365 7273 2f62 756d 6761  ...V/Users/bumga
 000002c0: 726e 6572 2f50 7974 686f 6e5f 5072 6f6a  rner/Python_Proj
-000002d0: 6563 7473 2f77 6f72 6468 6f61 7264 5f64  ects/wordhoard_d
-000002e0: 6576 656c 6f70 6d65 6e74 2f77 6f72 6468  evelopment/wordh
-000002f0: 6f61 7264 2f75 7469 6c69 7469 6573 2f63  oard/utilities/c
-00000300: 6c65 616e 7369 6e67 2e70 79da 0a3c 6c69  leansing.py..<li
-00000310: 7374 636f 6d70 3e28 0000 00f3 0000 0000  stcomp>(........
-00000320: 7a23 6e6f 726d 616c 697a 655f 7370 6163  z#normalize_spac
-00000330: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
-00000340: 636f 6d70 3e72 0800 0000 2902 7206 0000  comp>r....).r...
-00000350: 005a 0e6e 6f72 6d61 6c69 7a65 5f6c 6973  .Z.normalize_lis
-00000360: 7472 0800 0000 7208 0000 0072 0c00 0000  tr....r....r....
-00000370: da0f 6e6f 726d 616c 697a 655f 7370 6163  ..normalize_spac
-00000380: 651f 0000 0073 0400 0000 0009 0e01 720f  e....s........r.
-00000390: 0000 0029 02da 0c69 6e70 7574 5f73 7472  ...)...input_str
-000003a0: 696e 6772 0700 0000 6301 0000 0000 0000  ingr....c.......
-000003b0: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-000003c0: 0073 0e00 0000 6401 a000 7c00 a001 a100  .s....d...|.....
-000003d0: a101 5300 2902 7ab4 0a20 2020 2054 6869  ..S.).z..    Thi
-000003e0: 7320 6675 6e63 7469 6f6e 2075 7365 7320  s function uses 
-000003f0: 7468 6520 6a6f 696e 2829 2061 6e64 2073  the join() and s
-00000400: 706c 6974 2829 206d 6574 686f 6473 2074  plit() methods t
-00000410: 6f67 6574 6865 7220 746f 2072 656d 6f76  ogether to remov
-00000420: 6520 6475 706c 6963 6174 6520 7370 6163  e duplicate spac
-00000430: 6573 0a20 2020 2061 6e64 206e 6577 6c69  es.    and newli
-00000440: 6e65 2063 6861 7261 6374 6572 7320 6672  ne characters fr
-00000450: 6f6d 2061 2073 7472 696e 672e 0a0a 2020  om a string...  
-00000460: 2020 3a70 6172 616d 2069 6e70 7574 5f73    :param input_s
-00000470: 7472 696e 673a 0a20 2020 203a 7265 7475  tring:.    :retu
-00000480: 726e 3a20 7374 720a 2020 2020 da01 2029  rn: str.    .. )
-00000490: 02da 046a 6f69 6eda 0573 706c 6974 2901  ...join..split).
-000004a0: 7210 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
-000004b0: 0c00 0000 da18 7265 6d6f 7665 5f65 7863  ......remove_exc
-000004c0: 6573 735f 7768 6974 6573 7061 6365 2b00  ess_whitespace+.
-000004d0: 0000 7302 0000 0000 0872 1400 0000 2902  ..s......r....).
-000004e0: da0d 6c69 7374 5f6f 665f 6c69 7374 7372  ..list_of_listsr
-000004f0: 0700 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00000500: 0002 0000 0003 0000 0043 0000 0073 2c00  .........C...s,.
-00000510: 0000 7400 6401 6402 8400 7c00 4400 8301  ..t.d.d...|.D...
-00000520: 8301 7224 6403 6404 8400 7c00 4400 8301  ..r$d.d...|.D...
-00000530: 7d01 7c01 5300 7c00 5300 6405 5300 2906  }.|.S.|.S.d.S.).
-00000540: 7aa5 0a20 2020 2054 6869 7320 6675 6e63  z..    This func
-00000550: 7469 6f6e 2069 7320 7573 6564 2074 6f20  tion is used to 
-00000560: 666c 6174 7465 6e20 6120 6d75 6c74 6964  flatten a multid
-00000570: 696d 656e 7369 6f6e 616c 206c 6973 7420  imensional list 
-00000580: 696e 746f 2061 2073 696e 676c 6520 6c69  into a single li
-00000590: 7374 2e0a 0a20 2020 203a 7265 7475 726e  st...    :return
-000005a0: 3a20 6120 6d75 6c74 6964 696d 656e 7369  : a multidimensi
-000005b0: 6f6e 616c 206c 6973 7420 7468 6174 2068  onal list that h
-000005c0: 6173 2062 6565 6e20 666c 6174 7465 6e65  as been flattene
-000005d0: 640a 2020 2020 3a72 7479 7065 3a20 6c69  d.    :rtype: li
-000005e0: 7374 0a20 2020 2063 0100 0000 0000 0000  st.    c........
-000005f0: 0000 0000 0200 0000 0400 0000 7300 0000  ............s...
-00000600: 7318 0000 007c 005d 107d 0174 007c 0174  s....|.].}.t.|.t
-00000610: 0183 0256 0001 0071 0264 0053 0029 014e  ...V...q.d.S.).N
-00000620: 2902 da0a 6973 696e 7374 616e 6365 7204  )...isinstancer.
-00000630: 0000 0029 0272 0a00 0000 da01 6972 0800  ...).r......ir..
-00000640: 0000 7208 0000 0072 0c00 0000 da09 3c67  ..r....r......<g
-00000650: 656e 6578 7072 3e3c 0000 0072 0e00 0000  enexpr><...r....
-00000660: 7a30 666c 6174 7465 6e5f 6d75 6c74 6964  z0flatten_multid
-00000670: 696d 656e 7369 6f6e 616c 5f6c 6973 742e  imensional_list.
-00000680: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
-00000690: 723e 6301 0000 0000 0000 0000 0000 0003  r>c.............
-000006a0: 0000 0004 0000 0053 0000 0073 1a00 0000  .......S...s....
-000006b0: 6700 7c00 5d12 7d01 7c01 4400 5d08 7d02  g.|.].}.|.D.].}.
-000006c0: 7c02 9103 710c 7104 5300 7208 0000 0072  |...q.q.S.r....r
-000006d0: 0800 0000 2903 720a 0000 005a 0873 7562  ....).r....Z.sub
-000006e0: 5f6c 6973 74da 0765 6c65 6d65 6e74 7208  _list..elementr.
-000006f0: 0000 0072 0800 0000 720c 0000 0072 0d00  ...r....r....r..
-00000700: 0000 3d00 0000 720e 0000 007a 3166 6c61  ..=...r....z1fla
-00000710: 7474 656e 5f6d 756c 7469 6469 6d65 6e73  tten_multidimens
-00000720: 696f 6e61 6c5f 6c69 7374 2e3c 6c6f 6361  ional_list.<loca
-00000730: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 4e29  ls>.<listcomp>N)
-00000740: 01da 0361 6e79 2902 7215 0000 005a 0e66  ...any).r....Z.f
-00000750: 6c61 7474 656e 6564 5f6c 6973 7472 0800  lattened_listr..
-00000760: 0000 7208 0000 0072 0c00 0000 da1d 666c  ..r....r......fl
-00000770: 6174 7465 6e5f 6d75 6c74 6964 696d 656e  atten_multidimen
-00000780: 7369 6f6e 616c 5f6c 6973 7435 0000 0073  sional_list5...s
-00000790: 0800 0000 0007 1201 0e01 0402 721b 0000  ............r...
-000007a0: 004e 290d da07 5f5f 646f 635f 5fda 0a5f  .N)...__doc__.._
-000007b0: 5f61 7574 686f 725f 5fda 085f 5f64 6174  _author__..__dat
-000007c0: 655f 5fda 0a5f 5f73 7461 7475 735f 5fda  e__..__status__.
-000007d0: 0b5f 5f6c 6963 656e 7365 5f5f da0d 5f5f  .__license__..__
-000007e0: 636f 7079 7269 6768 745f 5fda 0674 7970  copyright__..typ
-000007f0: 696e 6772 0400 0000 7205 0000 0072 0f00  ingr....r....r..
-00000800: 0000 da03 7374 7272 1400 0000 721b 0000  ....strr....r...
-00000810: 0072 0800 0000 7208 0000 0072 0800 0000  .r....r....r....
-00000820: 720c 0000 00da 083c 6d6f 6475 6c65 3e03  r......<module>.
-00000830: 0000 0073 1200 0000 0403 0401 0401 0401  ...s............
-00000840: 0401 0413 1002 100c 100a                 ..........
+000002d0: 6563 7473 2f77 6f72 6468 6f61 7264 5f70  ects/wordhoard_p
+000002e0: 726f 6475 6374 696f 6e2f 776f 7264 686f  roduction/wordho
+000002f0: 6172 642f 7574 696c 6974 6965 732f 636c  ard/utilities/cl
+00000300: 6561 6e73 696e 672e 7079 da0a 3c6c 6973  eansing.py..<lis
+00000310: 7463 6f6d 703e 2800 0000 f300 0000 007a  tcomp>(........z
+00000320: 236e 6f72 6d61 6c69 7a65 5f73 7061 6365  #normalize_space
+00000330: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00000340: 6f6d 703e 7208 0000 0029 0272 0600 0000  omp>r....).r....
+00000350: 5a0e 6e6f 726d 616c 697a 655f 6c69 7374  Z.normalize_list
+00000360: 7208 0000 0072 0800 0000 720c 0000 00da  r....r....r.....
+00000370: 0f6e 6f72 6d61 6c69 7a65 5f73 7061 6365  .normalize_space
+00000380: 1f00 0000 7304 0000 0000 090e 0172 0f00  ....s........r..
+00000390: 0000 2902 da0c 696e 7075 745f 7374 7269  ..)...input_stri
+000003a0: 6e67 7207 0000 0063 0100 0000 0000 0000  ngr....c........
+000003b0: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
+000003c0: 730e 0000 0064 01a0 007c 00a0 01a1 00a1  s....d...|......
+000003d0: 0153 0029 027a b40a 2020 2020 5468 6973  .S.).z..    This
+000003e0: 2066 756e 6374 696f 6e20 7573 6573 2074   function uses t
+000003f0: 6865 206a 6f69 6e28 2920 616e 6420 7370  he join() and sp
+00000400: 6c69 7428 2920 6d65 7468 6f64 7320 746f  lit() methods to
+00000410: 6765 7468 6572 2074 6f20 7265 6d6f 7665  gether to remove
+00000420: 2064 7570 6c69 6361 7465 2073 7061 6365   duplicate space
+00000430: 730a 2020 2020 616e 6420 6e65 776c 696e  s.    and newlin
+00000440: 6520 6368 6172 6163 7465 7273 2066 726f  e characters fro
+00000450: 6d20 6120 7374 7269 6e67 2e0a 0a20 2020  m a string...   
+00000460: 203a 7061 7261 6d20 696e 7075 745f 7374   :param input_st
+00000470: 7269 6e67 3a0a 2020 2020 3a72 6574 7572  ring:.    :retur
+00000480: 6e3a 2073 7472 0a20 2020 20da 0120 2902  n: str.    .. ).
+00000490: da04 6a6f 696e da05 7370 6c69 7429 0172  ..join..split).r
+000004a0: 1000 0000 7208 0000 0072 0800 0000 720c  ....r....r....r.
+000004b0: 0000 00da 1872 656d 6f76 655f 6578 6365  .....remove_exce
+000004c0: 7373 5f77 6869 7465 7370 6163 652b 0000  ss_whitespace+..
+000004d0: 0073 0200 0000 0008 7214 0000 0029 02da  .s......r....)..
+000004e0: 0d6c 6973 745f 6f66 5f6c 6973 7473 7207  .list_of_listsr.
+000004f0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000500: 0200 0000 0300 0000 4300 0000 732c 0000  ........C...s,..
+00000510: 0074 0064 0164 0284 007c 0044 0083 0183  .t.d.d...|.D....
+00000520: 0172 2464 0364 0484 007c 0044 0083 017d  .r$d.d...|.D...}
+00000530: 017c 0153 007c 0053 0064 0553 0029 067a  .|.S.|.S.d.S.).z
+00000540: a50a 2020 2020 5468 6973 2066 756e 6374  ..    This funct
+00000550: 696f 6e20 6973 2075 7365 6420 746f 2066  ion is used to f
+00000560: 6c61 7474 656e 2061 206d 756c 7469 6469  latten a multidi
+00000570: 6d65 6e73 696f 6e61 6c20 6c69 7374 2069  mensional list i
+00000580: 6e74 6f20 6120 7369 6e67 6c65 206c 6973  nto a single lis
+00000590: 742e 0a0a 2020 2020 3a72 6574 7572 6e3a  t...    :return:
+000005a0: 2061 206d 756c 7469 6469 6d65 6e73 696f   a multidimensio
+000005b0: 6e61 6c20 6c69 7374 2074 6861 7420 6861  nal list that ha
+000005c0: 7320 6265 656e 2066 6c61 7474 656e 6564  s been flattened
+000005d0: 0a20 2020 203a 7274 7970 653a 206c 6973  .    :rtype: lis
+000005e0: 740a 2020 2020 6301 0000 0000 0000 0000  t.    c.........
+000005f0: 0000 0002 0000 0004 0000 0073 0000 0073  ...........s...s
+00000600: 1800 0000 7c00 5d10 7d01 7400 7c01 7401  ....|.].}.t.|.t.
+00000610: 8302 5600 0100 7102 6400 5300 2901 4e29  ..V...q.d.S.).N)
+00000620: 02da 0a69 7369 6e73 7461 6e63 6572 0400  ...isinstancer..
+00000630: 0000 2902 720a 0000 00da 0169 7208 0000  ..).r......ir...
+00000640: 0072 0800 0000 720c 0000 00da 093c 6765  .r....r......<ge
+00000650: 6e65 7870 723e 3c00 0000 720e 0000 007a  nexpr><...r....z
+00000660: 3066 6c61 7474 656e 5f6d 756c 7469 6469  0flatten_multidi
+00000670: 6d65 6e73 696f 6e61 6c5f 6c69 7374 2e3c  mensional_list.<
+00000680: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
+00000690: 3e63 0100 0000 0000 0000 0000 0000 0300  >c..............
+000006a0: 0000 0400 0000 5300 0000 731a 0000 0067  ......S...s....g
+000006b0: 007c 005d 127d 017c 0144 005d 087d 027c  .|.].}.|.D.].}.|
+000006c0: 0291 0371 0c71 0453 0072 0800 0000 7208  ...q.q.S.r....r.
+000006d0: 0000 0029 0372 0a00 0000 5a08 7375 625f  ...).r....Z.sub_
+000006e0: 6c69 7374 da07 656c 656d 656e 7472 0800  list..elementr..
+000006f0: 0000 7208 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000700: 003d 0000 0072 0e00 0000 7a31 666c 6174  .=...r....z1flat
+00000710: 7465 6e5f 6d75 6c74 6964 696d 656e 7369  ten_multidimensi
+00000720: 6f6e 616c 5f6c 6973 742e 3c6c 6f63 616c  onal_list.<local
+00000730: 733e 2e3c 6c69 7374 636f 6d70 3e4e 2901  s>.<listcomp>N).
+00000740: da03 616e 7929 0272 1500 0000 5a0e 666c  ..any).r....Z.fl
+00000750: 6174 7465 6e65 645f 6c69 7374 7208 0000  attened_listr...
+00000760: 0072 0800 0000 720c 0000 00da 1d66 6c61  .r....r......fla
+00000770: 7474 656e 5f6d 756c 7469 6469 6d65 6e73  tten_multidimens
+00000780: 696f 6e61 6c5f 6c69 7374 3500 0000 7308  ional_list5...s.
+00000790: 0000 0000 0712 010e 0104 0272 1b00 0000  ...........r....
+000007a0: 4e29 0dda 075f 5f64 6f63 5f5f da0a 5f5f  N)...__doc__..__
+000007b0: 6175 7468 6f72 5f5f da08 5f5f 6461 7465  author__..__date
+000007c0: 5f5f da0a 5f5f 7374 6174 7573 5f5f da0b  __..__status__..
+000007d0: 5f5f 6c69 6365 6e73 655f 5fda 0d5f 5f63  __license__..__c
+000007e0: 6f70 7972 6967 6874 5f5f da06 7479 7069  opyright__..typi
+000007f0: 6e67 7204 0000 0072 0500 0000 720f 0000  ngr....r....r...
+00000800: 00da 0373 7472 7214 0000 0072 1b00 0000  ...strr....r....
+00000810: 7208 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
+00000820: 0c00 0000 da08 3c6d 6f64 756c 653e 0300  ......<module>..
+00000830: 0000 7312 0000 0004 0304 0104 0104 0104  ..s.............
+00000840: 0104 1310 0210 0c10 0a                   .........
```

### Comparing `wordhoard-1.5.4/wordhoard/utilities/__pycache__/deep_translator.cpython-39.pyc` & `wordhoard-1.5.5/wordhoard/utilities/__pycache__/deep_translator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.4/wordhoard/utilities/__pycache__/email_address_verification.cpython-39.pyc` & `wordhoard-1.5.5/wordhoard/utilities/__pycache__/email_address_verification.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.4/wordhoard/utilities/__pycache__/exceptions.cpython-39.pyc` & `wordhoard-1.5.5/wordhoard/utilities/__pycache__/exceptions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.4/wordhoard/utilities/__pycache__/google_translator.cpython-39.pyc` & `wordhoard-1.5.5/wordhoard/utilities/__pycache__/google_translator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.4/wordhoard/utilities/__pycache__/mymemory_translator.cpython-39.pyc` & `wordhoard-1.5.5/wordhoard/utilities/__pycache__/mymemory_translator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.4/wordhoard/utilities/__pycache__/translator_languages.cpython-39.pyc` & `wordhoard-1.5.5/wordhoard/utilities/__pycache__/translator_languages.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.4/wordhoard/utilities/captcha_checker.py` & `wordhoard-1.5.5/wordhoard/utilities/captcha_checker.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,21 +27,24 @@
 # Date Revised: February 25, 2023
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
-import bs4
+# Standard library imports
 import logging
 
+# Third-party imports
+import bs4
+
 logger = logging.getLogger(__name__)
 
 
-class CaptchaVerification(object):
+class CaptchaVerification:
     """
     This Class is used to query a webpage to determine if it is protected by a captcha.
     """
 
     def __init__(self, url, soup):
         self._url: str = url
         self._raw_soup: bs4.BeautifulSoup = soup
@@ -81,21 +84,19 @@
         """
         This function is designed to query for the existence
         of specific captcha related text contained in an H2 tag.
 
         :return: True or False
         :rtype: boolean
         """
-        captcha_protected_h2_tag = bool(self._raw_soup.find(name='h2', attrs={'class': 'main__heading'}))
-        if captcha_protected_h2_tag is True:
+        captcha_protected_tag = bool(self._raw_soup.find(name='h2', attrs={'class': 'main__heading'}))
+        if captcha_protected_tag:
             captcha_protected_tag = self._raw_soup.find(name='h2', attrs={'class': 'main__heading'})
-            if "We've detected unusual activity from your computer network" in captcha_protected_tag.text:
-                return True
-            else:
-                return False
+            return  "We've detected unusual activity from your computer network" in captcha_protected_tag.text
+        return False
 
     def captcha_protected_url(self)  -> bool:
         """
         This function is designed to query specific elements, which
         will determine if a webpage is protected by a captcha.
 
         :return: True or False
@@ -106,11 +107,8 @@
             return True
         elif div_tag_bool is False:
             title_tag_bool = self._check_title_tag()
             if title_tag_bool is True:
                 return True
             else:
                 h2_tag_bool = self._check_h2_tag()
-                if h2_tag_bool is True:
-                    return True
-                else:
-                    return False
+                return bool(h2_tag_bool)
```

### Comparing `wordhoard-1.5.4/wordhoard/utilities/cleansing.py` & `wordhoard-1.5.5/wordhoard/utilities/cleansing.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,8 +58,7 @@
     :rtype: list
     """
     if any(isinstance(i, List) for i in list_of_lists):
         flattened_list = [element for sub_list in list_of_lists for element in sub_list]
         return flattened_list
     else:
         return list_of_lists
-
```

### Comparing `wordhoard-1.5.4/wordhoard/utilities/cloudflare_checker.py` & `wordhoard-1.5.5/wordhoard/utilities/cloudflare_checker.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Date Completed: January 08, 2022
 # Author: John Bumgarner
 #
-# Date Revised: February 25, 2023
+# Date Revised: May 25, 2024
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
 from bs4 import BeautifulSoup
 
-class CloudflareVerification(object):
+class CloudflareVerification:
     """
     This Class is used to query a webpage to determine if it is protected by
     Cloudflare's DDoS mitigation services.
     """
 
     def __init__(self, url, soup):
         self._url: str = url
@@ -48,57 +48,52 @@
         This function is designed to query for the existence
         of specific tag known to be commonly related to a
         Cloudflare protected webpage.
 
         :return: True or False
         :rtype: boolean
         """
-        if self._raw_soup.find(name='p', attrs={'data-translate': 'why_captcha_detail'}):
-            p_tag = self._raw_soup.find(name='p', attrs={'data-translate': 'why_captcha_detail'})
-            if p_tag.text == 'Completing the CAPTCHA proves you are a human and gives you temporary access to ' \
-                             'the web property.':
-                return True
-            else:
-                return False
+        p_tag = self._raw_soup.find(name='p', attrs={'data-translate': 'why_captcha_detail'})
+        return bool(p_tag and p_tag.text == 'Completing the CAPTCHA proves you are a human and gives you temporary access to the web property.')
 
     def _check_div_tag(self) -> bool:
-        if self._raw_soup.find(name='div', attrs={'id': 'challenge-body-text'}):
-            return True
-        else:
-            return False
+        """
+        This function is designed to query for the existence
+        of a specific div tag with the id 'challenge-body-text'.
+
+        :return: True or False
+        :rtype: boolean
+        """
+        return bool(self._raw_soup.find(name='div', attrs={'id': 'challenge-body-text'}))
 
     def _check_title_tag(self) -> bool:
         """
         This function is designed to query for the existence
         of specific Cloudflare related text contained in a title tag.
 
         :return: True or False
         :rtype: boolean
         """
         title_tag = self._raw_soup.find(name='title')
-        try:
-            if 'Please Wait... | Cloudflare' in title_tag.text or 'Just a moment...' in title_tag.text:
-                return True
-            else:
-                return False
-        except AttributeError:
-            pass
+        return bool(
+                title_tag and (
+                    'Please Wait... | Cloudflare' in title_tag.text or
+                    'Just a moment...' in title_tag.text or
+                    'Attention Required! | Cloudflare' in title_tag.text)
+                    )
 
     def _check_meta_tag(self) -> bool:
         """
         This function is designed to query for the existence
         of specific Cloudflare related meta tag.
 
         :return: True or False
         :rtype: boolean
         """
-        if self._raw_soup.find(name='meta', attrs={'id': 'captcha-bypass'}):
-            return True
-        else:
-            return False
+        return bool(self._raw_soup.find(name='meta', attrs={'id': 'captcha-bypass'}))
 
     def cloudflare_protected_url(self) -> bool:
         """
         This function is designed to query specific elements, which
         will determine if a webpage is protected by Cloudflare's
         DDoS mitigation services.
```

### Comparing `wordhoard-1.5.4/wordhoard/utilities/colorized_text.py` & `wordhoard-1.5.5/wordhoard/utilities/colorized_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,9 +39,7 @@
         print(f'\033[1;31m{text}{RESET}')
     elif color == 'blue':
         print(f'\033[1;34m{text}{RESET}')
     elif color == 'green':
         print(f'\033[1;32m{text}{RESET}')
     elif color == 'magenta':
         print(f'\033[1;35m{text}{RESET}')
-
-
```

### Comparing `wordhoard-1.5.4/wordhoard/utilities/deep_translator.py` & `wordhoard-1.5.5/wordhoard/utilities/deep_translator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 """
-This Python script is used to translate a specific word from it source language,
+This Python module is used to translate a specific word from it source language,
 such as Spanish into American English using the Deep Translation service.
 """
 __author__ = 'John Bumgarner'
 __date__ = 'September 24, 2021'
 __status__ = 'Production'
 __license__ = 'MIT'
 __copyright__ = "Copyright (C) 2021 John Bumgarner"
@@ -20,94 +20,206 @@
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Date Completed: September 24, 2021
 # Author: John Bumgarner
 #
-# Date Last Revised: May 31, 2023
+# Date Last Revised: May 12, 2024
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
-import deepl
+# Standard library imports
+import ast
 import logging
 import traceback
 from typing import Union
+
+# Third-party imports
+import deepl
 from backoff import on_exception, expo
 from ratelimit import limits, RateLimitException
 from deepl.exceptions import AuthorizationException
 from deepl.exceptions import QuotaExceededException
 from deepl.exceptions import TooManyRequestsException
+
+# Local or project-specific imports
 from wordhoard.utilities.colorized_text import colorized_text
 from wordhoard.utilities.translator_languages import Languages
 from wordhoard.utilities.exceptions import LanguageNotSupportedException
 
 logger = logging.getLogger(__name__)
 
 
-class Translator(object):
-
+class Translator:
+    """
+        This class handles translation operations using the DeepL translation service. It supports translating words
+        from one language to another, handling rate limits, and dealing with various exceptions that may occur during
+        translation requests.
+
+        Args:
+            source_language (str): The source language for translation. Defaults to an empty string.
+            str_to_translate (str): The text to translate. Defaults to an empty string.
+            api_key (str): The API key for accessing the DeepL translation service. Defaults to an empty string.
+
+        Attributes:
+            _source_language (str): The source language for translation.
+            _str_to_translate (str): The text to translate.
+            _api_key (str): The API key for accessing the DeepL translation service.
+            _rate_limit_status (bool): A flag indicating the rate limit status for translation requests.
+
+        Methods:
+            __init__: Initializes the Translator object with source language, text to translate, and API key.
+            _backoff_handler: Handles rate limit exceeded situations by logging and setting rate_limit_status.
+            _deep_supported_languages: Checks if the source language is supported by DeepL translation service.
+            _handle_standard_exceptions: Handles standard exceptions like TypeError and ValueError during translation.
+            _handle_custom_exceptions: Handles custom exceptions specific to DeepL translation service.
+            _deep_translate: Translates text from the source language to American English using DeepL service.
+            _deep_translate_reverse: Translates text from American English to the source language using DeepL service.
+            translate_word: Translates text from the source language to American English, handling unsupported languages.
+            reverse_translate: Translates text from American English to the source language.
+
+        Note:
+            This class relies on the `deepl` module for translation functionality. Ensure that the module is installed
+            and configured correctly for translation operations.
+        """
     def __init__(self,
                  source_language: str = '',
                  str_to_translate: str = '',
+                 max_number_of_requests: int = 30,
+                 rate_limit_timeout_period: int = 60,
                  api_key: str = ''
                  ):
 
         self._source_language = source_language
         self._str_to_translate = str_to_translate
         self._api_key = api_key
 
         ratelimit_status = False
         self._rate_limit_status = ratelimit_status
 
         # Retries the requests after a certain time period has elapsed
-        handler = on_exception(expo, RateLimitException, max_time=60, on_backoff=self._backoff_handler)
+        handler = on_exception(wait_gen=expo,
+                               exception=RateLimitException,
+                               max_time=60,
+                               on_backoff=self._backoff_handler)
         # Establishes a rate limit for making requests to the Deep translation service
-        limiter = limits(calls=60, period=60)
+        limiter = limits(calls=max_number_of_requests, period=rate_limit_timeout_period)
         self.translate_word = handler(limiter(self.translate_word))
         self.reverse_translate = handler(limiter(self.reverse_translate))
 
-    def _backoff_handler(self):
+    def _backoff_handler(self, details) -> None:
+        """
+        Handles the backoff mechanism when the rate limit for querying the Deep translation service is reached.
+
+        This method is triggered when the rate limit is encountered. It logs the rate limit event and displays
+        colorized messages indicating that the process is entering a temporary hibernation mode. If the rate
+        limit has already been reached, it continues to display colorized backoff messages for subsequent
+        retries.
+
+        :param details: A dictionary containing information about the backoff event, including:
+                        - 'wait' (float): The number of seconds to wait before retrying.
+                        - 'tries' (int): The number of retry attempts made so far.
+                        - Additional details such as 'target', 'args', 'kwargs', 'elapsed', and 'exception' which provide
+                          context about the event (not used in this method but part of the details dictionary).
+
+        type details: Dict
+
+        Side Effects:
+        - Displays colorized text messages to indicate the backoff status.
+        - Logs an info message when the rate limit is initially reached.
+        - Sets the `_rate_limit_status` attribute to True when the rate limit is first encountered.
+
+        :returns: None
+        :rtype: NoneType
+        """
         if self._rate_limit_status is False:
-            colorized_text('The Deep translation service query rate Limit was reached. The querying '
-                           'process is entering a temporary hibernation mode.', 'red')
+            colorized_text(text='The Deep translation service query rate limit was reached. '
+                                'The querying process is entering a temporary hibernation mode.', color='red')
+            colorized_text(text=f"Backing off {details['wait']:.1f} seconds afters {details['tries']} tries.",
+                           color='blue')
             logger.info('The Deep translation service query rate limit was reached.')
             self._rate_limit_status = True
+        elif self._rate_limit_status is True:
+            colorized_text(text=f"Backing off {details['wait']:.1f} seconds afters {details['tries']} tries.",
+                           color='blue')
 
     def _deep_supported_languages(self) -> Union[str, None]:
         """
         This function determines if the requested source language is
         one of the supported languages for the Deep translation service.
 
         :return: language
         :rtype: string
         """
         languages = Languages()
         deep_languages = languages.deep_supported_languages()
-        supported_languages = eval(str(deep_languages))
+        deep_languages_str = str(deep_languages)
+        supported_languages = ast.literal_eval(deep_languages_str)
         try:
             if self._source_language in supported_languages.keys():
                 return self._source_language
             elif self._source_language in supported_languages.values():
                 return self._source_language
             else:
                 return None
-
         except LanguageNotSupportedException as error:
-            """
-            An exception is thrown if the user uses a language that is not supported by the Deep Translation service.
-            """
-            logger.info(f'The language provided is not one of the supported languages for the Deep Translation '
-                        f'service.')
+            logger.info('The language provided is not one of the supported languages for the Deep Translation service.')
             logger.info(f'Requested language: {self._source_language}')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
+    def _handle_standard_exceptions(self, error):
+        """
+            Helper method to handle standard exceptions
+        """
+        if isinstance(error, TypeError):
+            logger.error(f'A TypeError occurred when attempting to translate the word {self._str_to_translate}')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        elif isinstance(error, ValueError):
+            if str(error) == "auth_key must not be empty":
+                colorized_text(text='An Authorization failure has occurred when using the Deep translation service.  '
+                                    'Please verify your authentication key', color='red')
+                logger.error('An Authorization key cannot be empty when using the Deep translation service.')
+                logger.error(''.join(traceback.format_tb(error.__traceback__)))
+            elif str(error) == 'text must not be empty':
+                colorized_text(text='An empty string was passed to the Deep translation service.', color='red')
+                logger.error('An empty string was passed to the Deep translation service.')
+                logger.error(''.join(traceback.format_tb(error.__traceback__)))
+            else:
+                logger.error(f'An unknown ValueError occurred when attempting to translate the word'
+                             f' {self._str_to_translate}')
+                logger.error(''.join(traceback.format_tb(error.__traceback__)))
+
+    @staticmethod
+    def _handle_custom_exceptions(error):
+        """
+        Helper method to handle custom exceptions
+        """
+        if isinstance(error, AuthorizationException):
+            colorized_text(text='The authentication key used for Deep Translation service is invalid.\nPlease verify '
+                                'that the authentication key used is valid.', color='red')
+            logger.error('Authorization Error:')
+            logger.error('An authorization error has occurred when using the Deep Translation service.')
+            logger.error('Please verify that the authentication key used is valid.')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        elif isinstance(error, QuotaExceededException):
+            colorized_text(text='The quota for the Deep Translation service for this billing period has '
+                                'been exceeded.', color='red')
+            logger.error('The quota for the the Deep Translation service for this billing period has been exceeded.')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        elif isinstance(error, TooManyRequestsException):
+            colorized_text(text='There has been too many connection requests to the Deep Translation service.',
+                           color='red')
+            logger.error('Connection Request Error:')
+            logger.error('There has been too many connection requests to the Deep Translation service.')
+            logger.error(''.join(traceback.format_tb(error.__traceback__)))
+
     def _deep_translate(self, original_language: str) -> str:
         """
         This function is used to translate a word from it source language, such as Spanish
         into American English.
 
         :param original_language: language to translated from
         :return: translated word
@@ -117,159 +229,56 @@
             translator = deepl.Translator(auth_key=self._api_key)
             result = translator.translate_text(self._str_to_translate,
                                                target_lang='EN-US',
                                                source_lang=original_language)
 
             translated_text = result.text
             return translated_text
-
-        except AuthorizationException as error:
-            """
-            The exception is thrown when the authentication key is not valid for the Deep Translation service.
-            """
-            colorized_text('The authentication key used for Deep Translation service is invalid.\nPlease verify '
-                           'that the authentication key used is valid.', 'red')
-            logger.error('Authorization Error:')
-            logger.error('An authorization error has occurred when using the Deep Translation service.')
-            logger.error('Please verify that the authentication key used is valid.')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-
-        except QuotaExceededException as error:
-            """
-            The exception is thrown when the translation quota for this billing period has been exceeded.
-            """
-            colorized_text('The quota for the Deep Translation service for this billing period has '
-                           'been exceeded.', 'red')
-            logger.error('The quota for the the Deep Translation service for this billing period has been exceeded.')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-
-        except TooManyRequestsException as error:
-            """
-            This exception is thrown when the maximum number of connection requests have been exceeded for a 
-            specific time for the Deep Translation service.
-            """
-            colorized_text('There has been too many connection requests to the Deep Translation service.', 'red')
-            logger.error('Connection Request Error:')
-            logger.error('There has been too many connection requests to the Deep Translation service.')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-
-        except TypeError as error:
-            """
-            The exception is thrown when an operation or function is applied to an object of inappropriate type.
-            """
-            logger.error(f'A TypeError occurred when attempting to translate the word {self._str_to_translate}')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-
-        except ValueError as error:
-            """
-            The exception is thrown when an operation or function receives an argument that 
-            has the right type but an inappropriate value.
-            """
-            if str(error) == "auth_key must not be empty":
-                colorized_text('An Authorization failure has occurred when using the Deep translation service.  '
-                               'Please verify your authentication key', 'red')
-                logger.error('An Authorization key cannot be empty when using the Deep translation service.')
-                logger.error(''.join(traceback.format_tb(error.__traceback__)))
-            elif str(error) == 'text must not be empty':
-                colorized_text('An empty string was passed to the Deep translation service.', 'red')
-                logger.error('An empty string was passed to the Deep translation service.')
-                logger.error(''.join(traceback.format_tb(error.__traceback__)))
-            else:
-                logger.error(f'An unknown ValueError occurred when attempting to translate the word'
-                             f' {self._str_to_translate}')
-                logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        except (AuthorizationException, QuotaExceededException, TooManyRequestsException) as error:
+            self._handle_custom_exceptions(error)
+        except (TypeError, ValueError) as error:
+            self._handle_standard_exceptions(error)
 
     def _deep_translate_reverse(self) -> str:
         """
         This function is used to translate a word from it source language, such as Spanish into American English.
 
         :return: translated word
         :rtype: string
         """
         try:
             translator = deepl.Translator(auth_key=self._api_key)
-            result = translator.translate_text(self._str_to_translate,
+            result = translator.translate_text(text=self._str_to_translate,
                                                target_lang=self._source_language,
                                                source_lang='EN')
             translated_text = result.text
             return translated_text
 
-        except AuthorizationException as error:
-            """
-            The exception is thrown when the authentication key is not valid for the Deep Translation service.
-            """
-            colorized_text('The authentication key used for Deep Translation service is invalid.\nPlease verify '
-                           'that the authentication key used is valid.', 'red')
-            logger.error('Authorization Error:')
-            logger.error('An authorization error has occurred when using the Deep Translation service.')
-            logger.error('Please verify that the authentication key used is valid.')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-
-        except QuotaExceededException as error:
-            """
-            The exception is thrown when the translation quota for this billing period has been exceeded.
-            """
-            colorized_text('The quota for the Deep Translation service for this billing period has '
-                           'been exceeded.', 'red')
-            logger.error('The quota for the Deep Translation service for this billing period has been exceeded.')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-
-        except TooManyRequestsException as error:
-            """
-            This exception is thrown when the maximum number of connection requests have been exceeded for a 
-            specific time for the Deep Translation service.
-            """
-            colorized_text('There has been too many connection requests to the Deep Translation service.', 'red')
-            logger.error('Connection Request Error:')
-            logger.error('There has been too many connection requests to the Deep Translation service.')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-
-        except TypeError as error:
-            """
-            The exception is thrown when an operation or function is applied to an object of inappropriate type.
-            """
-            logger.error(f'A TypeError occurred when attempting to translate the word {self._str_to_translate}')
-            logger.error(''.join(traceback.format_tb(error.__traceback__)))
-
-        except ValueError as error:
-            """
-            The exception is thrown when an operation or function receives an argument that 
-            has the right type but an inappropriate value.
-            """
-            if str(error) == "auth_key must not be empty":
-                colorized_text('An Authorization failure has occurred when using the Deep Translation service.\n'
-                               'Please verify your authentication key', 'red')
-                logger.error('An Authorization key cannot be empty when using the Deep Translation service.')
-                logger.error(''.join(traceback.format_tb(error.__traceback__)))
-            elif str(error) == 'text must not be empty':
-                colorized_text('An empty string was passed to the Deep Translation service.', 'red')
-                logger.error('An empty string was passed to the Deep translation service.')
-                logger.error(''.join(traceback.format_tb(error.__traceback__)))
-            else:
-                logger.error(f'An unknown ValueError occurred when attempting to translate the word'
-                             f' {self._str_to_translate}')
-                logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        except (AuthorizationException, QuotaExceededException, TooManyRequestsException) as error:
+            self._handle_custom_exceptions(error)
+        except (TypeError, ValueError) as error:
+            self._handle_standard_exceptions(error)
 
     def translate_word(self) -> Union[str, None]:
         """
         This function is used to translate a word from it source language, such as Spanish into American English.
 
         :return: translated word
         :rtype: string
         """
         supported_language = self._deep_supported_languages()
         if supported_language:
             return self._deep_translate(supported_language)
         elif not supported_language:
-            colorized_text(f'The language provided is not one of the supported languages for the '
-                           f'Deep Translation service.', 'red')
-            colorized_text(f'Requested language: {self._source_language}', 'red')
-            colorized_text(f'Please review the languages supported by the Deep Translate service\n'
-                           f'https://wordhoard.readthedocs.io/en/latest/translations'
-                           f'/deepl_supported_translation_languages/', 'green')
+            colorized_text(text='The language provided is not one of the supported languages for the Deep Translation service.',
+                           color='red')
+            colorized_text(text=f'Requested language: {self._source_language}', color='red')
+            colorized_text(text='Please review the languages supported by the Deep Translate service\n'
+                           'https://wordhoard.readthedocs.io/en/latest/translations'
+                           '/deepl_supported_translation_languages/', color='green')
             return None
 
     def reverse_translate(self) -> str:
         """
         This function is used to translate a word from American English into another language, such as Spanish.
 
         :return: translated word
```

### Comparing `wordhoard-1.5.4/wordhoard/utilities/email_address_verification.py` & `wordhoard-1.5.5/wordhoard/utilities/email_address_verification.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Date Completed: February 09, 2023
 # Author: John Bumgarner
 #
-# Date Last Revised: February 19, 2023
+# Date Last Revised: May 12, 2024
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
 import re as regex
@@ -36,11 +36,9 @@
     """
     This function is designed to validate the format of email address provided by
     an end user.
 
     :param email_address: input string
     :return: boolean
     """
-    if regex.fullmatch(r'([A-Za-z0-9]+[.-_])*[A-Za-z0-9]+@[A-Za-z0-9-]+(\.[A-Z|a-z]{2,})+', email_address):
-        return True
-    else:
-        return False
+    return bool(regex.fullmatch(pattern=r'([A-Za-z0-9]+[.-_])*[A-Za-z0-9]+@[A-Za-z0-9-]+(\.[A-Z|a-z]{2,})+', string=email_address))
+
```

### Comparing `wordhoard-1.5.4/wordhoard/utilities/exceptions.py` & `wordhoard-1.5.5/wordhoard/utilities/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,54 +29,41 @@
 
 
 class ElementNotFoundException(Exception):
     """
     The exception is thrown if the requested HTML element was not found in the body element being
     parsed by BeautifulSoup.
     """
-    pass
-
 
 class InvalidEmailAddressException(Exception):
     """
     This exception is thrown when the email address provided for authentication to the MyMemory Translation
     service is invalid.
     """
-    pass
-
 
 class InvalidLengthException(Exception):
     """
     This exception is thrown if the provided text exceed the length limit of the the Translator service being used.
     """
-    pass
-
 
 class LanguageNotSupportedException(Exception):
     """
     This exception is thrown when the requested langauge is not supported by the Translator service being used.
     """
-    pass
-
 
 class QuotaExceededException(Exception):
     """
     This exception is thrown when the translation quota for a specific time period for the Translator service
     being used has been exceeded.
     """
-    pass
-
 
 class TooManyRequestsException(Exception):
     """
     This exception is thrown when the maximum number of connection requests have been exceeded for a specific time
     period for the Translator service being used.
     """
-    pass
-
 
 class RequestException(Exception):
     """
     This exception is thrown when an ambiguous exception occurs during a connection to the Translator service
     being used.
     """
-    pass
```

### Comparing `wordhoard-1.5.4/wordhoard/utilities/translator_languages.py` & `wordhoard-1.5.5/wordhoard/utilities/translator_languages.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,32 +20,40 @@
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Date Completed: February 12, 2023
 # Author: John Bumgarner
 #
-# Date Last Revised: February 28, 2023
+# Date Last Revised: May 24, 2024
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
 from typing import Dict
 
 class Languages:
+    """
+        This class provides static methods to retrieve supported languages for different translation services.
+
+        Methods:
+            - deep_supported_languages: Retrieves the supported languages for the Deep Translation service.
+            - google_supported_languages: Retrieves the supported languages for the Google Translation service.
+            - mymemory_supported_languages: Retrieves the supported languages for the MyMemory Translation service.
+    """
 
     @staticmethod
     def deep_supported_languages() -> Dict[str, str]:
         """
         This function returns the supported languages for the Deep Translation service.
 
         :return: languages
-        :rtype: string
+        :rtype: dict
         """
         # Deep Translator supported languages listed in as of 02-04-2023
         supported_languages = {'bg': 'bulgarian',
                                'zh': 'chinese',
                                'cs': 'czech',
                                'da': 'danish',
                                'nl': 'dutch',
@@ -78,15 +86,15 @@
 
     @staticmethod
     def google_supported_languages() -> Dict[str, str]:
         """
         This function returns the supported languages for the Google Translation service.
 
         :return: languages
-        :rtype: string
+        :rtype: dict
         """
         # Google Translator supported languages listed as of 02-10-2023
         supported_languages = {'af': 'afrikaans',
                                'sq': 'albanian',
                                'am': 'amharic',
                                'ar': 'arabic',
                                'hy': 'armenian',
@@ -224,15 +232,15 @@
 
     @staticmethod
     def mymemory_supported_languages() -> Dict[str, str]:
         """
         This function returns the supported languages for the MyMemory Translation service.
 
         :return: languages
-        :rtype: string
+        :rtype: dict
         """
         # MyMemory Translator supported languages as of 02-09-2023
         supported_languages = {'af': 'afrikaans',
                                'sq': 'albanian',
                                'am': 'amharic',
                                'ar': 'arabic',
                                'hy': 'armenian',
```

### Comparing `wordhoard-1.5.4/wordhoard/utilities/user_agents.py` & `wordhoard-1.5.5/wordhoard/utilities/user_agents.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 """
-This Python script obtains a random user agent from a pre-built dictionary.
+This Python module obtains a random user agent from a pre-built dictionary.
 """
 __author__ = 'John Bumgarner'
 __date__ = 'September 12, 2021'
 __status__ = 'Production'
 __license__ = 'MIT'
 __copyright__ = "Copyright (C) 2021 John Bumgarner"
 
@@ -19,15 +19,15 @@
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Date Completed: September 12, 2021
 # Author: John Bumgarner
 #
-# Date Last Revised: March 04, 2023
+# Date Last Revised: May 12, 2024
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
 import os
@@ -45,43 +45,54 @@
 
 ######################################################################
 # Array of common user agents to use for the HTTP connection
 # source:  http://http://www.useragentstring.com
 # source:  https://deviceatlas.com/blog/list-of-user-agent-strings
 # source:  https://developers.whatismybrowser.com/useragents/explore
 ########################################################################
-try:
-    _common_user_agents = os.path.join(BASE_DIR, 'files/common_user_agents.pkl')
-    with open(_common_user_agents, 'rb') as _infile:
-        _user_agents_list = pickle.load(_infile)
-        _infile.close()
-except FileNotFoundError as error:
-    logger.error('The common_user_agents.pkl file was not found. Aborting operation.')
-    logger.error(''.join(traceback.format_tb(error.__traceback__)))
-    sys.exit(1)
-except OSError as error:
-    logger.error(f"An OS error occurred when trying to open the file common_user_agents.pkl")
-    logger.error(''.join(traceback.format_tb(error.__traceback__)))
-    sys.exit(1)
 
+def _unpickle_user_agents():
+    """
+    Load user agents from a pickle file.
+
+    This function attempts to load user agents from the common_user_agents.pkl file located
+    in the 'files' directory under BASE_DIR. If successful, it returns a dictionary containing
+    the user agents. If the file is not found or an OS error occurs during loading, the function
+    logs the error using the logger and exits the program with an error code.
+
+    :return: A dictionary containing user agents if loaded successfully.
+    :rtype: dict
+    """
+    try:
+        _common_user_agents = os.path.join(BASE_DIR, 'files/common_user_agents.pkl')
+        with open(file=_common_user_agents, mode='rb') as _infile:
+            user_agents_list = pickle.load(_infile)
+            return user_agents_list
+    except FileNotFoundError as error:
+        logger.error('The common_user_agents.pkl file was not found. Aborting operation.')
+        logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        sys.exit(1)
+    except OSError as error:
+        logger.error("An OS error occurred when trying to open the file common_user_agents.pkl")
+        logger.error(''.join(traceback.format_tb(error.__traceback__)))
+        sys.exit(1)
 
 def get_random_user_agent() -> str:
     """
     This function obtains a random user agent from a
     dictionary of available agents.
 
     :return: random user agent
     :rtype: string
     """
-    global _user_agents_list
-    random_key = random.choice(list(_user_agents_list.keys()))
-    random_value = random.choice(list(_user_agents_list[random_key]))
+    user_agents_list = _unpickle_user_agents()
+    random_key = random.choice(list(user_agents_list.keys()))
+    random_value = random.choice(list(user_agents_list[random_key]))
     return random_value
 
-
 def get_specific_user_agent(requested_key: str) -> Union[str, None]:
     """
     This function obtains a specific user agent type from a
     dictionary of available agents. The available agents types
     are listed below:
 
     - android
@@ -101,14 +112,15 @@
     user_agent_keys = {'chrome macOS': 'chrome_mac_os_x', 'chrome windows': 'chrome_windows_10',
                        'firefox macOS': 'firefox_mac_os_x', 'firefox windows': 'firefox_windows_10',
                        'safari macOS': 'safari_mac_os_x', 'safari iphone': 'safari_iphone',
                        'safari ipad': 'safari_ipad', 'android': 'samsung_browser_android'}
 
     if bool([v for k, v in user_agent_keys.items() if k == requested_key]):
         key = ''.join([v for k, v in user_agent_keys.items() if k == requested_key])
-        global _user_agents_list
-        random_value = random.choice(list(_user_agents_list[key]))
+        user_agents_list = _unpickle_user_agents()
+        random_value = random.choice(list(user_agents_list[key]))
+        print(random_value)
         return random_value
     else:
         logger.error('The requested user agent was not found in the list of available agents.')
         logger.info(f'Agent requested: {requested_key}')
         return None
```

### Comparing `wordhoard-1.5.4/wordhoard/utilities/word_verification.py` & `wordhoard-1.5.5/wordhoard/utilities/word_verification.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,12 +44,9 @@
 
     :param word: string to validate
     :return: boolean true or false
     """
     if len(word) == 0:
         return False
     else:
-        temp = regex.match(r'^[a-zA-Z-\s]*$', word.strip())
-        if temp:
-            return True
-        else:
-            return False
+        temp = regex.match(pattern=r'^[a-zA-Z-\s]*$', string=word.strip())
+        return bool(temp)
```

### Comparing `wordhoard-1.5.4/wordhoard.egg-info/PKG-INFO` & `wordhoard-1.5.5/wordhoard.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 Metadata-Version: 2.1
 Name: wordhoard
-Version: 1.5.4
+Version: 1.5.5
 Summary: A comprehensive lexical discovery application that is useful for finding semantic relationships such as, the antonyms, synonyms, hypernyms, hyponyms, homophones and definitions for a specific word.
 Home-page: https://github.com/johnbumgarner/wordhoard
 Author: John Bumgarner
 Author-email: wordhoardproject@gmail.com
 License: LICENSE.txt
 Keywords: antonyms,bag of words,definitions,hypernyms,hyponyms,homophones,information retrieval,lexicon,semantic relationships,synonyms,natural language processing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Processing :: General
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: backoff>=2.2.1
+Requires-Dist: beautifulsoup4>=4.12.3
+Requires-Dist: certifi>=2024.2.2
+Requires-Dist: charset-normalizer>=3.3.2
+Requires-Dist: cloudscraper>=1.2.71
+Requires-Dist: deckar01-ratelimit>=3.0.2
+Requires-Dist: deepl>=1.18.0
+Requires-Dist: idna>=3.7
+Requires-Dist: lxml>=5.2.2
+Requires-Dist: pyparsing>=3.1.2
+Requires-Dist: requests>=2.32.2
+Requires-Dist: requests-toolbelt>=1.0.0
+Requires-Dist: soupsieve>=2.5
+Requires-Dist: urllib3>=2.2.1
 
 # Primary Use Case
 <p align="justify"> 
 Textual analysis is a broad term for various research methodologies used to qualitatively describe, interpret and understand text data. These methodologies are mainly used in academic research to analyze content related to media and communication studies, popular culture, sociology, and philosophy. Textual analysis allows these researchers to quickly obtain relevant insights from unstructured data. All types of information can be gleaned from textual data, especially from social media posts or news articles. Some of this information includes the overall concept of the subtext, symbolism within the text, assumptions being made and potential relative value to a subject (e.g. data science). In some cases it is possible to deduce the relative historical and cultural context of a body of text using analysis techniques coupled with knowledge from different disciplines, like linguistics and semiotics.
    
 Word frequency is the technique used in textual analysis to measure the frequency of a specific word or word grouping within unstructured data. Measuring the number of word occurrences in a corpus allows a researcher to garner interesting insights about the text. A subset of word frequency is the correlation between a given word and that word's relationship to either antonyms and synonyms within the specific corpus being analyzed. Knowing these relationships is critical to improving word frequencies and topic modeling.
 
@@ -113,9 +124,9 @@
 The MIT License (MIT).  Please see <a href="https://wordhoard.readthedocs.io/en/latest/license" target="_blank">License File</a> for more information.
 </p>
 
 
 # Author
 
 <p align="justify">
-   Copyright (c) 2020 John Bumgarner 
+   Copyright (c) 2021 John Bumgarner 
 </p>
```

#### html2text {}

```diff
@@ -1,26 +1,30 @@
-Metadata-Version: 2.1 Name: wordhoard Version: 1.5.4 Summary: A comprehensive
+Metadata-Version: 2.1 Name: wordhoard Version: 1.5.5 Summary: A comprehensive
 lexical discovery application that is useful for finding semantic relationships
 such as, the antonyms, synonyms, hypernyms, hyponyms, homophones and
 definitions for a specific word. Home-page: https://github.com/johnbumgarner/
 wordhoard Author: John Bumgarner Author-email: wordhoardproject@gmail.com
 License: LICENSE.txt Keywords: antonyms,bag of
 words,definitions,hypernyms,hyponyms,homophones,information
 retrieval,lexicon,semantic relationships,synonyms,natural language processing
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Topic :: Text Processing
-:: General Classifier: Topic :: Text Processing :: Linguistic Classifier: Topic
-:: Utilities Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE # Primary Use Case
+Independent Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Text Processing :: Linguistic Classifier: Topic ::
+Utilities Requires-Python: >=3.8 Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: backoff>=2.2.1 Requires-Dist:
+beautifulsoup4>=4.12.3 Requires-Dist: certifi>=2024.2.2 Requires-Dist: charset-
+normalizer>=3.3.2 Requires-Dist: cloudscraper>=1.2.71 Requires-Dist: deckar01-
+ratelimit>=3.0.2 Requires-Dist: deepl>=1.18.0 Requires-Dist: idna>=3.7
+Requires-Dist: lxml>=5.2.2 Requires-Dist: pyparsing>=3.1.2 Requires-Dist:
+requests>=2.32.2 Requires-Dist: requests-toolbelt>=1.0.0 Requires-Dist:
+soupsieve>=2.5 Requires-Dist: urllib3>=2.2.1 # Primary Use Case
 Textual analysis is a broad term for various research methodologies used to
 qualitatively describe, interpret and understand text data. These methodologies
 are mainly used in academic research to analyze content related to media and
 communication studies, popular culture, sociology, and philosophy. Textual
 analysis allows these researchers to quickly obtain relevant insights from
 unstructured data. All types of information can be gleaned from textual data,
 especially from social media posts or news articles. Some of this information
@@ -64,8 +68,8 @@
 [GitHub]%20wordhoard%20project%20request) with any issues or enhancement
 requests.
 # Sponsorship If you would like to contribute financially to the development
 and maintenance of the WWoorrddhhooaarrdd project please read the _s_p_o_n_s_o_r_s_h_i_p
 _i_n_f_o_r_m_a_t_i_o_n. # License
 The MIT License (MIT). Please see _L_i_c_e_n_s_e_ _F_i_l_e for more information.
 # Author
-Copyright (c) 2020 John Bumgarner
+Copyright (c) 2021 John Bumgarner
```

### Comparing `wordhoard-1.5.4/wordhoard.egg-info/SOURCES.txt` & `wordhoard-1.5.5/wordhoard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

