# Comparing `tmp/jupyterlite_terminal-0.0.0a0.tar.gz` & `tmp/jupyterlite_terminal-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlite_terminal-0.0.0a0.tar", last modified: Wed May 29 16:10:59 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlite_terminal-0.0.0a0.tar` & `jupyterlite_terminal-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,43 @@
-drwxrwxr-x   0 jtp       (1000) jtp       (1000)        0 2024-05-29 16:10:59.806224 jupyterlite_terminal-0.0.0a0/
--rw-r--r--   0 jtp       (1000) jtp       (1000)       66 2024-05-29 16:10:59.806224 jupyterlite_terminal-0.0.0a0/PKG-INFO
-drwxrwxr-x   0 jtp       (1000) jtp       (1000)        0 2024-05-29 16:10:59.802224 jupyterlite_terminal-0.0.0a0/jupyterlite_terminal.egg-info/
--rw-r--r--   0 jtp       (1000) jtp       (1000)       66 2024-05-29 16:10:59.000000 jupyterlite_terminal-0.0.0a0/jupyterlite_terminal.egg-info/PKG-INFO
--rw-rw-r--   0 jtp       (1000) jtp       (1000)      184 2024-05-29 16:10:59.000000 jupyterlite_terminal-0.0.0a0/jupyterlite_terminal.egg-info/SOURCES.txt
--rw-rw-r--   0 jtp       (1000) jtp       (1000)        1 2024-05-29 16:10:59.000000 jupyterlite_terminal-0.0.0a0/jupyterlite_terminal.egg-info/dependency_links.txt
--rw-rw-r--   0 jtp       (1000) jtp       (1000)        1 2024-05-29 16:10:59.000000 jupyterlite_terminal-0.0.0a0/jupyterlite_terminal.egg-info/top_level.txt
--rw-rw-r--   0 jtp       (1000) jtp       (1000)       38 2024-05-29 16:10:59.806224 jupyterlite_terminal-0.0.0a0/setup.cfg
--rw-rw-r--   0 jtp       (1000) jtp       (1000)       94 2024-05-29 16:09:39.000000 jupyterlite_terminal-0.0.0a0/setup.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/.copier-answers.yml
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/.yarnrc.yml
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/babel.config.js
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/jest.config.js
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/jupyter-lite.json
+-rw-r--r--   0        0        0     6809 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/tsconfig.test.json
+-rw-r--r--   0        0        0   392280 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/yarn.lock
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/jupyterlite_terminal/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/jupyterlite_terminal/_version.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/jupyterlite_terminal/labextension/package.json
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/jupyterlite_terminal/labextension/static/353.2acc78de46aaa5d592af.js
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/jupyterlite_terminal/labextension/static/610.072cfacabcead899674d.js
+-rw-r--r--   0        0        0    24721 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/jupyterlite_terminal/labextension/static/644.3c458de5a0ca33a9756d.js
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/jupyterlite_terminal/labextension/static/728.2fd50c8de7f922692b1e.js
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/jupyterlite_terminal/labextension/static/remoteEntry.c2ac13e2a67fbf21986b.js
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/jupyterlite_terminal/labextension/static/style.js
+-rw-r--r--   0        0        0     6662 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/jupyterlite_terminal/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/src/index.ts
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/src/terminal.ts
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/src/terminals.ts
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/src/tokens.ts
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/src/__tests__/jupyterlite_terminal.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/style/index.js
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/ui-tests/tests/jupyterlite_terminal.spec.ts
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/README.md
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 jupyterlite_terminal-0.1.0/PKG-INFO
```

