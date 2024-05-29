# Comparing `tmp/ansible-compat-4.1.8.tar.gz` & `tmp/ansible-compat-4.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-compat-4.1.8.tar", last modified: Tue Aug 29 11:23:17 2023, max compression
+gzip compressed data, was "ansible-compat-4.1.9.tar", last modified: Tue Sep  5 14:10:14 2023, max compression
```

## Comparing `ansible-compat-4.1.8.tar` & `ansible-compat-4.1.9.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.189220 ansible-compat-4.1.8/
--rw-r--r--   0 runner    (1001) docker     (999)      111 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (999)      145 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.181219 ansible-compat-4.1.8/.github/
--rw-r--r--   0 runner    (1001) docker     (999)       26 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (999)      162 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (999)      593 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (999)       69 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.181219 ansible-compat-4.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)      240 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (999)      244 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (999)      997 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (999)     3103 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1907 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)     1179 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.packit.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     3995 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (999)       75 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (999)      355 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1041 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.181219 ansible-compat-4.1.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (999)      458 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (999)     1359 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (999)      175 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/.yamllint
--rw-r--r--   0 runner    (1001) docker     (999)     1095 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     2244 2023-08-29 11:23:17.189220 ansible-compat-4.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      764 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (999)       90 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      123 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.181219 ansible-compat-4.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (999)      170 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.181219 ansible-compat-4.1.8/docs/images/
--rw-r--r--   0 runner    (1001) docker     (999)    15406 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (999)    10993 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (999)     1047 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (999)      360 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.173219 ansible-compat-4.1.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.181219 ansible-compat-4.1.8/examples/reqs_broken/
--rw-r--r--   0 runner    (1001) docker     (999)      125 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/examples/reqs_broken/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.181219 ansible-compat-4.1.8/examples/reqs_v1/
--rw-r--r--   0 runner    (1001) docker     (999)      179 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/examples/reqs_v1/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.181219 ansible-compat-4.1.8/examples/reqs_v2/
--rw-r--r--   0 runner    (1001) docker     (999)     7615 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/examples/reqs_v2/community-molecule-0.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (999)      393 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/examples/reqs_v2/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (999)     2265 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (999)     4493 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)      263 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (999)     6498 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-29 11:23:17.189220 ansible-compat-4.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.173219 ansible-compat-4.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.185219 ansible-compat-4.1.8/src/ansible_compat/
--rw-r--r--   0 runner    (1001) docker     (999)      246 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/src/ansible_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      160 2023-08-29 11:23:17.000000 ansible-compat-4.1.8/src/ansible_compat/_version.py
--rw-r--r--   0 runner    (1001) docker     (999)    15701 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/src/ansible_compat/config.py
--rw-r--r--   0 runner    (1001) docker     (999)     1574 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/src/ansible_compat/constants.py
--rw-r--r--   0 runner    (1001) docker     (999)     1559 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/src/ansible_compat/errors.py
--rw-r--r--   0 runner    (1001) docker     (999)      920 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/src/ansible_compat/loaders.py
--rw-r--r--   0 runner    (1001) docker     (999)      112 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/src/ansible_compat/ports.py
--rw-r--r--   0 runner    (1001) docker     (999)      807 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/src/ansible_compat/prerun.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/src/ansible_compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (999)    36955 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/src/ansible_compat/runtime.py
--rw-r--r--   0 runner    (1001) docker     (999)     3265 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/src/ansible_compat/schema.py
--rw-r--r--   0 runner    (1001) docker     (999)      552 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/src/ansible_compat/types.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.185219 ansible-compat-4.1.8/src/ansible_compat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     2244 2023-08-29 11:23:17.000000 ansible-compat-4.1.8/src/ansible_compat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2576 2023-08-29 11:23:17.000000 ansible-compat-4.1.8/src/ansible_compat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-29 11:23:17.000000 ansible-compat-4.1.8/src/ansible_compat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      253 2023-08-29 11:23:17.000000 ansible-compat-4.1.8/src/ansible_compat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       15 2023-08-29 11:23:17.000000 ansible-compat-4.1.8/src/ansible_compat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.185219 ansible-compat-4.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (999)       40 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.185219 ansible-compat-4.1.8/test/assets/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.173219 ansible-compat-4.1.8/test/assets/galaxy_paths/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.185219 ansible-compat-4.1.8/test/assets/galaxy_paths/.bar/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/assets/galaxy_paths/.bar/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.185219 ansible-compat-4.1.8/test/assets/galaxy_paths/foo/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/assets/galaxy_paths/foo/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (999)      102 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/assets/requirements-invalid-collection.yml
--rw-r--r--   0 runner    (1001) docker     (999)       98 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/assets/requirements-invalid-role.yml
--rw-r--r--   0 runner    (1001) docker     (999)       57 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/assets/validate0_data.json
--rw-r--r--   0 runner    (1001) docker     (999)      631 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/assets/validate0_expected.json
--rw-r--r--   0 runner    (1001) docker     (999)      184 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/assets/validate0_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.173219 ansible-compat-4.1.8/test/collections/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.185219 ansible-compat-4.1.8/test/collections/acme.broken/
--rw-r--r--   0 runner    (1001) docker     (999)       37 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/collections/acme.broken/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.185219 ansible-compat-4.1.8/test/collections/acme.goodies/
--rw-r--r--   0 runner    (1001) docker     (999)      681 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/collections/acme.goodies/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.173219 ansible-compat-4.1.8/test/collections/acme.goodies/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.185219 ansible-compat-4.1.8/test/collections/acme.goodies/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (999)      158 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/collections/acme.goodies/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)      142 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/collections/acme.goodies/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.173219 ansible-compat-4.1.8/test/collections/acme.goodies/roles/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.177219 ansible-compat-4.1.8/test/collections/acme.goodies/roles/baz/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.173219 ansible-compat-4.1.8/test/collections/acme.goodies/roles/baz/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.185219 ansible-compat-4.1.8/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
--rw-r--r--   0 runner    (1001) docker     (999)      156 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)      142 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.189220 ansible-compat-4.1.8/test/collections/acme.goodies/roles/baz/tasks/
--rw-r--r--   0 runner    (1001) docker     (999)       79 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/collections/acme.goodies/roles/baz/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.189220 ansible-compat-4.1.8/test/collections/acme.goodies/tests/
--rw-r--r--   0 runner    (1001) docker     (999)       58 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/collections/acme.goodies/tests/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (999)     3661 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.177219 ansible-compat-4.1.8/test/roles/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.189220 ansible-compat-4.1.8/test/roles/acme.missing_deps/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.189220 ansible-compat-4.1.8/test/roles/acme.missing_deps/meta/
--rw-r--r--   0 runner    (1001) docker     (999)      136 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/roles/acme.missing_deps/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (999)       87 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/roles/acme.missing_deps/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.177219 ansible-compat-4.1.8/test/roles/acme.sample2/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.189220 ansible-compat-4.1.8/test/roles/acme.sample2/meta/
--rw-r--r--   0 runner    (1001) docker     (999)      308 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/roles/acme.sample2/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.177219 ansible-compat-4.1.8/test/roles/ansible-role-sample/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.189220 ansible-compat-4.1.8/test/roles/ansible-role-sample/meta/
--rw-r--r--   0 runner    (1001) docker     (999)      259 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/roles/ansible-role-sample/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.177219 ansible-compat-4.1.8/test/roles/sample3/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.189220 ansible-compat-4.1.8/test/roles/sample3/meta/
--rw-r--r--   0 runner    (1001) docker     (999)      308 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/roles/sample3/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.177219 ansible-compat-4.1.8/test/roles/sample4/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.189220 ansible-compat-4.1.8/test/roles/sample4/meta/
--rw-r--r--   0 runner    (1001) docker     (999)      308 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/roles/sample4/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (999)      102 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (999)     2897 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (999)      430 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/test_configuration_example.py
--rw-r--r--   0 runner    (1001) docker     (999)      273 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (999)      341 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/test_prerun.py
--rw-r--r--   0 runner    (1001) docker     (999)    29523 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (999)      934 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/test_runtime_example.py
--rw-r--r--   0 runner    (1001) docker     (999)     3562 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/test_runtime_scan_path.py
--rw-r--r--   0 runner    (1001) docker     (999)     2377 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/test/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 11:23:17.189220 ansible-compat-4.1.8/tools/
--rwxr-xr-x   0 runner    (1001) docker     (999)      248 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/tools/get-version.sh
--rwxr-xr-x   0 runner    (1001) docker     (999)      240 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/tools/update-version.sh
--rw-r--r--   0 runner    (1001) docker     (999)     5067 2023-08-29 11:22:52.000000 ansible-compat-4.1.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/
+-rw-r--r--   0 runner    (1001) docker     (999)      111 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      145 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.055059 ansible-compat-4.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (999)       26 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (999)      162 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (999)      593 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (999)       69 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.055059 ansible-compat-4.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (999)      240 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      244 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      997 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (999)     3103 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (999)     1907 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (999)     1179 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.packit.yaml
+-rw-r--r--   0 runner    (1001) docker     (999)     3995 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (999)       75 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (999)      355 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (999)     1041 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.055059 ansible-compat-4.1.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (999)      458 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (999)     1359 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (999)      175 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (999)     1095 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)     2244 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      764 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (999)       90 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)      123 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.055059 ansible-compat-4.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (999)      170 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.055059 ansible-compat-4.1.9/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (999)    15406 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (999)    10993 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (999)     1047 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (999)      360 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.047059 ansible-compat-4.1.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.055059 ansible-compat-4.1.9/examples/reqs_broken/
+-rw-r--r--   0 runner    (1001) docker     (999)      125 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/examples/reqs_broken/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.055059 ansible-compat-4.1.9/examples/reqs_v1/
+-rw-r--r--   0 runner    (1001) docker     (999)      179 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/examples/reqs_v1/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.055059 ansible-compat-4.1.9/examples/reqs_v2/
+-rw-r--r--   0 runner    (1001) docker     (999)     7615 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/examples/reqs_v2/community-molecule-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (999)      814 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/examples/reqs_v2/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (999)     2265 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (999)     4493 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (999)      238 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (999)     6498 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.047059 ansible-compat-4.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.059059 ansible-compat-4.1.9/src/ansible_compat/
+-rw-r--r--   0 runner    (1001) docker     (999)      246 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/src/ansible_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      160 2023-09-05 14:10:13.000000 ansible-compat-4.1.9/src/ansible_compat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15701 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/src/ansible_compat/config.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1574 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/src/ansible_compat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1559 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/src/ansible_compat/errors.py
+-rw-r--r--   0 runner    (1001) docker     (999)      920 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/src/ansible_compat/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (999)      112 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/src/ansible_compat/ports.py
+-rw-r--r--   0 runner    (1001) docker     (999)      807 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/src/ansible_compat/prerun.py
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/src/ansible_compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (999)    37346 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/src/ansible_compat/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3265 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/src/ansible_compat/schema.py
+-rw-r--r--   0 runner    (1001) docker     (999)      552 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/src/ansible_compat/types.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.059059 ansible-compat-4.1.9/src/ansible_compat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     2244 2023-09-05 14:10:13.000000 ansible-compat-4.1.9/src/ansible_compat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     2576 2023-09-05 14:10:14.000000 ansible-compat-4.1.9/src/ansible_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-05 14:10:13.000000 ansible-compat-4.1.9/src/ansible_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      253 2023-09-05 14:10:13.000000 ansible-compat-4.1.9/src/ansible_compat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       15 2023-09-05 14:10:13.000000 ansible-compat-4.1.9/src/ansible_compat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.059059 ansible-compat-4.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (999)       40 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/test/assets/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.047059 ansible-compat-4.1.9/test/assets/galaxy_paths/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/test/assets/galaxy_paths/.bar/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/assets/galaxy_paths/.bar/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/test/assets/galaxy_paths/foo/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/assets/galaxy_paths/foo/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      102 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/assets/requirements-invalid-collection.yml
+-rw-r--r--   0 runner    (1001) docker     (999)       98 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/assets/requirements-invalid-role.yml
+-rw-r--r--   0 runner    (1001) docker     (999)       57 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/assets/validate0_data.json
+-rw-r--r--   0 runner    (1001) docker     (999)      631 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/assets/validate0_expected.json
+-rw-r--r--   0 runner    (1001) docker     (999)      184 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/assets/validate0_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.051059 ansible-compat-4.1.9/test/collections/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/test/collections/acme.broken/
+-rw-r--r--   0 runner    (1001) docker     (999)       37 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/collections/acme.broken/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/test/collections/acme.goodies/
+-rw-r--r--   0 runner    (1001) docker     (999)      681 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/collections/acme.goodies/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.051059 ansible-compat-4.1.9/test/collections/acme.goodies/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/test/collections/acme.goodies/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (999)      158 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/collections/acme.goodies/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      142 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/collections/acme.goodies/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.051059 ansible-compat-4.1.9/test/collections/acme.goodies/roles/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.051059 ansible-compat-4.1.9/test/collections/acme.goodies/roles/baz/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.051059 ansible-compat-4.1.9/test/collections/acme.goodies/roles/baz/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
+-rw-r--r--   0 runner    (1001) docker     (999)      156 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      142 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/test/collections/acme.goodies/roles/baz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (999)       79 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/collections/acme.goodies/roles/baz/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/test/collections/acme.goodies/tests/
+-rw-r--r--   0 runner    (1001) docker     (999)       58 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/collections/acme.goodies/tests/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (999)     3661 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.051059 ansible-compat-4.1.9/test/roles/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/test/roles/acme.missing_deps/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/test/roles/acme.missing_deps/meta/
+-rw-r--r--   0 runner    (1001) docker     (999)      136 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/roles/acme.missing_deps/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (999)       87 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/roles/acme.missing_deps/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.051059 ansible-compat-4.1.9/test/roles/acme.sample2/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/test/roles/acme.sample2/meta/
+-rw-r--r--   0 runner    (1001) docker     (999)      308 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/roles/acme.sample2/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.051059 ansible-compat-4.1.9/test/roles/ansible-role-sample/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/test/roles/ansible-role-sample/meta/
+-rw-r--r--   0 runner    (1001) docker     (999)      259 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/roles/ansible-role-sample/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.051059 ansible-compat-4.1.9/test/roles/sample3/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/test/roles/sample3/meta/
+-rw-r--r--   0 runner    (1001) docker     (999)      308 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/roles/sample3/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.051059 ansible-compat-4.1.9/test/roles/sample4/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/test/roles/sample4/meta/
+-rw-r--r--   0 runner    (1001) docker     (999)      308 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/roles/sample4/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (999)      102 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2897 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (999)      430 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/test_configuration_example.py
+-rw-r--r--   0 runner    (1001) docker     (999)      273 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (999)      341 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/test_prerun.py
+-rw-r--r--   0 runner    (1001) docker     (999)    29523 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (999)      934 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/test_runtime_example.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3562 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/test_runtime_scan_path.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2377 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/test/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 14:10:14.063059 ansible-compat-4.1.9/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (999)      248 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/tools/get-version.sh
+-rwxr-xr-x   0 runner    (1001) docker     (999)      240 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/tools/update-version.sh
+-rw-r--r--   0 runner    (1001) docker     (999)     5067 2023-09-05 14:09:45.000000 ansible-compat-4.1.9/tox.ini
```

### Comparing `ansible-compat-4.1.8/.github/dependabot.yml` & `ansible-compat-4.1.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/.github/workflows/release.yml` & `ansible-compat-4.1.9/.github/workflows/release.yml`

 * *Files 11% similar despite different names*

```diff
@@ -26,14 +26,14 @@
       - name: Switch to using Python 3.9 by default
         uses: actions/setup-python@v4
         with:
           python-version: 3.9
       - name: Install tox
         run: python3 -m pip install --user "tox>=4.0.0"
       - name: Check out src from Git
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0 # needed by setuptools-scm
       - name: Build dists
         run: python -m tox -e pkg
       - name: Publish to pypi.org
         uses: pypa/gh-action-pypi-publish@unstable/v1
