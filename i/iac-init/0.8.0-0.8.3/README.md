# Comparing `tmp/iac_init-0.8.0.tar.gz` & `tmp/iac_init-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.8.0.tar", max compression
+gzip compressed data, was "iac_init-0.8.3.tar", max compression
```

## Comparing `iac_init-0.8.0.tar` & `iac_init-0.8.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    16295 2024-05-29 09:25:19.634145 iac_init-0.8.0/LICENSE
--rw-r--r--   0        0        0        0 2024-05-29 09:25:19.634145 iac_init-0.8.0/README.md
--rw-r--r--   0        0        0      392 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/__main__.py
--rwxr-xr-x   0        0        0   727848 2024-05-29 09:25:35.526234 iac_init-0.8.0/iac_init/cli/main.so
--rwxr-xr-x   0        0        0    69824 2024-05-29 09:25:35.746235 iac_init-0.8.0/iac_init/cli/options.so
--rw-r--r--   0        0        0     1827 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/conf/__init__.py
--rwxr-xr-x   0        0        0   103464 2024-05-29 09:25:36.086237 iac_init-0.8.0/iac_init/conf/global_settings.so
--rwxr-xr-x   0        0        0   246168 2024-05-29 09:25:39.806259 iac_init-0.8.0/iac_init/scripts/ansible_tool.so
--rwxr-xr-x   0        0        0   294536 2024-05-29 09:25:41.658285 iac_init-0.8.0/iac_init/scripts/apic_connecton_tool.so
--rwxr-xr-x   0        0        0   675792 2024-05-29 09:25:38.538251 iac_init-0.8.0/iac_init/scripts/cimc_precheck_tool.so
--rwxr-xr-x   0        0        0   168632 2024-05-29 09:25:42.190292 iac_init-0.8.0/iac_init/scripts/ssh_tool.so
--rwxr-xr-x   0        0        0   269536 2024-05-29 09:25:40.662271 iac_init-0.8.0/iac_init/scripts/telnet_tool.so
--rwxr-xr-x   0        0        0   156336 2024-05-29 09:25:39.018254 iac_init-0.8.0/iac_init/scripts/thread_tool.so
--rw-r--r--   0        0        0     3778 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6989 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1370 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1557 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-05-29 09:25:19.634145 iac_init-0.8.0/iac_init/templates/03-nac-tasks/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-29 09:25:19.638145 iac_init-0.8.0/iac_init/templates/03-nac-tasks/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-29 09:25:19.638145 iac_init-0.8.0/iac_init/templates/03-nac-tasks/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-29 09:25:19.638145 iac_init-0.8.0/iac_init/templates/03-nac-tasks/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-29 09:25:19.638145 iac_init-0.8.0/iac_init/templates/03-nac-tasks/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-29 09:25:19.638145 iac_init-0.8.0/iac_init/templates/03-nac-tasks/inventory.yaml.j2
--rwxr-xr-x   0        0        0    62360 2024-05-29 09:25:27.270187 iac_init-0.8.0/iac_init/utils/exceptions.so
--rwxr-xr-x   0        0        0   333200 2024-05-29 09:25:27.082186 iac_init-0.8.0/iac_init/utils/functional.so
--rwxr-xr-x   0        0        0  1043320 2024-05-29 09:25:26.026179 iac_init-0.8.0/iac_init/validator.so
--rwxr-xr-x   0        0        0   503352 2024-05-29 09:25:29.018197 iac_init-0.8.0/iac_init/yaml_conf/yaml.so
--rwxr-xr-x   0        0        0   600936 2024-05-29 09:25:31.426210 iac_init-0.8.0/iac_init/yaml_conf/yaml_writer.so
--rw-r--r--   0        0        0     1636 2024-05-29 09:25:19.638145 iac_init-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-05-29 09:37:22.132596 iac_init-0.8.3/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-29 09:37:22.132596 iac_init-0.8.3/README.md
+-rw-r--r--   0        0        0      392 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/__main__.py
+-rw-r--r--   0        0        0    13636 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/cli/main.py
+-rw-r--r--   0        0        0      228 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/cli/options.py
+-rw-r--r--   0        0        0     1827 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     1166 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0     1583 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2847 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     7992 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      443 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0     1871 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0      336 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/scripts/thread_tool.py
+-rw-r--r--   0        0        0     3778 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6989 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1370 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1557 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/templates/03-nac-tasks/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/templates/03-nac-tasks/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/templates/03-nac-tasks/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/templates/03-nac-tasks/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/templates/03-nac-tasks/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/templates/03-nac-tasks/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4924 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    14188 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/validator.py
+-rw-r--r--   0        0        0     5269 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5542 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1636 2024-05-29 09:37:22.136596 iac_init-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.8.3/PKG-INFO
```

### Comparing `iac_init-0.8.0/LICENSE` & `iac_init-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/iac_init/conf/__init__.py` & `iac_init-0.8.3/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.0/pyproject.toml` & `iac_init-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.8.0"
+version = "0.8.3"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.8.0/PKG-INFO` & `iac_init-0.8.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.8.0
+Version: 0.8.3
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

