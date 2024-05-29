# Comparing `tmp/freva_deployment-2405.1.0.tar.gz` & `tmp/freva_deployment-2405.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freva_deployment-2405.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "freva_deployment-2405.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `freva_deployment-2405.1.0.tar` & `freva_deployment-2405.1.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0       21 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/.dockerignore
--rw-r--r--   0        0        0      125 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      121 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/.github/dependabot/constraints.txt
--rw-r--r--   0        0        0     2946 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/.github/workflows/build_containers.yml
--rw-r--r--   0        0        0     3693 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/.github/workflows/build_job.yml
--rw-r--r--   0        0        0     1192 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/.github/workflows/bump_version.yml
--rw-r--r--   0        0        0     1230 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/.github/workflows/ci_job.yml
--rw-r--r--   0        0        0      346 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/.gitignore
--rw-r--r--   0        0        0     1301 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      135 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0      935 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/Dockerfile
--rw-r--r--   0        0        0     1078 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/LICENSE
--rw-r--r--   0        0        0       15 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/MANIFEST.in
--rw-r--r--   0        0        0      449 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/Makefile
--rw-r--r--   0        0        0    15618 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/README.md
--rw-r--r--   0        0        0    11564 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/assets/share/freva/deployment/config/create_tables.sql
--rw-r--r--   0        0        0     2578 2024-05-15 16:04:33.707509 freva_deployment-2405.1.0/assets/share/freva/deployment/config/evaluation_system.conf.tmpl
--rw-r--r--   0        0        0    11849 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/assets/share/freva/deployment/config/inventory.toml
--rw-r--r--   0        0        0    11896 2024-05-15 16:04:26.439468 freva_deployment-2405.1.0/assets/share/freva/deployment/config/unprivileged-user.toml
--rw-r--r--   0        0        0     1360 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/db_service/password_rotate.py
--rw-r--r--   0        0        0      388 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/db_service/reset_root_pw.sh
--rw-r--r--   0        0        0     6772 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/core-server-playbook.yml
--rw-r--r--   0        0        0     1370 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/db-server-compose-template.yml
--rw-r--r--   0        0        0     9150 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/db-server-playbook.yml
--rw-r--r--   0        0        0     1866 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/freva_rest-server-compose-template.yml
--rw-r--r--   0        0        0     7280 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/freva_rest-server-playbook.yml
--rw-r--r--   0        0        0     2325 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/versions.yaml
--rw-r--r--   0        0        0     3019 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/web-server-compose-template.yml
--rw-r--r--   0        0        0     9360 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/web-server-playbook.yml
--rwxr-xr-x   0        0        0     1036 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/scripts/create_cron.sh
--rw-r--r--   0        0        0     4754 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/scripts/create_systemd.py
--rwxr-xr-x   0        0        0    18447 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/scripts/docker-or-podman
--rwxr-xr-x   0        0        0     1856 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/scripts/download.py
--rwxr-xr-x   0        0        0       66 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/scripts/dump_sql
--rwxr-xr-x   0        0        0      792 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/scripts/inspect.sh
--rwxr-xr-x   0        0        0      160 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/scripts/prepare-httpd
--rw-r--r--   0        0        0     1067 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/vault/Dockerfile
--rw-r--r--   0        0        0     1005 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/vault/add-vault-secret
--rw-r--r--   0        0        0     1610 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/vault/checks.py
--rw-r--r--   0        0        0     1398 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/vault/deploy_vault.py
--rw-r--r--   0        0        0      246 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/vault/mypy.ini
--rw-r--r--   0        0        0       80 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/vault/policy-file.hcl
--rwxr-xr-x   0        0        0     9196 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/vault/runserver.py
--rw-r--r--   0        0        0      175 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/vault/vault-server-no-tls.hcl
--rw-r--r--   0        0        0      190 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/vault/vault-server-tls.hcl
--rwxr-xr-x   0        0        0     2305 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/web/Dockerfile
--rwxr-xr-x   0        0        0       38 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/web/docker_cmd.sh
--rwxr-xr-x   0        0        0       17 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/web/entrypoint.sh
--rw-r--r--   0        0        0    16008 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/assets/share/freva/deployment/web/freva_web.conf
--rwxr-xr-x   0        0        0     4095 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/cloud-init/start-vm.sh
--rwxr-xr-x   0        0        0    43499 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/Concept_Map.png
--rw-r--r--   0        0        0      634 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/Makefile
--rw-r--r--   0        0        0        0 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/_static/.keep
--rw-r--r--   0        0        0     8432 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/_static/freva_owl.svg
--rw-r--r--   0        0        0     4595 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/after-deployment/AfterDeployment.md
--rw-r--r--   0        0        0    11811 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/after-deployment/LegalNotes.md
--rw-r--r--   0        0        0     9862 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/after-deployment/TransitionPlugins.md
--rw-r--r--   0        0        0     2783 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/after-deployment/TransitionService.md
--rw-r--r--   0        0        0      427 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/after-deployment/index.rst
--rw-r--r--   0        0        0     5510 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/architecture/Architecture.md
--rw-r--r--   0        0        0     6832 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/architecture/Folders.md
--rwxr-xr-x   0        0        0    43499 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/architecture/_static/Concept_Map.png
--rw-r--r--   0        0        0    57311 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/architecture/_static/Topography.png
--rwxr-xr-x   0        0        0    41164 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/architecture/_static/Topography_1.png
--rwxr-xr-x   0        0        0    29463 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/architecture/_static/Topography_2.png
--rwxr-xr-x   0        0        0    46480 2024-05-15 16:04:26.443468 freva_deployment-2405.1.0/docs/architecture/_static/Topography_3.png
--rw-r--r--   0        0        0   119110 2024-05-15 16:04:26.447468 freva_deployment-2405.1.0/docs/architecture/_static/freva_flowchart-new.jpg
--rw-r--r--   0        0        0     2129 2024-05-15 16:04:26.447468 freva_deployment-2405.1.0/docs/architecture/index.rst
--rw-r--r--   0        0        0     4200 2024-05-15 16:04:26.447468 freva_deployment-2405.1.0/docs/conf.py
--rw-r--r--   0        0        0     3440 2024-05-15 16:04:26.447468 freva_deployment-2405.1.0/docs/contributing.md
--rw-r--r--   0        0        0    24540 2024-05-15 16:04:26.447468 freva_deployment-2405.1.0/docs/deployment/Config.md
--rw-r--r--   0        0        0    12942 2024-05-15 16:04:26.447468 freva_deployment-2405.1.0/docs/deployment/Configure.md
--rw-r--r--   0        0        0     3244 2024-05-15 16:04:26.447468 freva_deployment-2405.1.0/docs/deployment/Installation.md
--rw-r--r--   0        0        0    16690 2024-05-15 16:04:26.447468 freva_deployment-2405.1.0/docs/deployment/TuiHowto.md
--rw-r--r--   0        0        0    14354 2024-05-15 16:04:26.447468 freva_deployment-2405.1.0/docs/deployment/_static/Variable.png
--rw-r--r--   0        0        0   153459 2024-05-15 16:04:26.447468 freva_deployment-2405.1.0/docs/deployment/_static/tui_core.png
--rw-r--r--   0        0        0    76747 2024-05-15 16:04:26.447468 freva_deployment-2405.1.0/docs/deployment/_static/tui_db.png
--rw-r--r--   0        0        0    95292 2024-05-15 16:04:26.447468 freva_deployment-2405.1.0/docs/deployment/_static/tui_run.png
--rw-r--r--   0        0        0    70322 2024-05-15 16:04:26.447468 freva_deployment-2405.1.0/docs/deployment/_static/tui_solr.png
--rw-r--r--   0        0        0   153250 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/docs/deployment/_static/tui_web.png
--rw-r--r--   0        0        0     1421 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/docs/deployment/index.rst
--rw-r--r--   0        0        0      132 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/docs/environment.yml
--rw-r--r--   0        0        0     2429 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/docs/make.bat
--rw-r--r--   0        0        0     1360 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/docs/whatsnew.rst
--rw-r--r--   0        0        0      750 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/mypy.ini
--rw-r--r--   0        0        0       89 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/pyinstaller/pyinstaller-script.py
--rw-r--r--   0        0        0     2662 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/pyproject.toml
--rw-r--r--   0        0        0    15726 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/release.py
--rw-r--r--   0        0        0     1400 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/__init__.py
--rw-r--r--   0        0        0      290 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/cli/__init__.py
--rw-r--r--   0        0        0     2977 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/cli/_deploy.py
--rw-r--r--   0        0        0     7554 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/cli/_migrate.py
--rw-r--r--   0        0        0    36891 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/deploy.py
--rw-r--r--   0        0        0     2813 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/error.py
--rw-r--r--   0        0        0     5611 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/keys.py
--rw-r--r--   0        0        0      602 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/logger.py
--rw-r--r--   0        0        0        0 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/py.typed
--rw-r--r--   0        0        0     1949 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/runner.py
--rw-r--r--   0        0        0        0 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/ui/__init__.py
--rw-r--r--   0        0        0     2113 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/ui/deployment_tui/__init__.py
--rw-r--r--   0        0        0    13384 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/ui/deployment_tui/base.py
--rw-r--r--   0        0        0    35764 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/ui/deployment_tui/deploy_forms.py
--rw-r--r--   0        0        0    10872 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/ui/deployment_tui/main_window.py
--rw-r--r--   0        0        0    10774 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/utils.py
--rw-r--r--   0        0        0      121 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/versions.json
--rw-r--r--   0        0        0     2990 2024-05-15 16:04:26.451468 freva_deployment-2405.1.0/src/freva_deployment/versions.py
--rw-r--r--   0        0        0    17358 1970-01-01 00:00:00.000000 freva_deployment-2405.1.0/PKG-INFO
+-rw-r--r--   0        0        0       21 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/.dockerignore
+-rw-r--r--   0        0        0      125 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      121 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/.github/dependabot/constraints.txt
+-rw-r--r--   0        0        0     2946 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/.github/workflows/build_containers.yml
+-rw-r--r--   0        0        0     3693 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/.github/workflows/build_job.yml
+-rw-r--r--   0        0        0     1192 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/.github/workflows/bump_version.yml
+-rw-r--r--   0        0        0     1230 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/.github/workflows/ci_job.yml
+-rw-r--r--   0        0        0      346 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/.gitignore
+-rw-r--r--   0        0        0     1301 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      135 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      935 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/Dockerfile
+-rw-r--r--   0        0        0     1078 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/LICENSE
+-rw-r--r--   0        0        0       15 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/MANIFEST.in
+-rw-r--r--   0        0        0      449 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/Makefile
+-rw-r--r--   0        0        0    15618 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/README.md
+-rw-r--r--   0        0        0    11564 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/config/create_tables.sql
+-rw-r--r--   0        0        0     2578 2024-05-29 14:29:19.313383 freva_deployment-2405.1.1/assets/share/freva/deployment/config/evaluation_system.conf.tmpl
+-rw-r--r--   0        0        0    11849 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/config/inventory.toml
+-rw-r--r--   0        0        0    11896 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/config/unprivileged-user.toml
+-rw-r--r--   0        0        0     1360 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/db_service/password_rotate.py
+-rw-r--r--   0        0        0      388 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/db_service/reset_root_pw.sh
+-rw-r--r--   0        0        0     6772 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/core-server-playbook.yml
+-rw-r--r--   0        0        0     1370 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/db-server-compose-template.yml
+-rw-r--r--   0        0        0     9150 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/db-server-playbook.yml
+-rw-r--r--   0        0        0     1866 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/freva_rest-server-compose-template.yml
+-rw-r--r--   0        0        0     7280 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/freva_rest-server-playbook.yml
+-rw-r--r--   0        0        0     2325 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/versions.yaml
+-rw-r--r--   0        0        0     2935 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/web-server-compose-template.yml
+-rw-r--r--   0        0        0     9360 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/web-server-playbook.yml
+-rwxr-xr-x   0        0        0     1036 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/scripts/create_cron.sh
+-rw-r--r--   0        0        0     4754 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/scripts/create_systemd.py
+-rwxr-xr-x   0        0        0    18447 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/scripts/docker-or-podman
+-rwxr-xr-x   0        0        0     1856 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/scripts/download.py
+-rwxr-xr-x   0        0        0       66 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/scripts/dump_sql
+-rwxr-xr-x   0        0        0      792 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/scripts/inspect.sh
+-rwxr-xr-x   0        0        0      161 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/scripts/prepare-httpd
+-rw-r--r--   0        0        0     1067 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/vault/Dockerfile
+-rw-r--r--   0        0        0     1005 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/vault/add-vault-secret
+-rw-r--r--   0        0        0     1610 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/vault/checks.py
+-rw-r--r--   0        0        0     1398 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/vault/deploy_vault.py
+-rw-r--r--   0        0        0      246 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/vault/mypy.ini
+-rw-r--r--   0        0        0       80 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/vault/policy-file.hcl
+-rwxr-xr-x   0        0        0     9196 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/vault/runserver.py
+-rw-r--r--   0        0        0      175 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/vault/vault-server-no-tls.hcl
+-rw-r--r--   0        0        0      190 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/vault/vault-server-tls.hcl
+-rwxr-xr-x   0        0        0     2305 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/web/Dockerfile
+-rwxr-xr-x   0        0        0       38 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/web/docker_cmd.sh
+-rwxr-xr-x   0        0        0       17 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/web/entrypoint.sh
+-rw-r--r--   0        0        0    16008 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/assets/share/freva/deployment/web/freva_web.conf
+-rwxr-xr-x   0        0        0     4095 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/cloud-init/start-vm.sh
+-rwxr-xr-x   0        0        0    43499 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/docs/Concept_Map.png
+-rw-r--r--   0        0        0      634 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/docs/Makefile
+-rw-r--r--   0        0        0        0 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/docs/_static/.keep
+-rw-r--r--   0        0        0     8432 2024-05-29 14:29:17.633383 freva_deployment-2405.1.1/docs/_static/freva_owl.svg
+-rw-r--r--   0        0        0     4595 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/after-deployment/AfterDeployment.md
+-rw-r--r--   0        0        0    11811 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/after-deployment/LegalNotes.md
+-rw-r--r--   0        0        0     9862 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/after-deployment/TransitionPlugins.md
+-rw-r--r--   0        0        0     2783 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/after-deployment/TransitionService.md
+-rw-r--r--   0        0        0      427 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/after-deployment/index.rst
+-rw-r--r--   0        0        0     5510 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/architecture/Architecture.md
+-rw-r--r--   0        0        0     6832 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/architecture/Folders.md
+-rwxr-xr-x   0        0        0    43499 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/architecture/_static/Concept_Map.png
+-rw-r--r--   0        0        0    57311 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/architecture/_static/Topography.png
+-rwxr-xr-x   0        0        0    41164 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/architecture/_static/Topography_1.png
+-rwxr-xr-x   0        0        0    29463 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/architecture/_static/Topography_2.png
+-rwxr-xr-x   0        0        0    46480 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/architecture/_static/Topography_3.png
+-rw-r--r--   0        0        0   119110 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/architecture/_static/freva_flowchart-new.jpg
+-rw-r--r--   0        0        0     2129 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/architecture/index.rst
+-rw-r--r--   0        0        0     4200 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/conf.py
+-rw-r--r--   0        0        0     3440 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/contributing.md
+-rw-r--r--   0        0        0    24540 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/deployment/Config.md
+-rw-r--r--   0        0        0    12942 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/deployment/Configure.md
+-rw-r--r--   0        0        0     3244 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/deployment/Installation.md
+-rw-r--r--   0        0        0    16690 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/deployment/TuiHowto.md
+-rw-r--r--   0        0        0    14354 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/deployment/_static/Variable.png
+-rw-r--r--   0        0        0   153459 2024-05-29 14:29:17.637383 freva_deployment-2405.1.1/docs/deployment/_static/tui_core.png
+-rw-r--r--   0        0        0    76747 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/docs/deployment/_static/tui_db.png
+-rw-r--r--   0        0        0    95292 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/docs/deployment/_static/tui_run.png
+-rw-r--r--   0        0        0    70322 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/docs/deployment/_static/tui_solr.png
+-rw-r--r--   0        0        0   153250 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/docs/deployment/_static/tui_web.png
+-rw-r--r--   0        0        0     1421 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/docs/deployment/index.rst
+-rw-r--r--   0        0        0      132 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/docs/environment.yml
+-rw-r--r--   0        0        0     2429 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/docs/make.bat
+-rw-r--r--   0        0        0     1402 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/docs/whatsnew.rst
+-rw-r--r--   0        0        0      750 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/mypy.ini
+-rw-r--r--   0        0        0       89 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/pyinstaller/pyinstaller-script.py
+-rw-r--r--   0        0        0     2662 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/pyproject.toml
+-rw-r--r--   0        0        0    15726 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/release.py
+-rw-r--r--   0        0        0     1400 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/__init__.py
+-rw-r--r--   0        0        0      290 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/cli/__init__.py
+-rw-r--r--   0        0        0     2977 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/cli/_deploy.py
+-rw-r--r--   0        0        0     7554 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/cli/_migrate.py
+-rw-r--r--   0        0        0    35862 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/deploy.py
+-rw-r--r--   0        0        0     2813 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/error.py
+-rw-r--r--   0        0        0     5611 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/keys.py
+-rw-r--r--   0        0        0      602 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/logger.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/py.typed
+-rw-r--r--   0        0        0     1949 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/runner.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/ui/__init__.py
+-rw-r--r--   0        0        0     2113 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/ui/deployment_tui/__init__.py
+-rw-r--r--   0        0        0    13384 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/ui/deployment_tui/base.py
+-rw-r--r--   0        0        0    35764 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/ui/deployment_tui/deploy_forms.py
+-rw-r--r--   0        0        0    10872 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/ui/deployment_tui/main_window.py
+-rw-r--r--   0        0        0    10817 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/utils.py
+-rw-r--r--   0        0        0      121 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/versions.json
+-rw-r--r--   0        0        0     2990 2024-05-29 14:29:17.641383 freva_deployment-2405.1.1/src/freva_deployment/versions.py
+-rw-r--r--   0        0        0    17358 1970-01-01 00:00:00.000000 freva_deployment-2405.1.1/PKG-INFO
```

### Comparing `freva_deployment-2405.1.0/.github/workflows/build_containers.yml` & `freva_deployment-2405.1.1/.github/workflows/build_containers.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/.github/workflows/build_job.yml` & `freva_deployment-2405.1.1/.github/workflows/build_job.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/.github/workflows/bump_version.yml` & `freva_deployment-2405.1.1/.github/workflows/bump_version.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/.github/workflows/ci_job.yml` & `freva_deployment-2405.1.1/.github/workflows/ci_job.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/.gitlab-ci.yml` & `freva_deployment-2405.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/Dockerfile` & `freva_deployment-2405.1.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/LICENSE` & `freva_deployment-2405.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/README.md` & `freva_deployment-2405.1.1/README.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/config/create_tables.sql` & `freva_deployment-2405.1.1/assets/share/freva/deployment/config/create_tables.sql`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/config/evaluation_system.conf.tmpl` & `freva_deployment-2405.1.1/assets/share/freva/deployment/config/evaluation_system.conf.tmpl`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/config/inventory.toml` & `freva_deployment-2405.1.1/assets/share/freva/deployment/config/inventory.toml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/config/unprivileged-user.toml` & `freva_deployment-2405.1.1/assets/share/freva/deployment/config/unprivileged-user.toml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/db_service/password_rotate.py` & `freva_deployment-2405.1.1/assets/share/freva/deployment/db_service/password_rotate.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/core-server-playbook.yml` & `freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/core-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/db-server-compose-template.yml` & `freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/db-server-compose-template.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/db-server-playbook.yml` & `freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/db-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/freva_rest-server-compose-template.yml` & `freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/freva_rest-server-compose-template.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/freva_rest-server-playbook.yml` & `freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/freva_rest-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/versions.yaml` & `freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/versions.yaml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/web-server-compose-template.yml` & `freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/web-server-compose-template.yml`

 * *Files 3% similar despite different names*

```diff
@@ -59,16 +59,14 @@
     network_mode: host
 {% else %}
     networks:
       - {{web_name}}
 {% endif %}
     environment:
       - EVALUATION_SYSTEM_CONFIG_FILE={{core_root_dir|regex_replace('^~', ansible_env.HOME)}}/freva/evaluation_system.conf