```

### Comparing `ansible-compat-4.1.8/.github/workflows/tox.yml` & `ansible-compat-4.1.9/.github/workflows/tox.yml`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
       fail-fast: false
       matrix: ${{ fromJson(needs.pre.outputs.matrix) }}
     env:
       FORCE_COLOR: 1
 
     steps:
       - name: Check out src from Git
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0 # needed by setuptools-scm
 
       - name: Set up Python ${{ matrix.python_version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python_version }}
```

### Comparing `ansible-compat-4.1.8/.gitignore` & `ansible-compat-4.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/.packit.yaml` & `ansible-compat-4.1.9/.packit.yaml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/.pre-commit-config.yaml` & `ansible-compat-4.1.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
   python: python3.9
 exclude: |
   (?x)^(
     test/assets/.*
   )$
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.284"
+    rev: "v0.0.287"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/pre-commit/mirrors-prettier
     # keep it before yamllint
-    rev: "v3.0.1"
+    rev: "v3.0.3"
     hooks:
       - id: prettier
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
           - prettier-plugin-sort-json
   - repo: https://github.com/pre-commit/pre-commit-hooks.git
@@ -63,15 +63,15 @@
         entry: yamllint --strict
   - repo: https://github.com/psf/black
     rev: 23.7.0
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.4.1
+    rev: v1.5.1
     hooks:
       - id: mypy
         # empty args needed in order to match mypy cli behavior
         args: ["--strict"]
         additional_dependencies:
           - ansible-core
           - cached_property
