# Comparing `tmp/solo_cli-1.1.2.tar.gz` & `tmp/solo_cli-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solo_cli-1.1.2.tar", last modified: Wed May 29 05:37:40 2024, max compression
+gzip compressed data, was "solo_cli-1.1.3.tar", last modified: Wed May 29 05:42:25 2024, max compression
```

## Comparing `solo_cli-1.1.2.tar` & `solo_cli-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ddiddi     (501) staff       (20)        0 2024-05-29 05:37:40.963002 solo_cli-1.1.2/
--rw-r--r--   0 ddiddi     (501) staff       (20)      468 2024-05-29 05:37:40.962799 solo_cli-1.1.2/PKG-INFO
--rw-r--r--   0 ddiddi     (501) staff       (20)        3 2024-05-29 05:04:08.000000 solo_cli-1.1.2/README.md
--rw-r--r--   0 ddiddi     (501) staff       (20)       38 2024-05-29 05:37:40.963043 solo_cli-1.1.2/setup.cfg
--rw-r--r--   0 ddiddi     (501) staff       (20)      754 2024-05-29 05:37:29.000000 solo_cli-1.1.2/setup.py
-drwxr-xr-x   0 ddiddi     (501) staff       (20)        0 2024-05-29 05:37:40.962596 solo_cli-1.1.2/solo_cli.egg-info/
--rw-r--r--   0 ddiddi     (501) staff       (20)      468 2024-05-29 05:37:40.000000 solo_cli-1.1.2/solo_cli.egg-info/PKG-INFO
--rw-r--r--   0 ddiddi     (501) staff       (20)      224 2024-05-29 05:37:40.000000 solo_cli-1.1.2/solo_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ddiddi     (501) staff       (20)        1 2024-05-29 05:37:40.000000 solo_cli-1.1.2/solo_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ddiddi     (501) staff       (20)       38 2024-05-29 05:37:40.000000 solo_cli-1.1.2/solo_cli.egg-info/entry_points.txt
--rw-r--r--   0 ddiddi     (501) staff       (20)        6 2024-05-29 05:37:40.000000 solo_cli-1.1.2/solo_cli.egg-info/requires.txt
--rw-r--r--   0 ddiddi     (501) staff       (20)        9 2024-05-29 05:37:40.000000 solo_cli-1.1.2/solo_cli.egg-info/top_level.txt
--rw-r--r--   0 ddiddi     (501) staff       (20)     3900 2024-05-29 05:37:24.000000 solo_cli-1.1.2/solo_cli.py
+drwxr-xr-x   0 ddiddi     (501) staff       (20)        0 2024-05-29 05:42:25.158840 solo_cli-1.1.3/
+-rw-r--r--   0 ddiddi     (501) staff       (20)      468 2024-05-29 05:42:25.158646 solo_cli-1.1.3/PKG-INFO
+-rw-r--r--   0 ddiddi     (501) staff       (20)        3 2024-05-29 05:04:08.000000 solo_cli-1.1.3/README.md
+-rw-r--r--   0 ddiddi     (501) staff       (20)       38 2024-05-29 05:42:25.158878 solo_cli-1.1.3/setup.cfg
+-rw-r--r--   0 ddiddi     (501) staff       (20)      754 2024-05-29 05:42:11.000000 solo_cli-1.1.3/setup.py
+drwxr-xr-x   0 ddiddi     (501) staff       (20)        0 2024-05-29 05:42:25.158455 solo_cli-1.1.3/solo_cli.egg-info/
+-rw-r--r--   0 ddiddi     (501) staff       (20)      468 2024-05-29 05:42:25.000000 solo_cli-1.1.3/solo_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ddiddi     (501) staff       (20)      224 2024-05-29 05:42:25.000000 solo_cli-1.1.3/solo_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ddiddi     (501) staff       (20)        1 2024-05-29 05:42:25.000000 solo_cli-1.1.3/solo_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ddiddi     (501) staff       (20)       38 2024-05-29 05:42:25.000000 solo_cli-1.1.3/solo_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ddiddi     (501) staff       (20)        6 2024-05-29 05:42:25.000000 solo_cli-1.1.3/solo_cli.egg-info/requires.txt
+-rw-r--r--   0 ddiddi     (501) staff       (20)        9 2024-05-29 05:42:25.000000 solo_cli-1.1.3/solo_cli.egg-info/top_level.txt
+-rw-r--r--   0 ddiddi     (501) staff       (20)     4241 2024-05-29 05:42:08.000000 solo_cli-1.1.3/solo_cli.py
```

### Comparing `solo_cli-1.1.2/setup.py` & `solo_cli-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='solo-cli',
-    version='1.1.2',
+    version='1.1.3',
     py_modules=['solo_cli'],
     install_requires=[
         'click',
     ],
     entry_points='''
         [console_scripts]
         solo=solo_cli:cli
```

### Comparing `solo_cli-1.1.2/solo_cli.py` & `solo_cli-1.1.3/solo_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,18 +68,28 @@
     subprocess.run(["sudo", "userdel", "ollama"], check=True)
     subprocess.run(["sudo", "groupdel", "ollama"], check=True)
     click.echo("Ollama uninstalled.")
 
 @cli.command()
 def serve():
     """Serve OpenUI with ngrok"""
-    click.echo("Cloning the OpenUI repository...")
-    subprocess.run(["git", "clone", "https://github.com/open-webui/open-webui.git"], check=True)
-    
-    os.chdir("open-webui")
+    repo_url = "https://github.com/open-webui/open-webui.git"
+    clone_dir = "open-webui"
+
+    # Check if the directory exists
+    if os.path.exists(clone_dir):
+        click.echo(f"Directory '{clone_dir}' already exists.")
+        # Optionally, clean the directory
+        # shutil.rmtree(clone_dir)
+        # subprocess.run(["git", "clone", repo_url], check=True)
+    else:
+        click.echo(f"Cloning the OpenUI repository...")
+        subprocess.run(["git", "clone", repo_url], check=True)
+
+    os.chdir(clone_dir)
     
     click.echo("Copying required .env file...")
     subprocess.run(["cp", "-RPp", ".env.example", ".env"], check=True)
     
     click.echo("Building frontend using Node...")
     subprocess.run(["npm", "i"], check=True)
     subprocess.run(["npm", "run", "build"], check=True)
```