-      - LDAP_USER_DN={{web_ldap_user_dn}}
-      - LDAP_USER_PW={{web_ldap_user_pw}}
       - DJANGO_SUPERUSER_PASSWORD={{ root_passwd }}
       - FREVA_WEB_CONFIG_FILE={{web_config_file}}
       - AUTH_LDAP_SERVER_URI={{web_auth_ldap_server_uri}}
       - AUTH_LDAP_START_TLS={{ 1 if web_auth_ldap_start_tls else 0 }}
       - ALLOWED_GROUP={{web_allowed_group}}
       - ALLOWED_HOSTS={{web_allowed_hosts | join(',')}}
       - LDAP_USER_BASE={{web_ldap_user_base}}
```

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/playbooks/web-server-playbook.yml` & `freva_deployment-2405.1.1/assets/share/freva/deployment/playbooks/web-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/scripts/create_cron.sh` & `freva_deployment-2405.1.1/assets/share/freva/deployment/scripts/create_cron.sh`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/scripts/create_systemd.py` & `freva_deployment-2405.1.1/assets/share/freva/deployment/scripts/create_systemd.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/scripts/docker-or-podman` & `freva_deployment-2405.1.1/assets/share/freva/deployment/scripts/docker-or-podman`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/scripts/download.py` & `freva_deployment-2405.1.1/assets/share/freva/deployment/scripts/download.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/scripts/inspect.sh` & `freva_deployment-2405.1.1/assets/share/freva/deployment/scripts/inspect.sh`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/vault/Dockerfile` & `freva_deployment-2405.1.1/assets/share/freva/deployment/vault/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/vault/add-vault-secret` & `freva_deployment-2405.1.1/assets/share/freva/deployment/vault/add-vault-secret`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/vault/checks.py` & `freva_deployment-2405.1.1/assets/share/freva/deployment/vault/checks.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/vault/deploy_vault.py` & `freva_deployment-2405.1.1/assets/share/freva/deployment/vault/deploy_vault.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/vault/runserver.py` & `freva_deployment-2405.1.1/assets/share/freva/deployment/vault/runserver.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/web/Dockerfile` & `freva_deployment-2405.1.1/assets/share/freva/deployment/web/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/assets/share/freva/deployment/web/freva_web.conf` & `freva_deployment-2405.1.1/assets/share/freva/deployment/web/freva_web.conf`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/cloud-init/start-vm.sh` & `freva_deployment-2405.1.1/cloud-init/start-vm.sh`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/Concept_Map.png` & `freva_deployment-2405.1.1/docs/Concept_Map.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/Makefile` & `freva_deployment-2405.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/_static/freva_owl.svg` & `freva_deployment-2405.1.1/docs/_static/freva_owl.svg`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/after-deployment/AfterDeployment.md` & `freva_deployment-2405.1.1/docs/after-deployment/AfterDeployment.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/after-deployment/LegalNotes.md` & `freva_deployment-2405.1.1/docs/after-deployment/LegalNotes.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/after-deployment/TransitionPlugins.md` & `freva_deployment-2405.1.1/docs/after-deployment/TransitionPlugins.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/after-deployment/TransitionService.md` & `freva_deployment-2405.1.1/docs/after-deployment/TransitionService.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/architecture/Architecture.md` & `freva_deployment-2405.1.1/docs/architecture/Architecture.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/architecture/Folders.md` & `freva_deployment-2405.1.1/docs/architecture/Folders.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/architecture/_static/Concept_Map.png` & `freva_deployment-2405.1.1/docs/architecture/_static/Concept_Map.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/architecture/_static/Topography.png` & `freva_deployment-2405.1.1/docs/architecture/_static/Topography.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/architecture/_static/Topography_1.png` & `freva_deployment-2405.1.1/docs/architecture/_static/Topography_1.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/architecture/_static/Topography_2.png` & `freva_deployment-2405.1.1/docs/architecture/_static/Topography_2.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/architecture/_static/Topography_3.png` & `freva_deployment-2405.1.1/docs/architecture/_static/Topography_3.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/architecture/_static/freva_flowchart-new.jpg` & `freva_deployment-2405.1.1/docs/architecture/_static/freva_flowchart-new.jpg`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/architecture/index.rst` & `freva_deployment-2405.1.1/docs/architecture/index.rst`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/conf.py` & `freva_deployment-2405.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/contributing.md` & `freva_deployment-2405.1.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/deployment/Config.md` & `freva_deployment-2405.1.1/docs/deployment/Config.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/deployment/Configure.md` & `freva_deployment-2405.1.1/docs/deployment/Configure.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/deployment/Installation.md` & `freva_deployment-2405.1.1/docs/deployment/Installation.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/deployment/TuiHowto.md` & `freva_deployment-2405.1.1/docs/deployment/TuiHowto.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/deployment/_static/Variable.png` & `freva_deployment-2405.1.1/docs/deployment/_static/Variable.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/deployment/_static/tui_core.png` & `freva_deployment-2405.1.1/docs/deployment/_static/tui_core.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/deployment/_static/tui_db.png` & `freva_deployment-2405.1.1/docs/deployment/_static/tui_db.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/deployment/_static/tui_run.png` & `freva_deployment-2405.1.1/docs/deployment/_static/tui_run.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/deployment/_static/tui_solr.png` & `freva_deployment-2405.1.1/docs/deployment/_static/tui_solr.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/deployment/_static/tui_web.png` & `freva_deployment-2405.1.1/docs/deployment/_static/tui_web.png`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/deployment/index.rst` & `freva_deployment-2405.1.1/docs/deployment/index.rst`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/index.rst` & `freva_deployment-2405.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/make.bat` & `freva_deployment-2405.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/docs/whatsnew.rst` & `freva_deployment-2405.1.1/docs/whatsnew.rst`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 What's new
 ===========
 
 .. toctree::
    :maxdepth: 0
    :titlesonly:
 
+v2405.1.1
+~~~~~~~~
+* Minor bug fixing.
+
+
+
 v2405.1.0
 ~~~~~~~~
 * Bumped version of freva core to 2406.0.0
 
 
 
 v2405.0.0
```

