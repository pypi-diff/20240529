# Comparing `tmp/iac_init-0.8.3.tar.gz` & `tmp/iac_init-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.8.3.tar", max compression
+gzip compressed data, was "iac_init-0.8.4.tar", max compression
```

## Comparing `iac_init-0.8.3.tar` & `iac_init-0.8.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    16295 2024-05-29 09:37:22.132596 iac_init-0.8.3/LICENSE
--rw-r--r--   0        0        0        0 2024-05-29 09:37:22.132596 iac_init-0.8.3/README.md
--rw-r--r--   0        0        0      392 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/__main__.py
--rw-r--r--   0        0        0    13636 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/cli/main.py
--rw-r--r--   0        0        0      228 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/cli/options.py
--rw-r--r--   0        0        0     1827 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     1166 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0     1583 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2847 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     7992 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      443 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0     1871 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0      336 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/scripts/thread_tool.py
--rw-r--r--   0        0        0     3778 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6989 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1370 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1557 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-05-29 09:37:22.132596 iac_init-0.8.3/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/templates/03-nac-tasks/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/templates/03-nac-tasks/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/templates/03-nac-tasks/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/templates/03-nac-tasks/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/templates/03-nac-tasks/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/templates/03-nac-tasks/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4924 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/utils/functional.py
--rw-r--r--   0        0        0    14188 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/validator.py
--rw-r--r--   0        0        0     5269 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5542 2024-05-29 09:37:22.136596 iac_init-0.8.3/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1636 2024-05-29 09:37:22.136596 iac_init-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-05-29 10:15:27.855421 iac_init-0.8.4/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-29 10:15:27.855421 iac_init-0.8.4/README.md
+-rw-r--r--   0        0        0      392 2024-05-29 10:15:27.855421 iac_init-0.8.4/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-29 10:15:27.855421 iac_init-0.8.4/iac_init/__main__.py
+-rw-r--r--   0        0        0    13438 2024-05-29 10:15:27.855421 iac_init-0.8.4/iac_init/cli/main.py
+-rw-r--r--   0        0        0      228 2024-05-29 10:15:27.855421 iac_init-0.8.4/iac_init/cli/options.py
+-rw-r--r--   0        0        0     1827 2024-05-29 10:15:27.855421 iac_init-0.8.4/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     1166 2024-05-29 10:15:27.855421 iac_init-0.8.4/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0     1583 2024-05-29 10:15:27.855421 iac_init-0.8.4/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2847 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     7992 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      443 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0     1871 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0      336 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/scripts/thread_tool.py
+-rw-r--r--   0        0        0     3778 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6989 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1370 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1557 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-05-29 10:15:27.859421 iac_init-0.8.4/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-05-29 10:15:27.863421 iac_init-0.8.4/iac_init/templates/03-nac-tasks/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-29 10:15:27.863421 iac_init-0.8.4/iac_init/templates/03-nac-tasks/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-29 10:15:27.863421 iac_init-0.8.4/iac_init/templates/03-nac-tasks/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-29 10:15:27.863421 iac_init-0.8.4/iac_init/templates/03-nac-tasks/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-29 10:15:27.863421 iac_init-0.8.4/iac_init/templates/03-nac-tasks/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-29 10:15:27.863421 iac_init-0.8.4/iac_init/templates/03-nac-tasks/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-05-29 10:15:27.863421 iac_init-0.8.4/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4924 2024-05-29 10:15:27.863421 iac_init-0.8.4/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    14664 2024-05-29 10:15:27.863421 iac_init-0.8.4/iac_init/validator.py
+-rw-r--r--   0        0        0     5269 2024-05-29 10:15:27.863421 iac_init-0.8.4/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5542 2024-05-29 10:15:27.863421 iac_init-0.8.4/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1636 2024-05-29 10:15:27.863421 iac_init-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.8.4/PKG-INFO
```

### Comparing `iac_init-0.8.3/LICENSE` & `iac_init-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/cli/main.py` & `iac_init-0.8.4/iac_init/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,26 +280,24 @@
                     output,
                     os.path.basename(settings.TEMPLATE_DIR[int(option)-1]),
                     'host_vars',
                     'apic1'
                 )
                 if os.path.exists(dir_path) and os.path.isdir(dir_path):
                     yaml_cp_output_path = os.path.join(
-                        dir_path
+                        dir_path,
+                        'data.yaml'
                     )