@@ -80,15 +80,15 @@
           - pytest-mock
           - subprocess-tee>=0.4.1
           - "typing-extensions>=4.5.0;python_version<'3.10'"
           - types-PyYAML
           - types-pkg_resources
           - types-jsonschema>=4.4.9
   - repo: https://github.com/pycqa/pylint
-    rev: v3.0.0a6
+    rev: v3.0.0a7
     hooks:
       - id: pylint
         additional_dependencies:
           - PyYAML
           - pytest
           - typing_extensions
   # Keep last due to being considerably slower than the others:
```

### Comparing `ansible-compat-4.1.8/.readthedocs.yml` & `ansible-compat-4.1.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/.vscode/settings.json` & `ansible-compat-4.1.9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/LICENSE` & `ansible-compat-4.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/PKG-INFO` & `ansible-compat-4.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.1.8
+Version: 4.1.9
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.1.8/README.md` & `ansible-compat-4.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/docs/images/favicon.ico` & `ansible-compat-4.1.9/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/docs/images/logo.png` & `ansible-compat-4.1.9/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/docs/images/logo.svg` & `ansible-compat-4.1.9/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/examples/reqs_v2/community-molecule-0.1.0.tar.gz` & `ansible-compat-4.1.9/examples/reqs_v2/community-molecule-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/mkdocs.yml` & `ansible-compat-4.1.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/pyproject.toml` & `ansible-compat-4.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/requirements.txt` & `ansible-compat-4.1.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/src/ansible_compat/config.py` & `ansible-compat-4.1.9/src/ansible_compat/config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/src/ansible_compat/constants.py` & `ansible-compat-4.1.9/src/ansible_compat/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/src/ansible_compat/errors.py` & `ansible-compat-4.1.9/src/ansible_compat/errors.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/src/ansible_compat/loaders.py` & `ansible-compat-4.1.9/src/ansible_compat/loaders.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/src/ansible_compat/prerun.py` & `ansible-compat-4.1.9/src/ansible_compat/prerun.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/src/ansible_compat/runtime.py` & `ansible-compat-4.1.9/src/ansible_compat/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         """Add the sys.path to the collection paths."""
         if not self.isolated and self.config.collections_scan_sys_path:
             for path in sys.path:
                 if (
                     path not in self.config.collections_paths
                     and (Path(path) / "ansible_collections").is_dir()
                 ):