### Comparing `freva_deployment-2405.1.0/mypy.ini` & `freva_deployment-2405.1.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/pyproject.toml` & `freva_deployment-2405.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/release.py` & `freva_deployment-2405.1.1/release.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/src/freva_deployment/__init__.py` & `freva_deployment-2405.1.1/src/freva_deployment/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 from urllib.request import urlretrieve
 
-__version__ = "2405.1.0"
+__version__ = "2405.1.1"
 
 FREVA_PYTHON_VERSION = "3.11"
 AVAILABLE_PYTHON_VERSIONS = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 AVAILABLE_CONDA_ARCHS = [
     "linux-64",
     "linux-aarch64",
     "linux-ppc64le",
```

### Comparing `freva_deployment-2405.1.0/src/freva_deployment/cli/_deploy.py` & `freva_deployment-2405.1.1/src/freva_deployment/cli/_deploy.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/src/freva_deployment/cli/_migrate.py` & `freva_deployment-2405.1.1/src/freva_deployment/cli/_migrate.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/src/freva_deployment/deploy.py` & `freva_deployment-2405.1.1/src/freva_deployment/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,17 +81,15 @@
     ) -> None:
         self.gen_keys = gen_keys or local_debug
         self.local_debug = local_debug
         self._config_keys: list[str] = []
         self._master_pass: str = ""
         self.email_password: str = ""
         self._td: RunnerDir = RunnerDir()
