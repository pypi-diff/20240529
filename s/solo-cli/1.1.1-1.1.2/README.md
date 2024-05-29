# Comparing `tmp/solo_cli-1.1.1.tar.gz` & `tmp/solo_cli-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solo_cli-1.1.1.tar", last modified: Wed May 29 05:19:01 2024, max compression
+gzip compressed data, was "solo_cli-1.1.2.tar", last modified: Wed May 29 05:37:40 2024, max compression
```

## Comparing `solo_cli-1.1.1.tar` & `solo_cli-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ddiddi     (501) staff       (20)        0 2024-05-29 05:19:01.137116 solo_cli-1.1.1/
--rw-r--r--   0 ddiddi     (501) staff       (20)      468 2024-05-29 05:19:01.136923 solo_cli-1.1.1/PKG-INFO
--rw-r--r--   0 ddiddi     (501) staff       (20)        3 2024-05-29 05:04:08.000000 solo_cli-1.1.1/README.md
--rw-r--r--   0 ddiddi     (501) staff       (20)       38 2024-05-29 05:19:01.137159 solo_cli-1.1.1/setup.cfg
--rw-r--r--   0 ddiddi     (501) staff       (20)      754 2024-05-29 05:18:06.000000 solo_cli-1.1.1/setup.py
-drwxr-xr-x   0 ddiddi     (501) staff       (20)        0 2024-05-29 05:19:01.136735 solo_cli-1.1.1/solo_cli.egg-info/
--rw-r--r--   0 ddiddi     (501) staff       (20)      468 2024-05-29 05:19:01.000000 solo_cli-1.1.1/solo_cli.egg-info/PKG-INFO
--rw-r--r--   0 ddiddi     (501) staff       (20)      224 2024-05-29 05:19:01.000000 solo_cli-1.1.1/solo_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ddiddi     (501) staff       (20)        1 2024-05-29 05:19:01.000000 solo_cli-1.1.1/solo_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ddiddi     (501) staff       (20)       38 2024-05-29 05:19:01.000000 solo_cli-1.1.1/solo_cli.egg-info/entry_points.txt
--rw-r--r--   0 ddiddi     (501) staff       (20)        6 2024-05-29 05:19:01.000000 solo_cli-1.1.1/solo_cli.egg-info/requires.txt
--rw-r--r--   0 ddiddi     (501) staff       (20)        9 2024-05-29 05:19:01.000000 solo_cli-1.1.1/solo_cli.egg-info/top_level.txt
--rw-r--r--   0 ddiddi     (501) staff       (20)     5286 2024-05-29 05:12:49.000000 solo_cli-1.1.1/solo_cli.py
+drwxr-xr-x   0 ddiddi     (501) staff       (20)        0 2024-05-29 05:37:40.963002 solo_cli-1.1.2/
+-rw-r--r--   0 ddiddi     (501) staff       (20)      468 2024-05-29 05:37:40.962799 solo_cli-1.1.2/PKG-INFO
+-rw-r--r--   0 ddiddi     (501) staff       (20)        3 2024-05-29 05:04:08.000000 solo_cli-1.1.2/README.md
+-rw-r--r--   0 ddiddi     (501) staff       (20)       38 2024-05-29 05:37:40.963043 solo_cli-1.1.2/setup.cfg
+-rw-r--r--   0 ddiddi     (501) staff       (20)      754 2024-05-29 05:37:29.000000 solo_cli-1.1.2/setup.py
+drwxr-xr-x   0 ddiddi     (501) staff       (20)        0 2024-05-29 05:37:40.962596 solo_cli-1.1.2/solo_cli.egg-info/
+-rw-r--r--   0 ddiddi     (501) staff       (20)      468 2024-05-29 05:37:40.000000 solo_cli-1.1.2/solo_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ddiddi     (501) staff       (20)      224 2024-05-29 05:37:40.000000 solo_cli-1.1.2/solo_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ddiddi     (501) staff       (20)        1 2024-05-29 05:37:40.000000 solo_cli-1.1.2/solo_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ddiddi     (501) staff       (20)       38 2024-05-29 05:37:40.000000 solo_cli-1.1.2/solo_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ddiddi     (501) staff       (20)        6 2024-05-29 05:37:40.000000 solo_cli-1.1.2/solo_cli.egg-info/requires.txt
+-rw-r--r--   0 ddiddi     (501) staff       (20)        9 2024-05-29 05:37:40.000000 solo_cli-1.1.2/solo_cli.egg-info/top_level.txt
+-rw-r--r--   0 ddiddi     (501) staff       (20)     3900 2024-05-29 05:37:24.000000 solo_cli-1.1.2/solo_cli.py
```

### Comparing `solo_cli-1.1.1/setup.py` & `solo_cli-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='solo-cli',
-    version='1.1.1',
+    version='1.1.2',
     py_modules=['solo_cli'],
     install_requires=[
         'click',
     ],
     entry_points='''
         [console_scripts]
         solo=solo_cli:cli
```

### Comparing `solo_cli-1.1.1/solo_cli.py` & `solo_cli-1.1.2/solo_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import click
 import os
 import subprocess
 import shutil
+import re
 
 @click.group()
 def cli():
     pass
 
 @cli.command()
 def install():
@@ -96,45 +97,16 @@
         click.echo("ngrok not found, installing ngrok...")
         subprocess.run(["curl", "-s", "https://ngrok-agent.s3.amazonaws.com/ngrok.asc", "|", "sudo", "tee", "/etc/apt/trusted.gpg.d/ngrok.asc"], check=True)
         subprocess.run(["echo", '"deb https://ngrok-agent.s3.amazonaws.com buster main"', "|", "sudo", "tee", "/etc/apt/sources.list.d/ngrok.list"], check=True)
         subprocess.run(["sudo", "apt", "update"], check=True)
         subprocess.run(["sudo", "apt", "install", "ngrok"], check=True)
 
     click.echo("Starting ngrok tunnel...")
-    subprocess.run(["ngrok", "http", "5000"], check=True)
+    result = subprocess.run(["ngrok", "http", "3000"], capture_output=True, text=True, check=True)
+    url = re.search(r"Forwarding\s+(https://[a-z0-9\-]+\.ngrok-free\.app)", result.stdout).group(1)
+    uuid = re.search(r"https://([a-z0-9\-]+)\.ngrok-free\.app", url).group(1)
 
-@cli.command()
-def web():
-    """Run OpenUI frontend and serve it with ngrok"""
-    click.echo("Checking Docker installation...")
-    if not shutil.which("docker"):
-        click.echo("Please install Docker to continue.")
-        return
-
-    click.echo("Checking if Docker container 'open-webui' is running...")
-    container_status = subprocess.run(["docker", "ps", "-q", "-f", "name=open-webui"], capture_output=True, text=True).stdout.strip()
-    
-    if container_status:
-        click.echo("Docker container 'open-webui' is already running. Stopping and removing it...")
-        subprocess.run(["docker", "stop", "open-webui"], check=True)
-        subprocess.run(["docker", "rm", "open-webui"], check=True)
-
-    click.echo("Running OpenUI Docker container...")
-    subprocess.run([
-        "docker", "run", "-d", "-p", "3000:8080", "--add-host=host.docker.internal:host-gateway",
-        "-v", "open-webui:/app/backend/data", "--name", "open-webui", "--restart", "always",
-        "ghcr.io/open-webui/open-webui:main"
-    ], check=True)
-
-    click.echo("Setting up ngrok...")
-    if not shutil.which("ngrok"):
-        click.echo("ngrok not found, installing ngrok...")
-        subprocess.run(["curl", "-s", "https://ngrok-agent.s3.amazonaws.com/ngrok.asc", "|", "sudo", "tee", "/etc/apt/trusted.gpg.d/ngrok.asc"], check=True)
-        subprocess.run(["echo", '"deb https://ngrok-agent.s3.amazonaws.com buster main"', "|", "sudo", "tee", "/etc/apt/sources.list.d/ngrok.list"], check=True)
-        subprocess.run(["sudo", "apt", "update"], check=True)
-        subprocess.run(["sudo", "apt", "install", "ngrok"], check=True)
-
-    click.echo("Starting ngrok tunnel...")
-    subprocess.run(["ngrok", "http", "3000"], check=True)
+    final_url = f"https://getsolo.tech/chat/{uuid}"
+    click.echo(f"Your service is available at: {final_url}")
 
 if __name__ == "__main__":
     cli()
```