-                    for oyp in option_yaml_path:
-                        shutil.copy(
-                            oyp,
-                            os.path.join(
-                                yaml_cp_output_path,
-                                os.path.basename(oyp)
-                            )
-                        )
-                        logger.info("Copied Yaml {} to {} success."
-                                    .format(oyp, yaml_cp_output_path))
+                    result = validator.write_output(
+                        option_yaml_path,
+                        yaml_cp_output_path
+                    )
+                    if not result:
+                        exit()
+
             except Exception as e:
                 msg = "Generate working directory fail, detail: {}"\
                     .format(e)
                 logger.error(msg)
                 exit()
 
             try:
```

### Comparing `iac_init-0.8.3/iac_init/conf/__init__.py` & `iac_init-0.8.4/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/conf/global_settings.py` & `iac_init-0.8.4/iac_init/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/scripts/ansible_tool.py` & `iac_init-0.8.4/iac_init/scripts/ansible_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.8.4/iac_init/scripts/apic_connecton_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.8.4/iac_init/scripts/cimc_precheck_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/scripts/telnet_tool.py` & `iac_init-0.8.4/iac_init/scripts/telnet_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.8.4/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.8.4/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.8.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.8.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.8.4/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/utils/functional.py` & `iac_init-0.8.4/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/validator.py` & `iac_init-0.8.4/iac_init/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 # Copyright: (c) 2022, Wang Xiao <xiawang3@cisco.com>
 
 import os
 import re
 import time
-import yaml
+from ruamel import yaml
 
 from loguru import logger
 from typing import Any, Dict, List, Optional
 
 from iac_init.conf import settings
 from iac_init.yaml_conf.yaml import load_yaml_files
 from iac_init.scripts.ssh_tool import check_ssh_connection
@@ -331,31 +331,31 @@
             logger.error(msg)
             self.errors.append(msg)
             return False
 
     # This function is used for option 3.
     def validate_yaml_dir_exist(self, yaml_dir):
         try:
-            file_dir_list = []
+            self.file_dir_list = []
             folder_path = os.path.join(self.data_path, yaml_dir)
             if os.path.exists(folder_path) and os.path.isdir(folder_path):
                 for dir, _, files in os.walk(folder_path):
                     for filename in files:
                         option3_yaml_path = os.path.join(dir, filename)
                         if option3_yaml_path:
-                            file_dir_list.append(option3_yaml_path)
+                            self.file_dir_list.append(option3_yaml_path)
             else:
                 msg = "Validate Error: Directory {} not exist."\
                     .format(folder_path)
                 logger.error(msg)
                 self.errors.append(msg)
                 return False
 
-            if file_dir_list:
-                return file_dir_list
+            if self.file_dir_list:
+                return self.file_dir_list
             else:
                 msg = "Validate Error: No file fount in dir: {}"\
                     .format(folder_path)
                 logger.error(msg)
                 self.errors.append(msg)
                 return False
         except Exception as e:
@@ -387,7 +387,21 @@
         return True
 
     def _validate_bool(self, bool):
         if bool == "yes":
             pass
         else:
             exit(1)
+
+    def write_output(self, input_paths: List[str], path: str):
+        if self.data is None:
+            self.data = load_yaml_files(input_paths)
+        try:
+            with open(path, "w") as fh:
+                y = yaml.YAML()
+                y.default_flow_style = False
+                y.dump(self.data, fh)
+            return True
+
+        except:
+            logger.error("Cannot write file: {}".format(path))
+            return False
```

### Comparing `iac_init-0.8.3/iac_init/yaml_conf/yaml.py` & `iac_init-0.8.4/iac_init/yaml_conf/yaml.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.8.4/iac_init/yaml_conf/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.8.3/pyproject.toml` & `iac_init-0.8.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.8.3"
+version = "0.8.4"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.8.3/PKG-INFO` & `iac_init-0.8.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.8.3
+Version: 0.8.4
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