-        self.eval_conf_file: Path = (
-            self._td.parent_dir / "evaluation_system.conf"
-        )
+        self.eval_conf_file: Path = self._td.parent_dir / "evaluation_system.conf"
         self.web_conf_file: Path = self._td.parent_dir / "freva_web.toml"
         self.apache_config: Path = self._td.parent_dir / "freva_web.conf"
         self._db_pass: str = ""
         self._steps = steps or ["db", "freva_rest", "web", "core"]
         if self._steps == ["auto"] or self._steps == "auto":
             self._steps = []
         self._inv_tmpl = Path(config_file or config_dir / "inventory.toml")
@@ -166,29 +164,29 @@
             "You must give a valid path to a private key file."
         ) from None
 
     def _prep_vault(self) -> None:
         """Prepare the vault."""
         self.cfg["vault"]["config"].setdefault("ansible_become_user", "root")
         self.cfg["vault"]["config"].pop("db_playbook", "")
-        self.cfg["vault"]["config"]["db_port"] = self.cfg["vault"][
-            "config"
-        ].get("port", 3306)
-        self.cfg["vault"]["config"]["db_user"] = self.cfg["vault"][
-            "config"
-        ].get("user", "")
+        self.cfg["vault"]["config"]["db_port"] = self.cfg["vault"]["config"].get(
+            "port", 3306
+        )
+        self.cfg["vault"]["config"]["db_user"] = self.cfg["vault"]["config"].get(
+            "user", ""
+        )
         self.cfg["vault"]["config"]["root_passwd"] = self.master_pass
         self.cfg["vault"]["config"]["passwd"] = self.db_pass
         self.cfg["vault"]["config"]["keyfile"] = self.public_key_file
         self.cfg["vault"]["config"]["email"] = self.cfg["web"]["config"].get(
             "contacts", ""
         )