-                    self.config.collections_paths.append(  # noqa: PERF401 pylint: disable=E1101
+                    self.config.collections_paths.append(  # pylint: disable=E1101
                         path,
                     )
 
     def load_collections(self) -> None:
         """Load collection data."""
         self.collections = OrderedDict()
         no_collections_msg = "None of the provided paths were usable"
@@ -551,14 +551,21 @@
         if "collections" in reqs_yaml:
             cmd = [
                 "ansible-galaxy",
                 "collection",
                 "install",
                 "-v",
             ]
+            for collection in reqs_yaml["collections"]:
+                if isinstance(collection, dict) and collection.get("type", "") == "git":
+                    _logger.info(
+                        "Adding '--pre' to ansible-galaxy collection install because we detected one collection being sourced from git.",
+                    )
+                    cmd.append("--pre")
+                    break
             if offline:
                 _logger.warning(
                     "Skipped installing collection dependencies due to running in offline mode.",
                 )
             else:
                 cmd.extend(["-r", str(requirement)])
                 cpaths = self.config.collections_paths
```

### Comparing `ansible-compat-4.1.8/src/ansible_compat/schema.py` & `ansible-compat-4.1.9/src/ansible_compat/schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/src/ansible_compat/types.py` & `ansible-compat-4.1.9/src/ansible_compat/types.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/src/ansible_compat.egg-info/PKG-INFO` & `ansible-compat-4.1.9/src/ansible_compat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.1.8
+Version: 4.1.9
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.1.8/src/ansible_compat.egg-info/SOURCES.txt` & `ansible-compat-4.1.9/src/ansible_compat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/test/assets/validate0_expected.json` & `ansible-compat-4.1.9/test/assets/validate0_expected.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/test/collections/acme.goodies/galaxy.yml` & `ansible-compat-4.1.9/test/collections/acme.goodies/galaxy.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/test/conftest.py` & `ansible-compat-4.1.9/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/test/test_config.py` & `ansible-compat-4.1.9/test/test_config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/test/test_runtime.py` & `ansible-compat-4.1.9/test/test_runtime.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/test/test_runtime_example.py` & `ansible-compat-4.1.9/test/test_runtime_example.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/test/test_runtime_scan_path.py` & `ansible-compat-4.1.9/test/test_runtime_scan_path.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/test/test_schema.py` & `ansible-compat-4.1.9/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.8/tox.ini` & `ansible-compat-4.1.9/tox.ini`

 * *Files identical despite different names*

