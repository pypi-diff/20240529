# Comparing `tmp/solo_cli-1.0.0.tar.gz` & `tmp/solo_cli-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solo_cli-1.0.0.tar", last modified: Wed May 29 05:09:06 2024, max compression
+gzip compressed data, was "solo_cli-1.1.1.tar", last modified: Wed May 29 05:19:01 2024, max compression
```

## Comparing `solo_cli-1.0.0.tar` & `solo_cli-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ddiddi     (501) staff       (20)        0 2024-05-29 05:09:06.191378 solo_cli-1.0.0/
--rw-r--r--   0 ddiddi     (501) staff       (20)      466 2024-05-29 05:09:06.191183 solo_cli-1.0.0/PKG-INFO
--rw-r--r--   0 ddiddi     (501) staff       (20)        3 2024-05-29 05:04:08.000000 solo_cli-1.0.0/README.md
--rw-r--r--   0 ddiddi     (501) staff       (20)       38 2024-05-29 05:09:06.191419 solo_cli-1.0.0/setup.cfg
--rw-r--r--   0 ddiddi     (501) staff       (20)      752 2024-05-29 05:01:08.000000 solo_cli-1.0.0/setup.py
-drwxr-xr-x   0 ddiddi     (501) staff       (20)        0 2024-05-29 05:09:06.191000 solo_cli-1.0.0/solo_cli.egg-info/
--rw-r--r--   0 ddiddi     (501) staff       (20)      466 2024-05-29 05:09:06.000000 solo_cli-1.0.0/solo_cli.egg-info/PKG-INFO
--rw-r--r--   0 ddiddi     (501) staff       (20)      224 2024-05-29 05:09:06.000000 solo_cli-1.0.0/solo_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ddiddi     (501) staff       (20)        1 2024-05-29 05:09:06.000000 solo_cli-1.0.0/solo_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ddiddi     (501) staff       (20)       38 2024-05-29 05:09:06.000000 solo_cli-1.0.0/solo_cli.egg-info/entry_points.txt
--rw-r--r--   0 ddiddi     (501) staff       (20)        6 2024-05-29 05:09:06.000000 solo_cli-1.0.0/solo_cli.egg-info/requires.txt
--rw-r--r--   0 ddiddi     (501) staff       (20)        9 2024-05-29 05:09:06.000000 solo_cli-1.0.0/solo_cli.egg-info/top_level.txt
--rw-r--r--   0 ddiddi     (501) staff       (20)     4825 2024-05-29 05:00:39.000000 solo_cli-1.0.0/solo_cli.py
+drwxr-xr-x   0 ddiddi     (501) staff       (20)        0 2024-05-29 05:19:01.137116 solo_cli-1.1.1/
+-rw-r--r--   0 ddiddi     (501) staff       (20)      468 2024-05-29 05:19:01.136923 solo_cli-1.1.1/PKG-INFO
+-rw-r--r--   0 ddiddi     (501) staff       (20)        3 2024-05-29 05:04:08.000000 solo_cli-1.1.1/README.md
+-rw-r--r--   0 ddiddi     (501) staff       (20)       38 2024-05-29 05:19:01.137159 solo_cli-1.1.1/setup.cfg
+-rw-r--r--   0 ddiddi     (501) staff       (20)      754 2024-05-29 05:18:06.000000 solo_cli-1.1.1/setup.py
+drwxr-xr-x   0 ddiddi     (501) staff       (20)        0 2024-05-29 05:19:01.136735 solo_cli-1.1.1/solo_cli.egg-info/
+-rw-r--r--   0 ddiddi     (501) staff       (20)      468 2024-05-29 05:19:01.000000 solo_cli-1.1.1/solo_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ddiddi     (501) staff       (20)      224 2024-05-29 05:19:01.000000 solo_cli-1.1.1/solo_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ddiddi     (501) staff       (20)        1 2024-05-29 05:19:01.000000 solo_cli-1.1.1/solo_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ddiddi     (501) staff       (20)       38 2024-05-29 05:19:01.000000 solo_cli-1.1.1/solo_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ddiddi     (501) staff       (20)        6 2024-05-29 05:19:01.000000 solo_cli-1.1.1/solo_cli.egg-info/requires.txt
+-rw-r--r--   0 ddiddi     (501) staff       (20)        9 2024-05-29 05:19:01.000000 solo_cli-1.1.1/solo_cli.egg-info/top_level.txt
+-rw-r--r--   0 ddiddi     (501) staff       (20)     5286 2024-05-29 05:12:49.000000 solo_cli-1.1.1/solo_cli.py
```

### Comparing `solo_cli-1.0.0/setup.py` & `solo_cli-1.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='solo-cli',
-    version='1.0.0',
+    version='1.1.1',
     py_modules=['solo_cli'],
     install_requires=[
         'click',
     ],
     entry_points='''
         [console_scripts]
         solo=solo_cli:cli
     ''',
-    author="Your Name",
+    author="Dhruv Diddi",
     author_email="your.email@example.com",
     description="A CLI to install and manage Ollama, and serve OpenUI with ngrok",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/yourusername/solo-cli",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `solo_cli-1.0.0/solo_cli.py` & `solo_cli-1.1.1/solo_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,20 +100,28 @@
         subprocess.run(["sudo", "apt", "install", "ngrok"], check=True)
 
     click.echo("Starting ngrok tunnel...")
     subprocess.run(["ngrok", "http", "5000"], check=True)
 
 @cli.command()
 def web():
-    """Run OpenUI frontend using Docker and serve it with ngrok"""
+    """Run OpenUI frontend and serve it with ngrok"""
     click.echo("Checking Docker installation...")
     if not shutil.which("docker"):
         click.echo("Please install Docker to continue.")
         return
 
+    click.echo("Checking if Docker container 'open-webui' is running...")
+    container_status = subprocess.run(["docker", "ps", "-q", "-f", "name=open-webui"], capture_output=True, text=True).stdout.strip()
+    
+    if container_status:
+        click.echo("Docker container 'open-webui' is already running. Stopping and removing it...")
+        subprocess.run(["docker", "stop", "open-webui"], check=True)
+        subprocess.run(["docker", "rm", "open-webui"], check=True)
+
     click.echo("Running OpenUI Docker container...")
     subprocess.run([
         "docker", "run", "-d", "-p", "3000:8080", "--add-host=host.docker.internal:host-gateway",
         "-v", "open-webui:/app/backend/data", "--name", "open-webui", "--restart", "always",
         "ghcr.io/open-webui/open-webui:main"
     ], check=True)
 
@@ -126,8 +134,7 @@
         subprocess.run(["sudo", "apt", "install", "ngrok"], check=True)
 
     click.echo("Starting ngrok tunnel...")
     subprocess.run(["ngrok", "http", "3000"], check=True)
 
 if __name__ == "__main__":
     cli()
-
```