-        self.cfg["vault"]["config"]["db_host"] = self.cfg["db"]["config"][
-            "host"
-        ]
+        self.cfg["vault"]["config"]["db_host"] = self.cfg["db"]["config"].get(
+            "host", self.cfg["db"]["hosts"]
+        )
 
     def _prep_db(self) -> None:
         """prepare the mariadb service."""
         self._config_keys.append("db")
         self.cfg["db"]["config"].setdefault("ansible_become_user", "root")
         host = self.cfg["db"]["hosts"]
         self.cfg["db"]["config"]["root_passwd"] = self.master_pass
@@ -198,65 +196,57 @@
             cast(
                 str,
                 self.cfg["db"]["config"].get("data_path", "/opt/freva"),
             )
         )
         self.cfg["db"]["config"]["data_path"] = str(data_path)
         for key in ("name", "user", "db"):
-            self.cfg["db"]["config"][key] = (
-                self.cfg["db"]["config"].get(key) or "freva"
-            )
+            self.cfg["db"]["config"][key] = self.cfg["db"]["config"].get(key) or "freva"
         db_host = self.cfg["db"]["config"].get("host", "").strip()
         if not db_host:
             self.cfg["db"]["config"]["host"] = host
         self.cfg["db"]["config"].setdefault("port", "3306")
         self.cfg["db"]["config"]["email"] = self.cfg["web"]["config"].get(
             "contacts", ""
         )
         self.playbooks["db"] = self.cfg["db"]["config"].get("db_playbook")
         self._prep_vault()
         self._prep_web(False)
 
     def _prep_freva_rest(self, prep_web=True) -> None:
         """prepare the freva_rest service."""
         self._config_keys.append("freva_rest")
-        self.cfg["freva_rest"]["config"].setdefault(
-            "ansible_become_user", "root"
-        )
+        self.cfg["freva_rest"]["config"].setdefault("ansible_become_user", "root")
         self.cfg["freva_rest"]["config"]["root_passwd"] = self.master_pass
         self.cfg["freva_rest"]["config"].pop("core", None)
         data_path = Path(
             cast(
                 str,
-                self.cfg["freva_rest"]["config"].get(
-                    "data_path", "/opt/freva"
-                ),
+                self.cfg["freva_rest"]["config"].get("data_path", "/opt/freva"),
             )
         )
         self.cfg["freva_rest"]["config"]["data_path"] = str(data_path)
         self.playbooks["freva_rest"] = self.cfg["freva_rest"]["config"].get(
             "freva_rest_playbook"
         )
         for key, default in dict(solr_mem="4g", freva_rest_port=7777).items():
             self.cfg["freva_rest"]["config"][key] = (
                 self.cfg["freva_rest"]["config"].get(key) or default
             )
-        self.cfg["freva_rest"]["config"]["email"] = self.cfg["web"][
-            "config"
-        ].get("contacts", "")
+        self.cfg["freva_rest"]["config"]["email"] = self.cfg["web"]["config"].get(
+            "contacts", ""
+        )
         if prep_web:
             self._prep_web(False)
 
     def _prep_core(self) -> None:
         """prepare the core deployment."""
         self._config_keys.append("core")
         self.cfg["core"]["config"].setdefault("ansible_become_user", "")
-        self.playbooks["core"] = self.cfg["core"]["config"].get(
-            "core_playbook"
-        )
+        self.playbooks["core"] = self.cfg["core"]["config"].get("core_playbook")
         # Legacy args as we are going to use micromamba
         self.cfg["core"]["config"]["arch"] = (
             self.cfg["core"]["config"]
             .get("arch", "linux-64")
             .lower()
             .replace("x86_", "")
             .replace("mac", "")
@@ -264,43 +254,35 @@
         self.cfg["core"]["config"]["python_version"] = FREVA_PYTHON_VERSION
         self.cfg["core"]["config"]["admins"] = (
             self.cfg["core"]["config"].get("admins") or getuser()
         )
         if not self.cfg["core"]["config"]["admins"]:
             self.cfg["core"]["config"]["admins"] = getuser()
         install_dir = Path(self.cfg["core"]["config"]["install_dir"])
-        root_dir = Path(
-            self.cfg["core"]["config"].get("root_dir", "") or install_dir
-        )
+        root_dir = Path(self.cfg["core"]["config"].get("root_dir", "") or install_dir)
         self.cfg["core"]["config"]["install_dir"] = str(install_dir)
         self.cfg["core"]["config"]["root_dir"] = str(root_dir)
         preview_path = self.cfg["core"]["config"].get("preview_path", "")
         base_dir_location = self.cfg["core"]["config"].get(
             "base_dir_location", ""
         ) or str(root_dir / "work")
         self.cfg["core"]["config"]["base_dir_location"] = base_dir_location
         scheduler_output_dir = self.cfg["core"]["config"].get(
             "scheduler_output_dir", ""
         )
-        scheduler_system = self.cfg["core"]["config"].get(
-            "scheduler_system", "local"
-        )
+        scheduler_system = self.cfg["core"]["config"].get("scheduler_system", "local")
         if not preview_path:
             self.cfg["core"]["config"]["preview_path"] = str(
                 Path(base_dir_location) / "share" / "preview"
             )
         if not scheduler_output_dir:
             scheduler_output_dir = str(Path(base_dir_location) / "share")
         elif Path(scheduler_output_dir).parts[-1] != scheduler_system:
-            scheduler_output_dir = (
-                Path(scheduler_output_dir) / scheduler_system
-            )
-        self.cfg["core"]["config"]["scheduler_output_dir"] = str(
-            scheduler_output_dir
-        )
+            scheduler_output_dir = Path(scheduler_output_dir) / scheduler_system
+        self.cfg["core"]["config"]["scheduler_output_dir"] = str(scheduler_output_dir)
         self.cfg["core"]["config"]["keyfile"] = self.public_key_file
         git_exe = self.cfg["core"]["config"].get("git_path")
         self.cfg["core"]["config"]["git_path"] = git_exe or "git"
         self.cfg["core"]["config"][
             "git_url"
         ] = "https://github.com/FREVA-CLINT/freva.git"
 
@@ -331,49 +313,31 @@
             raise ConfigurationError(
                 "No web config section given, please configure the web.config"
             ) from None
         if not isinstance(admin, str):
             self.cfg["web"]["config"]["admin"] = admin[0]
         else:
             self.cfg["web"]["config"]["admin"] = admin
-        allowed_hosts = self.cfg["web"]["config"].get("allowed_hosts") or [
-            "localhost"
-        ]
+        allowed_hosts = self.cfg["web"]["config"].get("allowed_hosts") or ["localhost"]
         allowed_hosts.append(self.cfg["web"]["hosts"])
         allowed_hosts.append(f"{self.project_name}-httpd")
         self.cfg["web"]["config"]["allowed_hosts"] = list(set(allowed_hosts))
         self.cfg["web"]["config"].setdefault("allowed_hosts", ["localhost"])
 
         _webserver_items = {
-            "institution_logo": self.cfg["web"]["config"].get(
-                "institution_logo", ""
-            ),
-            "main_color": self.cfg["web"]["config"].get(
-                "main_color", "Tomato"
-            ),
-            "border_color": self.cfg["web"]["config"].get(
-                "border_color", "#6c2e1f"
-            ),
-            "hover_color": self.cfg["web"]["config"].get(
-                "hover_color", "#d0513a"
-            ),
-            "homepage_text": self.cfg["web"]["config"].get(
-                "homepage_text", ""
-            ),
+            "institution_logo": self.cfg["web"]["config"].get("institution_logo", ""),
+            "main_color": self.cfg["web"]["config"].get("main_color", "Tomato"),
+            "border_color": self.cfg["web"]["config"].get("border_color", "#6c2e1f"),
+            "hover_color": self.cfg["web"]["config"].get("hover_color", "#d0513a"),
+            "homepage_text": self.cfg["web"]["config"].get("homepage_text", ""),
             "imprint": self.cfg["web"]["config"].get("imprint", []),
-            "homepage_heading": self.cfg["web"]["config"].get(
-                "homepage_heading", ""
-            ),
-            "about_us_text": self.cfg["web"]["config"].get(
-                "about_us_text", ""
-            ),
+            "homepage_heading": self.cfg["web"]["config"].get("homepage_heading", ""),
+            "about_us_text": self.cfg["web"]["config"].get("about_us_text", ""),
             "contacts": self.cfg["web"]["config"].get("contacts", []),
-            "insitution_name": self.cfg["web"]["config"].get(
-                "insitution_name", ""
-            ),
+            "insitution_name": self.cfg["web"]["config"].get("insitution_name", ""),
             "menu_entries": self.cfg["web"]["config"].get("menu_entries", []),
         }
         try:
             with Path(_webserver_items["homepage_text"]).open("r") as f_obj:
                 _webserver_items["homepage_text"] = f_obj.read()
         except (FileNotFoundError, IOError, KeyError):
             pass
@@ -384,17 +348,15 @@
             pass
         with self.web_conf_file.open("w") as f_obj:
             tomlkit.dump(_webserver_items, f_obj)
 
         if self.local_debug:
             self.cfg["web"]["config"]["redis_host"] = self.cfg["web"]["hosts"]
         else:
-            self.cfg["web"]["config"][
-                "redis_host"
-            ] = f"{self.project_name}-redis"
+            self.cfg["web"]["config"]["redis_host"] = f"{self.project_name}-redis"
 
         server_name = self.cfg["web"]["config"].pop("server_name", [])
         if isinstance(server_name, str):
             server_name = server_name.split(",")
         server_name = ",".join([a for a in server_name if a.strip()])
         if not server_name:
             server_name = self.cfg["web"]["hosts"]
@@ -415,87 +377,72 @@
                 self.cfg["web"]["config"]["csrf_trusted_origins"].append(
                     f"https://{trusted_origin.path}"
                 )
         self.cfg["web"]["config"]["freva_bin"] = os.path.join(
             self.cfg["core"]["config"]["install_dir"], "bin"
         )
         for key in ("core", "web"):
-            self.cfg[key]["config"]["config_toml_file"] = str(
-                self.web_conf_file
-            )
+            self.cfg[key]["config"]["config_toml_file"] = str(self.web_conf_file)
         self._prep_vault()
         if ask_pass:
             email_user, self.email_password = get_email_credentials()
             self.cfg["vault"]["config"]["email_user"] = email_user
             self.cfg["vault"]["config"]["email_password"] = self.email_password
-        self.cfg["vault"]["config"]["ansible_python_interpreter"] = self.cfg[
-            "db"
-        ]["config"].get("ansible_python_interpreter", "/usr/bin/python3")
+        self.cfg["vault"]["config"]["ansible_python_interpreter"] = self.cfg["db"][
+            "config"
+        ].get("ansible_python_interpreter", "/usr/bin/python3")
         self.cfg["web"]["config"]["root_passwd"] = self.master_pass
         self.cfg["web"]["config"]["private_keyfile"] = self.private_key_file
         self.cfg["web"]["config"]["public_keyfile"] = self.public_key_file
-        self.cfg["web"]["config"]["apache_config_file"] = str(
-            self.apache_config
-        )
+        self.cfg["web"]["config"]["apache_config_file"] = str(self.apache_config)
         if ask_pass:
             self._prep_apache_config()
 
     def _prep_apache_config(self):
         with open(self.apache_config, "w") as f_obj:
-            f_obj.write(
-                (Path(asset_dir) / "web" / "freva_web.conf").read_text()
-            )
+            f_obj.write((Path(asset_dir) / "web" / "freva_web.conf").read_text())
 
     def _set_hostnames(self) -> None:
         """Set the hostnames from the config or if debug the alias."""
         default_ports = {"db": 3306, "freva_rest": 8080}
         if self.local_debug:
             for step in self.steps:
-                if (
-                    isinstance(self.cfg[step], dict)
-                    and "hosts" in self.cfg[step]
-                ):
+                if isinstance(self.cfg[step], dict) and "hosts" in self.cfg[step]:
                     self.cfg[step]["hosts"] = gethostbyname(gethostname())
                 if step in ("db", "freva_rest"):
                     self.cfg[step]["config"]["port"] = default_ports[step]
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self._td.cleanup()
 
     def _read_cfg(self) -> dict[str, Any]:
         try:
-            config = dict(load_config(self._inv_tmpl).items())
+            config = dict(load_config(self._inv_tmpl, convert=True).items())
             config["vault"] = deepcopy(config["db"])
             return config
         except FileNotFoundError:
-            raise ConfigurationError(
-                f"No such file {self._inv_tmpl}"
-            ) from None
+            raise ConfigurationError(f"No such file {self._inv_tmpl}") from None
         except KeyError:
             raise ConfigurationError("You must define a db section") from None
 
     def _check_config(self) -> None:
         sections = []
         config_keys = deepcopy(self._config_keys)
         if "db" in config_keys:
             config_keys.append("vault")
         for section in self.cfg.keys():
             for step in config_keys:
                 if section.startswith(step) and section not in sections:
                     sections.append(section)
         for section in sections:
             for key, value in self.cfg[section]["config"].items():
-                if (
-                    not value
-                    and not self._empty_ok
-                    and not isinstance(value, bool)
-                ):
+                if not value and not self._empty_ok and not isinstance(value, bool):
                     raise ConfigurationError(
                         f"{key} in {section} is empty in {self._inv_tmpl}"
                     ) from None
 
     @property
     def ask_become_password(self) -> bool:
         """Check if we have to ask for the sudo passwd at all."""
@@ -526,26 +473,22 @@
     def db_pass(self) -> str:
         """Create a password for the database."""
         if self._db_pass:
             return self._db_pass
         num_chars, num_digits = 30, 8
         num_chars -= num_digits
         characters = [
-            "".join(
-                [random.choice(string.ascii_letters) for i in range(num_chars)]
-            ),
+            "".join([random.choice(string.ascii_letters) for i in range(num_chars)]),
             "".join([random.choice(string.digits) for i in range(num_digits)]),
         ]
         str_characters = "".join(characters)
         _db_pass = "".join(random.sample(str_characters, len(str_characters)))
         while _db_pass.startswith("@"):
             # Vault treats values starting with "@" as file names.
-            _db_pass = "".join(
-                random.sample(str_characters, len(str_characters))
-            )
+            _db_pass = "".join(random.sample(str_characters, len(str_characters)))
         self._db_pass = _db_pass
         return self._db_pass
 
     @property
     def _needs_core(self) -> list[str]:
         """Define the steps that need the core config."""
         return ["web", "core"]
@@ -577,17 +520,15 @@
         )
         dump_file = self._get_files_copy(step)
         if dump_file:
             config[step]["vars"][f"{step}_dump"] = str(dump_file)
 
     def parse_config(self, steps: list[str]) -> str | None:
         """Create config files for anisble and evaluation_system.conf."""
-        versions = json.loads(
-            (Path(__file__).parent / "versions.json").read_text()
-        )
+        versions = json.loads((Path(__file__).parent / "versions.json").read_text())
         additional_steps = set(steps) - set(self.steps)
         if additional_steps:
             pprint(
                 "The following, [b]not selected[/b] steps will be auto "
                 f"updated.\n[green]{', '.join(additional_steps)}[/]"
             )
             time.sleep(3)
@@ -611,16 +552,16 @@
             for key, value in self.cfg[step]["config"].items():
                 if key in ("root_passwd",) or key.startswith(step):
                     new_key = key
                 else:
                     new_key = f"{step.replace('-', '_')}_{key}"
                 config[step]["vars"][new_key] = value
             config[step]["vars"]["project_name"] = self.project_name
-            config[step]["vars"][f"{step.replace('-', '_')}_version"] = (
-                versions.get(step, "")
+            config[step]["vars"][f"{step.replace('-', '_')}_version"] = versions.get(
+                step, ""
             )
             config[step]["vars"]["debug"] = self.local_debug
             # Add additional keys
             self._set_additional_config_values(step, config)
         if "freva_rest" in config:
             config["freva_rest"]["vars"]["solr_version"] = versions["solr"]
         for step in info:
@@ -706,36 +647,30 @@
                     if line.startswith(f"{step}.port"):
                         lines[num] = f"{step}.port={cfg}\n"
                     if line.startswith(f"{step}.host"):
                         lines[num] = f"{step}.host={self.cfg[step]['hosts']}\n"
                 if line.startswith("solr.host"):
                     lines[num] = f"solr.host={self.cfg[step]['hosts']}\n"
                 if line.startswith("db.host"):
-                    lines[num] = (
-                        f"db.host={self.cfg['db']['config']['host']}\n"
-                    )
+                    lines[num] = f"db.host={self.cfg['db']['config']['host']}\n"
         dump_file = self._get_files_copy("core")
         if dump_file:
             with dump_file.open("w") as f_obj:
                 f_obj.write("".join(lines))
 
     def get_ansible_password(self, ask_pass: bool = False) -> dict[str, str]:
         """The passwords for the ansible environments."""
         ssh_pass_msg = "Give the [b]ssh[/b] password for remote login"
-        sudo_pass_msg = (
-            "Give the password elevating user privilege ([b]sudo[/b])"
-        )
+        sudo_pass_msg = "Give the password elevating user privilege ([b]sudo[/b])"
         if ask_pass:
             sudo_pass_msg += ", defaults to ssh password"
         passwords = {}
         sudo_key = "^BECOME password.*:\\s*?$"
         ssh_key = "^SSH password:\\s*?$"
-        passwords[sudo_key] = (
-            os.environ.get("ANSIBLE_BECOME_PASSWORD", "") or ""
-        )
+        passwords[sudo_key] = os.environ.get("ANSIBLE_BECOME_PASSWORD", "") or ""
         passwords[ssh_key] = os.environ.get("ANSIBLE_SSH_PASSWORD", "") or ""
         if ask_pass and not passwords[ssh_key]:
             passwords[ssh_key] = Prompt.ask(
                 f"[green]{ssh_pass_msg}[/green]", password=True
             )
         if not passwords[sudo_key] and self.ask_become_password:
             passwords[sudo_key] = Prompt.ask(
@@ -758,21 +693,17 @@
             ssh key
         verbosity: int, default: 0
             Verbosity level, default 0
         ssh_port: int, default: 22
             Set the ssh port, in 99.9% of cases this should be left at port 22
         """
         try:
-            return self._play(
-                ask_pass=ask_pass, verbosity=verbosity, ssh_port=ssh_port
-            )
+            return self._play(ask_pass=ask_pass, verbosity=verbosity, ssh_port=ssh_port)
         except KeyboardInterrupt:
-            pprint(
-                " [red][ERROR]: User interrupted execution[/]", file=sys.stderr
-            )
+            pprint(" [red][ERROR]: User interrupted execution[/]", file=sys.stderr)
             raise KeyboardInterrupt() from None
 
     def get_steps_from_versions(
         self,
         envvars: dict[str, str],
         extravars: dict[str, str | int],
         cmdline: str,
@@ -897,17 +828,15 @@
         )
         inventory = self.parse_config(steps)
         if inventory is None:
             logger.info("Services up to date, nothing to do!")
             return None
         self.create_eval_config()
         logger.debug(inventory)
-        logger.info(
-            "Playing the playbooks for %s with ansible", ", ".join(self.steps)
-        )
+        logger.info("Playing the playbooks for %s with ansible", ", ".join(self.steps))
         logger.debug(self.playbooks)
         time.sleep(3)
         sig_handler = signal.getsignal(signal.SIGINT)
         try:
             result = run(
                 private_data_dir=str(self._td.parent_dir),
                 playbook=str(self._td.playbook_file),
@@ -917,13 +846,11 @@
                 extravars=extravars,
                 cmdline=cmdline,
                 verbosity=verbosity,
             )
         finally:
             signal.signal(signal.SIGINT, sig_handler)
         if result.status in ("timeout", "failed"):
-            raise DeploymentError(
-                f"Deployment not successful: {result.status}"
-            )
+            raise DeploymentError(f"Deployment not successful: {result.status}")
         elif result.status == "canceled":
             raise KeyboardInterrupt() from None
         return result
```

### Comparing `freva_deployment-2405.1.0/src/freva_deployment/error.py` & `freva_deployment-2405.1.1/src/freva_deployment/error.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/src/freva_deployment/keys.py` & `freva_deployment-2405.1.1/src/freva_deployment/keys.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/src/freva_deployment/logger.py` & `freva_deployment-2405.1.1/src/freva_deployment/logger.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/src/freva_deployment/runner.py` & `freva_deployment-2405.1.1/src/freva_deployment/runner.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/src/freva_deployment/ui/deployment_tui/__init__.py` & `freva_deployment-2405.1.1/src/freva_deployment/ui/deployment_tui/__init__.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/src/freva_deployment/ui/deployment_tui/base.py` & `freva_deployment-2405.1.1/src/freva_deployment/ui/deployment_tui/base.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/src/freva_deployment/ui/deployment_tui/deploy_forms.py` & `freva_deployment-2405.1.1/src/freva_deployment/ui/deployment_tui/deploy_forms.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/src/freva_deployment/ui/deployment_tui/main_window.py` & `freva_deployment-2405.1.1/src/freva_deployment/ui/deployment_tui/main_window.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/src/freva_deployment/utils.py` & `freva_deployment-2405.1.1/src/freva_deployment/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,22 +188,23 @@
         )
         backup_file.write_text(inp_file.read_text())
         _update_config(config_tmpl, config)
         inp_file.write_text(tomlkit.dumps(config_tmpl))
     return inp_file
 
 
-def load_config(inp_file: str | Path) -> dict[str, Any]:
+def load_config(inp_file: str | Path, convert: bool = False) -> dict[str, Any]:
     """Load the inventory toml file and replace all environment variables."""
     inp_file = _create_new_config(Path(inp_file).expanduser().absolute())
     variables = cast(
         dict[str, str], tomlkit.loads(config_file.read_text())["variables"]
     )
     config = tomlkit.loads(inp_file.read_text())
-    _convert_dict(config, variables, inp_file.parent)
+    if convert:
+        _convert_dict(config, variables, inp_file.parent)
     return config
 
 
 def get_setup_for_service(service: str, setups: list[ServiceInfo]) -> tuple[str, str]:
     """Get the setup of a service configuration."""
     for setup in setups:
         if setup.name == service:
```

### Comparing `freva_deployment-2405.1.0/src/freva_deployment/versions.py` & `freva_deployment-2405.1.1/src/freva_deployment/versions.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2405.1.0/PKG-INFO` & `freva_deployment-2405.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva-deployment
-Version: 2405.1.0
+Version: 2405.1.1
 Summary: Deployment of the Free Evaluation Framework Freva
 Author-email: "DKRZ, Clint" <freva@dkrz.de>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

