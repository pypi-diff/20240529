# Comparing `tmp/mypy-boto3-securityhub-1.34.76.tar.gz` & `tmp/mypy_boto3_securityhub-1.34.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-securityhub-1.34.76.tar", last modified: Tue Apr  2 19:32:32 2024, max compression
+gzip compressed data, was "mypy_boto3_securityhub-1.34.96.tar", last modified: Wed May  1 19:21:16 2024, max compression
```

## Comparing `mypy-boto3-securityhub-1.34.76.tar` & `mypy_boto3_securityhub-1.34.96.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:32.495226 mypy-boto3-securityhub-1.34.76/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-04-02 19:32:32.491227 mypy-boto3-securityhub-1.34.76/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:32.491227 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61446 2024-04-02 19:32:11.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    61443 2024-04-02 19:32:11.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16100 2024-04-02 19:32:11.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16100 2024-04-02 19:32:11.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20877 2024-04-02 19:32:11.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    20859 2024-04-02 19:32:11.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   475828 2024-04-02 19:32:20.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   475828 2024-04-02 19:32:17.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:32.491227 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-04-02 19:32:32.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-02 19:32:32.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:32:32.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:32:32.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:32:32.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 19:32:32.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:32:32.495226 mypy-boto3-securityhub-1.34.76/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:16.712331 mypy_boto3_securityhub-1.34.96/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 19:20:49.000000 mypy_boto3_securityhub-1.34.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-05-01 19:21:16.712331 mypy_boto3_securityhub-1.34.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-05-01 19:20:49.000000 mypy_boto3_securityhub-1.34.96/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:16.712331 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-01 19:20:49.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-01 19:20:49.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-01 19:20:49.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61538 2024-05-01 19:20:49.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61535 2024-05-01 19:20:49.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16145 2024-05-01 19:20:50.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16145 2024-05-01 19:20:50.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20869 2024-05-01 19:20:49.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20851 2024-05-01 19:20:49.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:20:49.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   636411 2024-05-01 19:21:01.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   636411 2024-05-01 19:20:58.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 19:20:49.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:21:16.712331 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-05-01 19:21:16.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-01 19:21:16.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:16.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:21:16.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 19:21:16.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 19:21:16.000000 mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:21:16.712331 mypy_boto3_securityhub-1.34.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-01 19:20:49.000000 mypy_boto3_securityhub-1.34.96/setup.py
```

### Comparing `mypy-boto3-securityhub-1.34.76/LICENSE` & `mypy_boto3_securityhub-1.34.96/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.34.76/PKG-INFO` & `mypy_boto3_securityhub-1.34.96/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securityhub
-Version: 1.34.76
-Summary: Type annotations for boto3.SecurityHub 1.34.76 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.96
+Summary: Type annotations for boto3.SecurityHub 1.34.96 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securityhub)](https://pepy.tech/project/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-securityhub-1.34.76/README.md` & `mypy_boto3_securityhub-1.34.96/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securityhub)](https://pepy.tech/project/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/__init__.py` & `mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/__init__.pyi` & `mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/__main__.py` & `mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecurityHub 1.34.76\n"
-        "Version:         1.34.76\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.SecurityHub 1.34.96\n"
+        "Version:         1.34.96\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.76")
+    print("1.34.96")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/client.py` & `mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,19 +45,19 @@
     ListOrganizationAdminAccountsPaginator,
     ListSecurityControlDefinitionsPaginator,
     ListStandardsControlAssociationsPaginator,
 )
 from .type_defs import (
     AccountDetailsTypeDef,
     AssociationFiltersTypeDef,
-    AutomationRulesActionTypeDef,
-    AutomationRulesFindingFiltersTypeDef,
-    AwsSecurityFindingFiltersTypeDef,
+    AutomationRulesActionUnionTypeDef,
+    AutomationRulesFindingFiltersUnionTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
-    AwsSecurityFindingTypeDef,
+    AwsSecurityFindingUnionTypeDef,
     BatchDeleteAutomationRulesResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     BatchGetAutomationRulesResponseTypeDef,
     BatchGetConfigurationPolicyAssociationsResponseTypeDef,
     BatchGetSecurityControlsResponseTypeDef,
     BatchGetStandardsControlAssociationsResponseTypeDef,
@@ -107,16 +107,16 @@
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
     ListSecurityControlDefinitionsResponseTypeDef,
     ListStandardsControlAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NoteUpdateTypeDef,
     OrganizationConfigurationTypeDef,
-    ParameterConfigurationTypeDef,
-    PolicyTypeDef,
+    ParameterConfigurationUnionTypeDef,
+    PolicyUnionTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     SortCriterionTypeDef,
     StandardsControlAssociationIdTypeDef,
     StandardsControlAssociationUpdateTypeDef,
     StandardsSubscriptionRequestTypeDef,
     StartConfigurationPolicyAssociationResponseTypeDef,
@@ -270,15 +270,15 @@
         standard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_standards_control_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_standards_control_associations)
         """
 
     def batch_import_findings(
-        self, *, Findings: Sequence[AwsSecurityFindingTypeDef]
+        self, *, Findings: Sequence[AwsSecurityFindingUnionTypeDef]
     ) -> BatchImportFindingsResponseTypeDef:
         """
         Imports security findings generated by a finding provider into Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_import_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_import_findings)
         """
@@ -362,16 +362,16 @@
 
     def create_automation_rule(
         self,
         *,
         RuleOrder: int,
         RuleName: str,
         Description: str,
-        Criteria: AutomationRulesFindingFiltersTypeDef,
-        Actions: Sequence[AutomationRulesActionTypeDef],
+        Criteria: AutomationRulesFindingFiltersUnionTypeDef,
+        Actions: Sequence[AutomationRulesActionUnionTypeDef],
         Tags: Mapping[str, str] = ...,
         RuleStatus: RuleStatusType = ...,
         IsTerminal: bool = ...,
     ) -> CreateAutomationRuleResponseTypeDef:
         """
         Creates an automation rule based on input parameters.
 
@@ -379,15 +379,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_automation_rule)
         """
 
     def create_configuration_policy(
         self,
         *,
         Name: str,
-        ConfigurationPolicy: PolicyTypeDef,
+        ConfigurationPolicy: PolicyUnionTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
     ) -> CreateConfigurationPolicyResponseTypeDef:
         """
         Creates a configuration policy with the defined configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_configuration_policy)
@@ -401,15 +401,15 @@
         Used to enable finding aggregation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_finding_aggregator)
         """
 
     def create_insight(
-        self, *, Name: str, Filters: AwsSecurityFindingFiltersTypeDef, GroupByAttribute: str
+        self, *, Name: str, Filters: AwsSecurityFindingFiltersUnionTypeDef, GroupByAttribute: str
     ) -> CreateInsightResponseTypeDef:
         """
         Creates a custom insight in Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_insight)
         """
@@ -716,15 +716,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_finding_history)
         """
 
     def get_findings(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
     ) -> GetFindingsResponseTypeDef:
         """
         Returns a list of findings that match the specified criteria.
 
@@ -976,15 +976,15 @@
     def update_configuration_policy(
         self,
         *,
         Identifier: str,
         Name: str = ...,
         Description: str = ...,
         UpdatedReason: str = ...,
-        ConfigurationPolicy: PolicyTypeDef = ...,
+        ConfigurationPolicy: PolicyUnionTypeDef = ...,
     ) -> UpdateConfigurationPolicyResponseTypeDef:
         """
         Updates a configuration policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_configuration_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_configuration_policy)
         """
@@ -998,31 +998,31 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_finding_aggregator)
         """
 
     def update_findings(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef,
         Note: NoteUpdateTypeDef = ...,
         RecordState: RecordStateType = ...,
     ) -> Dict[str, Any]:
         """
-        `UpdateFindings` is deprecated.
+        `UpdateFindings` is a deprecated operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_findings)
         """
 
     def update_insight(
         self,
         *,
         InsightArn: str,
         Name: str = ...,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         GroupByAttribute: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the Security Hub insight identified by the specified insight ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_insight)
@@ -1042,15 +1042,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_organization_configuration)
         """
 
     def update_security_control(
         self,
         *,
         SecurityControlId: str,
-        Parameters: Mapping[str, ParameterConfigurationTypeDef],
+        Parameters: Mapping[str, ParameterConfigurationUnionTypeDef],
         LastUpdateReason: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the properties of a security control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_security_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_security_control)
```

### Comparing `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/client.pyi` & `mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -45,19 +45,19 @@
     ListOrganizationAdminAccountsPaginator,
     ListSecurityControlDefinitionsPaginator,
     ListStandardsControlAssociationsPaginator,
 )
 from .type_defs import (
     AccountDetailsTypeDef,
     AssociationFiltersTypeDef,
-    AutomationRulesActionTypeDef,
-    AutomationRulesFindingFiltersTypeDef,
-    AwsSecurityFindingFiltersTypeDef,
+    AutomationRulesActionUnionTypeDef,
+    AutomationRulesFindingFiltersUnionTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
-    AwsSecurityFindingTypeDef,
+    AwsSecurityFindingUnionTypeDef,
     BatchDeleteAutomationRulesResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     BatchGetAutomationRulesResponseTypeDef,
     BatchGetConfigurationPolicyAssociationsResponseTypeDef,
     BatchGetSecurityControlsResponseTypeDef,
     BatchGetStandardsControlAssociationsResponseTypeDef,
@@ -107,16 +107,16 @@
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
     ListSecurityControlDefinitionsResponseTypeDef,
     ListStandardsControlAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NoteUpdateTypeDef,
     OrganizationConfigurationTypeDef,
-    ParameterConfigurationTypeDef,
-    PolicyTypeDef,
+    ParameterConfigurationUnionTypeDef,
+    PolicyUnionTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     SortCriterionTypeDef,
     StandardsControlAssociationIdTypeDef,
     StandardsControlAssociationUpdateTypeDef,
     StandardsSubscriptionRequestTypeDef,
     StartConfigurationPolicyAssociationResponseTypeDef,
@@ -267,15 +267,15 @@
         standard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_standards_control_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_standards_control_associations)
         """
 
     def batch_import_findings(
-        self, *, Findings: Sequence[AwsSecurityFindingTypeDef]
+        self, *, Findings: Sequence[AwsSecurityFindingUnionTypeDef]
     ) -> BatchImportFindingsResponseTypeDef:
         """
         Imports security findings generated by a finding provider into Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_import_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_import_findings)
         """
@@ -359,16 +359,16 @@
 
     def create_automation_rule(
         self,
         *,
         RuleOrder: int,
         RuleName: str,
         Description: str,
-        Criteria: AutomationRulesFindingFiltersTypeDef,
-        Actions: Sequence[AutomationRulesActionTypeDef],
+        Criteria: AutomationRulesFindingFiltersUnionTypeDef,
+        Actions: Sequence[AutomationRulesActionUnionTypeDef],
         Tags: Mapping[str, str] = ...,
         RuleStatus: RuleStatusType = ...,
         IsTerminal: bool = ...,
     ) -> CreateAutomationRuleResponseTypeDef:
         """
         Creates an automation rule based on input parameters.
 
@@ -376,15 +376,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_automation_rule)
         """
 
     def create_configuration_policy(
         self,
         *,
         Name: str,
-        ConfigurationPolicy: PolicyTypeDef,
+        ConfigurationPolicy: PolicyUnionTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
     ) -> CreateConfigurationPolicyResponseTypeDef:
         """
         Creates a configuration policy with the defined configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_configuration_policy)
@@ -398,15 +398,15 @@
         Used to enable finding aggregation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_finding_aggregator)
         """
 
     def create_insight(
-        self, *, Name: str, Filters: AwsSecurityFindingFiltersTypeDef, GroupByAttribute: str
+        self, *, Name: str, Filters: AwsSecurityFindingFiltersUnionTypeDef, GroupByAttribute: str
     ) -> CreateInsightResponseTypeDef:
         """
         Creates a custom insight in Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.create_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#create_insight)
         """
@@ -713,15 +713,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_finding_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_finding_history)
         """
 
     def get_findings(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
     ) -> GetFindingsResponseTypeDef:
         """
         Returns a list of findings that match the specified criteria.
 
@@ -973,15 +973,15 @@
     def update_configuration_policy(
         self,
         *,
         Identifier: str,
         Name: str = ...,
         Description: str = ...,
         UpdatedReason: str = ...,
-        ConfigurationPolicy: PolicyTypeDef = ...,
+        ConfigurationPolicy: PolicyUnionTypeDef = ...,
     ) -> UpdateConfigurationPolicyResponseTypeDef:
         """
         Updates a configuration policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_configuration_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_configuration_policy)
         """
@@ -995,31 +995,31 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_finding_aggregator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_finding_aggregator)
         """
 
     def update_findings(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef,
         Note: NoteUpdateTypeDef = ...,
         RecordState: RecordStateType = ...,
     ) -> Dict[str, Any]:
         """
-        `UpdateFindings` is deprecated.
+        `UpdateFindings` is a deprecated operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_findings)
         """
 
     def update_insight(
         self,
         *,
         InsightArn: str,
         Name: str = ...,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         GroupByAttribute: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the Security Hub insight identified by the specified insight ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_insight)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_insight)
@@ -1039,15 +1039,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_organization_configuration)
         """
 
     def update_security_control(
         self,
         *,
         SecurityControlId: str,
-        Parameters: Mapping[str, ParameterConfigurationTypeDef],
+        Parameters: Mapping[str, ParameterConfigurationUnionTypeDef],
         LastUpdateReason: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the properties of a security control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_security_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_security_control)
```

### Comparing `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/literals.py` & `mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,14 +270,15 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
@@ -485,14 +486,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/literals.pyi` & `mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -270,14 +270,15 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
@@ -485,14 +486,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/paginator.py` & `mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,23 @@
 
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     AssociationFiltersTypeDef,
-    AwsSecurityFindingFiltersTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
     DescribeActionTargetsResponseTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
     DescribeStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     GetFindingHistoryResponseTypeDef,
-    GetFindingsResponsePaginatorTypeDef,
+    GetFindingsResponseTypeDef,
     GetInsightsResponseTypeDef,
     ListConfigurationPoliciesResponseTypeDef,
     ListConfigurationPolicyAssociationsResponseTypeDef,
     ListEnabledProductsForImportResponseTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListMembersResponseTypeDef,
@@ -218,18 +218,18 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[GetFindingsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
         """
 
 
 class GetInsightsPaginator(Paginator):
```

### Comparing `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/paginator.pyi` & `mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -54,23 +54,23 @@
 
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     AssociationFiltersTypeDef,
-    AwsSecurityFindingFiltersTypeDef,
+    AwsSecurityFindingFiltersUnionTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
     DescribeActionTargetsResponseTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
     DescribeStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     GetFindingHistoryResponseTypeDef,
-    GetFindingsResponsePaginatorTypeDef,
+    GetFindingsResponseTypeDef,
     GetInsightsResponseTypeDef,
     ListConfigurationPoliciesResponseTypeDef,
     ListConfigurationPolicyAssociationsResponseTypeDef,
     ListEnabledProductsForImportResponseTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListMembersResponseTypeDef,
@@ -210,18 +210,18 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        Filters: AwsSecurityFindingFiltersTypeDef = ...,
+        Filters: AwsSecurityFindingFiltersUnionTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[GetFindingsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#getfindingspaginator)
         """
 
 class GetInsightsPaginator(Paginator):
     """
```

### Comparing `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/type_defs.py` & `mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/type_defs.py`

 * *Files 22% similar despite different names*

```diff
@@ -71,17 +71,17 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     "AcceptInvitationRequestRequestTypeDef",
     "AccountDetailsTypeDef",
+    "DnsRequestActionTypeDef",
     "ActionLocalIpDetailsTypeDef",
     "ActionLocalPortDetailsTypeDef",
-    "DnsRequestActionTypeDef",
     "CityTypeDef",
     "CountryTypeDef",
     "GeoLocationTypeDef",
     "IpOrganizationDetailsTypeDef",
     "ActionRemotePortDetailsTypeDef",
     "ActionTargetTypeDef",
     "AdjustmentTypeDef",
@@ -95,27 +95,31 @@
     "WorkflowUpdateTypeDef",
     "MapFilterTypeDef",
     "NumberFilterTypeDef",
     "StringFilterTypeDef",
     "AutomationRulesMetadataTypeDef",
     "AvailabilityZoneTypeDef",
     "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
-    "AwsAmazonMqBrokerLdapServerMetadataDetailsPaginatorTypeDef",
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsExtraOutputTypeDef",
     "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef",
     "AwsAmazonMqBrokerUsersDetailsTypeDef",
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef",
     "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
     "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
     "AwsApiCallActionDomainDetailsTypeDef",
     "AwsApiGatewayAccessLogSettingsTypeDef",
-    "AwsApiGatewayCanarySettingsPaginatorTypeDef",
+    "AwsApiGatewayCanarySettingsExtraOutputTypeDef",
+    "AwsApiGatewayCanarySettingsOutputTypeDef",
     "AwsApiGatewayCanarySettingsTypeDef",
-    "AwsApiGatewayEndpointConfigurationPaginatorTypeDef",
+    "AwsApiGatewayEndpointConfigurationExtraOutputTypeDef",
+    "AwsApiGatewayEndpointConfigurationOutputTypeDef",
     "AwsApiGatewayEndpointConfigurationTypeDef",
     "AwsApiGatewayMethodSettingsTypeDef",
-    "AwsCorsConfigurationPaginatorTypeDef",
+    "AwsCorsConfigurationExtraOutputTypeDef",
+    "AwsCorsConfigurationOutputTypeDef",
     "AwsCorsConfigurationTypeDef",
     "AwsApiGatewayV2RouteSettingsTypeDef",
     "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiLogConfigDetailsTypeDef",
     "AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef",
@@ -123,42 +127,47 @@
     "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef",
-    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsPaginatorTypeDef",
+    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsExtraOutputTypeDef",
+    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef",
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef",
     "AwsBackupBackupPlanLifecycleDetailsTypeDef",
-    "AwsBackupBackupVaultNotificationsDetailsPaginatorTypeDef",
+    "AwsBackupBackupVaultNotificationsDetailsExtraOutputTypeDef",
+    "AwsBackupBackupVaultNotificationsDetailsOutputTypeDef",
     "AwsBackupBackupVaultNotificationsDetailsTypeDef",
     "AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef",
     "AwsBackupRecoveryPointCreatedByDetailsTypeDef",
     "AwsBackupRecoveryPointLifecycleDetailsTypeDef",
     "AwsCertificateManagerCertificateExtendedKeyUsageTypeDef",
     "AwsCertificateManagerCertificateKeyUsageTypeDef",
     "AwsCertificateManagerCertificateOptionsTypeDef",
     "AwsCertificateManagerCertificateResourceRecordTypeDef",
     "AwsCloudFormationStackDriftInformationDetailsTypeDef",
     "AwsCloudFormationStackOutputsDetailsTypeDef",
     "AwsCloudFrontDistributionCacheBehaviorTypeDef",
     "AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef",
     "AwsCloudFrontDistributionLoggingTypeDef",
     "AwsCloudFrontDistributionViewerCertificateTypeDef",
-    "AwsCloudFrontDistributionOriginSslProtocolsPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginSslProtocolsExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef",
     "AwsCloudFrontDistributionOriginSslProtocolsTypeDef",
-    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef",
     "AwsCloudFrontDistributionOriginS3OriginConfigTypeDef",
     "AwsCloudTrailTrailDetailsTypeDef",
     "AwsCloudWatchAlarmDimensionsDetailsTypeDef",
     "AwsCodeBuildProjectArtifactsDetailsTypeDef",
     "AwsCodeBuildProjectSourceTypeDef",
-    "AwsCodeBuildProjectVpcConfigPaginatorTypeDef",
+    "AwsCodeBuildProjectVpcConfigExtraOutputTypeDef",
+    "AwsCodeBuildProjectVpcConfigOutputTypeDef",
     "AwsCodeBuildProjectVpcConfigTypeDef",
     "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef",
     "AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef",
     "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef",
     "AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef",
     "AwsDmsEndpointDetailsTypeDef",
     "AwsDmsReplicationInstanceReplicationSubnetGroupDetailsTypeDef",
@@ -167,15 +176,16 @@
     "AwsDynamoDbTableAttributeDefinitionTypeDef",
     "AwsDynamoDbTableBillingModeSummaryTypeDef",
     "AwsDynamoDbTableKeySchemaTypeDef",
     "AwsDynamoDbTableProvisionedThroughputTypeDef",
     "AwsDynamoDbTableRestoreSummaryTypeDef",
     "AwsDynamoDbTableSseDescriptionTypeDef",
     "AwsDynamoDbTableStreamSpecificationTypeDef",
-    "AwsDynamoDbTableProjectionPaginatorTypeDef",
+    "AwsDynamoDbTableProjectionExtraOutputTypeDef",
+    "AwsDynamoDbTableProjectionOutputTypeDef",
     "AwsDynamoDbTableProjectionTypeDef",
     "AwsDynamoDbTableProvisionedThroughputOverrideTypeDef",
     "AwsEc2ClientVpnEndpointAuthenticationOptionsActiveDirectoryDetailsTypeDef",
     "AwsEc2ClientVpnEndpointAuthenticationOptionsFederatedAuthenticationDetailsTypeDef",
     "AwsEc2ClientVpnEndpointAuthenticationOptionsMutualAuthenticationDetailsTypeDef",
     "AwsEc2ClientVpnEndpointClientConnectOptionsStatusDetailsTypeDef",
     "AwsEc2ClientVpnEndpointClientLoginBannerOptionsDetailsTypeDef",
@@ -222,101 +232,116 @@
     "PropagatingVgwSetDetailsTypeDef",
     "RouteSetDetailsTypeDef",
     "AwsEc2SecurityGroupIpRangeTypeDef",
     "AwsEc2SecurityGroupIpv6RangeTypeDef",
     "AwsEc2SecurityGroupPrefixListIdTypeDef",
     "AwsEc2SecurityGroupUserIdGroupPairTypeDef",
     "Ipv6CidrBlockAssociationTypeDef",
-    "AwsEc2TransitGatewayDetailsPaginatorTypeDef",
+    "AwsEc2TransitGatewayDetailsExtraOutputTypeDef",
+    "AwsEc2TransitGatewayDetailsOutputTypeDef",
     "AwsEc2TransitGatewayDetailsTypeDef",
     "AwsEc2VolumeAttachmentTypeDef",
     "CidrBlockAssociationTypeDef",
     "AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef",
     "AwsEc2VpcPeeringConnectionStatusDetailsTypeDef",
     "VpcInfoCidrBlockSetDetailsTypeDef",
     "VpcInfoIpv6CidrBlockSetDetailsTypeDef",
     "VpcInfoPeeringOptionsDetailsTypeDef",
     "AwsEc2VpnConnectionRoutesDetailsTypeDef",
     "AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef",
-    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsPaginatorTypeDef",
+    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsExtraOutputTypeDef",
+    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef",
     "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef",
-    "AwsEcrContainerImageDetailsPaginatorTypeDef",
+    "AwsEcrContainerImageDetailsExtraOutputTypeDef",
+    "AwsEcrContainerImageDetailsOutputTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef",
     "AwsEcrRepositoryLifecyclePolicyDetailsTypeDef",
     "AwsEcsClusterClusterSettingsDetailsTypeDef",
     "AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef",
     "AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef",
     "AwsMountPointTypeDef",
     "AwsEcsServiceCapacityProviderStrategyDetailsTypeDef",
     "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef",
     "AwsEcsServiceDeploymentControllerDetailsTypeDef",
     "AwsEcsServiceLoadBalancersDetailsTypeDef",
     "AwsEcsServicePlacementConstraintsDetailsTypeDef",
     "AwsEcsServicePlacementStrategiesDetailsTypeDef",
     "AwsEcsServiceServiceRegistriesDetailsTypeDef",
-    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsPaginatorTypeDef",
+    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsExtraOutputTypeDef",
+    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef",
     "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsPaginatorTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsExtraOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsPaginatorTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef",
     "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef",
     "AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef",
     "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef",
-    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsExtraOutputTypeDef",
     "AwsEcsTaskDefinitionVolumesHostDetailsTypeDef",
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef",
     "AwsEcsTaskVolumeHostDetailsTypeDef",
-    "AwsEfsAccessPointPosixUserDetailsPaginatorTypeDef",
+    "AwsEfsAccessPointPosixUserDetailsExtraOutputTypeDef",
+    "AwsEfsAccessPointPosixUserDetailsOutputTypeDef",
     "AwsEfsAccessPointPosixUserDetailsTypeDef",
     "AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef",
-    "AwsEksClusterResourcesVpcConfigDetailsPaginatorTypeDef",
+    "AwsEksClusterResourcesVpcConfigDetailsExtraOutputTypeDef",
+    "AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef",
     "AwsEksClusterResourcesVpcConfigDetailsTypeDef",
-    "AwsEksClusterLoggingClusterLoggingDetailsPaginatorTypeDef",
+    "AwsEksClusterLoggingClusterLoggingDetailsExtraOutputTypeDef",
+    "AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef",
     "AwsEksClusterLoggingClusterLoggingDetailsTypeDef",
     "AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef",
     "AwsElasticBeanstalkEnvironmentOptionSettingTypeDef",
     "AwsElasticBeanstalkEnvironmentTierTypeDef",
     "AwsElasticsearchDomainDomainEndpointOptionsTypeDef",
     "AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef",
     "AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef",
     "AwsElasticsearchDomainServiceSoftwareOptionsTypeDef",
-    "AwsElasticsearchDomainVPCOptionsPaginatorTypeDef",
+    "AwsElasticsearchDomainVPCOptionsExtraOutputTypeDef",
+    "AwsElasticsearchDomainVPCOptionsOutputTypeDef",
     "AwsElasticsearchDomainVPCOptionsTypeDef",
     "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef",
     "AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef",
     "AwsElbAppCookieStickinessPolicyTypeDef",
     "AwsElbLbCookieStickinessPolicyTypeDef",
     "AwsElbLoadBalancerAccessLogTypeDef",
     "AwsElbLoadBalancerAdditionalAttributeTypeDef",
     "AwsElbLoadBalancerConnectionDrainingTypeDef",
     "AwsElbLoadBalancerConnectionSettingsTypeDef",
     "AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef",
-    "AwsElbLoadBalancerBackendServerDescriptionPaginatorTypeDef",
+    "AwsElbLoadBalancerBackendServerDescriptionExtraOutputTypeDef",
+    "AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef",
     "AwsElbLoadBalancerBackendServerDescriptionTypeDef",
     "AwsElbLoadBalancerHealthCheckTypeDef",
     "AwsElbLoadBalancerInstanceTypeDef",
     "AwsElbLoadBalancerSourceSecurityGroupTypeDef",
     "AwsElbLoadBalancerListenerTypeDef",
     "AwsElbv2LoadBalancerAttributeTypeDef",
     "LoadBalancerStateTypeDef",
@@ -344,55 +369,62 @@
     "AwsIamUserPolicyTypeDef",
     "AwsKinesisStreamStreamEncryptionDetailsTypeDef",
     "AwsKmsKeyDetailsTypeDef",
     "AwsLambdaFunctionCodeTypeDef",
     "AwsLambdaFunctionDeadLetterConfigTypeDef",
     "AwsLambdaFunctionLayerTypeDef",
     "AwsLambdaFunctionTracingConfigTypeDef",
-    "AwsLambdaFunctionVpcConfigPaginatorTypeDef",
+    "AwsLambdaFunctionVpcConfigExtraOutputTypeDef",
+    "AwsLambdaFunctionVpcConfigOutputTypeDef",
     "AwsLambdaFunctionVpcConfigTypeDef",
     "AwsLambdaFunctionEnvironmentErrorTypeDef",
-    "AwsLambdaLayerVersionDetailsPaginatorTypeDef",
+    "AwsLambdaLayerVersionDetailsExtraOutputTypeDef",
+    "AwsLambdaLayerVersionDetailsOutputTypeDef",
     "AwsLambdaLayerVersionDetailsTypeDef",
-    "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsPaginatorTypeDef",
+    "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsExtraOutputTypeDef",
     "AwsMskClusterClusterInfoClientAuthenticationUnauthenticatedDetailsTypeDef",
+    "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsOutputTypeDef",
     "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsTypeDef",
     "AwsMskClusterClusterInfoClientAuthenticationSaslIamDetailsTypeDef",
     "AwsMskClusterClusterInfoClientAuthenticationSaslScramDetailsTypeDef",
     "AwsMskClusterClusterInfoEncryptionInfoEncryptionAtRestDetailsTypeDef",
     "AwsMskClusterClusterInfoEncryptionInfoEncryptionInTransitDetailsTypeDef",
     "AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef",
     "AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef",
     "AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef",
-    "AwsOpenSearchServiceDomainVpcOptionsDetailsPaginatorTypeDef",
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsExtraOutputTypeDef",
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainLogPublishingOptionTypeDef",
     "AwsRdsDbClusterAssociatedRoleTypeDef",
     "AwsRdsDbClusterMemberTypeDef",
     "AwsRdsDbClusterOptionGroupMembershipTypeDef",
     "AwsRdsDbDomainMembershipTypeDef",
     "AwsRdsDbInstanceVpcSecurityGroupTypeDef",
-    "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributePaginatorTypeDef",
+    "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeExtraOutputTypeDef",
+    "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef",
     "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef",
     "AwsRdsDbInstanceAssociatedRoleTypeDef",
     "AwsRdsDbInstanceEndpointTypeDef",
     "AwsRdsDbOptionGroupMembershipTypeDef",
     "AwsRdsDbParameterGroupTypeDef",
     "AwsRdsDbProcessorFeatureTypeDef",
     "AwsRdsDbStatusInfoTypeDef",
-    "AwsRdsPendingCloudWatchLogsExportsPaginatorTypeDef",
+    "AwsRdsPendingCloudWatchLogsExportsExtraOutputTypeDef",
+    "AwsRdsPendingCloudWatchLogsExportsOutputTypeDef",
     "AwsRdsPendingCloudWatchLogsExportsTypeDef",
     "AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef",
     "AwsRdsDbSecurityGroupIpRangeTypeDef",
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef",
-    "AwsRdsEventSubscriptionDetailsPaginatorTypeDef",
+    "AwsRdsEventSubscriptionDetailsExtraOutputTypeDef",
+    "AwsRdsEventSubscriptionDetailsOutputTypeDef",
     "AwsRdsEventSubscriptionDetailsTypeDef",
     "AwsRedshiftClusterClusterNodeTypeDef",
     "AwsRedshiftClusterClusterParameterStatusTypeDef",
     "AwsRedshiftClusterClusterSecurityGroupTypeDef",
     "AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef",
     "AwsRedshiftClusterDeferredMaintenanceWindowTypeDef",
     "AwsRedshiftClusterElasticIpStatusTypeDef",
@@ -421,26 +453,27 @@
     "AwsS3BucketServerSideEncryptionByDefaultTypeDef",
     "AwsS3BucketWebsiteConfigurationRedirectToTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef",
     "AwsS3ObjectDetailsTypeDef",
     "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
     "AwsSecretsManagerSecretRotationRulesTypeDef",
-    "BooleanFilterTypeDef",
-    "IpFilterTypeDef",
-    "KeywordFilterTypeDef",
-    "AwsSecurityFindingIdentifierTypeDef",
-    "GeneratorDetailsPaginatorTypeDef",
+    "GeneratorDetailsExtraOutputTypeDef",
     "MalwareTypeDef",
     "NoteTypeDef",
     "PatchSummaryTypeDef",
     "ProcessDetailsTypeDef",
     "SeverityTypeDef",
     "ThreatIntelIndicatorTypeDef",
     "WorkflowTypeDef",
+    "BooleanFilterTypeDef",
+    "IpFilterTypeDef",
+    "KeywordFilterTypeDef",
+    "AwsSecurityFindingIdentifierTypeDef",
+    "GeneratorDetailsOutputTypeDef",
     "GeneratorDetailsTypeDef",
     "AwsSnsTopicSubscriptionTypeDef",
     "AwsSqsQueueDetailsTypeDef",
     "AwsSsmComplianceSummaryTypeDef",
     "AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef",
     "AwsWafRateBasedRuleMatchPredicateTypeDef",
@@ -471,16 +504,17 @@
     "StandardsControlAssociationDetailTypeDef",
     "ImportFindingsErrorTypeDef",
     "StandardsControlAssociationUpdateTypeDef",
     "BooleanConfigurationOptionsTypeDef",
     "CellTypeDef",
     "ClassificationStatusTypeDef",
     "CodeVulnerabilitiesFilePathTypeDef",
-    "SecurityControlParameterPaginatorTypeDef",
+    "SecurityControlParameterExtraOutputTypeDef",
     "StatusReasonTypeDef",
+    "SecurityControlParameterOutputTypeDef",
     "SecurityControlParameterTypeDef",
     "DoubleConfigurationOptionsTypeDef",
     "EnumConfigurationOptionsTypeDef",
     "EnumListConfigurationOptionsTypeDef",
     "IntegerConfigurationOptionsTypeDef",
     "IntegerListConfigurationOptionsTypeDef",
     "StringConfigurationOptionsTypeDef",
@@ -544,216 +578,284 @@
     "ListSecurityControlDefinitionsRequestRequestTypeDef",
     "ListStandardsControlAssociationsRequestRequestTypeDef",
     "StandardsControlAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PortRangeTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
+    "ParameterValueOutputTypeDef",
     "ParameterValueTypeDef",
     "RecommendationTypeDef",
-    "RuleGroupSourceListDetailsPaginatorTypeDef",
+    "RuleGroupSourceListDetailsExtraOutputTypeDef",
+    "RuleGroupSourceListDetailsOutputTypeDef",
     "RuleGroupSourceListDetailsTypeDef",
     "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
-    "RuleGroupSourceStatefulRulesOptionsDetailsPaginatorTypeDef",
+    "RuleGroupSourceStatefulRulesOptionsDetailsExtraOutputTypeDef",
+    "RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef",
     "RuleGroupSourceStatefulRulesOptionsDetailsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
-    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsPaginatorTypeDef",
+    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsExtraOutputTypeDef",
+    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
-    "RuleGroupVariablesIpSetsDetailsPaginatorTypeDef",
+    "RuleGroupVariablesIpSetsDetailsExtraOutputTypeDef",
+    "RuleGroupVariablesPortSetsDetailsExtraOutputTypeDef",
+    "RuleGroupVariablesIpSetsDetailsOutputTypeDef",
     "RuleGroupVariablesIpSetsDetailsTypeDef",
-    "RuleGroupVariablesPortSetsDetailsPaginatorTypeDef",
+    "RuleGroupVariablesPortSetsDetailsOutputTypeDef",
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     "SoftwarePackageTypeDef",
     "StandardsManagedByTypeDef",
     "StandardsStatusReasonTypeDef",
     "StatelessCustomPublishMetricActionDimensionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateActionTargetRequestRequestTypeDef",
     "UpdateFindingAggregatorRequestRequestTypeDef",
     "UpdateSecurityHubConfigurationRequestRequestTypeDef",
     "UpdateStandardsControlRequestRequestTypeDef",
     "VulnerabilityVendorTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "ActionRemoteIpDetailsTypeDef",
-    "CvssPaginatorTypeDef",
+    "CvssExtraOutputTypeDef",
+    "CvssOutputTypeDef",
     "CvssTypeDef",
     "ListConfigurationPolicyAssociationsRequestRequestTypeDef",
     "AssociationSetDetailsTypeDef",
+    "AutomationRulesFindingFieldsUpdateOutputTypeDef",
     "AutomationRulesFindingFieldsUpdateTypeDef",
     "AwsAmazonMqBrokerLogsDetailsTypeDef",
-    "AwsApiGatewayRestApiDetailsPaginatorTypeDef",
+    "AwsApiGatewayRestApiDetailsExtraOutputTypeDef",
+    "AwsApiGatewayRestApiDetailsOutputTypeDef",
     "AwsApiGatewayRestApiDetailsTypeDef",
-    "AwsApiGatewayStageDetailsPaginatorTypeDef",
+    "AwsApiGatewayStageDetailsExtraOutputTypeDef",
+    "AwsApiGatewayStageDetailsOutputTypeDef",
     "AwsApiGatewayStageDetailsTypeDef",
-    "AwsApiGatewayV2ApiDetailsPaginatorTypeDef",
+    "AwsApiGatewayV2ApiDetailsExtraOutputTypeDef",
+    "AwsApiGatewayV2ApiDetailsOutputTypeDef",
     "AwsApiGatewayV2ApiDetailsTypeDef",
-    "AwsApiGatewayV2StageDetailsPaginatorTypeDef",
+    "AwsApiGatewayV2StageDetailsExtraOutputTypeDef",
+    "AwsApiGatewayV2StageDetailsOutputTypeDef",
     "AwsApiGatewayV2StageDetailsTypeDef",
     "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef",
     "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef",
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsPaginatorTypeDef",
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsExtraOutputTypeDef",
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef",
     "AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef",
-    "AwsBackupBackupVaultDetailsPaginatorTypeDef",
+    "AwsBackupBackupVaultDetailsExtraOutputTypeDef",
+    "AwsBackupBackupVaultDetailsOutputTypeDef",
     "AwsBackupBackupVaultDetailsTypeDef",
     "AwsBackupRecoveryPointDetailsTypeDef",
-    "AwsCertificateManagerCertificateDomainValidationOptionPaginatorTypeDef",
+    "AwsCertificateManagerCertificateDomainValidationOptionExtraOutputTypeDef",
+    "AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef",
     "AwsCertificateManagerCertificateDomainValidationOptionTypeDef",
-    "AwsCloudFormationStackDetailsPaginatorTypeDef",
+    "AwsCloudFormationStackDetailsExtraOutputTypeDef",
+    "AwsCloudFormationStackDetailsOutputTypeDef",
     "AwsCloudFormationStackDetailsTypeDef",
-    "AwsCloudFrontDistributionCacheBehaviorsPaginatorTypeDef",
+    "AwsCloudFrontDistributionCacheBehaviorsExtraOutputTypeDef",
+    "AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef",
     "AwsCloudFrontDistributionCacheBehaviorsTypeDef",
-    "AwsCloudFrontDistributionOriginCustomOriginConfigPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginCustomOriginConfigExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef",
     "AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef",
-    "AwsCloudFrontDistributionOriginGroupFailoverPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginGroupFailoverExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverTypeDef",
-    "AwsCloudWatchAlarmDetailsPaginatorTypeDef",
+    "AwsCloudWatchAlarmDetailsExtraOutputTypeDef",
+    "AwsCloudWatchAlarmDetailsOutputTypeDef",
     "AwsCloudWatchAlarmDetailsTypeDef",
-    "AwsCodeBuildProjectEnvironmentPaginatorTypeDef",
+    "AwsCodeBuildProjectEnvironmentExtraOutputTypeDef",
+    "AwsCodeBuildProjectEnvironmentOutputTypeDef",
     "AwsCodeBuildProjectEnvironmentTypeDef",
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
-    "AwsDmsReplicationInstanceDetailsPaginatorTypeDef",
+    "AwsDmsReplicationInstanceDetailsExtraOutputTypeDef",
+    "AwsDmsReplicationInstanceDetailsOutputTypeDef",
     "AwsDmsReplicationInstanceDetailsTypeDef",
-    "AwsDynamoDbTableGlobalSecondaryIndexPaginatorTypeDef",
-    "AwsDynamoDbTableLocalSecondaryIndexPaginatorTypeDef",
+    "AwsDynamoDbTableGlobalSecondaryIndexExtraOutputTypeDef",
+    "AwsDynamoDbTableLocalSecondaryIndexExtraOutputTypeDef",
+    "AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef",
+    "AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef",
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     "AwsDynamoDbTableLocalSecondaryIndexTypeDef",
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef",
     "AwsEc2ClientVpnEndpointAuthenticationOptionsDetailsTypeDef",
     "AwsEc2ClientVpnEndpointClientConnectOptionsDetailsTypeDef",
-    "AwsEc2InstanceDetailsPaginatorTypeDef",
+    "AwsEc2InstanceDetailsExtraOutputTypeDef",
+    "AwsEc2InstanceDetailsOutputTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsPaginatorTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsExtraOutputTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsPaginatorTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsExtraOutputTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
     "AwsEc2NetworkAclEntryTypeDef",
-    "AwsEc2NetworkInterfaceDetailsPaginatorTypeDef",
+    "AwsEc2NetworkInterfaceDetailsExtraOutputTypeDef",
+    "AwsEc2NetworkInterfaceDetailsOutputTypeDef",
     "AwsEc2NetworkInterfaceDetailsTypeDef",
-    "AwsEc2SecurityGroupIpPermissionPaginatorTypeDef",
+    "AwsEc2SecurityGroupIpPermissionExtraOutputTypeDef",
+    "AwsEc2SecurityGroupIpPermissionOutputTypeDef",
     "AwsEc2SecurityGroupIpPermissionTypeDef",
-    "AwsEc2SubnetDetailsPaginatorTypeDef",
+    "AwsEc2SubnetDetailsExtraOutputTypeDef",
+    "AwsEc2SubnetDetailsOutputTypeDef",
     "AwsEc2SubnetDetailsTypeDef",
-    "AwsEc2VolumeDetailsPaginatorTypeDef",
+    "AwsEc2VolumeDetailsExtraOutputTypeDef",
+    "AwsEc2VolumeDetailsOutputTypeDef",
     "AwsEc2VolumeDetailsTypeDef",
-    "AwsEc2VpcDetailsPaginatorTypeDef",
+    "AwsEc2VpcDetailsExtraOutputTypeDef",
+    "AwsEc2VpcDetailsOutputTypeDef",
     "AwsEc2VpcDetailsTypeDef",
-    "AwsEc2VpcEndpointServiceDetailsPaginatorTypeDef",
+    "AwsEc2VpcEndpointServiceDetailsExtraOutputTypeDef",
+    "AwsEc2VpcEndpointServiceDetailsOutputTypeDef",
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
-    "AwsEc2VpcPeeringConnectionVpcInfoDetailsPaginatorTypeDef",
+    "AwsEc2VpcPeeringConnectionVpcInfoDetailsExtraOutputTypeDef",
+    "AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef",
     "AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef",
-    "AwsEc2VpnConnectionOptionsDetailsPaginatorTypeDef",
+    "AwsEc2VpnConnectionOptionsDetailsExtraOutputTypeDef",
+    "AwsEc2VpnConnectionOptionsDetailsOutputTypeDef",
     "AwsEc2VpnConnectionOptionsDetailsTypeDef",
     "AwsEcrRepositoryDetailsTypeDef",
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef",
-    "AwsEcsContainerDetailsPaginatorTypeDef",
+    "AwsEcsContainerDetailsExtraOutputTypeDef",
+    "AwsEcsContainerDetailsOutputTypeDef",
     "AwsEcsContainerDetailsTypeDef",
     "AwsEcsServiceDeploymentConfigurationDetailsTypeDef",
-    "AwsEcsServiceNetworkConfigurationDetailsPaginatorTypeDef",
+    "AwsEcsServiceNetworkConfigurationDetailsExtraOutputTypeDef",
+    "AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef",
     "AwsEcsServiceNetworkConfigurationDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef",
-    "AwsEcsTaskDefinitionProxyConfigurationDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionProxyConfigurationDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef",
     "AwsEcsTaskVolumeDetailsTypeDef",
     "AwsEfsAccessPointRootDirectoryDetailsTypeDef",
-    "AwsEksClusterLoggingDetailsPaginatorTypeDef",
+    "AwsEksClusterLoggingDetailsExtraOutputTypeDef",
+    "AwsEksClusterLoggingDetailsOutputTypeDef",
     "AwsEksClusterLoggingDetailsTypeDef",
-    "AwsElasticBeanstalkEnvironmentDetailsPaginatorTypeDef",
+    "AwsElasticBeanstalkEnvironmentDetailsExtraOutputTypeDef",
+    "AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef",
     "AwsElasticBeanstalkEnvironmentDetailsTypeDef",
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
-    "AwsElbLoadBalancerPoliciesPaginatorTypeDef",
+    "AwsElbLoadBalancerPoliciesExtraOutputTypeDef",
+    "AwsElbLoadBalancerPoliciesOutputTypeDef",
     "AwsElbLoadBalancerPoliciesTypeDef",
-    "AwsElbLoadBalancerAttributesPaginatorTypeDef",
+    "AwsElbLoadBalancerAttributesExtraOutputTypeDef",
+    "AwsElbLoadBalancerAttributesOutputTypeDef",
     "AwsElbLoadBalancerAttributesTypeDef",
-    "AwsElbLoadBalancerListenerDescriptionPaginatorTypeDef",
+    "AwsElbLoadBalancerListenerDescriptionExtraOutputTypeDef",
+    "AwsElbLoadBalancerListenerDescriptionOutputTypeDef",
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
-    "AwsElbv2LoadBalancerDetailsPaginatorTypeDef",
+    "AwsElbv2LoadBalancerDetailsExtraOutputTypeDef",
+    "AwsElbv2LoadBalancerDetailsOutputTypeDef",
     "AwsElbv2LoadBalancerDetailsTypeDef",
     "AwsEventsEndpointRoutingConfigFailoverConfigDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef",
     "AwsIamAccessKeySessionContextTypeDef",
-    "AwsIamGroupDetailsPaginatorTypeDef",
+    "AwsIamGroupDetailsExtraOutputTypeDef",
+    "AwsIamGroupDetailsOutputTypeDef",
     "AwsIamGroupDetailsTypeDef",
-    "AwsIamInstanceProfilePaginatorTypeDef",
+    "AwsIamInstanceProfileExtraOutputTypeDef",
+    "AwsIamInstanceProfileOutputTypeDef",
     "AwsIamInstanceProfileTypeDef",
-    "AwsIamPolicyDetailsPaginatorTypeDef",
+    "AwsIamPolicyDetailsExtraOutputTypeDef",
+    "AwsIamPolicyDetailsOutputTypeDef",
     "AwsIamPolicyDetailsTypeDef",
-    "AwsIamUserDetailsPaginatorTypeDef",
+    "AwsIamUserDetailsExtraOutputTypeDef",
+    "AwsIamUserDetailsOutputTypeDef",
     "AwsIamUserDetailsTypeDef",
     "AwsKinesisStreamDetailsTypeDef",
-    "AwsLambdaFunctionEnvironmentPaginatorTypeDef",
+    "AwsLambdaFunctionEnvironmentExtraOutputTypeDef",
+    "AwsLambdaFunctionEnvironmentOutputTypeDef",
     "AwsLambdaFunctionEnvironmentTypeDef",
     "AwsMskClusterClusterInfoClientAuthenticationSaslDetailsTypeDef",
     "AwsMskClusterClusterInfoEncryptionInfoDetailsTypeDef",
-    "AwsNetworkFirewallFirewallDetailsPaginatorTypeDef",
+    "AwsNetworkFirewallFirewallDetailsExtraOutputTypeDef",
+    "AwsNetworkFirewallFirewallDetailsOutputTypeDef",
     "AwsNetworkFirewallFirewallDetailsTypeDef",
     "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef",
     "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef",
-    "AwsRdsDbClusterDetailsPaginatorTypeDef",
+    "AwsRdsDbClusterDetailsExtraOutputTypeDef",
+    "AwsRdsDbClusterDetailsOutputTypeDef",
     "AwsRdsDbClusterDetailsTypeDef",
-    "AwsRdsDbClusterSnapshotDetailsPaginatorTypeDef",
+    "AwsRdsDbClusterSnapshotDetailsExtraOutputTypeDef",
+    "AwsRdsDbClusterSnapshotDetailsOutputTypeDef",
     "AwsRdsDbClusterSnapshotDetailsTypeDef",
-    "AwsRdsDbSnapshotDetailsPaginatorTypeDef",
+    "AwsRdsDbSnapshotDetailsExtraOutputTypeDef",
+    "AwsRdsDbSnapshotDetailsOutputTypeDef",
     "AwsRdsDbSnapshotDetailsTypeDef",
-    "AwsRdsDbPendingModifiedValuesPaginatorTypeDef",
+    "AwsRdsDbPendingModifiedValuesExtraOutputTypeDef",
+    "AwsRdsDbPendingModifiedValuesOutputTypeDef",
     "AwsRdsDbPendingModifiedValuesTypeDef",
-    "AwsRdsDbSecurityGroupDetailsPaginatorTypeDef",
+    "AwsRdsDbSecurityGroupDetailsExtraOutputTypeDef",
+    "AwsRdsDbSecurityGroupDetailsOutputTypeDef",
     "AwsRdsDbSecurityGroupDetailsTypeDef",
     "AwsRdsDbSubnetGroupSubnetTypeDef",
-    "AwsRedshiftClusterClusterParameterGroupPaginatorTypeDef",
+    "AwsRedshiftClusterClusterParameterGroupExtraOutputTypeDef",
+    "AwsRedshiftClusterClusterParameterGroupOutputTypeDef",
     "AwsRedshiftClusterClusterParameterGroupTypeDef",
     "AwsRoute53HostedZoneObjectDetailsTypeDef",
     "AwsRoute53QueryLoggingConfigDetailsTypeDef",
     "AwsS3AccessPointDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef",
-    "AwsS3BucketNotificationConfigurationS3KeyFilterPaginatorTypeDef",
+    "AwsS3BucketNotificationConfigurationS3KeyFilterExtraOutputTypeDef",
+    "AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
     "AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef",
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
-    "AwsSageMakerNotebookInstanceDetailsPaginatorTypeDef",
+    "AwsSageMakerNotebookInstanceDetailsExtraOutputTypeDef",
+    "AwsSageMakerNotebookInstanceDetailsOutputTypeDef",
     "AwsSageMakerNotebookInstanceDetailsTypeDef",
     "AwsSecretsManagerSecretDetailsTypeDef",
     "BatchUpdateFindingsRequestRequestTypeDef",
     "BatchUpdateFindingsUnprocessedFindingTypeDef",
-    "AwsSnsTopicDetailsPaginatorTypeDef",
+    "AwsSnsTopicDetailsExtraOutputTypeDef",
+    "AwsSnsTopicDetailsOutputTypeDef",
     "AwsSnsTopicDetailsTypeDef",
     "AwsSsmPatchTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
-    "AwsWafRateBasedRuleDetailsPaginatorTypeDef",
+    "AwsWafRateBasedRuleDetailsExtraOutputTypeDef",
+    "AwsWafRateBasedRuleDetailsOutputTypeDef",
     "AwsWafRateBasedRuleDetailsTypeDef",
-    "AwsWafRegionalRateBasedRuleDetailsPaginatorTypeDef",
+    "AwsWafRegionalRateBasedRuleDetailsExtraOutputTypeDef",
+    "AwsWafRegionalRateBasedRuleDetailsOutputTypeDef",
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
-    "AwsWafRegionalRuleDetailsPaginatorTypeDef",
+    "AwsWafRegionalRuleDetailsExtraOutputTypeDef",
+    "AwsWafRegionalRuleDetailsOutputTypeDef",
     "AwsWafRegionalRuleDetailsTypeDef",
     "AwsWafRegionalRuleGroupRulesDetailsTypeDef",
     "AwsWafRegionalWebAclRulesListDetailsTypeDef",
-    "AwsWafRuleDetailsPaginatorTypeDef",
+    "AwsWafRuleDetailsExtraOutputTypeDef",
+    "AwsWafRuleDetailsOutputTypeDef",
     "AwsWafRuleDetailsTypeDef",
     "AwsWafRuleGroupRulesDetailsTypeDef",
-    "AwsWafWebAclRulePaginatorTypeDef",
+    "AwsWafWebAclRuleExtraOutputTypeDef",
+    "AwsWafWebAclRuleOutputTypeDef",
     "AwsWafWebAclRuleTypeDef",
-    "AwsWafv2CustomRequestHandlingDetailsPaginatorTypeDef",
+    "AwsWafv2CustomRequestHandlingDetailsExtraOutputTypeDef",
+    "AwsWafv2CustomRequestHandlingDetailsOutputTypeDef",
     "AwsWafv2CustomRequestHandlingDetailsTypeDef",
-    "AwsWafv2CustomResponseDetailsPaginatorTypeDef",
+    "AwsWafv2CustomResponseDetailsExtraOutputTypeDef",
+    "AwsWafv2CustomResponseDetailsOutputTypeDef",
     "AwsWafv2CustomResponseDetailsTypeDef",
     "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
     "CreateActionTargetResponseTypeDef",
     "CreateAutomationRuleResponseTypeDef",
     "CreateFindingAggregatorResponseTypeDef",
     "CreateInsightResponseTypeDef",
     "DeleteActionTargetResponseTypeDef",
@@ -775,25 +877,28 @@
     "BatchEnableStandardsRequestRequestTypeDef",
     "ListConfigurationPolicyAssociationsResponseTypeDef",
     "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
     "UnprocessedStandardsControlAssociationTypeDef",
     "BatchImportFindingsResponseTypeDef",
     "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
     "UnprocessedStandardsControlAssociationUpdateTypeDef",
-    "VulnerabilityCodeVulnerabilitiesPaginatorTypeDef",
+    "VulnerabilityCodeVulnerabilitiesExtraOutputTypeDef",
+    "VulnerabilityCodeVulnerabilitiesOutputTypeDef",
     "VulnerabilityCodeVulnerabilitiesTypeDef",
-    "CompliancePaginatorTypeDef",
+    "ComplianceExtraOutputTypeDef",
+    "ComplianceOutputTypeDef",
     "ComplianceTypeDef",
     "ConfigurationOptionsTypeDef",
     "ConfigurationPolicyAssociationTypeDef",
     "GetConfigurationPolicyAssociationRequestRequestTypeDef",
     "StartConfigurationPolicyAssociationRequestRequestTypeDef",
     "StartConfigurationPolicyDisassociationRequestRequestTypeDef",
     "ListConfigurationPoliciesResponseTypeDef",
-    "ContainerDetailsPaginatorTypeDef",
+    "ContainerDetailsExtraOutputTypeDef",
+    "ContainerDetailsOutputTypeDef",
     "ContainerDetailsTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
     "DateFilterTypeDef",
@@ -812,302 +917,423 @@
     "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
     "ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
     "DescribeOrganizationConfigurationResponseTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "DescribeProductsResponseTypeDef",
     "DescribeStandardsControlsResponseTypeDef",
-    "ThreatPaginatorTypeDef",
+    "ThreatExtraOutputTypeDef",
+    "ThreatOutputTypeDef",
     "ThreatTypeDef",
     "ListFindingAggregatorsResponseTypeDef",
     "FindingHistoryRecordTypeDef",
-    "FindingProviderFieldsPaginatorTypeDef",
+    "FindingProviderFieldsExtraOutputTypeDef",
+    "FindingProviderFieldsOutputTypeDef",
     "FindingProviderFieldsTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
     "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
     "GetFindingHistoryRequestRequestTypeDef",
     "GetMembersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "InsightResultsTypeDef",
     "ListStandardsControlAssociationsResponseTypeDef",
-    "NetworkPathComponentDetailsPaginatorTypeDef",
+    "NetworkPathComponentDetailsExtraOutputTypeDef",
+    "NetworkPathComponentDetailsOutputTypeDef",
     "NetworkPathComponentDetailsTypeDef",
     "NetworkTypeDef",
     "PageTypeDef",
+    "ParameterConfigurationOutputTypeDef",
     "ParameterConfigurationTypeDef",
     "RemediationTypeDef",
-    "RuleGroupSourceStatefulRulesDetailsPaginatorTypeDef",
+    "RuleGroupSourceStatefulRulesDetailsExtraOutputTypeDef",
+    "RuleGroupSourceStatefulRulesDetailsOutputTypeDef",
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
-    "RuleGroupSourceStatelessRuleMatchAttributesPaginatorTypeDef",
+    "RuleGroupSourceStatelessRuleMatchAttributesExtraOutputTypeDef",
+    "RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
-    "RuleGroupVariablesPaginatorTypeDef",
+    "RuleGroupVariablesExtraOutputTypeDef",
+    "RuleGroupVariablesOutputTypeDef",
     "RuleGroupVariablesTypeDef",
     "StandardTypeDef",
     "StandardsSubscriptionTypeDef",
-    "StatelessCustomPublishMetricActionPaginatorTypeDef",
+    "StatelessCustomPublishMetricActionExtraOutputTypeDef",
+    "StatelessCustomPublishMetricActionOutputTypeDef",
     "StatelessCustomPublishMetricActionTypeDef",
-    "AwsApiCallActionPaginatorTypeDef",
+    "AwsApiCallActionExtraOutputTypeDef",
+    "AwsApiCallActionOutputTypeDef",
     "AwsApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
-    "AwsEc2RouteTableDetailsPaginatorTypeDef",
+    "AwsEc2RouteTableDetailsExtraOutputTypeDef",
+    "AwsEc2RouteTableDetailsOutputTypeDef",
     "AwsEc2RouteTableDetailsTypeDef",
+    "AutomationRulesActionOutputTypeDef",
     "AutomationRulesActionTypeDef",
-    "AwsAmazonMqBrokerDetailsPaginatorTypeDef",
+    "AwsAmazonMqBrokerDetailsExtraOutputTypeDef",
+    "AwsAmazonMqBrokerDetailsOutputTypeDef",
     "AwsAmazonMqBrokerDetailsTypeDef",
-    "AwsAppSyncGraphQlApiDetailsPaginatorTypeDef",
+    "AwsAppSyncGraphQlApiDetailsExtraOutputTypeDef",
+    "AwsAppSyncGraphQlApiDetailsOutputTypeDef",
     "AwsAppSyncGraphQlApiDetailsTypeDef",
     "AwsAthenaWorkGroupConfigurationDetailsTypeDef",
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsPaginatorTypeDef",
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsExtraOutputTypeDef",
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
-    "AwsAutoScalingLaunchConfigurationDetailsPaginatorTypeDef",
+    "AwsAutoScalingLaunchConfigurationDetailsExtraOutputTypeDef",
+    "AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef",
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
-    "AwsBackupBackupPlanRuleDetailsPaginatorTypeDef",
+    "AwsBackupBackupPlanRuleDetailsExtraOutputTypeDef",
+    "AwsBackupBackupPlanRuleDetailsOutputTypeDef",
     "AwsBackupBackupPlanRuleDetailsTypeDef",
-    "AwsCertificateManagerCertificateRenewalSummaryPaginatorTypeDef",
+    "AwsCertificateManagerCertificateRenewalSummaryExtraOutputTypeDef",
+    "AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef",
     "AwsCertificateManagerCertificateRenewalSummaryTypeDef",
-    "AwsCloudFrontDistributionOriginItemPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginItemExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginItemOutputTypeDef",
     "AwsCloudFrontDistributionOriginItemTypeDef",
-    "AwsCloudFrontDistributionOriginGroupPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginGroupExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginGroupOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupTypeDef",
-    "AwsCodeBuildProjectDetailsPaginatorTypeDef",
+    "AwsCodeBuildProjectDetailsExtraOutputTypeDef",
+    "AwsCodeBuildProjectDetailsOutputTypeDef",
     "AwsCodeBuildProjectDetailsTypeDef",
-    "AwsDynamoDbTableReplicaPaginatorTypeDef",
+    "AwsDynamoDbTableReplicaExtraOutputTypeDef",
+    "AwsDynamoDbTableReplicaOutputTypeDef",
     "AwsDynamoDbTableReplicaTypeDef",
-    "AwsEc2ClientVpnEndpointDetailsPaginatorTypeDef",
+    "AwsEc2ClientVpnEndpointDetailsExtraOutputTypeDef",
+    "AwsEc2ClientVpnEndpointDetailsOutputTypeDef",
     "AwsEc2ClientVpnEndpointDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataDetailsPaginatorTypeDef",
+    "AwsEc2LaunchTemplateDataDetailsExtraOutputTypeDef",
+    "AwsEc2LaunchTemplateDataDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataDetailsTypeDef",
-    "AwsEc2NetworkAclDetailsPaginatorTypeDef",
+    "AwsEc2NetworkAclDetailsExtraOutputTypeDef",
+    "AwsEc2NetworkAclDetailsOutputTypeDef",
     "AwsEc2NetworkAclDetailsTypeDef",
-    "AwsEc2SecurityGroupDetailsPaginatorTypeDef",
+    "AwsEc2SecurityGroupDetailsExtraOutputTypeDef",
+    "AwsEc2SecurityGroupDetailsOutputTypeDef",
     "AwsEc2SecurityGroupDetailsTypeDef",
-    "AwsEc2VpcPeeringConnectionDetailsPaginatorTypeDef",
+    "AwsEc2VpcPeeringConnectionDetailsExtraOutputTypeDef",
+    "AwsEc2VpcPeeringConnectionDetailsOutputTypeDef",
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
-    "AwsEc2VpnConnectionDetailsPaginatorTypeDef",
+    "AwsEc2VpnConnectionDetailsExtraOutputTypeDef",
+    "AwsEc2VpnConnectionDetailsOutputTypeDef",
     "AwsEc2VpnConnectionDetailsTypeDef",
     "AwsEcsClusterConfigurationDetailsTypeDef",
-    "AwsEcsServiceDetailsPaginatorTypeDef",
+    "AwsEcsServiceDetailsExtraOutputTypeDef",
+    "AwsEcsServiceDetailsOutputTypeDef",
     "AwsEcsServiceDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
-    "AwsEcsTaskDefinitionVolumesDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionVolumesDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
-    "AwsEcsTaskDetailsPaginatorTypeDef",
+    "AwsEcsTaskDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDetailsOutputTypeDef",
     "AwsEcsTaskDetailsTypeDef",
-    "AwsEfsAccessPointDetailsPaginatorTypeDef",
+    "AwsEfsAccessPointDetailsExtraOutputTypeDef",
+    "AwsEfsAccessPointDetailsOutputTypeDef",
     "AwsEfsAccessPointDetailsTypeDef",
-    "AwsEksClusterDetailsPaginatorTypeDef",
+    "AwsEksClusterDetailsExtraOutputTypeDef",
+    "AwsEksClusterDetailsOutputTypeDef",
     "AwsEksClusterDetailsTypeDef",
-    "AwsElasticsearchDomainDetailsPaginatorTypeDef",
+    "AwsElasticsearchDomainDetailsExtraOutputTypeDef",
+    "AwsElasticsearchDomainDetailsOutputTypeDef",
     "AwsElasticsearchDomainDetailsTypeDef",
-    "AwsElbLoadBalancerDetailsPaginatorTypeDef",
+    "AwsElbLoadBalancerDetailsExtraOutputTypeDef",
+    "AwsElbLoadBalancerDetailsOutputTypeDef",
     "AwsElbLoadBalancerDetailsTypeDef",
     "AwsEventsEndpointRoutingConfigDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef",
     "AwsIamAccessKeyDetailsTypeDef",
-    "AwsIamRoleDetailsPaginatorTypeDef",
+    "AwsIamRoleDetailsExtraOutputTypeDef",
+    "AwsIamRoleDetailsOutputTypeDef",
     "AwsIamRoleDetailsTypeDef",
-    "AwsLambdaFunctionDetailsPaginatorTypeDef",
+    "AwsLambdaFunctionDetailsExtraOutputTypeDef",
+    "AwsLambdaFunctionDetailsOutputTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
-    "AwsMskClusterClusterInfoClientAuthenticationDetailsPaginatorTypeDef",
+    "AwsMskClusterClusterInfoClientAuthenticationDetailsExtraOutputTypeDef",
+    "AwsMskClusterClusterInfoClientAuthenticationDetailsOutputTypeDef",
     "AwsMskClusterClusterInfoClientAuthenticationDetailsTypeDef",
-    "AwsOpenSearchServiceDomainDetailsPaginatorTypeDef",
+    "AwsOpenSearchServiceDomainDetailsExtraOutputTypeDef",
+    "AwsOpenSearchServiceDomainDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainDetailsTypeDef",
-    "AwsRdsDbSubnetGroupPaginatorTypeDef",
+    "AwsRdsDbSubnetGroupExtraOutputTypeDef",
+    "AwsRdsDbSubnetGroupOutputTypeDef",
     "AwsRdsDbSubnetGroupTypeDef",
-    "AwsRedshiftClusterDetailsPaginatorTypeDef",
+    "AwsRedshiftClusterDetailsExtraOutputTypeDef",
+    "AwsRedshiftClusterDetailsOutputTypeDef",
     "AwsRedshiftClusterDetailsTypeDef",
-    "AwsRoute53HostedZoneDetailsPaginatorTypeDef",
+    "AwsRoute53HostedZoneDetailsExtraOutputTypeDef",
+    "AwsRoute53HostedZoneDetailsOutputTypeDef",
     "AwsRoute53HostedZoneDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsPaginatorTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsExtraOutputTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef",
-    "AwsS3BucketNotificationConfigurationFilterPaginatorTypeDef",
+    "AwsS3BucketNotificationConfigurationFilterExtraOutputTypeDef",
+    "AwsS3BucketNotificationConfigurationFilterOutputTypeDef",
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
     "AwsS3BucketObjectLockConfigurationTypeDef",
-    "AwsS3BucketServerSideEncryptionConfigurationPaginatorTypeDef",
+    "AwsS3BucketServerSideEncryptionConfigurationExtraOutputTypeDef",
+    "AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef",
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
-    "AwsS3BucketWebsiteConfigurationPaginatorTypeDef",
+    "AwsS3BucketWebsiteConfigurationExtraOutputTypeDef",
+    "AwsS3BucketWebsiteConfigurationOutputTypeDef",
     "AwsS3BucketWebsiteConfigurationTypeDef",
     "BatchUpdateFindingsResponseTypeDef",
     "AwsSsmPatchComplianceDetailsTypeDef",
-    "AwsStepFunctionStateMachineLoggingConfigurationDetailsPaginatorTypeDef",
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsExtraOutputTypeDef",
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef",
-    "AwsWafRegionalRuleGroupDetailsPaginatorTypeDef",
+    "AwsWafRegionalRuleGroupDetailsExtraOutputTypeDef",
+    "AwsWafRegionalRuleGroupDetailsOutputTypeDef",
     "AwsWafRegionalRuleGroupDetailsTypeDef",
-    "AwsWafRegionalWebAclDetailsPaginatorTypeDef",
+    "AwsWafRegionalWebAclDetailsExtraOutputTypeDef",
+    "AwsWafRegionalWebAclDetailsOutputTypeDef",
     "AwsWafRegionalWebAclDetailsTypeDef",
-    "AwsWafRuleGroupDetailsPaginatorTypeDef",
+    "AwsWafRuleGroupDetailsExtraOutputTypeDef",
+    "AwsWafRuleGroupDetailsOutputTypeDef",
     "AwsWafRuleGroupDetailsTypeDef",
-    "AwsWafWebAclDetailsPaginatorTypeDef",
+    "AwsWafWebAclDetailsExtraOutputTypeDef",
+    "AwsWafWebAclDetailsOutputTypeDef",
     "AwsWafWebAclDetailsTypeDef",
-    "AwsWafv2ActionAllowDetailsPaginatorTypeDef",
-    "AwsWafv2RulesActionCaptchaDetailsPaginatorTypeDef",
-    "AwsWafv2RulesActionCountDetailsPaginatorTypeDef",
+    "AwsWafv2ActionAllowDetailsExtraOutputTypeDef",
+    "AwsWafv2RulesActionCaptchaDetailsExtraOutputTypeDef",
+    "AwsWafv2RulesActionCountDetailsExtraOutputTypeDef",
+    "AwsWafv2ActionAllowDetailsOutputTypeDef",
+    "AwsWafv2RulesActionCaptchaDetailsOutputTypeDef",
+    "AwsWafv2RulesActionCountDetailsOutputTypeDef",
     "AwsWafv2ActionAllowDetailsTypeDef",
     "AwsWafv2RulesActionCaptchaDetailsTypeDef",
     "AwsWafv2RulesActionCountDetailsTypeDef",
-    "AwsWafv2ActionBlockDetailsPaginatorTypeDef",
+    "AwsWafv2ActionBlockDetailsExtraOutputTypeDef",
+    "AwsWafv2ActionBlockDetailsOutputTypeDef",
     "AwsWafv2ActionBlockDetailsTypeDef",
     "BatchGetStandardsControlAssociationsResponseTypeDef",
     "BatchUpdateStandardsControlAssociationsResponseTypeDef",
-    "VulnerabilityPaginatorTypeDef",
+    "VulnerabilityExtraOutputTypeDef",
+    "VulnerabilityOutputTypeDef",
     "VulnerabilityTypeDef",
     "ParameterDefinitionTypeDef",
     "BatchGetConfigurationPolicyAssociationsRequestRequestTypeDef",
     "UnprocessedConfigurationPolicyAssociationTypeDef",
+    "AutomationRulesFindingFiltersOutputTypeDef",
     "AutomationRulesFindingFiltersTypeDef",
+    "AwsSecurityFindingFiltersExtraOutputTypeDef",
+    "AwsSecurityFindingFiltersOutputTypeDef",
     "AwsSecurityFindingFiltersTypeDef",
     "GetFindingHistoryResponseTypeDef",
     "GetInsightResultsResponseTypeDef",
-    "NetworkHeaderPaginatorTypeDef",
+    "NetworkHeaderExtraOutputTypeDef",
+    "NetworkHeaderOutputTypeDef",
     "NetworkHeaderTypeDef",
-    "OccurrencesPaginatorTypeDef",
+    "OccurrencesExtraOutputTypeDef",
+    "OccurrencesOutputTypeDef",
     "OccurrencesTypeDef",
-    "SecurityControlCustomParameterTypeDef",
+    "SecurityControlCustomParameterOutputTypeDef",
     "SecurityControlTypeDef",
-    "UpdateSecurityControlRequestRequestTypeDef",
-    "RuleGroupSourceStatelessRuleDefinitionPaginatorTypeDef",
+    "ParameterConfigurationUnionTypeDef",
+    "SecurityControlCustomParameterTypeDef",
+    "RuleGroupSourceStatelessRuleDefinitionExtraOutputTypeDef",
+    "RuleGroupSourceStatelessRuleDefinitionOutputTypeDef",
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
     "DescribeStandardsResponseTypeDef",
     "BatchDisableStandardsResponseTypeDef",
     "BatchEnableStandardsResponseTypeDef",
     "GetEnabledStandardsResponseTypeDef",
-    "StatelessCustomActionDefinitionPaginatorTypeDef",
+    "StatelessCustomActionDefinitionExtraOutputTypeDef",
+    "StatelessCustomActionDefinitionOutputTypeDef",
     "StatelessCustomActionDefinitionTypeDef",
-    "PortProbeActionPaginatorTypeDef",
+    "PortProbeActionExtraOutputTypeDef",
+    "PortProbeActionOutputTypeDef",
     "PortProbeActionTypeDef",
+    "AutomationRulesActionUnionTypeDef",
     "AwsAthenaWorkGroupDetailsTypeDef",
-    "AwsAutoScalingAutoScalingGroupDetailsPaginatorTypeDef",
+    "AwsAutoScalingAutoScalingGroupDetailsExtraOutputTypeDef",
+    "AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
-    "AwsBackupBackupPlanBackupPlanDetailsPaginatorTypeDef",
+    "AwsBackupBackupPlanBackupPlanDetailsExtraOutputTypeDef",
+    "AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
-    "AwsCertificateManagerCertificateDetailsPaginatorTypeDef",
+    "AwsCertificateManagerCertificateDetailsExtraOutputTypeDef",
+    "AwsCertificateManagerCertificateDetailsOutputTypeDef",
     "AwsCertificateManagerCertificateDetailsTypeDef",
-    "AwsCloudFrontDistributionOriginsPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginsExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginsOutputTypeDef",
     "AwsCloudFrontDistributionOriginsTypeDef",
-    "AwsCloudFrontDistributionOriginGroupsPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginGroupsExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginGroupsOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupsTypeDef",
-    "AwsDynamoDbTableDetailsPaginatorTypeDef",
+    "AwsDynamoDbTableDetailsExtraOutputTypeDef",
+    "AwsDynamoDbTableDetailsOutputTypeDef",
     "AwsDynamoDbTableDetailsTypeDef",
-    "AwsEc2LaunchTemplateDetailsPaginatorTypeDef",
+    "AwsEc2LaunchTemplateDetailsExtraOutputTypeDef",
+    "AwsEc2LaunchTemplateDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDetailsTypeDef",
-    "AwsEcsClusterDetailsPaginatorTypeDef",
+    "AwsEcsClusterDetailsExtraOutputTypeDef",
+    "AwsEcsClusterDetailsOutputTypeDef",
     "AwsEcsClusterDetailsTypeDef",
-    "AwsEcsTaskDefinitionDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionDetailsTypeDef",
-    "AwsEventsEndpointDetailsPaginatorTypeDef",
+    "AwsEventsEndpointDetailsExtraOutputTypeDef",
+    "AwsEventsEndpointDetailsOutputTypeDef",
     "AwsEventsEndpointDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesDetailsTypeDef",
-    "AwsMskClusterClusterInfoDetailsPaginatorTypeDef",
+    "AwsMskClusterClusterInfoDetailsExtraOutputTypeDef",
+    "AwsMskClusterClusterInfoDetailsOutputTypeDef",
     "AwsMskClusterClusterInfoDetailsTypeDef",
-    "AwsRdsDbInstanceDetailsPaginatorTypeDef",
+    "AwsRdsDbInstanceDetailsExtraOutputTypeDef",
+    "AwsRdsDbInstanceDetailsOutputTypeDef",
     "AwsRdsDbInstanceDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsPaginatorTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsExtraOutputTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
-    "AwsS3BucketNotificationConfigurationDetailPaginatorTypeDef",
+    "AwsS3BucketNotificationConfigurationDetailExtraOutputTypeDef",
+    "AwsS3BucketNotificationConfigurationDetailOutputTypeDef",
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
-    "AwsStepFunctionStateMachineDetailsPaginatorTypeDef",
+    "AwsStepFunctionStateMachineDetailsExtraOutputTypeDef",
+    "AwsStepFunctionStateMachineDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineDetailsTypeDef",
-    "AwsWafv2RulesActionDetailsPaginatorTypeDef",
-    "AwsWafv2WebAclActionDetailsPaginatorTypeDef",
+    "AwsWafv2RulesActionDetailsExtraOutputTypeDef",
+    "AwsWafv2WebAclActionDetailsExtraOutputTypeDef",
+    "AwsWafv2RulesActionDetailsOutputTypeDef",
+    "AwsWafv2WebAclActionDetailsOutputTypeDef",
     "AwsWafv2RulesActionDetailsTypeDef",
     "AwsWafv2WebAclActionDetailsTypeDef",
     "SecurityControlDefinitionTypeDef",
     "BatchGetConfigurationPolicyAssociationsResponseTypeDef",
     "AutomationRulesConfigTypeDef",
-    "CreateAutomationRuleRequestRequestTypeDef",
+    "AutomationRulesFindingFiltersUnionTypeDef",
     "UpdateAutomationRulesRequestItemTypeDef",
+    "InsightTypeDef",
+    "AwsSecurityFindingFiltersUnionTypeDef",
     "CreateInsightRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
-    "InsightTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "UpdateInsightRequestRequestTypeDef",
-    "NetworkPathComponentPaginatorTypeDef",
+    "NetworkPathComponentExtraOutputTypeDef",
+    "NetworkPathComponentOutputTypeDef",
     "NetworkPathComponentTypeDef",
-    "CustomDataIdentifiersDetectionsPaginatorTypeDef",
-    "SensitiveDataDetectionsPaginatorTypeDef",
+    "CustomDataIdentifiersDetectionsExtraOutputTypeDef",
+    "SensitiveDataDetectionsExtraOutputTypeDef",
+    "CustomDataIdentifiersDetectionsOutputTypeDef",
+    "SensitiveDataDetectionsOutputTypeDef",
     "CustomDataIdentifiersDetectionsTypeDef",
     "SensitiveDataDetectionsTypeDef",
-    "SecurityControlsConfigurationTypeDef",
+    "SecurityControlsConfigurationOutputTypeDef",
     "BatchGetSecurityControlsResponseTypeDef",
-    "RuleGroupSourceStatelessRulesDetailsPaginatorTypeDef",
+    "UpdateSecurityControlRequestRequestTypeDef",
+    "SecurityControlsConfigurationTypeDef",
+    "RuleGroupSourceStatelessRulesDetailsExtraOutputTypeDef",
+    "RuleGroupSourceStatelessRulesDetailsOutputTypeDef",
     "RuleGroupSourceStatelessRulesDetailsTypeDef",
-    "FirewallPolicyStatelessCustomActionsDetailsPaginatorTypeDef",
-    "RuleGroupSourceCustomActionsDetailsPaginatorTypeDef",
+    "FirewallPolicyStatelessCustomActionsDetailsExtraOutputTypeDef",
+    "RuleGroupSourceCustomActionsDetailsExtraOutputTypeDef",
+    "FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef",
+    "RuleGroupSourceCustomActionsDetailsOutputTypeDef",
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     "RuleGroupSourceCustomActionsDetailsTypeDef",
-    "ActionPaginatorTypeDef",
+    "ActionExtraOutputTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
-    "AwsBackupBackupPlanDetailsPaginatorTypeDef",
+    "CreateAutomationRuleRequestRequestTypeDef",
+    "AwsBackupBackupPlanDetailsExtraOutputTypeDef",
+    "AwsBackupBackupPlanDetailsOutputTypeDef",
     "AwsBackupBackupPlanDetailsTypeDef",
-    "AwsCloudFrontDistributionDetailsPaginatorTypeDef",
+    "AwsCloudFrontDistributionDetailsExtraOutputTypeDef",
+    "AwsCloudFrontDistributionDetailsOutputTypeDef",
     "AwsCloudFrontDistributionDetailsTypeDef",
-    "AwsGuardDutyDetectorDetailsPaginatorTypeDef",
+    "AwsGuardDutyDetectorDetailsExtraOutputTypeDef",
+    "AwsGuardDutyDetectorDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDetailsTypeDef",
-    "AwsMskClusterDetailsPaginatorTypeDef",
+    "AwsMskClusterDetailsExtraOutputTypeDef",
+    "AwsMskClusterDetailsOutputTypeDef",
     "AwsMskClusterDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsPaginatorTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsExtraOutputTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
-    "AwsS3BucketNotificationConfigurationPaginatorTypeDef",
+    "AwsS3BucketNotificationConfigurationExtraOutputTypeDef",
+    "AwsS3BucketNotificationConfigurationOutputTypeDef",
     "AwsS3BucketNotificationConfigurationTypeDef",
-    "AwsWafv2RulesDetailsPaginatorTypeDef",
+    "AwsWafv2RulesDetailsExtraOutputTypeDef",
+    "AwsWafv2RulesDetailsOutputTypeDef",
     "AwsWafv2RulesDetailsTypeDef",
     "GetSecurityControlDefinitionResponseTypeDef",
     "ListSecurityControlDefinitionsResponseTypeDef",
     "BatchGetAutomationRulesResponseTypeDef",
     "BatchUpdateAutomationRulesRequestRequestTypeDef",
     "GetInsightsResponseTypeDef",
-    "CustomDataIdentifiersResultPaginatorTypeDef",
-    "SensitiveDataResultPaginatorTypeDef",
+    "CustomDataIdentifiersResultExtraOutputTypeDef",
+    "SensitiveDataResultExtraOutputTypeDef",
+    "CustomDataIdentifiersResultOutputTypeDef",
+    "SensitiveDataResultOutputTypeDef",
     "CustomDataIdentifiersResultTypeDef",
     "SensitiveDataResultTypeDef",
+    "SecurityHubPolicyOutputTypeDef",
     "SecurityHubPolicyTypeDef",
-    "FirewallPolicyDetailsPaginatorTypeDef",
-    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsPaginatorTypeDef",
+    "FirewallPolicyDetailsExtraOutputTypeDef",
+    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsExtraOutputTypeDef",
+    "FirewallPolicyDetailsOutputTypeDef",
+    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef",
     "FirewallPolicyDetailsTypeDef",
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationDetailsPaginatorTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationDetailsExtraOutputTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
-    "AwsWafv2RuleGroupDetailsPaginatorTypeDef",
-    "AwsWafv2WebAclDetailsPaginatorTypeDef",
+    "AwsWafv2RuleGroupDetailsExtraOutputTypeDef",
+    "AwsWafv2WebAclDetailsExtraOutputTypeDef",
+    "AwsWafv2RuleGroupDetailsOutputTypeDef",
+    "AwsWafv2WebAclDetailsOutputTypeDef",
     "AwsWafv2RuleGroupDetailsTypeDef",
     "AwsWafv2WebAclDetailsTypeDef",
-    "ClassificationResultPaginatorTypeDef",
+    "ClassificationResultExtraOutputTypeDef",
+    "ClassificationResultOutputTypeDef",
     "ClassificationResultTypeDef",
+    "PolicyOutputTypeDef",
     "PolicyTypeDef",
-    "AwsNetworkFirewallFirewallPolicyDetailsPaginatorTypeDef",
-    "RuleGroupSourcePaginatorTypeDef",
+    "AwsNetworkFirewallFirewallPolicyDetailsExtraOutputTypeDef",
+    "RuleGroupSourceExtraOutputTypeDef",
+    "AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef",
+    "RuleGroupSourceOutputTypeDef",
     "AwsNetworkFirewallFirewallPolicyDetailsTypeDef",
     "RuleGroupSourceTypeDef",
-    "AwsS3BucketDetailsPaginatorTypeDef",
+    "AwsS3BucketDetailsExtraOutputTypeDef",
+    "AwsS3BucketDetailsOutputTypeDef",
     "AwsS3BucketDetailsTypeDef",
-    "DataClassificationDetailsPaginatorTypeDef",
+    "DataClassificationDetailsExtraOutputTypeDef",
+    "DataClassificationDetailsOutputTypeDef",
     "DataClassificationDetailsTypeDef",
-    "CreateConfigurationPolicyRequestRequestTypeDef",
     "CreateConfigurationPolicyResponseTypeDef",
     "GetConfigurationPolicyResponseTypeDef",
-    "UpdateConfigurationPolicyRequestRequestTypeDef",
     "UpdateConfigurationPolicyResponseTypeDef",
-    "RuleGroupDetailsPaginatorTypeDef",
+    "CreateConfigurationPolicyRequestRequestTypeDef",
+    "PolicyUnionTypeDef",
+    "UpdateConfigurationPolicyRequestRequestTypeDef",
+    "RuleGroupDetailsExtraOutputTypeDef",
+    "RuleGroupDetailsOutputTypeDef",
     "RuleGroupDetailsTypeDef",
-    "AwsNetworkFirewallRuleGroupDetailsPaginatorTypeDef",
+    "AwsNetworkFirewallRuleGroupDetailsExtraOutputTypeDef",
+    "AwsNetworkFirewallRuleGroupDetailsOutputTypeDef",
     "AwsNetworkFirewallRuleGroupDetailsTypeDef",
-    "ResourceDetailsPaginatorTypeDef",
+    "ResourceDetailsExtraOutputTypeDef",
+    "ResourceDetailsOutputTypeDef",
     "ResourceDetailsTypeDef",
-    "ResourcePaginatorTypeDef",
+    "ResourceExtraOutputTypeDef",
+    "ResourceOutputTypeDef",
     "ResourceTypeDef",
-    "AwsSecurityFindingPaginatorTypeDef",
+    "AwsSecurityFindingExtraOutputTypeDef",
+    "AwsSecurityFindingOutputTypeDef",
     "AwsSecurityFindingTypeDef",
-    "GetFindingsResponsePaginatorTypeDef",
-    "BatchImportFindingsRequestRequestTypeDef",
     "GetFindingsResponseTypeDef",
+    "AwsSecurityFindingUnionTypeDef",
+    "BatchImportFindingsRequestRequestTypeDef",
 )
 
 AcceptAdministratorInvitationRequestRequestTypeDef = TypedDict(
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     {
         "AdministratorId": str,
         "InvitationId": str,
@@ -1123,35 +1349,35 @@
 AccountDetailsTypeDef = TypedDict(
     "AccountDetailsTypeDef",
     {
         "AccountId": str,
         "Email": NotRequired[str],
     },
 )
+DnsRequestActionTypeDef = TypedDict(
+    "DnsRequestActionTypeDef",
+    {
+        "Domain": NotRequired[str],
+        "Protocol": NotRequired[str],
+        "Blocked": NotRequired[bool],
+    },
+)
 ActionLocalIpDetailsTypeDef = TypedDict(
     "ActionLocalIpDetailsTypeDef",
     {
         "IpAddressV4": NotRequired[str],
     },
 )
 ActionLocalPortDetailsTypeDef = TypedDict(
     "ActionLocalPortDetailsTypeDef",
     {
         "Port": NotRequired[int],
         "PortName": NotRequired[str],
     },
 )
-DnsRequestActionTypeDef = TypedDict(
-    "DnsRequestActionTypeDef",
-    {
-        "Domain": NotRequired[str],
-        "Protocol": NotRequired[str],
-        "Blocked": NotRequired[bool],
-    },
-)
 CityTypeDef = TypedDict(
     "CityTypeDef",
     {
         "CityName": NotRequired[str],
     },
 )
 CountryTypeDef = TypedDict(
@@ -1304,16 +1530,16 @@
 AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
     {
         "KmsKeyId": NotRequired[str],
         "UseAwsOwnedKey": NotRequired[bool],
     },
 )
-AwsAmazonMqBrokerLdapServerMetadataDetailsPaginatorTypeDef = TypedDict(
-    "AwsAmazonMqBrokerLdapServerMetadataDetailsPaginatorTypeDef",
+AwsAmazonMqBrokerLdapServerMetadataDetailsExtraOutputTypeDef = TypedDict(
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsExtraOutputTypeDef",
     {
         "Hosts": NotRequired[List[str]],
         "RoleBase": NotRequired[str],
         "RoleName": NotRequired[str],
         "RoleSearchMatching": NotRequired[str],
         "RoleSearchSubtree": NotRequired[bool],
         "ServiceAccountUsername": NotRequired[str],
@@ -1334,14 +1560,29 @@
 AwsAmazonMqBrokerUsersDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerUsersDetailsTypeDef",
     {
         "PendingChange": NotRequired[str],
         "Username": NotRequired[str],
     },
 )
+AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef = TypedDict(
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef",
+    {
+        "Hosts": NotRequired[List[str]],
+        "RoleBase": NotRequired[str],
+        "RoleName": NotRequired[str],
+        "RoleSearchMatching": NotRequired[str],
+        "RoleSearchSubtree": NotRequired[bool],
+        "ServiceAccountUsername": NotRequired[str],
+        "UserBase": NotRequired[str],
+        "UserRoleName": NotRequired[str],
+        "UserSearchMatching": NotRequired[str],
+        "UserSearchSubtree": NotRequired[bool],
+    },
+)
 AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
     {
         "Hosts": NotRequired[Sequence[str]],
         "RoleBase": NotRequired[str],
         "RoleName": NotRequired[str],
         "RoleSearchMatching": NotRequired[str],
@@ -1369,16 +1610,25 @@
 AwsApiGatewayAccessLogSettingsTypeDef = TypedDict(
     "AwsApiGatewayAccessLogSettingsTypeDef",
     {
         "Format": NotRequired[str],
         "DestinationArn": NotRequired[str],
     },
 )
-AwsApiGatewayCanarySettingsPaginatorTypeDef = TypedDict(
-    "AwsApiGatewayCanarySettingsPaginatorTypeDef",
+AwsApiGatewayCanarySettingsExtraOutputTypeDef = TypedDict(
+    "AwsApiGatewayCanarySettingsExtraOutputTypeDef",
+    {
+        "PercentTraffic": NotRequired[float],
+        "DeploymentId": NotRequired[str],
+        "StageVariableOverrides": NotRequired[Dict[str, str]],
+        "UseStageCache": NotRequired[bool],
+    },
+)
+AwsApiGatewayCanarySettingsOutputTypeDef = TypedDict(
+    "AwsApiGatewayCanarySettingsOutputTypeDef",
     {
         "PercentTraffic": NotRequired[float],
         "DeploymentId": NotRequired[str],
         "StageVariableOverrides": NotRequired[Dict[str, str]],
         "UseStageCache": NotRequired[bool],
     },
 )
@@ -1387,16 +1637,22 @@
     {
         "PercentTraffic": NotRequired[float],
         "DeploymentId": NotRequired[str],
         "StageVariableOverrides": NotRequired[Mapping[str, str]],
         "UseStageCache": NotRequired[bool],
     },
 )
-AwsApiGatewayEndpointConfigurationPaginatorTypeDef = TypedDict(
-    "AwsApiGatewayEndpointConfigurationPaginatorTypeDef",
+AwsApiGatewayEndpointConfigurationExtraOutputTypeDef = TypedDict(
+    "AwsApiGatewayEndpointConfigurationExtraOutputTypeDef",
+    {
+        "Types": NotRequired[List[str]],
+    },
+)
+AwsApiGatewayEndpointConfigurationOutputTypeDef = TypedDict(
+    "AwsApiGatewayEndpointConfigurationOutputTypeDef",
     {
         "Types": NotRequired[List[str]],
     },
 )
 AwsApiGatewayEndpointConfigurationTypeDef = TypedDict(
     "AwsApiGatewayEndpointConfigurationTypeDef",
     {
@@ -1416,16 +1672,27 @@
         "CacheDataEncrypted": NotRequired[bool],
         "RequireAuthorizationForCacheControl": NotRequired[bool],
         "UnauthorizedCacheControlHeaderStrategy": NotRequired[str],
         "HttpMethod": NotRequired[str],
         "ResourcePath": NotRequired[str],
     },
 )
-AwsCorsConfigurationPaginatorTypeDef = TypedDict(
-    "AwsCorsConfigurationPaginatorTypeDef",
+AwsCorsConfigurationExtraOutputTypeDef = TypedDict(
+    "AwsCorsConfigurationExtraOutputTypeDef",
+    {
+        "AllowOrigins": NotRequired[List[str]],
+        "AllowCredentials": NotRequired[bool],
+        "ExposeHeaders": NotRequired[List[str]],
+        "MaxAge": NotRequired[int],
+        "AllowMethods": NotRequired[List[str]],
+        "AllowHeaders": NotRequired[List[str]],
+    },
+)
+AwsCorsConfigurationOutputTypeDef = TypedDict(
+    "AwsCorsConfigurationOutputTypeDef",
     {
         "AllowOrigins": NotRequired[List[str]],
         "AllowCredentials": NotRequired[bool],
         "ExposeHeaders": NotRequired[List[str]],
         "MaxAge": NotRequired[int],
         "AllowMethods": NotRequired[List[str]],
         "AllowHeaders": NotRequired[List[str]],
@@ -1554,16 +1821,23 @@
     "AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef",
     {
         "HttpEndpoint": NotRequired[str],
         "HttpPutResponseHopLimit": NotRequired[int],
         "HttpTokens": NotRequired[str],
     },
 )
-AwsBackupBackupPlanAdvancedBackupSettingsDetailsPaginatorTypeDef = TypedDict(
-    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsPaginatorTypeDef",
+AwsBackupBackupPlanAdvancedBackupSettingsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsExtraOutputTypeDef",
+    {
+        "BackupOptions": NotRequired[Dict[str, str]],
+        "ResourceType": NotRequired[str],
+    },
+)
+AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef",
     {
         "BackupOptions": NotRequired[Dict[str, str]],
         "ResourceType": NotRequired[str],
     },
 )
 AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef",
@@ -1575,16 +1849,23 @@
 AwsBackupBackupPlanLifecycleDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanLifecycleDetailsTypeDef",
     {
         "DeleteAfterDays": NotRequired[int],
         "MoveToColdStorageAfterDays": NotRequired[int],
     },
 )
-AwsBackupBackupVaultNotificationsDetailsPaginatorTypeDef = TypedDict(
-    "AwsBackupBackupVaultNotificationsDetailsPaginatorTypeDef",
+AwsBackupBackupVaultNotificationsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsBackupBackupVaultNotificationsDetailsExtraOutputTypeDef",
+    {
+        "BackupVaultEvents": NotRequired[List[str]],
+        "SnsTopicArn": NotRequired[str],
+    },
+)
+AwsBackupBackupVaultNotificationsDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupVaultNotificationsDetailsOutputTypeDef",
     {
         "BackupVaultEvents": NotRequired[List[str]],
         "SnsTopicArn": NotRequired[str],
     },
 )
 AwsBackupBackupVaultNotificationsDetailsTypeDef = TypedDict(
     "AwsBackupBackupVaultNotificationsDetailsTypeDef",
@@ -1686,30 +1967,44 @@
         "CertificateSource": NotRequired[str],
         "CloudFrontDefaultCertificate": NotRequired[bool],
         "IamCertificateId": NotRequired[str],
         "MinimumProtocolVersion": NotRequired[str],
         "SslSupportMethod": NotRequired[str],
     },
 )
-AwsCloudFrontDistributionOriginSslProtocolsPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginSslProtocolsPaginatorTypeDef",
+AwsCloudFrontDistributionOriginSslProtocolsExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginSslProtocolsExtraOutputTypeDef",
+    {
+        "Items": NotRequired[List[str]],
+        "Quantity": NotRequired[int],
+    },
+)
+AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef",
     {
         "Items": NotRequired[List[str]],
         "Quantity": NotRequired[int],
     },
 )
 AwsCloudFrontDistributionOriginSslProtocolsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginSslProtocolsTypeDef",
     {
         "Items": NotRequired[Sequence[str]],
         "Quantity": NotRequired[int],
     },
 )
-AwsCloudFrontDistributionOriginGroupFailoverStatusCodesPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesPaginatorTypeDef",
+AwsCloudFrontDistributionOriginGroupFailoverStatusCodesExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesExtraOutputTypeDef",
+    {
+        "Items": NotRequired[List[int]],
+        "Quantity": NotRequired[int],
+    },
+)
+AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef",
     {
         "Items": NotRequired[List[int]],
         "Quantity": NotRequired[int],
     },
 )
 AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef",
@@ -1770,16 +2065,24 @@
     {
         "Type": NotRequired[str],
         "Location": NotRequired[str],
         "GitCloneDepth": NotRequired[int],
         "InsecureSsl": NotRequired[bool],
     },
 )
-AwsCodeBuildProjectVpcConfigPaginatorTypeDef = TypedDict(
-    "AwsCodeBuildProjectVpcConfigPaginatorTypeDef",
+AwsCodeBuildProjectVpcConfigExtraOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectVpcConfigExtraOutputTypeDef",
+    {
+        "VpcId": NotRequired[str],
+        "Subnets": NotRequired[List[str]],
+        "SecurityGroupIds": NotRequired[List[str]],
+    },
+)
+AwsCodeBuildProjectVpcConfigOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectVpcConfigOutputTypeDef",
     {
         "VpcId": NotRequired[str],
         "Subnets": NotRequired[List[str]],
         "SecurityGroupIds": NotRequired[List[str]],
     },
 )
 AwsCodeBuildProjectVpcConfigTypeDef = TypedDict(
@@ -1921,16 +2224,23 @@
 AwsDynamoDbTableStreamSpecificationTypeDef = TypedDict(
     "AwsDynamoDbTableStreamSpecificationTypeDef",
     {
         "StreamEnabled": NotRequired[bool],
         "StreamViewType": NotRequired[str],
     },
 )
-AwsDynamoDbTableProjectionPaginatorTypeDef = TypedDict(
-    "AwsDynamoDbTableProjectionPaginatorTypeDef",
+AwsDynamoDbTableProjectionExtraOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableProjectionExtraOutputTypeDef",
+    {
+        "NonKeyAttributes": NotRequired[List[str]],
+        "ProjectionType": NotRequired[str],
+    },
+)
+AwsDynamoDbTableProjectionOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableProjectionOutputTypeDef",
     {
         "NonKeyAttributes": NotRequired[List[str]],
         "ProjectionType": NotRequired[str],
     },
 )
 AwsDynamoDbTableProjectionTypeDef = TypedDict(
     "AwsDynamoDbTableProjectionTypeDef",
@@ -2342,16 +2652,33 @@
     "Ipv6CidrBlockAssociationTypeDef",
     {
         "AssociationId": NotRequired[str],
         "Ipv6CidrBlock": NotRequired[str],
         "CidrBlockState": NotRequired[str],
     },
 )
-AwsEc2TransitGatewayDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2TransitGatewayDetailsPaginatorTypeDef",
+AwsEc2TransitGatewayDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2TransitGatewayDetailsExtraOutputTypeDef",
+    {
+        "Id": NotRequired[str],
+        "Description": NotRequired[str],
+        "DefaultRouteTablePropagation": NotRequired[str],
+        "AutoAcceptSharedAttachments": NotRequired[str],
+        "DefaultRouteTableAssociation": NotRequired[str],
+        "TransitGatewayCidrBlocks": NotRequired[List[str]],
+        "AssociationDefaultRouteTableId": NotRequired[str],
+        "PropagationDefaultRouteTableId": NotRequired[str],
+        "VpnEcmpSupport": NotRequired[str],
+        "DnsSupport": NotRequired[str],
+        "MulticastSupport": NotRequired[str],
+        "AmazonSideAsn": NotRequired[int],
+    },
+)
+AwsEc2TransitGatewayDetailsOutputTypeDef = TypedDict(
+    "AwsEc2TransitGatewayDetailsOutputTypeDef",
     {
         "Id": NotRequired[str],
         "Description": NotRequired[str],
         "DefaultRouteTablePropagation": NotRequired[str],
         "AutoAcceptSharedAttachments": NotRequired[str],
         "DefaultRouteTableAssociation": NotRequired[str],
         "TransitGatewayCidrBlocks": NotRequired[List[str]],
@@ -2444,16 +2771,37 @@
         "CertificateArn": NotRequired[str],
         "LastStatusChange": NotRequired[str],
         "OutsideIpAddress": NotRequired[str],
         "Status": NotRequired[str],
         "StatusMessage": NotRequired[str],
     },
 )
-AwsEc2VpnConnectionOptionsTunnelOptionsDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsPaginatorTypeDef",
+AwsEc2VpnConnectionOptionsTunnelOptionsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsExtraOutputTypeDef",
+    {
+        "DpdTimeoutSeconds": NotRequired[int],
+        "IkeVersions": NotRequired[List[str]],
+        "OutsideIpAddress": NotRequired[str],
+        "Phase1DhGroupNumbers": NotRequired[List[int]],
+        "Phase1EncryptionAlgorithms": NotRequired[List[str]],
+        "Phase1IntegrityAlgorithms": NotRequired[List[str]],
+        "Phase1LifetimeSeconds": NotRequired[int],
+        "Phase2DhGroupNumbers": NotRequired[List[int]],
+        "Phase2EncryptionAlgorithms": NotRequired[List[str]],
+        "Phase2IntegrityAlgorithms": NotRequired[List[str]],
+        "Phase2LifetimeSeconds": NotRequired[int],
+        "PreSharedKey": NotRequired[str],
+        "RekeyFuzzPercentage": NotRequired[int],
+        "RekeyMarginTimeSeconds": NotRequired[int],
+        "ReplayWindowSize": NotRequired[int],
+        "TunnelInsideCidr": NotRequired[str],
+    },
+)
+AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef",
     {
         "DpdTimeoutSeconds": NotRequired[int],
         "IkeVersions": NotRequired[List[str]],
         "OutsideIpAddress": NotRequired[str],
         "Phase1DhGroupNumbers": NotRequired[List[int]],
         "Phase1EncryptionAlgorithms": NotRequired[List[str]],
         "Phase1IntegrityAlgorithms": NotRequired[List[str]],
@@ -2486,16 +2834,27 @@
         "PreSharedKey": NotRequired[str],
         "RekeyFuzzPercentage": NotRequired[int],
         "RekeyMarginTimeSeconds": NotRequired[int],
         "ReplayWindowSize": NotRequired[int],
         "TunnelInsideCidr": NotRequired[str],
     },
 )
-AwsEcrContainerImageDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcrContainerImageDetailsPaginatorTypeDef",
+AwsEcrContainerImageDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcrContainerImageDetailsExtraOutputTypeDef",
+    {
+        "RegistryId": NotRequired[str],
+        "RepositoryName": NotRequired[str],
+        "Architecture": NotRequired[str],
+        "ImageDigest": NotRequired[str],
+        "ImageTags": NotRequired[List[str]],
+        "ImagePublishedAt": NotRequired[str],
+    },
+)
+AwsEcrContainerImageDetailsOutputTypeDef = TypedDict(
+    "AwsEcrContainerImageDetailsOutputTypeDef",
     {
         "RegistryId": NotRequired[str],
         "RepositoryName": NotRequired[str],
         "Architecture": NotRequired[str],
         "ImageDigest": NotRequired[str],
         "ImageTags": NotRequired[List[str]],
         "ImagePublishedAt": NotRequired[str],
@@ -2606,16 +2965,24 @@
     {
         "ContainerName": NotRequired[str],
         "ContainerPort": NotRequired[int],
         "Port": NotRequired[int],
         "RegistryArn": NotRequired[str],
     },
 )
-AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsPaginatorTypeDef",
+AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsExtraOutputTypeDef",
+    {
+        "AssignPublicIp": NotRequired[str],
+        "SecurityGroups": NotRequired[List[str]],
+        "Subnets": NotRequired[List[str]],
+    },
+)
+AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef",
     {
         "AssignPublicIp": NotRequired[str],
         "SecurityGroups": NotRequired[List[str]],
         "Subnets": NotRequired[List[str]],
     },
 )
 AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef = TypedDict(
@@ -2650,23 +3017,23 @@
 AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef",
     {
         "Hostname": NotRequired[str],
         "IpAddress": NotRequired[str],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsExtraOutputTypeDef",
     {
         "Options": NotRequired[Dict[str, str]],
         "Type": NotRequired[str],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsExtraOutputTypeDef",
     {
         "Command": NotRequired[List[str]],
         "Interval": NotRequired[int],
         "Retries": NotRequired[int],
         "StartPeriod": NotRequired[int],
         "Timeout": NotRequired[int],
     },
@@ -2725,14 +3092,31 @@
 AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef",
     {
         "ReadOnly": NotRequired[bool],
         "SourceContainer": NotRequired[str],
     },
 )
+AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef",
+    {
+        "Options": NotRequired[Dict[str, str]],
+        "Type": NotRequired[str],
+    },
+)
+AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef",
+    {
+        "Command": NotRequired[List[str]],
+        "Interval": NotRequired[int],
+        "Retries": NotRequired[int],
+        "StartPeriod": NotRequired[int],
+        "Timeout": NotRequired[int],
+    },
+)
 AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
     {
         "Options": NotRequired[Mapping[str, str]],
         "Type": NotRequired[str],
     },
 )
@@ -2742,38 +3126,61 @@
         "Command": NotRequired[Sequence[str]],
         "Interval": NotRequired[int],
         "Retries": NotRequired[int],
         "StartPeriod": NotRequired[int],
         "Timeout": NotRequired[int],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsExtraOutputTypeDef",
+    {
+        "Add": NotRequired[List[str]],
+        "Drop": NotRequired[List[str]],
+    },
+)
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef",
     {
         "Add": NotRequired[List[str]],
         "Drop": NotRequired[List[str]],
     },
 )
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef",
     {
         "Add": NotRequired[Sequence[str]],
         "Drop": NotRequired[Sequence[str]],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsExtraOutputTypeDef",
+    {
+        "ContainerPath": NotRequired[str],
+        "HostPath": NotRequired[str],
+        "Permissions": NotRequired[List[str]],
+    },
+)
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsExtraOutputTypeDef",
+    {
+        "ContainerPath": NotRequired[str],
+        "MountOptions": NotRequired[List[str]],
+        "Size": NotRequired[int],
+    },
+)
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef",
     {
         "ContainerPath": NotRequired[str],
         "HostPath": NotRequired[str],
         "Permissions": NotRequired[List[str]],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef",
     {
         "ContainerPath": NotRequired[str],
         "MountOptions": NotRequired[List[str]],
         "Size": NotRequired[int],
     },
 )
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef = TypedDict(
@@ -2816,30 +3223,40 @@
 AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef",
     {
         "Name": NotRequired[str],
         "Value": NotRequired[str],
     },
 )
-AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsExtraOutputTypeDef",
     {
         "Autoprovision": NotRequired[bool],
         "Driver": NotRequired[str],
         "DriverOpts": NotRequired[Dict[str, str]],
         "Labels": NotRequired[Dict[str, str]],
         "Scope": NotRequired[str],
     },
 )
 AwsEcsTaskDefinitionVolumesHostDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesHostDetailsTypeDef",
     {
         "SourcePath": NotRequired[str],
     },
 )
+AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef",
+    {
+        "Autoprovision": NotRequired[bool],
+        "Driver": NotRequired[str],
+        "DriverOpts": NotRequired[Dict[str, str]],
+        "Labels": NotRequired[Dict[str, str]],
+        "Scope": NotRequired[str],
+    },
+)
 AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
     {
         "Autoprovision": NotRequired[bool],
         "Driver": NotRequired[str],
         "DriverOpts": NotRequired[Mapping[str, str]],
         "Labels": NotRequired[Mapping[str, str]],
@@ -2855,16 +3272,24 @@
 )
 AwsEcsTaskVolumeHostDetailsTypeDef = TypedDict(
     "AwsEcsTaskVolumeHostDetailsTypeDef",
     {
         "SourcePath": NotRequired[str],
     },
 )
-AwsEfsAccessPointPosixUserDetailsPaginatorTypeDef = TypedDict(
-    "AwsEfsAccessPointPosixUserDetailsPaginatorTypeDef",
+AwsEfsAccessPointPosixUserDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEfsAccessPointPosixUserDetailsExtraOutputTypeDef",
+    {
+        "Gid": NotRequired[str],
+        "SecondaryGids": NotRequired[List[str]],
+        "Uid": NotRequired[str],
+    },
+)
+AwsEfsAccessPointPosixUserDetailsOutputTypeDef = TypedDict(
+    "AwsEfsAccessPointPosixUserDetailsOutputTypeDef",
     {
         "Gid": NotRequired[str],
         "SecondaryGids": NotRequired[List[str]],
         "Uid": NotRequired[str],
     },
 )
 AwsEfsAccessPointPosixUserDetailsTypeDef = TypedDict(
@@ -2879,32 +3304,47 @@
     "AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef",
     {
         "OwnerGid": NotRequired[str],
         "OwnerUid": NotRequired[str],
         "Permissions": NotRequired[str],
     },
 )
-AwsEksClusterResourcesVpcConfigDetailsPaginatorTypeDef = TypedDict(
-    "AwsEksClusterResourcesVpcConfigDetailsPaginatorTypeDef",
+AwsEksClusterResourcesVpcConfigDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEksClusterResourcesVpcConfigDetailsExtraOutputTypeDef",
+    {
+        "SecurityGroupIds": NotRequired[List[str]],
+        "SubnetIds": NotRequired[List[str]],
+        "EndpointPublicAccess": NotRequired[bool],
+    },
+)
+AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef",
     {
         "SecurityGroupIds": NotRequired[List[str]],
         "SubnetIds": NotRequired[List[str]],
         "EndpointPublicAccess": NotRequired[bool],
     },
 )
 AwsEksClusterResourcesVpcConfigDetailsTypeDef = TypedDict(
     "AwsEksClusterResourcesVpcConfigDetailsTypeDef",
     {
         "SecurityGroupIds": NotRequired[Sequence[str]],
         "SubnetIds": NotRequired[Sequence[str]],
         "EndpointPublicAccess": NotRequired[bool],
     },
 )
-AwsEksClusterLoggingClusterLoggingDetailsPaginatorTypeDef = TypedDict(
-    "AwsEksClusterLoggingClusterLoggingDetailsPaginatorTypeDef",
+AwsEksClusterLoggingClusterLoggingDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEksClusterLoggingClusterLoggingDetailsExtraOutputTypeDef",
+    {
+        "Enabled": NotRequired[bool],
+        "Types": NotRequired[List[str]],
+    },
+)
+AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef",
     {
         "Enabled": NotRequired[bool],
         "Types": NotRequired[List[str]],
     },
 )
 AwsEksClusterLoggingClusterLoggingDetailsTypeDef = TypedDict(
     "AwsEksClusterLoggingClusterLoggingDetailsTypeDef",
@@ -2965,16 +3405,25 @@
         "CurrentVersion": NotRequired[str],
         "Description": NotRequired[str],
         "NewVersion": NotRequired[str],
         "UpdateAvailable": NotRequired[bool],
         "UpdateStatus": NotRequired[str],
     },
 )
-AwsElasticsearchDomainVPCOptionsPaginatorTypeDef = TypedDict(
-    "AwsElasticsearchDomainVPCOptionsPaginatorTypeDef",
+AwsElasticsearchDomainVPCOptionsExtraOutputTypeDef = TypedDict(
+    "AwsElasticsearchDomainVPCOptionsExtraOutputTypeDef",
+    {
+        "AvailabilityZones": NotRequired[List[str]],
+        "SecurityGroupIds": NotRequired[List[str]],
+        "SubnetIds": NotRequired[List[str]],
+        "VPCId": NotRequired[str],
+    },
+)
+AwsElasticsearchDomainVPCOptionsOutputTypeDef = TypedDict(
+    "AwsElasticsearchDomainVPCOptionsOutputTypeDef",
     {
         "AvailabilityZones": NotRequired[List[str]],
         "SecurityGroupIds": NotRequired[List[str]],
         "SubnetIds": NotRequired[List[str]],
         "VPCId": NotRequired[str],
     },
 )
@@ -3045,16 +3494,23 @@
 )
 AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef = TypedDict(
     "AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef",
     {
         "Enabled": NotRequired[bool],
     },
 )
-AwsElbLoadBalancerBackendServerDescriptionPaginatorTypeDef = TypedDict(
-    "AwsElbLoadBalancerBackendServerDescriptionPaginatorTypeDef",
+AwsElbLoadBalancerBackendServerDescriptionExtraOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerBackendServerDescriptionExtraOutputTypeDef",
+    {
+        "InstancePort": NotRequired[int],
+        "PolicyNames": NotRequired[List[str]],
+    },
+)
+AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef",
     {
         "InstancePort": NotRequired[int],
         "PolicyNames": NotRequired[List[str]],
     },
 )
 AwsElbLoadBalancerBackendServerDescriptionTypeDef = TypedDict(
     "AwsElbLoadBalancerBackendServerDescriptionTypeDef",
@@ -3306,16 +3762,24 @@
 )
 AwsLambdaFunctionTracingConfigTypeDef = TypedDict(
     "AwsLambdaFunctionTracingConfigTypeDef",
     {
         "Mode": NotRequired[str],
     },
 )
-AwsLambdaFunctionVpcConfigPaginatorTypeDef = TypedDict(
-    "AwsLambdaFunctionVpcConfigPaginatorTypeDef",
+AwsLambdaFunctionVpcConfigExtraOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionVpcConfigExtraOutputTypeDef",
+    {
+        "SecurityGroupIds": NotRequired[List[str]],
+        "SubnetIds": NotRequired[List[str]],
+        "VpcId": NotRequired[str],
+    },
+)
+AwsLambdaFunctionVpcConfigOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionVpcConfigOutputTypeDef",
     {
         "SecurityGroupIds": NotRequired[List[str]],
         "SubnetIds": NotRequired[List[str]],
         "VpcId": NotRequired[str],
     },
 )
 AwsLambdaFunctionVpcConfigTypeDef = TypedDict(
@@ -3329,43 +3793,58 @@
 AwsLambdaFunctionEnvironmentErrorTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentErrorTypeDef",
     {
         "ErrorCode": NotRequired[str],
         "Message": NotRequired[str],
     },
 )
-AwsLambdaLayerVersionDetailsPaginatorTypeDef = TypedDict(
-    "AwsLambdaLayerVersionDetailsPaginatorTypeDef",
+AwsLambdaLayerVersionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsLambdaLayerVersionDetailsExtraOutputTypeDef",
+    {
+        "Version": NotRequired[int],
+        "CompatibleRuntimes": NotRequired[List[str]],
+        "CreatedDate": NotRequired[str],
+    },
+)
+AwsLambdaLayerVersionDetailsOutputTypeDef = TypedDict(
+    "AwsLambdaLayerVersionDetailsOutputTypeDef",
     {
         "Version": NotRequired[int],
         "CompatibleRuntimes": NotRequired[List[str]],
         "CreatedDate": NotRequired[str],
     },
 )
 AwsLambdaLayerVersionDetailsTypeDef = TypedDict(
     "AwsLambdaLayerVersionDetailsTypeDef",
     {
         "Version": NotRequired[int],
         "CompatibleRuntimes": NotRequired[Sequence[str]],
         "CreatedDate": NotRequired[str],
     },
 )
-AwsMskClusterClusterInfoClientAuthenticationTlsDetailsPaginatorTypeDef = TypedDict(
-    "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsPaginatorTypeDef",
+AwsMskClusterClusterInfoClientAuthenticationTlsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsExtraOutputTypeDef",
     {
         "CertificateAuthorityArnList": NotRequired[List[str]],
         "Enabled": NotRequired[bool],
     },
 )
 AwsMskClusterClusterInfoClientAuthenticationUnauthenticatedDetailsTypeDef = TypedDict(
     "AwsMskClusterClusterInfoClientAuthenticationUnauthenticatedDetailsTypeDef",
     {
         "Enabled": NotRequired[bool],
     },
 )
+AwsMskClusterClusterInfoClientAuthenticationTlsDetailsOutputTypeDef = TypedDict(
+    "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsOutputTypeDef",
+    {
+        "CertificateAuthorityArnList": NotRequired[List[str]],
+        "Enabled": NotRequired[bool],
+    },
+)
 AwsMskClusterClusterInfoClientAuthenticationTlsDetailsTypeDef = TypedDict(
     "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsTypeDef",
     {
         "CertificateAuthorityArnList": NotRequired[Sequence[str]],
         "Enabled": NotRequired[bool],
     },
 )
@@ -3446,16 +3925,23 @@
         "Description": NotRequired[str],
         "NewVersion": NotRequired[str],
         "UpdateAvailable": NotRequired[bool],
         "UpdateStatus": NotRequired[str],
         "OptionalDeployment": NotRequired[bool],
     },
 )
-AwsOpenSearchServiceDomainVpcOptionsDetailsPaginatorTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainVpcOptionsDetailsPaginatorTypeDef",
+AwsOpenSearchServiceDomainVpcOptionsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsExtraOutputTypeDef",
+    {
+        "SecurityGroupIds": NotRequired[List[str]],
+        "SubnetIds": NotRequired[List[str]],
+    },
+)
+AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
     {
         "SecurityGroupIds": NotRequired[List[str]],
         "SubnetIds": NotRequired[List[str]],
     },
 )
 AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef",
@@ -3506,16 +3992,23 @@
 AwsRdsDbInstanceVpcSecurityGroupTypeDef = TypedDict(
     "AwsRdsDbInstanceVpcSecurityGroupTypeDef",
     {
         "VpcSecurityGroupId": NotRequired[str],
         "Status": NotRequired[str],
     },
 )
-AwsRdsDbClusterSnapshotDbClusterSnapshotAttributePaginatorTypeDef = TypedDict(
-    "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributePaginatorTypeDef",
+AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeExtraOutputTypeDef",
+    {
+        "AttributeName": NotRequired[str],
+        "AttributeValues": NotRequired[List[str]],
+    },
+)
+AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef",
     {
         "AttributeName": NotRequired[str],
         "AttributeValues": NotRequired[List[str]],
     },
 )
 AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef = TypedDict(
     "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef",
@@ -3566,16 +4059,23 @@
     {
         "StatusType": NotRequired[str],
         "Normal": NotRequired[bool],
         "Status": NotRequired[str],
         "Message": NotRequired[str],
     },
 )
-AwsRdsPendingCloudWatchLogsExportsPaginatorTypeDef = TypedDict(
-    "AwsRdsPendingCloudWatchLogsExportsPaginatorTypeDef",
+AwsRdsPendingCloudWatchLogsExportsExtraOutputTypeDef = TypedDict(
+    "AwsRdsPendingCloudWatchLogsExportsExtraOutputTypeDef",
+    {
+        "LogTypesToEnable": NotRequired[List[str]],
+        "LogTypesToDisable": NotRequired[List[str]],
+    },
+)
+AwsRdsPendingCloudWatchLogsExportsOutputTypeDef = TypedDict(
+    "AwsRdsPendingCloudWatchLogsExportsOutputTypeDef",
     {
         "LogTypesToEnable": NotRequired[List[str]],
         "LogTypesToDisable": NotRequired[List[str]],
     },
 )
 AwsRdsPendingCloudWatchLogsExportsTypeDef = TypedDict(
     "AwsRdsPendingCloudWatchLogsExportsTypeDef",
@@ -3602,16 +4102,31 @@
 )
 AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef",
     {
         "Name": NotRequired[str],
     },
 )
-AwsRdsEventSubscriptionDetailsPaginatorTypeDef = TypedDict(
-    "AwsRdsEventSubscriptionDetailsPaginatorTypeDef",
+AwsRdsEventSubscriptionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRdsEventSubscriptionDetailsExtraOutputTypeDef",
+    {
+        "CustSubscriptionId": NotRequired[str],
+        "CustomerAwsId": NotRequired[str],
+        "Enabled": NotRequired[bool],
+        "EventCategoriesList": NotRequired[List[str]],
+        "EventSubscriptionArn": NotRequired[str],
+        "SnsTopicArn": NotRequired[str],
+        "SourceIdsList": NotRequired[List[str]],
+        "SourceType": NotRequired[str],
+        "Status": NotRequired[str],
+        "SubscriptionCreationTime": NotRequired[str],
+    },
+)
+AwsRdsEventSubscriptionDetailsOutputTypeDef = TypedDict(
+    "AwsRdsEventSubscriptionDetailsOutputTypeDef",
     {
         "CustSubscriptionId": NotRequired[str],
         "CustomerAwsId": NotRequired[str],
         "Enabled": NotRequired[bool],
         "EventCategoriesList": NotRequired[List[str]],
         "EventSubscriptionArn": NotRequired[str],
         "SnsTopicArn": NotRequired[str],
@@ -3909,41 +4424,16 @@
 )
 AwsSecretsManagerSecretRotationRulesTypeDef = TypedDict(
     "AwsSecretsManagerSecretRotationRulesTypeDef",
     {
         "AutomaticallyAfterDays": NotRequired[int],
     },
 )
-BooleanFilterTypeDef = TypedDict(
-    "BooleanFilterTypeDef",
-    {
-        "Value": NotRequired[bool],
-    },
-)
-IpFilterTypeDef = TypedDict(
-    "IpFilterTypeDef",
-    {
-        "Cidr": NotRequired[str],
-    },
-)
-KeywordFilterTypeDef = TypedDict(
-    "KeywordFilterTypeDef",
-    {
-        "Value": NotRequired[str],
-    },
-)
-AwsSecurityFindingIdentifierTypeDef = TypedDict(
-    "AwsSecurityFindingIdentifierTypeDef",
-    {
-        "Id": str,
-        "ProductArn": str,
-    },
-)
-GeneratorDetailsPaginatorTypeDef = TypedDict(
-    "GeneratorDetailsPaginatorTypeDef",
+GeneratorDetailsExtraOutputTypeDef = TypedDict(
+    "GeneratorDetailsExtraOutputTypeDef",
     {
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "Labels": NotRequired[List[str]],
     },
 )
 MalwareTypeDef = TypedDict(
@@ -4012,14 +4502,47 @@
 )
 WorkflowTypeDef = TypedDict(
     "WorkflowTypeDef",
     {
         "Status": NotRequired[WorkflowStatusType],
     },
 )
+BooleanFilterTypeDef = TypedDict(
+    "BooleanFilterTypeDef",
+    {
+        "Value": NotRequired[bool],
+    },
+)
+IpFilterTypeDef = TypedDict(
+    "IpFilterTypeDef",
+    {
+        "Cidr": NotRequired[str],
+    },
+)
+KeywordFilterTypeDef = TypedDict(
+    "KeywordFilterTypeDef",
+    {
+        "Value": NotRequired[str],
+    },
+)
+AwsSecurityFindingIdentifierTypeDef = TypedDict(
+    "AwsSecurityFindingIdentifierTypeDef",
+    {
+        "Id": str,
+        "ProductArn": str,
+    },
+)
+GeneratorDetailsOutputTypeDef = TypedDict(
+    "GeneratorDetailsOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "Description": NotRequired[str],
+        "Labels": NotRequired[List[str]],
+    },
+)
 GeneratorDetailsTypeDef = TypedDict(
     "GeneratorDetailsTypeDef",
     {
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "Labels": NotRequired[Sequence[str]],
     },
@@ -4313,28 +4836,35 @@
     {
         "EndLine": NotRequired[int],
         "FileName": NotRequired[str],
         "FilePath": NotRequired[str],
         "StartLine": NotRequired[int],
     },
 )
-SecurityControlParameterPaginatorTypeDef = TypedDict(
-    "SecurityControlParameterPaginatorTypeDef",
+SecurityControlParameterExtraOutputTypeDef = TypedDict(
+    "SecurityControlParameterExtraOutputTypeDef",
     {
         "Name": NotRequired[str],
         "Value": NotRequired[List[str]],
     },
 )
 StatusReasonTypeDef = TypedDict(
     "StatusReasonTypeDef",
     {
         "ReasonCode": str,
         "Description": NotRequired[str],
     },
 )
+SecurityControlParameterOutputTypeDef = TypedDict(
+    "SecurityControlParameterOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "Value": NotRequired[List[str]],
+    },
+)
 SecurityControlParameterTypeDef = TypedDict(
     "SecurityControlParameterTypeDef",
     {
         "Name": NotRequired[str],
         "Value": NotRequired[Sequence[str]],
     },
 )
@@ -4854,36 +5384,57 @@
 RecordTypeDef = TypedDict(
     "RecordTypeDef",
     {
         "JsonPath": NotRequired[str],
         "RecordIndex": NotRequired[int],
     },
 )
-ParameterValueTypeDef = TypedDict(
-    "ParameterValueTypeDef",
+ParameterValueOutputTypeDef = TypedDict(
+    "ParameterValueOutputTypeDef",
     {
         "Integer": NotRequired[int],
         "IntegerList": NotRequired[List[int]],
         "Double": NotRequired[float],
         "String": NotRequired[str],
         "StringList": NotRequired[List[str]],
         "Boolean": NotRequired[bool],
         "Enum": NotRequired[str],
         "EnumList": NotRequired[List[str]],
     },
 )
+ParameterValueTypeDef = TypedDict(
+    "ParameterValueTypeDef",
+    {
+        "Integer": NotRequired[int],
+        "IntegerList": NotRequired[Sequence[int]],
+        "Double": NotRequired[float],
+        "String": NotRequired[str],
+        "StringList": NotRequired[Sequence[str]],
+        "Boolean": NotRequired[bool],
+        "Enum": NotRequired[str],
+        "EnumList": NotRequired[Sequence[str]],
+    },
+)
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Text": NotRequired[str],
         "Url": NotRequired[str],
     },
 )
-RuleGroupSourceListDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceListDetailsPaginatorTypeDef",
+RuleGroupSourceListDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceListDetailsExtraOutputTypeDef",
+    {
+        "GeneratedRulesType": NotRequired[str],
+        "TargetTypes": NotRequired[List[str]],
+        "Targets": NotRequired[List[str]],
+    },
+)
+RuleGroupSourceListDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceListDetailsOutputTypeDef",
     {
         "GeneratedRulesType": NotRequired[str],
         "TargetTypes": NotRequired[List[str]],
         "Targets": NotRequired[List[str]],
     },
 )
 RuleGroupSourceListDetailsTypeDef = TypedDict(
@@ -4901,16 +5452,23 @@
         "DestinationPort": NotRequired[str],
         "Direction": NotRequired[str],
         "Protocol": NotRequired[str],
         "Source": NotRequired[str],
         "SourcePort": NotRequired[str],
     },
 )
-RuleGroupSourceStatefulRulesOptionsDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceStatefulRulesOptionsDetailsPaginatorTypeDef",
+RuleGroupSourceStatefulRulesOptionsDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatefulRulesOptionsDetailsExtraOutputTypeDef",
+    {
+        "Keyword": NotRequired[str],
+        "Settings": NotRequired[List[str]],
+    },
+)
+RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef",
     {
         "Keyword": NotRequired[str],
         "Settings": NotRequired[List[str]],
     },
 )
 RuleGroupSourceStatefulRulesOptionsDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesOptionsDetailsTypeDef",
@@ -4941,42 +5499,61 @@
 )
 RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
     {
         "AddressDefinition": NotRequired[str],
     },
 )
-RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsPaginatorTypeDef",
+RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsExtraOutputTypeDef",
+    {
+        "Flags": NotRequired[List[str]],
+        "Masks": NotRequired[List[str]],
+    },
+)
+RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef",
     {
         "Flags": NotRequired[List[str]],
         "Masks": NotRequired[List[str]],
     },
 )
 RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
     {
         "Flags": NotRequired[Sequence[str]],
         "Masks": NotRequired[Sequence[str]],
     },
 )
-RuleGroupVariablesIpSetsDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupVariablesIpSetsDetailsPaginatorTypeDef",
+RuleGroupVariablesIpSetsDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupVariablesIpSetsDetailsExtraOutputTypeDef",
+    {
+        "Definition": NotRequired[List[str]],
+    },
+)
+RuleGroupVariablesPortSetsDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupVariablesPortSetsDetailsExtraOutputTypeDef",
+    {
+        "Definition": NotRequired[List[str]],
+    },
+)
+RuleGroupVariablesIpSetsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupVariablesIpSetsDetailsOutputTypeDef",
     {
         "Definition": NotRequired[List[str]],
     },
 )
 RuleGroupVariablesIpSetsDetailsTypeDef = TypedDict(
     "RuleGroupVariablesIpSetsDetailsTypeDef",
     {
         "Definition": NotRequired[Sequence[str]],
     },
 )
-RuleGroupVariablesPortSetsDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupVariablesPortSetsDetailsPaginatorTypeDef",
+RuleGroupVariablesPortSetsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupVariablesPortSetsDetailsOutputTypeDef",
     {
         "Definition": NotRequired[List[str]],
     },
 )
 RuleGroupVariablesPortSetsDetailsTypeDef = TypedDict(
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     {
@@ -5085,16 +5662,26 @@
         "IpAddressV4": NotRequired[str],
         "Organization": NotRequired[IpOrganizationDetailsTypeDef],
         "Country": NotRequired[CountryTypeDef],
         "City": NotRequired[CityTypeDef],
         "GeoLocation": NotRequired[GeoLocationTypeDef],
     },
 )
-CvssPaginatorTypeDef = TypedDict(
-    "CvssPaginatorTypeDef",
+CvssExtraOutputTypeDef = TypedDict(
+    "CvssExtraOutputTypeDef",
+    {
+        "Version": NotRequired[str],
+        "BaseScore": NotRequired[float],
+        "BaseVector": NotRequired[str],
+        "Source": NotRequired[str],
+        "Adjustments": NotRequired[List[AdjustmentTypeDef]],
+    },
+)
+CvssOutputTypeDef = TypedDict(
+    "CvssOutputTypeDef",
     {
         "Version": NotRequired[str],
         "BaseScore": NotRequired[float],
         "BaseVector": NotRequired[str],
         "Source": NotRequired[str],
         "Adjustments": NotRequired[List[AdjustmentTypeDef]],
     },
@@ -5124,50 +5711,78 @@
         "GatewayId": NotRequired[str],
         "Main": NotRequired[bool],
         "RouteTableAssociationId": NotRequired[str],
         "RouteTableId": NotRequired[str],
         "SubnetId": NotRequired[str],
     },
 )
-AutomationRulesFindingFieldsUpdateTypeDef = TypedDict(
-    "AutomationRulesFindingFieldsUpdateTypeDef",
+AutomationRulesFindingFieldsUpdateOutputTypeDef = TypedDict(
+    "AutomationRulesFindingFieldsUpdateOutputTypeDef",
     {
         "Note": NotRequired[NoteUpdateTypeDef],
         "Severity": NotRequired[SeverityUpdateTypeDef],
         "VerificationState": NotRequired[VerificationStateType],
         "Confidence": NotRequired[int],
         "Criticality": NotRequired[int],
         "Types": NotRequired[List[str]],
         "UserDefinedFields": NotRequired[Dict[str, str]],
         "Workflow": NotRequired[WorkflowUpdateTypeDef],
         "RelatedFindings": NotRequired[List[RelatedFindingTypeDef]],
     },
 )
+AutomationRulesFindingFieldsUpdateTypeDef = TypedDict(
+    "AutomationRulesFindingFieldsUpdateTypeDef",
+    {
+        "Note": NotRequired[NoteUpdateTypeDef],
+        "Severity": NotRequired[SeverityUpdateTypeDef],
+        "VerificationState": NotRequired[VerificationStateType],
+        "Confidence": NotRequired[int],
+        "Criticality": NotRequired[int],
+        "Types": NotRequired[Sequence[str]],
+        "UserDefinedFields": NotRequired[Mapping[str, str]],
+        "Workflow": NotRequired[WorkflowUpdateTypeDef],
+        "RelatedFindings": NotRequired[Sequence[RelatedFindingTypeDef]],
+    },
+)
 AwsAmazonMqBrokerLogsDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsDetailsTypeDef",
     {
         "Audit": NotRequired[bool],
         "General": NotRequired[bool],
         "AuditLogGroup": NotRequired[str],
         "GeneralLogGroup": NotRequired[str],
         "Pending": NotRequired[AwsAmazonMqBrokerLogsPendingDetailsTypeDef],
     },
 )
-AwsApiGatewayRestApiDetailsPaginatorTypeDef = TypedDict(
-    "AwsApiGatewayRestApiDetailsPaginatorTypeDef",
+AwsApiGatewayRestApiDetailsExtraOutputTypeDef = TypedDict(
+    "AwsApiGatewayRestApiDetailsExtraOutputTypeDef",
     {
         "Id": NotRequired[str],
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "CreatedDate": NotRequired[str],
         "Version": NotRequired[str],
         "BinaryMediaTypes": NotRequired[List[str]],
         "MinimumCompressionSize": NotRequired[int],
         "ApiKeySource": NotRequired[str],
-        "EndpointConfiguration": NotRequired[AwsApiGatewayEndpointConfigurationPaginatorTypeDef],
+        "EndpointConfiguration": NotRequired[AwsApiGatewayEndpointConfigurationExtraOutputTypeDef],
+    },
+)
+AwsApiGatewayRestApiDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayRestApiDetailsOutputTypeDef",
+    {
+        "Id": NotRequired[str],
+        "Name": NotRequired[str],
+        "Description": NotRequired[str],
+        "CreatedDate": NotRequired[str],
+        "Version": NotRequired[str],
+        "BinaryMediaTypes": NotRequired[List[str]],
+        "MinimumCompressionSize": NotRequired[int],
+        "ApiKeySource": NotRequired[str],
+        "EndpointConfiguration": NotRequired[AwsApiGatewayEndpointConfigurationOutputTypeDef],
     },
 )
 AwsApiGatewayRestApiDetailsTypeDef = TypedDict(
     "AwsApiGatewayRestApiDetailsTypeDef",
     {
         "Id": NotRequired[str],
         "Name": NotRequired[str],
@@ -5176,29 +5791,50 @@
         "Version": NotRequired[str],
         "BinaryMediaTypes": NotRequired[Sequence[str]],
         "MinimumCompressionSize": NotRequired[int],
         "ApiKeySource": NotRequired[str],
         "EndpointConfiguration": NotRequired[AwsApiGatewayEndpointConfigurationTypeDef],
     },
 )
-AwsApiGatewayStageDetailsPaginatorTypeDef = TypedDict(
-    "AwsApiGatewayStageDetailsPaginatorTypeDef",
+AwsApiGatewayStageDetailsExtraOutputTypeDef = TypedDict(
+    "AwsApiGatewayStageDetailsExtraOutputTypeDef",
+    {
+        "DeploymentId": NotRequired[str],
+        "ClientCertificateId": NotRequired[str],
+        "StageName": NotRequired[str],
+        "Description": NotRequired[str],
+        "CacheClusterEnabled": NotRequired[bool],
+        "CacheClusterSize": NotRequired[str],
+        "CacheClusterStatus": NotRequired[str],
+        "MethodSettings": NotRequired[List[AwsApiGatewayMethodSettingsTypeDef]],
+        "Variables": NotRequired[Dict[str, str]],
+        "DocumentationVersion": NotRequired[str],
+        "AccessLogSettings": NotRequired[AwsApiGatewayAccessLogSettingsTypeDef],
+        "CanarySettings": NotRequired[AwsApiGatewayCanarySettingsExtraOutputTypeDef],
+        "TracingEnabled": NotRequired[bool],
+        "CreatedDate": NotRequired[str],
+        "LastUpdatedDate": NotRequired[str],
+        "WebAclArn": NotRequired[str],
+    },
+)
+AwsApiGatewayStageDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayStageDetailsOutputTypeDef",
     {
         "DeploymentId": NotRequired[str],
         "ClientCertificateId": NotRequired[str],
         "StageName": NotRequired[str],
         "Description": NotRequired[str],
         "CacheClusterEnabled": NotRequired[bool],
         "CacheClusterSize": NotRequired[str],
         "CacheClusterStatus": NotRequired[str],
         "MethodSettings": NotRequired[List[AwsApiGatewayMethodSettingsTypeDef]],
         "Variables": NotRequired[Dict[str, str]],
         "DocumentationVersion": NotRequired[str],
         "AccessLogSettings": NotRequired[AwsApiGatewayAccessLogSettingsTypeDef],
-        "CanarySettings": NotRequired[AwsApiGatewayCanarySettingsPaginatorTypeDef],
+        "CanarySettings": NotRequired[AwsApiGatewayCanarySettingsOutputTypeDef],
         "TracingEnabled": NotRequired[bool],
         "CreatedDate": NotRequired[str],
         "LastUpdatedDate": NotRequired[str],
         "WebAclArn": NotRequired[str],
     },
 )
 AwsApiGatewayStageDetailsTypeDef = TypedDict(
@@ -5218,27 +5854,42 @@
         "CanarySettings": NotRequired[AwsApiGatewayCanarySettingsTypeDef],
         "TracingEnabled": NotRequired[bool],
         "CreatedDate": NotRequired[str],
         "LastUpdatedDate": NotRequired[str],
         "WebAclArn": NotRequired[str],
     },
 )
-AwsApiGatewayV2ApiDetailsPaginatorTypeDef = TypedDict(
-    "AwsApiGatewayV2ApiDetailsPaginatorTypeDef",
+AwsApiGatewayV2ApiDetailsExtraOutputTypeDef = TypedDict(
+    "AwsApiGatewayV2ApiDetailsExtraOutputTypeDef",
+    {
+        "ApiEndpoint": NotRequired[str],
+        "ApiId": NotRequired[str],
+        "ApiKeySelectionExpression": NotRequired[str],
+        "CreatedDate": NotRequired[str],
+        "Description": NotRequired[str],
+        "Version": NotRequired[str],
+        "Name": NotRequired[str],
+        "ProtocolType": NotRequired[str],
+        "RouteSelectionExpression": NotRequired[str],
+        "CorsConfiguration": NotRequired[AwsCorsConfigurationExtraOutputTypeDef],
+    },
+)
+AwsApiGatewayV2ApiDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayV2ApiDetailsOutputTypeDef",
     {
         "ApiEndpoint": NotRequired[str],
         "ApiId": NotRequired[str],
         "ApiKeySelectionExpression": NotRequired[str],
         "CreatedDate": NotRequired[str],
         "Description": NotRequired[str],
         "Version": NotRequired[str],
         "Name": NotRequired[str],
         "ProtocolType": NotRequired[str],
         "RouteSelectionExpression": NotRequired[str],
-        "CorsConfiguration": NotRequired[AwsCorsConfigurationPaginatorTypeDef],
+        "CorsConfiguration": NotRequired[AwsCorsConfigurationOutputTypeDef],
     },
 )
 AwsApiGatewayV2ApiDetailsTypeDef = TypedDict(
     "AwsApiGatewayV2ApiDetailsTypeDef",
     {
         "ApiEndpoint": NotRequired[str],
         "ApiId": NotRequired[str],
@@ -5248,16 +5899,34 @@
         "Version": NotRequired[str],
         "Name": NotRequired[str],
         "ProtocolType": NotRequired[str],
         "RouteSelectionExpression": NotRequired[str],
         "CorsConfiguration": NotRequired[AwsCorsConfigurationTypeDef],
     },
 )
-AwsApiGatewayV2StageDetailsPaginatorTypeDef = TypedDict(
-    "AwsApiGatewayV2StageDetailsPaginatorTypeDef",
+AwsApiGatewayV2StageDetailsExtraOutputTypeDef = TypedDict(
+    "AwsApiGatewayV2StageDetailsExtraOutputTypeDef",
+    {
+        "ClientCertificateId": NotRequired[str],
+        "CreatedDate": NotRequired[str],
+        "Description": NotRequired[str],
+        "DefaultRouteSettings": NotRequired[AwsApiGatewayV2RouteSettingsTypeDef],
+        "DeploymentId": NotRequired[str],
+        "LastUpdatedDate": NotRequired[str],
+        "RouteSettings": NotRequired[AwsApiGatewayV2RouteSettingsTypeDef],
+        "StageName": NotRequired[str],
+        "StageVariables": NotRequired[Dict[str, str]],
+        "AccessLogSettings": NotRequired[AwsApiGatewayAccessLogSettingsTypeDef],
+        "AutoDeploy": NotRequired[bool],
+        "LastDeploymentStatusMessage": NotRequired[str],
+        "ApiGatewayManaged": NotRequired[bool],
+    },
+)
+AwsApiGatewayV2StageDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayV2StageDetailsOutputTypeDef",
     {
         "ClientCertificateId": NotRequired[str],
         "CreatedDate": NotRequired[str],
         "Description": NotRequired[str],
         "DefaultRouteSettings": NotRequired[AwsApiGatewayV2RouteSettingsTypeDef],
         "DeploymentId": NotRequired[str],
         "LastUpdatedDate": NotRequired[str],
@@ -5303,16 +5972,29 @@
     "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef",
     {
         "EncryptionConfiguration": NotRequired[
             AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef
         ],
     },
 )
-AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsPaginatorTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsPaginatorTypeDef",
+AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsExtraOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsExtraOutputTypeDef",
+    {
+        "LaunchTemplateSpecification": NotRequired[
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef
+        ],
+        "Overrides": NotRequired[
+            List[
+                AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef
+            ]
+        ],
+    },
+)
+AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef",
     {
         "LaunchTemplateSpecification": NotRequired[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef
         ],
         "Overrides": NotRequired[
             List[
                 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef
@@ -5345,21 +6027,31 @@
 AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef",
     {
         "DestinationBackupVaultArn": NotRequired[str],
         "Lifecycle": NotRequired[AwsBackupBackupPlanLifecycleDetailsTypeDef],
     },
 )
-AwsBackupBackupVaultDetailsPaginatorTypeDef = TypedDict(
-    "AwsBackupBackupVaultDetailsPaginatorTypeDef",
+AwsBackupBackupVaultDetailsExtraOutputTypeDef = TypedDict(
+    "AwsBackupBackupVaultDetailsExtraOutputTypeDef",
     {
         "BackupVaultArn": NotRequired[str],
         "BackupVaultName": NotRequired[str],
         "EncryptionKeyArn": NotRequired[str],
-        "Notifications": NotRequired[AwsBackupBackupVaultNotificationsDetailsPaginatorTypeDef],
+        "Notifications": NotRequired[AwsBackupBackupVaultNotificationsDetailsExtraOutputTypeDef],
+        "AccessPolicy": NotRequired[str],
+    },
+)
+AwsBackupBackupVaultDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupVaultDetailsOutputTypeDef",
+    {
+        "BackupVaultArn": NotRequired[str],
+        "BackupVaultName": NotRequired[str],
+        "EncryptionKeyArn": NotRequired[str],
+        "Notifications": NotRequired[AwsBackupBackupVaultNotificationsDetailsOutputTypeDef],
         "AccessPolicy": NotRequired[str],
     },
 )
 AwsBackupBackupVaultDetailsTypeDef = TypedDict(
     "AwsBackupBackupVaultDetailsTypeDef",
     {
         "BackupVaultArn": NotRequired[str],
@@ -5389,16 +6081,27 @@
         "ResourceType": NotRequired[str],
         "SourceBackupVaultArn": NotRequired[str],
         "Status": NotRequired[str],
         "StatusMessage": NotRequired[str],
         "StorageClass": NotRequired[str],
     },
 )
-AwsCertificateManagerCertificateDomainValidationOptionPaginatorTypeDef = TypedDict(
-    "AwsCertificateManagerCertificateDomainValidationOptionPaginatorTypeDef",
+AwsCertificateManagerCertificateDomainValidationOptionExtraOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateDomainValidationOptionExtraOutputTypeDef",
+    {
+        "DomainName": NotRequired[str],
+        "ResourceRecord": NotRequired[AwsCertificateManagerCertificateResourceRecordTypeDef],
+        "ValidationDomain": NotRequired[str],
+        "ValidationEmails": NotRequired[List[str]],
+        "ValidationMethod": NotRequired[str],
+        "ValidationStatus": NotRequired[str],
+    },
+)
+AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef",
     {
         "DomainName": NotRequired[str],
         "ResourceRecord": NotRequired[AwsCertificateManagerCertificateResourceRecordTypeDef],
         "ValidationDomain": NotRequired[str],
         "ValidationEmails": NotRequired[List[str]],
         "ValidationMethod": NotRequired[str],
         "ValidationStatus": NotRequired[str],
@@ -5411,16 +6114,36 @@
         "ResourceRecord": NotRequired[AwsCertificateManagerCertificateResourceRecordTypeDef],
         "ValidationDomain": NotRequired[str],
         "ValidationEmails": NotRequired[Sequence[str]],
         "ValidationMethod": NotRequired[str],
         "ValidationStatus": NotRequired[str],
     },
 )
-AwsCloudFormationStackDetailsPaginatorTypeDef = TypedDict(
-    "AwsCloudFormationStackDetailsPaginatorTypeDef",
+AwsCloudFormationStackDetailsExtraOutputTypeDef = TypedDict(
+    "AwsCloudFormationStackDetailsExtraOutputTypeDef",
+    {
+        "Capabilities": NotRequired[List[str]],
+        "CreationTime": NotRequired[str],
+        "Description": NotRequired[str],
+        "DisableRollback": NotRequired[bool],
+        "DriftInformation": NotRequired[AwsCloudFormationStackDriftInformationDetailsTypeDef],
+        "EnableTerminationProtection": NotRequired[bool],
+        "LastUpdatedTime": NotRequired[str],
+        "NotificationArns": NotRequired[List[str]],
+        "Outputs": NotRequired[List[AwsCloudFormationStackOutputsDetailsTypeDef]],
+        "RoleArn": NotRequired[str],
+        "StackId": NotRequired[str],
+        "StackName": NotRequired[str],
+        "StackStatus": NotRequired[str],
+        "StackStatusReason": NotRequired[str],
+        "TimeoutInMinutes": NotRequired[int],
+    },
+)
+AwsCloudFormationStackDetailsOutputTypeDef = TypedDict(
+    "AwsCloudFormationStackDetailsOutputTypeDef",
     {
         "Capabilities": NotRequired[List[str]],
         "CreationTime": NotRequired[str],
         "Description": NotRequired[str],
         "DisableRollback": NotRequired[bool],
         "DriftInformation": NotRequired[AwsCloudFormationStackDriftInformationDetailsTypeDef],
         "EnableTerminationProtection": NotRequired[bool],
@@ -5451,66 +6174,118 @@
         "StackId": NotRequired[str],
         "StackName": NotRequired[str],
         "StackStatus": NotRequired[str],
         "StackStatusReason": NotRequired[str],
         "TimeoutInMinutes": NotRequired[int],
     },
 )
-AwsCloudFrontDistributionCacheBehaviorsPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionCacheBehaviorsPaginatorTypeDef",
+AwsCloudFrontDistributionCacheBehaviorsExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionCacheBehaviorsExtraOutputTypeDef",
+    {
+        "Items": NotRequired[List[AwsCloudFrontDistributionCacheBehaviorTypeDef]],
+    },
+)
+AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef",
     {
         "Items": NotRequired[List[AwsCloudFrontDistributionCacheBehaviorTypeDef]],
     },
 )
 AwsCloudFrontDistributionCacheBehaviorsTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorsTypeDef",
     {
         "Items": NotRequired[Sequence[AwsCloudFrontDistributionCacheBehaviorTypeDef]],
     },
 )
-AwsCloudFrontDistributionOriginCustomOriginConfigPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginCustomOriginConfigPaginatorTypeDef",
+AwsCloudFrontDistributionOriginCustomOriginConfigExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginCustomOriginConfigExtraOutputTypeDef",
     {
         "HttpPort": NotRequired[int],
         "HttpsPort": NotRequired[int],
         "OriginKeepaliveTimeout": NotRequired[int],
         "OriginProtocolPolicy": NotRequired[str],
         "OriginReadTimeout": NotRequired[int],
         "OriginSslProtocols": NotRequired[
-            AwsCloudFrontDistributionOriginSslProtocolsPaginatorTypeDef
+            AwsCloudFrontDistributionOriginSslProtocolsExtraOutputTypeDef
         ],
     },
 )
+AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef",
+    {
+        "HttpPort": NotRequired[int],
+        "HttpsPort": NotRequired[int],
+        "OriginKeepaliveTimeout": NotRequired[int],
+        "OriginProtocolPolicy": NotRequired[str],
+        "OriginReadTimeout": NotRequired[int],
+        "OriginSslProtocols": NotRequired[AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef],
+    },
+)
 AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef",
     {
         "HttpPort": NotRequired[int],
         "HttpsPort": NotRequired[int],
         "OriginKeepaliveTimeout": NotRequired[int],
         "OriginProtocolPolicy": NotRequired[str],
         "OriginReadTimeout": NotRequired[int],
         "OriginSslProtocols": NotRequired[AwsCloudFrontDistributionOriginSslProtocolsTypeDef],
     },
 )
-AwsCloudFrontDistributionOriginGroupFailoverPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginGroupFailoverPaginatorTypeDef",
+AwsCloudFrontDistributionOriginGroupFailoverExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupFailoverExtraOutputTypeDef",
+    {
+        "StatusCodes": NotRequired[
+            AwsCloudFrontDistributionOriginGroupFailoverStatusCodesExtraOutputTypeDef
+        ],
+    },
+)
+AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef",
     {
         "StatusCodes": NotRequired[
-            AwsCloudFrontDistributionOriginGroupFailoverStatusCodesPaginatorTypeDef
+            AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef
         ],
     },
 )
 AwsCloudFrontDistributionOriginGroupFailoverTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverTypeDef",
     {
         "StatusCodes": NotRequired[AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef],
     },
 )
-AwsCloudWatchAlarmDetailsPaginatorTypeDef = TypedDict(
-    "AwsCloudWatchAlarmDetailsPaginatorTypeDef",
+AwsCloudWatchAlarmDetailsExtraOutputTypeDef = TypedDict(
+    "AwsCloudWatchAlarmDetailsExtraOutputTypeDef",
+    {
+        "ActionsEnabled": NotRequired[bool],
+        "AlarmActions": NotRequired[List[str]],
+        "AlarmArn": NotRequired[str],
+        "AlarmConfigurationUpdatedTimestamp": NotRequired[str],
+        "AlarmDescription": NotRequired[str],
+        "AlarmName": NotRequired[str],
+        "ComparisonOperator": NotRequired[str],
+        "DatapointsToAlarm": NotRequired[int],
+        "Dimensions": NotRequired[List[AwsCloudWatchAlarmDimensionsDetailsTypeDef]],
+        "EvaluateLowSampleCountPercentile": NotRequired[str],
+        "EvaluationPeriods": NotRequired[int],
+        "ExtendedStatistic": NotRequired[str],
+        "InsufficientDataActions": NotRequired[List[str]],
+        "MetricName": NotRequired[str],
+        "Namespace": NotRequired[str],
+        "OkActions": NotRequired[List[str]],
+        "Period": NotRequired[int],
+        "Statistic": NotRequired[str],
+        "Threshold": NotRequired[float],
+        "ThresholdMetricId": NotRequired[str],
+        "TreatMissingData": NotRequired[str],
+        "Unit": NotRequired[str],
+    },
+)
+AwsCloudWatchAlarmDetailsOutputTypeDef = TypedDict(
+    "AwsCloudWatchAlarmDetailsOutputTypeDef",
     {
         "ActionsEnabled": NotRequired[bool],
         "AlarmActions": NotRequired[List[str]],
         "AlarmArn": NotRequired[str],
         "AlarmConfigurationUpdatedTimestamp": NotRequired[str],
         "AlarmDescription": NotRequired[str],
         "AlarmName": NotRequired[str],
@@ -5555,16 +6330,29 @@
         "Statistic": NotRequired[str],
         "Threshold": NotRequired[float],
         "ThresholdMetricId": NotRequired[str],
         "TreatMissingData": NotRequired[str],
         "Unit": NotRequired[str],
     },
 )
-AwsCodeBuildProjectEnvironmentPaginatorTypeDef = TypedDict(
-    "AwsCodeBuildProjectEnvironmentPaginatorTypeDef",
+AwsCodeBuildProjectEnvironmentExtraOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectEnvironmentExtraOutputTypeDef",
+    {
+        "Certificate": NotRequired[str],
+        "EnvironmentVariables": NotRequired[
+            List[AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef]
+        ],
+        "PrivilegedMode": NotRequired[bool],
+        "ImagePullCredentialsType": NotRequired[str],
+        "RegistryCredential": NotRequired[AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef],
+        "Type": NotRequired[str],
+    },
+)
+AwsCodeBuildProjectEnvironmentOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectEnvironmentOutputTypeDef",
     {
         "Certificate": NotRequired[str],
         "EnvironmentVariables": NotRequired[
             List[AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef]
         ],
         "PrivilegedMode": NotRequired[bool],
         "ImagePullCredentialsType": NotRequired[str],
@@ -5588,16 +6376,37 @@
 AwsCodeBuildProjectLogsConfigDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
     {
         "CloudWatchLogs": NotRequired[AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef],
         "S3Logs": NotRequired[AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef],
     },
 )
-AwsDmsReplicationInstanceDetailsPaginatorTypeDef = TypedDict(
-    "AwsDmsReplicationInstanceDetailsPaginatorTypeDef",
+AwsDmsReplicationInstanceDetailsExtraOutputTypeDef = TypedDict(
+    "AwsDmsReplicationInstanceDetailsExtraOutputTypeDef",
+    {
+        "AllocatedStorage": NotRequired[int],
+        "AutoMinorVersionUpgrade": NotRequired[bool],
+        "AvailabilityZone": NotRequired[str],
+        "EngineVersion": NotRequired[str],
+        "KmsKeyId": NotRequired[str],
+        "MultiAZ": NotRequired[bool],
+        "PreferredMaintenanceWindow": NotRequired[str],
+        "PubliclyAccessible": NotRequired[bool],
+        "ReplicationInstanceClass": NotRequired[str],
+        "ReplicationInstanceIdentifier": NotRequired[str],
+        "ReplicationSubnetGroup": NotRequired[
+            AwsDmsReplicationInstanceReplicationSubnetGroupDetailsTypeDef
+        ],
+        "VpcSecurityGroups": NotRequired[
+            List[AwsDmsReplicationInstanceVpcSecurityGroupsDetailsTypeDef]
+        ],
+    },
+)
+AwsDmsReplicationInstanceDetailsOutputTypeDef = TypedDict(
+    "AwsDmsReplicationInstanceDetailsOutputTypeDef",
     {
         "AllocatedStorage": NotRequired[int],
         "AutoMinorVersionUpgrade": NotRequired[bool],
         "AvailabilityZone": NotRequired[str],
         "EngineVersion": NotRequired[str],
         "KmsKeyId": NotRequired[str],
         "MultiAZ": NotRequired[bool],
@@ -5630,35 +6439,58 @@
             AwsDmsReplicationInstanceReplicationSubnetGroupDetailsTypeDef
         ],
         "VpcSecurityGroups": NotRequired[
             Sequence[AwsDmsReplicationInstanceVpcSecurityGroupsDetailsTypeDef]
         ],
     },
 )
-AwsDynamoDbTableGlobalSecondaryIndexPaginatorTypeDef = TypedDict(
-    "AwsDynamoDbTableGlobalSecondaryIndexPaginatorTypeDef",
+AwsDynamoDbTableGlobalSecondaryIndexExtraOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableGlobalSecondaryIndexExtraOutputTypeDef",
+    {
+        "Backfilling": NotRequired[bool],
+        "IndexArn": NotRequired[str],
+        "IndexName": NotRequired[str],
+        "IndexSizeBytes": NotRequired[int],
+        "IndexStatus": NotRequired[str],
+        "ItemCount": NotRequired[int],
+        "KeySchema": NotRequired[List[AwsDynamoDbTableKeySchemaTypeDef]],
+        "Projection": NotRequired[AwsDynamoDbTableProjectionExtraOutputTypeDef],
+        "ProvisionedThroughput": NotRequired[AwsDynamoDbTableProvisionedThroughputTypeDef],
+    },
+)
+AwsDynamoDbTableLocalSecondaryIndexExtraOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableLocalSecondaryIndexExtraOutputTypeDef",
+    {
+        "IndexArn": NotRequired[str],
+        "IndexName": NotRequired[str],
+        "KeySchema": NotRequired[List[AwsDynamoDbTableKeySchemaTypeDef]],
+        "Projection": NotRequired[AwsDynamoDbTableProjectionExtraOutputTypeDef],
+    },
+)
+AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef",
     {
         "Backfilling": NotRequired[bool],
         "IndexArn": NotRequired[str],
         "IndexName": NotRequired[str],
         "IndexSizeBytes": NotRequired[int],
         "IndexStatus": NotRequired[str],
         "ItemCount": NotRequired[int],
         "KeySchema": NotRequired[List[AwsDynamoDbTableKeySchemaTypeDef]],
-        "Projection": NotRequired[AwsDynamoDbTableProjectionPaginatorTypeDef],
+        "Projection": NotRequired[AwsDynamoDbTableProjectionOutputTypeDef],
         "ProvisionedThroughput": NotRequired[AwsDynamoDbTableProvisionedThroughputTypeDef],
     },
 )
-AwsDynamoDbTableLocalSecondaryIndexPaginatorTypeDef = TypedDict(
-    "AwsDynamoDbTableLocalSecondaryIndexPaginatorTypeDef",
+AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef",
     {
         "IndexArn": NotRequired[str],
         "IndexName": NotRequired[str],
         "KeySchema": NotRequired[List[AwsDynamoDbTableKeySchemaTypeDef]],
-        "Projection": NotRequired[AwsDynamoDbTableProjectionPaginatorTypeDef],
+        "Projection": NotRequired[AwsDynamoDbTableProjectionOutputTypeDef],
     },
 )
 AwsDynamoDbTableGlobalSecondaryIndexTypeDef = TypedDict(
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     {
         "Backfilling": NotRequired[bool],
         "IndexArn": NotRequired[str],
@@ -5708,16 +6540,34 @@
     "AwsEc2ClientVpnEndpointClientConnectOptionsDetailsTypeDef",
     {
         "Enabled": NotRequired[bool],
         "LambdaFunctionArn": NotRequired[str],
         "Status": NotRequired[AwsEc2ClientVpnEndpointClientConnectOptionsStatusDetailsTypeDef],
     },
 )
-AwsEc2InstanceDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2InstanceDetailsPaginatorTypeDef",
+AwsEc2InstanceDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2InstanceDetailsExtraOutputTypeDef",
+    {
+        "Type": NotRequired[str],
+        "ImageId": NotRequired[str],
+        "IpV4Addresses": NotRequired[List[str]],
+        "IpV6Addresses": NotRequired[List[str]],
+        "KeyName": NotRequired[str],
+        "IamInstanceProfileArn": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "SubnetId": NotRequired[str],
+        "LaunchedAt": NotRequired[str],
+        "NetworkInterfaces": NotRequired[List[AwsEc2InstanceNetworkInterfacesDetailsTypeDef]],
+        "VirtualizationType": NotRequired[str],
+        "MetadataOptions": NotRequired[AwsEc2InstanceMetadataOptionsTypeDef],
+        "Monitoring": NotRequired[AwsEc2InstanceMonitoringDetailsTypeDef],
+    },
+)
+AwsEc2InstanceDetailsOutputTypeDef = TypedDict(
+    "AwsEc2InstanceDetailsOutputTypeDef",
     {
         "Type": NotRequired[str],
         "ImageId": NotRequired[str],
         "IpV4Addresses": NotRequired[List[str]],
         "IpV6Addresses": NotRequired[List[str]],
         "KeyName": NotRequired[str],
         "IamInstanceProfileArn": NotRequired[str],
@@ -5771,16 +6621,58 @@
     {
         "MarketType": NotRequired[str],
         "SpotOptions": NotRequired[
             AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef
         ],
     },
 )
-AwsEc2LaunchTemplateDataInstanceRequirementsDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsPaginatorTypeDef",
+AwsEc2LaunchTemplateDataInstanceRequirementsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsExtraOutputTypeDef",
+    {
+        "AcceleratorCount": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
+        ],
+        "AcceleratorManufacturers": NotRequired[List[str]],
+        "AcceleratorNames": NotRequired[List[str]],
+        "AcceleratorTotalMemoryMiB": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef
+        ],
+        "AcceleratorTypes": NotRequired[List[str]],
+        "BareMetal": NotRequired[str],
+        "BaselineEbsBandwidthMbps": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef
+        ],
+        "BurstablePerformance": NotRequired[str],
+        "CpuManufacturers": NotRequired[List[str]],
+        "ExcludedInstanceTypes": NotRequired[List[str]],
+        "InstanceGenerations": NotRequired[List[str]],
+        "LocalStorage": NotRequired[str],
+        "LocalStorageTypes": NotRequired[List[str]],
+        "MemoryGiBPerVCpu": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef
+        ],
+        "MemoryMiB": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef
+        ],
+        "NetworkInterfaceCount": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef
+        ],
+        "OnDemandMaxPricePercentageOverLowestPrice": NotRequired[int],
+        "RequireHibernateSupport": NotRequired[bool],
+        "SpotMaxPricePercentageOverLowestPrice": NotRequired[int],
+        "TotalLocalStorageGB": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef
+        ],
+        "VCpuCount": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef
+        ],
+    },
+)
+AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef",
     {
         "AcceleratorCount": NotRequired[
             AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
         ],
         "AcceleratorManufacturers": NotRequired[List[str]],
         "AcceleratorNames": NotRequired[List[str]],
         "AcceleratorTotalMemoryMiB": NotRequired[
@@ -5855,16 +6747,48 @@
             AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef
         ],
         "VCpuCount": NotRequired[
             AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef
         ],
     },
 )
-AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsPaginatorTypeDef",
+AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsExtraOutputTypeDef",
+    {
+        "AssociateCarrierIpAddress": NotRequired[bool],
+        "AssociatePublicIpAddress": NotRequired[bool],
+        "DeleteOnTermination": NotRequired[bool],
+        "Description": NotRequired[str],
+        "DeviceIndex": NotRequired[int],
+        "Groups": NotRequired[List[str]],
+        "InterfaceType": NotRequired[str],
+        "Ipv4PrefixCount": NotRequired[int],
+        "Ipv4Prefixes": NotRequired[
+            List[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef]
+        ],
+        "Ipv6AddressCount": NotRequired[int],
+        "Ipv6Addresses": NotRequired[
+            List[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef]
+        ],
+        "Ipv6PrefixCount": NotRequired[int],
+        "Ipv6Prefixes": NotRequired[
+            List[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef]
+        ],
+        "NetworkCardIndex": NotRequired[int],
+        "NetworkInterfaceId": NotRequired[str],
+        "PrivateIpAddress": NotRequired[str],
+        "PrivateIpAddresses": NotRequired[
+            List[AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef]
+        ],
+        "SecondaryPrivateIpAddressCount": NotRequired[int],
+        "SubnetId": NotRequired[str],
+    },
+)
+AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef",
     {
         "AssociateCarrierIpAddress": NotRequired[bool],
         "AssociatePublicIpAddress": NotRequired[bool],
         "DeleteOnTermination": NotRequired[bool],
         "Description": NotRequired[str],
         "DeviceIndex": NotRequired[int],
         "Groups": NotRequired[List[str]],
@@ -5932,16 +6856,31 @@
         "Ipv6CidrBlock": NotRequired[str],
         "PortRange": NotRequired[PortRangeFromToTypeDef],
         "Protocol": NotRequired[str],
         "RuleAction": NotRequired[str],
         "RuleNumber": NotRequired[int],
     },
 )
-AwsEc2NetworkInterfaceDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2NetworkInterfaceDetailsPaginatorTypeDef",
+AwsEc2NetworkInterfaceDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2NetworkInterfaceDetailsExtraOutputTypeDef",
+    {
+        "Attachment": NotRequired[AwsEc2NetworkInterfaceAttachmentTypeDef],
+        "NetworkInterfaceId": NotRequired[str],
+        "SecurityGroups": NotRequired[List[AwsEc2NetworkInterfaceSecurityGroupTypeDef]],
+        "SourceDestCheck": NotRequired[bool],
+        "IpV6Addresses": NotRequired[List[AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef]],
+        "PrivateIpAddresses": NotRequired[
+            List[AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef]
+        ],
+        "PublicDnsName": NotRequired[str],
+        "PublicIp": NotRequired[str],
+    },
+)
+AwsEc2NetworkInterfaceDetailsOutputTypeDef = TypedDict(
+    "AwsEc2NetworkInterfaceDetailsOutputTypeDef",
     {
         "Attachment": NotRequired[AwsEc2NetworkInterfaceAttachmentTypeDef],
         "NetworkInterfaceId": NotRequired[str],
         "SecurityGroups": NotRequired[List[AwsEc2NetworkInterfaceSecurityGroupTypeDef]],
         "SourceDestCheck": NotRequired[bool],
         "IpV6Addresses": NotRequired[List[AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef]],
         "PrivateIpAddresses": NotRequired[
@@ -5962,16 +6901,28 @@
         "PrivateIpAddresses": NotRequired[
             Sequence[AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef]
         ],
         "PublicDnsName": NotRequired[str],
         "PublicIp": NotRequired[str],
     },
 )
-AwsEc2SecurityGroupIpPermissionPaginatorTypeDef = TypedDict(
-    "AwsEc2SecurityGroupIpPermissionPaginatorTypeDef",
+AwsEc2SecurityGroupIpPermissionExtraOutputTypeDef = TypedDict(
+    "AwsEc2SecurityGroupIpPermissionExtraOutputTypeDef",
+    {
+        "IpProtocol": NotRequired[str],
+        "FromPort": NotRequired[int],
+        "ToPort": NotRequired[int],
+        "UserIdGroupPairs": NotRequired[List[AwsEc2SecurityGroupUserIdGroupPairTypeDef]],
+        "IpRanges": NotRequired[List[AwsEc2SecurityGroupIpRangeTypeDef]],
+        "Ipv6Ranges": NotRequired[List[AwsEc2SecurityGroupIpv6RangeTypeDef]],
+        "PrefixListIds": NotRequired[List[AwsEc2SecurityGroupPrefixListIdTypeDef]],
+    },
+)
+AwsEc2SecurityGroupIpPermissionOutputTypeDef = TypedDict(
+    "AwsEc2SecurityGroupIpPermissionOutputTypeDef",
     {
         "IpProtocol": NotRequired[str],
         "FromPort": NotRequired[int],
         "ToPort": NotRequired[int],
         "UserIdGroupPairs": NotRequired[List[AwsEc2SecurityGroupUserIdGroupPairTypeDef]],
         "IpRanges": NotRequired[List[AwsEc2SecurityGroupIpRangeTypeDef]],
         "Ipv6Ranges": NotRequired[List[AwsEc2SecurityGroupIpv6RangeTypeDef]],
@@ -5986,16 +6937,34 @@
         "ToPort": NotRequired[int],
         "UserIdGroupPairs": NotRequired[Sequence[AwsEc2SecurityGroupUserIdGroupPairTypeDef]],
         "IpRanges": NotRequired[Sequence[AwsEc2SecurityGroupIpRangeTypeDef]],
         "Ipv6Ranges": NotRequired[Sequence[AwsEc2SecurityGroupIpv6RangeTypeDef]],
         "PrefixListIds": NotRequired[Sequence[AwsEc2SecurityGroupPrefixListIdTypeDef]],
     },
 )
-AwsEc2SubnetDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2SubnetDetailsPaginatorTypeDef",
+AwsEc2SubnetDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2SubnetDetailsExtraOutputTypeDef",
+    {
+        "AssignIpv6AddressOnCreation": NotRequired[bool],
+        "AvailabilityZone": NotRequired[str],
+        "AvailabilityZoneId": NotRequired[str],
+        "AvailableIpAddressCount": NotRequired[int],
+        "CidrBlock": NotRequired[str],
+        "DefaultForAz": NotRequired[bool],
+        "MapPublicIpOnLaunch": NotRequired[bool],
+        "OwnerId": NotRequired[str],
+        "State": NotRequired[str],
+        "SubnetArn": NotRequired[str],
+        "SubnetId": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "Ipv6CidrBlockAssociationSet": NotRequired[List[Ipv6CidrBlockAssociationTypeDef]],
+    },
+)
+AwsEc2SubnetDetailsOutputTypeDef = TypedDict(
+    "AwsEc2SubnetDetailsOutputTypeDef",
     {
         "AssignIpv6AddressOnCreation": NotRequired[bool],
         "AvailabilityZone": NotRequired[str],
         "AvailabilityZoneId": NotRequired[str],
         "AvailableIpAddressCount": NotRequired[int],
         "CidrBlock": NotRequired[str],
         "DefaultForAz": NotRequired[bool],
@@ -6022,16 +6991,32 @@
         "State": NotRequired[str],
         "SubnetArn": NotRequired[str],
         "SubnetId": NotRequired[str],
         "VpcId": NotRequired[str],
         "Ipv6CidrBlockAssociationSet": NotRequired[Sequence[Ipv6CidrBlockAssociationTypeDef]],
     },
 )
-AwsEc2VolumeDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VolumeDetailsPaginatorTypeDef",
+AwsEc2VolumeDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VolumeDetailsExtraOutputTypeDef",
+    {
+        "CreateTime": NotRequired[str],
+        "DeviceName": NotRequired[str],
+        "Encrypted": NotRequired[bool],
+        "Size": NotRequired[int],
+        "SnapshotId": NotRequired[str],
+        "Status": NotRequired[str],
+        "KmsKeyId": NotRequired[str],
+        "Attachments": NotRequired[List[AwsEc2VolumeAttachmentTypeDef]],
+        "VolumeId": NotRequired[str],
+        "VolumeType": NotRequired[str],
+        "VolumeScanStatus": NotRequired[str],
+    },
+)
+AwsEc2VolumeDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VolumeDetailsOutputTypeDef",
     {
         "CreateTime": NotRequired[str],
         "DeviceName": NotRequired[str],
         "Encrypted": NotRequired[bool],
         "Size": NotRequired[int],
         "SnapshotId": NotRequired[str],
         "Status": NotRequired[str],
@@ -6054,16 +7039,25 @@
         "KmsKeyId": NotRequired[str],
         "Attachments": NotRequired[Sequence[AwsEc2VolumeAttachmentTypeDef]],
         "VolumeId": NotRequired[str],
         "VolumeType": NotRequired[str],
         "VolumeScanStatus": NotRequired[str],
     },
 )
-AwsEc2VpcDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VpcDetailsPaginatorTypeDef",
+AwsEc2VpcDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VpcDetailsExtraOutputTypeDef",
+    {
+        "CidrBlockAssociationSet": NotRequired[List[CidrBlockAssociationTypeDef]],
+        "Ipv6CidrBlockAssociationSet": NotRequired[List[Ipv6CidrBlockAssociationTypeDef]],
+        "DhcpOptionsId": NotRequired[str],
+        "State": NotRequired[str],
+    },
+)
+AwsEc2VpcDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcDetailsOutputTypeDef",
     {
         "CidrBlockAssociationSet": NotRequired[List[CidrBlockAssociationTypeDef]],
         "Ipv6CidrBlockAssociationSet": NotRequired[List[Ipv6CidrBlockAssociationTypeDef]],
         "DhcpOptionsId": NotRequired[str],
         "State": NotRequired[str],
     },
 )
@@ -6072,16 +7066,32 @@
     {
         "CidrBlockAssociationSet": NotRequired[Sequence[CidrBlockAssociationTypeDef]],
         "Ipv6CidrBlockAssociationSet": NotRequired[Sequence[Ipv6CidrBlockAssociationTypeDef]],
         "DhcpOptionsId": NotRequired[str],
         "State": NotRequired[str],
     },
 )
-AwsEc2VpcEndpointServiceDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VpcEndpointServiceDetailsPaginatorTypeDef",
+AwsEc2VpcEndpointServiceDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VpcEndpointServiceDetailsExtraOutputTypeDef",
+    {
+        "AcceptanceRequired": NotRequired[bool],
+        "AvailabilityZones": NotRequired[List[str]],
+        "BaseEndpointDnsNames": NotRequired[List[str]],
+        "ManagesVpcEndpoints": NotRequired[bool],
+        "GatewayLoadBalancerArns": NotRequired[List[str]],
+        "NetworkLoadBalancerArns": NotRequired[List[str]],
+        "PrivateDnsName": NotRequired[str],
+        "ServiceId": NotRequired[str],
+        "ServiceName": NotRequired[str],
+        "ServiceState": NotRequired[str],
+        "ServiceType": NotRequired[List[AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef]],
+    },
+)
+AwsEc2VpcEndpointServiceDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcEndpointServiceDetailsOutputTypeDef",
     {
         "AcceptanceRequired": NotRequired[bool],
         "AvailabilityZones": NotRequired[List[str]],
         "BaseEndpointDnsNames": NotRequired[List[str]],
         "ManagesVpcEndpoints": NotRequired[bool],
         "GatewayLoadBalancerArns": NotRequired[List[str]],
         "NetworkLoadBalancerArns": NotRequired[List[str]],
@@ -6104,16 +7114,28 @@
         "PrivateDnsName": NotRequired[str],
         "ServiceId": NotRequired[str],
         "ServiceName": NotRequired[str],
         "ServiceState": NotRequired[str],
         "ServiceType": NotRequired[Sequence[AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef]],
     },
 )
-AwsEc2VpcPeeringConnectionVpcInfoDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VpcPeeringConnectionVpcInfoDetailsPaginatorTypeDef",
+AwsEc2VpcPeeringConnectionVpcInfoDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VpcPeeringConnectionVpcInfoDetailsExtraOutputTypeDef",
+    {
+        "CidrBlock": NotRequired[str],
+        "CidrBlockSet": NotRequired[List[VpcInfoCidrBlockSetDetailsTypeDef]],
+        "Ipv6CidrBlockSet": NotRequired[List[VpcInfoIpv6CidrBlockSetDetailsTypeDef]],
+        "OwnerId": NotRequired[str],
+        "PeeringOptions": NotRequired[VpcInfoPeeringOptionsDetailsTypeDef],
+        "Region": NotRequired[str],
+        "VpcId": NotRequired[str],
+    },
+)
+AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef",
     {
         "CidrBlock": NotRequired[str],
         "CidrBlockSet": NotRequired[List[VpcInfoCidrBlockSetDetailsTypeDef]],
         "Ipv6CidrBlockSet": NotRequired[List[VpcInfoIpv6CidrBlockSetDetailsTypeDef]],
         "OwnerId": NotRequired[str],
         "PeeringOptions": NotRequired[VpcInfoPeeringOptionsDetailsTypeDef],
         "Region": NotRequired[str],
@@ -6128,20 +7150,29 @@
         "Ipv6CidrBlockSet": NotRequired[Sequence[VpcInfoIpv6CidrBlockSetDetailsTypeDef]],
         "OwnerId": NotRequired[str],
         "PeeringOptions": NotRequired[VpcInfoPeeringOptionsDetailsTypeDef],
         "Region": NotRequired[str],
         "VpcId": NotRequired[str],
     },
 )
-AwsEc2VpnConnectionOptionsDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VpnConnectionOptionsDetailsPaginatorTypeDef",
+AwsEc2VpnConnectionOptionsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionOptionsDetailsExtraOutputTypeDef",
     {
         "StaticRoutesOnly": NotRequired[bool],
         "TunnelOptions": NotRequired[
-            List[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsPaginatorTypeDef]
+            List[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsExtraOutputTypeDef]
+        ],
+    },
+)
+AwsEc2VpnConnectionOptionsDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionOptionsDetailsOutputTypeDef",
+    {
+        "StaticRoutesOnly": NotRequired[bool],
+        "TunnelOptions": NotRequired[
+            List[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef]
         ],
     },
 )
 AwsEc2VpnConnectionOptionsDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionOptionsDetailsTypeDef",
     {
         "StaticRoutesOnly": NotRequired[bool],
@@ -6169,16 +7200,25 @@
         "KmsKeyId": NotRequired[str],
         "LogConfiguration": NotRequired[
             AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef
         ],
         "Logging": NotRequired[str],
     },
 )
-AwsEcsContainerDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsContainerDetailsPaginatorTypeDef",
+AwsEcsContainerDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsContainerDetailsExtraOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "Image": NotRequired[str],
+        "MountPoints": NotRequired[List[AwsMountPointTypeDef]],
+        "Privileged": NotRequired[bool],
+    },
+)
+AwsEcsContainerDetailsOutputTypeDef = TypedDict(
+    "AwsEcsContainerDetailsOutputTypeDef",
     {
         "Name": NotRequired[str],
         "Image": NotRequired[str],
         "MountPoints": NotRequired[List[AwsMountPointTypeDef]],
         "Privileged": NotRequired[bool],
     },
 )
@@ -6197,52 +7237,78 @@
         "DeploymentCircuitBreaker": NotRequired[
             AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef
         ],
         "MaximumPercent": NotRequired[int],
         "MinimumHealthyPercent": NotRequired[int],
     },
 )
-AwsEcsServiceNetworkConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsServiceNetworkConfigurationDetailsPaginatorTypeDef",
+AwsEcsServiceNetworkConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsServiceNetworkConfigurationDetailsExtraOutputTypeDef",
+    {
+        "AwsVpcConfiguration": NotRequired[
+            AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef",
     {
         "AwsVpcConfiguration": NotRequired[
-            AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsPaginatorTypeDef
+            AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef
         ],
     },
 )
 AwsEcsServiceNetworkConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceNetworkConfigurationDetailsTypeDef",
     {
         "AwsVpcConfiguration": NotRequired[
             AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef
         ],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsExtraOutputTypeDef",
     {
         "Capabilities": NotRequired[
-            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsPaginatorTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsExtraOutputTypeDef
         ],
         "Devices": NotRequired[
             List[
-                AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsPaginatorTypeDef
+                AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsExtraOutputTypeDef
             ]
         ],
         "InitProcessEnabled": NotRequired[bool],
         "MaxSwap": NotRequired[int],
         "SharedMemorySize": NotRequired[int],
         "Swappiness": NotRequired[int],
         "Tmpfs": NotRequired[
             List[
-                AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsPaginatorTypeDef
+                AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsExtraOutputTypeDef
             ]
         ],
     },
 )
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef",
+    {
+        "Capabilities": NotRequired[
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef
+        ],
+        "Devices": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef]
+        ],
+        "InitProcessEnabled": NotRequired[bool],
+        "MaxSwap": NotRequired[int],
+        "SharedMemorySize": NotRequired[int],
+        "Swappiness": NotRequired[int],
+        "Tmpfs": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef]
+        ],
+    },
+)
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
     {
         "Capabilities": NotRequired[
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef
         ],
         "Devices": NotRequired[
@@ -6253,16 +7319,28 @@
         "SharedMemorySize": NotRequired[int],
         "Swappiness": NotRequired[int],
         "Tmpfs": NotRequired[
             Sequence[AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef]
         ],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsExtraOutputTypeDef",
+    {
+        "LogDriver": NotRequired[str],
+        "Options": NotRequired[Dict[str, str]],
+        "SecretOptions": NotRequired[
+            List[
+                AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef
+            ]
+        ],
+    },
+)
+AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef",
     {
         "LogDriver": NotRequired[str],
         "Options": NotRequired[Dict[str, str]],
         "SecretOptions": NotRequired[
             List[
                 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef
             ]
@@ -6277,16 +7355,26 @@
         "SecretOptions": NotRequired[
             Sequence[
                 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef
             ]
         ],
     },
 )
-AwsEcsTaskDefinitionProxyConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionProxyConfigurationDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionProxyConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionProxyConfigurationDetailsExtraOutputTypeDef",
+    {
+        "ContainerName": NotRequired[str],
+        "ProxyConfigurationProperties": NotRequired[
+            List[AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef]
+        ],
+        "Type": NotRequired[str],
+    },
+)
+AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef",
     {
         "ContainerName": NotRequired[str],
         "ProxyConfigurationProperties": NotRequired[
             List[AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef]
         ],
         "Type": NotRequired[str],
     },
@@ -6325,30 +7413,57 @@
 AwsEfsAccessPointRootDirectoryDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointRootDirectoryDetailsTypeDef",
     {
         "CreationInfo": NotRequired[AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef],
         "Path": NotRequired[str],
     },
 )
-AwsEksClusterLoggingDetailsPaginatorTypeDef = TypedDict(
-    "AwsEksClusterLoggingDetailsPaginatorTypeDef",
+AwsEksClusterLoggingDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEksClusterLoggingDetailsExtraOutputTypeDef",
     {
         "ClusterLogging": NotRequired[
-            List[AwsEksClusterLoggingClusterLoggingDetailsPaginatorTypeDef]
+            List[AwsEksClusterLoggingClusterLoggingDetailsExtraOutputTypeDef]
         ],
     },
 )
+AwsEksClusterLoggingDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterLoggingDetailsOutputTypeDef",
+    {
+        "ClusterLogging": NotRequired[List[AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef]],
+    },
+)
 AwsEksClusterLoggingDetailsTypeDef = TypedDict(
     "AwsEksClusterLoggingDetailsTypeDef",
     {
         "ClusterLogging": NotRequired[Sequence[AwsEksClusterLoggingClusterLoggingDetailsTypeDef]],
     },
 )
-AwsElasticBeanstalkEnvironmentDetailsPaginatorTypeDef = TypedDict(
-    "AwsElasticBeanstalkEnvironmentDetailsPaginatorTypeDef",
+AwsElasticBeanstalkEnvironmentDetailsExtraOutputTypeDef = TypedDict(
+    "AwsElasticBeanstalkEnvironmentDetailsExtraOutputTypeDef",
+    {
+        "ApplicationName": NotRequired[str],
+        "Cname": NotRequired[str],
+        "DateCreated": NotRequired[str],
+        "DateUpdated": NotRequired[str],
+        "Description": NotRequired[str],
+        "EndpointUrl": NotRequired[str],
+        "EnvironmentArn": NotRequired[str],
+        "EnvironmentId": NotRequired[str],
+        "EnvironmentLinks": NotRequired[List[AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef]],
+        "EnvironmentName": NotRequired[str],
+        "OptionSettings": NotRequired[List[AwsElasticBeanstalkEnvironmentOptionSettingTypeDef]],
+        "PlatformArn": NotRequired[str],
+        "SolutionStackName": NotRequired[str],
+        "Status": NotRequired[str],
+        "Tier": NotRequired[AwsElasticBeanstalkEnvironmentTierTypeDef],
+        "VersionLabel": NotRequired[str],
+    },
+)
+AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef = TypedDict(
+    "AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef",
     {
         "ApplicationName": NotRequired[str],
         "Cname": NotRequired[str],
         "DateCreated": NotRequired[str],
         "DateUpdated": NotRequired[str],
         "Description": NotRequired[str],
         "EndpointUrl": NotRequired[str],
@@ -6405,16 +7520,24 @@
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
     {
         "IndexSlowLogs": NotRequired[AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef],
         "SearchSlowLogs": NotRequired[AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef],
         "AuditLogs": NotRequired[AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef],
     },
 )
-AwsElbLoadBalancerPoliciesPaginatorTypeDef = TypedDict(
-    "AwsElbLoadBalancerPoliciesPaginatorTypeDef",
+AwsElbLoadBalancerPoliciesExtraOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerPoliciesExtraOutputTypeDef",
+    {
+        "AppCookieStickinessPolicies": NotRequired[List[AwsElbAppCookieStickinessPolicyTypeDef]],
+        "LbCookieStickinessPolicies": NotRequired[List[AwsElbLbCookieStickinessPolicyTypeDef]],
+        "OtherPolicies": NotRequired[List[str]],
+    },
+)
+AwsElbLoadBalancerPoliciesOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerPoliciesOutputTypeDef",
     {
         "AppCookieStickinessPolicies": NotRequired[List[AwsElbAppCookieStickinessPolicyTypeDef]],
         "LbCookieStickinessPolicies": NotRequired[List[AwsElbLbCookieStickinessPolicyTypeDef]],
         "OtherPolicies": NotRequired[List[str]],
     },
 )
 AwsElbLoadBalancerPoliciesTypeDef = TypedDict(
@@ -6423,16 +7546,26 @@
         "AppCookieStickinessPolicies": NotRequired[
             Sequence[AwsElbAppCookieStickinessPolicyTypeDef]
         ],
         "LbCookieStickinessPolicies": NotRequired[Sequence[AwsElbLbCookieStickinessPolicyTypeDef]],
         "OtherPolicies": NotRequired[Sequence[str]],
     },
 )
-AwsElbLoadBalancerAttributesPaginatorTypeDef = TypedDict(
-    "AwsElbLoadBalancerAttributesPaginatorTypeDef",
+AwsElbLoadBalancerAttributesExtraOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerAttributesExtraOutputTypeDef",
+    {
+        "AccessLog": NotRequired[AwsElbLoadBalancerAccessLogTypeDef],
+        "ConnectionDraining": NotRequired[AwsElbLoadBalancerConnectionDrainingTypeDef],
+        "ConnectionSettings": NotRequired[AwsElbLoadBalancerConnectionSettingsTypeDef],
+        "CrossZoneLoadBalancing": NotRequired[AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef],
+        "AdditionalAttributes": NotRequired[List[AwsElbLoadBalancerAdditionalAttributeTypeDef]],
+    },
+)
+AwsElbLoadBalancerAttributesOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerAttributesOutputTypeDef",
     {
         "AccessLog": NotRequired[AwsElbLoadBalancerAccessLogTypeDef],
         "ConnectionDraining": NotRequired[AwsElbLoadBalancerConnectionDrainingTypeDef],
         "ConnectionSettings": NotRequired[AwsElbLoadBalancerConnectionSettingsTypeDef],
         "CrossZoneLoadBalancing": NotRequired[AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef],
         "AdditionalAttributes": NotRequired[List[AwsElbLoadBalancerAdditionalAttributeTypeDef]],
     },
@@ -6443,30 +7576,53 @@
         "AccessLog": NotRequired[AwsElbLoadBalancerAccessLogTypeDef],
         "ConnectionDraining": NotRequired[AwsElbLoadBalancerConnectionDrainingTypeDef],
         "ConnectionSettings": NotRequired[AwsElbLoadBalancerConnectionSettingsTypeDef],
         "CrossZoneLoadBalancing": NotRequired[AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef],
         "AdditionalAttributes": NotRequired[Sequence[AwsElbLoadBalancerAdditionalAttributeTypeDef]],
     },
 )
-AwsElbLoadBalancerListenerDescriptionPaginatorTypeDef = TypedDict(
-    "AwsElbLoadBalancerListenerDescriptionPaginatorTypeDef",
+AwsElbLoadBalancerListenerDescriptionExtraOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerListenerDescriptionExtraOutputTypeDef",
+    {
+        "Listener": NotRequired[AwsElbLoadBalancerListenerTypeDef],
+        "PolicyNames": NotRequired[List[str]],
+    },
+)
+AwsElbLoadBalancerListenerDescriptionOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerListenerDescriptionOutputTypeDef",
     {
         "Listener": NotRequired[AwsElbLoadBalancerListenerTypeDef],
         "PolicyNames": NotRequired[List[str]],
     },
 )
 AwsElbLoadBalancerListenerDescriptionTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
     {
         "Listener": NotRequired[AwsElbLoadBalancerListenerTypeDef],
         "PolicyNames": NotRequired[Sequence[str]],
     },
 )
-AwsElbv2LoadBalancerDetailsPaginatorTypeDef = TypedDict(
-    "AwsElbv2LoadBalancerDetailsPaginatorTypeDef",
+AwsElbv2LoadBalancerDetailsExtraOutputTypeDef = TypedDict(
+    "AwsElbv2LoadBalancerDetailsExtraOutputTypeDef",
+    {
+        "AvailabilityZones": NotRequired[List[AvailabilityZoneTypeDef]],
+        "CanonicalHostedZoneId": NotRequired[str],
+        "CreatedTime": NotRequired[str],
+        "DNSName": NotRequired[str],
+        "IpAddressType": NotRequired[str],
+        "Scheme": NotRequired[str],
+        "SecurityGroups": NotRequired[List[str]],
+        "State": NotRequired[LoadBalancerStateTypeDef],
+        "Type": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "LoadBalancerAttributes": NotRequired[List[AwsElbv2LoadBalancerAttributeTypeDef]],
+    },
+)
+AwsElbv2LoadBalancerDetailsOutputTypeDef = TypedDict(
+    "AwsElbv2LoadBalancerDetailsOutputTypeDef",
     {
         "AvailabilityZones": NotRequired[List[AvailabilityZoneTypeDef]],
         "CanonicalHostedZoneId": NotRequired[str],
         "CreatedTime": NotRequired[str],
         "DNSName": NotRequired[str],
         "IpAddressType": NotRequired[str],
         "Scheme": NotRequired[str],
@@ -6519,16 +7675,27 @@
 AwsIamAccessKeySessionContextTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextTypeDef",
     {
         "Attributes": NotRequired[AwsIamAccessKeySessionContextAttributesTypeDef],
         "SessionIssuer": NotRequired[AwsIamAccessKeySessionContextSessionIssuerTypeDef],
     },
 )
-AwsIamGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsIamGroupDetailsPaginatorTypeDef",
+AwsIamGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsIamGroupDetailsExtraOutputTypeDef",
+    {
+        "AttachedManagedPolicies": NotRequired[List[AwsIamAttachedManagedPolicyTypeDef]],
+        "CreateDate": NotRequired[str],
+        "GroupId": NotRequired[str],
+        "GroupName": NotRequired[str],
+        "GroupPolicyList": NotRequired[List[AwsIamGroupPolicyTypeDef]],
+        "Path": NotRequired[str],
+    },
+)
+AwsIamGroupDetailsOutputTypeDef = TypedDict(
+    "AwsIamGroupDetailsOutputTypeDef",
     {
         "AttachedManagedPolicies": NotRequired[List[AwsIamAttachedManagedPolicyTypeDef]],
         "CreateDate": NotRequired[str],
         "GroupId": NotRequired[str],
         "GroupName": NotRequired[str],
         "GroupPolicyList": NotRequired[List[AwsIamGroupPolicyTypeDef]],
         "Path": NotRequired[str],
@@ -6541,16 +7708,27 @@
         "CreateDate": NotRequired[str],
         "GroupId": NotRequired[str],
         "GroupName": NotRequired[str],
         "GroupPolicyList": NotRequired[Sequence[AwsIamGroupPolicyTypeDef]],
         "Path": NotRequired[str],
     },
 )
-AwsIamInstanceProfilePaginatorTypeDef = TypedDict(
-    "AwsIamInstanceProfilePaginatorTypeDef",
+AwsIamInstanceProfileExtraOutputTypeDef = TypedDict(
+    "AwsIamInstanceProfileExtraOutputTypeDef",
+    {
+        "Arn": NotRequired[str],
+        "CreateDate": NotRequired[str],
+        "InstanceProfileId": NotRequired[str],
+        "InstanceProfileName": NotRequired[str],
+        "Path": NotRequired[str],
+        "Roles": NotRequired[List[AwsIamInstanceProfileRoleTypeDef]],
+    },
+)
+AwsIamInstanceProfileOutputTypeDef = TypedDict(
+    "AwsIamInstanceProfileOutputTypeDef",
     {
         "Arn": NotRequired[str],
         "CreateDate": NotRequired[str],
         "InstanceProfileId": NotRequired[str],
         "InstanceProfileName": NotRequired[str],
         "Path": NotRequired[str],
         "Roles": NotRequired[List[AwsIamInstanceProfileRoleTypeDef]],
@@ -6563,16 +7741,32 @@
         "CreateDate": NotRequired[str],
         "InstanceProfileId": NotRequired[str],
         "InstanceProfileName": NotRequired[str],
         "Path": NotRequired[str],
         "Roles": NotRequired[Sequence[AwsIamInstanceProfileRoleTypeDef]],
     },
 )
-AwsIamPolicyDetailsPaginatorTypeDef = TypedDict(
-    "AwsIamPolicyDetailsPaginatorTypeDef",
+AwsIamPolicyDetailsExtraOutputTypeDef = TypedDict(
+    "AwsIamPolicyDetailsExtraOutputTypeDef",
+    {
+        "AttachmentCount": NotRequired[int],
+        "CreateDate": NotRequired[str],
+        "DefaultVersionId": NotRequired[str],
+        "Description": NotRequired[str],
+        "IsAttachable": NotRequired[bool],
+        "Path": NotRequired[str],
+        "PermissionsBoundaryUsageCount": NotRequired[int],
+        "PolicyId": NotRequired[str],
+        "PolicyName": NotRequired[str],
+        "PolicyVersionList": NotRequired[List[AwsIamPolicyVersionTypeDef]],
+        "UpdateDate": NotRequired[str],
+    },
+)
+AwsIamPolicyDetailsOutputTypeDef = TypedDict(
+    "AwsIamPolicyDetailsOutputTypeDef",
     {
         "AttachmentCount": NotRequired[int],
         "CreateDate": NotRequired[str],
         "DefaultVersionId": NotRequired[str],
         "Description": NotRequired[str],
         "IsAttachable": NotRequired[bool],
         "Path": NotRequired[str],
@@ -6595,16 +7789,29 @@
         "PermissionsBoundaryUsageCount": NotRequired[int],
         "PolicyId": NotRequired[str],
         "PolicyName": NotRequired[str],
         "PolicyVersionList": NotRequired[Sequence[AwsIamPolicyVersionTypeDef]],
         "UpdateDate": NotRequired[str],
     },
 )
-AwsIamUserDetailsPaginatorTypeDef = TypedDict(
-    "AwsIamUserDetailsPaginatorTypeDef",
+AwsIamUserDetailsExtraOutputTypeDef = TypedDict(
+    "AwsIamUserDetailsExtraOutputTypeDef",
+    {
+        "AttachedManagedPolicies": NotRequired[List[AwsIamAttachedManagedPolicyTypeDef]],
+        "CreateDate": NotRequired[str],
+        "GroupList": NotRequired[List[str]],
+        "Path": NotRequired[str],
+        "PermissionsBoundary": NotRequired[AwsIamPermissionsBoundaryTypeDef],
+        "UserId": NotRequired[str],
+        "UserName": NotRequired[str],
+        "UserPolicyList": NotRequired[List[AwsIamUserPolicyTypeDef]],
+    },
+)
+AwsIamUserDetailsOutputTypeDef = TypedDict(
+    "AwsIamUserDetailsOutputTypeDef",
     {
         "AttachedManagedPolicies": NotRequired[List[AwsIamAttachedManagedPolicyTypeDef]],
         "CreateDate": NotRequired[str],
         "GroupList": NotRequired[List[str]],
         "Path": NotRequired[str],
         "PermissionsBoundary": NotRequired[AwsIamPermissionsBoundaryTypeDef],
         "UserId": NotRequired[str],
@@ -6631,16 +7838,23 @@
         "Name": NotRequired[str],
         "Arn": NotRequired[str],
         "StreamEncryption": NotRequired[AwsKinesisStreamStreamEncryptionDetailsTypeDef],
         "ShardCount": NotRequired[int],
         "RetentionPeriodHours": NotRequired[int],
     },
 )
-AwsLambdaFunctionEnvironmentPaginatorTypeDef = TypedDict(
-    "AwsLambdaFunctionEnvironmentPaginatorTypeDef",
+AwsLambdaFunctionEnvironmentExtraOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionEnvironmentExtraOutputTypeDef",
+    {
+        "Variables": NotRequired[Dict[str, str]],
+        "Error": NotRequired[AwsLambdaFunctionEnvironmentErrorTypeDef],
+    },
+)
+AwsLambdaFunctionEnvironmentOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionEnvironmentOutputTypeDef",
     {
         "Variables": NotRequired[Dict[str, str]],
         "Error": NotRequired[AwsLambdaFunctionEnvironmentErrorTypeDef],
     },
 )
 AwsLambdaFunctionEnvironmentTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentTypeDef",
@@ -6663,16 +7877,31 @@
             AwsMskClusterClusterInfoEncryptionInfoEncryptionInTransitDetailsTypeDef
         ],
         "EncryptionAtRest": NotRequired[
             AwsMskClusterClusterInfoEncryptionInfoEncryptionAtRestDetailsTypeDef
         ],
     },
 )
-AwsNetworkFirewallFirewallDetailsPaginatorTypeDef = TypedDict(
-    "AwsNetworkFirewallFirewallDetailsPaginatorTypeDef",
+AwsNetworkFirewallFirewallDetailsExtraOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallFirewallDetailsExtraOutputTypeDef",
+    {
+        "DeleteProtection": NotRequired[bool],
+        "Description": NotRequired[str],
+        "FirewallArn": NotRequired[str],
+        "FirewallId": NotRequired[str],
+        "FirewallName": NotRequired[str],
+        "FirewallPolicyArn": NotRequired[str],
+        "FirewallPolicyChangeProtection": NotRequired[bool],
+        "SubnetChangeProtection": NotRequired[bool],
+        "SubnetMappings": NotRequired[List[AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef]],
+        "VpcId": NotRequired[str],
+    },
+)
+AwsNetworkFirewallFirewallDetailsOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallFirewallDetailsOutputTypeDef",
     {
         "DeleteProtection": NotRequired[bool],
         "Description": NotRequired[str],
         "FirewallArn": NotRequired[str],
         "FirewallId": NotRequired[str],
         "FirewallName": NotRequired[str],
         "FirewallPolicyArn": NotRequired[str],
@@ -6728,16 +7957,61 @@
     "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef",
     {
         "IndexSlowLogs": NotRequired[AwsOpenSearchServiceDomainLogPublishingOptionTypeDef],
         "SearchSlowLogs": NotRequired[AwsOpenSearchServiceDomainLogPublishingOptionTypeDef],
         "AuditLogs": NotRequired[AwsOpenSearchServiceDomainLogPublishingOptionTypeDef],
     },
 )
-AwsRdsDbClusterDetailsPaginatorTypeDef = TypedDict(
-    "AwsRdsDbClusterDetailsPaginatorTypeDef",
+AwsRdsDbClusterDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterDetailsExtraOutputTypeDef",
+    {
+        "AllocatedStorage": NotRequired[int],
+        "AvailabilityZones": NotRequired[List[str]],
+        "BackupRetentionPeriod": NotRequired[int],
+        "DatabaseName": NotRequired[str],
+        "Status": NotRequired[str],
+        "Endpoint": NotRequired[str],
+        "ReaderEndpoint": NotRequired[str],
+        "CustomEndpoints": NotRequired[List[str]],
+        "MultiAz": NotRequired[bool],
+        "Engine": NotRequired[str],
+        "EngineVersion": NotRequired[str],
+        "Port": NotRequired[int],
+        "MasterUsername": NotRequired[str],
+        "PreferredBackupWindow": NotRequired[str],
+        "PreferredMaintenanceWindow": NotRequired[str],
+        "ReadReplicaIdentifiers": NotRequired[List[str]],
+        "VpcSecurityGroups": NotRequired[List[AwsRdsDbInstanceVpcSecurityGroupTypeDef]],
+        "HostedZoneId": NotRequired[str],
+        "StorageEncrypted": NotRequired[bool],
+        "KmsKeyId": NotRequired[str],
+        "DbClusterResourceId": NotRequired[str],
+        "AssociatedRoles": NotRequired[List[AwsRdsDbClusterAssociatedRoleTypeDef]],
+        "ClusterCreateTime": NotRequired[str],
+        "EnabledCloudWatchLogsExports": NotRequired[List[str]],
+        "EngineMode": NotRequired[str],
+        "DeletionProtection": NotRequired[bool],
+        "HttpEndpointEnabled": NotRequired[bool],
+        "ActivityStreamStatus": NotRequired[str],
+        "CopyTagsToSnapshot": NotRequired[bool],
+        "CrossAccountClone": NotRequired[bool],
+        "DomainMemberships": NotRequired[List[AwsRdsDbDomainMembershipTypeDef]],
+        "DbClusterParameterGroup": NotRequired[str],
+        "DbSubnetGroup": NotRequired[str],
+        "DbClusterOptionGroupMemberships": NotRequired[
+            List[AwsRdsDbClusterOptionGroupMembershipTypeDef]
+        ],
+        "DbClusterIdentifier": NotRequired[str],
+        "DbClusterMembers": NotRequired[List[AwsRdsDbClusterMemberTypeDef]],
+        "IamDatabaseAuthenticationEnabled": NotRequired[bool],
+        "AutoMinorVersionUpgrade": NotRequired[bool],
+    },
+)
+AwsRdsDbClusterDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterDetailsOutputTypeDef",
     {
         "AllocatedStorage": NotRequired[int],
         "AvailabilityZones": NotRequired[List[str]],
         "BackupRetentionPeriod": NotRequired[int],
         "DatabaseName": NotRequired[str],
         "Status": NotRequired[str],
         "Endpoint": NotRequired[str],
@@ -6818,16 +8092,16 @@
         ],
         "DbClusterIdentifier": NotRequired[str],
         "DbClusterMembers": NotRequired[Sequence[AwsRdsDbClusterMemberTypeDef]],
         "IamDatabaseAuthenticationEnabled": NotRequired[bool],
         "AutoMinorVersionUpgrade": NotRequired[bool],
     },
 )
-AwsRdsDbClusterSnapshotDetailsPaginatorTypeDef = TypedDict(
-    "AwsRdsDbClusterSnapshotDetailsPaginatorTypeDef",
+AwsRdsDbClusterSnapshotDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterSnapshotDetailsExtraOutputTypeDef",
     {
         "AvailabilityZones": NotRequired[List[str]],
         "SnapshotCreateTime": NotRequired[str],
         "Engine": NotRequired[str],
         "AllocatedStorage": NotRequired[int],
         "Status": NotRequired[str],
         "Port": NotRequired[int],
@@ -6840,15 +8114,41 @@
         "PercentProgress": NotRequired[int],
         "StorageEncrypted": NotRequired[bool],
         "KmsKeyId": NotRequired[str],
         "DbClusterIdentifier": NotRequired[str],
         "DbClusterSnapshotIdentifier": NotRequired[str],
         "IamDatabaseAuthenticationEnabled": NotRequired[bool],
         "DbClusterSnapshotAttributes": NotRequired[
-            List[AwsRdsDbClusterSnapshotDbClusterSnapshotAttributePaginatorTypeDef]
+            List[AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeExtraOutputTypeDef]
+        ],
+    },
+)
+AwsRdsDbClusterSnapshotDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterSnapshotDetailsOutputTypeDef",
+    {
+        "AvailabilityZones": NotRequired[List[str]],
+        "SnapshotCreateTime": NotRequired[str],
+        "Engine": NotRequired[str],
+        "AllocatedStorage": NotRequired[int],
+        "Status": NotRequired[str],
+        "Port": NotRequired[int],
+        "VpcId": NotRequired[str],
+        "ClusterCreateTime": NotRequired[str],
+        "MasterUsername": NotRequired[str],
+        "EngineVersion": NotRequired[str],
+        "LicenseModel": NotRequired[str],
+        "SnapshotType": NotRequired[str],
+        "PercentProgress": NotRequired[int],
+        "StorageEncrypted": NotRequired[bool],
+        "KmsKeyId": NotRequired[str],
+        "DbClusterIdentifier": NotRequired[str],
+        "DbClusterSnapshotIdentifier": NotRequired[str],
+        "IamDatabaseAuthenticationEnabled": NotRequired[bool],
+        "DbClusterSnapshotAttributes": NotRequired[
+            List[AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef]
         ],
     },
 )
 AwsRdsDbClusterSnapshotDetailsTypeDef = TypedDict(
     "AwsRdsDbClusterSnapshotDetailsTypeDef",
     {
         "AvailabilityZones": NotRequired[Sequence[str]],
@@ -6870,16 +8170,48 @@
         "DbClusterSnapshotIdentifier": NotRequired[str],
         "IamDatabaseAuthenticationEnabled": NotRequired[bool],
         "DbClusterSnapshotAttributes": NotRequired[
             Sequence[AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef]
         ],
     },
 )
-AwsRdsDbSnapshotDetailsPaginatorTypeDef = TypedDict(
-    "AwsRdsDbSnapshotDetailsPaginatorTypeDef",
+AwsRdsDbSnapshotDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbSnapshotDetailsExtraOutputTypeDef",
+    {
+        "DbSnapshotIdentifier": NotRequired[str],
+        "DbInstanceIdentifier": NotRequired[str],
+        "SnapshotCreateTime": NotRequired[str],
+        "Engine": NotRequired[str],
+        "AllocatedStorage": NotRequired[int],
+        "Status": NotRequired[str],
+        "Port": NotRequired[int],
+        "AvailabilityZone": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "InstanceCreateTime": NotRequired[str],
+        "MasterUsername": NotRequired[str],
+        "EngineVersion": NotRequired[str],
+        "LicenseModel": NotRequired[str],
+        "SnapshotType": NotRequired[str],
+        "Iops": NotRequired[int],
+        "OptionGroupName": NotRequired[str],
+        "PercentProgress": NotRequired[int],
+        "SourceRegion": NotRequired[str],
+        "SourceDbSnapshotIdentifier": NotRequired[str],
+        "StorageType": NotRequired[str],
+        "TdeCredentialArn": NotRequired[str],
+        "Encrypted": NotRequired[bool],
+        "KmsKeyId": NotRequired[str],
+        "Timezone": NotRequired[str],
+        "IamDatabaseAuthenticationEnabled": NotRequired[bool],
+        "ProcessorFeatures": NotRequired[List[AwsRdsDbProcessorFeatureTypeDef]],
+        "DbiResourceId": NotRequired[str],
+    },
+)
+AwsRdsDbSnapshotDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbSnapshotDetailsOutputTypeDef",
     {
         "DbSnapshotIdentifier": NotRequired[str],
         "DbInstanceIdentifier": NotRequired[str],
         "SnapshotCreateTime": NotRequired[str],
         "Engine": NotRequired[str],
         "AllocatedStorage": NotRequired[int],
         "Status": NotRequired[str],
@@ -6934,16 +8266,16 @@
         "KmsKeyId": NotRequired[str],
         "Timezone": NotRequired[str],
         "IamDatabaseAuthenticationEnabled": NotRequired[bool],
         "ProcessorFeatures": NotRequired[Sequence[AwsRdsDbProcessorFeatureTypeDef]],
         "DbiResourceId": NotRequired[str],
     },
 )
-AwsRdsDbPendingModifiedValuesPaginatorTypeDef = TypedDict(
-    "AwsRdsDbPendingModifiedValuesPaginatorTypeDef",
+AwsRdsDbPendingModifiedValuesExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbPendingModifiedValuesExtraOutputTypeDef",
     {
         "DbInstanceClass": NotRequired[str],
         "AllocatedStorage": NotRequired[int],
         "MasterUserPassword": NotRequired[str],
         "Port": NotRequired[int],
         "BackupRetentionPeriod": NotRequired[int],
         "MultiAZ": NotRequired[bool],
@@ -6951,15 +8283,37 @@
         "LicenseModel": NotRequired[str],
         "Iops": NotRequired[int],
         "DbInstanceIdentifier": NotRequired[str],
         "StorageType": NotRequired[str],
         "CaCertificateIdentifier": NotRequired[str],
         "DbSubnetGroupName": NotRequired[str],
         "PendingCloudWatchLogsExports": NotRequired[
-            AwsRdsPendingCloudWatchLogsExportsPaginatorTypeDef
+            AwsRdsPendingCloudWatchLogsExportsExtraOutputTypeDef
+        ],
+        "ProcessorFeatures": NotRequired[List[AwsRdsDbProcessorFeatureTypeDef]],
+    },
+)
+AwsRdsDbPendingModifiedValuesOutputTypeDef = TypedDict(
+    "AwsRdsDbPendingModifiedValuesOutputTypeDef",
+    {
+        "DbInstanceClass": NotRequired[str],
+        "AllocatedStorage": NotRequired[int],
+        "MasterUserPassword": NotRequired[str],
+        "Port": NotRequired[int],
+        "BackupRetentionPeriod": NotRequired[int],
+        "MultiAZ": NotRequired[bool],
+        "EngineVersion": NotRequired[str],
+        "LicenseModel": NotRequired[str],
+        "Iops": NotRequired[int],
+        "DbInstanceIdentifier": NotRequired[str],
+        "StorageType": NotRequired[str],
+        "CaCertificateIdentifier": NotRequired[str],
+        "DbSubnetGroupName": NotRequired[str],
+        "PendingCloudWatchLogsExports": NotRequired[
+            AwsRdsPendingCloudWatchLogsExportsOutputTypeDef
         ],
         "ProcessorFeatures": NotRequired[List[AwsRdsDbProcessorFeatureTypeDef]],
     },
 )
 AwsRdsDbPendingModifiedValuesTypeDef = TypedDict(
     "AwsRdsDbPendingModifiedValuesTypeDef",
     {
@@ -6976,16 +8330,28 @@
         "StorageType": NotRequired[str],
         "CaCertificateIdentifier": NotRequired[str],
         "DbSubnetGroupName": NotRequired[str],
         "PendingCloudWatchLogsExports": NotRequired[AwsRdsPendingCloudWatchLogsExportsTypeDef],
         "ProcessorFeatures": NotRequired[Sequence[AwsRdsDbProcessorFeatureTypeDef]],
     },
 )
-AwsRdsDbSecurityGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsRdsDbSecurityGroupDetailsPaginatorTypeDef",
+AwsRdsDbSecurityGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbSecurityGroupDetailsExtraOutputTypeDef",
+    {
+        "DbSecurityGroupArn": NotRequired[str],
+        "DbSecurityGroupDescription": NotRequired[str],
+        "DbSecurityGroupName": NotRequired[str],
+        "Ec2SecurityGroups": NotRequired[List[AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef]],
+        "IpRanges": NotRequired[List[AwsRdsDbSecurityGroupIpRangeTypeDef]],
+        "OwnerId": NotRequired[str],
+        "VpcId": NotRequired[str],
+    },
+)
+AwsRdsDbSecurityGroupDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbSecurityGroupDetailsOutputTypeDef",
     {
         "DbSecurityGroupArn": NotRequired[str],
         "DbSecurityGroupDescription": NotRequired[str],
         "DbSecurityGroupName": NotRequired[str],
         "Ec2SecurityGroups": NotRequired[List[AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef]],
         "IpRanges": NotRequired[List[AwsRdsDbSecurityGroupIpRangeTypeDef]],
         "OwnerId": NotRequired[str],
@@ -7008,16 +8374,26 @@
     "AwsRdsDbSubnetGroupSubnetTypeDef",
     {
         "SubnetIdentifier": NotRequired[str],
         "SubnetAvailabilityZone": NotRequired[AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef],
         "SubnetStatus": NotRequired[str],
     },
 )
-AwsRedshiftClusterClusterParameterGroupPaginatorTypeDef = TypedDict(
-    "AwsRedshiftClusterClusterParameterGroupPaginatorTypeDef",
+AwsRedshiftClusterClusterParameterGroupExtraOutputTypeDef = TypedDict(
+    "AwsRedshiftClusterClusterParameterGroupExtraOutputTypeDef",
+    {
+        "ClusterParameterStatusList": NotRequired[
+            List[AwsRedshiftClusterClusterParameterStatusTypeDef]
+        ],
+        "ParameterApplyStatus": NotRequired[str],
+        "ParameterGroupName": NotRequired[str],
+    },
+)
+AwsRedshiftClusterClusterParameterGroupOutputTypeDef = TypedDict(
+    "AwsRedshiftClusterClusterParameterGroupOutputTypeDef",
     {
         "ClusterParameterStatusList": NotRequired[
             List[AwsRedshiftClusterClusterParameterStatusTypeDef]
         ],
         "ParameterApplyStatus": NotRequired[str],
         "ParameterGroupName": NotRequired[str],
     },
@@ -7065,16 +8441,24 @@
         "Prefix": NotRequired[str],
         "Tag": NotRequired[
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef
         ],
         "Type": NotRequired[str],
     },
 )
-AwsS3BucketNotificationConfigurationS3KeyFilterPaginatorTypeDef = TypedDict(
-    "AwsS3BucketNotificationConfigurationS3KeyFilterPaginatorTypeDef",
+AwsS3BucketNotificationConfigurationS3KeyFilterExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationS3KeyFilterExtraOutputTypeDef",
+    {
+        "FilterRules": NotRequired[
+            List[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef]
+        ],
+    },
+)
+AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef",
     {
         "FilterRules": NotRequired[
             List[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef]
         ],
     },
 )
 AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef = TypedDict(
@@ -7104,16 +8488,43 @@
 AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
     {
         "Condition": NotRequired[AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef],
         "Redirect": NotRequired[AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef],
     },
 )
-AwsSageMakerNotebookInstanceDetailsPaginatorTypeDef = TypedDict(
-    "AwsSageMakerNotebookInstanceDetailsPaginatorTypeDef",
+AwsSageMakerNotebookInstanceDetailsExtraOutputTypeDef = TypedDict(
+    "AwsSageMakerNotebookInstanceDetailsExtraOutputTypeDef",
+    {
+        "AcceleratorTypes": NotRequired[List[str]],
+        "AdditionalCodeRepositories": NotRequired[List[str]],
+        "DefaultCodeRepository": NotRequired[str],
+        "DirectInternetAccess": NotRequired[str],
+        "FailureReason": NotRequired[str],
+        "InstanceMetadataServiceConfiguration": NotRequired[
+            AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef
+        ],
+        "InstanceType": NotRequired[str],
+        "KmsKeyId": NotRequired[str],
+        "NetworkInterfaceId": NotRequired[str],
+        "NotebookInstanceArn": NotRequired[str],
+        "NotebookInstanceLifecycleConfigName": NotRequired[str],
+        "NotebookInstanceName": NotRequired[str],
+        "NotebookInstanceStatus": NotRequired[str],
+        "PlatformIdentifier": NotRequired[str],
+        "RoleArn": NotRequired[str],
+        "RootAccess": NotRequired[str],
+        "SecurityGroups": NotRequired[List[str]],
+        "SubnetId": NotRequired[str],
+        "Url": NotRequired[str],
+        "VolumeSizeInGB": NotRequired[int],
+    },
+)
+AwsSageMakerNotebookInstanceDetailsOutputTypeDef = TypedDict(
+    "AwsSageMakerNotebookInstanceDetailsOutputTypeDef",
     {
         "AcceleratorTypes": NotRequired[List[str]],
         "AdditionalCodeRepositories": NotRequired[List[str]],
         "DefaultCodeRepository": NotRequired[str],
         "DirectInternetAccess": NotRequired[str],
         "FailureReason": NotRequired[str],
         "InstanceMetadataServiceConfiguration": NotRequired[
@@ -7194,16 +8605,32 @@
     "BatchUpdateFindingsUnprocessedFindingTypeDef",
     {
         "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
-AwsSnsTopicDetailsPaginatorTypeDef = TypedDict(
-    "AwsSnsTopicDetailsPaginatorTypeDef",
+AwsSnsTopicDetailsExtraOutputTypeDef = TypedDict(
+    "AwsSnsTopicDetailsExtraOutputTypeDef",
+    {
+        "KmsMasterKeyId": NotRequired[str],
+        "Subscription": NotRequired[List[AwsSnsTopicSubscriptionTypeDef]],
+        "TopicName": NotRequired[str],
+        "Owner": NotRequired[str],
+        "SqsSuccessFeedbackRoleArn": NotRequired[str],
+        "SqsFailureFeedbackRoleArn": NotRequired[str],
+        "ApplicationSuccessFeedbackRoleArn": NotRequired[str],
+        "FirehoseSuccessFeedbackRoleArn": NotRequired[str],
+        "FirehoseFailureFeedbackRoleArn": NotRequired[str],
+        "HttpSuccessFeedbackRoleArn": NotRequired[str],
+        "HttpFailureFeedbackRoleArn": NotRequired[str],
+    },
+)
+AwsSnsTopicDetailsOutputTypeDef = TypedDict(
+    "AwsSnsTopicDetailsOutputTypeDef",
     {
         "KmsMasterKeyId": NotRequired[str],
         "Subscription": NotRequired[List[AwsSnsTopicSubscriptionTypeDef]],
         "TopicName": NotRequired[str],
         "Owner": NotRequired[str],
         "SqsSuccessFeedbackRoleArn": NotRequired[str],
         "SqsFailureFeedbackRoleArn": NotRequired[str],
@@ -7240,16 +8667,27 @@
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
     {
         "CloudWatchLogsLogGroup": NotRequired[
             AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef
         ],
     },
 )
-AwsWafRateBasedRuleDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafRateBasedRuleDetailsPaginatorTypeDef",
+AwsWafRateBasedRuleDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafRateBasedRuleDetailsExtraOutputTypeDef",
+    {
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "RateKey": NotRequired[str],
+        "RateLimit": NotRequired[int],
+        "RuleId": NotRequired[str],
+        "MatchPredicates": NotRequired[List[AwsWafRateBasedRuleMatchPredicateTypeDef]],
+    },
+)
+AwsWafRateBasedRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRateBasedRuleDetailsOutputTypeDef",
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RateKey": NotRequired[str],
         "RateLimit": NotRequired[int],
         "RuleId": NotRequired[str],
         "MatchPredicates": NotRequired[List[AwsWafRateBasedRuleMatchPredicateTypeDef]],
@@ -7262,16 +8700,27 @@
         "Name": NotRequired[str],
         "RateKey": NotRequired[str],
         "RateLimit": NotRequired[int],
         "RuleId": NotRequired[str],
         "MatchPredicates": NotRequired[Sequence[AwsWafRateBasedRuleMatchPredicateTypeDef]],
     },
 )
-AwsWafRegionalRateBasedRuleDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafRegionalRateBasedRuleDetailsPaginatorTypeDef",
+AwsWafRegionalRateBasedRuleDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafRegionalRateBasedRuleDetailsExtraOutputTypeDef",
+    {
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "RateKey": NotRequired[str],
+        "RateLimit": NotRequired[int],
+        "RuleId": NotRequired[str],
+        "MatchPredicates": NotRequired[List[AwsWafRegionalRateBasedRuleMatchPredicateTypeDef]],
+    },
+)
+AwsWafRegionalRateBasedRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalRateBasedRuleDetailsOutputTypeDef",
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RateKey": NotRequired[str],
         "RateLimit": NotRequired[int],
         "RuleId": NotRequired[str],
         "MatchPredicates": NotRequired[List[AwsWafRegionalRateBasedRuleMatchPredicateTypeDef]],
@@ -7284,16 +8733,25 @@
         "Name": NotRequired[str],
         "RateKey": NotRequired[str],
         "RateLimit": NotRequired[int],
         "RuleId": NotRequired[str],
         "MatchPredicates": NotRequired[Sequence[AwsWafRegionalRateBasedRuleMatchPredicateTypeDef]],
     },
 )
-AwsWafRegionalRuleDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafRegionalRuleDetailsPaginatorTypeDef",
+AwsWafRegionalRuleDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafRegionalRuleDetailsExtraOutputTypeDef",
+    {
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "PredicateList": NotRequired[List[AwsWafRegionalRulePredicateListDetailsTypeDef]],
+        "RuleId": NotRequired[str],
+    },
+)
+AwsWafRegionalRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalRuleDetailsOutputTypeDef",
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "PredicateList": NotRequired[List[AwsWafRegionalRulePredicateListDetailsTypeDef]],
         "RuleId": NotRequired[str],
     },
 )
@@ -7321,16 +8779,25 @@
         "Action": NotRequired[AwsWafRegionalWebAclRulesListActionDetailsTypeDef],
         "OverrideAction": NotRequired[AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef],
         "Priority": NotRequired[int],
         "RuleId": NotRequired[str],
         "Type": NotRequired[str],
     },
 )
-AwsWafRuleDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafRuleDetailsPaginatorTypeDef",
+AwsWafRuleDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafRuleDetailsExtraOutputTypeDef",
+    {
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "PredicateList": NotRequired[List[AwsWafRulePredicateListDetailsTypeDef]],
+        "RuleId": NotRequired[str],
+    },
+)
+AwsWafRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRuleDetailsOutputTypeDef",
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "PredicateList": NotRequired[List[AwsWafRulePredicateListDetailsTypeDef]],
         "RuleId": NotRequired[str],
     },
 )
@@ -7348,16 +8815,27 @@
     {
         "Action": NotRequired[AwsWafRuleGroupRulesActionDetailsTypeDef],
         "Priority": NotRequired[int],
         "RuleId": NotRequired[str],
         "Type": NotRequired[str],
     },
 )
-AwsWafWebAclRulePaginatorTypeDef = TypedDict(
-    "AwsWafWebAclRulePaginatorTypeDef",
+AwsWafWebAclRuleExtraOutputTypeDef = TypedDict(
+    "AwsWafWebAclRuleExtraOutputTypeDef",
+    {
+        "Action": NotRequired[WafActionTypeDef],
+        "ExcludedRules": NotRequired[List[WafExcludedRuleTypeDef]],
+        "OverrideAction": NotRequired[WafOverrideActionTypeDef],
+        "Priority": NotRequired[int],
+        "RuleId": NotRequired[str],
+        "Type": NotRequired[str],
+    },
+)
+AwsWafWebAclRuleOutputTypeDef = TypedDict(
+    "AwsWafWebAclRuleOutputTypeDef",
     {
         "Action": NotRequired[WafActionTypeDef],
         "ExcludedRules": NotRequired[List[WafExcludedRuleTypeDef]],
         "OverrideAction": NotRequired[WafOverrideActionTypeDef],
         "Priority": NotRequired[int],
         "RuleId": NotRequired[str],
         "Type": NotRequired[str],
@@ -7370,28 +8848,42 @@
         "ExcludedRules": NotRequired[Sequence[WafExcludedRuleTypeDef]],
         "OverrideAction": NotRequired[WafOverrideActionTypeDef],
         "Priority": NotRequired[int],
         "RuleId": NotRequired[str],
         "Type": NotRequired[str],
     },
 )
-AwsWafv2CustomRequestHandlingDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2CustomRequestHandlingDetailsPaginatorTypeDef",
+AwsWafv2CustomRequestHandlingDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2CustomRequestHandlingDetailsExtraOutputTypeDef",
+    {
+        "InsertHeaders": NotRequired[List[AwsWafv2CustomHttpHeaderTypeDef]],
+    },
+)
+AwsWafv2CustomRequestHandlingDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2CustomRequestHandlingDetailsOutputTypeDef",
     {
         "InsertHeaders": NotRequired[List[AwsWafv2CustomHttpHeaderTypeDef]],
     },
 )
 AwsWafv2CustomRequestHandlingDetailsTypeDef = TypedDict(
     "AwsWafv2CustomRequestHandlingDetailsTypeDef",
     {
         "InsertHeaders": NotRequired[Sequence[AwsWafv2CustomHttpHeaderTypeDef]],
     },
 )
-AwsWafv2CustomResponseDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2CustomResponseDetailsPaginatorTypeDef",
+AwsWafv2CustomResponseDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2CustomResponseDetailsExtraOutputTypeDef",
+    {
+        "CustomResponseBodyKey": NotRequired[str],
+        "ResponseCode": NotRequired[int],
+        "ResponseHeaders": NotRequired[List[AwsWafv2CustomHttpHeaderTypeDef]],
+    },
+)
+AwsWafv2CustomResponseDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2CustomResponseDetailsOutputTypeDef",
     {
         "CustomResponseBodyKey": NotRequired[str],
         "ResponseCode": NotRequired[int],
         "ResponseHeaders": NotRequired[List[AwsWafv2CustomHttpHeaderTypeDef]],
     },
 )
 AwsWafv2CustomResponseDetailsTypeDef = TypedDict(
@@ -7455,16 +8947,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeActionTargetsResponseTypeDef = TypedDict(
     "DescribeActionTargetsResponseTypeDef",
     {
         "ActionTargets": List[ActionTargetTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeHubResponseTypeDef = TypedDict(
     "DescribeHubResponseTypeDef",
     {
         "HubArn": str,
         "SubscribedAt": str,
@@ -7510,32 +9002,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAutomationRulesResponseTypeDef = TypedDict(
     "ListAutomationRulesResponseTypeDef",
     {
         "AutomationRulesMetadata": List[AutomationRulesMetadataTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListEnabledProductsForImportResponseTypeDef = TypedDict(
     "ListEnabledProductsForImportResponseTypeDef",
     {
         "ProductSubscriptions": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
     "ListOrganizationAdminAccountsResponseTypeDef",
     {
         "AdminAccounts": List[AdminAccountTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -7588,16 +9080,16 @@
 )
 ListConfigurationPolicyAssociationsResponseTypeDef = TypedDict(
     "ListConfigurationPolicyAssociationsResponseTypeDef",
     {
         "ConfigurationPolicyAssociationSummaries": List[
             ConfigurationPolicyAssociationSummaryTypeDef
         ],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 BatchGetStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
     "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
     {
         "StandardsControlAssociationIds": Sequence[StandardsControlAssociationIdTypeDef],
     },
@@ -7629,39 +9121,58 @@
     "UnprocessedStandardsControlAssociationUpdateTypeDef",
     {
         "StandardsControlAssociationUpdate": StandardsControlAssociationUpdateTypeDef,
         "ErrorCode": UnprocessedErrorCodeType,
         "ErrorReason": NotRequired[str],
     },
 )
-VulnerabilityCodeVulnerabilitiesPaginatorTypeDef = TypedDict(
-    "VulnerabilityCodeVulnerabilitiesPaginatorTypeDef",
+VulnerabilityCodeVulnerabilitiesExtraOutputTypeDef = TypedDict(
+    "VulnerabilityCodeVulnerabilitiesExtraOutputTypeDef",
+    {
+        "Cwes": NotRequired[List[str]],
+        "FilePath": NotRequired[CodeVulnerabilitiesFilePathTypeDef],
+        "SourceArn": NotRequired[str],
+    },
+)
+VulnerabilityCodeVulnerabilitiesOutputTypeDef = TypedDict(
+    "VulnerabilityCodeVulnerabilitiesOutputTypeDef",
     {
         "Cwes": NotRequired[List[str]],
         "FilePath": NotRequired[CodeVulnerabilitiesFilePathTypeDef],
         "SourceArn": NotRequired[str],
     },
 )
 VulnerabilityCodeVulnerabilitiesTypeDef = TypedDict(
     "VulnerabilityCodeVulnerabilitiesTypeDef",
     {
         "Cwes": NotRequired[Sequence[str]],
         "FilePath": NotRequired[CodeVulnerabilitiesFilePathTypeDef],
         "SourceArn": NotRequired[str],
     },
 )
-CompliancePaginatorTypeDef = TypedDict(
-    "CompliancePaginatorTypeDef",
+ComplianceExtraOutputTypeDef = TypedDict(
+    "ComplianceExtraOutputTypeDef",
     {
         "Status": NotRequired[ComplianceStatusType],
         "RelatedRequirements": NotRequired[List[str]],
         "StatusReasons": NotRequired[List[StatusReasonTypeDef]],
         "SecurityControlId": NotRequired[str],
         "AssociatedStandards": NotRequired[List[AssociatedStandardTypeDef]],
-        "SecurityControlParameters": NotRequired[List[SecurityControlParameterPaginatorTypeDef]],
+        "SecurityControlParameters": NotRequired[List[SecurityControlParameterExtraOutputTypeDef]],
+    },
+)
+ComplianceOutputTypeDef = TypedDict(
+    "ComplianceOutputTypeDef",
+    {
+        "Status": NotRequired[ComplianceStatusType],
+        "RelatedRequirements": NotRequired[List[str]],
+        "StatusReasons": NotRequired[List[StatusReasonTypeDef]],
+        "SecurityControlId": NotRequired[str],
+        "AssociatedStandards": NotRequired[List[AssociatedStandardTypeDef]],
+        "SecurityControlParameters": NotRequired[List[SecurityControlParameterOutputTypeDef]],
     },
 )
 ComplianceTypeDef = TypedDict(
     "ComplianceTypeDef",
     {
         "Status": NotRequired[ComplianceStatusType],
         "RelatedRequirements": NotRequired[Sequence[str]],
@@ -7710,20 +9221,32 @@
         "Target": NotRequired[TargetTypeDef],
     },
 )
 ListConfigurationPoliciesResponseTypeDef = TypedDict(
     "ListConfigurationPoliciesResponseTypeDef",
     {
         "ConfigurationPolicySummaries": List[ConfigurationPolicySummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+ContainerDetailsExtraOutputTypeDef = TypedDict(
+    "ContainerDetailsExtraOutputTypeDef",
+    {
+        "ContainerRuntime": NotRequired[str],
+        "Name": NotRequired[str],
+        "ImageId": NotRequired[str],
+        "ImageName": NotRequired[str],
+        "LaunchedAt": NotRequired[str],
+        "VolumeMounts": NotRequired[List[VolumeMountTypeDef]],
+        "Privileged": NotRequired[bool],
     },
 )
-ContainerDetailsPaginatorTypeDef = TypedDict(
-    "ContainerDetailsPaginatorTypeDef",
+ContainerDetailsOutputTypeDef = TypedDict(
+    "ContainerDetailsOutputTypeDef",
     {
         "ContainerRuntime": NotRequired[str],
         "Name": NotRequired[str],
         "ImageId": NotRequired[str],
         "ImageName": NotRequired[str],
         "LaunchedAt": NotRequired[str],
         "VolumeMounts": NotRequired[List[VolumeMountTypeDef]],
@@ -7902,28 +9425,37 @@
         "OrganizationConfiguration": NotRequired[OrganizationConfigurationTypeDef],
     },
 )
 DescribeProductsResponseTypeDef = TypedDict(
     "DescribeProductsResponseTypeDef",
     {
         "Products": List[ProductTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeStandardsControlsResponseTypeDef = TypedDict(
     "DescribeStandardsControlsResponseTypeDef",
     {
         "Controls": List[StandardsControlTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-ThreatPaginatorTypeDef = TypedDict(
-    "ThreatPaginatorTypeDef",
+ThreatExtraOutputTypeDef = TypedDict(
+    "ThreatExtraOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "Severity": NotRequired[str],
+        "ItemCount": NotRequired[int],
+        "FilePaths": NotRequired[List[FilePathsTypeDef]],
+    },
+)
+ThreatOutputTypeDef = TypedDict(
+    "ThreatOutputTypeDef",
     {
         "Name": NotRequired[str],
         "Severity": NotRequired[str],
         "ItemCount": NotRequired[int],
         "FilePaths": NotRequired[List[FilePathsTypeDef]],
     },
 )
@@ -7936,31 +9468,41 @@
         "FilePaths": NotRequired[Sequence[FilePathsTypeDef]],
     },
 )
 ListFindingAggregatorsResponseTypeDef = TypedDict(
     "ListFindingAggregatorsResponseTypeDef",
     {
         "FindingAggregators": List[FindingAggregatorTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 FindingHistoryRecordTypeDef = TypedDict(
     "FindingHistoryRecordTypeDef",
     {
         "FindingIdentifier": NotRequired[AwsSecurityFindingIdentifierTypeDef],
         "UpdateTime": NotRequired[datetime],
         "FindingCreated": NotRequired[bool],
         "UpdateSource": NotRequired[FindingHistoryUpdateSourceTypeDef],
         "Updates": NotRequired[List[FindingHistoryUpdateTypeDef]],
         "NextToken": NotRequired[str],
     },
 )
-FindingProviderFieldsPaginatorTypeDef = TypedDict(
-    "FindingProviderFieldsPaginatorTypeDef",
+FindingProviderFieldsExtraOutputTypeDef = TypedDict(
+    "FindingProviderFieldsExtraOutputTypeDef",
+    {
+        "Confidence": NotRequired[int],
+        "Criticality": NotRequired[int],
+        "RelatedFindings": NotRequired[List[RelatedFindingTypeDef]],
+        "Severity": NotRequired[FindingProviderSeverityTypeDef],
+        "Types": NotRequired[List[str]],
+    },
+)
+FindingProviderFieldsOutputTypeDef = TypedDict(
+    "FindingProviderFieldsOutputTypeDef",
     {
         "Confidence": NotRequired[int],
         "Criticality": NotRequired[int],
         "RelatedFindings": NotRequired[List[RelatedFindingTypeDef]],
         "Severity": NotRequired[FindingProviderSeverityTypeDef],
         "Types": NotRequired[List[str]],
     },
@@ -7989,16 +9531,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
     "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
     {
         "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
         "StartTime": NotRequired[TimestampTypeDef],
@@ -8024,36 +9566,43 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 InsightResultsTypeDef = TypedDict(
     "InsightResultsTypeDef",
     {
         "InsightArn": str,
         "GroupByAttribute": str,
         "ResultValues": List[InsightResultValueTypeDef],
     },
 )
 ListStandardsControlAssociationsResponseTypeDef = TypedDict(
     "ListStandardsControlAssociationsResponseTypeDef",
     {
         "StandardsControlAssociationSummaries": List[StandardsControlAssociationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-NetworkPathComponentDetailsPaginatorTypeDef = TypedDict(
-    "NetworkPathComponentDetailsPaginatorTypeDef",
+NetworkPathComponentDetailsExtraOutputTypeDef = TypedDict(
+    "NetworkPathComponentDetailsExtraOutputTypeDef",
+    {
+        "Address": NotRequired[List[str]],
+        "PortRanges": NotRequired[List[PortRangeTypeDef]],
+    },
+)
+NetworkPathComponentDetailsOutputTypeDef = TypedDict(
+    "NetworkPathComponentDetailsOutputTypeDef",
     {
         "Address": NotRequired[List[str]],
         "PortRanges": NotRequired[List[PortRangeTypeDef]],
     },
 )
 NetworkPathComponentDetailsTypeDef = TypedDict(
     "NetworkPathComponentDetailsTypeDef",
@@ -8083,61 +9632,95 @@
     "PageTypeDef",
     {
         "PageNumber": NotRequired[int],
         "LineRange": NotRequired[RangeTypeDef],
         "OffsetRange": NotRequired[RangeTypeDef],
     },
 )
+ParameterConfigurationOutputTypeDef = TypedDict(
+    "ParameterConfigurationOutputTypeDef",
+    {
+        "ValueType": ParameterValueTypeType,
+        "Value": NotRequired[ParameterValueOutputTypeDef],
+    },
+)
 ParameterConfigurationTypeDef = TypedDict(
     "ParameterConfigurationTypeDef",
     {
         "ValueType": ParameterValueTypeType,
         "Value": NotRequired[ParameterValueTypeDef],
     },
 )
 RemediationTypeDef = TypedDict(
     "RemediationTypeDef",
     {
         "Recommendation": NotRequired[RecommendationTypeDef],
     },
 )
-RuleGroupSourceStatefulRulesDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceStatefulRulesDetailsPaginatorTypeDef",
+RuleGroupSourceStatefulRulesDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatefulRulesDetailsExtraOutputTypeDef",
     {
         "Action": NotRequired[str],
         "Header": NotRequired[RuleGroupSourceStatefulRulesHeaderDetailsTypeDef],
         "RuleOptions": NotRequired[
-            List[RuleGroupSourceStatefulRulesOptionsDetailsPaginatorTypeDef]
+            List[RuleGroupSourceStatefulRulesOptionsDetailsExtraOutputTypeDef]
         ],
     },
 )
+RuleGroupSourceStatefulRulesDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatefulRulesDetailsOutputTypeDef",
+    {
+        "Action": NotRequired[str],
+        "Header": NotRequired[RuleGroupSourceStatefulRulesHeaderDetailsTypeDef],
+        "RuleOptions": NotRequired[List[RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef]],
+    },
+)
 RuleGroupSourceStatefulRulesDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
     {
         "Action": NotRequired[str],
         "Header": NotRequired[RuleGroupSourceStatefulRulesHeaderDetailsTypeDef],
         "RuleOptions": NotRequired[Sequence[RuleGroupSourceStatefulRulesOptionsDetailsTypeDef]],
     },
 )
-RuleGroupSourceStatelessRuleMatchAttributesPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesPaginatorTypeDef",
+RuleGroupSourceStatelessRuleMatchAttributesExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesExtraOutputTypeDef",
     {
         "DestinationPorts": NotRequired[
             List[RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef]
         ],
         "Destinations": NotRequired[
             List[RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef]
         ],
         "Protocols": NotRequired[List[int]],
         "SourcePorts": NotRequired[
             List[RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef]
         ],
         "Sources": NotRequired[List[RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef]],
         "TcpFlags": NotRequired[
-            List[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsPaginatorTypeDef]
+            List[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsExtraOutputTypeDef]
+        ],
+    },
+)
+RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef",
+    {
+        "DestinationPorts": NotRequired[
+            List[RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef]
+        ],
+        "Destinations": NotRequired[
+            List[RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef]
+        ],
+        "Protocols": NotRequired[List[int]],
+        "SourcePorts": NotRequired[
+            List[RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef]
+        ],
+        "Sources": NotRequired[List[RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef]],
+        "TcpFlags": NotRequired[
+            List[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef]
         ],
     },
 )
 RuleGroupSourceStatelessRuleMatchAttributesTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
     {
         "DestinationPorts": NotRequired[
@@ -8152,19 +9735,26 @@
         ],
         "Sources": NotRequired[Sequence[RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef]],
         "TcpFlags": NotRequired[
             Sequence[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef]
         ],
     },
 )
-RuleGroupVariablesPaginatorTypeDef = TypedDict(
-    "RuleGroupVariablesPaginatorTypeDef",
+RuleGroupVariablesExtraOutputTypeDef = TypedDict(
+    "RuleGroupVariablesExtraOutputTypeDef",
+    {
+        "IpSets": NotRequired[RuleGroupVariablesIpSetsDetailsExtraOutputTypeDef],
+        "PortSets": NotRequired[RuleGroupVariablesPortSetsDetailsExtraOutputTypeDef],
+    },
+)
+RuleGroupVariablesOutputTypeDef = TypedDict(
+    "RuleGroupVariablesOutputTypeDef",
     {
-        "IpSets": NotRequired[RuleGroupVariablesIpSetsDetailsPaginatorTypeDef],
-        "PortSets": NotRequired[RuleGroupVariablesPortSetsDetailsPaginatorTypeDef],
+        "IpSets": NotRequired[RuleGroupVariablesIpSetsDetailsOutputTypeDef],
+        "PortSets": NotRequired[RuleGroupVariablesPortSetsDetailsOutputTypeDef],
     },
 )
 RuleGroupVariablesTypeDef = TypedDict(
     "RuleGroupVariablesTypeDef",
     {
         "IpSets": NotRequired[RuleGroupVariablesIpSetsDetailsTypeDef],
         "PortSets": NotRequired[RuleGroupVariablesPortSetsDetailsTypeDef],
@@ -8186,28 +9776,47 @@
         "StandardsSubscriptionArn": str,
         "StandardsArn": str,
         "StandardsInput": Dict[str, str],
         "StandardsStatus": StandardsStatusType,
         "StandardsStatusReason": NotRequired[StandardsStatusReasonTypeDef],
     },
 )
-StatelessCustomPublishMetricActionPaginatorTypeDef = TypedDict(
-    "StatelessCustomPublishMetricActionPaginatorTypeDef",
+StatelessCustomPublishMetricActionExtraOutputTypeDef = TypedDict(
+    "StatelessCustomPublishMetricActionExtraOutputTypeDef",
+    {
+        "Dimensions": NotRequired[List[StatelessCustomPublishMetricActionDimensionTypeDef]],
+    },
+)
+StatelessCustomPublishMetricActionOutputTypeDef = TypedDict(
+    "StatelessCustomPublishMetricActionOutputTypeDef",
     {
         "Dimensions": NotRequired[List[StatelessCustomPublishMetricActionDimensionTypeDef]],
     },
 )
 StatelessCustomPublishMetricActionTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionTypeDef",
     {
         "Dimensions": NotRequired[Sequence[StatelessCustomPublishMetricActionDimensionTypeDef]],
     },
 )
-AwsApiCallActionPaginatorTypeDef = TypedDict(
-    "AwsApiCallActionPaginatorTypeDef",
+AwsApiCallActionExtraOutputTypeDef = TypedDict(
+    "AwsApiCallActionExtraOutputTypeDef",
+    {
+        "Api": NotRequired[str],
+        "ServiceName": NotRequired[str],
+        "CallerType": NotRequired[str],
+        "RemoteIpDetails": NotRequired[ActionRemoteIpDetailsTypeDef],
+        "DomainDetails": NotRequired[AwsApiCallActionDomainDetailsTypeDef],
+        "AffectedResources": NotRequired[Dict[str, str]],
+        "FirstSeen": NotRequired[str],
+        "LastSeen": NotRequired[str],
+    },
+)
+AwsApiCallActionOutputTypeDef = TypedDict(
+    "AwsApiCallActionOutputTypeDef",
     {
         "Api": NotRequired[str],
         "ServiceName": NotRequired[str],
         "CallerType": NotRequired[str],
         "RemoteIpDetails": NotRequired[ActionRemoteIpDetailsTypeDef],
         "DomainDetails": NotRequired[AwsApiCallActionDomainDetailsTypeDef],
         "AffectedResources": NotRequired[Dict[str, str]],
@@ -8243,16 +9852,27 @@
     "PortProbeDetailTypeDef",
     {
         "LocalPortDetails": NotRequired[ActionLocalPortDetailsTypeDef],
         "LocalIpDetails": NotRequired[ActionLocalIpDetailsTypeDef],
         "RemoteIpDetails": NotRequired[ActionRemoteIpDetailsTypeDef],
     },
 )
-AwsEc2RouteTableDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2RouteTableDetailsPaginatorTypeDef",
+AwsEc2RouteTableDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2RouteTableDetailsExtraOutputTypeDef",
+    {
+        "AssociationSet": NotRequired[List[AssociationSetDetailsTypeDef]],
+        "OwnerId": NotRequired[str],
+        "PropagatingVgwSet": NotRequired[List[PropagatingVgwSetDetailsTypeDef]],
+        "RouteTableId": NotRequired[str],
+        "RouteSet": NotRequired[List[RouteSetDetailsTypeDef]],
+        "VpcId": NotRequired[str],
+    },
+)
+AwsEc2RouteTableDetailsOutputTypeDef = TypedDict(
+    "AwsEc2RouteTableDetailsOutputTypeDef",
     {
         "AssociationSet": NotRequired[List[AssociationSetDetailsTypeDef]],
         "OwnerId": NotRequired[str],
         "PropagatingVgwSet": NotRequired[List[PropagatingVgwSetDetailsTypeDef]],
         "RouteTableId": NotRequired[str],
         "RouteSet": NotRequired[List[RouteSetDetailsTypeDef]],
         "VpcId": NotRequired[str],
@@ -8265,48 +9885,80 @@
         "OwnerId": NotRequired[str],
         "PropagatingVgwSet": NotRequired[Sequence[PropagatingVgwSetDetailsTypeDef]],
         "RouteTableId": NotRequired[str],
         "RouteSet": NotRequired[Sequence[RouteSetDetailsTypeDef]],
         "VpcId": NotRequired[str],
     },
 )
+AutomationRulesActionOutputTypeDef = TypedDict(
+    "AutomationRulesActionOutputTypeDef",
+    {
+        "Type": NotRequired[Literal["FINDING_FIELDS_UPDATE"]],
+        "FindingFieldsUpdate": NotRequired[AutomationRulesFindingFieldsUpdateOutputTypeDef],
+    },
+)
 AutomationRulesActionTypeDef = TypedDict(
     "AutomationRulesActionTypeDef",
     {
         "Type": NotRequired[Literal["FINDING_FIELDS_UPDATE"]],
         "FindingFieldsUpdate": NotRequired[AutomationRulesFindingFieldsUpdateTypeDef],
     },
 )
-AwsAmazonMqBrokerDetailsPaginatorTypeDef = TypedDict(
-    "AwsAmazonMqBrokerDetailsPaginatorTypeDef",
+AwsAmazonMqBrokerDetailsExtraOutputTypeDef = TypedDict(
+    "AwsAmazonMqBrokerDetailsExtraOutputTypeDef",
     {
         "AuthenticationStrategy": NotRequired[str],
         "AutoMinorVersionUpgrade": NotRequired[bool],
         "BrokerArn": NotRequired[str],
         "BrokerName": NotRequired[str],
         "DeploymentMode": NotRequired[str],
         "EncryptionOptions": NotRequired[AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef],
         "EngineType": NotRequired[str],
         "EngineVersion": NotRequired[str],
         "HostInstanceType": NotRequired[str],
         "BrokerId": NotRequired[str],
         "LdapServerMetadata": NotRequired[
-            AwsAmazonMqBrokerLdapServerMetadataDetailsPaginatorTypeDef
+            AwsAmazonMqBrokerLdapServerMetadataDetailsExtraOutputTypeDef
         ],
         "Logs": NotRequired[AwsAmazonMqBrokerLogsDetailsTypeDef],
         "MaintenanceWindowStartTime": NotRequired[
             AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef
         ],
         "PubliclyAccessible": NotRequired[bool],
         "SecurityGroups": NotRequired[List[str]],
         "StorageType": NotRequired[str],
         "SubnetIds": NotRequired[List[str]],
         "Users": NotRequired[List[AwsAmazonMqBrokerUsersDetailsTypeDef]],
     },
 )
+AwsAmazonMqBrokerDetailsOutputTypeDef = TypedDict(
+    "AwsAmazonMqBrokerDetailsOutputTypeDef",
+    {
+        "AuthenticationStrategy": NotRequired[str],
+        "AutoMinorVersionUpgrade": NotRequired[bool],
+        "BrokerArn": NotRequired[str],
+        "BrokerName": NotRequired[str],
+        "DeploymentMode": NotRequired[str],
+        "EncryptionOptions": NotRequired[AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef],
+        "EngineType": NotRequired[str],
+        "EngineVersion": NotRequired[str],
+        "HostInstanceType": NotRequired[str],
+        "BrokerId": NotRequired[str],
+        "LdapServerMetadata": NotRequired[AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef],
+        "Logs": NotRequired[AwsAmazonMqBrokerLogsDetailsTypeDef],
+        "MaintenanceWindowStartTime": NotRequired[
+            AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef
+        ],
+        "PubliclyAccessible": NotRequired[bool],
+        "SecurityGroups": NotRequired[List[str]],
+        "StorageType": NotRequired[str],
+        "SubnetIds": NotRequired[List[str]],
+        "Users": NotRequired[List[AwsAmazonMqBrokerUsersDetailsTypeDef]],
+    },
+)
 AwsAmazonMqBrokerDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerDetailsTypeDef",
     {
         "AuthenticationStrategy": NotRequired[str],
         "AutoMinorVersionUpgrade": NotRequired[bool],
         "BrokerArn": NotRequired[str],
         "BrokerName": NotRequired[str],
@@ -8324,16 +9976,37 @@
         "PubliclyAccessible": NotRequired[bool],
         "SecurityGroups": NotRequired[Sequence[str]],
         "StorageType": NotRequired[str],
         "SubnetIds": NotRequired[Sequence[str]],
         "Users": NotRequired[Sequence[AwsAmazonMqBrokerUsersDetailsTypeDef]],
     },
 )
-AwsAppSyncGraphQlApiDetailsPaginatorTypeDef = TypedDict(
-    "AwsAppSyncGraphQlApiDetailsPaginatorTypeDef",
+AwsAppSyncGraphQlApiDetailsExtraOutputTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiDetailsExtraOutputTypeDef",
+    {
+        "ApiId": NotRequired[str],
+        "Id": NotRequired[str],
+        "OpenIdConnectConfig": NotRequired[AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef],
+        "Name": NotRequired[str],
+        "LambdaAuthorizerConfig": NotRequired[
+            AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef
+        ],
+        "XrayEnabled": NotRequired[bool],
+        "Arn": NotRequired[str],
+        "UserPoolConfig": NotRequired[AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef],
+        "AuthenticationType": NotRequired[str],
+        "LogConfig": NotRequired[AwsAppSyncGraphQlApiLogConfigDetailsTypeDef],
+        "AdditionalAuthenticationProviders": NotRequired[
+            List[AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef]
+        ],
+        "WafWebAclArn": NotRequired[str],
+    },
+)
+AwsAppSyncGraphQlApiDetailsOutputTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiDetailsOutputTypeDef",
     {
         "ApiId": NotRequired[str],
         "Id": NotRequired[str],
         "OpenIdConnectConfig": NotRequired[AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef],
         "Name": NotRequired[str],
         "LambdaAuthorizerConfig": NotRequired[
             AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef
@@ -8374,38 +10047,77 @@
     "AwsAthenaWorkGroupConfigurationDetailsTypeDef",
     {
         "ResultConfiguration": NotRequired[
             AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef
         ],
     },
 )
-AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsPaginatorTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsPaginatorTypeDef",
+AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsExtraOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsExtraOutputTypeDef",
     {
         "InstancesDistribution": NotRequired[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
         ],
         "LaunchTemplate": NotRequired[
-            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsPaginatorTypeDef
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef",
+    {
+        "InstancesDistribution": NotRequired[
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
+        ],
+        "LaunchTemplate": NotRequired[
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef
         ],
     },
 )
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     {
         "InstancesDistribution": NotRequired[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
         ],
         "LaunchTemplate": NotRequired[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef
         ],
     },
 )
-AwsAutoScalingLaunchConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsAutoScalingLaunchConfigurationDetailsPaginatorTypeDef",
+AwsAutoScalingLaunchConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsAutoScalingLaunchConfigurationDetailsExtraOutputTypeDef",
+    {
+        "AssociatePublicIpAddress": NotRequired[bool],
+        "BlockDeviceMappings": NotRequired[
+            List[AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef]
+        ],
+        "ClassicLinkVpcId": NotRequired[str],
+        "ClassicLinkVpcSecurityGroups": NotRequired[List[str]],
+        "CreatedTime": NotRequired[str],
+        "EbsOptimized": NotRequired[bool],
+        "IamInstanceProfile": NotRequired[str],
+        "ImageId": NotRequired[str],
+        "InstanceMonitoring": NotRequired[
+            AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef
+        ],
+        "InstanceType": NotRequired[str],
+        "KernelId": NotRequired[str],
+        "KeyName": NotRequired[str],
+        "LaunchConfigurationName": NotRequired[str],
+        "PlacementTenancy": NotRequired[str],
+        "RamdiskId": NotRequired[str],
+        "SecurityGroups": NotRequired[List[str]],
+        "SpotPrice": NotRequired[str],
+        "UserData": NotRequired[str],
+        "MetadataOptions": NotRequired[AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef],
+    },
+)
+AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef",
     {
         "AssociatePublicIpAddress": NotRequired[bool],
         "BlockDeviceMappings": NotRequired[
             List[AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef]
         ],
         "ClassicLinkVpcId": NotRequired[str],
         "ClassicLinkVpcSecurityGroups": NotRequired[List[str]],
@@ -8452,16 +10164,30 @@
         "RamdiskId": NotRequired[str],
         "SecurityGroups": NotRequired[Sequence[str]],
         "SpotPrice": NotRequired[str],
         "UserData": NotRequired[str],
         "MetadataOptions": NotRequired[AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef],
     },
 )
-AwsBackupBackupPlanRuleDetailsPaginatorTypeDef = TypedDict(
-    "AwsBackupBackupPlanRuleDetailsPaginatorTypeDef",
+AwsBackupBackupPlanRuleDetailsExtraOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanRuleDetailsExtraOutputTypeDef",
+    {
+        "TargetBackupVault": NotRequired[str],
+        "StartWindowMinutes": NotRequired[int],
+        "ScheduleExpression": NotRequired[str],
+        "RuleName": NotRequired[str],
+        "RuleId": NotRequired[str],
+        "EnableContinuousBackup": NotRequired[bool],
+        "CompletionWindowMinutes": NotRequired[int],
+        "CopyActions": NotRequired[List[AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef]],
+        "Lifecycle": NotRequired[AwsBackupBackupPlanLifecycleDetailsTypeDef],
+    },
+)
+AwsBackupBackupPlanRuleDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanRuleDetailsOutputTypeDef",
     {
         "TargetBackupVault": NotRequired[str],
         "StartWindowMinutes": NotRequired[int],
         "ScheduleExpression": NotRequired[str],
         "RuleName": NotRequired[str],
         "RuleId": NotRequired[str],
         "EnableContinuousBackup": NotRequired[bool],
@@ -8480,19 +10206,30 @@
         "RuleId": NotRequired[str],
         "EnableContinuousBackup": NotRequired[bool],
         "CompletionWindowMinutes": NotRequired[int],
         "CopyActions": NotRequired[Sequence[AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef]],
         "Lifecycle": NotRequired[AwsBackupBackupPlanLifecycleDetailsTypeDef],
     },
 )
-AwsCertificateManagerCertificateRenewalSummaryPaginatorTypeDef = TypedDict(
-    "AwsCertificateManagerCertificateRenewalSummaryPaginatorTypeDef",
+AwsCertificateManagerCertificateRenewalSummaryExtraOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateRenewalSummaryExtraOutputTypeDef",
     {
         "DomainValidationOptions": NotRequired[
-            List[AwsCertificateManagerCertificateDomainValidationOptionPaginatorTypeDef]
+            List[AwsCertificateManagerCertificateDomainValidationOptionExtraOutputTypeDef]
+        ],
+        "RenewalStatus": NotRequired[str],
+        "RenewalStatusReason": NotRequired[str],
+        "UpdatedAt": NotRequired[str],
+    },
+)
+AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef",
+    {
+        "DomainValidationOptions": NotRequired[
+            List[AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef]
         ],
         "RenewalStatus": NotRequired[str],
         "RenewalStatusReason": NotRequired[str],
         "UpdatedAt": NotRequired[str],
     },
 )
 AwsCertificateManagerCertificateRenewalSummaryTypeDef = TypedDict(
@@ -8502,61 +10239,93 @@
             Sequence[AwsCertificateManagerCertificateDomainValidationOptionTypeDef]
         ],
         "RenewalStatus": NotRequired[str],
         "RenewalStatusReason": NotRequired[str],
         "UpdatedAt": NotRequired[str],
     },
 )
-AwsCloudFrontDistributionOriginItemPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginItemPaginatorTypeDef",
+AwsCloudFrontDistributionOriginItemExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginItemExtraOutputTypeDef",
     {
         "DomainName": NotRequired[str],
         "Id": NotRequired[str],
         "OriginPath": NotRequired[str],
         "S3OriginConfig": NotRequired[AwsCloudFrontDistributionOriginS3OriginConfigTypeDef],
         "CustomOriginConfig": NotRequired[
-            AwsCloudFrontDistributionOriginCustomOriginConfigPaginatorTypeDef
+            AwsCloudFrontDistributionOriginCustomOriginConfigExtraOutputTypeDef
+        ],
+    },
+)
+AwsCloudFrontDistributionOriginItemOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginItemOutputTypeDef",
+    {
+        "DomainName": NotRequired[str],
+        "Id": NotRequired[str],
+        "OriginPath": NotRequired[str],
+        "S3OriginConfig": NotRequired[AwsCloudFrontDistributionOriginS3OriginConfigTypeDef],
+        "CustomOriginConfig": NotRequired[
+            AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef
         ],
     },
 )
 AwsCloudFrontDistributionOriginItemTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginItemTypeDef",
     {
         "DomainName": NotRequired[str],
         "Id": NotRequired[str],
         "OriginPath": NotRequired[str],
         "S3OriginConfig": NotRequired[AwsCloudFrontDistributionOriginS3OriginConfigTypeDef],
         "CustomOriginConfig": NotRequired[AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef],
     },
 )
-AwsCloudFrontDistributionOriginGroupPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginGroupPaginatorTypeDef",
+AwsCloudFrontDistributionOriginGroupExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupExtraOutputTypeDef",
     {
         "FailoverCriteria": NotRequired[
-            AwsCloudFrontDistributionOriginGroupFailoverPaginatorTypeDef
+            AwsCloudFrontDistributionOriginGroupFailoverExtraOutputTypeDef
         ],
     },
 )
+AwsCloudFrontDistributionOriginGroupOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupOutputTypeDef",
+    {
+        "FailoverCriteria": NotRequired[AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef],
+    },
+)
 AwsCloudFrontDistributionOriginGroupTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupTypeDef",
     {
         "FailoverCriteria": NotRequired[AwsCloudFrontDistributionOriginGroupFailoverTypeDef],
     },
 )
-AwsCodeBuildProjectDetailsPaginatorTypeDef = TypedDict(
-    "AwsCodeBuildProjectDetailsPaginatorTypeDef",
+AwsCodeBuildProjectDetailsExtraOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectDetailsExtraOutputTypeDef",
+    {
+        "EncryptionKey": NotRequired[str],
+        "Artifacts": NotRequired[List[AwsCodeBuildProjectArtifactsDetailsTypeDef]],
+        "Environment": NotRequired[AwsCodeBuildProjectEnvironmentExtraOutputTypeDef],
+        "Name": NotRequired[str],
+        "Source": NotRequired[AwsCodeBuildProjectSourceTypeDef],
+        "ServiceRole": NotRequired[str],
+        "LogsConfig": NotRequired[AwsCodeBuildProjectLogsConfigDetailsTypeDef],
+        "VpcConfig": NotRequired[AwsCodeBuildProjectVpcConfigExtraOutputTypeDef],
+        "SecondaryArtifacts": NotRequired[List[AwsCodeBuildProjectArtifactsDetailsTypeDef]],
+    },
+)
+AwsCodeBuildProjectDetailsOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectDetailsOutputTypeDef",
     {
         "EncryptionKey": NotRequired[str],
         "Artifacts": NotRequired[List[AwsCodeBuildProjectArtifactsDetailsTypeDef]],
-        "Environment": NotRequired[AwsCodeBuildProjectEnvironmentPaginatorTypeDef],
+        "Environment": NotRequired[AwsCodeBuildProjectEnvironmentOutputTypeDef],
         "Name": NotRequired[str],
         "Source": NotRequired[AwsCodeBuildProjectSourceTypeDef],
         "ServiceRole": NotRequired[str],
         "LogsConfig": NotRequired[AwsCodeBuildProjectLogsConfigDetailsTypeDef],
-        "VpcConfig": NotRequired[AwsCodeBuildProjectVpcConfigPaginatorTypeDef],
+        "VpcConfig": NotRequired[AwsCodeBuildProjectVpcConfigOutputTypeDef],
         "SecondaryArtifacts": NotRequired[List[AwsCodeBuildProjectArtifactsDetailsTypeDef]],
     },
 )
 AwsCodeBuildProjectDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectDetailsTypeDef",
     {
         "EncryptionKey": NotRequired[str],
@@ -8566,16 +10335,31 @@
         "Source": NotRequired[AwsCodeBuildProjectSourceTypeDef],
         "ServiceRole": NotRequired[str],
         "LogsConfig": NotRequired[AwsCodeBuildProjectLogsConfigDetailsTypeDef],
         "VpcConfig": NotRequired[AwsCodeBuildProjectVpcConfigTypeDef],
         "SecondaryArtifacts": NotRequired[Sequence[AwsCodeBuildProjectArtifactsDetailsTypeDef]],
     },
 )
-AwsDynamoDbTableReplicaPaginatorTypeDef = TypedDict(
-    "AwsDynamoDbTableReplicaPaginatorTypeDef",
+AwsDynamoDbTableReplicaExtraOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableReplicaExtraOutputTypeDef",
+    {
+        "GlobalSecondaryIndexes": NotRequired[
+            List[AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef]
+        ],
+        "KmsMasterKeyId": NotRequired[str],
+        "ProvisionedThroughputOverride": NotRequired[
+            AwsDynamoDbTableProvisionedThroughputOverrideTypeDef
+        ],
+        "RegionName": NotRequired[str],
+        "ReplicaStatus": NotRequired[str],
+        "ReplicaStatusDescription": NotRequired[str],
+    },
+)
+AwsDynamoDbTableReplicaOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableReplicaOutputTypeDef",
     {
         "GlobalSecondaryIndexes": NotRequired[
             List[AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef]
         ],
         "KmsMasterKeyId": NotRequired[str],
         "ProvisionedThroughputOverride": NotRequired[
             AwsDynamoDbTableProvisionedThroughputOverrideTypeDef
@@ -8596,16 +10380,45 @@
             AwsDynamoDbTableProvisionedThroughputOverrideTypeDef
         ],
         "RegionName": NotRequired[str],
         "ReplicaStatus": NotRequired[str],
         "ReplicaStatusDescription": NotRequired[str],
     },
 )
-AwsEc2ClientVpnEndpointDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2ClientVpnEndpointDetailsPaginatorTypeDef",
+AwsEc2ClientVpnEndpointDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2ClientVpnEndpointDetailsExtraOutputTypeDef",
+    {
+        "ClientVpnEndpointId": NotRequired[str],
+        "Description": NotRequired[str],
+        "ClientCidrBlock": NotRequired[str],
+        "DnsServer": NotRequired[List[str]],
+        "SplitTunnel": NotRequired[bool],
+        "TransportProtocol": NotRequired[str],
+        "VpnPort": NotRequired[int],
+        "ServerCertificateArn": NotRequired[str],
+        "AuthenticationOptions": NotRequired[
+            List[AwsEc2ClientVpnEndpointAuthenticationOptionsDetailsTypeDef]
+        ],
+        "ConnectionLogOptions": NotRequired[
+            AwsEc2ClientVpnEndpointConnectionLogOptionsDetailsTypeDef
+        ],
+        "SecurityGroupIdSet": NotRequired[List[str]],
+        "VpcId": NotRequired[str],
+        "SelfServicePortalUrl": NotRequired[str],
+        "ClientConnectOptions": NotRequired[
+            AwsEc2ClientVpnEndpointClientConnectOptionsDetailsTypeDef
+        ],
+        "SessionTimeoutHours": NotRequired[int],
+        "ClientLoginBannerOptions": NotRequired[
+            AwsEc2ClientVpnEndpointClientLoginBannerOptionsDetailsTypeDef
+        ],
+    },
+)
+AwsEc2ClientVpnEndpointDetailsOutputTypeDef = TypedDict(
+    "AwsEc2ClientVpnEndpointDetailsOutputTypeDef",
     {
         "ClientVpnEndpointId": NotRequired[str],
         "Description": NotRequired[str],
         "ClientCidrBlock": NotRequired[str],
         "DnsServer": NotRequired[List[str]],
         "SplitTunnel": NotRequired[bool],
         "TransportProtocol": NotRequired[str],
@@ -8654,16 +10467,69 @@
         ],
         "SessionTimeoutHours": NotRequired[int],
         "ClientLoginBannerOptions": NotRequired[
             AwsEc2ClientVpnEndpointClientLoginBannerOptionsDetailsTypeDef
         ],
     },
 )
-AwsEc2LaunchTemplateDataDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataDetailsPaginatorTypeDef",
+AwsEc2LaunchTemplateDataDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataDetailsExtraOutputTypeDef",
+    {
+        "BlockDeviceMappingSet": NotRequired[
+            List[AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef]
+        ],
+        "CapacityReservationSpecification": NotRequired[
+            AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef
+        ],
+        "CpuOptions": NotRequired[AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef],
+        "CreditSpecification": NotRequired[
+            AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef
+        ],
+        "DisableApiStop": NotRequired[bool],
+        "DisableApiTermination": NotRequired[bool],
+        "EbsOptimized": NotRequired[bool],
+        "ElasticGpuSpecificationSet": NotRequired[
+            List[AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef]
+        ],
+        "ElasticInferenceAcceleratorSet": NotRequired[
+            List[AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef]
+        ],
+        "EnclaveOptions": NotRequired[AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef],
+        "HibernationOptions": NotRequired[AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef],
+        "IamInstanceProfile": NotRequired[AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef],
+        "ImageId": NotRequired[str],
+        "InstanceInitiatedShutdownBehavior": NotRequired[str],
+        "InstanceMarketOptions": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef
+        ],
+        "InstanceRequirements": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsDetailsExtraOutputTypeDef
+        ],
+        "InstanceType": NotRequired[str],
+        "KernelId": NotRequired[str],
+        "KeyName": NotRequired[str],
+        "LicenseSet": NotRequired[List[AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef]],
+        "MaintenanceOptions": NotRequired[AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef],
+        "MetadataOptions": NotRequired[AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef],
+        "Monitoring": NotRequired[AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef],
+        "NetworkInterfaceSet": NotRequired[
+            List[AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsExtraOutputTypeDef]
+        ],
+        "Placement": NotRequired[AwsEc2LaunchTemplateDataPlacementDetailsTypeDef],
+        "PrivateDnsNameOptions": NotRequired[
+            AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef
+        ],
+        "RamDiskId": NotRequired[str],
+        "SecurityGroupIdSet": NotRequired[List[str]],
+        "SecurityGroupSet": NotRequired[List[str]],
+        "UserData": NotRequired[str],
+    },
+)
+AwsEc2LaunchTemplateDataDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataDetailsOutputTypeDef",
     {
         "BlockDeviceMappingSet": NotRequired[
             List[AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef]
         ],
         "CapacityReservationSpecification": NotRequired[
             AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef
         ],
@@ -8685,25 +10551,25 @@
         "IamInstanceProfile": NotRequired[AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef],
         "ImageId": NotRequired[str],
         "InstanceInitiatedShutdownBehavior": NotRequired[str],
         "InstanceMarketOptions": NotRequired[
             AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef
         ],
         "InstanceRequirements": NotRequired[
-            AwsEc2LaunchTemplateDataInstanceRequirementsDetailsPaginatorTypeDef
+            AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef
         ],
         "InstanceType": NotRequired[str],
         "KernelId": NotRequired[str],
         "KeyName": NotRequired[str],
         "LicenseSet": NotRequired[List[AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef]],
         "MaintenanceOptions": NotRequired[AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef],
         "MetadataOptions": NotRequired[AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef],
         "Monitoring": NotRequired[AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef],
         "NetworkInterfaceSet": NotRequired[
-            List[AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsPaginatorTypeDef]
+            List[AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef]
         ],
         "Placement": NotRequired[AwsEc2LaunchTemplateDataPlacementDetailsTypeDef],
         "PrivateDnsNameOptions": NotRequired[
             AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef
         ],
         "RamDiskId": NotRequired[str],
         "SecurityGroupIdSet": NotRequired[List[str]],
@@ -8760,16 +10626,27 @@
         ],
         "RamDiskId": NotRequired[str],
         "SecurityGroupIdSet": NotRequired[Sequence[str]],
         "SecurityGroupSet": NotRequired[Sequence[str]],
         "UserData": NotRequired[str],
     },
 )
-AwsEc2NetworkAclDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2NetworkAclDetailsPaginatorTypeDef",
+AwsEc2NetworkAclDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2NetworkAclDetailsExtraOutputTypeDef",
+    {
+        "IsDefault": NotRequired[bool],
+        "NetworkAclId": NotRequired[str],
+        "OwnerId": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "Associations": NotRequired[List[AwsEc2NetworkAclAssociationTypeDef]],
+        "Entries": NotRequired[List[AwsEc2NetworkAclEntryTypeDef]],
+    },
+)
+AwsEc2NetworkAclDetailsOutputTypeDef = TypedDict(
+    "AwsEc2NetworkAclDetailsOutputTypeDef",
     {
         "IsDefault": NotRequired[bool],
         "NetworkAclId": NotRequired[str],
         "OwnerId": NotRequired[str],
         "VpcId": NotRequired[str],
         "Associations": NotRequired[List[AwsEc2NetworkAclAssociationTypeDef]],
         "Entries": NotRequired[List[AwsEc2NetworkAclEntryTypeDef]],
@@ -8782,68 +10659,105 @@
         "NetworkAclId": NotRequired[str],
         "OwnerId": NotRequired[str],
         "VpcId": NotRequired[str],
         "Associations": NotRequired[Sequence[AwsEc2NetworkAclAssociationTypeDef]],
         "Entries": NotRequired[Sequence[AwsEc2NetworkAclEntryTypeDef]],
     },
 )
-AwsEc2SecurityGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2SecurityGroupDetailsPaginatorTypeDef",
+AwsEc2SecurityGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2SecurityGroupDetailsExtraOutputTypeDef",
     {
         "GroupName": NotRequired[str],
         "GroupId": NotRequired[str],
         "OwnerId": NotRequired[str],
         "VpcId": NotRequired[str],
-        "IpPermissions": NotRequired[List[AwsEc2SecurityGroupIpPermissionPaginatorTypeDef]],
-        "IpPermissionsEgress": NotRequired[List[AwsEc2SecurityGroupIpPermissionPaginatorTypeDef]],
+        "IpPermissions": NotRequired[List[AwsEc2SecurityGroupIpPermissionExtraOutputTypeDef]],
+        "IpPermissionsEgress": NotRequired[List[AwsEc2SecurityGroupIpPermissionExtraOutputTypeDef]],
+    },
+)
+AwsEc2SecurityGroupDetailsOutputTypeDef = TypedDict(
+    "AwsEc2SecurityGroupDetailsOutputTypeDef",
+    {
+        "GroupName": NotRequired[str],
+        "GroupId": NotRequired[str],
+        "OwnerId": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "IpPermissions": NotRequired[List[AwsEc2SecurityGroupIpPermissionOutputTypeDef]],
+        "IpPermissionsEgress": NotRequired[List[AwsEc2SecurityGroupIpPermissionOutputTypeDef]],
     },
 )
 AwsEc2SecurityGroupDetailsTypeDef = TypedDict(
     "AwsEc2SecurityGroupDetailsTypeDef",
     {
         "GroupName": NotRequired[str],
         "GroupId": NotRequired[str],
         "OwnerId": NotRequired[str],
         "VpcId": NotRequired[str],
         "IpPermissions": NotRequired[Sequence[AwsEc2SecurityGroupIpPermissionTypeDef]],
         "IpPermissionsEgress": NotRequired[Sequence[AwsEc2SecurityGroupIpPermissionTypeDef]],
     },
 )
-AwsEc2VpcPeeringConnectionDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VpcPeeringConnectionDetailsPaginatorTypeDef",
+AwsEc2VpcPeeringConnectionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VpcPeeringConnectionDetailsExtraOutputTypeDef",
+    {
+        "AccepterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsExtraOutputTypeDef],
+        "ExpirationTime": NotRequired[str],
+        "RequesterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsExtraOutputTypeDef],
+        "Status": NotRequired[AwsEc2VpcPeeringConnectionStatusDetailsTypeDef],
+        "VpcPeeringConnectionId": NotRequired[str],
+    },
+)
+AwsEc2VpcPeeringConnectionDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcPeeringConnectionDetailsOutputTypeDef",
     {
-        "AccepterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsPaginatorTypeDef],
+        "AccepterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef],
         "ExpirationTime": NotRequired[str],
-        "RequesterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsPaginatorTypeDef],
+        "RequesterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef],
         "Status": NotRequired[AwsEc2VpcPeeringConnectionStatusDetailsTypeDef],
         "VpcPeeringConnectionId": NotRequired[str],
     },
 )
 AwsEc2VpcPeeringConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
     {
         "AccepterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef],
         "ExpirationTime": NotRequired[str],
         "RequesterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef],
         "Status": NotRequired[AwsEc2VpcPeeringConnectionStatusDetailsTypeDef],
         "VpcPeeringConnectionId": NotRequired[str],
     },
 )
-AwsEc2VpnConnectionDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VpnConnectionDetailsPaginatorTypeDef",
+AwsEc2VpnConnectionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionDetailsExtraOutputTypeDef",
     {
         "VpnConnectionId": NotRequired[str],
         "State": NotRequired[str],
         "CustomerGatewayId": NotRequired[str],
         "CustomerGatewayConfiguration": NotRequired[str],
         "Type": NotRequired[str],
         "VpnGatewayId": NotRequired[str],
         "Category": NotRequired[str],
         "VgwTelemetry": NotRequired[List[AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef]],
-        "Options": NotRequired[AwsEc2VpnConnectionOptionsDetailsPaginatorTypeDef],
+        "Options": NotRequired[AwsEc2VpnConnectionOptionsDetailsExtraOutputTypeDef],
+        "Routes": NotRequired[List[AwsEc2VpnConnectionRoutesDetailsTypeDef]],
+        "TransitGatewayId": NotRequired[str],
+    },
+)
+AwsEc2VpnConnectionDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionDetailsOutputTypeDef",
+    {
+        "VpnConnectionId": NotRequired[str],
+        "State": NotRequired[str],
+        "CustomerGatewayId": NotRequired[str],
+        "CustomerGatewayConfiguration": NotRequired[str],
+        "Type": NotRequired[str],
+        "VpnGatewayId": NotRequired[str],
+        "Category": NotRequired[str],
+        "VgwTelemetry": NotRequired[List[AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef]],
+        "Options": NotRequired[AwsEc2VpnConnectionOptionsDetailsOutputTypeDef],
         "Routes": NotRequired[List[AwsEc2VpnConnectionRoutesDetailsTypeDef]],
         "TransitGatewayId": NotRequired[str],
     },
 )
 AwsEc2VpnConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionDetailsTypeDef",
     {
@@ -8864,16 +10778,16 @@
     "AwsEcsClusterConfigurationDetailsTypeDef",
     {
         "ExecuteCommandConfiguration": NotRequired[
             AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef
         ],
     },
 )
-AwsEcsServiceDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsServiceDetailsPaginatorTypeDef",
+AwsEcsServiceDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsServiceDetailsExtraOutputTypeDef",
     {
         "CapacityProviderStrategy": NotRequired[
             List[AwsEcsServiceCapacityProviderStrategyDetailsTypeDef]
         ],
         "Cluster": NotRequired[str],
         "DeploymentConfiguration": NotRequired[AwsEcsServiceDeploymentConfigurationDetailsTypeDef],
         "DeploymentController": NotRequired[AwsEcsServiceDeploymentControllerDetailsTypeDef],
@@ -8881,16 +10795,45 @@
         "EnableEcsManagedTags": NotRequired[bool],
         "EnableExecuteCommand": NotRequired[bool],
         "HealthCheckGracePeriodSeconds": NotRequired[int],
         "LaunchType": NotRequired[str],
         "LoadBalancers": NotRequired[List[AwsEcsServiceLoadBalancersDetailsTypeDef]],
         "Name": NotRequired[str],
         "NetworkConfiguration": NotRequired[
-            AwsEcsServiceNetworkConfigurationDetailsPaginatorTypeDef
+            AwsEcsServiceNetworkConfigurationDetailsExtraOutputTypeDef
+        ],
+        "PlacementConstraints": NotRequired[List[AwsEcsServicePlacementConstraintsDetailsTypeDef]],
+        "PlacementStrategies": NotRequired[List[AwsEcsServicePlacementStrategiesDetailsTypeDef]],
+        "PlatformVersion": NotRequired[str],
+        "PropagateTags": NotRequired[str],
+        "Role": NotRequired[str],
+        "SchedulingStrategy": NotRequired[str],
+        "ServiceArn": NotRequired[str],
+        "ServiceName": NotRequired[str],
+        "ServiceRegistries": NotRequired[List[AwsEcsServiceServiceRegistriesDetailsTypeDef]],
+        "TaskDefinition": NotRequired[str],
+    },
+)
+AwsEcsServiceDetailsOutputTypeDef = TypedDict(
+    "AwsEcsServiceDetailsOutputTypeDef",
+    {
+        "CapacityProviderStrategy": NotRequired[
+            List[AwsEcsServiceCapacityProviderStrategyDetailsTypeDef]
         ],
+        "Cluster": NotRequired[str],
+        "DeploymentConfiguration": NotRequired[AwsEcsServiceDeploymentConfigurationDetailsTypeDef],
+        "DeploymentController": NotRequired[AwsEcsServiceDeploymentControllerDetailsTypeDef],
+        "DesiredCount": NotRequired[int],
+        "EnableEcsManagedTags": NotRequired[bool],
+        "EnableExecuteCommand": NotRequired[bool],
+        "HealthCheckGracePeriodSeconds": NotRequired[int],
+        "LaunchType": NotRequired[str],
+        "LoadBalancers": NotRequired[List[AwsEcsServiceLoadBalancersDetailsTypeDef]],
+        "Name": NotRequired[str],
+        "NetworkConfiguration": NotRequired[AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef],
         "PlacementConstraints": NotRequired[List[AwsEcsServicePlacementConstraintsDetailsTypeDef]],
         "PlacementStrategies": NotRequired[List[AwsEcsServicePlacementStrategiesDetailsTypeDef]],
         "PlatformVersion": NotRequired[str],
         "PropagateTags": NotRequired[str],
         "Role": NotRequired[str],
         "SchedulingStrategy": NotRequired[str],
         "ServiceArn": NotRequired[str],
@@ -8928,16 +10871,88 @@
         "SchedulingStrategy": NotRequired[str],
         "ServiceArn": NotRequired[str],
         "ServiceName": NotRequired[str],
         "ServiceRegistries": NotRequired[Sequence[AwsEcsServiceServiceRegistriesDetailsTypeDef]],
         "TaskDefinition": NotRequired[str],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsDetailsExtraOutputTypeDef",
+    {
+        "Command": NotRequired[List[str]],
+        "Cpu": NotRequired[int],
+        "DependsOn": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef]
+        ],
+        "DisableNetworking": NotRequired[bool],
+        "DnsSearchDomains": NotRequired[List[str]],
+        "DnsServers": NotRequired[List[str]],
+        "DockerLabels": NotRequired[Dict[str, str]],
+        "DockerSecurityOptions": NotRequired[List[str]],
+        "EntryPoint": NotRequired[List[str]],
+        "Environment": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef]
+        ],
+        "EnvironmentFiles": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef]
+        ],
+        "Essential": NotRequired[bool],
+        "ExtraHosts": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef]
+        ],
+        "FirelensConfiguration": NotRequired[
+            AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsExtraOutputTypeDef
+        ],
+        "HealthCheck": NotRequired[
+            AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsExtraOutputTypeDef
+        ],
+        "Hostname": NotRequired[str],
+        "Image": NotRequired[str],
+        "Interactive": NotRequired[bool],
+        "Links": NotRequired[List[str]],
+        "LinuxParameters": NotRequired[
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsExtraOutputTypeDef
+        ],
+        "LogConfiguration": NotRequired[
+            AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsExtraOutputTypeDef
+        ],
+        "Memory": NotRequired[int],
+        "MemoryReservation": NotRequired[int],
+        "MountPoints": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef]
+        ],
+        "Name": NotRequired[str],
+        "PortMappings": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef]
+        ],
+        "Privileged": NotRequired[bool],
+        "PseudoTerminal": NotRequired[bool],
+        "ReadonlyRootFilesystem": NotRequired[bool],
+        "RepositoryCredentials": NotRequired[
+            AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef
+        ],
+        "ResourceRequirements": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef]
+        ],
+        "Secrets": NotRequired[List[AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef]],
+        "StartTimeout": NotRequired[int],
+        "StopTimeout": NotRequired[int],
+        "SystemControls": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef]
+        ],
+        "Ulimits": NotRequired[List[AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef]],
+        "User": NotRequired[str],
+        "VolumesFrom": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef]
+        ],
+        "WorkingDirectory": NotRequired[str],
+    },
+)
+AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef",
     {
         "Command": NotRequired[List[str]],
         "Cpu": NotRequired[int],
         "DependsOn": NotRequired[
             List[AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef]
         ],
         "DisableNetworking": NotRequired[bool],
@@ -8953,28 +10968,28 @@
             List[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef]
         ],
         "Essential": NotRequired[bool],
         "ExtraHosts": NotRequired[
             List[AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef]
         ],
         "FirelensConfiguration": NotRequired[
-            AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsPaginatorTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef
         ],
         "HealthCheck": NotRequired[
-            AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsPaginatorTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef
         ],
         "Hostname": NotRequired[str],
         "Image": NotRequired[str],
         "Interactive": NotRequired[bool],
         "Links": NotRequired[List[str]],
         "LinuxParameters": NotRequired[
-            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsPaginatorTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef
         ],
         "LogConfiguration": NotRequired[
-            AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsPaginatorTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef
         ],
         "Memory": NotRequired[int],
         "MemoryReservation": NotRequired[int],
         "MountPoints": NotRequired[
             List[AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef]
         ],
         "Name": NotRequired[str],
@@ -9076,19 +11091,32 @@
         "User": NotRequired[str],
         "VolumesFrom": NotRequired[
             Sequence[AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef]
         ],
         "WorkingDirectory": NotRequired[str],
     },
 )
-AwsEcsTaskDefinitionVolumesDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionVolumesDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionVolumesDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesDetailsExtraOutputTypeDef",
+    {
+        "DockerVolumeConfiguration": NotRequired[
+            AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsExtraOutputTypeDef
+        ],
+        "EfsVolumeConfiguration": NotRequired[
+            AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef
+        ],
+        "Host": NotRequired[AwsEcsTaskDefinitionVolumesHostDetailsTypeDef],
+        "Name": NotRequired[str],
+    },
+)
+AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef",
     {
         "DockerVolumeConfiguration": NotRequired[
-            AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsPaginatorTypeDef
+            AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef
         ],
         "EfsVolumeConfiguration": NotRequired[
             AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef
         ],
         "Host": NotRequired[AwsEcsTaskDefinitionVolumesHostDetailsTypeDef],
         "Name": NotRequired[str],
     },
@@ -9102,26 +11130,40 @@
         "EfsVolumeConfiguration": NotRequired[
             AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef
         ],
         "Host": NotRequired[AwsEcsTaskDefinitionVolumesHostDetailsTypeDef],
         "Name": NotRequired[str],
     },
 )
-AwsEcsTaskDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDetailsPaginatorTypeDef",
+AwsEcsTaskDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDetailsExtraOutputTypeDef",
     {
         "ClusterArn": NotRequired[str],
         "TaskDefinitionArn": NotRequired[str],
         "Version": NotRequired[str],
         "CreatedAt": NotRequired[str],
         "StartedAt": NotRequired[str],
         "StartedBy": NotRequired[str],
         "Group": NotRequired[str],
         "Volumes": NotRequired[List[AwsEcsTaskVolumeDetailsTypeDef]],
-        "Containers": NotRequired[List[AwsEcsContainerDetailsPaginatorTypeDef]],
+        "Containers": NotRequired[List[AwsEcsContainerDetailsExtraOutputTypeDef]],
+    },
+)
+AwsEcsTaskDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDetailsOutputTypeDef",
+    {
+        "ClusterArn": NotRequired[str],
+        "TaskDefinitionArn": NotRequired[str],
+        "Version": NotRequired[str],
+        "CreatedAt": NotRequired[str],
+        "StartedAt": NotRequired[str],
+        "StartedBy": NotRequired[str],
+        "Group": NotRequired[str],
+        "Volumes": NotRequired[List[AwsEcsTaskVolumeDetailsTypeDef]],
+        "Containers": NotRequired[List[AwsEcsContainerDetailsOutputTypeDef]],
     },
 )
 AwsEcsTaskDetailsTypeDef = TypedDict(
     "AwsEcsTaskDetailsTypeDef",
     {
         "ClusterArn": NotRequired[str],
         "TaskDefinitionArn": NotRequired[str],
@@ -9130,48 +11172,73 @@
         "StartedAt": NotRequired[str],
         "StartedBy": NotRequired[str],
         "Group": NotRequired[str],
         "Volumes": NotRequired[Sequence[AwsEcsTaskVolumeDetailsTypeDef]],
         "Containers": NotRequired[Sequence[AwsEcsContainerDetailsTypeDef]],
     },
 )
-AwsEfsAccessPointDetailsPaginatorTypeDef = TypedDict(
-    "AwsEfsAccessPointDetailsPaginatorTypeDef",
+AwsEfsAccessPointDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEfsAccessPointDetailsExtraOutputTypeDef",
+    {
+        "AccessPointId": NotRequired[str],
+        "Arn": NotRequired[str],
+        "ClientToken": NotRequired[str],
+        "FileSystemId": NotRequired[str],
+        "PosixUser": NotRequired[AwsEfsAccessPointPosixUserDetailsExtraOutputTypeDef],
+        "RootDirectory": NotRequired[AwsEfsAccessPointRootDirectoryDetailsTypeDef],
+    },
+)
+AwsEfsAccessPointDetailsOutputTypeDef = TypedDict(
+    "AwsEfsAccessPointDetailsOutputTypeDef",
     {
         "AccessPointId": NotRequired[str],
         "Arn": NotRequired[str],
         "ClientToken": NotRequired[str],
         "FileSystemId": NotRequired[str],
-        "PosixUser": NotRequired[AwsEfsAccessPointPosixUserDetailsPaginatorTypeDef],
+        "PosixUser": NotRequired[AwsEfsAccessPointPosixUserDetailsOutputTypeDef],
         "RootDirectory": NotRequired[AwsEfsAccessPointRootDirectoryDetailsTypeDef],
     },
 )
 AwsEfsAccessPointDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointDetailsTypeDef",
     {
         "AccessPointId": NotRequired[str],
         "Arn": NotRequired[str],
         "ClientToken": NotRequired[str],
         "FileSystemId": NotRequired[str],
         "PosixUser": NotRequired[AwsEfsAccessPointPosixUserDetailsTypeDef],
         "RootDirectory": NotRequired[AwsEfsAccessPointRootDirectoryDetailsTypeDef],
     },
 )
-AwsEksClusterDetailsPaginatorTypeDef = TypedDict(
-    "AwsEksClusterDetailsPaginatorTypeDef",
+AwsEksClusterDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEksClusterDetailsExtraOutputTypeDef",
+    {
+        "Arn": NotRequired[str],
+        "CertificateAuthorityData": NotRequired[str],
+        "ClusterStatus": NotRequired[str],
+        "Endpoint": NotRequired[str],
+        "Name": NotRequired[str],
+        "ResourcesVpcConfig": NotRequired[AwsEksClusterResourcesVpcConfigDetailsExtraOutputTypeDef],
+        "RoleArn": NotRequired[str],
+        "Version": NotRequired[str],
+        "Logging": NotRequired[AwsEksClusterLoggingDetailsExtraOutputTypeDef],
+    },
+)
+AwsEksClusterDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterDetailsOutputTypeDef",
     {
         "Arn": NotRequired[str],
         "CertificateAuthorityData": NotRequired[str],
         "ClusterStatus": NotRequired[str],
         "Endpoint": NotRequired[str],
         "Name": NotRequired[str],
-        "ResourcesVpcConfig": NotRequired[AwsEksClusterResourcesVpcConfigDetailsPaginatorTypeDef],
+        "ResourcesVpcConfig": NotRequired[AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef],
         "RoleArn": NotRequired[str],
         "Version": NotRequired[str],
-        "Logging": NotRequired[AwsEksClusterLoggingDetailsPaginatorTypeDef],
+        "Logging": NotRequired[AwsEksClusterLoggingDetailsOutputTypeDef],
     },
 )
 AwsEksClusterDetailsTypeDef = TypedDict(
     "AwsEksClusterDetailsTypeDef",
     {
         "Arn": NotRequired[str],
         "CertificateAuthorityData": NotRequired[str],
@@ -9180,16 +11247,16 @@
         "Name": NotRequired[str],
         "ResourcesVpcConfig": NotRequired[AwsEksClusterResourcesVpcConfigDetailsTypeDef],
         "RoleArn": NotRequired[str],
         "Version": NotRequired[str],
         "Logging": NotRequired[AwsEksClusterLoggingDetailsTypeDef],
     },
 )
-AwsElasticsearchDomainDetailsPaginatorTypeDef = TypedDict(
-    "AwsElasticsearchDomainDetailsPaginatorTypeDef",
+AwsElasticsearchDomainDetailsExtraOutputTypeDef = TypedDict(
+    "AwsElasticsearchDomainDetailsExtraOutputTypeDef",
     {
         "AccessPolicies": NotRequired[str],
         "DomainEndpointOptions": NotRequired[AwsElasticsearchDomainDomainEndpointOptionsTypeDef],
         "DomainId": NotRequired[str],
         "DomainName": NotRequired[str],
         "Endpoint": NotRequired[str],
         "Endpoints": NotRequired[Dict[str, str]],
@@ -9201,15 +11268,39 @@
             AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef
         ],
         "LogPublishingOptions": NotRequired[AwsElasticsearchDomainLogPublishingOptionsTypeDef],
         "NodeToNodeEncryptionOptions": NotRequired[
             AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef
         ],
         "ServiceSoftwareOptions": NotRequired[AwsElasticsearchDomainServiceSoftwareOptionsTypeDef],
-        "VPCOptions": NotRequired[AwsElasticsearchDomainVPCOptionsPaginatorTypeDef],
+        "VPCOptions": NotRequired[AwsElasticsearchDomainVPCOptionsExtraOutputTypeDef],
+    },
+)
+AwsElasticsearchDomainDetailsOutputTypeDef = TypedDict(
+    "AwsElasticsearchDomainDetailsOutputTypeDef",
+    {
+        "AccessPolicies": NotRequired[str],
+        "DomainEndpointOptions": NotRequired[AwsElasticsearchDomainDomainEndpointOptionsTypeDef],
+        "DomainId": NotRequired[str],
+        "DomainName": NotRequired[str],
+        "Endpoint": NotRequired[str],
+        "Endpoints": NotRequired[Dict[str, str]],
+        "ElasticsearchVersion": NotRequired[str],
+        "ElasticsearchClusterConfig": NotRequired[
+            AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef
+        ],
+        "EncryptionAtRestOptions": NotRequired[
+            AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef
+        ],
+        "LogPublishingOptions": NotRequired[AwsElasticsearchDomainLogPublishingOptionsTypeDef],
+        "NodeToNodeEncryptionOptions": NotRequired[
+            AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef
+        ],
+        "ServiceSoftwareOptions": NotRequired[AwsElasticsearchDomainServiceSoftwareOptionsTypeDef],
+        "VPCOptions": NotRequired[AwsElasticsearchDomainVPCOptionsOutputTypeDef],
     },
 )
 AwsElasticsearchDomainDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainDetailsTypeDef",
     {
         "AccessPolicies": NotRequired[str],
         "DomainEndpointOptions": NotRequired[AwsElasticsearchDomainDomainEndpointOptionsTypeDef],
@@ -9228,33 +11319,59 @@
         "NodeToNodeEncryptionOptions": NotRequired[
             AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef
         ],
         "ServiceSoftwareOptions": NotRequired[AwsElasticsearchDomainServiceSoftwareOptionsTypeDef],
         "VPCOptions": NotRequired[AwsElasticsearchDomainVPCOptionsTypeDef],
     },
 )
-AwsElbLoadBalancerDetailsPaginatorTypeDef = TypedDict(
-    "AwsElbLoadBalancerDetailsPaginatorTypeDef",
+AwsElbLoadBalancerDetailsExtraOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerDetailsExtraOutputTypeDef",
     {
         "AvailabilityZones": NotRequired[List[str]],
         "BackendServerDescriptions": NotRequired[
-            List[AwsElbLoadBalancerBackendServerDescriptionPaginatorTypeDef]
+            List[AwsElbLoadBalancerBackendServerDescriptionExtraOutputTypeDef]
         ],
         "CanonicalHostedZoneName": NotRequired[str],
         "CanonicalHostedZoneNameID": NotRequired[str],
         "CreatedTime": NotRequired[str],
         "DnsName": NotRequired[str],
         "HealthCheck": NotRequired[AwsElbLoadBalancerHealthCheckTypeDef],
         "Instances": NotRequired[List[AwsElbLoadBalancerInstanceTypeDef]],
         "ListenerDescriptions": NotRequired[
-            List[AwsElbLoadBalancerListenerDescriptionPaginatorTypeDef]
+            List[AwsElbLoadBalancerListenerDescriptionExtraOutputTypeDef]
         ],
-        "LoadBalancerAttributes": NotRequired[AwsElbLoadBalancerAttributesPaginatorTypeDef],
+        "LoadBalancerAttributes": NotRequired[AwsElbLoadBalancerAttributesExtraOutputTypeDef],
         "LoadBalancerName": NotRequired[str],
-        "Policies": NotRequired[AwsElbLoadBalancerPoliciesPaginatorTypeDef],
+        "Policies": NotRequired[AwsElbLoadBalancerPoliciesExtraOutputTypeDef],
+        "Scheme": NotRequired[str],
+        "SecurityGroups": NotRequired[List[str]],
+        "SourceSecurityGroup": NotRequired[AwsElbLoadBalancerSourceSecurityGroupTypeDef],
+        "Subnets": NotRequired[List[str]],
+        "VpcId": NotRequired[str],
+    },
+)
+AwsElbLoadBalancerDetailsOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerDetailsOutputTypeDef",
+    {
+        "AvailabilityZones": NotRequired[List[str]],
+        "BackendServerDescriptions": NotRequired[
+            List[AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef]
+        ],
+        "CanonicalHostedZoneName": NotRequired[str],
+        "CanonicalHostedZoneNameID": NotRequired[str],
+        "CreatedTime": NotRequired[str],
+        "DnsName": NotRequired[str],
+        "HealthCheck": NotRequired[AwsElbLoadBalancerHealthCheckTypeDef],
+        "Instances": NotRequired[List[AwsElbLoadBalancerInstanceTypeDef]],
+        "ListenerDescriptions": NotRequired[
+            List[AwsElbLoadBalancerListenerDescriptionOutputTypeDef]
+        ],
+        "LoadBalancerAttributes": NotRequired[AwsElbLoadBalancerAttributesOutputTypeDef],
+        "LoadBalancerName": NotRequired[str],
+        "Policies": NotRequired[AwsElbLoadBalancerPoliciesOutputTypeDef],
         "Scheme": NotRequired[str],
         "SecurityGroups": NotRequired[List[str]],
         "SourceSecurityGroup": NotRequired[AwsElbLoadBalancerSourceSecurityGroupTypeDef],
         "Subnets": NotRequired[List[str]],
         "VpcId": NotRequired[str],
     },
 )
@@ -9307,21 +11424,36 @@
         "PrincipalType": NotRequired[str],
         "PrincipalName": NotRequired[str],
         "AccountId": NotRequired[str],
         "AccessKeyId": NotRequired[str],
         "SessionContext": NotRequired[AwsIamAccessKeySessionContextTypeDef],
     },
 )
-AwsIamRoleDetailsPaginatorTypeDef = TypedDict(
-    "AwsIamRoleDetailsPaginatorTypeDef",
+AwsIamRoleDetailsExtraOutputTypeDef = TypedDict(
+    "AwsIamRoleDetailsExtraOutputTypeDef",
+    {
+        "AssumeRolePolicyDocument": NotRequired[str],
+        "AttachedManagedPolicies": NotRequired[List[AwsIamAttachedManagedPolicyTypeDef]],
+        "CreateDate": NotRequired[str],
+        "InstanceProfileList": NotRequired[List[AwsIamInstanceProfileExtraOutputTypeDef]],
+        "PermissionsBoundary": NotRequired[AwsIamPermissionsBoundaryTypeDef],
+        "RoleId": NotRequired[str],
+        "RoleName": NotRequired[str],
+        "RolePolicyList": NotRequired[List[AwsIamRolePolicyTypeDef]],
+        "MaxSessionDuration": NotRequired[int],
+        "Path": NotRequired[str],
+    },
+)
+AwsIamRoleDetailsOutputTypeDef = TypedDict(
+    "AwsIamRoleDetailsOutputTypeDef",
     {
         "AssumeRolePolicyDocument": NotRequired[str],
         "AttachedManagedPolicies": NotRequired[List[AwsIamAttachedManagedPolicyTypeDef]],
         "CreateDate": NotRequired[str],
-        "InstanceProfileList": NotRequired[List[AwsIamInstanceProfilePaginatorTypeDef]],
+        "InstanceProfileList": NotRequired[List[AwsIamInstanceProfileOutputTypeDef]],
         "PermissionsBoundary": NotRequired[AwsIamPermissionsBoundaryTypeDef],
         "RoleId": NotRequired[str],
         "RoleName": NotRequired[str],
         "RolePolicyList": NotRequired[List[AwsIamRolePolicyTypeDef]],
         "MaxSessionDuration": NotRequired[int],
         "Path": NotRequired[str],
     },
@@ -9337,34 +11469,59 @@
         "RoleId": NotRequired[str],
         "RoleName": NotRequired[str],
         "RolePolicyList": NotRequired[Sequence[AwsIamRolePolicyTypeDef]],
         "MaxSessionDuration": NotRequired[int],
         "Path": NotRequired[str],
     },
 )
-AwsLambdaFunctionDetailsPaginatorTypeDef = TypedDict(
-    "AwsLambdaFunctionDetailsPaginatorTypeDef",
+AwsLambdaFunctionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionDetailsExtraOutputTypeDef",
     {
         "Code": NotRequired[AwsLambdaFunctionCodeTypeDef],
         "CodeSha256": NotRequired[str],
         "DeadLetterConfig": NotRequired[AwsLambdaFunctionDeadLetterConfigTypeDef],
-        "Environment": NotRequired[AwsLambdaFunctionEnvironmentPaginatorTypeDef],
+        "Environment": NotRequired[AwsLambdaFunctionEnvironmentExtraOutputTypeDef],
         "FunctionName": NotRequired[str],
         "Handler": NotRequired[str],
         "KmsKeyArn": NotRequired[str],
         "LastModified": NotRequired[str],
         "Layers": NotRequired[List[AwsLambdaFunctionLayerTypeDef]],
         "MasterArn": NotRequired[str],
         "MemorySize": NotRequired[int],
         "RevisionId": NotRequired[str],
         "Role": NotRequired[str],
         "Runtime": NotRequired[str],
         "Timeout": NotRequired[int],
         "TracingConfig": NotRequired[AwsLambdaFunctionTracingConfigTypeDef],
-        "VpcConfig": NotRequired[AwsLambdaFunctionVpcConfigPaginatorTypeDef],
+        "VpcConfig": NotRequired[AwsLambdaFunctionVpcConfigExtraOutputTypeDef],
+        "Version": NotRequired[str],
+        "Architectures": NotRequired[List[str]],
+        "PackageType": NotRequired[str],
+    },
+)
+AwsLambdaFunctionDetailsOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionDetailsOutputTypeDef",
+    {
+        "Code": NotRequired[AwsLambdaFunctionCodeTypeDef],
+        "CodeSha256": NotRequired[str],
+        "DeadLetterConfig": NotRequired[AwsLambdaFunctionDeadLetterConfigTypeDef],
+        "Environment": NotRequired[AwsLambdaFunctionEnvironmentOutputTypeDef],
+        "FunctionName": NotRequired[str],
+        "Handler": NotRequired[str],
+        "KmsKeyArn": NotRequired[str],
+        "LastModified": NotRequired[str],
+        "Layers": NotRequired[List[AwsLambdaFunctionLayerTypeDef]],
+        "MasterArn": NotRequired[str],
+        "MemorySize": NotRequired[int],
+        "RevisionId": NotRequired[str],
+        "Role": NotRequired[str],
+        "Runtime": NotRequired[str],
+        "Timeout": NotRequired[int],
+        "TracingConfig": NotRequired[AwsLambdaFunctionTracingConfigTypeDef],
+        "VpcConfig": NotRequired[AwsLambdaFunctionVpcConfigOutputTypeDef],
         "Version": NotRequired[str],
         "Architectures": NotRequired[List[str]],
         "PackageType": NotRequired[str],
     },
 )
 AwsLambdaFunctionDetailsTypeDef = TypedDict(
     "AwsLambdaFunctionDetailsTypeDef",
@@ -9387,36 +11544,48 @@
         "TracingConfig": NotRequired[AwsLambdaFunctionTracingConfigTypeDef],
         "VpcConfig": NotRequired[AwsLambdaFunctionVpcConfigTypeDef],
         "Version": NotRequired[str],
         "Architectures": NotRequired[Sequence[str]],
         "PackageType": NotRequired[str],
     },
 )
-AwsMskClusterClusterInfoClientAuthenticationDetailsPaginatorTypeDef = TypedDict(
-    "AwsMskClusterClusterInfoClientAuthenticationDetailsPaginatorTypeDef",
+AwsMskClusterClusterInfoClientAuthenticationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsMskClusterClusterInfoClientAuthenticationDetailsExtraOutputTypeDef",
+    {
+        "Sasl": NotRequired[AwsMskClusterClusterInfoClientAuthenticationSaslDetailsTypeDef],
+        "Unauthenticated": NotRequired[
+            AwsMskClusterClusterInfoClientAuthenticationUnauthenticatedDetailsTypeDef
+        ],
+        "Tls": NotRequired[
+            AwsMskClusterClusterInfoClientAuthenticationTlsDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsMskClusterClusterInfoClientAuthenticationDetailsOutputTypeDef = TypedDict(
+    "AwsMskClusterClusterInfoClientAuthenticationDetailsOutputTypeDef",
     {
         "Sasl": NotRequired[AwsMskClusterClusterInfoClientAuthenticationSaslDetailsTypeDef],
         "Unauthenticated": NotRequired[
             AwsMskClusterClusterInfoClientAuthenticationUnauthenticatedDetailsTypeDef
         ],
-        "Tls": NotRequired[AwsMskClusterClusterInfoClientAuthenticationTlsDetailsPaginatorTypeDef],
+        "Tls": NotRequired[AwsMskClusterClusterInfoClientAuthenticationTlsDetailsOutputTypeDef],
     },
 )
 AwsMskClusterClusterInfoClientAuthenticationDetailsTypeDef = TypedDict(
     "AwsMskClusterClusterInfoClientAuthenticationDetailsTypeDef",
     {
         "Sasl": NotRequired[AwsMskClusterClusterInfoClientAuthenticationSaslDetailsTypeDef],
         "Unauthenticated": NotRequired[
             AwsMskClusterClusterInfoClientAuthenticationUnauthenticatedDetailsTypeDef
         ],
         "Tls": NotRequired[AwsMskClusterClusterInfoClientAuthenticationTlsDetailsTypeDef],
     },
 )
-AwsOpenSearchServiceDomainDetailsPaginatorTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainDetailsPaginatorTypeDef",
+AwsOpenSearchServiceDomainDetailsExtraOutputTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainDetailsExtraOutputTypeDef",
     {
         "Arn": NotRequired[str],
         "AccessPolicies": NotRequired[str],
         "DomainName": NotRequired[str],
         "Id": NotRequired[str],
         "DomainEndpoint": NotRequired[str],
         "EngineVersion": NotRequired[str],
@@ -9429,15 +11598,47 @@
         "ServiceSoftwareOptions": NotRequired[
             AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef
         ],
         "ClusterConfig": NotRequired[AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef],
         "DomainEndpointOptions": NotRequired[
             AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef
         ],
-        "VpcOptions": NotRequired[AwsOpenSearchServiceDomainVpcOptionsDetailsPaginatorTypeDef],
+        "VpcOptions": NotRequired[AwsOpenSearchServiceDomainVpcOptionsDetailsExtraOutputTypeDef],
+        "LogPublishingOptions": NotRequired[
+            AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef
+        ],
+        "DomainEndpoints": NotRequired[Dict[str, str]],
+        "AdvancedSecurityOptions": NotRequired[
+            AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef
+        ],
+    },
+)
+AwsOpenSearchServiceDomainDetailsOutputTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainDetailsOutputTypeDef",
+    {
+        "Arn": NotRequired[str],
+        "AccessPolicies": NotRequired[str],
+        "DomainName": NotRequired[str],
+        "Id": NotRequired[str],
+        "DomainEndpoint": NotRequired[str],
+        "EngineVersion": NotRequired[str],
+        "EncryptionAtRestOptions": NotRequired[
+            AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef
+        ],
+        "NodeToNodeEncryptionOptions": NotRequired[
+            AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef
+        ],
+        "ServiceSoftwareOptions": NotRequired[
+            AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef
+        ],
+        "ClusterConfig": NotRequired[AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef],
+        "DomainEndpointOptions": NotRequired[
+            AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef
+        ],
+        "VpcOptions": NotRequired[AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef],
         "LogPublishingOptions": NotRequired[
             AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef
         ],
         "DomainEndpoints": NotRequired[Dict[str, str]],
         "AdvancedSecurityOptions": NotRequired[
             AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef
         ],
@@ -9471,16 +11672,27 @@
         ],
         "DomainEndpoints": NotRequired[Mapping[str, str]],
         "AdvancedSecurityOptions": NotRequired[
             AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef
         ],
     },
 )
-AwsRdsDbSubnetGroupPaginatorTypeDef = TypedDict(
-    "AwsRdsDbSubnetGroupPaginatorTypeDef",
+AwsRdsDbSubnetGroupExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbSubnetGroupExtraOutputTypeDef",
+    {
+        "DbSubnetGroupName": NotRequired[str],
+        "DbSubnetGroupDescription": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "SubnetGroupStatus": NotRequired[str],
+        "Subnets": NotRequired[List[AwsRdsDbSubnetGroupSubnetTypeDef]],
+        "DbSubnetGroupArn": NotRequired[str],
+    },
+)
+AwsRdsDbSubnetGroupOutputTypeDef = TypedDict(
+    "AwsRdsDbSubnetGroupOutputTypeDef",
     {
         "DbSubnetGroupName": NotRequired[str],
         "DbSubnetGroupDescription": NotRequired[str],
         "VpcId": NotRequired[str],
         "SubnetGroupStatus": NotRequired[str],
         "Subnets": NotRequired[List[AwsRdsDbSubnetGroupSubnetTypeDef]],
         "DbSubnetGroupArn": NotRequired[str],
@@ -9493,26 +11705,81 @@
         "DbSubnetGroupDescription": NotRequired[str],
         "VpcId": NotRequired[str],
         "SubnetGroupStatus": NotRequired[str],
         "Subnets": NotRequired[Sequence[AwsRdsDbSubnetGroupSubnetTypeDef]],
         "DbSubnetGroupArn": NotRequired[str],
     },
 )
-AwsRedshiftClusterDetailsPaginatorTypeDef = TypedDict(
-    "AwsRedshiftClusterDetailsPaginatorTypeDef",
+AwsRedshiftClusterDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRedshiftClusterDetailsExtraOutputTypeDef",
+    {
+        "AllowVersionUpgrade": NotRequired[bool],
+        "AutomatedSnapshotRetentionPeriod": NotRequired[int],
+        "AvailabilityZone": NotRequired[str],
+        "ClusterAvailabilityStatus": NotRequired[str],
+        "ClusterCreateTime": NotRequired[str],
+        "ClusterIdentifier": NotRequired[str],
+        "ClusterNodes": NotRequired[List[AwsRedshiftClusterClusterNodeTypeDef]],
+        "ClusterParameterGroups": NotRequired[
+            List[AwsRedshiftClusterClusterParameterGroupExtraOutputTypeDef]
+        ],
+        "ClusterPublicKey": NotRequired[str],
+        "ClusterRevisionNumber": NotRequired[str],
+        "ClusterSecurityGroups": NotRequired[List[AwsRedshiftClusterClusterSecurityGroupTypeDef]],
+        "ClusterSnapshotCopyStatus": NotRequired[
+            AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef
+        ],
+        "ClusterStatus": NotRequired[str],
+        "ClusterSubnetGroupName": NotRequired[str],
+        "ClusterVersion": NotRequired[str],
+        "DBName": NotRequired[str],
+        "DeferredMaintenanceWindows": NotRequired[
+            List[AwsRedshiftClusterDeferredMaintenanceWindowTypeDef]
+        ],
+        "ElasticIpStatus": NotRequired[AwsRedshiftClusterElasticIpStatusTypeDef],
+        "ElasticResizeNumberOfNodeOptions": NotRequired[str],
+        "Encrypted": NotRequired[bool],
+        "Endpoint": NotRequired[AwsRedshiftClusterEndpointTypeDef],
+        "EnhancedVpcRouting": NotRequired[bool],
+        "ExpectedNextSnapshotScheduleTime": NotRequired[str],
+        "ExpectedNextSnapshotScheduleTimeStatus": NotRequired[str],
+        "HsmStatus": NotRequired[AwsRedshiftClusterHsmStatusTypeDef],
+        "IamRoles": NotRequired[List[AwsRedshiftClusterIamRoleTypeDef]],
+        "KmsKeyId": NotRequired[str],
+        "MaintenanceTrackName": NotRequired[str],
+        "ManualSnapshotRetentionPeriod": NotRequired[int],
+        "MasterUsername": NotRequired[str],
+        "NextMaintenanceWindowStartTime": NotRequired[str],
+        "NodeType": NotRequired[str],
+        "NumberOfNodes": NotRequired[int],
+        "PendingActions": NotRequired[List[str]],
+        "PendingModifiedValues": NotRequired[AwsRedshiftClusterPendingModifiedValuesTypeDef],
+        "PreferredMaintenanceWindow": NotRequired[str],
+        "PubliclyAccessible": NotRequired[bool],
+        "ResizeInfo": NotRequired[AwsRedshiftClusterResizeInfoTypeDef],
+        "RestoreStatus": NotRequired[AwsRedshiftClusterRestoreStatusTypeDef],
+        "SnapshotScheduleIdentifier": NotRequired[str],
+        "SnapshotScheduleState": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "VpcSecurityGroups": NotRequired[List[AwsRedshiftClusterVpcSecurityGroupTypeDef]],
+        "LoggingStatus": NotRequired[AwsRedshiftClusterLoggingStatusTypeDef],
+    },
+)
+AwsRedshiftClusterDetailsOutputTypeDef = TypedDict(
+    "AwsRedshiftClusterDetailsOutputTypeDef",
     {
         "AllowVersionUpgrade": NotRequired[bool],
         "AutomatedSnapshotRetentionPeriod": NotRequired[int],
         "AvailabilityZone": NotRequired[str],
         "ClusterAvailabilityStatus": NotRequired[str],
         "ClusterCreateTime": NotRequired[str],
         "ClusterIdentifier": NotRequired[str],
         "ClusterNodes": NotRequired[List[AwsRedshiftClusterClusterNodeTypeDef]],
         "ClusterParameterGroups": NotRequired[
-            List[AwsRedshiftClusterClusterParameterGroupPaginatorTypeDef]
+            List[AwsRedshiftClusterClusterParameterGroupOutputTypeDef]
         ],
         "ClusterPublicKey": NotRequired[str],
         "ClusterRevisionNumber": NotRequired[str],
         "ClusterSecurityGroups": NotRequired[List[AwsRedshiftClusterClusterSecurityGroupTypeDef]],
         "ClusterSnapshotCopyStatus": NotRequired[
             AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef
         ],
@@ -9605,16 +11872,25 @@
         "SnapshotScheduleIdentifier": NotRequired[str],
         "SnapshotScheduleState": NotRequired[str],
         "VpcId": NotRequired[str],
         "VpcSecurityGroups": NotRequired[Sequence[AwsRedshiftClusterVpcSecurityGroupTypeDef]],
         "LoggingStatus": NotRequired[AwsRedshiftClusterLoggingStatusTypeDef],
     },
 )
-AwsRoute53HostedZoneDetailsPaginatorTypeDef = TypedDict(
-    "AwsRoute53HostedZoneDetailsPaginatorTypeDef",
+AwsRoute53HostedZoneDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRoute53HostedZoneDetailsExtraOutputTypeDef",
+    {
+        "HostedZone": NotRequired[AwsRoute53HostedZoneObjectDetailsTypeDef],
+        "Vpcs": NotRequired[List[AwsRoute53HostedZoneVpcDetailsTypeDef]],
+        "NameServers": NotRequired[List[str]],
+        "QueryLoggingConfig": NotRequired[AwsRoute53QueryLoggingConfigDetailsTypeDef],
+    },
+)
+AwsRoute53HostedZoneDetailsOutputTypeDef = TypedDict(
+    "AwsRoute53HostedZoneDetailsOutputTypeDef",
     {
         "HostedZone": NotRequired[AwsRoute53HostedZoneObjectDetailsTypeDef],
         "Vpcs": NotRequired[List[AwsRoute53HostedZoneVpcDetailsTypeDef]],
         "NameServers": NotRequired[List[str]],
         "QueryLoggingConfig": NotRequired[AwsRoute53QueryLoggingConfigDetailsTypeDef],
     },
 )
@@ -9623,16 +11899,29 @@
     {
         "HostedZone": NotRequired[AwsRoute53HostedZoneObjectDetailsTypeDef],
         "Vpcs": NotRequired[Sequence[AwsRoute53HostedZoneVpcDetailsTypeDef]],
         "NameServers": NotRequired[Sequence[str]],
         "QueryLoggingConfig": NotRequired[AwsRoute53QueryLoggingConfigDetailsTypeDef],
     },
 )
-AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsPaginatorTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsPaginatorTypeDef",
+AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsExtraOutputTypeDef",
+    {
+        "Operands": NotRequired[
+            List[AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef]
+        ],
+        "Prefix": NotRequired[str],
+        "Tag": NotRequired[
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef
+        ],
+        "Type": NotRequired[str],
+    },
+)
+AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef",
     {
         "Operands": NotRequired[
             List[AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef]
         ],
         "Prefix": NotRequired[str],
         "Tag": NotRequired[
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef
@@ -9651,18 +11940,26 @@
         "Prefix": NotRequired[str],
         "Tag": NotRequired[
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef
         ],
         "Type": NotRequired[str],
     },
 )
-AwsS3BucketNotificationConfigurationFilterPaginatorTypeDef = TypedDict(
-    "AwsS3BucketNotificationConfigurationFilterPaginatorTypeDef",
+AwsS3BucketNotificationConfigurationFilterExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationFilterExtraOutputTypeDef",
+    {
+        "S3KeyFilter": NotRequired[
+            AwsS3BucketNotificationConfigurationS3KeyFilterExtraOutputTypeDef
+        ],
+    },
+)
+AwsS3BucketNotificationConfigurationFilterOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationFilterOutputTypeDef",
     {
-        "S3KeyFilter": NotRequired[AwsS3BucketNotificationConfigurationS3KeyFilterPaginatorTypeDef],
+        "S3KeyFilter": NotRequired[AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef],
     },
 )
 AwsS3BucketNotificationConfigurationFilterTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
     {
         "S3KeyFilter": NotRequired[AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef],
     },
@@ -9670,28 +11967,43 @@
 AwsS3BucketObjectLockConfigurationTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationTypeDef",
     {
         "ObjectLockEnabled": NotRequired[str],
         "Rule": NotRequired[AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef],
     },
 )
-AwsS3BucketServerSideEncryptionConfigurationPaginatorTypeDef = TypedDict(
-    "AwsS3BucketServerSideEncryptionConfigurationPaginatorTypeDef",
+AwsS3BucketServerSideEncryptionConfigurationExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketServerSideEncryptionConfigurationExtraOutputTypeDef",
+    {
+        "Rules": NotRequired[List[AwsS3BucketServerSideEncryptionRuleTypeDef]],
+    },
+)
+AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
+    "AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef",
     {
         "Rules": NotRequired[List[AwsS3BucketServerSideEncryptionRuleTypeDef]],
     },
 )
 AwsS3BucketServerSideEncryptionConfigurationTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
     {
         "Rules": NotRequired[Sequence[AwsS3BucketServerSideEncryptionRuleTypeDef]],
     },
 )
-AwsS3BucketWebsiteConfigurationPaginatorTypeDef = TypedDict(
-    "AwsS3BucketWebsiteConfigurationPaginatorTypeDef",
+AwsS3BucketWebsiteConfigurationExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketWebsiteConfigurationExtraOutputTypeDef",
+    {
+        "ErrorDocument": NotRequired[str],
+        "IndexDocumentSuffix": NotRequired[str],
+        "RedirectAllRequestsTo": NotRequired[AwsS3BucketWebsiteConfigurationRedirectToTypeDef],
+        "RoutingRules": NotRequired[List[AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef]],
+    },
+)
+AwsS3BucketWebsiteConfigurationOutputTypeDef = TypedDict(
+    "AwsS3BucketWebsiteConfigurationOutputTypeDef",
     {
         "ErrorDocument": NotRequired[str],
         "IndexDocumentSuffix": NotRequired[str],
         "RedirectAllRequestsTo": NotRequired[AwsS3BucketWebsiteConfigurationRedirectToTypeDef],
         "RoutingRules": NotRequired[List[AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef]],
     },
 )
@@ -9714,16 +12026,26 @@
 )
 AwsSsmPatchComplianceDetailsTypeDef = TypedDict(
     "AwsSsmPatchComplianceDetailsTypeDef",
     {
         "Patch": NotRequired[AwsSsmPatchTypeDef],
     },
 )
-AwsStepFunctionStateMachineLoggingConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsStepFunctionStateMachineLoggingConfigurationDetailsPaginatorTypeDef",
+AwsStepFunctionStateMachineLoggingConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsExtraOutputTypeDef",
+    {
+        "Destinations": NotRequired[
+            List[AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef]
+        ],
+        "IncludeExecutionData": NotRequired[bool],
+        "Level": NotRequired[str],
+    },
+)
+AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef",
     {
         "Destinations": NotRequired[
             List[AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef]
         ],
         "IncludeExecutionData": NotRequired[bool],
         "Level": NotRequired[str],
     },
@@ -9734,16 +12056,25 @@
         "Destinations": NotRequired[
             Sequence[AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef]
         ],
         "IncludeExecutionData": NotRequired[bool],
         "Level": NotRequired[str],
     },
 )
-AwsWafRegionalRuleGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafRegionalRuleGroupDetailsPaginatorTypeDef",
+AwsWafRegionalRuleGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafRegionalRuleGroupDetailsExtraOutputTypeDef",
+    {
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "RuleGroupId": NotRequired[str],
+        "Rules": NotRequired[List[AwsWafRegionalRuleGroupRulesDetailsTypeDef]],
+    },
+)
+AwsWafRegionalRuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalRuleGroupDetailsOutputTypeDef",
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RuleGroupId": NotRequired[str],
         "Rules": NotRequired[List[AwsWafRegionalRuleGroupRulesDetailsTypeDef]],
     },
 )
@@ -9752,16 +12083,26 @@
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RuleGroupId": NotRequired[str],
         "Rules": NotRequired[Sequence[AwsWafRegionalRuleGroupRulesDetailsTypeDef]],
     },
 )
-AwsWafRegionalWebAclDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafRegionalWebAclDetailsPaginatorTypeDef",
+AwsWafRegionalWebAclDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafRegionalWebAclDetailsExtraOutputTypeDef",
+    {
+        "DefaultAction": NotRequired[str],
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "RulesList": NotRequired[List[AwsWafRegionalWebAclRulesListDetailsTypeDef]],
+        "WebAclId": NotRequired[str],
+    },
+)
+AwsWafRegionalWebAclDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalWebAclDetailsOutputTypeDef",
     {
         "DefaultAction": NotRequired[str],
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RulesList": NotRequired[List[AwsWafRegionalWebAclRulesListDetailsTypeDef]],
         "WebAclId": NotRequired[str],
     },
@@ -9772,16 +12113,25 @@
         "DefaultAction": NotRequired[str],
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RulesList": NotRequired[Sequence[AwsWafRegionalWebAclRulesListDetailsTypeDef]],
         "WebAclId": NotRequired[str],
     },
 )
-AwsWafRuleGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafRuleGroupDetailsPaginatorTypeDef",
+AwsWafRuleGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafRuleGroupDetailsExtraOutputTypeDef",
+    {
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "RuleGroupId": NotRequired[str],
+        "Rules": NotRequired[List[AwsWafRuleGroupRulesDetailsTypeDef]],
+    },
+)
+AwsWafRuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsWafRuleGroupDetailsOutputTypeDef",
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RuleGroupId": NotRequired[str],
         "Rules": NotRequired[List[AwsWafRuleGroupRulesDetailsTypeDef]],
     },
 )
@@ -9790,48 +12140,81 @@
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RuleGroupId": NotRequired[str],
         "Rules": NotRequired[Sequence[AwsWafRuleGroupRulesDetailsTypeDef]],
     },
 )
-AwsWafWebAclDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafWebAclDetailsPaginatorTypeDef",
+AwsWafWebAclDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafWebAclDetailsExtraOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "DefaultAction": NotRequired[str],
+        "Rules": NotRequired[List[AwsWafWebAclRuleExtraOutputTypeDef]],
+        "WebAclId": NotRequired[str],
+    },
+)
+AwsWafWebAclDetailsOutputTypeDef = TypedDict(
+    "AwsWafWebAclDetailsOutputTypeDef",
     {
         "Name": NotRequired[str],
         "DefaultAction": NotRequired[str],
-        "Rules": NotRequired[List[AwsWafWebAclRulePaginatorTypeDef]],
+        "Rules": NotRequired[List[AwsWafWebAclRuleOutputTypeDef]],
         "WebAclId": NotRequired[str],
     },
 )
 AwsWafWebAclDetailsTypeDef = TypedDict(
     "AwsWafWebAclDetailsTypeDef",
     {
         "Name": NotRequired[str],
         "DefaultAction": NotRequired[str],
         "Rules": NotRequired[Sequence[AwsWafWebAclRuleTypeDef]],
         "WebAclId": NotRequired[str],
     },
 )
-AwsWafv2ActionAllowDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2ActionAllowDetailsPaginatorTypeDef",
+AwsWafv2ActionAllowDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2ActionAllowDetailsExtraOutputTypeDef",
     {
-        "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsPaginatorTypeDef],
+        "CustomRequestHandling": NotRequired[
+            AwsWafv2CustomRequestHandlingDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsWafv2RulesActionCaptchaDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionCaptchaDetailsExtraOutputTypeDef",
+    {
+        "CustomRequestHandling": NotRequired[
+            AwsWafv2CustomRequestHandlingDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsWafv2RulesActionCountDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionCountDetailsExtraOutputTypeDef",
+    {
+        "CustomRequestHandling": NotRequired[
+            AwsWafv2CustomRequestHandlingDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsWafv2ActionAllowDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2ActionAllowDetailsOutputTypeDef",
+    {
+        "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsOutputTypeDef],
     },
 )
-AwsWafv2RulesActionCaptchaDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2RulesActionCaptchaDetailsPaginatorTypeDef",
+AwsWafv2RulesActionCaptchaDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionCaptchaDetailsOutputTypeDef",
     {
-        "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsPaginatorTypeDef],
+        "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsOutputTypeDef],
     },
 )
-AwsWafv2RulesActionCountDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2RulesActionCountDetailsPaginatorTypeDef",
+AwsWafv2RulesActionCountDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionCountDetailsOutputTypeDef",
     {
-        "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsPaginatorTypeDef],
+        "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsOutputTypeDef],
     },
 )
 AwsWafv2ActionAllowDetailsTypeDef = TypedDict(
     "AwsWafv2ActionAllowDetailsTypeDef",
     {
         "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsTypeDef],
     },
@@ -9844,18 +12227,24 @@
 )
 AwsWafv2RulesActionCountDetailsTypeDef = TypedDict(
     "AwsWafv2RulesActionCountDetailsTypeDef",
     {
         "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsTypeDef],
     },
 )
-AwsWafv2ActionBlockDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2ActionBlockDetailsPaginatorTypeDef",
+AwsWafv2ActionBlockDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2ActionBlockDetailsExtraOutputTypeDef",
+    {
+        "CustomResponse": NotRequired[AwsWafv2CustomResponseDetailsExtraOutputTypeDef],
+    },
+)
+AwsWafv2ActionBlockDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2ActionBlockDetailsOutputTypeDef",
     {
-        "CustomResponse": NotRequired[AwsWafv2CustomResponseDetailsPaginatorTypeDef],
+        "CustomResponse": NotRequired[AwsWafv2CustomResponseDetailsOutputTypeDef],
     },
 )
 AwsWafv2ActionBlockDetailsTypeDef = TypedDict(
     "AwsWafv2ActionBlockDetailsTypeDef",
     {
         "CustomResponse": NotRequired[AwsWafv2CustomResponseDetailsTypeDef],
     },
@@ -9871,28 +12260,46 @@
 BatchUpdateStandardsControlAssociationsResponseTypeDef = TypedDict(
     "BatchUpdateStandardsControlAssociationsResponseTypeDef",
     {
         "UnprocessedAssociationUpdates": List[UnprocessedStandardsControlAssociationUpdateTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-VulnerabilityPaginatorTypeDef = TypedDict(
-    "VulnerabilityPaginatorTypeDef",
+VulnerabilityExtraOutputTypeDef = TypedDict(
+    "VulnerabilityExtraOutputTypeDef",
     {
         "Id": str,
         "VulnerablePackages": NotRequired[List[SoftwarePackageTypeDef]],
-        "Cvss": NotRequired[List[CvssPaginatorTypeDef]],
+        "Cvss": NotRequired[List[CvssExtraOutputTypeDef]],
         "RelatedVulnerabilities": NotRequired[List[str]],
         "Vendor": NotRequired[VulnerabilityVendorTypeDef],
         "ReferenceUrls": NotRequired[List[str]],
         "FixAvailable": NotRequired[VulnerabilityFixAvailableType],
         "EpssScore": NotRequired[float],
         "ExploitAvailable": NotRequired[VulnerabilityExploitAvailableType],
         "LastKnownExploitAt": NotRequired[str],
-        "CodeVulnerabilities": NotRequired[List[VulnerabilityCodeVulnerabilitiesPaginatorTypeDef]],
+        "CodeVulnerabilities": NotRequired[
+            List[VulnerabilityCodeVulnerabilitiesExtraOutputTypeDef]
+        ],
+    },
+)
+VulnerabilityOutputTypeDef = TypedDict(
+    "VulnerabilityOutputTypeDef",
+    {
+        "Id": str,
+        "VulnerablePackages": NotRequired[List[SoftwarePackageTypeDef]],
+        "Cvss": NotRequired[List[CvssOutputTypeDef]],
+        "RelatedVulnerabilities": NotRequired[List[str]],
+        "Vendor": NotRequired[VulnerabilityVendorTypeDef],
+        "ReferenceUrls": NotRequired[List[str]],
+        "FixAvailable": NotRequired[VulnerabilityFixAvailableType],
+        "EpssScore": NotRequired[float],
+        "ExploitAvailable": NotRequired[VulnerabilityExploitAvailableType],
+        "LastKnownExploitAt": NotRequired[str],
+        "CodeVulnerabilities": NotRequired[List[VulnerabilityCodeVulnerabilitiesOutputTypeDef]],
     },
 )
 VulnerabilityTypeDef = TypedDict(
     "VulnerabilityTypeDef",
     {
         "Id": str,
         "VulnerablePackages": NotRequired[Sequence[SoftwarePackageTypeDef]],
@@ -9928,16 +12335,16 @@
         "ConfigurationPolicyAssociationIdentifiers": NotRequired[
             ConfigurationPolicyAssociationTypeDef
         ],
         "ErrorCode": NotRequired[str],
         "ErrorReason": NotRequired[str],
     },
 )
-AutomationRulesFindingFiltersTypeDef = TypedDict(
-    "AutomationRulesFindingFiltersTypeDef",
+AutomationRulesFindingFiltersOutputTypeDef = TypedDict(
+    "AutomationRulesFindingFiltersOutputTypeDef",
     {
         "ProductArn": NotRequired[List[StringFilterTypeDef]],
         "AwsAccountId": NotRequired[List[StringFilterTypeDef]],
         "Id": NotRequired[List[StringFilterTypeDef]],
         "GeneratorId": NotRequired[List[StringFilterTypeDef]],
         "Type": NotRequired[List[StringFilterTypeDef]],
         "FirstObservedAt": NotRequired[List[DateFilterTypeDef]],
@@ -9971,14 +12378,275 @@
         "NoteUpdatedBy": NotRequired[List[StringFilterTypeDef]],
         "UserDefinedFields": NotRequired[List[MapFilterTypeDef]],
         "ResourceApplicationArn": NotRequired[List[StringFilterTypeDef]],
         "ResourceApplicationName": NotRequired[List[StringFilterTypeDef]],
         "AwsAccountName": NotRequired[List[StringFilterTypeDef]],
     },
 )
+AutomationRulesFindingFiltersTypeDef = TypedDict(
+    "AutomationRulesFindingFiltersTypeDef",
+    {
+        "ProductArn": NotRequired[Sequence[StringFilterTypeDef]],
+        "AwsAccountId": NotRequired[Sequence[StringFilterTypeDef]],
+        "Id": NotRequired[Sequence[StringFilterTypeDef]],
+        "GeneratorId": NotRequired[Sequence[StringFilterTypeDef]],
+        "Type": NotRequired[Sequence[StringFilterTypeDef]],
+        "FirstObservedAt": NotRequired[Sequence[DateFilterTypeDef]],
+        "LastObservedAt": NotRequired[Sequence[DateFilterTypeDef]],
+        "CreatedAt": NotRequired[Sequence[DateFilterTypeDef]],
+        "UpdatedAt": NotRequired[Sequence[DateFilterTypeDef]],
+        "Confidence": NotRequired[Sequence[NumberFilterTypeDef]],
+        "Criticality": NotRequired[Sequence[NumberFilterTypeDef]],
+        "Title": NotRequired[Sequence[StringFilterTypeDef]],
+        "Description": NotRequired[Sequence[StringFilterTypeDef]],
+        "SourceUrl": NotRequired[Sequence[StringFilterTypeDef]],
+        "ProductName": NotRequired[Sequence[StringFilterTypeDef]],
+        "CompanyName": NotRequired[Sequence[StringFilterTypeDef]],
+        "SeverityLabel": NotRequired[Sequence[StringFilterTypeDef]],
+        "ResourceType": NotRequired[Sequence[StringFilterTypeDef]],
+        "ResourceId": NotRequired[Sequence[StringFilterTypeDef]],
+        "ResourcePartition": NotRequired[Sequence[StringFilterTypeDef]],
+        "ResourceRegion": NotRequired[Sequence[StringFilterTypeDef]],
+        "ResourceTags": NotRequired[Sequence[MapFilterTypeDef]],
+        "ResourceDetailsOther": NotRequired[Sequence[MapFilterTypeDef]],
+        "ComplianceStatus": NotRequired[Sequence[StringFilterTypeDef]],
+        "ComplianceSecurityControlId": NotRequired[Sequence[StringFilterTypeDef]],
+        "ComplianceAssociatedStandardsId": NotRequired[Sequence[StringFilterTypeDef]],
+        "VerificationState": NotRequired[Sequence[StringFilterTypeDef]],
+        "WorkflowStatus": NotRequired[Sequence[StringFilterTypeDef]],
+        "RecordState": NotRequired[Sequence[StringFilterTypeDef]],
+        "RelatedFindingsProductArn": NotRequired[Sequence[StringFilterTypeDef]],
+        "RelatedFindingsId": NotRequired[Sequence[StringFilterTypeDef]],
+        "NoteText": NotRequired[Sequence[StringFilterTypeDef]],
+        "NoteUpdatedAt": NotRequired[Sequence[DateFilterTypeDef]],
+        "NoteUpdatedBy": NotRequired[Sequence[StringFilterTypeDef]],
+        "UserDefinedFields": NotRequired[Sequence[MapFilterTypeDef]],
+        "ResourceApplicationArn": NotRequired[Sequence[StringFilterTypeDef]],
+        "ResourceApplicationName": NotRequired[Sequence[StringFilterTypeDef]],
+        "AwsAccountName": NotRequired[Sequence[StringFilterTypeDef]],
+    },
+)
+AwsSecurityFindingFiltersExtraOutputTypeDef = TypedDict(
+    "AwsSecurityFindingFiltersExtraOutputTypeDef",
+    {
+        "ProductArn": NotRequired[List[StringFilterTypeDef]],
+        "AwsAccountId": NotRequired[List[StringFilterTypeDef]],
+        "Id": NotRequired[List[StringFilterTypeDef]],
+        "GeneratorId": NotRequired[List[StringFilterTypeDef]],
+        "Region": NotRequired[List[StringFilterTypeDef]],
+        "Type": NotRequired[List[StringFilterTypeDef]],
+        "FirstObservedAt": NotRequired[List[DateFilterTypeDef]],
+        "LastObservedAt": NotRequired[List[DateFilterTypeDef]],
+        "CreatedAt": NotRequired[List[DateFilterTypeDef]],
+        "UpdatedAt": NotRequired[List[DateFilterTypeDef]],
+        "SeverityProduct": NotRequired[List[NumberFilterTypeDef]],
+        "SeverityNormalized": NotRequired[List[NumberFilterTypeDef]],
+        "SeverityLabel": NotRequired[List[StringFilterTypeDef]],
+        "Confidence": NotRequired[List[NumberFilterTypeDef]],
+        "Criticality": NotRequired[List[NumberFilterTypeDef]],
+        "Title": NotRequired[List[StringFilterTypeDef]],
+        "Description": NotRequired[List[StringFilterTypeDef]],
+        "RecommendationText": NotRequired[List[StringFilterTypeDef]],
+        "SourceUrl": NotRequired[List[StringFilterTypeDef]],
+        "ProductFields": NotRequired[List[MapFilterTypeDef]],
+        "ProductName": NotRequired[List[StringFilterTypeDef]],
+        "CompanyName": NotRequired[List[StringFilterTypeDef]],
+        "UserDefinedFields": NotRequired[List[MapFilterTypeDef]],
+        "MalwareName": NotRequired[List[StringFilterTypeDef]],
+        "MalwareType": NotRequired[List[StringFilterTypeDef]],
+        "MalwarePath": NotRequired[List[StringFilterTypeDef]],
+        "MalwareState": NotRequired[List[StringFilterTypeDef]],
+        "NetworkDirection": NotRequired[List[StringFilterTypeDef]],
+        "NetworkProtocol": NotRequired[List[StringFilterTypeDef]],
+        "NetworkSourceIpV4": NotRequired[List[IpFilterTypeDef]],
+        "NetworkSourceIpV6": NotRequired[List[IpFilterTypeDef]],
+        "NetworkSourcePort": NotRequired[List[NumberFilterTypeDef]],
+        "NetworkSourceDomain": NotRequired[List[StringFilterTypeDef]],
+        "NetworkSourceMac": NotRequired[List[StringFilterTypeDef]],
+        "NetworkDestinationIpV4": NotRequired[List[IpFilterTypeDef]],
+        "NetworkDestinationIpV6": NotRequired[List[IpFilterTypeDef]],
+        "NetworkDestinationPort": NotRequired[List[NumberFilterTypeDef]],
+        "NetworkDestinationDomain": NotRequired[List[StringFilterTypeDef]],
+        "ProcessName": NotRequired[List[StringFilterTypeDef]],
+        "ProcessPath": NotRequired[List[StringFilterTypeDef]],
+        "ProcessPid": NotRequired[List[NumberFilterTypeDef]],
+        "ProcessParentPid": NotRequired[List[NumberFilterTypeDef]],
+        "ProcessLaunchedAt": NotRequired[List[DateFilterTypeDef]],
+        "ProcessTerminatedAt": NotRequired[List[DateFilterTypeDef]],
+        "ThreatIntelIndicatorType": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorValue": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorCategory": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorLastObservedAt": NotRequired[List[DateFilterTypeDef]],
+        "ThreatIntelIndicatorSource": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorSourceUrl": NotRequired[List[StringFilterTypeDef]],
+        "ResourceType": NotRequired[List[StringFilterTypeDef]],
+        "ResourceId": NotRequired[List[StringFilterTypeDef]],
+        "ResourcePartition": NotRequired[List[StringFilterTypeDef]],
+        "ResourceRegion": NotRequired[List[StringFilterTypeDef]],
+        "ResourceTags": NotRequired[List[MapFilterTypeDef]],
+        "ResourceAwsEc2InstanceType": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceImageId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceIpV4Addresses": NotRequired[List[IpFilterTypeDef]],
+        "ResourceAwsEc2InstanceIpV6Addresses": NotRequired[List[IpFilterTypeDef]],
+        "ResourceAwsEc2InstanceKeyName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceIamInstanceProfileArn": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceVpcId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceSubnetId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceLaunchedAt": NotRequired[List[DateFilterTypeDef]],
+        "ResourceAwsS3BucketOwnerId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsS3BucketOwnerName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyUserName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyPrincipalName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyStatus": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyCreatedAt": NotRequired[List[DateFilterTypeDef]],
+        "ResourceAwsIamUserUserName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerImageId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerImageName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerLaunchedAt": NotRequired[List[DateFilterTypeDef]],
+        "ResourceDetailsOther": NotRequired[List[MapFilterTypeDef]],
+        "ComplianceStatus": NotRequired[List[StringFilterTypeDef]],
+        "VerificationState": NotRequired[List[StringFilterTypeDef]],
+        "WorkflowState": NotRequired[List[StringFilterTypeDef]],
+        "WorkflowStatus": NotRequired[List[StringFilterTypeDef]],
+        "RecordState": NotRequired[List[StringFilterTypeDef]],
+        "RelatedFindingsProductArn": NotRequired[List[StringFilterTypeDef]],
+        "RelatedFindingsId": NotRequired[List[StringFilterTypeDef]],
+        "NoteText": NotRequired[List[StringFilterTypeDef]],
+        "NoteUpdatedAt": NotRequired[List[DateFilterTypeDef]],
+        "NoteUpdatedBy": NotRequired[List[StringFilterTypeDef]],
+        "Keyword": NotRequired[List[KeywordFilterTypeDef]],
+        "FindingProviderFieldsConfidence": NotRequired[List[NumberFilterTypeDef]],
+        "FindingProviderFieldsCriticality": NotRequired[List[NumberFilterTypeDef]],
+        "FindingProviderFieldsRelatedFindingsId": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsRelatedFindingsProductArn": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsSeverityLabel": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsSeverityOriginal": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsTypes": NotRequired[List[StringFilterTypeDef]],
+        "Sample": NotRequired[List[BooleanFilterTypeDef]],
+        "ComplianceSecurityControlId": NotRequired[List[StringFilterTypeDef]],
+        "ComplianceAssociatedStandardsId": NotRequired[List[StringFilterTypeDef]],
+        "VulnerabilitiesExploitAvailable": NotRequired[List[StringFilterTypeDef]],
+        "VulnerabilitiesFixAvailable": NotRequired[List[StringFilterTypeDef]],
+        "ComplianceSecurityControlParametersName": NotRequired[List[StringFilterTypeDef]],
+        "ComplianceSecurityControlParametersValue": NotRequired[List[StringFilterTypeDef]],
+        "AwsAccountName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceApplicationName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceApplicationArn": NotRequired[List[StringFilterTypeDef]],
+    },
+)
+AwsSecurityFindingFiltersOutputTypeDef = TypedDict(
+    "AwsSecurityFindingFiltersOutputTypeDef",
+    {
+        "ProductArn": NotRequired[List[StringFilterTypeDef]],
+        "AwsAccountId": NotRequired[List[StringFilterTypeDef]],
+        "Id": NotRequired[List[StringFilterTypeDef]],
+        "GeneratorId": NotRequired[List[StringFilterTypeDef]],
+        "Region": NotRequired[List[StringFilterTypeDef]],
+        "Type": NotRequired[List[StringFilterTypeDef]],
+        "FirstObservedAt": NotRequired[List[DateFilterTypeDef]],
+        "LastObservedAt": NotRequired[List[DateFilterTypeDef]],
+        "CreatedAt": NotRequired[List[DateFilterTypeDef]],
+        "UpdatedAt": NotRequired[List[DateFilterTypeDef]],
+        "SeverityProduct": NotRequired[List[NumberFilterTypeDef]],
+        "SeverityNormalized": NotRequired[List[NumberFilterTypeDef]],
+        "SeverityLabel": NotRequired[List[StringFilterTypeDef]],
+        "Confidence": NotRequired[List[NumberFilterTypeDef]],
+        "Criticality": NotRequired[List[NumberFilterTypeDef]],
+        "Title": NotRequired[List[StringFilterTypeDef]],
+        "Description": NotRequired[List[StringFilterTypeDef]],
+        "RecommendationText": NotRequired[List[StringFilterTypeDef]],
+        "SourceUrl": NotRequired[List[StringFilterTypeDef]],
+        "ProductFields": NotRequired[List[MapFilterTypeDef]],
+        "ProductName": NotRequired[List[StringFilterTypeDef]],
+        "CompanyName": NotRequired[List[StringFilterTypeDef]],
+        "UserDefinedFields": NotRequired[List[MapFilterTypeDef]],
+        "MalwareName": NotRequired[List[StringFilterTypeDef]],
+        "MalwareType": NotRequired[List[StringFilterTypeDef]],
+        "MalwarePath": NotRequired[List[StringFilterTypeDef]],
+        "MalwareState": NotRequired[List[StringFilterTypeDef]],
+        "NetworkDirection": NotRequired[List[StringFilterTypeDef]],
+        "NetworkProtocol": NotRequired[List[StringFilterTypeDef]],
+        "NetworkSourceIpV4": NotRequired[List[IpFilterTypeDef]],
+        "NetworkSourceIpV6": NotRequired[List[IpFilterTypeDef]],
+        "NetworkSourcePort": NotRequired[List[NumberFilterTypeDef]],
+        "NetworkSourceDomain": NotRequired[List[StringFilterTypeDef]],
+        "NetworkSourceMac": NotRequired[List[StringFilterTypeDef]],
+        "NetworkDestinationIpV4": NotRequired[List[IpFilterTypeDef]],
+        "NetworkDestinationIpV6": NotRequired[List[IpFilterTypeDef]],
+        "NetworkDestinationPort": NotRequired[List[NumberFilterTypeDef]],
+        "NetworkDestinationDomain": NotRequired[List[StringFilterTypeDef]],
+        "ProcessName": NotRequired[List[StringFilterTypeDef]],
+        "ProcessPath": NotRequired[List[StringFilterTypeDef]],
+        "ProcessPid": NotRequired[List[NumberFilterTypeDef]],
+        "ProcessParentPid": NotRequired[List[NumberFilterTypeDef]],
+        "ProcessLaunchedAt": NotRequired[List[DateFilterTypeDef]],
+        "ProcessTerminatedAt": NotRequired[List[DateFilterTypeDef]],
+        "ThreatIntelIndicatorType": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorValue": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorCategory": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorLastObservedAt": NotRequired[List[DateFilterTypeDef]],
+        "ThreatIntelIndicatorSource": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorSourceUrl": NotRequired[List[StringFilterTypeDef]],
+        "ResourceType": NotRequired[List[StringFilterTypeDef]],
+        "ResourceId": NotRequired[List[StringFilterTypeDef]],
+        "ResourcePartition": NotRequired[List[StringFilterTypeDef]],
+        "ResourceRegion": NotRequired[List[StringFilterTypeDef]],
+        "ResourceTags": NotRequired[List[MapFilterTypeDef]],
+        "ResourceAwsEc2InstanceType": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceImageId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceIpV4Addresses": NotRequired[List[IpFilterTypeDef]],
+        "ResourceAwsEc2InstanceIpV6Addresses": NotRequired[List[IpFilterTypeDef]],
+        "ResourceAwsEc2InstanceKeyName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceIamInstanceProfileArn": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceVpcId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceSubnetId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceLaunchedAt": NotRequired[List[DateFilterTypeDef]],
+        "ResourceAwsS3BucketOwnerId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsS3BucketOwnerName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyUserName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyPrincipalName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyStatus": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyCreatedAt": NotRequired[List[DateFilterTypeDef]],
+        "ResourceAwsIamUserUserName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerImageId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerImageName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerLaunchedAt": NotRequired[List[DateFilterTypeDef]],
+        "ResourceDetailsOther": NotRequired[List[MapFilterTypeDef]],
+        "ComplianceStatus": NotRequired[List[StringFilterTypeDef]],
+        "VerificationState": NotRequired[List[StringFilterTypeDef]],
+        "WorkflowState": NotRequired[List[StringFilterTypeDef]],
+        "WorkflowStatus": NotRequired[List[StringFilterTypeDef]],
+        "RecordState": NotRequired[List[StringFilterTypeDef]],
+        "RelatedFindingsProductArn": NotRequired[List[StringFilterTypeDef]],
+        "RelatedFindingsId": NotRequired[List[StringFilterTypeDef]],
+        "NoteText": NotRequired[List[StringFilterTypeDef]],
+        "NoteUpdatedAt": NotRequired[List[DateFilterTypeDef]],
+        "NoteUpdatedBy": NotRequired[List[StringFilterTypeDef]],
+        "Keyword": NotRequired[List[KeywordFilterTypeDef]],
+        "FindingProviderFieldsConfidence": NotRequired[List[NumberFilterTypeDef]],
+        "FindingProviderFieldsCriticality": NotRequired[List[NumberFilterTypeDef]],
+        "FindingProviderFieldsRelatedFindingsId": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsRelatedFindingsProductArn": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsSeverityLabel": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsSeverityOriginal": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsTypes": NotRequired[List[StringFilterTypeDef]],
+        "Sample": NotRequired[List[BooleanFilterTypeDef]],
+        "ComplianceSecurityControlId": NotRequired[List[StringFilterTypeDef]],
+        "ComplianceAssociatedStandardsId": NotRequired[List[StringFilterTypeDef]],
+        "VulnerabilitiesExploitAvailable": NotRequired[List[StringFilterTypeDef]],
+        "VulnerabilitiesFixAvailable": NotRequired[List[StringFilterTypeDef]],
+        "ComplianceSecurityControlParametersName": NotRequired[List[StringFilterTypeDef]],
+        "ComplianceSecurityControlParametersValue": NotRequired[List[StringFilterTypeDef]],
+        "AwsAccountName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceApplicationName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceApplicationArn": NotRequired[List[StringFilterTypeDef]],
+    },
+)
 AwsSecurityFindingFiltersTypeDef = TypedDict(
     "AwsSecurityFindingFiltersTypeDef",
     {
         "ProductArn": NotRequired[Sequence[StringFilterTypeDef]],
         "AwsAccountId": NotRequired[Sequence[StringFilterTypeDef]],
         "Id": NotRequired[Sequence[StringFilterTypeDef]],
         "GeneratorId": NotRequired[Sequence[StringFilterTypeDef]],
@@ -10086,43 +12754,61 @@
         "ResourceApplicationArn": NotRequired[Sequence[StringFilterTypeDef]],
     },
 )
 GetFindingHistoryResponseTypeDef = TypedDict(
     "GetFindingHistoryResponseTypeDef",
     {
         "Records": List[FindingHistoryRecordTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetInsightResultsResponseTypeDef = TypedDict(
     "GetInsightResultsResponseTypeDef",
     {
         "InsightResults": InsightResultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-NetworkHeaderPaginatorTypeDef = TypedDict(
-    "NetworkHeaderPaginatorTypeDef",
+NetworkHeaderExtraOutputTypeDef = TypedDict(
+    "NetworkHeaderExtraOutputTypeDef",
     {
         "Protocol": NotRequired[str],
-        "Destination": NotRequired[NetworkPathComponentDetailsPaginatorTypeDef],
-        "Source": NotRequired[NetworkPathComponentDetailsPaginatorTypeDef],
+        "Destination": NotRequired[NetworkPathComponentDetailsExtraOutputTypeDef],
+        "Source": NotRequired[NetworkPathComponentDetailsExtraOutputTypeDef],
+    },
+)
+NetworkHeaderOutputTypeDef = TypedDict(
+    "NetworkHeaderOutputTypeDef",
+    {
+        "Protocol": NotRequired[str],
+        "Destination": NotRequired[NetworkPathComponentDetailsOutputTypeDef],
+        "Source": NotRequired[NetworkPathComponentDetailsOutputTypeDef],
     },
 )
 NetworkHeaderTypeDef = TypedDict(
     "NetworkHeaderTypeDef",
     {
         "Protocol": NotRequired[str],
         "Destination": NotRequired[NetworkPathComponentDetailsTypeDef],
         "Source": NotRequired[NetworkPathComponentDetailsTypeDef],
     },
 )
-OccurrencesPaginatorTypeDef = TypedDict(
-    "OccurrencesPaginatorTypeDef",
+OccurrencesExtraOutputTypeDef = TypedDict(
+    "OccurrencesExtraOutputTypeDef",
+    {
+        "LineRanges": NotRequired[List[RangeTypeDef]],
+        "OffsetRanges": NotRequired[List[RangeTypeDef]],
+        "Pages": NotRequired[List[PageTypeDef]],
+        "Records": NotRequired[List[RecordTypeDef]],
+        "Cells": NotRequired[List[CellTypeDef]],
+    },
+)
+OccurrencesOutputTypeDef = TypedDict(
+    "OccurrencesOutputTypeDef",
     {
         "LineRanges": NotRequired[List[RangeTypeDef]],
         "OffsetRanges": NotRequired[List[RangeTypeDef]],
         "Pages": NotRequired[List[PageTypeDef]],
         "Records": NotRequired[List[RecordTypeDef]],
         "Cells": NotRequired[List[CellTypeDef]],
     },
@@ -10133,64 +12819,75 @@
         "LineRanges": NotRequired[Sequence[RangeTypeDef]],
         "OffsetRanges": NotRequired[Sequence[RangeTypeDef]],
         "Pages": NotRequired[Sequence[PageTypeDef]],
         "Records": NotRequired[Sequence[RecordTypeDef]],
         "Cells": NotRequired[Sequence[CellTypeDef]],
     },
 )
-SecurityControlCustomParameterTypeDef = TypedDict(
-    "SecurityControlCustomParameterTypeDef",
+SecurityControlCustomParameterOutputTypeDef = TypedDict(
+    "SecurityControlCustomParameterOutputTypeDef",
     {
         "SecurityControlId": NotRequired[str],
-        "Parameters": NotRequired[Mapping[str, ParameterConfigurationTypeDef]],
+        "Parameters": NotRequired[Dict[str, ParameterConfigurationOutputTypeDef]],
     },
 )
 SecurityControlTypeDef = TypedDict(
     "SecurityControlTypeDef",
     {
         "SecurityControlId": str,
         "SecurityControlArn": str,
         "Title": str,
         "Description": str,
         "RemediationUrl": str,
         "SeverityRating": SeverityRatingType,
         "SecurityControlStatus": ControlStatusType,
         "UpdateStatus": NotRequired[UpdateStatusType],
-        "Parameters": NotRequired[Dict[str, ParameterConfigurationTypeDef]],
+        "Parameters": NotRequired[Dict[str, ParameterConfigurationOutputTypeDef]],
         "LastUpdateReason": NotRequired[str],
     },
 )
-UpdateSecurityControlRequestRequestTypeDef = TypedDict(
-    "UpdateSecurityControlRequestRequestTypeDef",
+ParameterConfigurationUnionTypeDef = Union[
+    ParameterConfigurationTypeDef, ParameterConfigurationOutputTypeDef
+]
+SecurityControlCustomParameterTypeDef = TypedDict(
+    "SecurityControlCustomParameterTypeDef",
     {
-        "SecurityControlId": str,
-        "Parameters": Mapping[str, ParameterConfigurationTypeDef],
-        "LastUpdateReason": NotRequired[str],
+        "SecurityControlId": NotRequired[str],
+        "Parameters": NotRequired[Mapping[str, ParameterConfigurationTypeDef]],
+    },
+)
+RuleGroupSourceStatelessRuleDefinitionExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleDefinitionExtraOutputTypeDef",
+    {
+        "Actions": NotRequired[List[str]],
+        "MatchAttributes": NotRequired[
+            RuleGroupSourceStatelessRuleMatchAttributesExtraOutputTypeDef
+        ],
     },
 )
-RuleGroupSourceStatelessRuleDefinitionPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleDefinitionPaginatorTypeDef",
+RuleGroupSourceStatelessRuleDefinitionOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleDefinitionOutputTypeDef",
     {
         "Actions": NotRequired[List[str]],
-        "MatchAttributes": NotRequired[RuleGroupSourceStatelessRuleMatchAttributesPaginatorTypeDef],
+        "MatchAttributes": NotRequired[RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef],
     },
 )
 RuleGroupSourceStatelessRuleDefinitionTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
     {
         "Actions": NotRequired[Sequence[str]],
         "MatchAttributes": NotRequired[RuleGroupSourceStatelessRuleMatchAttributesTypeDef],
     },
 )
 DescribeStandardsResponseTypeDef = TypedDict(
     "DescribeStandardsResponseTypeDef",
     {
         "Standards": List[StandardTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 BatchDisableStandardsResponseTypeDef = TypedDict(
     "BatchDisableStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -10203,63 +12900,99 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetEnabledStandardsResponseTypeDef = TypedDict(
     "GetEnabledStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-StatelessCustomActionDefinitionPaginatorTypeDef = TypedDict(
-    "StatelessCustomActionDefinitionPaginatorTypeDef",
+StatelessCustomActionDefinitionExtraOutputTypeDef = TypedDict(
+    "StatelessCustomActionDefinitionExtraOutputTypeDef",
     {
-        "PublishMetricAction": NotRequired[StatelessCustomPublishMetricActionPaginatorTypeDef],
+        "PublishMetricAction": NotRequired[StatelessCustomPublishMetricActionExtraOutputTypeDef],
+    },
+)
+StatelessCustomActionDefinitionOutputTypeDef = TypedDict(
+    "StatelessCustomActionDefinitionOutputTypeDef",
+    {
+        "PublishMetricAction": NotRequired[StatelessCustomPublishMetricActionOutputTypeDef],
     },
 )
 StatelessCustomActionDefinitionTypeDef = TypedDict(
     "StatelessCustomActionDefinitionTypeDef",
     {
         "PublishMetricAction": NotRequired[StatelessCustomPublishMetricActionTypeDef],
     },
 )
-PortProbeActionPaginatorTypeDef = TypedDict(
-    "PortProbeActionPaginatorTypeDef",
+PortProbeActionExtraOutputTypeDef = TypedDict(
+    "PortProbeActionExtraOutputTypeDef",
+    {
+        "PortProbeDetails": NotRequired[List[PortProbeDetailTypeDef]],
+        "Blocked": NotRequired[bool],
+    },
+)
+PortProbeActionOutputTypeDef = TypedDict(
+    "PortProbeActionOutputTypeDef",
     {
         "PortProbeDetails": NotRequired[List[PortProbeDetailTypeDef]],
         "Blocked": NotRequired[bool],
     },
 )
 PortProbeActionTypeDef = TypedDict(
     "PortProbeActionTypeDef",
     {
         "PortProbeDetails": NotRequired[Sequence[PortProbeDetailTypeDef]],
         "Blocked": NotRequired[bool],
     },
 )
+AutomationRulesActionUnionTypeDef = Union[
+    AutomationRulesActionTypeDef, AutomationRulesActionOutputTypeDef
+]
 AwsAthenaWorkGroupDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupDetailsTypeDef",
     {
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "State": NotRequired[str],
         "Configuration": NotRequired[AwsAthenaWorkGroupConfigurationDetailsTypeDef],
     },
 )
-AwsAutoScalingAutoScalingGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupDetailsPaginatorTypeDef",
+AwsAutoScalingAutoScalingGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupDetailsExtraOutputTypeDef",
     {
         "LaunchConfigurationName": NotRequired[str],
         "LoadBalancerNames": NotRequired[List[str]],
         "HealthCheckType": NotRequired[str],
         "HealthCheckGracePeriod": NotRequired[int],
         "CreatedTime": NotRequired[str],
         "MixedInstancesPolicy": NotRequired[
-            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsPaginatorTypeDef
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsExtraOutputTypeDef
+        ],
+        "AvailabilityZones": NotRequired[
+            List[AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef]
+        ],
+        "LaunchTemplate": NotRequired[
+            AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
+        ],
+        "CapacityRebalance": NotRequired[bool],
+    },
+)
+AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef",
+    {
+        "LaunchConfigurationName": NotRequired[str],
+        "LoadBalancerNames": NotRequired[List[str]],
+        "HealthCheckType": NotRequired[str],
+        "HealthCheckGracePeriod": NotRequired[int],
+        "CreatedTime": NotRequired[str],
+        "MixedInstancesPolicy": NotRequired[
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef
         ],
         "AvailabilityZones": NotRequired[
             List[AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef]
         ],
         "LaunchTemplate": NotRequired[
             AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
         ],
@@ -10282,42 +13015,52 @@
         ],
         "LaunchTemplate": NotRequired[
             AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
         ],
         "CapacityRebalance": NotRequired[bool],
     },
 )
-AwsBackupBackupPlanBackupPlanDetailsPaginatorTypeDef = TypedDict(
-    "AwsBackupBackupPlanBackupPlanDetailsPaginatorTypeDef",
+AwsBackupBackupPlanBackupPlanDetailsExtraOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanBackupPlanDetailsExtraOutputTypeDef",
     {
         "BackupPlanName": NotRequired[str],
         "AdvancedBackupSettings": NotRequired[
-            List[AwsBackupBackupPlanAdvancedBackupSettingsDetailsPaginatorTypeDef]
+            List[AwsBackupBackupPlanAdvancedBackupSettingsDetailsExtraOutputTypeDef]
         ],
-        "BackupPlanRule": NotRequired[List[AwsBackupBackupPlanRuleDetailsPaginatorTypeDef]],
+        "BackupPlanRule": NotRequired[List[AwsBackupBackupPlanRuleDetailsExtraOutputTypeDef]],
+    },
+)
+AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef",
+    {
+        "BackupPlanName": NotRequired[str],
+        "AdvancedBackupSettings": NotRequired[
+            List[AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef]
+        ],
+        "BackupPlanRule": NotRequired[List[AwsBackupBackupPlanRuleDetailsOutputTypeDef]],
     },
 )
 AwsBackupBackupPlanBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
     {
         "BackupPlanName": NotRequired[str],
         "AdvancedBackupSettings": NotRequired[
             Sequence[AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef]
         ],
         "BackupPlanRule": NotRequired[Sequence[AwsBackupBackupPlanRuleDetailsTypeDef]],
     },
 )
-AwsCertificateManagerCertificateDetailsPaginatorTypeDef = TypedDict(
-    "AwsCertificateManagerCertificateDetailsPaginatorTypeDef",
+AwsCertificateManagerCertificateDetailsExtraOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateDetailsExtraOutputTypeDef",
     {
         "CertificateAuthorityArn": NotRequired[str],
         "CreatedAt": NotRequired[str],
         "DomainName": NotRequired[str],
         "DomainValidationOptions": NotRequired[
-            List[AwsCertificateManagerCertificateDomainValidationOptionPaginatorTypeDef]
+            List[AwsCertificateManagerCertificateDomainValidationOptionExtraOutputTypeDef]
         ],
         "ExtendedKeyUsages": NotRequired[
             List[AwsCertificateManagerCertificateExtendedKeyUsageTypeDef]
         ],
         "FailureReason": NotRequired[str],
         "ImportedAt": NotRequired[str],
         "InUseBy": NotRequired[List[str]],
@@ -10326,16 +13069,48 @@
         "KeyAlgorithm": NotRequired[str],
         "KeyUsages": NotRequired[List[AwsCertificateManagerCertificateKeyUsageTypeDef]],
         "NotAfter": NotRequired[str],
         "NotBefore": NotRequired[str],
         "Options": NotRequired[AwsCertificateManagerCertificateOptionsTypeDef],
         "RenewalEligibility": NotRequired[str],
         "RenewalSummary": NotRequired[
-            AwsCertificateManagerCertificateRenewalSummaryPaginatorTypeDef
+            AwsCertificateManagerCertificateRenewalSummaryExtraOutputTypeDef
+        ],
+        "Serial": NotRequired[str],
+        "SignatureAlgorithm": NotRequired[str],
+        "Status": NotRequired[str],
+        "Subject": NotRequired[str],
+        "SubjectAlternativeNames": NotRequired[List[str]],
+        "Type": NotRequired[str],
+    },
+)
+AwsCertificateManagerCertificateDetailsOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateDetailsOutputTypeDef",
+    {
+        "CertificateAuthorityArn": NotRequired[str],
+        "CreatedAt": NotRequired[str],
+        "DomainName": NotRequired[str],
+        "DomainValidationOptions": NotRequired[
+            List[AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef]
+        ],
+        "ExtendedKeyUsages": NotRequired[
+            List[AwsCertificateManagerCertificateExtendedKeyUsageTypeDef]
         ],
+        "FailureReason": NotRequired[str],
+        "ImportedAt": NotRequired[str],
+        "InUseBy": NotRequired[List[str]],
+        "IssuedAt": NotRequired[str],
+        "Issuer": NotRequired[str],
+        "KeyAlgorithm": NotRequired[str],
+        "KeyUsages": NotRequired[List[AwsCertificateManagerCertificateKeyUsageTypeDef]],
+        "NotAfter": NotRequired[str],
+        "NotBefore": NotRequired[str],
+        "Options": NotRequired[AwsCertificateManagerCertificateOptionsTypeDef],
+        "RenewalEligibility": NotRequired[str],
+        "RenewalSummary": NotRequired[AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef],
         "Serial": NotRequired[str],
         "SignatureAlgorithm": NotRequired[str],
         "Status": NotRequired[str],
         "Subject": NotRequired[str],
         "SubjectAlternativeNames": NotRequired[List[str]],
         "Type": NotRequired[str],
     },
@@ -10368,57 +13143,98 @@
         "SignatureAlgorithm": NotRequired[str],
         "Status": NotRequired[str],
         "Subject": NotRequired[str],
         "SubjectAlternativeNames": NotRequired[Sequence[str]],
         "Type": NotRequired[str],
     },
 )
-AwsCloudFrontDistributionOriginsPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginsPaginatorTypeDef",
+AwsCloudFrontDistributionOriginsExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginsExtraOutputTypeDef",
     {
-        "Items": NotRequired[List[AwsCloudFrontDistributionOriginItemPaginatorTypeDef]],
+        "Items": NotRequired[List[AwsCloudFrontDistributionOriginItemExtraOutputTypeDef]],
+    },
+)
+AwsCloudFrontDistributionOriginsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginsOutputTypeDef",
+    {
+        "Items": NotRequired[List[AwsCloudFrontDistributionOriginItemOutputTypeDef]],
     },
 )
 AwsCloudFrontDistributionOriginsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginsTypeDef",
     {
         "Items": NotRequired[Sequence[AwsCloudFrontDistributionOriginItemTypeDef]],
     },
 )
-AwsCloudFrontDistributionOriginGroupsPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginGroupsPaginatorTypeDef",
+AwsCloudFrontDistributionOriginGroupsExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupsExtraOutputTypeDef",
+    {
+        "Items": NotRequired[List[AwsCloudFrontDistributionOriginGroupExtraOutputTypeDef]],
+    },
+)
+AwsCloudFrontDistributionOriginGroupsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupsOutputTypeDef",
     {
-        "Items": NotRequired[List[AwsCloudFrontDistributionOriginGroupPaginatorTypeDef]],
+        "Items": NotRequired[List[AwsCloudFrontDistributionOriginGroupOutputTypeDef]],
     },
 )
 AwsCloudFrontDistributionOriginGroupsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupsTypeDef",
     {
         "Items": NotRequired[Sequence[AwsCloudFrontDistributionOriginGroupTypeDef]],
     },
 )
-AwsDynamoDbTableDetailsPaginatorTypeDef = TypedDict(
-    "AwsDynamoDbTableDetailsPaginatorTypeDef",
+AwsDynamoDbTableDetailsExtraOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableDetailsExtraOutputTypeDef",
+    {
+        "AttributeDefinitions": NotRequired[List[AwsDynamoDbTableAttributeDefinitionTypeDef]],
+        "BillingModeSummary": NotRequired[AwsDynamoDbTableBillingModeSummaryTypeDef],
+        "CreationDateTime": NotRequired[str],
+        "GlobalSecondaryIndexes": NotRequired[
+            List[AwsDynamoDbTableGlobalSecondaryIndexExtraOutputTypeDef]
+        ],
+        "GlobalTableVersion": NotRequired[str],
+        "ItemCount": NotRequired[int],
+        "KeySchema": NotRequired[List[AwsDynamoDbTableKeySchemaTypeDef]],
+        "LatestStreamArn": NotRequired[str],
+        "LatestStreamLabel": NotRequired[str],
+        "LocalSecondaryIndexes": NotRequired[
+            List[AwsDynamoDbTableLocalSecondaryIndexExtraOutputTypeDef]
+        ],
+        "ProvisionedThroughput": NotRequired[AwsDynamoDbTableProvisionedThroughputTypeDef],
+        "Replicas": NotRequired[List[AwsDynamoDbTableReplicaExtraOutputTypeDef]],
+        "RestoreSummary": NotRequired[AwsDynamoDbTableRestoreSummaryTypeDef],
+        "SseDescription": NotRequired[AwsDynamoDbTableSseDescriptionTypeDef],
+        "StreamSpecification": NotRequired[AwsDynamoDbTableStreamSpecificationTypeDef],
+        "TableId": NotRequired[str],
+        "TableName": NotRequired[str],
+        "TableSizeBytes": NotRequired[int],
+        "TableStatus": NotRequired[str],
+        "DeletionProtectionEnabled": NotRequired[bool],
+    },
+)
+AwsDynamoDbTableDetailsOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableDetailsOutputTypeDef",
     {
         "AttributeDefinitions": NotRequired[List[AwsDynamoDbTableAttributeDefinitionTypeDef]],
         "BillingModeSummary": NotRequired[AwsDynamoDbTableBillingModeSummaryTypeDef],
         "CreationDateTime": NotRequired[str],
         "GlobalSecondaryIndexes": NotRequired[
-            List[AwsDynamoDbTableGlobalSecondaryIndexPaginatorTypeDef]
+            List[AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef]
         ],
         "GlobalTableVersion": NotRequired[str],
         "ItemCount": NotRequired[int],
         "KeySchema": NotRequired[List[AwsDynamoDbTableKeySchemaTypeDef]],
         "LatestStreamArn": NotRequired[str],
         "LatestStreamLabel": NotRequired[str],
         "LocalSecondaryIndexes": NotRequired[
-            List[AwsDynamoDbTableLocalSecondaryIndexPaginatorTypeDef]
+            List[AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef]
         ],
         "ProvisionedThroughput": NotRequired[AwsDynamoDbTableProvisionedThroughputTypeDef],
-        "Replicas": NotRequired[List[AwsDynamoDbTableReplicaPaginatorTypeDef]],
+        "Replicas": NotRequired[List[AwsDynamoDbTableReplicaOutputTypeDef]],
         "RestoreSummary": NotRequired[AwsDynamoDbTableRestoreSummaryTypeDef],
         "SseDescription": NotRequired[AwsDynamoDbTableSseDescriptionTypeDef],
         "StreamSpecification": NotRequired[AwsDynamoDbTableStreamSpecificationTypeDef],
         "TableId": NotRequired[str],
         "TableName": NotRequired[str],
         "TableSizeBytes": NotRequired[int],
         "TableStatus": NotRequired[str],
@@ -10448,36 +13264,63 @@
         "TableId": NotRequired[str],
         "TableName": NotRequired[str],
         "TableSizeBytes": NotRequired[int],
         "TableStatus": NotRequired[str],
         "DeletionProtectionEnabled": NotRequired[bool],
     },
 )
-AwsEc2LaunchTemplateDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDetailsPaginatorTypeDef",
+AwsEc2LaunchTemplateDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDetailsExtraOutputTypeDef",
     {
         "LaunchTemplateName": NotRequired[str],
         "Id": NotRequired[str],
-        "LaunchTemplateData": NotRequired[AwsEc2LaunchTemplateDataDetailsPaginatorTypeDef],
+        "LaunchTemplateData": NotRequired[AwsEc2LaunchTemplateDataDetailsExtraOutputTypeDef],
+        "DefaultVersionNumber": NotRequired[int],
+        "LatestVersionNumber": NotRequired[int],
+    },
+)
+AwsEc2LaunchTemplateDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDetailsOutputTypeDef",
+    {
+        "LaunchTemplateName": NotRequired[str],
+        "Id": NotRequired[str],
+        "LaunchTemplateData": NotRequired[AwsEc2LaunchTemplateDataDetailsOutputTypeDef],
         "DefaultVersionNumber": NotRequired[int],
         "LatestVersionNumber": NotRequired[int],
     },
 )
 AwsEc2LaunchTemplateDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDetailsTypeDef",
     {
         "LaunchTemplateName": NotRequired[str],
         "Id": NotRequired[str],
         "LaunchTemplateData": NotRequired[AwsEc2LaunchTemplateDataDetailsTypeDef],
         "DefaultVersionNumber": NotRequired[int],
         "LatestVersionNumber": NotRequired[int],
     },
 )
-AwsEcsClusterDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsClusterDetailsPaginatorTypeDef",
+AwsEcsClusterDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsClusterDetailsExtraOutputTypeDef",
+    {
+        "ClusterArn": NotRequired[str],
+        "ActiveServicesCount": NotRequired[int],
+        "CapacityProviders": NotRequired[List[str]],
+        "ClusterSettings": NotRequired[List[AwsEcsClusterClusterSettingsDetailsTypeDef]],
+        "Configuration": NotRequired[AwsEcsClusterConfigurationDetailsTypeDef],
+        "DefaultCapacityProviderStrategy": NotRequired[
+            List[AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef]
+        ],
+        "ClusterName": NotRequired[str],
+        "RegisteredContainerInstancesCount": NotRequired[int],
+        "RunningTasksCount": NotRequired[int],
+        "Status": NotRequired[str],
+    },
+)
+AwsEcsClusterDetailsOutputTypeDef = TypedDict(
+    "AwsEcsClusterDetailsOutputTypeDef",
     {
         "ClusterArn": NotRequired[str],
         "ActiveServicesCount": NotRequired[int],
         "CapacityProviders": NotRequired[List[str]],
         "ClusterSettings": NotRequired[List[AwsEcsClusterClusterSettingsDetailsTypeDef]],
         "Configuration": NotRequired[AwsEcsClusterConfigurationDetailsTypeDef],
         "DefaultCapacityProviderStrategy": NotRequired[
@@ -10502,19 +13345,19 @@
         ],
         "ClusterName": NotRequired[str],
         "RegisteredContainerInstancesCount": NotRequired[int],
         "RunningTasksCount": NotRequired[int],
         "Status": NotRequired[str],
     },
 )
-AwsEcsTaskDefinitionDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionDetailsExtraOutputTypeDef",
     {
         "ContainerDefinitions": NotRequired[
-            List[AwsEcsTaskDefinitionContainerDefinitionsDetailsPaginatorTypeDef]
+            List[AwsEcsTaskDefinitionContainerDefinitionsDetailsExtraOutputTypeDef]
         ],
         "Cpu": NotRequired[str],
         "ExecutionRoleArn": NotRequired[str],
         "Family": NotRequired[str],
         "InferenceAccelerators": NotRequired[
             List[AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef]
         ],
@@ -10522,19 +13365,47 @@
         "Memory": NotRequired[str],
         "NetworkMode": NotRequired[str],
         "PidMode": NotRequired[str],
         "PlacementConstraints": NotRequired[
             List[AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef]
         ],
         "ProxyConfiguration": NotRequired[
-            AwsEcsTaskDefinitionProxyConfigurationDetailsPaginatorTypeDef
+            AwsEcsTaskDefinitionProxyConfigurationDetailsExtraOutputTypeDef
         ],
         "RequiresCompatibilities": NotRequired[List[str]],
         "TaskRoleArn": NotRequired[str],
-        "Volumes": NotRequired[List[AwsEcsTaskDefinitionVolumesDetailsPaginatorTypeDef]],
+        "Volumes": NotRequired[List[AwsEcsTaskDefinitionVolumesDetailsExtraOutputTypeDef]],
+        "Status": NotRequired[str],
+    },
+)
+AwsEcsTaskDefinitionDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionDetailsOutputTypeDef",
+    {
+        "ContainerDefinitions": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef]
+        ],
+        "Cpu": NotRequired[str],
+        "ExecutionRoleArn": NotRequired[str],
+        "Family": NotRequired[str],
+        "InferenceAccelerators": NotRequired[
+            List[AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef]
+        ],
+        "IpcMode": NotRequired[str],
+        "Memory": NotRequired[str],
+        "NetworkMode": NotRequired[str],
+        "PidMode": NotRequired[str],
+        "PlacementConstraints": NotRequired[
+            List[AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef]
+        ],
+        "ProxyConfiguration": NotRequired[
+            AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef
+        ],
+        "RequiresCompatibilities": NotRequired[List[str]],
+        "TaskRoleArn": NotRequired[str],
+        "Volumes": NotRequired[List[AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef]],
         "Status": NotRequired[str],
     },
 )
 AwsEcsTaskDefinitionDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionDetailsTypeDef",
     {
         "ContainerDefinitions": NotRequired[
@@ -10556,16 +13427,32 @@
         "ProxyConfiguration": NotRequired[AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef],
         "RequiresCompatibilities": NotRequired[Sequence[str]],
         "TaskRoleArn": NotRequired[str],
         "Volumes": NotRequired[Sequence[AwsEcsTaskDefinitionVolumesDetailsTypeDef]],
         "Status": NotRequired[str],
     },
 )
-AwsEventsEndpointDetailsPaginatorTypeDef = TypedDict(
-    "AwsEventsEndpointDetailsPaginatorTypeDef",
+AwsEventsEndpointDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEventsEndpointDetailsExtraOutputTypeDef",
+    {
+        "Arn": NotRequired[str],
+        "Description": NotRequired[str],
+        "EndpointId": NotRequired[str],
+        "EndpointUrl": NotRequired[str],
+        "EventBuses": NotRequired[List[AwsEventsEndpointEventBusesDetailsTypeDef]],
+        "Name": NotRequired[str],
+        "ReplicationConfig": NotRequired[AwsEventsEndpointReplicationConfigDetailsTypeDef],
+        "RoleArn": NotRequired[str],
+        "RoutingConfig": NotRequired[AwsEventsEndpointRoutingConfigDetailsTypeDef],
+        "State": NotRequired[str],
+        "StateReason": NotRequired[str],
+    },
+)
+AwsEventsEndpointDetailsOutputTypeDef = TypedDict(
+    "AwsEventsEndpointDetailsOutputTypeDef",
     {
         "Arn": NotRequired[str],
         "Description": NotRequired[str],
         "EndpointId": NotRequired[str],
         "EndpointUrl": NotRequired[str],
         "EventBuses": NotRequired[List[AwsEventsEndpointEventBusesDetailsTypeDef]],
         "Name": NotRequired[str],
@@ -10601,23 +13488,36 @@
         "Kubernetes": NotRequired[AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef],
         "MalwareProtection": NotRequired[
             AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef
         ],
         "S3Logs": NotRequired[AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef],
     },
 )
-AwsMskClusterClusterInfoDetailsPaginatorTypeDef = TypedDict(
-    "AwsMskClusterClusterInfoDetailsPaginatorTypeDef",
+AwsMskClusterClusterInfoDetailsExtraOutputTypeDef = TypedDict(
+    "AwsMskClusterClusterInfoDetailsExtraOutputTypeDef",
     {
         "EncryptionInfo": NotRequired[AwsMskClusterClusterInfoEncryptionInfoDetailsTypeDef],
         "CurrentVersion": NotRequired[str],
         "NumberOfBrokerNodes": NotRequired[int],
         "ClusterName": NotRequired[str],
         "ClientAuthentication": NotRequired[
-            AwsMskClusterClusterInfoClientAuthenticationDetailsPaginatorTypeDef
+            AwsMskClusterClusterInfoClientAuthenticationDetailsExtraOutputTypeDef
+        ],
+        "EnhancedMonitoring": NotRequired[str],
+    },
+)
+AwsMskClusterClusterInfoDetailsOutputTypeDef = TypedDict(
+    "AwsMskClusterClusterInfoDetailsOutputTypeDef",
+    {
+        "EncryptionInfo": NotRequired[AwsMskClusterClusterInfoEncryptionInfoDetailsTypeDef],
+        "CurrentVersion": NotRequired[str],
+        "NumberOfBrokerNodes": NotRequired[int],
+        "ClusterName": NotRequired[str],
+        "ClientAuthentication": NotRequired[
+            AwsMskClusterClusterInfoClientAuthenticationDetailsOutputTypeDef
         ],
         "EnhancedMonitoring": NotRequired[str],
     },
 )
 AwsMskClusterClusterInfoDetailsTypeDef = TypedDict(
     "AwsMskClusterClusterInfoDetailsTypeDef",
     {
@@ -10627,16 +13527,16 @@
         "ClusterName": NotRequired[str],
         "ClientAuthentication": NotRequired[
             AwsMskClusterClusterInfoClientAuthenticationDetailsTypeDef
         ],
         "EnhancedMonitoring": NotRequired[str],
     },
 )
-AwsRdsDbInstanceDetailsPaginatorTypeDef = TypedDict(
-    "AwsRdsDbInstanceDetailsPaginatorTypeDef",
+AwsRdsDbInstanceDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbInstanceDetailsExtraOutputTypeDef",
     {
         "AssociatedRoles": NotRequired[List[AwsRdsDbInstanceAssociatedRoleTypeDef]],
         "CACertificateIdentifier": NotRequired[str],
         "DBClusterIdentifier": NotRequired[str],
         "DBInstanceIdentifier": NotRequired[str],
         "DBInstanceClass": NotRequired[str],
         "DbInstancePort": NotRequired[int],
@@ -10659,17 +13559,79 @@
         "MasterUsername": NotRequired[str],
         "AllocatedStorage": NotRequired[int],
         "PreferredBackupWindow": NotRequired[str],
         "BackupRetentionPeriod": NotRequired[int],
         "DbSecurityGroups": NotRequired[List[str]],
         "DbParameterGroups": NotRequired[List[AwsRdsDbParameterGroupTypeDef]],
         "AvailabilityZone": NotRequired[str],
-        "DbSubnetGroup": NotRequired[AwsRdsDbSubnetGroupPaginatorTypeDef],
+        "DbSubnetGroup": NotRequired[AwsRdsDbSubnetGroupExtraOutputTypeDef],
         "PreferredMaintenanceWindow": NotRequired[str],
-        "PendingModifiedValues": NotRequired[AwsRdsDbPendingModifiedValuesPaginatorTypeDef],
+        "PendingModifiedValues": NotRequired[AwsRdsDbPendingModifiedValuesExtraOutputTypeDef],
+        "LatestRestorableTime": NotRequired[str],
+        "AutoMinorVersionUpgrade": NotRequired[bool],
+        "ReadReplicaSourceDBInstanceIdentifier": NotRequired[str],
+        "ReadReplicaDBInstanceIdentifiers": NotRequired[List[str]],
+        "ReadReplicaDBClusterIdentifiers": NotRequired[List[str]],
+        "LicenseModel": NotRequired[str],
+        "Iops": NotRequired[int],
+        "OptionGroupMemberships": NotRequired[List[AwsRdsDbOptionGroupMembershipTypeDef]],
+        "CharacterSetName": NotRequired[str],
+        "SecondaryAvailabilityZone": NotRequired[str],
+        "StatusInfos": NotRequired[List[AwsRdsDbStatusInfoTypeDef]],
+        "StorageType": NotRequired[str],
+        "DomainMemberships": NotRequired[List[AwsRdsDbDomainMembershipTypeDef]],
+        "CopyTagsToSnapshot": NotRequired[bool],
+        "MonitoringInterval": NotRequired[int],
+        "MonitoringRoleArn": NotRequired[str],
+        "PromotionTier": NotRequired[int],
+        "Timezone": NotRequired[str],
+        "PerformanceInsightsEnabled": NotRequired[bool],
+        "PerformanceInsightsKmsKeyId": NotRequired[str],
+        "PerformanceInsightsRetentionPeriod": NotRequired[int],
+        "EnabledCloudWatchLogsExports": NotRequired[List[str]],
+        "ProcessorFeatures": NotRequired[List[AwsRdsDbProcessorFeatureTypeDef]],
+        "ListenerEndpoint": NotRequired[AwsRdsDbInstanceEndpointTypeDef],
+        "MaxAllocatedStorage": NotRequired[int],
+    },
+)
+AwsRdsDbInstanceDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbInstanceDetailsOutputTypeDef",
+    {
+        "AssociatedRoles": NotRequired[List[AwsRdsDbInstanceAssociatedRoleTypeDef]],
+        "CACertificateIdentifier": NotRequired[str],
+        "DBClusterIdentifier": NotRequired[str],
+        "DBInstanceIdentifier": NotRequired[str],
+        "DBInstanceClass": NotRequired[str],
+        "DbInstancePort": NotRequired[int],
+        "DbiResourceId": NotRequired[str],
+        "DBName": NotRequired[str],
+        "DeletionProtection": NotRequired[bool],
+        "Endpoint": NotRequired[AwsRdsDbInstanceEndpointTypeDef],
+        "Engine": NotRequired[str],
+        "EngineVersion": NotRequired[str],
+        "IAMDatabaseAuthenticationEnabled": NotRequired[bool],
+        "InstanceCreateTime": NotRequired[str],
+        "KmsKeyId": NotRequired[str],
+        "PubliclyAccessible": NotRequired[bool],
+        "StorageEncrypted": NotRequired[bool],
+        "TdeCredentialArn": NotRequired[str],
+        "VpcSecurityGroups": NotRequired[List[AwsRdsDbInstanceVpcSecurityGroupTypeDef]],
+        "MultiAz": NotRequired[bool],
+        "EnhancedMonitoringResourceArn": NotRequired[str],
+        "DbInstanceStatus": NotRequired[str],
+        "MasterUsername": NotRequired[str],
+        "AllocatedStorage": NotRequired[int],
+        "PreferredBackupWindow": NotRequired[str],
+        "BackupRetentionPeriod": NotRequired[int],
+        "DbSecurityGroups": NotRequired[List[str]],
+        "DbParameterGroups": NotRequired[List[AwsRdsDbParameterGroupTypeDef]],
+        "AvailabilityZone": NotRequired[str],
+        "DbSubnetGroup": NotRequired[AwsRdsDbSubnetGroupOutputTypeDef],
+        "PreferredMaintenanceWindow": NotRequired[str],
+        "PendingModifiedValues": NotRequired[AwsRdsDbPendingModifiedValuesOutputTypeDef],
         "LatestRestorableTime": NotRequired[str],
         "AutoMinorVersionUpgrade": NotRequired[bool],
         "ReadReplicaSourceDBInstanceIdentifier": NotRequired[str],
         "ReadReplicaDBInstanceIdentifiers": NotRequired[List[str]],
         "ReadReplicaDBClusterIdentifiers": NotRequired[List[str]],
         "LicenseModel": NotRequired[str],
         "Iops": NotRequired[int],
@@ -10751,54 +13713,88 @@
         "PerformanceInsightsRetentionPeriod": NotRequired[int],
         "EnabledCloudWatchLogsExports": NotRequired[Sequence[str]],
         "ProcessorFeatures": NotRequired[Sequence[AwsRdsDbProcessorFeatureTypeDef]],
         "ListenerEndpoint": NotRequired[AwsRdsDbInstanceEndpointTypeDef],
         "MaxAllocatedStorage": NotRequired[int],
     },
 )
-AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsPaginatorTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsPaginatorTypeDef",
+AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsExtraOutputTypeDef",
+    {
+        "Predicate": NotRequired[
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef",
     {
         "Predicate": NotRequired[
-            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsPaginatorTypeDef
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef
         ],
     },
 )
 AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
     {
         "Predicate": NotRequired[
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef
         ],
     },
 )
-AwsS3BucketNotificationConfigurationDetailPaginatorTypeDef = TypedDict(
-    "AwsS3BucketNotificationConfigurationDetailPaginatorTypeDef",
+AwsS3BucketNotificationConfigurationDetailExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationDetailExtraOutputTypeDef",
     {
         "Events": NotRequired[List[str]],
-        "Filter": NotRequired[AwsS3BucketNotificationConfigurationFilterPaginatorTypeDef],
+        "Filter": NotRequired[AwsS3BucketNotificationConfigurationFilterExtraOutputTypeDef],
+        "Destination": NotRequired[str],
+        "Type": NotRequired[str],
+    },
+)
+AwsS3BucketNotificationConfigurationDetailOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationDetailOutputTypeDef",
+    {
+        "Events": NotRequired[List[str]],
+        "Filter": NotRequired[AwsS3BucketNotificationConfigurationFilterOutputTypeDef],
         "Destination": NotRequired[str],
         "Type": NotRequired[str],
     },
 )
 AwsS3BucketNotificationConfigurationDetailTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
     {
         "Events": NotRequired[Sequence[str]],
         "Filter": NotRequired[AwsS3BucketNotificationConfigurationFilterTypeDef],
         "Destination": NotRequired[str],
         "Type": NotRequired[str],
     },
 )
-AwsStepFunctionStateMachineDetailsPaginatorTypeDef = TypedDict(
-    "AwsStepFunctionStateMachineDetailsPaginatorTypeDef",
+AwsStepFunctionStateMachineDetailsExtraOutputTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineDetailsExtraOutputTypeDef",
     {
         "Label": NotRequired[str],
         "LoggingConfiguration": NotRequired[
-            AwsStepFunctionStateMachineLoggingConfigurationDetailsPaginatorTypeDef
+            AwsStepFunctionStateMachineLoggingConfigurationDetailsExtraOutputTypeDef
+        ],
+        "Name": NotRequired[str],
+        "RoleArn": NotRequired[str],
+        "StateMachineArn": NotRequired[str],
+        "Status": NotRequired[str],
+        "TracingConfiguration": NotRequired[
+            AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef
+        ],
+        "Type": NotRequired[str],
+    },
+)
+AwsStepFunctionStateMachineDetailsOutputTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineDetailsOutputTypeDef",
+    {
+        "Label": NotRequired[str],
+        "LoggingConfiguration": NotRequired[
+            AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef
         ],
         "Name": NotRequired[str],
         "RoleArn": NotRequired[str],
         "StateMachineArn": NotRequired[str],
         "Status": NotRequired[str],
         "TracingConfiguration": NotRequired[
             AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef
@@ -10819,28 +13815,44 @@
         "Status": NotRequired[str],
         "TracingConfiguration": NotRequired[
             AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef
         ],
         "Type": NotRequired[str],
     },
 )
-AwsWafv2RulesActionDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2RulesActionDetailsPaginatorTypeDef",
+AwsWafv2RulesActionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionDetailsExtraOutputTypeDef",
+    {
+        "Allow": NotRequired[AwsWafv2ActionAllowDetailsExtraOutputTypeDef],
+        "Block": NotRequired[AwsWafv2ActionBlockDetailsExtraOutputTypeDef],
+        "Captcha": NotRequired[AwsWafv2RulesActionCaptchaDetailsExtraOutputTypeDef],
+        "Count": NotRequired[AwsWafv2RulesActionCountDetailsExtraOutputTypeDef],
+    },
+)
+AwsWafv2WebAclActionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2WebAclActionDetailsExtraOutputTypeDef",
     {
-        "Allow": NotRequired[AwsWafv2ActionAllowDetailsPaginatorTypeDef],
-        "Block": NotRequired[AwsWafv2ActionBlockDetailsPaginatorTypeDef],
-        "Captcha": NotRequired[AwsWafv2RulesActionCaptchaDetailsPaginatorTypeDef],
-        "Count": NotRequired[AwsWafv2RulesActionCountDetailsPaginatorTypeDef],
+        "Allow": NotRequired[AwsWafv2ActionAllowDetailsExtraOutputTypeDef],
+        "Block": NotRequired[AwsWafv2ActionBlockDetailsExtraOutputTypeDef],
     },
 )
-AwsWafv2WebAclActionDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2WebAclActionDetailsPaginatorTypeDef",
+AwsWafv2RulesActionDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionDetailsOutputTypeDef",
     {
-        "Allow": NotRequired[AwsWafv2ActionAllowDetailsPaginatorTypeDef],
-        "Block": NotRequired[AwsWafv2ActionBlockDetailsPaginatorTypeDef],
+        "Allow": NotRequired[AwsWafv2ActionAllowDetailsOutputTypeDef],
+        "Block": NotRequired[AwsWafv2ActionBlockDetailsOutputTypeDef],
+        "Captcha": NotRequired[AwsWafv2RulesActionCaptchaDetailsOutputTypeDef],
+        "Count": NotRequired[AwsWafv2RulesActionCountDetailsOutputTypeDef],
+    },
+)
+AwsWafv2WebAclActionDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2WebAclActionDetailsOutputTypeDef",
+    {
+        "Allow": NotRequired[AwsWafv2ActionAllowDetailsOutputTypeDef],
+        "Block": NotRequired[AwsWafv2ActionBlockDetailsOutputTypeDef],
     },
 )
 AwsWafv2RulesActionDetailsTypeDef = TypedDict(
     "AwsWafv2RulesActionDetailsTypeDef",
     {
         "Allow": NotRequired[AwsWafv2ActionAllowDetailsTypeDef],
         "Block": NotRequired[AwsWafv2ActionBlockDetailsTypeDef],
@@ -10883,47 +13895,49 @@
     {
         "RuleArn": NotRequired[str],
         "RuleStatus": NotRequired[RuleStatusType],
         "RuleOrder": NotRequired[int],
         "RuleName": NotRequired[str],
         "Description": NotRequired[str],
         "IsTerminal": NotRequired[bool],
-        "Criteria": NotRequired[AutomationRulesFindingFiltersTypeDef],
-        "Actions": NotRequired[List[AutomationRulesActionTypeDef]],
+        "Criteria": NotRequired[AutomationRulesFindingFiltersOutputTypeDef],
+        "Actions": NotRequired[List[AutomationRulesActionOutputTypeDef]],
         "CreatedAt": NotRequired[datetime],
         "UpdatedAt": NotRequired[datetime],
         "CreatedBy": NotRequired[str],
     },
 )
-CreateAutomationRuleRequestRequestTypeDef = TypedDict(
-    "CreateAutomationRuleRequestRequestTypeDef",
-    {
-        "RuleOrder": int,
-        "RuleName": str,
-        "Description": str,
-        "Criteria": AutomationRulesFindingFiltersTypeDef,
-        "Actions": Sequence[AutomationRulesActionTypeDef],
-        "Tags": NotRequired[Mapping[str, str]],
-        "RuleStatus": NotRequired[RuleStatusType],
-        "IsTerminal": NotRequired[bool],
-    },
-)
+AutomationRulesFindingFiltersUnionTypeDef = Union[
+    AutomationRulesFindingFiltersTypeDef, AutomationRulesFindingFiltersOutputTypeDef
+]
 UpdateAutomationRulesRequestItemTypeDef = TypedDict(
     "UpdateAutomationRulesRequestItemTypeDef",
     {
         "RuleArn": str,
         "RuleStatus": NotRequired[RuleStatusType],
         "RuleOrder": NotRequired[int],
         "Description": NotRequired[str],
         "RuleName": NotRequired[str],
         "IsTerminal": NotRequired[bool],
         "Criteria": NotRequired[AutomationRulesFindingFiltersTypeDef],
         "Actions": NotRequired[Sequence[AutomationRulesActionTypeDef]],
     },
 )
+InsightTypeDef = TypedDict(
+    "InsightTypeDef",
+    {
+        "InsightArn": str,
+        "Name": str,
+        "Filters": AwsSecurityFindingFiltersOutputTypeDef,
+        "GroupByAttribute": str,
+    },
+)
+AwsSecurityFindingFiltersUnionTypeDef = Union[
+    AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersExtraOutputTypeDef
+]
 CreateInsightRequestRequestTypeDef = TypedDict(
     "CreateInsightRequestRequestTypeDef",
     {
         "Name": str,
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "GroupByAttribute": str,
     },
@@ -10941,23 +13955,14 @@
     {
         "Filters": NotRequired[AwsSecurityFindingFiltersTypeDef],
         "SortCriteria": NotRequired[Sequence[SortCriterionTypeDef]],
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
     },
 )
-InsightTypeDef = TypedDict(
-    "InsightTypeDef",
-    {
-        "InsightArn": str,
-        "Name": str,
-        "Filters": AwsSecurityFindingFiltersTypeDef,
-        "GroupByAttribute": str,
-    },
-)
 UpdateFindingsRequestRequestTypeDef = TypedDict(
     "UpdateFindingsRequestRequestTypeDef",
     {
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "Note": NotRequired[NoteUpdateTypeDef],
         "RecordState": NotRequired[RecordStateType],
     },
@@ -10967,47 +13972,73 @@
     {
         "InsightArn": str,
         "Name": NotRequired[str],
         "Filters": NotRequired[AwsSecurityFindingFiltersTypeDef],
         "GroupByAttribute": NotRequired[str],
     },
 )
-NetworkPathComponentPaginatorTypeDef = TypedDict(
-    "NetworkPathComponentPaginatorTypeDef",
+NetworkPathComponentExtraOutputTypeDef = TypedDict(
+    "NetworkPathComponentExtraOutputTypeDef",
+    {
+        "ComponentId": NotRequired[str],
+        "ComponentType": NotRequired[str],
+        "Egress": NotRequired[NetworkHeaderExtraOutputTypeDef],
+        "Ingress": NotRequired[NetworkHeaderExtraOutputTypeDef],
+    },
+)
+NetworkPathComponentOutputTypeDef = TypedDict(
+    "NetworkPathComponentOutputTypeDef",
     {
         "ComponentId": NotRequired[str],
         "ComponentType": NotRequired[str],
-        "Egress": NotRequired[NetworkHeaderPaginatorTypeDef],
-        "Ingress": NotRequired[NetworkHeaderPaginatorTypeDef],
+        "Egress": NotRequired[NetworkHeaderOutputTypeDef],
+        "Ingress": NotRequired[NetworkHeaderOutputTypeDef],
     },
 )
 NetworkPathComponentTypeDef = TypedDict(
     "NetworkPathComponentTypeDef",
     {
         "ComponentId": NotRequired[str],
         "ComponentType": NotRequired[str],
         "Egress": NotRequired[NetworkHeaderTypeDef],
         "Ingress": NotRequired[NetworkHeaderTypeDef],
     },
 )
-CustomDataIdentifiersDetectionsPaginatorTypeDef = TypedDict(
-    "CustomDataIdentifiersDetectionsPaginatorTypeDef",
+CustomDataIdentifiersDetectionsExtraOutputTypeDef = TypedDict(
+    "CustomDataIdentifiersDetectionsExtraOutputTypeDef",
     {
         "Count": NotRequired[int],
         "Arn": NotRequired[str],
         "Name": NotRequired[str],
-        "Occurrences": NotRequired[OccurrencesPaginatorTypeDef],
+        "Occurrences": NotRequired[OccurrencesExtraOutputTypeDef],
     },
 )
-SensitiveDataDetectionsPaginatorTypeDef = TypedDict(
-    "SensitiveDataDetectionsPaginatorTypeDef",
+SensitiveDataDetectionsExtraOutputTypeDef = TypedDict(
+    "SensitiveDataDetectionsExtraOutputTypeDef",
     {
         "Count": NotRequired[int],
         "Type": NotRequired[str],
-        "Occurrences": NotRequired[OccurrencesPaginatorTypeDef],
+        "Occurrences": NotRequired[OccurrencesExtraOutputTypeDef],
+    },
+)
+CustomDataIdentifiersDetectionsOutputTypeDef = TypedDict(
+    "CustomDataIdentifiersDetectionsOutputTypeDef",
+    {
+        "Count": NotRequired[int],
+        "Arn": NotRequired[str],
+        "Name": NotRequired[str],
+        "Occurrences": NotRequired[OccurrencesOutputTypeDef],
+    },
+)
+SensitiveDataDetectionsOutputTypeDef = TypedDict(
+    "SensitiveDataDetectionsOutputTypeDef",
+    {
+        "Count": NotRequired[int],
+        "Type": NotRequired[str],
+        "Occurrences": NotRequired[OccurrencesOutputTypeDef],
     },
 )
 CustomDataIdentifiersDetectionsTypeDef = TypedDict(
     "CustomDataIdentifiersDetectionsTypeDef",
     {
         "Count": NotRequired[int],
         "Arn": NotRequired[str],
@@ -11019,57 +14050,96 @@
     "SensitiveDataDetectionsTypeDef",
     {
         "Count": NotRequired[int],
         "Type": NotRequired[str],
         "Occurrences": NotRequired[OccurrencesTypeDef],
     },
 )
-SecurityControlsConfigurationTypeDef = TypedDict(
-    "SecurityControlsConfigurationTypeDef",
+SecurityControlsConfigurationOutputTypeDef = TypedDict(
+    "SecurityControlsConfigurationOutputTypeDef",
     {
-        "EnabledSecurityControlIdentifiers": NotRequired[Sequence[str]],
-        "DisabledSecurityControlIdentifiers": NotRequired[Sequence[str]],
+        "EnabledSecurityControlIdentifiers": NotRequired[List[str]],
+        "DisabledSecurityControlIdentifiers": NotRequired[List[str]],
         "SecurityControlCustomParameters": NotRequired[
-            Sequence[SecurityControlCustomParameterTypeDef]
+            List[SecurityControlCustomParameterOutputTypeDef]
         ],
     },
 )
 BatchGetSecurityControlsResponseTypeDef = TypedDict(
     "BatchGetSecurityControlsResponseTypeDef",
     {
         "SecurityControls": List[SecurityControlTypeDef],
         "UnprocessedIds": List[UnprocessedSecurityControlTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-RuleGroupSourceStatelessRulesDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRulesDetailsPaginatorTypeDef",
+UpdateSecurityControlRequestRequestTypeDef = TypedDict(
+    "UpdateSecurityControlRequestRequestTypeDef",
+    {
+        "SecurityControlId": str,
+        "Parameters": Mapping[str, ParameterConfigurationUnionTypeDef],
+        "LastUpdateReason": NotRequired[str],
+    },
+)
+SecurityControlsConfigurationTypeDef = TypedDict(
+    "SecurityControlsConfigurationTypeDef",
+    {
+        "EnabledSecurityControlIdentifiers": NotRequired[Sequence[str]],
+        "DisabledSecurityControlIdentifiers": NotRequired[Sequence[str]],
+        "SecurityControlCustomParameters": NotRequired[
+            Sequence[SecurityControlCustomParameterTypeDef]
+        ],
+    },
+)
+RuleGroupSourceStatelessRulesDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRulesDetailsExtraOutputTypeDef",
+    {
+        "Priority": NotRequired[int],
+        "RuleDefinition": NotRequired[RuleGroupSourceStatelessRuleDefinitionExtraOutputTypeDef],
+    },
+)
+RuleGroupSourceStatelessRulesDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRulesDetailsOutputTypeDef",
     {
         "Priority": NotRequired[int],
-        "RuleDefinition": NotRequired[RuleGroupSourceStatelessRuleDefinitionPaginatorTypeDef],
+        "RuleDefinition": NotRequired[RuleGroupSourceStatelessRuleDefinitionOutputTypeDef],
     },
 )
 RuleGroupSourceStatelessRulesDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRulesDetailsTypeDef",
     {
         "Priority": NotRequired[int],
         "RuleDefinition": NotRequired[RuleGroupSourceStatelessRuleDefinitionTypeDef],
     },
 )
-FirewallPolicyStatelessCustomActionsDetailsPaginatorTypeDef = TypedDict(
-    "FirewallPolicyStatelessCustomActionsDetailsPaginatorTypeDef",
+FirewallPolicyStatelessCustomActionsDetailsExtraOutputTypeDef = TypedDict(
+    "FirewallPolicyStatelessCustomActionsDetailsExtraOutputTypeDef",
+    {
+        "ActionDefinition": NotRequired[StatelessCustomActionDefinitionExtraOutputTypeDef],
+        "ActionName": NotRequired[str],
+    },
+)
+RuleGroupSourceCustomActionsDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceCustomActionsDetailsExtraOutputTypeDef",
+    {
+        "ActionDefinition": NotRequired[StatelessCustomActionDefinitionExtraOutputTypeDef],
+        "ActionName": NotRequired[str],
+    },
+)
+FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef = TypedDict(
+    "FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef",
     {
-        "ActionDefinition": NotRequired[StatelessCustomActionDefinitionPaginatorTypeDef],
+        "ActionDefinition": NotRequired[StatelessCustomActionDefinitionOutputTypeDef],
         "ActionName": NotRequired[str],
     },
 )
-RuleGroupSourceCustomActionsDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceCustomActionsDetailsPaginatorTypeDef",
+RuleGroupSourceCustomActionsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceCustomActionsDetailsOutputTypeDef",
     {
-        "ActionDefinition": NotRequired[StatelessCustomActionDefinitionPaginatorTypeDef],
+        "ActionDefinition": NotRequired[StatelessCustomActionDefinitionOutputTypeDef],
         "ActionName": NotRequired[str],
     },
 )
 FirewallPolicyStatelessCustomActionsDetailsTypeDef = TypedDict(
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     {
         "ActionDefinition": NotRequired[StatelessCustomActionDefinitionTypeDef],
@@ -11079,64 +14149,113 @@
 RuleGroupSourceCustomActionsDetailsTypeDef = TypedDict(
     "RuleGroupSourceCustomActionsDetailsTypeDef",
     {
         "ActionDefinition": NotRequired[StatelessCustomActionDefinitionTypeDef],
         "ActionName": NotRequired[str],
     },
 )
-ActionPaginatorTypeDef = TypedDict(
-    "ActionPaginatorTypeDef",
+ActionExtraOutputTypeDef = TypedDict(
+    "ActionExtraOutputTypeDef",
+    {
+        "ActionType": NotRequired[str],
+        "NetworkConnectionAction": NotRequired[NetworkConnectionActionTypeDef],
+        "AwsApiCallAction": NotRequired[AwsApiCallActionExtraOutputTypeDef],
+        "DnsRequestAction": NotRequired[DnsRequestActionTypeDef],
+        "PortProbeAction": NotRequired[PortProbeActionExtraOutputTypeDef],
+    },
+)
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
     {
         "ActionType": NotRequired[str],
         "NetworkConnectionAction": NotRequired[NetworkConnectionActionTypeDef],
-        "AwsApiCallAction": NotRequired[AwsApiCallActionPaginatorTypeDef],
+        "AwsApiCallAction": NotRequired[AwsApiCallActionOutputTypeDef],
         "DnsRequestAction": NotRequired[DnsRequestActionTypeDef],
-        "PortProbeAction": NotRequired[PortProbeActionPaginatorTypeDef],
+        "PortProbeAction": NotRequired[PortProbeActionOutputTypeDef],
     },
 )
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ActionType": NotRequired[str],
         "NetworkConnectionAction": NotRequired[NetworkConnectionActionTypeDef],
         "AwsApiCallAction": NotRequired[AwsApiCallActionTypeDef],
         "DnsRequestAction": NotRequired[DnsRequestActionTypeDef],
         "PortProbeAction": NotRequired[PortProbeActionTypeDef],
     },
 )
-AwsBackupBackupPlanDetailsPaginatorTypeDef = TypedDict(
-    "AwsBackupBackupPlanDetailsPaginatorTypeDef",
+CreateAutomationRuleRequestRequestTypeDef = TypedDict(
+    "CreateAutomationRuleRequestRequestTypeDef",
     {
-        "BackupPlan": NotRequired[AwsBackupBackupPlanBackupPlanDetailsPaginatorTypeDef],
+        "RuleOrder": int,
+        "RuleName": str,
+        "Description": str,
+        "Criteria": AutomationRulesFindingFiltersTypeDef,
+        "Actions": Sequence[AutomationRulesActionUnionTypeDef],
+        "Tags": NotRequired[Mapping[str, str]],
+        "RuleStatus": NotRequired[RuleStatusType],
+        "IsTerminal": NotRequired[bool],
+    },
+)
+AwsBackupBackupPlanDetailsExtraOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanDetailsExtraOutputTypeDef",
+    {
+        "BackupPlan": NotRequired[AwsBackupBackupPlanBackupPlanDetailsExtraOutputTypeDef],
+        "BackupPlanArn": NotRequired[str],
+        "BackupPlanId": NotRequired[str],
+        "VersionId": NotRequired[str],
+    },
+)
+AwsBackupBackupPlanDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanDetailsOutputTypeDef",
+    {
+        "BackupPlan": NotRequired[AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef],
         "BackupPlanArn": NotRequired[str],
         "BackupPlanId": NotRequired[str],
         "VersionId": NotRequired[str],
     },
 )
 AwsBackupBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanDetailsTypeDef",
     {
         "BackupPlan": NotRequired[AwsBackupBackupPlanBackupPlanDetailsTypeDef],
         "BackupPlanArn": NotRequired[str],
         "BackupPlanId": NotRequired[str],
         "VersionId": NotRequired[str],
     },
 )
-AwsCloudFrontDistributionDetailsPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionDetailsPaginatorTypeDef",
+AwsCloudFrontDistributionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionDetailsExtraOutputTypeDef",
     {
-        "CacheBehaviors": NotRequired[AwsCloudFrontDistributionCacheBehaviorsPaginatorTypeDef],
+        "CacheBehaviors": NotRequired[AwsCloudFrontDistributionCacheBehaviorsExtraOutputTypeDef],
         "DefaultCacheBehavior": NotRequired[AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef],
         "DefaultRootObject": NotRequired[str],
         "DomainName": NotRequired[str],
         "ETag": NotRequired[str],
         "LastModifiedTime": NotRequired[str],
         "Logging": NotRequired[AwsCloudFrontDistributionLoggingTypeDef],
-        "Origins": NotRequired[AwsCloudFrontDistributionOriginsPaginatorTypeDef],
-        "OriginGroups": NotRequired[AwsCloudFrontDistributionOriginGroupsPaginatorTypeDef],
+        "Origins": NotRequired[AwsCloudFrontDistributionOriginsExtraOutputTypeDef],
+        "OriginGroups": NotRequired[AwsCloudFrontDistributionOriginGroupsExtraOutputTypeDef],
+        "ViewerCertificate": NotRequired[AwsCloudFrontDistributionViewerCertificateTypeDef],
+        "Status": NotRequired[str],
+        "WebAclId": NotRequired[str],
+    },
+)
+AwsCloudFrontDistributionDetailsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionDetailsOutputTypeDef",
+    {
+        "CacheBehaviors": NotRequired[AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef],
+        "DefaultCacheBehavior": NotRequired[AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef],
+        "DefaultRootObject": NotRequired[str],
+        "DomainName": NotRequired[str],
+        "ETag": NotRequired[str],
+        "LastModifiedTime": NotRequired[str],
+        "Logging": NotRequired[AwsCloudFrontDistributionLoggingTypeDef],
+        "Origins": NotRequired[AwsCloudFrontDistributionOriginsOutputTypeDef],
+        "OriginGroups": NotRequired[AwsCloudFrontDistributionOriginGroupsOutputTypeDef],
         "ViewerCertificate": NotRequired[AwsCloudFrontDistributionViewerCertificateTypeDef],
         "Status": NotRequired[str],
         "WebAclId": NotRequired[str],
     },
 )
 AwsCloudFrontDistributionDetailsTypeDef = TypedDict(
     "AwsCloudFrontDistributionDetailsTypeDef",
@@ -11151,16 +14270,26 @@
         "Origins": NotRequired[AwsCloudFrontDistributionOriginsTypeDef],
         "OriginGroups": NotRequired[AwsCloudFrontDistributionOriginGroupsTypeDef],
         "ViewerCertificate": NotRequired[AwsCloudFrontDistributionViewerCertificateTypeDef],
         "Status": NotRequired[str],
         "WebAclId": NotRequired[str],
     },
 )
-AwsGuardDutyDetectorDetailsPaginatorTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDetailsPaginatorTypeDef",
+AwsGuardDutyDetectorDetailsExtraOutputTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDetailsExtraOutputTypeDef",
+    {
+        "DataSources": NotRequired[AwsGuardDutyDetectorDataSourcesDetailsTypeDef],
+        "Features": NotRequired[List[AwsGuardDutyDetectorFeaturesDetailsTypeDef]],
+        "FindingPublishingFrequency": NotRequired[str],
+        "ServiceRole": NotRequired[str],
+        "Status": NotRequired[str],
+    },
+)
+AwsGuardDutyDetectorDetailsOutputTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDetailsOutputTypeDef",
     {
         "DataSources": NotRequired[AwsGuardDutyDetectorDataSourcesDetailsTypeDef],
         "Features": NotRequired[List[AwsGuardDutyDetectorFeaturesDetailsTypeDef]],
         "FindingPublishingFrequency": NotRequired[str],
         "ServiceRole": NotRequired[str],
         "Status": NotRequired[str],
     },
@@ -11171,37 +14300,69 @@
         "DataSources": NotRequired[AwsGuardDutyDetectorDataSourcesDetailsTypeDef],
         "Features": NotRequired[Sequence[AwsGuardDutyDetectorFeaturesDetailsTypeDef]],
         "FindingPublishingFrequency": NotRequired[str],
         "ServiceRole": NotRequired[str],
         "Status": NotRequired[str],
     },
 )
-AwsMskClusterDetailsPaginatorTypeDef = TypedDict(
-    "AwsMskClusterDetailsPaginatorTypeDef",
+AwsMskClusterDetailsExtraOutputTypeDef = TypedDict(
+    "AwsMskClusterDetailsExtraOutputTypeDef",
     {
-        "ClusterInfo": NotRequired[AwsMskClusterClusterInfoDetailsPaginatorTypeDef],
+        "ClusterInfo": NotRequired[AwsMskClusterClusterInfoDetailsExtraOutputTypeDef],
+    },
+)
+AwsMskClusterDetailsOutputTypeDef = TypedDict(
+    "AwsMskClusterDetailsOutputTypeDef",
+    {
+        "ClusterInfo": NotRequired[AwsMskClusterClusterInfoDetailsOutputTypeDef],
     },
 )
 AwsMskClusterDetailsTypeDef = TypedDict(
     "AwsMskClusterDetailsTypeDef",
     {
         "ClusterInfo": NotRequired[AwsMskClusterClusterInfoDetailsTypeDef],
     },
 )
-AwsS3BucketBucketLifecycleConfigurationRulesDetailsPaginatorTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsPaginatorTypeDef",
+AwsS3BucketBucketLifecycleConfigurationRulesDetailsExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsExtraOutputTypeDef",
+    {
+        "AbortIncompleteMultipartUpload": NotRequired[
+            AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
+        ],
+        "ExpirationDate": NotRequired[str],
+        "ExpirationInDays": NotRequired[int],
+        "ExpiredObjectDeleteMarker": NotRequired[bool],
+        "Filter": NotRequired[
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsExtraOutputTypeDef
+        ],
+        "ID": NotRequired[str],
+        "NoncurrentVersionExpirationInDays": NotRequired[int],
+        "NoncurrentVersionTransitions": NotRequired[
+            List[
+                AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef
+            ]
+        ],
+        "Prefix": NotRequired[str],
+        "Status": NotRequired[str],
+        "Transitions": NotRequired[
+            List[AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef]
+        ],
+    },
+)
+AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef",
     {
         "AbortIncompleteMultipartUpload": NotRequired[
             AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
         ],
         "ExpirationDate": NotRequired[str],
         "ExpirationInDays": NotRequired[int],
         "ExpiredObjectDeleteMarker": NotRequired[bool],
         "Filter": NotRequired[
-            AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsPaginatorTypeDef
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef
         ],
         "ID": NotRequired[str],
         "NoncurrentVersionExpirationInDays": NotRequired[int],
         "NoncurrentVersionTransitions": NotRequired[
             List[
                 AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef
             ]
@@ -11233,32 +14394,50 @@
         "Prefix": NotRequired[str],
         "Status": NotRequired[str],
         "Transitions": NotRequired[
             Sequence[AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef]
         ],
     },
 )
-AwsS3BucketNotificationConfigurationPaginatorTypeDef = TypedDict(
-    "AwsS3BucketNotificationConfigurationPaginatorTypeDef",
+AwsS3BucketNotificationConfigurationExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationExtraOutputTypeDef",
     {
         "Configurations": NotRequired[
-            List[AwsS3BucketNotificationConfigurationDetailPaginatorTypeDef]
+            List[AwsS3BucketNotificationConfigurationDetailExtraOutputTypeDef]
+        ],
+    },
+)
+AwsS3BucketNotificationConfigurationOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationOutputTypeDef",
+    {
+        "Configurations": NotRequired[
+            List[AwsS3BucketNotificationConfigurationDetailOutputTypeDef]
         ],
     },
 )
 AwsS3BucketNotificationConfigurationTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationTypeDef",
     {
         "Configurations": NotRequired[Sequence[AwsS3BucketNotificationConfigurationDetailTypeDef]],
     },
 )
-AwsWafv2RulesDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2RulesDetailsPaginatorTypeDef",
+AwsWafv2RulesDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2RulesDetailsExtraOutputTypeDef",
+    {
+        "Action": NotRequired[AwsWafv2RulesActionDetailsExtraOutputTypeDef],
+        "Name": NotRequired[str],
+        "OverrideAction": NotRequired[str],
+        "Priority": NotRequired[int],
+        "VisibilityConfig": NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],
+    },
+)
+AwsWafv2RulesDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesDetailsOutputTypeDef",
     {
-        "Action": NotRequired[AwsWafv2RulesActionDetailsPaginatorTypeDef],
+        "Action": NotRequired[AwsWafv2RulesActionDetailsOutputTypeDef],
         "Name": NotRequired[str],
         "OverrideAction": NotRequired[str],
         "Priority": NotRequired[int],
         "VisibilityConfig": NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],
     },
 )
 AwsWafv2RulesDetailsTypeDef = TypedDict(
@@ -11278,16 +14457,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListSecurityControlDefinitionsResponseTypeDef = TypedDict(
     "ListSecurityControlDefinitionsResponseTypeDef",
     {
         "SecurityControlDefinitions": List[SecurityControlDefinitionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 BatchGetAutomationRulesResponseTypeDef = TypedDict(
     "BatchGetAutomationRulesResponseTypeDef",
     {
         "Rules": List[AutomationRulesConfigTypeDef],
         "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
@@ -11300,30 +14479,45 @@
         "UpdateAutomationRulesRequestItems": Sequence[UpdateAutomationRulesRequestItemTypeDef],
     },
 )
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "Insights": List[InsightTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+CustomDataIdentifiersResultExtraOutputTypeDef = TypedDict(
+    "CustomDataIdentifiersResultExtraOutputTypeDef",
+    {
+        "Detections": NotRequired[List[CustomDataIdentifiersDetectionsExtraOutputTypeDef]],
+        "TotalCount": NotRequired[int],
+    },
+)
+SensitiveDataResultExtraOutputTypeDef = TypedDict(
+    "SensitiveDataResultExtraOutputTypeDef",
+    {
+        "Category": NotRequired[str],
+        "Detections": NotRequired[List[SensitiveDataDetectionsExtraOutputTypeDef]],
+        "TotalCount": NotRequired[int],
     },
 )
-CustomDataIdentifiersResultPaginatorTypeDef = TypedDict(
-    "CustomDataIdentifiersResultPaginatorTypeDef",
+CustomDataIdentifiersResultOutputTypeDef = TypedDict(
+    "CustomDataIdentifiersResultOutputTypeDef",
     {
-        "Detections": NotRequired[List[CustomDataIdentifiersDetectionsPaginatorTypeDef]],
+        "Detections": NotRequired[List[CustomDataIdentifiersDetectionsOutputTypeDef]],
         "TotalCount": NotRequired[int],
     },
 )
-SensitiveDataResultPaginatorTypeDef = TypedDict(
-    "SensitiveDataResultPaginatorTypeDef",
+SensitiveDataResultOutputTypeDef = TypedDict(
+    "SensitiveDataResultOutputTypeDef",
     {
         "Category": NotRequired[str],
-        "Detections": NotRequired[List[SensitiveDataDetectionsPaginatorTypeDef]],
+        "Detections": NotRequired[List[SensitiveDataDetectionsOutputTypeDef]],
         "TotalCount": NotRequired[int],
     },
 )
 CustomDataIdentifiersResultTypeDef = TypedDict(
     "CustomDataIdentifiersResultTypeDef",
     {
         "Detections": NotRequired[Sequence[CustomDataIdentifiersDetectionsTypeDef]],
@@ -11334,43 +14528,74 @@
     "SensitiveDataResultTypeDef",
     {
         "Category": NotRequired[str],
         "Detections": NotRequired[Sequence[SensitiveDataDetectionsTypeDef]],
         "TotalCount": NotRequired[int],
     },
 )
+SecurityHubPolicyOutputTypeDef = TypedDict(
+    "SecurityHubPolicyOutputTypeDef",
+    {
+        "ServiceEnabled": NotRequired[bool],
+        "EnabledStandardIdentifiers": NotRequired[List[str]],
+        "SecurityControlsConfiguration": NotRequired[SecurityControlsConfigurationOutputTypeDef],
+    },
+)
 SecurityHubPolicyTypeDef = TypedDict(
     "SecurityHubPolicyTypeDef",
     {
         "ServiceEnabled": NotRequired[bool],
         "EnabledStandardIdentifiers": NotRequired[Sequence[str]],
         "SecurityControlsConfiguration": NotRequired[SecurityControlsConfigurationTypeDef],
     },
 )
-FirewallPolicyDetailsPaginatorTypeDef = TypedDict(
-    "FirewallPolicyDetailsPaginatorTypeDef",
+FirewallPolicyDetailsExtraOutputTypeDef = TypedDict(
+    "FirewallPolicyDetailsExtraOutputTypeDef",
     {
         "StatefulRuleGroupReferences": NotRequired[
             List[FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef]
         ],
         "StatelessCustomActions": NotRequired[
-            List[FirewallPolicyStatelessCustomActionsDetailsPaginatorTypeDef]
+            List[FirewallPolicyStatelessCustomActionsDetailsExtraOutputTypeDef]
         ],
         "StatelessDefaultActions": NotRequired[List[str]],
         "StatelessFragmentDefaultActions": NotRequired[List[str]],
         "StatelessRuleGroupReferences": NotRequired[
             List[FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef]
         ],
     },
 )
-RuleGroupSourceStatelessRulesAndCustomActionsDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsPaginatorTypeDef",
+RuleGroupSourceStatelessRulesAndCustomActionsDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsExtraOutputTypeDef",
     {
-        "CustomActions": NotRequired[List[RuleGroupSourceCustomActionsDetailsPaginatorTypeDef]],
-        "StatelessRules": NotRequired[List[RuleGroupSourceStatelessRulesDetailsPaginatorTypeDef]],
+        "CustomActions": NotRequired[List[RuleGroupSourceCustomActionsDetailsExtraOutputTypeDef]],
+        "StatelessRules": NotRequired[List[RuleGroupSourceStatelessRulesDetailsExtraOutputTypeDef]],
+    },
+)
+FirewallPolicyDetailsOutputTypeDef = TypedDict(
+    "FirewallPolicyDetailsOutputTypeDef",
+    {
+        "StatefulRuleGroupReferences": NotRequired[
+            List[FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef]
+        ],
+        "StatelessCustomActions": NotRequired[
+            List[FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef]
+        ],
+        "StatelessDefaultActions": NotRequired[List[str]],
+        "StatelessFragmentDefaultActions": NotRequired[List[str]],
+        "StatelessRuleGroupReferences": NotRequired[
+            List[FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef]
+        ],
+    },
+)
+RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef",
+    {
+        "CustomActions": NotRequired[List[RuleGroupSourceCustomActionsDetailsOutputTypeDef]],
+        "StatelessRules": NotRequired[List[RuleGroupSourceStatelessRulesDetailsOutputTypeDef]],
     },
 )
 FirewallPolicyDetailsTypeDef = TypedDict(
     "FirewallPolicyDetailsTypeDef",
     {
         "StatefulRuleGroupReferences": NotRequired[
             Sequence[FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef]
@@ -11388,53 +14613,89 @@
 RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef",
     {
         "CustomActions": NotRequired[Sequence[RuleGroupSourceCustomActionsDetailsTypeDef]],
         "StatelessRules": NotRequired[Sequence[RuleGroupSourceStatelessRulesDetailsTypeDef]],
     },
 )
-AwsS3BucketBucketLifecycleConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationDetailsPaginatorTypeDef",
+AwsS3BucketBucketLifecycleConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationDetailsExtraOutputTypeDef",
     {
         "Rules": NotRequired[
-            List[AwsS3BucketBucketLifecycleConfigurationRulesDetailsPaginatorTypeDef]
+            List[AwsS3BucketBucketLifecycleConfigurationRulesDetailsExtraOutputTypeDef]
+        ],
+    },
+)
+AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef",
+    {
+        "Rules": NotRequired[
+            List[AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef]
         ],
     },
 )
 AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
     {
         "Rules": NotRequired[Sequence[AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef]],
     },
 )
-AwsWafv2RuleGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2RuleGroupDetailsPaginatorTypeDef",
+AwsWafv2RuleGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2RuleGroupDetailsExtraOutputTypeDef",
     {
         "Capacity": NotRequired[int],
         "Description": NotRequired[str],
         "Id": NotRequired[str],
         "Name": NotRequired[str],
         "Arn": NotRequired[str],
-        "Rules": NotRequired[List[AwsWafv2RulesDetailsPaginatorTypeDef]],
+        "Rules": NotRequired[List[AwsWafv2RulesDetailsExtraOutputTypeDef]],
         "Scope": NotRequired[str],
         "VisibilityConfig": NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],
     },
 )
-AwsWafv2WebAclDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2WebAclDetailsPaginatorTypeDef",
+AwsWafv2WebAclDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2WebAclDetailsExtraOutputTypeDef",
     {
         "Name": NotRequired[str],
         "Arn": NotRequired[str],
         "ManagedbyFirewallManager": NotRequired[bool],
         "Id": NotRequired[str],
         "Capacity": NotRequired[int],
         "CaptchaConfig": NotRequired[AwsWafv2WebAclCaptchaConfigDetailsTypeDef],
-        "DefaultAction": NotRequired[AwsWafv2WebAclActionDetailsPaginatorTypeDef],
+        "DefaultAction": NotRequired[AwsWafv2WebAclActionDetailsExtraOutputTypeDef],
         "Description": NotRequired[str],
-        "Rules": NotRequired[List[AwsWafv2RulesDetailsPaginatorTypeDef]],
+        "Rules": NotRequired[List[AwsWafv2RulesDetailsExtraOutputTypeDef]],
+        "VisibilityConfig": NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],
+    },
+)
+AwsWafv2RuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RuleGroupDetailsOutputTypeDef",
+    {
+        "Capacity": NotRequired[int],
+        "Description": NotRequired[str],
+        "Id": NotRequired[str],
+        "Name": NotRequired[str],
+        "Arn": NotRequired[str],
+        "Rules": NotRequired[List[AwsWafv2RulesDetailsOutputTypeDef]],
+        "Scope": NotRequired[str],
+        "VisibilityConfig": NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],
+    },
+)
+AwsWafv2WebAclDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2WebAclDetailsOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "Arn": NotRequired[str],
+        "ManagedbyFirewallManager": NotRequired[bool],
+        "Id": NotRequired[str],
+        "Capacity": NotRequired[int],
+        "CaptchaConfig": NotRequired[AwsWafv2WebAclCaptchaConfigDetailsTypeDef],
+        "DefaultAction": NotRequired[AwsWafv2WebAclActionDetailsOutputTypeDef],
+        "Description": NotRequired[str],
+        "Rules": NotRequired[List[AwsWafv2RulesDetailsOutputTypeDef]],
         "VisibilityConfig": NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],
     },
 )
 AwsWafv2RuleGroupDetailsTypeDef = TypedDict(
     "AwsWafv2RuleGroupDetailsTypeDef",
     {
         "Capacity": NotRequired[int],
@@ -11458,60 +14719,98 @@
         "CaptchaConfig": NotRequired[AwsWafv2WebAclCaptchaConfigDetailsTypeDef],
         "DefaultAction": NotRequired[AwsWafv2WebAclActionDetailsTypeDef],
         "Description": NotRequired[str],
         "Rules": NotRequired[Sequence[AwsWafv2RulesDetailsTypeDef]],
         "VisibilityConfig": NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],
     },
 )
-ClassificationResultPaginatorTypeDef = TypedDict(
-    "ClassificationResultPaginatorTypeDef",
+ClassificationResultExtraOutputTypeDef = TypedDict(
+    "ClassificationResultExtraOutputTypeDef",
+    {
+        "MimeType": NotRequired[str],
+        "SizeClassified": NotRequired[int],
+        "AdditionalOccurrences": NotRequired[bool],
+        "Status": NotRequired[ClassificationStatusTypeDef],
+        "SensitiveData": NotRequired[List[SensitiveDataResultExtraOutputTypeDef]],
+        "CustomDataIdentifiers": NotRequired[CustomDataIdentifiersResultExtraOutputTypeDef],
+    },
+)
+ClassificationResultOutputTypeDef = TypedDict(
+    "ClassificationResultOutputTypeDef",
     {
         "MimeType": NotRequired[str],
         "SizeClassified": NotRequired[int],
         "AdditionalOccurrences": NotRequired[bool],
         "Status": NotRequired[ClassificationStatusTypeDef],
-        "SensitiveData": NotRequired[List[SensitiveDataResultPaginatorTypeDef]],
-        "CustomDataIdentifiers": NotRequired[CustomDataIdentifiersResultPaginatorTypeDef],
+        "SensitiveData": NotRequired[List[SensitiveDataResultOutputTypeDef]],
+        "CustomDataIdentifiers": NotRequired[CustomDataIdentifiersResultOutputTypeDef],
     },
 )
 ClassificationResultTypeDef = TypedDict(
     "ClassificationResultTypeDef",
     {
         "MimeType": NotRequired[str],
         "SizeClassified": NotRequired[int],
         "AdditionalOccurrences": NotRequired[bool],
         "Status": NotRequired[ClassificationStatusTypeDef],
         "SensitiveData": NotRequired[Sequence[SensitiveDataResultTypeDef]],
         "CustomDataIdentifiers": NotRequired[CustomDataIdentifiersResultTypeDef],
     },
 )
+PolicyOutputTypeDef = TypedDict(
+    "PolicyOutputTypeDef",
+    {
+        "SecurityHub": NotRequired[SecurityHubPolicyOutputTypeDef],
+    },
+)
 PolicyTypeDef = TypedDict(
     "PolicyTypeDef",
     {
         "SecurityHub": NotRequired[SecurityHubPolicyTypeDef],
     },
 )
-AwsNetworkFirewallFirewallPolicyDetailsPaginatorTypeDef = TypedDict(
-    "AwsNetworkFirewallFirewallPolicyDetailsPaginatorTypeDef",
+AwsNetworkFirewallFirewallPolicyDetailsExtraOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallFirewallPolicyDetailsExtraOutputTypeDef",
     {
-        "FirewallPolicy": NotRequired[FirewallPolicyDetailsPaginatorTypeDef],
+        "FirewallPolicy": NotRequired[FirewallPolicyDetailsExtraOutputTypeDef],
         "FirewallPolicyArn": NotRequired[str],
         "FirewallPolicyId": NotRequired[str],
         "FirewallPolicyName": NotRequired[str],
         "Description": NotRequired[str],
     },
 )
-RuleGroupSourcePaginatorTypeDef = TypedDict(
-    "RuleGroupSourcePaginatorTypeDef",
+RuleGroupSourceExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceExtraOutputTypeDef",
     {
-        "RulesSourceList": NotRequired[RuleGroupSourceListDetailsPaginatorTypeDef],
+        "RulesSourceList": NotRequired[RuleGroupSourceListDetailsExtraOutputTypeDef],
         "RulesString": NotRequired[str],
-        "StatefulRules": NotRequired[List[RuleGroupSourceStatefulRulesDetailsPaginatorTypeDef]],
+        "StatefulRules": NotRequired[List[RuleGroupSourceStatefulRulesDetailsExtraOutputTypeDef]],
         "StatelessRulesAndCustomActions": NotRequired[
-            RuleGroupSourceStatelessRulesAndCustomActionsDetailsPaginatorTypeDef
+            RuleGroupSourceStatelessRulesAndCustomActionsDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef",
+    {
+        "FirewallPolicy": NotRequired[FirewallPolicyDetailsOutputTypeDef],
+        "FirewallPolicyArn": NotRequired[str],
+        "FirewallPolicyId": NotRequired[str],
+        "FirewallPolicyName": NotRequired[str],
+        "Description": NotRequired[str],
+    },
+)
+RuleGroupSourceOutputTypeDef = TypedDict(
+    "RuleGroupSourceOutputTypeDef",
+    {
+        "RulesSourceList": NotRequired[RuleGroupSourceListDetailsOutputTypeDef],
+        "RulesString": NotRequired[str],
+        "StatefulRules": NotRequired[List[RuleGroupSourceStatefulRulesDetailsOutputTypeDef]],
+        "StatelessRulesAndCustomActions": NotRequired[
+            RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef
         ],
     },
 )
 AwsNetworkFirewallFirewallPolicyDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallPolicyDetailsTypeDef",
     {
         "FirewallPolicy": NotRequired[FirewallPolicyDetailsTypeDef],
@@ -11528,33 +14827,62 @@
         "RulesString": NotRequired[str],
         "StatefulRules": NotRequired[Sequence[RuleGroupSourceStatefulRulesDetailsTypeDef]],
         "StatelessRulesAndCustomActions": NotRequired[
             RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef
         ],
     },
 )
-AwsS3BucketDetailsPaginatorTypeDef = TypedDict(
-    "AwsS3BucketDetailsPaginatorTypeDef",
+AwsS3BucketDetailsExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketDetailsExtraOutputTypeDef",
     {
         "OwnerId": NotRequired[str],
         "OwnerName": NotRequired[str],
         "OwnerAccountId": NotRequired[str],
         "CreatedAt": NotRequired[str],
         "ServerSideEncryptionConfiguration": NotRequired[
-            AwsS3BucketServerSideEncryptionConfigurationPaginatorTypeDef
+            AwsS3BucketServerSideEncryptionConfigurationExtraOutputTypeDef
         ],
         "BucketLifecycleConfiguration": NotRequired[
-            AwsS3BucketBucketLifecycleConfigurationDetailsPaginatorTypeDef
+            AwsS3BucketBucketLifecycleConfigurationDetailsExtraOutputTypeDef
         ],
         "PublicAccessBlockConfiguration": NotRequired[AwsS3AccountPublicAccessBlockDetailsTypeDef],
         "AccessControlList": NotRequired[str],
         "BucketLoggingConfiguration": NotRequired[AwsS3BucketLoggingConfigurationTypeDef],
-        "BucketWebsiteConfiguration": NotRequired[AwsS3BucketWebsiteConfigurationPaginatorTypeDef],
+        "BucketWebsiteConfiguration": NotRequired[
+            AwsS3BucketWebsiteConfigurationExtraOutputTypeDef
+        ],
         "BucketNotificationConfiguration": NotRequired[
-            AwsS3BucketNotificationConfigurationPaginatorTypeDef
+            AwsS3BucketNotificationConfigurationExtraOutputTypeDef
+        ],
+        "BucketVersioningConfiguration": NotRequired[
+            AwsS3BucketBucketVersioningConfigurationTypeDef
+        ],
+        "ObjectLockConfiguration": NotRequired[AwsS3BucketObjectLockConfigurationTypeDef],
+        "Name": NotRequired[str],
+    },
+)
+AwsS3BucketDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketDetailsOutputTypeDef",
+    {
+        "OwnerId": NotRequired[str],
+        "OwnerName": NotRequired[str],
+        "OwnerAccountId": NotRequired[str],
+        "CreatedAt": NotRequired[str],
+        "ServerSideEncryptionConfiguration": NotRequired[
+            AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef
+        ],
+        "BucketLifecycleConfiguration": NotRequired[
+            AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef
+        ],
+        "PublicAccessBlockConfiguration": NotRequired[AwsS3AccountPublicAccessBlockDetailsTypeDef],
+        "AccessControlList": NotRequired[str],
+        "BucketLoggingConfiguration": NotRequired[AwsS3BucketLoggingConfigurationTypeDef],
+        "BucketWebsiteConfiguration": NotRequired[AwsS3BucketWebsiteConfigurationOutputTypeDef],
+        "BucketNotificationConfiguration": NotRequired[
+            AwsS3BucketNotificationConfigurationOutputTypeDef
         ],
         "BucketVersioningConfiguration": NotRequired[
             AwsS3BucketBucketVersioningConfigurationTypeDef
         ],
         "ObjectLockConfiguration": NotRequired[AwsS3BucketObjectLockConfigurationTypeDef],
         "Name": NotRequired[str],
     },
@@ -11580,106 +14908,133 @@
         "BucketVersioningConfiguration": NotRequired[
             AwsS3BucketBucketVersioningConfigurationTypeDef
         ],
         "ObjectLockConfiguration": NotRequired[AwsS3BucketObjectLockConfigurationTypeDef],
         "Name": NotRequired[str],
     },
 )
-DataClassificationDetailsPaginatorTypeDef = TypedDict(
-    "DataClassificationDetailsPaginatorTypeDef",
+DataClassificationDetailsExtraOutputTypeDef = TypedDict(
+    "DataClassificationDetailsExtraOutputTypeDef",
     {
         "DetailedResultsLocation": NotRequired[str],
-        "Result": NotRequired[ClassificationResultPaginatorTypeDef],
+        "Result": NotRequired[ClassificationResultExtraOutputTypeDef],
     },
 )
-DataClassificationDetailsTypeDef = TypedDict(
-    "DataClassificationDetailsTypeDef",
+DataClassificationDetailsOutputTypeDef = TypedDict(
+    "DataClassificationDetailsOutputTypeDef",
     {
         "DetailedResultsLocation": NotRequired[str],
-        "Result": NotRequired[ClassificationResultTypeDef],
+        "Result": NotRequired[ClassificationResultOutputTypeDef],
     },
 )
-CreateConfigurationPolicyRequestRequestTypeDef = TypedDict(
-    "CreateConfigurationPolicyRequestRequestTypeDef",
+DataClassificationDetailsTypeDef = TypedDict(
+    "DataClassificationDetailsTypeDef",
     {
-        "Name": str,
-        "ConfigurationPolicy": PolicyTypeDef,
-        "Description": NotRequired[str],
-        "Tags": NotRequired[Mapping[str, str]],
+        "DetailedResultsLocation": NotRequired[str],
+        "Result": NotRequired[ClassificationResultTypeDef],
     },
 )
 CreateConfigurationPolicyResponseTypeDef = TypedDict(
     "CreateConfigurationPolicyResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "UpdatedAt": datetime,
         "CreatedAt": datetime,
-        "ConfigurationPolicy": PolicyTypeDef,
+        "ConfigurationPolicy": PolicyOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetConfigurationPolicyResponseTypeDef = TypedDict(
     "GetConfigurationPolicyResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "UpdatedAt": datetime,
         "CreatedAt": datetime,
-        "ConfigurationPolicy": PolicyTypeDef,
+        "ConfigurationPolicy": PolicyOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateConfigurationPolicyResponseTypeDef = TypedDict(
+    "UpdateConfigurationPolicyResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "UpdatedAt": datetime,
+        "CreatedAt": datetime,
+        "ConfigurationPolicy": PolicyOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateConfigurationPolicyRequestRequestTypeDef = TypedDict(
+    "CreateConfigurationPolicyRequestRequestTypeDef",
+    {
+        "Name": str,
+        "ConfigurationPolicy": PolicyTypeDef,
+        "Description": NotRequired[str],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+PolicyUnionTypeDef = Union[PolicyTypeDef, PolicyOutputTypeDef]
 UpdateConfigurationPolicyRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationPolicyRequestRequestTypeDef",
     {
         "Identifier": str,
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "UpdatedReason": NotRequired[str],
         "ConfigurationPolicy": NotRequired[PolicyTypeDef],
     },
 )
-UpdateConfigurationPolicyResponseTypeDef = TypedDict(
-    "UpdateConfigurationPolicyResponseTypeDef",
+RuleGroupDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupDetailsExtraOutputTypeDef",
     {
-        "Arn": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "UpdatedAt": datetime,
-        "CreatedAt": datetime,
-        "ConfigurationPolicy": PolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RuleVariables": NotRequired[RuleGroupVariablesExtraOutputTypeDef],
+        "RulesSource": NotRequired[RuleGroupSourceExtraOutputTypeDef],
     },
 )
-RuleGroupDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupDetailsPaginatorTypeDef",
+RuleGroupDetailsOutputTypeDef = TypedDict(
+    "RuleGroupDetailsOutputTypeDef",
     {
-        "RuleVariables": NotRequired[RuleGroupVariablesPaginatorTypeDef],
-        "RulesSource": NotRequired[RuleGroupSourcePaginatorTypeDef],
+        "RuleVariables": NotRequired[RuleGroupVariablesOutputTypeDef],
+        "RulesSource": NotRequired[RuleGroupSourceOutputTypeDef],
     },
 )
 RuleGroupDetailsTypeDef = TypedDict(
     "RuleGroupDetailsTypeDef",
     {
         "RuleVariables": NotRequired[RuleGroupVariablesTypeDef],
         "RulesSource": NotRequired[RuleGroupSourceTypeDef],
     },
 )
-AwsNetworkFirewallRuleGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsNetworkFirewallRuleGroupDetailsPaginatorTypeDef",
+AwsNetworkFirewallRuleGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallRuleGroupDetailsExtraOutputTypeDef",
     {
         "Capacity": NotRequired[int],
         "Description": NotRequired[str],
-        "RuleGroup": NotRequired[RuleGroupDetailsPaginatorTypeDef],
+        "RuleGroup": NotRequired[RuleGroupDetailsExtraOutputTypeDef],
+        "RuleGroupArn": NotRequired[str],
+        "RuleGroupId": NotRequired[str],
+        "RuleGroupName": NotRequired[str],
+        "Type": NotRequired[str],
+    },
+)
+AwsNetworkFirewallRuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallRuleGroupDetailsOutputTypeDef",
+    {
+        "Capacity": NotRequired[int],
+        "Description": NotRequired[str],
+        "RuleGroup": NotRequired[RuleGroupDetailsOutputTypeDef],
         "RuleGroupArn": NotRequired[str],
         "RuleGroupId": NotRequired[str],
         "RuleGroupName": NotRequired[str],
         "Type": NotRequired[str],
     },
 )
 AwsNetworkFirewallRuleGroupDetailsTypeDef = TypedDict(
@@ -11690,140 +15045,260 @@
         "RuleGroup": NotRequired[RuleGroupDetailsTypeDef],
         "RuleGroupArn": NotRequired[str],
         "RuleGroupId": NotRequired[str],
         "RuleGroupName": NotRequired[str],
         "Type": NotRequired[str],
     },
 )
-ResourceDetailsPaginatorTypeDef = TypedDict(
-    "ResourceDetailsPaginatorTypeDef",
+ResourceDetailsExtraOutputTypeDef = TypedDict(
+    "ResourceDetailsExtraOutputTypeDef",
     {
         "AwsAutoScalingAutoScalingGroup": NotRequired[
-            AwsAutoScalingAutoScalingGroupDetailsPaginatorTypeDef
+            AwsAutoScalingAutoScalingGroupDetailsExtraOutputTypeDef
         ],
-        "AwsCodeBuildProject": NotRequired[AwsCodeBuildProjectDetailsPaginatorTypeDef],
-        "AwsCloudFrontDistribution": NotRequired[AwsCloudFrontDistributionDetailsPaginatorTypeDef],
-        "AwsEc2Instance": NotRequired[AwsEc2InstanceDetailsPaginatorTypeDef],
-        "AwsEc2NetworkInterface": NotRequired[AwsEc2NetworkInterfaceDetailsPaginatorTypeDef],
-        "AwsEc2SecurityGroup": NotRequired[AwsEc2SecurityGroupDetailsPaginatorTypeDef],
-        "AwsEc2Volume": NotRequired[AwsEc2VolumeDetailsPaginatorTypeDef],
-        "AwsEc2Vpc": NotRequired[AwsEc2VpcDetailsPaginatorTypeDef],
+        "AwsCodeBuildProject": NotRequired[AwsCodeBuildProjectDetailsExtraOutputTypeDef],
+        "AwsCloudFrontDistribution": NotRequired[
+            AwsCloudFrontDistributionDetailsExtraOutputTypeDef
+        ],
+        "AwsEc2Instance": NotRequired[AwsEc2InstanceDetailsExtraOutputTypeDef],
+        "AwsEc2NetworkInterface": NotRequired[AwsEc2NetworkInterfaceDetailsExtraOutputTypeDef],
+        "AwsEc2SecurityGroup": NotRequired[AwsEc2SecurityGroupDetailsExtraOutputTypeDef],
+        "AwsEc2Volume": NotRequired[AwsEc2VolumeDetailsExtraOutputTypeDef],
+        "AwsEc2Vpc": NotRequired[AwsEc2VpcDetailsExtraOutputTypeDef],
         "AwsEc2Eip": NotRequired[AwsEc2EipDetailsTypeDef],
-        "AwsEc2Subnet": NotRequired[AwsEc2SubnetDetailsPaginatorTypeDef],
-        "AwsEc2NetworkAcl": NotRequired[AwsEc2NetworkAclDetailsPaginatorTypeDef],
-        "AwsElbv2LoadBalancer": NotRequired[AwsElbv2LoadBalancerDetailsPaginatorTypeDef],
+        "AwsEc2Subnet": NotRequired[AwsEc2SubnetDetailsExtraOutputTypeDef],
+        "AwsEc2NetworkAcl": NotRequired[AwsEc2NetworkAclDetailsExtraOutputTypeDef],
+        "AwsElbv2LoadBalancer": NotRequired[AwsElbv2LoadBalancerDetailsExtraOutputTypeDef],
         "AwsElasticBeanstalkEnvironment": NotRequired[
-            AwsElasticBeanstalkEnvironmentDetailsPaginatorTypeDef
+            AwsElasticBeanstalkEnvironmentDetailsExtraOutputTypeDef
         ],
-        "AwsElasticsearchDomain": NotRequired[AwsElasticsearchDomainDetailsPaginatorTypeDef],
-        "AwsS3Bucket": NotRequired[AwsS3BucketDetailsPaginatorTypeDef],
+        "AwsElasticsearchDomain": NotRequired[AwsElasticsearchDomainDetailsExtraOutputTypeDef],
+        "AwsS3Bucket": NotRequired[AwsS3BucketDetailsExtraOutputTypeDef],
         "AwsS3AccountPublicAccessBlock": NotRequired[AwsS3AccountPublicAccessBlockDetailsTypeDef],
         "AwsS3Object": NotRequired[AwsS3ObjectDetailsTypeDef],
         "AwsSecretsManagerSecret": NotRequired[AwsSecretsManagerSecretDetailsTypeDef],
         "AwsIamAccessKey": NotRequired[AwsIamAccessKeyDetailsTypeDef],
-        "AwsIamUser": NotRequired[AwsIamUserDetailsPaginatorTypeDef],
-        "AwsIamPolicy": NotRequired[AwsIamPolicyDetailsPaginatorTypeDef],
-        "AwsApiGatewayV2Stage": NotRequired[AwsApiGatewayV2StageDetailsPaginatorTypeDef],
-        "AwsApiGatewayV2Api": NotRequired[AwsApiGatewayV2ApiDetailsPaginatorTypeDef],
-        "AwsDynamoDbTable": NotRequired[AwsDynamoDbTableDetailsPaginatorTypeDef],
-        "AwsApiGatewayStage": NotRequired[AwsApiGatewayStageDetailsPaginatorTypeDef],
-        "AwsApiGatewayRestApi": NotRequired[AwsApiGatewayRestApiDetailsPaginatorTypeDef],
+        "AwsIamUser": NotRequired[AwsIamUserDetailsExtraOutputTypeDef],
+        "AwsIamPolicy": NotRequired[AwsIamPolicyDetailsExtraOutputTypeDef],
+        "AwsApiGatewayV2Stage": NotRequired[AwsApiGatewayV2StageDetailsExtraOutputTypeDef],
+        "AwsApiGatewayV2Api": NotRequired[AwsApiGatewayV2ApiDetailsExtraOutputTypeDef],
+        "AwsDynamoDbTable": NotRequired[AwsDynamoDbTableDetailsExtraOutputTypeDef],
+        "AwsApiGatewayStage": NotRequired[AwsApiGatewayStageDetailsExtraOutputTypeDef],
+        "AwsApiGatewayRestApi": NotRequired[AwsApiGatewayRestApiDetailsExtraOutputTypeDef],
         "AwsCloudTrailTrail": NotRequired[AwsCloudTrailTrailDetailsTypeDef],
         "AwsSsmPatchCompliance": NotRequired[AwsSsmPatchComplianceDetailsTypeDef],
         "AwsCertificateManagerCertificate": NotRequired[
-            AwsCertificateManagerCertificateDetailsPaginatorTypeDef
+            AwsCertificateManagerCertificateDetailsExtraOutputTypeDef
         ],
-        "AwsRedshiftCluster": NotRequired[AwsRedshiftClusterDetailsPaginatorTypeDef],
-        "AwsElbLoadBalancer": NotRequired[AwsElbLoadBalancerDetailsPaginatorTypeDef],
-        "AwsIamGroup": NotRequired[AwsIamGroupDetailsPaginatorTypeDef],
-        "AwsIamRole": NotRequired[AwsIamRoleDetailsPaginatorTypeDef],
+        "AwsRedshiftCluster": NotRequired[AwsRedshiftClusterDetailsExtraOutputTypeDef],
+        "AwsElbLoadBalancer": NotRequired[AwsElbLoadBalancerDetailsExtraOutputTypeDef],
+        "AwsIamGroup": NotRequired[AwsIamGroupDetailsExtraOutputTypeDef],
+        "AwsIamRole": NotRequired[AwsIamRoleDetailsExtraOutputTypeDef],
         "AwsKmsKey": NotRequired[AwsKmsKeyDetailsTypeDef],
-        "AwsLambdaFunction": NotRequired[AwsLambdaFunctionDetailsPaginatorTypeDef],
-        "AwsLambdaLayerVersion": NotRequired[AwsLambdaLayerVersionDetailsPaginatorTypeDef],
-        "AwsRdsDbInstance": NotRequired[AwsRdsDbInstanceDetailsPaginatorTypeDef],
-        "AwsSnsTopic": NotRequired[AwsSnsTopicDetailsPaginatorTypeDef],
+        "AwsLambdaFunction": NotRequired[AwsLambdaFunctionDetailsExtraOutputTypeDef],
+        "AwsLambdaLayerVersion": NotRequired[AwsLambdaLayerVersionDetailsExtraOutputTypeDef],
+        "AwsRdsDbInstance": NotRequired[AwsRdsDbInstanceDetailsExtraOutputTypeDef],
+        "AwsSnsTopic": NotRequired[AwsSnsTopicDetailsExtraOutputTypeDef],
         "AwsSqsQueue": NotRequired[AwsSqsQueueDetailsTypeDef],
-        "AwsWafWebAcl": NotRequired[AwsWafWebAclDetailsPaginatorTypeDef],
-        "AwsRdsDbSnapshot": NotRequired[AwsRdsDbSnapshotDetailsPaginatorTypeDef],
-        "AwsRdsDbClusterSnapshot": NotRequired[AwsRdsDbClusterSnapshotDetailsPaginatorTypeDef],
-        "AwsRdsDbCluster": NotRequired[AwsRdsDbClusterDetailsPaginatorTypeDef],
-        "AwsEcsCluster": NotRequired[AwsEcsClusterDetailsPaginatorTypeDef],
-        "AwsEcsContainer": NotRequired[AwsEcsContainerDetailsPaginatorTypeDef],
-        "AwsEcsTaskDefinition": NotRequired[AwsEcsTaskDefinitionDetailsPaginatorTypeDef],
-        "Container": NotRequired[ContainerDetailsPaginatorTypeDef],
+        "AwsWafWebAcl": NotRequired[AwsWafWebAclDetailsExtraOutputTypeDef],
+        "AwsRdsDbSnapshot": NotRequired[AwsRdsDbSnapshotDetailsExtraOutputTypeDef],
+        "AwsRdsDbClusterSnapshot": NotRequired[AwsRdsDbClusterSnapshotDetailsExtraOutputTypeDef],
+        "AwsRdsDbCluster": NotRequired[AwsRdsDbClusterDetailsExtraOutputTypeDef],
+        "AwsEcsCluster": NotRequired[AwsEcsClusterDetailsExtraOutputTypeDef],
+        "AwsEcsContainer": NotRequired[AwsEcsContainerDetailsExtraOutputTypeDef],
+        "AwsEcsTaskDefinition": NotRequired[AwsEcsTaskDefinitionDetailsExtraOutputTypeDef],
+        "Container": NotRequired[ContainerDetailsExtraOutputTypeDef],
         "Other": NotRequired[Dict[str, str]],
-        "AwsRdsEventSubscription": NotRequired[AwsRdsEventSubscriptionDetailsPaginatorTypeDef],
-        "AwsEcsService": NotRequired[AwsEcsServiceDetailsPaginatorTypeDef],
+        "AwsRdsEventSubscription": NotRequired[AwsRdsEventSubscriptionDetailsExtraOutputTypeDef],
+        "AwsEcsService": NotRequired[AwsEcsServiceDetailsExtraOutputTypeDef],
         "AwsAutoScalingLaunchConfiguration": NotRequired[
-            AwsAutoScalingLaunchConfigurationDetailsPaginatorTypeDef
+            AwsAutoScalingLaunchConfigurationDetailsExtraOutputTypeDef
         ],
-        "AwsEc2VpnConnection": NotRequired[AwsEc2VpnConnectionDetailsPaginatorTypeDef],
-        "AwsEcrContainerImage": NotRequired[AwsEcrContainerImageDetailsPaginatorTypeDef],
+        "AwsEc2VpnConnection": NotRequired[AwsEc2VpnConnectionDetailsExtraOutputTypeDef],
+        "AwsEcrContainerImage": NotRequired[AwsEcrContainerImageDetailsExtraOutputTypeDef],
         "AwsOpenSearchServiceDomain": NotRequired[
-            AwsOpenSearchServiceDomainDetailsPaginatorTypeDef
+            AwsOpenSearchServiceDomainDetailsExtraOutputTypeDef
         ],
-        "AwsEc2VpcEndpointService": NotRequired[AwsEc2VpcEndpointServiceDetailsPaginatorTypeDef],
+        "AwsEc2VpcEndpointService": NotRequired[AwsEc2VpcEndpointServiceDetailsExtraOutputTypeDef],
         "AwsXrayEncryptionConfig": NotRequired[AwsXrayEncryptionConfigDetailsTypeDef],
-        "AwsWafRateBasedRule": NotRequired[AwsWafRateBasedRuleDetailsPaginatorTypeDef],
+        "AwsWafRateBasedRule": NotRequired[AwsWafRateBasedRuleDetailsExtraOutputTypeDef],
         "AwsWafRegionalRateBasedRule": NotRequired[
-            AwsWafRegionalRateBasedRuleDetailsPaginatorTypeDef
+            AwsWafRegionalRateBasedRuleDetailsExtraOutputTypeDef
         ],
         "AwsEcrRepository": NotRequired[AwsEcrRepositoryDetailsTypeDef],
-        "AwsEksCluster": NotRequired[AwsEksClusterDetailsPaginatorTypeDef],
+        "AwsEksCluster": NotRequired[AwsEksClusterDetailsExtraOutputTypeDef],
         "AwsNetworkFirewallFirewallPolicy": NotRequired[
-            AwsNetworkFirewallFirewallPolicyDetailsPaginatorTypeDef
+            AwsNetworkFirewallFirewallPolicyDetailsExtraOutputTypeDef
         ],
         "AwsNetworkFirewallFirewall": NotRequired[
-            AwsNetworkFirewallFirewallDetailsPaginatorTypeDef
+            AwsNetworkFirewallFirewallDetailsExtraOutputTypeDef
         ],
         "AwsNetworkFirewallRuleGroup": NotRequired[
-            AwsNetworkFirewallRuleGroupDetailsPaginatorTypeDef
+            AwsNetworkFirewallRuleGroupDetailsExtraOutputTypeDef
         ],
-        "AwsRdsDbSecurityGroup": NotRequired[AwsRdsDbSecurityGroupDetailsPaginatorTypeDef],
+        "AwsRdsDbSecurityGroup": NotRequired[AwsRdsDbSecurityGroupDetailsExtraOutputTypeDef],
         "AwsKinesisStream": NotRequired[AwsKinesisStreamDetailsTypeDef],
-        "AwsEc2TransitGateway": NotRequired[AwsEc2TransitGatewayDetailsPaginatorTypeDef],
-        "AwsEfsAccessPoint": NotRequired[AwsEfsAccessPointDetailsPaginatorTypeDef],
-        "AwsCloudFormationStack": NotRequired[AwsCloudFormationStackDetailsPaginatorTypeDef],
-        "AwsCloudWatchAlarm": NotRequired[AwsCloudWatchAlarmDetailsPaginatorTypeDef],
+        "AwsEc2TransitGateway": NotRequired[AwsEc2TransitGatewayDetailsExtraOutputTypeDef],
+        "AwsEfsAccessPoint": NotRequired[AwsEfsAccessPointDetailsExtraOutputTypeDef],
+        "AwsCloudFormationStack": NotRequired[AwsCloudFormationStackDetailsExtraOutputTypeDef],
+        "AwsCloudWatchAlarm": NotRequired[AwsCloudWatchAlarmDetailsExtraOutputTypeDef],
         "AwsEc2VpcPeeringConnection": NotRequired[
-            AwsEc2VpcPeeringConnectionDetailsPaginatorTypeDef
+            AwsEc2VpcPeeringConnectionDetailsExtraOutputTypeDef
         ],
-        "AwsWafRegionalRuleGroup": NotRequired[AwsWafRegionalRuleGroupDetailsPaginatorTypeDef],
-        "AwsWafRegionalRule": NotRequired[AwsWafRegionalRuleDetailsPaginatorTypeDef],
-        "AwsWafRegionalWebAcl": NotRequired[AwsWafRegionalWebAclDetailsPaginatorTypeDef],
-        "AwsWafRule": NotRequired[AwsWafRuleDetailsPaginatorTypeDef],
-        "AwsWafRuleGroup": NotRequired[AwsWafRuleGroupDetailsPaginatorTypeDef],
-        "AwsEcsTask": NotRequired[AwsEcsTaskDetailsPaginatorTypeDef],
-        "AwsBackupBackupVault": NotRequired[AwsBackupBackupVaultDetailsPaginatorTypeDef],
-        "AwsBackupBackupPlan": NotRequired[AwsBackupBackupPlanDetailsPaginatorTypeDef],
+        "AwsWafRegionalRuleGroup": NotRequired[AwsWafRegionalRuleGroupDetailsExtraOutputTypeDef],
+        "AwsWafRegionalRule": NotRequired[AwsWafRegionalRuleDetailsExtraOutputTypeDef],
+        "AwsWafRegionalWebAcl": NotRequired[AwsWafRegionalWebAclDetailsExtraOutputTypeDef],
+        "AwsWafRule": NotRequired[AwsWafRuleDetailsExtraOutputTypeDef],
+        "AwsWafRuleGroup": NotRequired[AwsWafRuleGroupDetailsExtraOutputTypeDef],
+        "AwsEcsTask": NotRequired[AwsEcsTaskDetailsExtraOutputTypeDef],
+        "AwsBackupBackupVault": NotRequired[AwsBackupBackupVaultDetailsExtraOutputTypeDef],
+        "AwsBackupBackupPlan": NotRequired[AwsBackupBackupPlanDetailsExtraOutputTypeDef],
         "AwsBackupRecoveryPoint": NotRequired[AwsBackupRecoveryPointDetailsTypeDef],
-        "AwsEc2LaunchTemplate": NotRequired[AwsEc2LaunchTemplateDetailsPaginatorTypeDef],
+        "AwsEc2LaunchTemplate": NotRequired[AwsEc2LaunchTemplateDetailsExtraOutputTypeDef],
         "AwsSageMakerNotebookInstance": NotRequired[
-            AwsSageMakerNotebookInstanceDetailsPaginatorTypeDef
+            AwsSageMakerNotebookInstanceDetailsExtraOutputTypeDef
         ],
-        "AwsWafv2WebAcl": NotRequired[AwsWafv2WebAclDetailsPaginatorTypeDef],
-        "AwsWafv2RuleGroup": NotRequired[AwsWafv2RuleGroupDetailsPaginatorTypeDef],
-        "AwsEc2RouteTable": NotRequired[AwsEc2RouteTableDetailsPaginatorTypeDef],
-        "AwsAmazonMqBroker": NotRequired[AwsAmazonMqBrokerDetailsPaginatorTypeDef],
-        "AwsAppSyncGraphQlApi": NotRequired[AwsAppSyncGraphQlApiDetailsPaginatorTypeDef],
+        "AwsWafv2WebAcl": NotRequired[AwsWafv2WebAclDetailsExtraOutputTypeDef],
+        "AwsWafv2RuleGroup": NotRequired[AwsWafv2RuleGroupDetailsExtraOutputTypeDef],
+        "AwsEc2RouteTable": NotRequired[AwsEc2RouteTableDetailsExtraOutputTypeDef],
+        "AwsAmazonMqBroker": NotRequired[AwsAmazonMqBrokerDetailsExtraOutputTypeDef],
+        "AwsAppSyncGraphQlApi": NotRequired[AwsAppSyncGraphQlApiDetailsExtraOutputTypeDef],
         "AwsEventSchemasRegistry": NotRequired[AwsEventSchemasRegistryDetailsTypeDef],
-        "AwsGuardDutyDetector": NotRequired[AwsGuardDutyDetectorDetailsPaginatorTypeDef],
+        "AwsGuardDutyDetector": NotRequired[AwsGuardDutyDetectorDetailsExtraOutputTypeDef],
         "AwsStepFunctionStateMachine": NotRequired[
-            AwsStepFunctionStateMachineDetailsPaginatorTypeDef
+            AwsStepFunctionStateMachineDetailsExtraOutputTypeDef
         ],
         "AwsAthenaWorkGroup": NotRequired[AwsAthenaWorkGroupDetailsTypeDef],
         "AwsEventsEventbus": NotRequired[AwsEventsEventbusDetailsTypeDef],
         "AwsDmsEndpoint": NotRequired[AwsDmsEndpointDetailsTypeDef],
-        "AwsEventsEndpoint": NotRequired[AwsEventsEndpointDetailsPaginatorTypeDef],
+        "AwsEventsEndpoint": NotRequired[AwsEventsEndpointDetailsExtraOutputTypeDef],
         "AwsDmsReplicationTask": NotRequired[AwsDmsReplicationTaskDetailsTypeDef],
-        "AwsDmsReplicationInstance": NotRequired[AwsDmsReplicationInstanceDetailsPaginatorTypeDef],
-        "AwsRoute53HostedZone": NotRequired[AwsRoute53HostedZoneDetailsPaginatorTypeDef],
-        "AwsMskCluster": NotRequired[AwsMskClusterDetailsPaginatorTypeDef],
+        "AwsDmsReplicationInstance": NotRequired[
+            AwsDmsReplicationInstanceDetailsExtraOutputTypeDef
+        ],
+        "AwsRoute53HostedZone": NotRequired[AwsRoute53HostedZoneDetailsExtraOutputTypeDef],
+        "AwsMskCluster": NotRequired[AwsMskClusterDetailsExtraOutputTypeDef],
         "AwsS3AccessPoint": NotRequired[AwsS3AccessPointDetailsTypeDef],
-        "AwsEc2ClientVpnEndpoint": NotRequired[AwsEc2ClientVpnEndpointDetailsPaginatorTypeDef],
+        "AwsEc2ClientVpnEndpoint": NotRequired[AwsEc2ClientVpnEndpointDetailsExtraOutputTypeDef],
+    },
+)
+ResourceDetailsOutputTypeDef = TypedDict(
+    "ResourceDetailsOutputTypeDef",
+    {
+        "AwsAutoScalingAutoScalingGroup": NotRequired[
+            AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef
+        ],
+        "AwsCodeBuildProject": NotRequired[AwsCodeBuildProjectDetailsOutputTypeDef],
+        "AwsCloudFrontDistribution": NotRequired[AwsCloudFrontDistributionDetailsOutputTypeDef],
+        "AwsEc2Instance": NotRequired[AwsEc2InstanceDetailsOutputTypeDef],
+        "AwsEc2NetworkInterface": NotRequired[AwsEc2NetworkInterfaceDetailsOutputTypeDef],
+        "AwsEc2SecurityGroup": NotRequired[AwsEc2SecurityGroupDetailsOutputTypeDef],
+        "AwsEc2Volume": NotRequired[AwsEc2VolumeDetailsOutputTypeDef],
+        "AwsEc2Vpc": NotRequired[AwsEc2VpcDetailsOutputTypeDef],
+        "AwsEc2Eip": NotRequired[AwsEc2EipDetailsTypeDef],
+        "AwsEc2Subnet": NotRequired[AwsEc2SubnetDetailsOutputTypeDef],
+        "AwsEc2NetworkAcl": NotRequired[AwsEc2NetworkAclDetailsOutputTypeDef],
+        "AwsElbv2LoadBalancer": NotRequired[AwsElbv2LoadBalancerDetailsOutputTypeDef],
+        "AwsElasticBeanstalkEnvironment": NotRequired[
+            AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef
+        ],
+        "AwsElasticsearchDomain": NotRequired[AwsElasticsearchDomainDetailsOutputTypeDef],
+        "AwsS3Bucket": NotRequired[AwsS3BucketDetailsOutputTypeDef],
+        "AwsS3AccountPublicAccessBlock": NotRequired[AwsS3AccountPublicAccessBlockDetailsTypeDef],
+        "AwsS3Object": NotRequired[AwsS3ObjectDetailsTypeDef],
+        "AwsSecretsManagerSecret": NotRequired[AwsSecretsManagerSecretDetailsTypeDef],
+        "AwsIamAccessKey": NotRequired[AwsIamAccessKeyDetailsTypeDef],
+        "AwsIamUser": NotRequired[AwsIamUserDetailsOutputTypeDef],
+        "AwsIamPolicy": NotRequired[AwsIamPolicyDetailsOutputTypeDef],
+        "AwsApiGatewayV2Stage": NotRequired[AwsApiGatewayV2StageDetailsOutputTypeDef],
+        "AwsApiGatewayV2Api": NotRequired[AwsApiGatewayV2ApiDetailsOutputTypeDef],
+        "AwsDynamoDbTable": NotRequired[AwsDynamoDbTableDetailsOutputTypeDef],
+        "AwsApiGatewayStage": NotRequired[AwsApiGatewayStageDetailsOutputTypeDef],
+        "AwsApiGatewayRestApi": NotRequired[AwsApiGatewayRestApiDetailsOutputTypeDef],
+        "AwsCloudTrailTrail": NotRequired[AwsCloudTrailTrailDetailsTypeDef],
+        "AwsSsmPatchCompliance": NotRequired[AwsSsmPatchComplianceDetailsTypeDef],
+        "AwsCertificateManagerCertificate": NotRequired[
+            AwsCertificateManagerCertificateDetailsOutputTypeDef
+        ],
+        "AwsRedshiftCluster": NotRequired[AwsRedshiftClusterDetailsOutputTypeDef],
+        "AwsElbLoadBalancer": NotRequired[AwsElbLoadBalancerDetailsOutputTypeDef],
+        "AwsIamGroup": NotRequired[AwsIamGroupDetailsOutputTypeDef],
+        "AwsIamRole": NotRequired[AwsIamRoleDetailsOutputTypeDef],
+        "AwsKmsKey": NotRequired[AwsKmsKeyDetailsTypeDef],
+        "AwsLambdaFunction": NotRequired[AwsLambdaFunctionDetailsOutputTypeDef],
+        "AwsLambdaLayerVersion": NotRequired[AwsLambdaLayerVersionDetailsOutputTypeDef],
+        "AwsRdsDbInstance": NotRequired[AwsRdsDbInstanceDetailsOutputTypeDef],
+        "AwsSnsTopic": NotRequired[AwsSnsTopicDetailsOutputTypeDef],
+        "AwsSqsQueue": NotRequired[AwsSqsQueueDetailsTypeDef],
+        "AwsWafWebAcl": NotRequired[AwsWafWebAclDetailsOutputTypeDef],
+        "AwsRdsDbSnapshot": NotRequired[AwsRdsDbSnapshotDetailsOutputTypeDef],
+        "AwsRdsDbClusterSnapshot": NotRequired[AwsRdsDbClusterSnapshotDetailsOutputTypeDef],
+        "AwsRdsDbCluster": NotRequired[AwsRdsDbClusterDetailsOutputTypeDef],
+        "AwsEcsCluster": NotRequired[AwsEcsClusterDetailsOutputTypeDef],
+        "AwsEcsContainer": NotRequired[AwsEcsContainerDetailsOutputTypeDef],
+        "AwsEcsTaskDefinition": NotRequired[AwsEcsTaskDefinitionDetailsOutputTypeDef],
+        "Container": NotRequired[ContainerDetailsOutputTypeDef],
+        "Other": NotRequired[Dict[str, str]],
+        "AwsRdsEventSubscription": NotRequired[AwsRdsEventSubscriptionDetailsOutputTypeDef],
+        "AwsEcsService": NotRequired[AwsEcsServiceDetailsOutputTypeDef],
+        "AwsAutoScalingLaunchConfiguration": NotRequired[
+            AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef
+        ],
+        "AwsEc2VpnConnection": NotRequired[AwsEc2VpnConnectionDetailsOutputTypeDef],
+        "AwsEcrContainerImage": NotRequired[AwsEcrContainerImageDetailsOutputTypeDef],
+        "AwsOpenSearchServiceDomain": NotRequired[AwsOpenSearchServiceDomainDetailsOutputTypeDef],
+        "AwsEc2VpcEndpointService": NotRequired[AwsEc2VpcEndpointServiceDetailsOutputTypeDef],
+        "AwsXrayEncryptionConfig": NotRequired[AwsXrayEncryptionConfigDetailsTypeDef],
+        "AwsWafRateBasedRule": NotRequired[AwsWafRateBasedRuleDetailsOutputTypeDef],
+        "AwsWafRegionalRateBasedRule": NotRequired[AwsWafRegionalRateBasedRuleDetailsOutputTypeDef],
+        "AwsEcrRepository": NotRequired[AwsEcrRepositoryDetailsTypeDef],
+        "AwsEksCluster": NotRequired[AwsEksClusterDetailsOutputTypeDef],
+        "AwsNetworkFirewallFirewallPolicy": NotRequired[
+            AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef
+        ],
+        "AwsNetworkFirewallFirewall": NotRequired[AwsNetworkFirewallFirewallDetailsOutputTypeDef],
+        "AwsNetworkFirewallRuleGroup": NotRequired[AwsNetworkFirewallRuleGroupDetailsOutputTypeDef],
+        "AwsRdsDbSecurityGroup": NotRequired[AwsRdsDbSecurityGroupDetailsOutputTypeDef],
+        "AwsKinesisStream": NotRequired[AwsKinesisStreamDetailsTypeDef],
+        "AwsEc2TransitGateway": NotRequired[AwsEc2TransitGatewayDetailsOutputTypeDef],
+        "AwsEfsAccessPoint": NotRequired[AwsEfsAccessPointDetailsOutputTypeDef],
+        "AwsCloudFormationStack": NotRequired[AwsCloudFormationStackDetailsOutputTypeDef],
+        "AwsCloudWatchAlarm": NotRequired[AwsCloudWatchAlarmDetailsOutputTypeDef],
+        "AwsEc2VpcPeeringConnection": NotRequired[AwsEc2VpcPeeringConnectionDetailsOutputTypeDef],
+        "AwsWafRegionalRuleGroup": NotRequired[AwsWafRegionalRuleGroupDetailsOutputTypeDef],
+        "AwsWafRegionalRule": NotRequired[AwsWafRegionalRuleDetailsOutputTypeDef],
+        "AwsWafRegionalWebAcl": NotRequired[AwsWafRegionalWebAclDetailsOutputTypeDef],
+        "AwsWafRule": NotRequired[AwsWafRuleDetailsOutputTypeDef],
+        "AwsWafRuleGroup": NotRequired[AwsWafRuleGroupDetailsOutputTypeDef],
+        "AwsEcsTask": NotRequired[AwsEcsTaskDetailsOutputTypeDef],
+        "AwsBackupBackupVault": NotRequired[AwsBackupBackupVaultDetailsOutputTypeDef],
+        "AwsBackupBackupPlan": NotRequired[AwsBackupBackupPlanDetailsOutputTypeDef],
+        "AwsBackupRecoveryPoint": NotRequired[AwsBackupRecoveryPointDetailsTypeDef],
+        "AwsEc2LaunchTemplate": NotRequired[AwsEc2LaunchTemplateDetailsOutputTypeDef],
+        "AwsSageMakerNotebookInstance": NotRequired[
+            AwsSageMakerNotebookInstanceDetailsOutputTypeDef
+        ],
+        "AwsWafv2WebAcl": NotRequired[AwsWafv2WebAclDetailsOutputTypeDef],
+        "AwsWafv2RuleGroup": NotRequired[AwsWafv2RuleGroupDetailsOutputTypeDef],
+        "AwsEc2RouteTable": NotRequired[AwsEc2RouteTableDetailsOutputTypeDef],
+        "AwsAmazonMqBroker": NotRequired[AwsAmazonMqBrokerDetailsOutputTypeDef],
+        "AwsAppSyncGraphQlApi": NotRequired[AwsAppSyncGraphQlApiDetailsOutputTypeDef],
+        "AwsEventSchemasRegistry": NotRequired[AwsEventSchemasRegistryDetailsTypeDef],
+        "AwsGuardDutyDetector": NotRequired[AwsGuardDutyDetectorDetailsOutputTypeDef],
+        "AwsStepFunctionStateMachine": NotRequired[AwsStepFunctionStateMachineDetailsOutputTypeDef],
+        "AwsAthenaWorkGroup": NotRequired[AwsAthenaWorkGroupDetailsTypeDef],
+        "AwsEventsEventbus": NotRequired[AwsEventsEventbusDetailsTypeDef],
+        "AwsDmsEndpoint": NotRequired[AwsDmsEndpointDetailsTypeDef],
+        "AwsEventsEndpoint": NotRequired[AwsEventsEndpointDetailsOutputTypeDef],
+        "AwsDmsReplicationTask": NotRequired[AwsDmsReplicationTaskDetailsTypeDef],
+        "AwsDmsReplicationInstance": NotRequired[AwsDmsReplicationInstanceDetailsOutputTypeDef],
+        "AwsRoute53HostedZone": NotRequired[AwsRoute53HostedZoneDetailsOutputTypeDef],
+        "AwsMskCluster": NotRequired[AwsMskClusterDetailsOutputTypeDef],
+        "AwsS3AccessPoint": NotRequired[AwsS3AccessPointDetailsTypeDef],
+        "AwsEc2ClientVpnEndpoint": NotRequired[AwsEc2ClientVpnEndpointDetailsOutputTypeDef],
     },
 )
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "AwsAutoScalingAutoScalingGroup": NotRequired[AwsAutoScalingAutoScalingGroupDetailsTypeDef],
         "AwsCodeBuildProject": NotRequired[AwsCodeBuildProjectDetailsTypeDef],
@@ -11928,25 +15403,40 @@
         "AwsDmsReplicationInstance": NotRequired[AwsDmsReplicationInstanceDetailsTypeDef],
         "AwsRoute53HostedZone": NotRequired[AwsRoute53HostedZoneDetailsTypeDef],
         "AwsMskCluster": NotRequired[AwsMskClusterDetailsTypeDef],
         "AwsS3AccessPoint": NotRequired[AwsS3AccessPointDetailsTypeDef],
         "AwsEc2ClientVpnEndpoint": NotRequired[AwsEc2ClientVpnEndpointDetailsTypeDef],
     },
 )
-ResourcePaginatorTypeDef = TypedDict(
-    "ResourcePaginatorTypeDef",
+ResourceExtraOutputTypeDef = TypedDict(
+    "ResourceExtraOutputTypeDef",
     {
         "Type": str,
         "Id": str,
         "Partition": NotRequired[PartitionType],
         "Region": NotRequired[str],
         "ResourceRole": NotRequired[str],
         "Tags": NotRequired[Dict[str, str]],
-        "DataClassification": NotRequired[DataClassificationDetailsPaginatorTypeDef],
-        "Details": NotRequired[ResourceDetailsPaginatorTypeDef],
+        "DataClassification": NotRequired[DataClassificationDetailsExtraOutputTypeDef],
+        "Details": NotRequired[ResourceDetailsExtraOutputTypeDef],
+        "ApplicationName": NotRequired[str],
+        "ApplicationArn": NotRequired[str],
+    },
+)
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
+    {
+        "Type": str,
+        "Id": str,
+        "Partition": NotRequired[PartitionType],
+        "Region": NotRequired[str],
+        "ResourceRole": NotRequired[str],
+        "Tags": NotRequired[Dict[str, str]],
+        "DataClassification": NotRequired[DataClassificationDetailsOutputTypeDef],
+        "Details": NotRequired[ResourceDetailsOutputTypeDef],
         "ApplicationName": NotRequired[str],
         "ApplicationArn": NotRequired[str],
     },
 )
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
@@ -11958,27 +15448,76 @@
         "Tags": NotRequired[Mapping[str, str]],
         "DataClassification": NotRequired[DataClassificationDetailsTypeDef],
         "Details": NotRequired[ResourceDetailsTypeDef],
         "ApplicationName": NotRequired[str],
         "ApplicationArn": NotRequired[str],
     },
 )
-AwsSecurityFindingPaginatorTypeDef = TypedDict(
-    "AwsSecurityFindingPaginatorTypeDef",
+AwsSecurityFindingExtraOutputTypeDef = TypedDict(
+    "AwsSecurityFindingExtraOutputTypeDef",
+    {
+        "SchemaVersion": str,
+        "Id": str,
+        "ProductArn": str,
+        "GeneratorId": str,
+        "AwsAccountId": str,
+        "CreatedAt": str,
+        "UpdatedAt": str,
+        "Title": str,
+        "Description": str,
+        "Resources": List[ResourceExtraOutputTypeDef],
+        "ProductName": NotRequired[str],
+        "CompanyName": NotRequired[str],
+        "Region": NotRequired[str],
+        "Types": NotRequired[List[str]],
+        "FirstObservedAt": NotRequired[str],
+        "LastObservedAt": NotRequired[str],
+        "Severity": NotRequired[SeverityTypeDef],
+        "Confidence": NotRequired[int],
+        "Criticality": NotRequired[int],
+        "Remediation": NotRequired[RemediationTypeDef],
+        "SourceUrl": NotRequired[str],
+        "ProductFields": NotRequired[Dict[str, str]],
+        "UserDefinedFields": NotRequired[Dict[str, str]],
+        "Malware": NotRequired[List[MalwareTypeDef]],
+        "Network": NotRequired[NetworkTypeDef],
+        "NetworkPath": NotRequired[List[NetworkPathComponentExtraOutputTypeDef]],
+        "Process": NotRequired[ProcessDetailsTypeDef],
+        "Threats": NotRequired[List[ThreatExtraOutputTypeDef]],
+        "ThreatIntelIndicators": NotRequired[List[ThreatIntelIndicatorTypeDef]],
+        "Compliance": NotRequired[ComplianceExtraOutputTypeDef],
+        "VerificationState": NotRequired[VerificationStateType],
+        "WorkflowState": NotRequired[WorkflowStateType],
+        "Workflow": NotRequired[WorkflowTypeDef],
+        "RecordState": NotRequired[RecordStateType],
+        "RelatedFindings": NotRequired[List[RelatedFindingTypeDef]],
+        "Note": NotRequired[NoteTypeDef],
+        "Vulnerabilities": NotRequired[List[VulnerabilityExtraOutputTypeDef]],
+        "PatchSummary": NotRequired[PatchSummaryTypeDef],
+        "Action": NotRequired[ActionExtraOutputTypeDef],
+        "FindingProviderFields": NotRequired[FindingProviderFieldsExtraOutputTypeDef],
+        "Sample": NotRequired[bool],
+        "GeneratorDetails": NotRequired[GeneratorDetailsExtraOutputTypeDef],
+        "ProcessedAt": NotRequired[str],
+        "AwsAccountName": NotRequired[str],
+    },
+)
+AwsSecurityFindingOutputTypeDef = TypedDict(
+    "AwsSecurityFindingOutputTypeDef",
     {
         "SchemaVersion": str,
         "Id": str,
         "ProductArn": str,
         "GeneratorId": str,
         "AwsAccountId": str,
         "CreatedAt": str,
         "UpdatedAt": str,
         "Title": str,
         "Description": str,
-        "Resources": List[ResourcePaginatorTypeDef],
+        "Resources": List[ResourceOutputTypeDef],
         "ProductName": NotRequired[str],
         "CompanyName": NotRequired[str],
         "Region": NotRequired[str],
         "Types": NotRequired[List[str]],
         "FirstObservedAt": NotRequired[str],
         "LastObservedAt": NotRequired[str],
         "Severity": NotRequired[SeverityTypeDef],
@@ -11986,31 +15525,31 @@
         "Criticality": NotRequired[int],
         "Remediation": NotRequired[RemediationTypeDef],
         "SourceUrl": NotRequired[str],
         "ProductFields": NotRequired[Dict[str, str]],
         "UserDefinedFields": NotRequired[Dict[str, str]],
         "Malware": NotRequired[List[MalwareTypeDef]],
         "Network": NotRequired[NetworkTypeDef],
-        "NetworkPath": NotRequired[List[NetworkPathComponentPaginatorTypeDef]],
+        "NetworkPath": NotRequired[List[NetworkPathComponentOutputTypeDef]],
         "Process": NotRequired[ProcessDetailsTypeDef],
-        "Threats": NotRequired[List[ThreatPaginatorTypeDef]],
+        "Threats": NotRequired[List[ThreatOutputTypeDef]],
         "ThreatIntelIndicators": NotRequired[List[ThreatIntelIndicatorTypeDef]],
-        "Compliance": NotRequired[CompliancePaginatorTypeDef],
+        "Compliance": NotRequired[ComplianceOutputTypeDef],
         "VerificationState": NotRequired[VerificationStateType],
         "WorkflowState": NotRequired[WorkflowStateType],
         "Workflow": NotRequired[WorkflowTypeDef],
         "RecordState": NotRequired[RecordStateType],
         "RelatedFindings": NotRequired[List[RelatedFindingTypeDef]],
         "Note": NotRequired[NoteTypeDef],
-        "Vulnerabilities": NotRequired[List[VulnerabilityPaginatorTypeDef]],
+        "Vulnerabilities": NotRequired[List[VulnerabilityOutputTypeDef]],
         "PatchSummary": NotRequired[PatchSummaryTypeDef],
-        "Action": NotRequired[ActionPaginatorTypeDef],
-        "FindingProviderFields": NotRequired[FindingProviderFieldsPaginatorTypeDef],
+        "Action": NotRequired[ActionOutputTypeDef],
+        "FindingProviderFields": NotRequired[FindingProviderFieldsOutputTypeDef],
         "Sample": NotRequired[bool],
-        "GeneratorDetails": NotRequired[GeneratorDetailsPaginatorTypeDef],
+        "GeneratorDetails": NotRequired[GeneratorDetailsOutputTypeDef],
         "ProcessedAt": NotRequired[str],
         "AwsAccountName": NotRequired[str],
     },
 )
 AwsSecurityFindingTypeDef = TypedDict(
     "AwsSecurityFindingTypeDef",
     {
@@ -12056,29 +15595,24 @@
         "FindingProviderFields": NotRequired[FindingProviderFieldsTypeDef],
         "Sample": NotRequired[bool],
         "GeneratorDetails": NotRequired[GeneratorDetailsTypeDef],
         "ProcessedAt": NotRequired[str],
         "AwsAccountName": NotRequired[str],
     },
 )
-GetFindingsResponsePaginatorTypeDef = TypedDict(
-    "GetFindingsResponsePaginatorTypeDef",
+GetFindingsResponseTypeDef = TypedDict(
+    "GetFindingsResponseTypeDef",
     {
-        "Findings": List[AwsSecurityFindingPaginatorTypeDef],
-        "NextToken": str,
+        "Findings": List[AwsSecurityFindingOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
+AwsSecurityFindingUnionTypeDef = Union[
+    AwsSecurityFindingTypeDef, AwsSecurityFindingExtraOutputTypeDef
+]
 BatchImportFindingsRequestRequestTypeDef = TypedDict(
     "BatchImportFindingsRequestRequestTypeDef",
     {
-        "Findings": Sequence[AwsSecurityFindingTypeDef],
-    },
-)
-GetFindingsResponseTypeDef = TypedDict(
-    "GetFindingsResponseTypeDef",
-    {
-        "Findings": List[AwsSecurityFindingTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Findings": Sequence[AwsSecurityFindingUnionTypeDef],
     },
 )
```

### Comparing `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/type_defs.pyi` & `mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub/type_defs.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -71,17 +71,17 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     "AcceptInvitationRequestRequestTypeDef",
     "AccountDetailsTypeDef",
+    "DnsRequestActionTypeDef",
     "ActionLocalIpDetailsTypeDef",
     "ActionLocalPortDetailsTypeDef",
-    "DnsRequestActionTypeDef",
     "CityTypeDef",
     "CountryTypeDef",
     "GeoLocationTypeDef",
     "IpOrganizationDetailsTypeDef",
     "ActionRemotePortDetailsTypeDef",
     "ActionTargetTypeDef",
     "AdjustmentTypeDef",
@@ -95,27 +95,31 @@
     "WorkflowUpdateTypeDef",
     "MapFilterTypeDef",
     "NumberFilterTypeDef",
     "StringFilterTypeDef",
     "AutomationRulesMetadataTypeDef",
     "AvailabilityZoneTypeDef",
     "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
-    "AwsAmazonMqBrokerLdapServerMetadataDetailsPaginatorTypeDef",
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsExtraOutputTypeDef",
     "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef",
     "AwsAmazonMqBrokerUsersDetailsTypeDef",
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef",
     "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
     "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
     "AwsApiCallActionDomainDetailsTypeDef",
     "AwsApiGatewayAccessLogSettingsTypeDef",
-    "AwsApiGatewayCanarySettingsPaginatorTypeDef",
+    "AwsApiGatewayCanarySettingsExtraOutputTypeDef",
+    "AwsApiGatewayCanarySettingsOutputTypeDef",
     "AwsApiGatewayCanarySettingsTypeDef",
-    "AwsApiGatewayEndpointConfigurationPaginatorTypeDef",
+    "AwsApiGatewayEndpointConfigurationExtraOutputTypeDef",
+    "AwsApiGatewayEndpointConfigurationOutputTypeDef",
     "AwsApiGatewayEndpointConfigurationTypeDef",
     "AwsApiGatewayMethodSettingsTypeDef",
-    "AwsCorsConfigurationPaginatorTypeDef",
+    "AwsCorsConfigurationExtraOutputTypeDef",
+    "AwsCorsConfigurationOutputTypeDef",
     "AwsCorsConfigurationTypeDef",
     "AwsApiGatewayV2RouteSettingsTypeDef",
     "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiLogConfigDetailsTypeDef",
     "AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef",
@@ -123,42 +127,47 @@
     "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef",
-    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsPaginatorTypeDef",
+    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsExtraOutputTypeDef",
+    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef",
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef",
     "AwsBackupBackupPlanLifecycleDetailsTypeDef",
-    "AwsBackupBackupVaultNotificationsDetailsPaginatorTypeDef",
+    "AwsBackupBackupVaultNotificationsDetailsExtraOutputTypeDef",
+    "AwsBackupBackupVaultNotificationsDetailsOutputTypeDef",
     "AwsBackupBackupVaultNotificationsDetailsTypeDef",
     "AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef",
     "AwsBackupRecoveryPointCreatedByDetailsTypeDef",
     "AwsBackupRecoveryPointLifecycleDetailsTypeDef",
     "AwsCertificateManagerCertificateExtendedKeyUsageTypeDef",
     "AwsCertificateManagerCertificateKeyUsageTypeDef",
     "AwsCertificateManagerCertificateOptionsTypeDef",
     "AwsCertificateManagerCertificateResourceRecordTypeDef",
     "AwsCloudFormationStackDriftInformationDetailsTypeDef",
     "AwsCloudFormationStackOutputsDetailsTypeDef",
     "AwsCloudFrontDistributionCacheBehaviorTypeDef",
     "AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef",
     "AwsCloudFrontDistributionLoggingTypeDef",
     "AwsCloudFrontDistributionViewerCertificateTypeDef",
-    "AwsCloudFrontDistributionOriginSslProtocolsPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginSslProtocolsExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef",
     "AwsCloudFrontDistributionOriginSslProtocolsTypeDef",
-    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef",
     "AwsCloudFrontDistributionOriginS3OriginConfigTypeDef",
     "AwsCloudTrailTrailDetailsTypeDef",
     "AwsCloudWatchAlarmDimensionsDetailsTypeDef",
     "AwsCodeBuildProjectArtifactsDetailsTypeDef",
     "AwsCodeBuildProjectSourceTypeDef",
-    "AwsCodeBuildProjectVpcConfigPaginatorTypeDef",
+    "AwsCodeBuildProjectVpcConfigExtraOutputTypeDef",
+    "AwsCodeBuildProjectVpcConfigOutputTypeDef",
     "AwsCodeBuildProjectVpcConfigTypeDef",
     "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef",
     "AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef",
     "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef",
     "AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef",
     "AwsDmsEndpointDetailsTypeDef",
     "AwsDmsReplicationInstanceReplicationSubnetGroupDetailsTypeDef",
@@ -167,15 +176,16 @@
     "AwsDynamoDbTableAttributeDefinitionTypeDef",
     "AwsDynamoDbTableBillingModeSummaryTypeDef",
     "AwsDynamoDbTableKeySchemaTypeDef",
     "AwsDynamoDbTableProvisionedThroughputTypeDef",
     "AwsDynamoDbTableRestoreSummaryTypeDef",
     "AwsDynamoDbTableSseDescriptionTypeDef",
     "AwsDynamoDbTableStreamSpecificationTypeDef",
-    "AwsDynamoDbTableProjectionPaginatorTypeDef",
+    "AwsDynamoDbTableProjectionExtraOutputTypeDef",
+    "AwsDynamoDbTableProjectionOutputTypeDef",
     "AwsDynamoDbTableProjectionTypeDef",
     "AwsDynamoDbTableProvisionedThroughputOverrideTypeDef",
     "AwsEc2ClientVpnEndpointAuthenticationOptionsActiveDirectoryDetailsTypeDef",
     "AwsEc2ClientVpnEndpointAuthenticationOptionsFederatedAuthenticationDetailsTypeDef",
     "AwsEc2ClientVpnEndpointAuthenticationOptionsMutualAuthenticationDetailsTypeDef",
     "AwsEc2ClientVpnEndpointClientConnectOptionsStatusDetailsTypeDef",
     "AwsEc2ClientVpnEndpointClientLoginBannerOptionsDetailsTypeDef",
@@ -222,101 +232,116 @@
     "PropagatingVgwSetDetailsTypeDef",
     "RouteSetDetailsTypeDef",
     "AwsEc2SecurityGroupIpRangeTypeDef",
     "AwsEc2SecurityGroupIpv6RangeTypeDef",
     "AwsEc2SecurityGroupPrefixListIdTypeDef",
     "AwsEc2SecurityGroupUserIdGroupPairTypeDef",
     "Ipv6CidrBlockAssociationTypeDef",
-    "AwsEc2TransitGatewayDetailsPaginatorTypeDef",
+    "AwsEc2TransitGatewayDetailsExtraOutputTypeDef",
+    "AwsEc2TransitGatewayDetailsOutputTypeDef",
     "AwsEc2TransitGatewayDetailsTypeDef",
     "AwsEc2VolumeAttachmentTypeDef",
     "CidrBlockAssociationTypeDef",
     "AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef",
     "AwsEc2VpcPeeringConnectionStatusDetailsTypeDef",
     "VpcInfoCidrBlockSetDetailsTypeDef",
     "VpcInfoIpv6CidrBlockSetDetailsTypeDef",
     "VpcInfoPeeringOptionsDetailsTypeDef",
     "AwsEc2VpnConnectionRoutesDetailsTypeDef",
     "AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef",
-    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsPaginatorTypeDef",
+    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsExtraOutputTypeDef",
+    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef",
     "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef",
-    "AwsEcrContainerImageDetailsPaginatorTypeDef",
+    "AwsEcrContainerImageDetailsExtraOutputTypeDef",
+    "AwsEcrContainerImageDetailsOutputTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef",
     "AwsEcrRepositoryLifecyclePolicyDetailsTypeDef",
     "AwsEcsClusterClusterSettingsDetailsTypeDef",
     "AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef",
     "AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef",
     "AwsMountPointTypeDef",
     "AwsEcsServiceCapacityProviderStrategyDetailsTypeDef",
     "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef",
     "AwsEcsServiceDeploymentControllerDetailsTypeDef",
     "AwsEcsServiceLoadBalancersDetailsTypeDef",
     "AwsEcsServicePlacementConstraintsDetailsTypeDef",
     "AwsEcsServicePlacementStrategiesDetailsTypeDef",
     "AwsEcsServiceServiceRegistriesDetailsTypeDef",
-    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsPaginatorTypeDef",
+    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsExtraOutputTypeDef",
+    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef",
     "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsPaginatorTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsExtraOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsPaginatorTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef",
     "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef",
     "AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef",
     "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef",
-    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsExtraOutputTypeDef",
     "AwsEcsTaskDefinitionVolumesHostDetailsTypeDef",
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef",
     "AwsEcsTaskVolumeHostDetailsTypeDef",
-    "AwsEfsAccessPointPosixUserDetailsPaginatorTypeDef",
+    "AwsEfsAccessPointPosixUserDetailsExtraOutputTypeDef",
+    "AwsEfsAccessPointPosixUserDetailsOutputTypeDef",
     "AwsEfsAccessPointPosixUserDetailsTypeDef",
     "AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef",
-    "AwsEksClusterResourcesVpcConfigDetailsPaginatorTypeDef",
+    "AwsEksClusterResourcesVpcConfigDetailsExtraOutputTypeDef",
+    "AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef",
     "AwsEksClusterResourcesVpcConfigDetailsTypeDef",
-    "AwsEksClusterLoggingClusterLoggingDetailsPaginatorTypeDef",
+    "AwsEksClusterLoggingClusterLoggingDetailsExtraOutputTypeDef",
+    "AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef",
     "AwsEksClusterLoggingClusterLoggingDetailsTypeDef",
     "AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef",
     "AwsElasticBeanstalkEnvironmentOptionSettingTypeDef",
     "AwsElasticBeanstalkEnvironmentTierTypeDef",
     "AwsElasticsearchDomainDomainEndpointOptionsTypeDef",
     "AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef",
     "AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef",
     "AwsElasticsearchDomainServiceSoftwareOptionsTypeDef",
-    "AwsElasticsearchDomainVPCOptionsPaginatorTypeDef",
+    "AwsElasticsearchDomainVPCOptionsExtraOutputTypeDef",
+    "AwsElasticsearchDomainVPCOptionsOutputTypeDef",
     "AwsElasticsearchDomainVPCOptionsTypeDef",
     "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef",
     "AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef",
     "AwsElbAppCookieStickinessPolicyTypeDef",
     "AwsElbLbCookieStickinessPolicyTypeDef",
     "AwsElbLoadBalancerAccessLogTypeDef",
     "AwsElbLoadBalancerAdditionalAttributeTypeDef",
     "AwsElbLoadBalancerConnectionDrainingTypeDef",
     "AwsElbLoadBalancerConnectionSettingsTypeDef",
     "AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef",
-    "AwsElbLoadBalancerBackendServerDescriptionPaginatorTypeDef",
+    "AwsElbLoadBalancerBackendServerDescriptionExtraOutputTypeDef",
+    "AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef",
     "AwsElbLoadBalancerBackendServerDescriptionTypeDef",
     "AwsElbLoadBalancerHealthCheckTypeDef",
     "AwsElbLoadBalancerInstanceTypeDef",
     "AwsElbLoadBalancerSourceSecurityGroupTypeDef",
     "AwsElbLoadBalancerListenerTypeDef",
     "AwsElbv2LoadBalancerAttributeTypeDef",
     "LoadBalancerStateTypeDef",
@@ -344,55 +369,62 @@
     "AwsIamUserPolicyTypeDef",
     "AwsKinesisStreamStreamEncryptionDetailsTypeDef",
     "AwsKmsKeyDetailsTypeDef",
     "AwsLambdaFunctionCodeTypeDef",
     "AwsLambdaFunctionDeadLetterConfigTypeDef",
     "AwsLambdaFunctionLayerTypeDef",
     "AwsLambdaFunctionTracingConfigTypeDef",
-    "AwsLambdaFunctionVpcConfigPaginatorTypeDef",
+    "AwsLambdaFunctionVpcConfigExtraOutputTypeDef",
+    "AwsLambdaFunctionVpcConfigOutputTypeDef",
     "AwsLambdaFunctionVpcConfigTypeDef",
     "AwsLambdaFunctionEnvironmentErrorTypeDef",
-    "AwsLambdaLayerVersionDetailsPaginatorTypeDef",
+    "AwsLambdaLayerVersionDetailsExtraOutputTypeDef",
+    "AwsLambdaLayerVersionDetailsOutputTypeDef",
     "AwsLambdaLayerVersionDetailsTypeDef",
-    "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsPaginatorTypeDef",
+    "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsExtraOutputTypeDef",
     "AwsMskClusterClusterInfoClientAuthenticationUnauthenticatedDetailsTypeDef",
+    "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsOutputTypeDef",
     "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsTypeDef",
     "AwsMskClusterClusterInfoClientAuthenticationSaslIamDetailsTypeDef",
     "AwsMskClusterClusterInfoClientAuthenticationSaslScramDetailsTypeDef",
     "AwsMskClusterClusterInfoEncryptionInfoEncryptionAtRestDetailsTypeDef",
     "AwsMskClusterClusterInfoEncryptionInfoEncryptionInTransitDetailsTypeDef",
     "AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef",
     "AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef",
     "AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef",
-    "AwsOpenSearchServiceDomainVpcOptionsDetailsPaginatorTypeDef",
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsExtraOutputTypeDef",
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainLogPublishingOptionTypeDef",
     "AwsRdsDbClusterAssociatedRoleTypeDef",
     "AwsRdsDbClusterMemberTypeDef",
     "AwsRdsDbClusterOptionGroupMembershipTypeDef",
     "AwsRdsDbDomainMembershipTypeDef",
     "AwsRdsDbInstanceVpcSecurityGroupTypeDef",
-    "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributePaginatorTypeDef",
+    "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeExtraOutputTypeDef",
+    "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef",
     "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef",
     "AwsRdsDbInstanceAssociatedRoleTypeDef",
     "AwsRdsDbInstanceEndpointTypeDef",
     "AwsRdsDbOptionGroupMembershipTypeDef",
     "AwsRdsDbParameterGroupTypeDef",
     "AwsRdsDbProcessorFeatureTypeDef",
     "AwsRdsDbStatusInfoTypeDef",
-    "AwsRdsPendingCloudWatchLogsExportsPaginatorTypeDef",
+    "AwsRdsPendingCloudWatchLogsExportsExtraOutputTypeDef",
+    "AwsRdsPendingCloudWatchLogsExportsOutputTypeDef",
     "AwsRdsPendingCloudWatchLogsExportsTypeDef",
     "AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef",
     "AwsRdsDbSecurityGroupIpRangeTypeDef",
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef",
-    "AwsRdsEventSubscriptionDetailsPaginatorTypeDef",
+    "AwsRdsEventSubscriptionDetailsExtraOutputTypeDef",
+    "AwsRdsEventSubscriptionDetailsOutputTypeDef",
     "AwsRdsEventSubscriptionDetailsTypeDef",
     "AwsRedshiftClusterClusterNodeTypeDef",
     "AwsRedshiftClusterClusterParameterStatusTypeDef",
     "AwsRedshiftClusterClusterSecurityGroupTypeDef",
     "AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef",
     "AwsRedshiftClusterDeferredMaintenanceWindowTypeDef",
     "AwsRedshiftClusterElasticIpStatusTypeDef",
@@ -421,26 +453,27 @@
     "AwsS3BucketServerSideEncryptionByDefaultTypeDef",
     "AwsS3BucketWebsiteConfigurationRedirectToTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef",
     "AwsS3ObjectDetailsTypeDef",
     "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
     "AwsSecretsManagerSecretRotationRulesTypeDef",
-    "BooleanFilterTypeDef",
-    "IpFilterTypeDef",
-    "KeywordFilterTypeDef",
-    "AwsSecurityFindingIdentifierTypeDef",
-    "GeneratorDetailsPaginatorTypeDef",
+    "GeneratorDetailsExtraOutputTypeDef",
     "MalwareTypeDef",
     "NoteTypeDef",
     "PatchSummaryTypeDef",
     "ProcessDetailsTypeDef",
     "SeverityTypeDef",
     "ThreatIntelIndicatorTypeDef",
     "WorkflowTypeDef",
+    "BooleanFilterTypeDef",
+    "IpFilterTypeDef",
+    "KeywordFilterTypeDef",
+    "AwsSecurityFindingIdentifierTypeDef",
+    "GeneratorDetailsOutputTypeDef",
     "GeneratorDetailsTypeDef",
     "AwsSnsTopicSubscriptionTypeDef",
     "AwsSqsQueueDetailsTypeDef",
     "AwsSsmComplianceSummaryTypeDef",
     "AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef",
     "AwsWafRateBasedRuleMatchPredicateTypeDef",
@@ -471,16 +504,17 @@
     "StandardsControlAssociationDetailTypeDef",
     "ImportFindingsErrorTypeDef",
     "StandardsControlAssociationUpdateTypeDef",
     "BooleanConfigurationOptionsTypeDef",
     "CellTypeDef",
     "ClassificationStatusTypeDef",
     "CodeVulnerabilitiesFilePathTypeDef",
-    "SecurityControlParameterPaginatorTypeDef",
+    "SecurityControlParameterExtraOutputTypeDef",
     "StatusReasonTypeDef",
+    "SecurityControlParameterOutputTypeDef",
     "SecurityControlParameterTypeDef",
     "DoubleConfigurationOptionsTypeDef",
     "EnumConfigurationOptionsTypeDef",
     "EnumListConfigurationOptionsTypeDef",
     "IntegerConfigurationOptionsTypeDef",
     "IntegerListConfigurationOptionsTypeDef",
     "StringConfigurationOptionsTypeDef",
@@ -544,216 +578,284 @@
     "ListSecurityControlDefinitionsRequestRequestTypeDef",
     "ListStandardsControlAssociationsRequestRequestTypeDef",
     "StandardsControlAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PortRangeTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
+    "ParameterValueOutputTypeDef",
     "ParameterValueTypeDef",
     "RecommendationTypeDef",
-    "RuleGroupSourceListDetailsPaginatorTypeDef",
+    "RuleGroupSourceListDetailsExtraOutputTypeDef",
+    "RuleGroupSourceListDetailsOutputTypeDef",
     "RuleGroupSourceListDetailsTypeDef",
     "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
-    "RuleGroupSourceStatefulRulesOptionsDetailsPaginatorTypeDef",
+    "RuleGroupSourceStatefulRulesOptionsDetailsExtraOutputTypeDef",
+    "RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef",
     "RuleGroupSourceStatefulRulesOptionsDetailsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
-    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsPaginatorTypeDef",
+    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsExtraOutputTypeDef",
+    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
-    "RuleGroupVariablesIpSetsDetailsPaginatorTypeDef",
+    "RuleGroupVariablesIpSetsDetailsExtraOutputTypeDef",
+    "RuleGroupVariablesPortSetsDetailsExtraOutputTypeDef",
+    "RuleGroupVariablesIpSetsDetailsOutputTypeDef",
     "RuleGroupVariablesIpSetsDetailsTypeDef",
-    "RuleGroupVariablesPortSetsDetailsPaginatorTypeDef",
+    "RuleGroupVariablesPortSetsDetailsOutputTypeDef",
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     "SoftwarePackageTypeDef",
     "StandardsManagedByTypeDef",
     "StandardsStatusReasonTypeDef",
     "StatelessCustomPublishMetricActionDimensionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateActionTargetRequestRequestTypeDef",
     "UpdateFindingAggregatorRequestRequestTypeDef",
     "UpdateSecurityHubConfigurationRequestRequestTypeDef",
     "UpdateStandardsControlRequestRequestTypeDef",
     "VulnerabilityVendorTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "ActionRemoteIpDetailsTypeDef",
-    "CvssPaginatorTypeDef",
+    "CvssExtraOutputTypeDef",
+    "CvssOutputTypeDef",
     "CvssTypeDef",
     "ListConfigurationPolicyAssociationsRequestRequestTypeDef",
     "AssociationSetDetailsTypeDef",
+    "AutomationRulesFindingFieldsUpdateOutputTypeDef",
     "AutomationRulesFindingFieldsUpdateTypeDef",
     "AwsAmazonMqBrokerLogsDetailsTypeDef",
-    "AwsApiGatewayRestApiDetailsPaginatorTypeDef",
+    "AwsApiGatewayRestApiDetailsExtraOutputTypeDef",
+    "AwsApiGatewayRestApiDetailsOutputTypeDef",
     "AwsApiGatewayRestApiDetailsTypeDef",
-    "AwsApiGatewayStageDetailsPaginatorTypeDef",
+    "AwsApiGatewayStageDetailsExtraOutputTypeDef",
+    "AwsApiGatewayStageDetailsOutputTypeDef",
     "AwsApiGatewayStageDetailsTypeDef",
-    "AwsApiGatewayV2ApiDetailsPaginatorTypeDef",
+    "AwsApiGatewayV2ApiDetailsExtraOutputTypeDef",
+    "AwsApiGatewayV2ApiDetailsOutputTypeDef",
     "AwsApiGatewayV2ApiDetailsTypeDef",
-    "AwsApiGatewayV2StageDetailsPaginatorTypeDef",
+    "AwsApiGatewayV2StageDetailsExtraOutputTypeDef",
+    "AwsApiGatewayV2StageDetailsOutputTypeDef",
     "AwsApiGatewayV2StageDetailsTypeDef",
     "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef",
     "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef",
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsPaginatorTypeDef",
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsExtraOutputTypeDef",
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef",
     "AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef",
-    "AwsBackupBackupVaultDetailsPaginatorTypeDef",
+    "AwsBackupBackupVaultDetailsExtraOutputTypeDef",
+    "AwsBackupBackupVaultDetailsOutputTypeDef",
     "AwsBackupBackupVaultDetailsTypeDef",
     "AwsBackupRecoveryPointDetailsTypeDef",
-    "AwsCertificateManagerCertificateDomainValidationOptionPaginatorTypeDef",
+    "AwsCertificateManagerCertificateDomainValidationOptionExtraOutputTypeDef",
+    "AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef",
     "AwsCertificateManagerCertificateDomainValidationOptionTypeDef",
-    "AwsCloudFormationStackDetailsPaginatorTypeDef",
+    "AwsCloudFormationStackDetailsExtraOutputTypeDef",
+    "AwsCloudFormationStackDetailsOutputTypeDef",
     "AwsCloudFormationStackDetailsTypeDef",
-    "AwsCloudFrontDistributionCacheBehaviorsPaginatorTypeDef",
+    "AwsCloudFrontDistributionCacheBehaviorsExtraOutputTypeDef",
+    "AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef",
     "AwsCloudFrontDistributionCacheBehaviorsTypeDef",
-    "AwsCloudFrontDistributionOriginCustomOriginConfigPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginCustomOriginConfigExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef",
     "AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef",
-    "AwsCloudFrontDistributionOriginGroupFailoverPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginGroupFailoverExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverTypeDef",
-    "AwsCloudWatchAlarmDetailsPaginatorTypeDef",
+    "AwsCloudWatchAlarmDetailsExtraOutputTypeDef",
+    "AwsCloudWatchAlarmDetailsOutputTypeDef",
     "AwsCloudWatchAlarmDetailsTypeDef",
-    "AwsCodeBuildProjectEnvironmentPaginatorTypeDef",
+    "AwsCodeBuildProjectEnvironmentExtraOutputTypeDef",
+    "AwsCodeBuildProjectEnvironmentOutputTypeDef",
     "AwsCodeBuildProjectEnvironmentTypeDef",
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
-    "AwsDmsReplicationInstanceDetailsPaginatorTypeDef",
+    "AwsDmsReplicationInstanceDetailsExtraOutputTypeDef",
+    "AwsDmsReplicationInstanceDetailsOutputTypeDef",
     "AwsDmsReplicationInstanceDetailsTypeDef",
-    "AwsDynamoDbTableGlobalSecondaryIndexPaginatorTypeDef",
-    "AwsDynamoDbTableLocalSecondaryIndexPaginatorTypeDef",
+    "AwsDynamoDbTableGlobalSecondaryIndexExtraOutputTypeDef",
+    "AwsDynamoDbTableLocalSecondaryIndexExtraOutputTypeDef",
+    "AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef",
+    "AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef",
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     "AwsDynamoDbTableLocalSecondaryIndexTypeDef",
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef",
     "AwsEc2ClientVpnEndpointAuthenticationOptionsDetailsTypeDef",
     "AwsEc2ClientVpnEndpointClientConnectOptionsDetailsTypeDef",
-    "AwsEc2InstanceDetailsPaginatorTypeDef",
+    "AwsEc2InstanceDetailsExtraOutputTypeDef",
+    "AwsEc2InstanceDetailsOutputTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsPaginatorTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsExtraOutputTypeDef",
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsPaginatorTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsExtraOutputTypeDef",
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
     "AwsEc2NetworkAclEntryTypeDef",
-    "AwsEc2NetworkInterfaceDetailsPaginatorTypeDef",
+    "AwsEc2NetworkInterfaceDetailsExtraOutputTypeDef",
+    "AwsEc2NetworkInterfaceDetailsOutputTypeDef",
     "AwsEc2NetworkInterfaceDetailsTypeDef",
-    "AwsEc2SecurityGroupIpPermissionPaginatorTypeDef",
+    "AwsEc2SecurityGroupIpPermissionExtraOutputTypeDef",
+    "AwsEc2SecurityGroupIpPermissionOutputTypeDef",
     "AwsEc2SecurityGroupIpPermissionTypeDef",
-    "AwsEc2SubnetDetailsPaginatorTypeDef",
+    "AwsEc2SubnetDetailsExtraOutputTypeDef",
+    "AwsEc2SubnetDetailsOutputTypeDef",
     "AwsEc2SubnetDetailsTypeDef",
-    "AwsEc2VolumeDetailsPaginatorTypeDef",
+    "AwsEc2VolumeDetailsExtraOutputTypeDef",
+    "AwsEc2VolumeDetailsOutputTypeDef",
     "AwsEc2VolumeDetailsTypeDef",
-    "AwsEc2VpcDetailsPaginatorTypeDef",
+    "AwsEc2VpcDetailsExtraOutputTypeDef",
+    "AwsEc2VpcDetailsOutputTypeDef",
     "AwsEc2VpcDetailsTypeDef",
-    "AwsEc2VpcEndpointServiceDetailsPaginatorTypeDef",
+    "AwsEc2VpcEndpointServiceDetailsExtraOutputTypeDef",
+    "AwsEc2VpcEndpointServiceDetailsOutputTypeDef",
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
-    "AwsEc2VpcPeeringConnectionVpcInfoDetailsPaginatorTypeDef",
+    "AwsEc2VpcPeeringConnectionVpcInfoDetailsExtraOutputTypeDef",
+    "AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef",
     "AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef",
-    "AwsEc2VpnConnectionOptionsDetailsPaginatorTypeDef",
+    "AwsEc2VpnConnectionOptionsDetailsExtraOutputTypeDef",
+    "AwsEc2VpnConnectionOptionsDetailsOutputTypeDef",
     "AwsEc2VpnConnectionOptionsDetailsTypeDef",
     "AwsEcrRepositoryDetailsTypeDef",
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef",
-    "AwsEcsContainerDetailsPaginatorTypeDef",
+    "AwsEcsContainerDetailsExtraOutputTypeDef",
+    "AwsEcsContainerDetailsOutputTypeDef",
     "AwsEcsContainerDetailsTypeDef",
     "AwsEcsServiceDeploymentConfigurationDetailsTypeDef",
-    "AwsEcsServiceNetworkConfigurationDetailsPaginatorTypeDef",
+    "AwsEcsServiceNetworkConfigurationDetailsExtraOutputTypeDef",
+    "AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef",
     "AwsEcsServiceNetworkConfigurationDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef",
-    "AwsEcsTaskDefinitionProxyConfigurationDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionProxyConfigurationDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef",
     "AwsEcsTaskVolumeDetailsTypeDef",
     "AwsEfsAccessPointRootDirectoryDetailsTypeDef",
-    "AwsEksClusterLoggingDetailsPaginatorTypeDef",
+    "AwsEksClusterLoggingDetailsExtraOutputTypeDef",
+    "AwsEksClusterLoggingDetailsOutputTypeDef",
     "AwsEksClusterLoggingDetailsTypeDef",
-    "AwsElasticBeanstalkEnvironmentDetailsPaginatorTypeDef",
+    "AwsElasticBeanstalkEnvironmentDetailsExtraOutputTypeDef",
+    "AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef",
     "AwsElasticBeanstalkEnvironmentDetailsTypeDef",
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
-    "AwsElbLoadBalancerPoliciesPaginatorTypeDef",
+    "AwsElbLoadBalancerPoliciesExtraOutputTypeDef",
+    "AwsElbLoadBalancerPoliciesOutputTypeDef",
     "AwsElbLoadBalancerPoliciesTypeDef",
-    "AwsElbLoadBalancerAttributesPaginatorTypeDef",
+    "AwsElbLoadBalancerAttributesExtraOutputTypeDef",
+    "AwsElbLoadBalancerAttributesOutputTypeDef",
     "AwsElbLoadBalancerAttributesTypeDef",
-    "AwsElbLoadBalancerListenerDescriptionPaginatorTypeDef",
+    "AwsElbLoadBalancerListenerDescriptionExtraOutputTypeDef",
+    "AwsElbLoadBalancerListenerDescriptionOutputTypeDef",
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
-    "AwsElbv2LoadBalancerDetailsPaginatorTypeDef",
+    "AwsElbv2LoadBalancerDetailsExtraOutputTypeDef",
+    "AwsElbv2LoadBalancerDetailsOutputTypeDef",
     "AwsElbv2LoadBalancerDetailsTypeDef",
     "AwsEventsEndpointRoutingConfigFailoverConfigDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef",
     "AwsIamAccessKeySessionContextTypeDef",
-    "AwsIamGroupDetailsPaginatorTypeDef",
+    "AwsIamGroupDetailsExtraOutputTypeDef",
+    "AwsIamGroupDetailsOutputTypeDef",
     "AwsIamGroupDetailsTypeDef",
-    "AwsIamInstanceProfilePaginatorTypeDef",
+    "AwsIamInstanceProfileExtraOutputTypeDef",
+    "AwsIamInstanceProfileOutputTypeDef",
     "AwsIamInstanceProfileTypeDef",
-    "AwsIamPolicyDetailsPaginatorTypeDef",
+    "AwsIamPolicyDetailsExtraOutputTypeDef",
+    "AwsIamPolicyDetailsOutputTypeDef",
     "AwsIamPolicyDetailsTypeDef",
-    "AwsIamUserDetailsPaginatorTypeDef",
+    "AwsIamUserDetailsExtraOutputTypeDef",
+    "AwsIamUserDetailsOutputTypeDef",
     "AwsIamUserDetailsTypeDef",
     "AwsKinesisStreamDetailsTypeDef",
-    "AwsLambdaFunctionEnvironmentPaginatorTypeDef",
+    "AwsLambdaFunctionEnvironmentExtraOutputTypeDef",
+    "AwsLambdaFunctionEnvironmentOutputTypeDef",
     "AwsLambdaFunctionEnvironmentTypeDef",
     "AwsMskClusterClusterInfoClientAuthenticationSaslDetailsTypeDef",
     "AwsMskClusterClusterInfoEncryptionInfoDetailsTypeDef",
-    "AwsNetworkFirewallFirewallDetailsPaginatorTypeDef",
+    "AwsNetworkFirewallFirewallDetailsExtraOutputTypeDef",
+    "AwsNetworkFirewallFirewallDetailsOutputTypeDef",
     "AwsNetworkFirewallFirewallDetailsTypeDef",
     "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef",
     "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef",
-    "AwsRdsDbClusterDetailsPaginatorTypeDef",
+    "AwsRdsDbClusterDetailsExtraOutputTypeDef",
+    "AwsRdsDbClusterDetailsOutputTypeDef",
     "AwsRdsDbClusterDetailsTypeDef",
-    "AwsRdsDbClusterSnapshotDetailsPaginatorTypeDef",
+    "AwsRdsDbClusterSnapshotDetailsExtraOutputTypeDef",
+    "AwsRdsDbClusterSnapshotDetailsOutputTypeDef",
     "AwsRdsDbClusterSnapshotDetailsTypeDef",
-    "AwsRdsDbSnapshotDetailsPaginatorTypeDef",
+    "AwsRdsDbSnapshotDetailsExtraOutputTypeDef",
+    "AwsRdsDbSnapshotDetailsOutputTypeDef",
     "AwsRdsDbSnapshotDetailsTypeDef",
-    "AwsRdsDbPendingModifiedValuesPaginatorTypeDef",
+    "AwsRdsDbPendingModifiedValuesExtraOutputTypeDef",
+    "AwsRdsDbPendingModifiedValuesOutputTypeDef",
     "AwsRdsDbPendingModifiedValuesTypeDef",
-    "AwsRdsDbSecurityGroupDetailsPaginatorTypeDef",
+    "AwsRdsDbSecurityGroupDetailsExtraOutputTypeDef",
+    "AwsRdsDbSecurityGroupDetailsOutputTypeDef",
     "AwsRdsDbSecurityGroupDetailsTypeDef",
     "AwsRdsDbSubnetGroupSubnetTypeDef",
-    "AwsRedshiftClusterClusterParameterGroupPaginatorTypeDef",
+    "AwsRedshiftClusterClusterParameterGroupExtraOutputTypeDef",
+    "AwsRedshiftClusterClusterParameterGroupOutputTypeDef",
     "AwsRedshiftClusterClusterParameterGroupTypeDef",
     "AwsRoute53HostedZoneObjectDetailsTypeDef",
     "AwsRoute53QueryLoggingConfigDetailsTypeDef",
     "AwsS3AccessPointDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef",
-    "AwsS3BucketNotificationConfigurationS3KeyFilterPaginatorTypeDef",
+    "AwsS3BucketNotificationConfigurationS3KeyFilterExtraOutputTypeDef",
+    "AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
     "AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef",
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
-    "AwsSageMakerNotebookInstanceDetailsPaginatorTypeDef",
+    "AwsSageMakerNotebookInstanceDetailsExtraOutputTypeDef",
+    "AwsSageMakerNotebookInstanceDetailsOutputTypeDef",
     "AwsSageMakerNotebookInstanceDetailsTypeDef",
     "AwsSecretsManagerSecretDetailsTypeDef",
     "BatchUpdateFindingsRequestRequestTypeDef",
     "BatchUpdateFindingsUnprocessedFindingTypeDef",
-    "AwsSnsTopicDetailsPaginatorTypeDef",
+    "AwsSnsTopicDetailsExtraOutputTypeDef",
+    "AwsSnsTopicDetailsOutputTypeDef",
     "AwsSnsTopicDetailsTypeDef",
     "AwsSsmPatchTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
-    "AwsWafRateBasedRuleDetailsPaginatorTypeDef",
+    "AwsWafRateBasedRuleDetailsExtraOutputTypeDef",
+    "AwsWafRateBasedRuleDetailsOutputTypeDef",
     "AwsWafRateBasedRuleDetailsTypeDef",
-    "AwsWafRegionalRateBasedRuleDetailsPaginatorTypeDef",
+    "AwsWafRegionalRateBasedRuleDetailsExtraOutputTypeDef",
+    "AwsWafRegionalRateBasedRuleDetailsOutputTypeDef",
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
-    "AwsWafRegionalRuleDetailsPaginatorTypeDef",
+    "AwsWafRegionalRuleDetailsExtraOutputTypeDef",
+    "AwsWafRegionalRuleDetailsOutputTypeDef",
     "AwsWafRegionalRuleDetailsTypeDef",
     "AwsWafRegionalRuleGroupRulesDetailsTypeDef",
     "AwsWafRegionalWebAclRulesListDetailsTypeDef",
-    "AwsWafRuleDetailsPaginatorTypeDef",
+    "AwsWafRuleDetailsExtraOutputTypeDef",
+    "AwsWafRuleDetailsOutputTypeDef",
     "AwsWafRuleDetailsTypeDef",
     "AwsWafRuleGroupRulesDetailsTypeDef",
-    "AwsWafWebAclRulePaginatorTypeDef",
+    "AwsWafWebAclRuleExtraOutputTypeDef",
+    "AwsWafWebAclRuleOutputTypeDef",
     "AwsWafWebAclRuleTypeDef",
-    "AwsWafv2CustomRequestHandlingDetailsPaginatorTypeDef",
+    "AwsWafv2CustomRequestHandlingDetailsExtraOutputTypeDef",
+    "AwsWafv2CustomRequestHandlingDetailsOutputTypeDef",
     "AwsWafv2CustomRequestHandlingDetailsTypeDef",
-    "AwsWafv2CustomResponseDetailsPaginatorTypeDef",
+    "AwsWafv2CustomResponseDetailsExtraOutputTypeDef",
+    "AwsWafv2CustomResponseDetailsOutputTypeDef",
     "AwsWafv2CustomResponseDetailsTypeDef",
     "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
     "CreateActionTargetResponseTypeDef",
     "CreateAutomationRuleResponseTypeDef",
     "CreateFindingAggregatorResponseTypeDef",
     "CreateInsightResponseTypeDef",
     "DeleteActionTargetResponseTypeDef",
@@ -775,25 +877,28 @@
     "BatchEnableStandardsRequestRequestTypeDef",
     "ListConfigurationPolicyAssociationsResponseTypeDef",
     "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
     "UnprocessedStandardsControlAssociationTypeDef",
     "BatchImportFindingsResponseTypeDef",
     "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
     "UnprocessedStandardsControlAssociationUpdateTypeDef",
-    "VulnerabilityCodeVulnerabilitiesPaginatorTypeDef",
+    "VulnerabilityCodeVulnerabilitiesExtraOutputTypeDef",
+    "VulnerabilityCodeVulnerabilitiesOutputTypeDef",
     "VulnerabilityCodeVulnerabilitiesTypeDef",
-    "CompliancePaginatorTypeDef",
+    "ComplianceExtraOutputTypeDef",
+    "ComplianceOutputTypeDef",
     "ComplianceTypeDef",
     "ConfigurationOptionsTypeDef",
     "ConfigurationPolicyAssociationTypeDef",
     "GetConfigurationPolicyAssociationRequestRequestTypeDef",
     "StartConfigurationPolicyAssociationRequestRequestTypeDef",
     "StartConfigurationPolicyDisassociationRequestRequestTypeDef",
     "ListConfigurationPoliciesResponseTypeDef",
-    "ContainerDetailsPaginatorTypeDef",
+    "ContainerDetailsExtraOutputTypeDef",
+    "ContainerDetailsOutputTypeDef",
     "ContainerDetailsTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
     "DateFilterTypeDef",
@@ -812,302 +917,423 @@
     "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
     "ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
     "DescribeOrganizationConfigurationResponseTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "DescribeProductsResponseTypeDef",
     "DescribeStandardsControlsResponseTypeDef",
-    "ThreatPaginatorTypeDef",
+    "ThreatExtraOutputTypeDef",
+    "ThreatOutputTypeDef",
     "ThreatTypeDef",
     "ListFindingAggregatorsResponseTypeDef",
     "FindingHistoryRecordTypeDef",
-    "FindingProviderFieldsPaginatorTypeDef",
+    "FindingProviderFieldsExtraOutputTypeDef",
+    "FindingProviderFieldsOutputTypeDef",
     "FindingProviderFieldsTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
     "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
     "GetFindingHistoryRequestRequestTypeDef",
     "GetMembersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "InsightResultsTypeDef",
     "ListStandardsControlAssociationsResponseTypeDef",
-    "NetworkPathComponentDetailsPaginatorTypeDef",
+    "NetworkPathComponentDetailsExtraOutputTypeDef",
+    "NetworkPathComponentDetailsOutputTypeDef",
     "NetworkPathComponentDetailsTypeDef",
     "NetworkTypeDef",
     "PageTypeDef",
+    "ParameterConfigurationOutputTypeDef",
     "ParameterConfigurationTypeDef",
     "RemediationTypeDef",
-    "RuleGroupSourceStatefulRulesDetailsPaginatorTypeDef",
+    "RuleGroupSourceStatefulRulesDetailsExtraOutputTypeDef",
+    "RuleGroupSourceStatefulRulesDetailsOutputTypeDef",
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
-    "RuleGroupSourceStatelessRuleMatchAttributesPaginatorTypeDef",
+    "RuleGroupSourceStatelessRuleMatchAttributesExtraOutputTypeDef",
+    "RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
-    "RuleGroupVariablesPaginatorTypeDef",
+    "RuleGroupVariablesExtraOutputTypeDef",
+    "RuleGroupVariablesOutputTypeDef",
     "RuleGroupVariablesTypeDef",
     "StandardTypeDef",
     "StandardsSubscriptionTypeDef",
-    "StatelessCustomPublishMetricActionPaginatorTypeDef",
+    "StatelessCustomPublishMetricActionExtraOutputTypeDef",
+    "StatelessCustomPublishMetricActionOutputTypeDef",
     "StatelessCustomPublishMetricActionTypeDef",
-    "AwsApiCallActionPaginatorTypeDef",
+    "AwsApiCallActionExtraOutputTypeDef",
+    "AwsApiCallActionOutputTypeDef",
     "AwsApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
-    "AwsEc2RouteTableDetailsPaginatorTypeDef",
+    "AwsEc2RouteTableDetailsExtraOutputTypeDef",
+    "AwsEc2RouteTableDetailsOutputTypeDef",
     "AwsEc2RouteTableDetailsTypeDef",
+    "AutomationRulesActionOutputTypeDef",
     "AutomationRulesActionTypeDef",
-    "AwsAmazonMqBrokerDetailsPaginatorTypeDef",
+    "AwsAmazonMqBrokerDetailsExtraOutputTypeDef",
+    "AwsAmazonMqBrokerDetailsOutputTypeDef",
     "AwsAmazonMqBrokerDetailsTypeDef",
-    "AwsAppSyncGraphQlApiDetailsPaginatorTypeDef",
+    "AwsAppSyncGraphQlApiDetailsExtraOutputTypeDef",
+    "AwsAppSyncGraphQlApiDetailsOutputTypeDef",
     "AwsAppSyncGraphQlApiDetailsTypeDef",
     "AwsAthenaWorkGroupConfigurationDetailsTypeDef",
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsPaginatorTypeDef",
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsExtraOutputTypeDef",
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
-    "AwsAutoScalingLaunchConfigurationDetailsPaginatorTypeDef",
+    "AwsAutoScalingLaunchConfigurationDetailsExtraOutputTypeDef",
+    "AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef",
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
-    "AwsBackupBackupPlanRuleDetailsPaginatorTypeDef",
+    "AwsBackupBackupPlanRuleDetailsExtraOutputTypeDef",
+    "AwsBackupBackupPlanRuleDetailsOutputTypeDef",
     "AwsBackupBackupPlanRuleDetailsTypeDef",
-    "AwsCertificateManagerCertificateRenewalSummaryPaginatorTypeDef",
+    "AwsCertificateManagerCertificateRenewalSummaryExtraOutputTypeDef",
+    "AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef",
     "AwsCertificateManagerCertificateRenewalSummaryTypeDef",
-    "AwsCloudFrontDistributionOriginItemPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginItemExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginItemOutputTypeDef",
     "AwsCloudFrontDistributionOriginItemTypeDef",
-    "AwsCloudFrontDistributionOriginGroupPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginGroupExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginGroupOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupTypeDef",
-    "AwsCodeBuildProjectDetailsPaginatorTypeDef",
+    "AwsCodeBuildProjectDetailsExtraOutputTypeDef",
+    "AwsCodeBuildProjectDetailsOutputTypeDef",
     "AwsCodeBuildProjectDetailsTypeDef",
-    "AwsDynamoDbTableReplicaPaginatorTypeDef",
+    "AwsDynamoDbTableReplicaExtraOutputTypeDef",
+    "AwsDynamoDbTableReplicaOutputTypeDef",
     "AwsDynamoDbTableReplicaTypeDef",
-    "AwsEc2ClientVpnEndpointDetailsPaginatorTypeDef",
+    "AwsEc2ClientVpnEndpointDetailsExtraOutputTypeDef",
+    "AwsEc2ClientVpnEndpointDetailsOutputTypeDef",
     "AwsEc2ClientVpnEndpointDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataDetailsPaginatorTypeDef",
+    "AwsEc2LaunchTemplateDataDetailsExtraOutputTypeDef",
+    "AwsEc2LaunchTemplateDataDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataDetailsTypeDef",
-    "AwsEc2NetworkAclDetailsPaginatorTypeDef",
+    "AwsEc2NetworkAclDetailsExtraOutputTypeDef",
+    "AwsEc2NetworkAclDetailsOutputTypeDef",
     "AwsEc2NetworkAclDetailsTypeDef",
-    "AwsEc2SecurityGroupDetailsPaginatorTypeDef",
+    "AwsEc2SecurityGroupDetailsExtraOutputTypeDef",
+    "AwsEc2SecurityGroupDetailsOutputTypeDef",
     "AwsEc2SecurityGroupDetailsTypeDef",
-    "AwsEc2VpcPeeringConnectionDetailsPaginatorTypeDef",
+    "AwsEc2VpcPeeringConnectionDetailsExtraOutputTypeDef",
+    "AwsEc2VpcPeeringConnectionDetailsOutputTypeDef",
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
-    "AwsEc2VpnConnectionDetailsPaginatorTypeDef",
+    "AwsEc2VpnConnectionDetailsExtraOutputTypeDef",
+    "AwsEc2VpnConnectionDetailsOutputTypeDef",
     "AwsEc2VpnConnectionDetailsTypeDef",
     "AwsEcsClusterConfigurationDetailsTypeDef",
-    "AwsEcsServiceDetailsPaginatorTypeDef",
+    "AwsEcsServiceDetailsExtraOutputTypeDef",
+    "AwsEcsServiceDetailsOutputTypeDef",
     "AwsEcsServiceDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
-    "AwsEcsTaskDefinitionVolumesDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionVolumesDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
-    "AwsEcsTaskDetailsPaginatorTypeDef",
+    "AwsEcsTaskDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDetailsOutputTypeDef",
     "AwsEcsTaskDetailsTypeDef",
-    "AwsEfsAccessPointDetailsPaginatorTypeDef",
+    "AwsEfsAccessPointDetailsExtraOutputTypeDef",
+    "AwsEfsAccessPointDetailsOutputTypeDef",
     "AwsEfsAccessPointDetailsTypeDef",
-    "AwsEksClusterDetailsPaginatorTypeDef",
+    "AwsEksClusterDetailsExtraOutputTypeDef",
+    "AwsEksClusterDetailsOutputTypeDef",
     "AwsEksClusterDetailsTypeDef",
-    "AwsElasticsearchDomainDetailsPaginatorTypeDef",
+    "AwsElasticsearchDomainDetailsExtraOutputTypeDef",
+    "AwsElasticsearchDomainDetailsOutputTypeDef",
     "AwsElasticsearchDomainDetailsTypeDef",
-    "AwsElbLoadBalancerDetailsPaginatorTypeDef",
+    "AwsElbLoadBalancerDetailsExtraOutputTypeDef",
+    "AwsElbLoadBalancerDetailsOutputTypeDef",
     "AwsElbLoadBalancerDetailsTypeDef",
     "AwsEventsEndpointRoutingConfigDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef",
     "AwsIamAccessKeyDetailsTypeDef",
-    "AwsIamRoleDetailsPaginatorTypeDef",
+    "AwsIamRoleDetailsExtraOutputTypeDef",
+    "AwsIamRoleDetailsOutputTypeDef",
     "AwsIamRoleDetailsTypeDef",
-    "AwsLambdaFunctionDetailsPaginatorTypeDef",
+    "AwsLambdaFunctionDetailsExtraOutputTypeDef",
+    "AwsLambdaFunctionDetailsOutputTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
-    "AwsMskClusterClusterInfoClientAuthenticationDetailsPaginatorTypeDef",
+    "AwsMskClusterClusterInfoClientAuthenticationDetailsExtraOutputTypeDef",
+    "AwsMskClusterClusterInfoClientAuthenticationDetailsOutputTypeDef",
     "AwsMskClusterClusterInfoClientAuthenticationDetailsTypeDef",
-    "AwsOpenSearchServiceDomainDetailsPaginatorTypeDef",
+    "AwsOpenSearchServiceDomainDetailsExtraOutputTypeDef",
+    "AwsOpenSearchServiceDomainDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainDetailsTypeDef",
-    "AwsRdsDbSubnetGroupPaginatorTypeDef",
+    "AwsRdsDbSubnetGroupExtraOutputTypeDef",
+    "AwsRdsDbSubnetGroupOutputTypeDef",
     "AwsRdsDbSubnetGroupTypeDef",
-    "AwsRedshiftClusterDetailsPaginatorTypeDef",
+    "AwsRedshiftClusterDetailsExtraOutputTypeDef",
+    "AwsRedshiftClusterDetailsOutputTypeDef",
     "AwsRedshiftClusterDetailsTypeDef",
-    "AwsRoute53HostedZoneDetailsPaginatorTypeDef",
+    "AwsRoute53HostedZoneDetailsExtraOutputTypeDef",
+    "AwsRoute53HostedZoneDetailsOutputTypeDef",
     "AwsRoute53HostedZoneDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsPaginatorTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsExtraOutputTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef",
-    "AwsS3BucketNotificationConfigurationFilterPaginatorTypeDef",
+    "AwsS3BucketNotificationConfigurationFilterExtraOutputTypeDef",
+    "AwsS3BucketNotificationConfigurationFilterOutputTypeDef",
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
     "AwsS3BucketObjectLockConfigurationTypeDef",
-    "AwsS3BucketServerSideEncryptionConfigurationPaginatorTypeDef",
+    "AwsS3BucketServerSideEncryptionConfigurationExtraOutputTypeDef",
+    "AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef",
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
-    "AwsS3BucketWebsiteConfigurationPaginatorTypeDef",
+    "AwsS3BucketWebsiteConfigurationExtraOutputTypeDef",
+    "AwsS3BucketWebsiteConfigurationOutputTypeDef",
     "AwsS3BucketWebsiteConfigurationTypeDef",
     "BatchUpdateFindingsResponseTypeDef",
     "AwsSsmPatchComplianceDetailsTypeDef",
-    "AwsStepFunctionStateMachineLoggingConfigurationDetailsPaginatorTypeDef",
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsExtraOutputTypeDef",
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef",
-    "AwsWafRegionalRuleGroupDetailsPaginatorTypeDef",
+    "AwsWafRegionalRuleGroupDetailsExtraOutputTypeDef",
+    "AwsWafRegionalRuleGroupDetailsOutputTypeDef",
     "AwsWafRegionalRuleGroupDetailsTypeDef",
-    "AwsWafRegionalWebAclDetailsPaginatorTypeDef",
+    "AwsWafRegionalWebAclDetailsExtraOutputTypeDef",
+    "AwsWafRegionalWebAclDetailsOutputTypeDef",
     "AwsWafRegionalWebAclDetailsTypeDef",
-    "AwsWafRuleGroupDetailsPaginatorTypeDef",
+    "AwsWafRuleGroupDetailsExtraOutputTypeDef",
+    "AwsWafRuleGroupDetailsOutputTypeDef",
     "AwsWafRuleGroupDetailsTypeDef",
-    "AwsWafWebAclDetailsPaginatorTypeDef",
+    "AwsWafWebAclDetailsExtraOutputTypeDef",
+    "AwsWafWebAclDetailsOutputTypeDef",
     "AwsWafWebAclDetailsTypeDef",
-    "AwsWafv2ActionAllowDetailsPaginatorTypeDef",
-    "AwsWafv2RulesActionCaptchaDetailsPaginatorTypeDef",
-    "AwsWafv2RulesActionCountDetailsPaginatorTypeDef",
+    "AwsWafv2ActionAllowDetailsExtraOutputTypeDef",
+    "AwsWafv2RulesActionCaptchaDetailsExtraOutputTypeDef",
+    "AwsWafv2RulesActionCountDetailsExtraOutputTypeDef",
+    "AwsWafv2ActionAllowDetailsOutputTypeDef",
+    "AwsWafv2RulesActionCaptchaDetailsOutputTypeDef",
+    "AwsWafv2RulesActionCountDetailsOutputTypeDef",
     "AwsWafv2ActionAllowDetailsTypeDef",
     "AwsWafv2RulesActionCaptchaDetailsTypeDef",
     "AwsWafv2RulesActionCountDetailsTypeDef",
-    "AwsWafv2ActionBlockDetailsPaginatorTypeDef",
+    "AwsWafv2ActionBlockDetailsExtraOutputTypeDef",
+    "AwsWafv2ActionBlockDetailsOutputTypeDef",
     "AwsWafv2ActionBlockDetailsTypeDef",
     "BatchGetStandardsControlAssociationsResponseTypeDef",
     "BatchUpdateStandardsControlAssociationsResponseTypeDef",
-    "VulnerabilityPaginatorTypeDef",
+    "VulnerabilityExtraOutputTypeDef",
+    "VulnerabilityOutputTypeDef",
     "VulnerabilityTypeDef",
     "ParameterDefinitionTypeDef",
     "BatchGetConfigurationPolicyAssociationsRequestRequestTypeDef",
     "UnprocessedConfigurationPolicyAssociationTypeDef",
+    "AutomationRulesFindingFiltersOutputTypeDef",
     "AutomationRulesFindingFiltersTypeDef",
+    "AwsSecurityFindingFiltersExtraOutputTypeDef",
+    "AwsSecurityFindingFiltersOutputTypeDef",
     "AwsSecurityFindingFiltersTypeDef",
     "GetFindingHistoryResponseTypeDef",
     "GetInsightResultsResponseTypeDef",
-    "NetworkHeaderPaginatorTypeDef",
+    "NetworkHeaderExtraOutputTypeDef",
+    "NetworkHeaderOutputTypeDef",
     "NetworkHeaderTypeDef",
-    "OccurrencesPaginatorTypeDef",
+    "OccurrencesExtraOutputTypeDef",
+    "OccurrencesOutputTypeDef",
     "OccurrencesTypeDef",
-    "SecurityControlCustomParameterTypeDef",
+    "SecurityControlCustomParameterOutputTypeDef",
     "SecurityControlTypeDef",
-    "UpdateSecurityControlRequestRequestTypeDef",
-    "RuleGroupSourceStatelessRuleDefinitionPaginatorTypeDef",
+    "ParameterConfigurationUnionTypeDef",
+    "SecurityControlCustomParameterTypeDef",
+    "RuleGroupSourceStatelessRuleDefinitionExtraOutputTypeDef",
+    "RuleGroupSourceStatelessRuleDefinitionOutputTypeDef",
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
     "DescribeStandardsResponseTypeDef",
     "BatchDisableStandardsResponseTypeDef",
     "BatchEnableStandardsResponseTypeDef",
     "GetEnabledStandardsResponseTypeDef",
-    "StatelessCustomActionDefinitionPaginatorTypeDef",
+    "StatelessCustomActionDefinitionExtraOutputTypeDef",
+    "StatelessCustomActionDefinitionOutputTypeDef",
     "StatelessCustomActionDefinitionTypeDef",
-    "PortProbeActionPaginatorTypeDef",
+    "PortProbeActionExtraOutputTypeDef",
+    "PortProbeActionOutputTypeDef",
     "PortProbeActionTypeDef",
+    "AutomationRulesActionUnionTypeDef",
     "AwsAthenaWorkGroupDetailsTypeDef",
-    "AwsAutoScalingAutoScalingGroupDetailsPaginatorTypeDef",
+    "AwsAutoScalingAutoScalingGroupDetailsExtraOutputTypeDef",
+    "AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
-    "AwsBackupBackupPlanBackupPlanDetailsPaginatorTypeDef",
+    "AwsBackupBackupPlanBackupPlanDetailsExtraOutputTypeDef",
+    "AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
-    "AwsCertificateManagerCertificateDetailsPaginatorTypeDef",
+    "AwsCertificateManagerCertificateDetailsExtraOutputTypeDef",
+    "AwsCertificateManagerCertificateDetailsOutputTypeDef",
     "AwsCertificateManagerCertificateDetailsTypeDef",
-    "AwsCloudFrontDistributionOriginsPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginsExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginsOutputTypeDef",
     "AwsCloudFrontDistributionOriginsTypeDef",
-    "AwsCloudFrontDistributionOriginGroupsPaginatorTypeDef",
+    "AwsCloudFrontDistributionOriginGroupsExtraOutputTypeDef",
+    "AwsCloudFrontDistributionOriginGroupsOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupsTypeDef",
-    "AwsDynamoDbTableDetailsPaginatorTypeDef",
+    "AwsDynamoDbTableDetailsExtraOutputTypeDef",
+    "AwsDynamoDbTableDetailsOutputTypeDef",
     "AwsDynamoDbTableDetailsTypeDef",
-    "AwsEc2LaunchTemplateDetailsPaginatorTypeDef",
+    "AwsEc2LaunchTemplateDetailsExtraOutputTypeDef",
+    "AwsEc2LaunchTemplateDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDetailsTypeDef",
-    "AwsEcsClusterDetailsPaginatorTypeDef",
+    "AwsEcsClusterDetailsExtraOutputTypeDef",
+    "AwsEcsClusterDetailsOutputTypeDef",
     "AwsEcsClusterDetailsTypeDef",
-    "AwsEcsTaskDefinitionDetailsPaginatorTypeDef",
+    "AwsEcsTaskDefinitionDetailsExtraOutputTypeDef",
+    "AwsEcsTaskDefinitionDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionDetailsTypeDef",
-    "AwsEventsEndpointDetailsPaginatorTypeDef",
+    "AwsEventsEndpointDetailsExtraOutputTypeDef",
+    "AwsEventsEndpointDetailsOutputTypeDef",
     "AwsEventsEndpointDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesDetailsTypeDef",
-    "AwsMskClusterClusterInfoDetailsPaginatorTypeDef",
+    "AwsMskClusterClusterInfoDetailsExtraOutputTypeDef",
+    "AwsMskClusterClusterInfoDetailsOutputTypeDef",
     "AwsMskClusterClusterInfoDetailsTypeDef",
-    "AwsRdsDbInstanceDetailsPaginatorTypeDef",
+    "AwsRdsDbInstanceDetailsExtraOutputTypeDef",
+    "AwsRdsDbInstanceDetailsOutputTypeDef",
     "AwsRdsDbInstanceDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsPaginatorTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsExtraOutputTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
-    "AwsS3BucketNotificationConfigurationDetailPaginatorTypeDef",
+    "AwsS3BucketNotificationConfigurationDetailExtraOutputTypeDef",
+    "AwsS3BucketNotificationConfigurationDetailOutputTypeDef",
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
-    "AwsStepFunctionStateMachineDetailsPaginatorTypeDef",
+    "AwsStepFunctionStateMachineDetailsExtraOutputTypeDef",
+    "AwsStepFunctionStateMachineDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineDetailsTypeDef",
-    "AwsWafv2RulesActionDetailsPaginatorTypeDef",
-    "AwsWafv2WebAclActionDetailsPaginatorTypeDef",
+    "AwsWafv2RulesActionDetailsExtraOutputTypeDef",
+    "AwsWafv2WebAclActionDetailsExtraOutputTypeDef",
+    "AwsWafv2RulesActionDetailsOutputTypeDef",
+    "AwsWafv2WebAclActionDetailsOutputTypeDef",
     "AwsWafv2RulesActionDetailsTypeDef",
     "AwsWafv2WebAclActionDetailsTypeDef",
     "SecurityControlDefinitionTypeDef",
     "BatchGetConfigurationPolicyAssociationsResponseTypeDef",
     "AutomationRulesConfigTypeDef",
-    "CreateAutomationRuleRequestRequestTypeDef",
+    "AutomationRulesFindingFiltersUnionTypeDef",
     "UpdateAutomationRulesRequestItemTypeDef",
+    "InsightTypeDef",
+    "AwsSecurityFindingFiltersUnionTypeDef",
     "CreateInsightRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
-    "InsightTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "UpdateInsightRequestRequestTypeDef",
-    "NetworkPathComponentPaginatorTypeDef",
+    "NetworkPathComponentExtraOutputTypeDef",
+    "NetworkPathComponentOutputTypeDef",
     "NetworkPathComponentTypeDef",
-    "CustomDataIdentifiersDetectionsPaginatorTypeDef",
-    "SensitiveDataDetectionsPaginatorTypeDef",
+    "CustomDataIdentifiersDetectionsExtraOutputTypeDef",
+    "SensitiveDataDetectionsExtraOutputTypeDef",
+    "CustomDataIdentifiersDetectionsOutputTypeDef",
+    "SensitiveDataDetectionsOutputTypeDef",
     "CustomDataIdentifiersDetectionsTypeDef",
     "SensitiveDataDetectionsTypeDef",
-    "SecurityControlsConfigurationTypeDef",
+    "SecurityControlsConfigurationOutputTypeDef",
     "BatchGetSecurityControlsResponseTypeDef",
-    "RuleGroupSourceStatelessRulesDetailsPaginatorTypeDef",
+    "UpdateSecurityControlRequestRequestTypeDef",
+    "SecurityControlsConfigurationTypeDef",
+    "RuleGroupSourceStatelessRulesDetailsExtraOutputTypeDef",
+    "RuleGroupSourceStatelessRulesDetailsOutputTypeDef",
     "RuleGroupSourceStatelessRulesDetailsTypeDef",
-    "FirewallPolicyStatelessCustomActionsDetailsPaginatorTypeDef",
-    "RuleGroupSourceCustomActionsDetailsPaginatorTypeDef",
+    "FirewallPolicyStatelessCustomActionsDetailsExtraOutputTypeDef",
+    "RuleGroupSourceCustomActionsDetailsExtraOutputTypeDef",
+    "FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef",
+    "RuleGroupSourceCustomActionsDetailsOutputTypeDef",
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     "RuleGroupSourceCustomActionsDetailsTypeDef",
-    "ActionPaginatorTypeDef",
+    "ActionExtraOutputTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
-    "AwsBackupBackupPlanDetailsPaginatorTypeDef",
+    "CreateAutomationRuleRequestRequestTypeDef",
+    "AwsBackupBackupPlanDetailsExtraOutputTypeDef",
+    "AwsBackupBackupPlanDetailsOutputTypeDef",
     "AwsBackupBackupPlanDetailsTypeDef",
-    "AwsCloudFrontDistributionDetailsPaginatorTypeDef",
+    "AwsCloudFrontDistributionDetailsExtraOutputTypeDef",
+    "AwsCloudFrontDistributionDetailsOutputTypeDef",
     "AwsCloudFrontDistributionDetailsTypeDef",
-    "AwsGuardDutyDetectorDetailsPaginatorTypeDef",
+    "AwsGuardDutyDetectorDetailsExtraOutputTypeDef",
+    "AwsGuardDutyDetectorDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDetailsTypeDef",
-    "AwsMskClusterDetailsPaginatorTypeDef",
+    "AwsMskClusterDetailsExtraOutputTypeDef",
+    "AwsMskClusterDetailsOutputTypeDef",
     "AwsMskClusterDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsPaginatorTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsExtraOutputTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
-    "AwsS3BucketNotificationConfigurationPaginatorTypeDef",
+    "AwsS3BucketNotificationConfigurationExtraOutputTypeDef",
+    "AwsS3BucketNotificationConfigurationOutputTypeDef",
     "AwsS3BucketNotificationConfigurationTypeDef",
-    "AwsWafv2RulesDetailsPaginatorTypeDef",
+    "AwsWafv2RulesDetailsExtraOutputTypeDef",
+    "AwsWafv2RulesDetailsOutputTypeDef",
     "AwsWafv2RulesDetailsTypeDef",
     "GetSecurityControlDefinitionResponseTypeDef",
     "ListSecurityControlDefinitionsResponseTypeDef",
     "BatchGetAutomationRulesResponseTypeDef",
     "BatchUpdateAutomationRulesRequestRequestTypeDef",
     "GetInsightsResponseTypeDef",
-    "CustomDataIdentifiersResultPaginatorTypeDef",
-    "SensitiveDataResultPaginatorTypeDef",
+    "CustomDataIdentifiersResultExtraOutputTypeDef",
+    "SensitiveDataResultExtraOutputTypeDef",
+    "CustomDataIdentifiersResultOutputTypeDef",
+    "SensitiveDataResultOutputTypeDef",
     "CustomDataIdentifiersResultTypeDef",
     "SensitiveDataResultTypeDef",
+    "SecurityHubPolicyOutputTypeDef",
     "SecurityHubPolicyTypeDef",
-    "FirewallPolicyDetailsPaginatorTypeDef",
-    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsPaginatorTypeDef",
+    "FirewallPolicyDetailsExtraOutputTypeDef",
+    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsExtraOutputTypeDef",
+    "FirewallPolicyDetailsOutputTypeDef",
+    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef",
     "FirewallPolicyDetailsTypeDef",
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationDetailsPaginatorTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationDetailsExtraOutputTypeDef",
+    "AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
-    "AwsWafv2RuleGroupDetailsPaginatorTypeDef",
-    "AwsWafv2WebAclDetailsPaginatorTypeDef",
+    "AwsWafv2RuleGroupDetailsExtraOutputTypeDef",
+    "AwsWafv2WebAclDetailsExtraOutputTypeDef",
+    "AwsWafv2RuleGroupDetailsOutputTypeDef",
+    "AwsWafv2WebAclDetailsOutputTypeDef",
     "AwsWafv2RuleGroupDetailsTypeDef",
     "AwsWafv2WebAclDetailsTypeDef",
-    "ClassificationResultPaginatorTypeDef",
+    "ClassificationResultExtraOutputTypeDef",
+    "ClassificationResultOutputTypeDef",
     "ClassificationResultTypeDef",
+    "PolicyOutputTypeDef",
     "PolicyTypeDef",
-    "AwsNetworkFirewallFirewallPolicyDetailsPaginatorTypeDef",
-    "RuleGroupSourcePaginatorTypeDef",
+    "AwsNetworkFirewallFirewallPolicyDetailsExtraOutputTypeDef",
+    "RuleGroupSourceExtraOutputTypeDef",
+    "AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef",
+    "RuleGroupSourceOutputTypeDef",
     "AwsNetworkFirewallFirewallPolicyDetailsTypeDef",
     "RuleGroupSourceTypeDef",
-    "AwsS3BucketDetailsPaginatorTypeDef",
+    "AwsS3BucketDetailsExtraOutputTypeDef",
+    "AwsS3BucketDetailsOutputTypeDef",
     "AwsS3BucketDetailsTypeDef",
-    "DataClassificationDetailsPaginatorTypeDef",
+    "DataClassificationDetailsExtraOutputTypeDef",
+    "DataClassificationDetailsOutputTypeDef",
     "DataClassificationDetailsTypeDef",
-    "CreateConfigurationPolicyRequestRequestTypeDef",
     "CreateConfigurationPolicyResponseTypeDef",
     "GetConfigurationPolicyResponseTypeDef",
-    "UpdateConfigurationPolicyRequestRequestTypeDef",
     "UpdateConfigurationPolicyResponseTypeDef",
-    "RuleGroupDetailsPaginatorTypeDef",
+    "CreateConfigurationPolicyRequestRequestTypeDef",
+    "PolicyUnionTypeDef",
+    "UpdateConfigurationPolicyRequestRequestTypeDef",
+    "RuleGroupDetailsExtraOutputTypeDef",
+    "RuleGroupDetailsOutputTypeDef",
     "RuleGroupDetailsTypeDef",
-    "AwsNetworkFirewallRuleGroupDetailsPaginatorTypeDef",
+    "AwsNetworkFirewallRuleGroupDetailsExtraOutputTypeDef",
+    "AwsNetworkFirewallRuleGroupDetailsOutputTypeDef",
     "AwsNetworkFirewallRuleGroupDetailsTypeDef",
-    "ResourceDetailsPaginatorTypeDef",
+    "ResourceDetailsExtraOutputTypeDef",
+    "ResourceDetailsOutputTypeDef",
     "ResourceDetailsTypeDef",
-    "ResourcePaginatorTypeDef",
+    "ResourceExtraOutputTypeDef",
+    "ResourceOutputTypeDef",
     "ResourceTypeDef",
-    "AwsSecurityFindingPaginatorTypeDef",
+    "AwsSecurityFindingExtraOutputTypeDef",
+    "AwsSecurityFindingOutputTypeDef",
     "AwsSecurityFindingTypeDef",
-    "GetFindingsResponsePaginatorTypeDef",
-    "BatchImportFindingsRequestRequestTypeDef",
     "GetFindingsResponseTypeDef",
+    "AwsSecurityFindingUnionTypeDef",
+    "BatchImportFindingsRequestRequestTypeDef",
 )
 
 AcceptAdministratorInvitationRequestRequestTypeDef = TypedDict(
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     {
         "AdministratorId": str,
         "InvitationId": str,
@@ -1123,35 +1349,35 @@
 AccountDetailsTypeDef = TypedDict(
     "AccountDetailsTypeDef",
     {
         "AccountId": str,
         "Email": NotRequired[str],
     },
 )
+DnsRequestActionTypeDef = TypedDict(
+    "DnsRequestActionTypeDef",
+    {
+        "Domain": NotRequired[str],
+        "Protocol": NotRequired[str],
+        "Blocked": NotRequired[bool],
+    },
+)
 ActionLocalIpDetailsTypeDef = TypedDict(
     "ActionLocalIpDetailsTypeDef",
     {
         "IpAddressV4": NotRequired[str],
     },
 )
 ActionLocalPortDetailsTypeDef = TypedDict(
     "ActionLocalPortDetailsTypeDef",
     {
         "Port": NotRequired[int],
         "PortName": NotRequired[str],
     },
 )
-DnsRequestActionTypeDef = TypedDict(
-    "DnsRequestActionTypeDef",
-    {
-        "Domain": NotRequired[str],
-        "Protocol": NotRequired[str],
-        "Blocked": NotRequired[bool],
-    },
-)
 CityTypeDef = TypedDict(
     "CityTypeDef",
     {
         "CityName": NotRequired[str],
     },
 )
 CountryTypeDef = TypedDict(
@@ -1304,16 +1530,16 @@
 AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
     {
         "KmsKeyId": NotRequired[str],
         "UseAwsOwnedKey": NotRequired[bool],
     },
 )
-AwsAmazonMqBrokerLdapServerMetadataDetailsPaginatorTypeDef = TypedDict(
-    "AwsAmazonMqBrokerLdapServerMetadataDetailsPaginatorTypeDef",
+AwsAmazonMqBrokerLdapServerMetadataDetailsExtraOutputTypeDef = TypedDict(
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsExtraOutputTypeDef",
     {
         "Hosts": NotRequired[List[str]],
         "RoleBase": NotRequired[str],
         "RoleName": NotRequired[str],
         "RoleSearchMatching": NotRequired[str],
         "RoleSearchSubtree": NotRequired[bool],
         "ServiceAccountUsername": NotRequired[str],
@@ -1334,14 +1560,29 @@
 AwsAmazonMqBrokerUsersDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerUsersDetailsTypeDef",
     {
         "PendingChange": NotRequired[str],
         "Username": NotRequired[str],
     },
 )
+AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef = TypedDict(
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef",
+    {
+        "Hosts": NotRequired[List[str]],
+        "RoleBase": NotRequired[str],
+        "RoleName": NotRequired[str],
+        "RoleSearchMatching": NotRequired[str],
+        "RoleSearchSubtree": NotRequired[bool],
+        "ServiceAccountUsername": NotRequired[str],
+        "UserBase": NotRequired[str],
+        "UserRoleName": NotRequired[str],
+        "UserSearchMatching": NotRequired[str],
+        "UserSearchSubtree": NotRequired[bool],
+    },
+)
 AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
     {
         "Hosts": NotRequired[Sequence[str]],
         "RoleBase": NotRequired[str],
         "RoleName": NotRequired[str],
         "RoleSearchMatching": NotRequired[str],
@@ -1369,16 +1610,25 @@
 AwsApiGatewayAccessLogSettingsTypeDef = TypedDict(
     "AwsApiGatewayAccessLogSettingsTypeDef",
     {
         "Format": NotRequired[str],
         "DestinationArn": NotRequired[str],
     },
 )
-AwsApiGatewayCanarySettingsPaginatorTypeDef = TypedDict(
-    "AwsApiGatewayCanarySettingsPaginatorTypeDef",
+AwsApiGatewayCanarySettingsExtraOutputTypeDef = TypedDict(
+    "AwsApiGatewayCanarySettingsExtraOutputTypeDef",
+    {
+        "PercentTraffic": NotRequired[float],
+        "DeploymentId": NotRequired[str],
+        "StageVariableOverrides": NotRequired[Dict[str, str]],
+        "UseStageCache": NotRequired[bool],
+    },
+)
+AwsApiGatewayCanarySettingsOutputTypeDef = TypedDict(
+    "AwsApiGatewayCanarySettingsOutputTypeDef",
     {
         "PercentTraffic": NotRequired[float],
         "DeploymentId": NotRequired[str],
         "StageVariableOverrides": NotRequired[Dict[str, str]],
         "UseStageCache": NotRequired[bool],
     },
 )
@@ -1387,16 +1637,22 @@
     {
         "PercentTraffic": NotRequired[float],
         "DeploymentId": NotRequired[str],
         "StageVariableOverrides": NotRequired[Mapping[str, str]],
         "UseStageCache": NotRequired[bool],
     },
 )
-AwsApiGatewayEndpointConfigurationPaginatorTypeDef = TypedDict(
-    "AwsApiGatewayEndpointConfigurationPaginatorTypeDef",
+AwsApiGatewayEndpointConfigurationExtraOutputTypeDef = TypedDict(
+    "AwsApiGatewayEndpointConfigurationExtraOutputTypeDef",
+    {
+        "Types": NotRequired[List[str]],
+    },
+)
+AwsApiGatewayEndpointConfigurationOutputTypeDef = TypedDict(
+    "AwsApiGatewayEndpointConfigurationOutputTypeDef",
     {
         "Types": NotRequired[List[str]],
     },
 )
 AwsApiGatewayEndpointConfigurationTypeDef = TypedDict(
     "AwsApiGatewayEndpointConfigurationTypeDef",
     {
@@ -1416,16 +1672,27 @@
         "CacheDataEncrypted": NotRequired[bool],
         "RequireAuthorizationForCacheControl": NotRequired[bool],
         "UnauthorizedCacheControlHeaderStrategy": NotRequired[str],
         "HttpMethod": NotRequired[str],
         "ResourcePath": NotRequired[str],
     },
 )
-AwsCorsConfigurationPaginatorTypeDef = TypedDict(
-    "AwsCorsConfigurationPaginatorTypeDef",
+AwsCorsConfigurationExtraOutputTypeDef = TypedDict(
+    "AwsCorsConfigurationExtraOutputTypeDef",
+    {
+        "AllowOrigins": NotRequired[List[str]],
+        "AllowCredentials": NotRequired[bool],
+        "ExposeHeaders": NotRequired[List[str]],
+        "MaxAge": NotRequired[int],
+        "AllowMethods": NotRequired[List[str]],
+        "AllowHeaders": NotRequired[List[str]],
+    },
+)
+AwsCorsConfigurationOutputTypeDef = TypedDict(
+    "AwsCorsConfigurationOutputTypeDef",
     {
         "AllowOrigins": NotRequired[List[str]],
         "AllowCredentials": NotRequired[bool],
         "ExposeHeaders": NotRequired[List[str]],
         "MaxAge": NotRequired[int],
         "AllowMethods": NotRequired[List[str]],
         "AllowHeaders": NotRequired[List[str]],
@@ -1554,16 +1821,23 @@
     "AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef",
     {
         "HttpEndpoint": NotRequired[str],
         "HttpPutResponseHopLimit": NotRequired[int],
         "HttpTokens": NotRequired[str],
     },
 )
-AwsBackupBackupPlanAdvancedBackupSettingsDetailsPaginatorTypeDef = TypedDict(
-    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsPaginatorTypeDef",
+AwsBackupBackupPlanAdvancedBackupSettingsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsExtraOutputTypeDef",
+    {
+        "BackupOptions": NotRequired[Dict[str, str]],
+        "ResourceType": NotRequired[str],
+    },
+)
+AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef",
     {
         "BackupOptions": NotRequired[Dict[str, str]],
         "ResourceType": NotRequired[str],
     },
 )
 AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef",
@@ -1575,16 +1849,23 @@
 AwsBackupBackupPlanLifecycleDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanLifecycleDetailsTypeDef",
     {
         "DeleteAfterDays": NotRequired[int],
         "MoveToColdStorageAfterDays": NotRequired[int],
     },
 )
-AwsBackupBackupVaultNotificationsDetailsPaginatorTypeDef = TypedDict(
-    "AwsBackupBackupVaultNotificationsDetailsPaginatorTypeDef",
+AwsBackupBackupVaultNotificationsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsBackupBackupVaultNotificationsDetailsExtraOutputTypeDef",
+    {
+        "BackupVaultEvents": NotRequired[List[str]],
+        "SnsTopicArn": NotRequired[str],
+    },
+)
+AwsBackupBackupVaultNotificationsDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupVaultNotificationsDetailsOutputTypeDef",
     {
         "BackupVaultEvents": NotRequired[List[str]],
         "SnsTopicArn": NotRequired[str],
     },
 )
 AwsBackupBackupVaultNotificationsDetailsTypeDef = TypedDict(
     "AwsBackupBackupVaultNotificationsDetailsTypeDef",
@@ -1686,30 +1967,44 @@
         "CertificateSource": NotRequired[str],
         "CloudFrontDefaultCertificate": NotRequired[bool],
         "IamCertificateId": NotRequired[str],
         "MinimumProtocolVersion": NotRequired[str],
         "SslSupportMethod": NotRequired[str],
     },
 )
-AwsCloudFrontDistributionOriginSslProtocolsPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginSslProtocolsPaginatorTypeDef",
+AwsCloudFrontDistributionOriginSslProtocolsExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginSslProtocolsExtraOutputTypeDef",
+    {
+        "Items": NotRequired[List[str]],
+        "Quantity": NotRequired[int],
+    },
+)
+AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef",
     {
         "Items": NotRequired[List[str]],
         "Quantity": NotRequired[int],
     },
 )
 AwsCloudFrontDistributionOriginSslProtocolsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginSslProtocolsTypeDef",
     {
         "Items": NotRequired[Sequence[str]],
         "Quantity": NotRequired[int],
     },
 )
-AwsCloudFrontDistributionOriginGroupFailoverStatusCodesPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesPaginatorTypeDef",
+AwsCloudFrontDistributionOriginGroupFailoverStatusCodesExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesExtraOutputTypeDef",
+    {
+        "Items": NotRequired[List[int]],
+        "Quantity": NotRequired[int],
+    },
+)
+AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef",
     {
         "Items": NotRequired[List[int]],
         "Quantity": NotRequired[int],
     },
 )
 AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef",
@@ -1770,16 +2065,24 @@
     {
         "Type": NotRequired[str],
         "Location": NotRequired[str],
         "GitCloneDepth": NotRequired[int],
         "InsecureSsl": NotRequired[bool],
     },
 )
-AwsCodeBuildProjectVpcConfigPaginatorTypeDef = TypedDict(
-    "AwsCodeBuildProjectVpcConfigPaginatorTypeDef",
+AwsCodeBuildProjectVpcConfigExtraOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectVpcConfigExtraOutputTypeDef",
+    {
+        "VpcId": NotRequired[str],
+        "Subnets": NotRequired[List[str]],
+        "SecurityGroupIds": NotRequired[List[str]],
+    },
+)
+AwsCodeBuildProjectVpcConfigOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectVpcConfigOutputTypeDef",
     {
         "VpcId": NotRequired[str],
         "Subnets": NotRequired[List[str]],
         "SecurityGroupIds": NotRequired[List[str]],
     },
 )
 AwsCodeBuildProjectVpcConfigTypeDef = TypedDict(
@@ -1921,16 +2224,23 @@
 AwsDynamoDbTableStreamSpecificationTypeDef = TypedDict(
     "AwsDynamoDbTableStreamSpecificationTypeDef",
     {
         "StreamEnabled": NotRequired[bool],
         "StreamViewType": NotRequired[str],
     },
 )
-AwsDynamoDbTableProjectionPaginatorTypeDef = TypedDict(
-    "AwsDynamoDbTableProjectionPaginatorTypeDef",
+AwsDynamoDbTableProjectionExtraOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableProjectionExtraOutputTypeDef",
+    {
+        "NonKeyAttributes": NotRequired[List[str]],
+        "ProjectionType": NotRequired[str],
+    },
+)
+AwsDynamoDbTableProjectionOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableProjectionOutputTypeDef",
     {
         "NonKeyAttributes": NotRequired[List[str]],
         "ProjectionType": NotRequired[str],
     },
 )
 AwsDynamoDbTableProjectionTypeDef = TypedDict(
     "AwsDynamoDbTableProjectionTypeDef",
@@ -2342,16 +2652,33 @@
     "Ipv6CidrBlockAssociationTypeDef",
     {
         "AssociationId": NotRequired[str],
         "Ipv6CidrBlock": NotRequired[str],
         "CidrBlockState": NotRequired[str],
     },
 )
-AwsEc2TransitGatewayDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2TransitGatewayDetailsPaginatorTypeDef",
+AwsEc2TransitGatewayDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2TransitGatewayDetailsExtraOutputTypeDef",
+    {
+        "Id": NotRequired[str],
+        "Description": NotRequired[str],
+        "DefaultRouteTablePropagation": NotRequired[str],
+        "AutoAcceptSharedAttachments": NotRequired[str],
+        "DefaultRouteTableAssociation": NotRequired[str],
+        "TransitGatewayCidrBlocks": NotRequired[List[str]],
+        "AssociationDefaultRouteTableId": NotRequired[str],
+        "PropagationDefaultRouteTableId": NotRequired[str],
+        "VpnEcmpSupport": NotRequired[str],
+        "DnsSupport": NotRequired[str],
+        "MulticastSupport": NotRequired[str],
+        "AmazonSideAsn": NotRequired[int],
+    },
+)
+AwsEc2TransitGatewayDetailsOutputTypeDef = TypedDict(
+    "AwsEc2TransitGatewayDetailsOutputTypeDef",
     {
         "Id": NotRequired[str],
         "Description": NotRequired[str],
         "DefaultRouteTablePropagation": NotRequired[str],
         "AutoAcceptSharedAttachments": NotRequired[str],
         "DefaultRouteTableAssociation": NotRequired[str],
         "TransitGatewayCidrBlocks": NotRequired[List[str]],
@@ -2444,16 +2771,37 @@
         "CertificateArn": NotRequired[str],
         "LastStatusChange": NotRequired[str],
         "OutsideIpAddress": NotRequired[str],
         "Status": NotRequired[str],
         "StatusMessage": NotRequired[str],
     },
 )
-AwsEc2VpnConnectionOptionsTunnelOptionsDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsPaginatorTypeDef",
+AwsEc2VpnConnectionOptionsTunnelOptionsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsExtraOutputTypeDef",
+    {
+        "DpdTimeoutSeconds": NotRequired[int],
+        "IkeVersions": NotRequired[List[str]],
+        "OutsideIpAddress": NotRequired[str],
+        "Phase1DhGroupNumbers": NotRequired[List[int]],
+        "Phase1EncryptionAlgorithms": NotRequired[List[str]],
+        "Phase1IntegrityAlgorithms": NotRequired[List[str]],
+        "Phase1LifetimeSeconds": NotRequired[int],
+        "Phase2DhGroupNumbers": NotRequired[List[int]],
+        "Phase2EncryptionAlgorithms": NotRequired[List[str]],
+        "Phase2IntegrityAlgorithms": NotRequired[List[str]],
+        "Phase2LifetimeSeconds": NotRequired[int],
+        "PreSharedKey": NotRequired[str],
+        "RekeyFuzzPercentage": NotRequired[int],
+        "RekeyMarginTimeSeconds": NotRequired[int],
+        "ReplayWindowSize": NotRequired[int],
+        "TunnelInsideCidr": NotRequired[str],
+    },
+)
+AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef",
     {
         "DpdTimeoutSeconds": NotRequired[int],
         "IkeVersions": NotRequired[List[str]],
         "OutsideIpAddress": NotRequired[str],
         "Phase1DhGroupNumbers": NotRequired[List[int]],
         "Phase1EncryptionAlgorithms": NotRequired[List[str]],
         "Phase1IntegrityAlgorithms": NotRequired[List[str]],
@@ -2486,16 +2834,27 @@
         "PreSharedKey": NotRequired[str],
         "RekeyFuzzPercentage": NotRequired[int],
         "RekeyMarginTimeSeconds": NotRequired[int],
         "ReplayWindowSize": NotRequired[int],
         "TunnelInsideCidr": NotRequired[str],
     },
 )
-AwsEcrContainerImageDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcrContainerImageDetailsPaginatorTypeDef",
+AwsEcrContainerImageDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcrContainerImageDetailsExtraOutputTypeDef",
+    {
+        "RegistryId": NotRequired[str],
+        "RepositoryName": NotRequired[str],
+        "Architecture": NotRequired[str],
+        "ImageDigest": NotRequired[str],
+        "ImageTags": NotRequired[List[str]],
+        "ImagePublishedAt": NotRequired[str],
+    },
+)
+AwsEcrContainerImageDetailsOutputTypeDef = TypedDict(
+    "AwsEcrContainerImageDetailsOutputTypeDef",
     {
         "RegistryId": NotRequired[str],
         "RepositoryName": NotRequired[str],
         "Architecture": NotRequired[str],
         "ImageDigest": NotRequired[str],
         "ImageTags": NotRequired[List[str]],
         "ImagePublishedAt": NotRequired[str],
@@ -2606,16 +2965,24 @@
     {
         "ContainerName": NotRequired[str],
         "ContainerPort": NotRequired[int],
         "Port": NotRequired[int],
         "RegistryArn": NotRequired[str],
     },
 )
-AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsPaginatorTypeDef",
+AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsExtraOutputTypeDef",
+    {
+        "AssignPublicIp": NotRequired[str],
+        "SecurityGroups": NotRequired[List[str]],
+        "Subnets": NotRequired[List[str]],
+    },
+)
+AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef",
     {
         "AssignPublicIp": NotRequired[str],
         "SecurityGroups": NotRequired[List[str]],
         "Subnets": NotRequired[List[str]],
     },
 )
 AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef = TypedDict(
@@ -2650,23 +3017,23 @@
 AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef",
     {
         "Hostname": NotRequired[str],
         "IpAddress": NotRequired[str],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsExtraOutputTypeDef",
     {
         "Options": NotRequired[Dict[str, str]],
         "Type": NotRequired[str],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsExtraOutputTypeDef",
     {
         "Command": NotRequired[List[str]],
         "Interval": NotRequired[int],
         "Retries": NotRequired[int],
         "StartPeriod": NotRequired[int],
         "Timeout": NotRequired[int],
     },
@@ -2725,14 +3092,31 @@
 AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef",
     {
         "ReadOnly": NotRequired[bool],
         "SourceContainer": NotRequired[str],
     },
 )
+AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef",
+    {
+        "Options": NotRequired[Dict[str, str]],
+        "Type": NotRequired[str],
+    },
+)
+AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef",
+    {
+        "Command": NotRequired[List[str]],
+        "Interval": NotRequired[int],
+        "Retries": NotRequired[int],
+        "StartPeriod": NotRequired[int],
+        "Timeout": NotRequired[int],
+    },
+)
 AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
     {
         "Options": NotRequired[Mapping[str, str]],
         "Type": NotRequired[str],
     },
 )
@@ -2742,38 +3126,61 @@
         "Command": NotRequired[Sequence[str]],
         "Interval": NotRequired[int],
         "Retries": NotRequired[int],
         "StartPeriod": NotRequired[int],
         "Timeout": NotRequired[int],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsExtraOutputTypeDef",
+    {
+        "Add": NotRequired[List[str]],
+        "Drop": NotRequired[List[str]],
+    },
+)
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef",
     {
         "Add": NotRequired[List[str]],
         "Drop": NotRequired[List[str]],
     },
 )
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef",
     {
         "Add": NotRequired[Sequence[str]],
         "Drop": NotRequired[Sequence[str]],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsExtraOutputTypeDef",
+    {
+        "ContainerPath": NotRequired[str],
+        "HostPath": NotRequired[str],
+        "Permissions": NotRequired[List[str]],
+    },
+)
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsExtraOutputTypeDef",
+    {
+        "ContainerPath": NotRequired[str],
+        "MountOptions": NotRequired[List[str]],
+        "Size": NotRequired[int],
+    },
+)
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef",
     {
         "ContainerPath": NotRequired[str],
         "HostPath": NotRequired[str],
         "Permissions": NotRequired[List[str]],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef",
     {
         "ContainerPath": NotRequired[str],
         "MountOptions": NotRequired[List[str]],
         "Size": NotRequired[int],
     },
 )
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef = TypedDict(
@@ -2816,30 +3223,40 @@
 AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef",
     {
         "Name": NotRequired[str],
         "Value": NotRequired[str],
     },
 )
-AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsExtraOutputTypeDef",
     {
         "Autoprovision": NotRequired[bool],
         "Driver": NotRequired[str],
         "DriverOpts": NotRequired[Dict[str, str]],
         "Labels": NotRequired[Dict[str, str]],
         "Scope": NotRequired[str],
     },
 )
 AwsEcsTaskDefinitionVolumesHostDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesHostDetailsTypeDef",
     {
         "SourcePath": NotRequired[str],
     },
 )
+AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef",
+    {
+        "Autoprovision": NotRequired[bool],
+        "Driver": NotRequired[str],
+        "DriverOpts": NotRequired[Dict[str, str]],
+        "Labels": NotRequired[Dict[str, str]],
+        "Scope": NotRequired[str],
+    },
+)
 AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
     {
         "Autoprovision": NotRequired[bool],
         "Driver": NotRequired[str],
         "DriverOpts": NotRequired[Mapping[str, str]],
         "Labels": NotRequired[Mapping[str, str]],
@@ -2855,16 +3272,24 @@
 )
 AwsEcsTaskVolumeHostDetailsTypeDef = TypedDict(
     "AwsEcsTaskVolumeHostDetailsTypeDef",
     {
         "SourcePath": NotRequired[str],
     },
 )
-AwsEfsAccessPointPosixUserDetailsPaginatorTypeDef = TypedDict(
-    "AwsEfsAccessPointPosixUserDetailsPaginatorTypeDef",
+AwsEfsAccessPointPosixUserDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEfsAccessPointPosixUserDetailsExtraOutputTypeDef",
+    {
+        "Gid": NotRequired[str],
+        "SecondaryGids": NotRequired[List[str]],
+        "Uid": NotRequired[str],
+    },
+)
+AwsEfsAccessPointPosixUserDetailsOutputTypeDef = TypedDict(
+    "AwsEfsAccessPointPosixUserDetailsOutputTypeDef",
     {
         "Gid": NotRequired[str],
         "SecondaryGids": NotRequired[List[str]],
         "Uid": NotRequired[str],
     },
 )
 AwsEfsAccessPointPosixUserDetailsTypeDef = TypedDict(
@@ -2879,32 +3304,47 @@
     "AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef",
     {
         "OwnerGid": NotRequired[str],
         "OwnerUid": NotRequired[str],
         "Permissions": NotRequired[str],
     },
 )
-AwsEksClusterResourcesVpcConfigDetailsPaginatorTypeDef = TypedDict(
-    "AwsEksClusterResourcesVpcConfigDetailsPaginatorTypeDef",
+AwsEksClusterResourcesVpcConfigDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEksClusterResourcesVpcConfigDetailsExtraOutputTypeDef",
+    {
+        "SecurityGroupIds": NotRequired[List[str]],
+        "SubnetIds": NotRequired[List[str]],
+        "EndpointPublicAccess": NotRequired[bool],
+    },
+)
+AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef",
     {
         "SecurityGroupIds": NotRequired[List[str]],
         "SubnetIds": NotRequired[List[str]],
         "EndpointPublicAccess": NotRequired[bool],
     },
 )
 AwsEksClusterResourcesVpcConfigDetailsTypeDef = TypedDict(
     "AwsEksClusterResourcesVpcConfigDetailsTypeDef",
     {
         "SecurityGroupIds": NotRequired[Sequence[str]],
         "SubnetIds": NotRequired[Sequence[str]],
         "EndpointPublicAccess": NotRequired[bool],
     },
 )
-AwsEksClusterLoggingClusterLoggingDetailsPaginatorTypeDef = TypedDict(
-    "AwsEksClusterLoggingClusterLoggingDetailsPaginatorTypeDef",
+AwsEksClusterLoggingClusterLoggingDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEksClusterLoggingClusterLoggingDetailsExtraOutputTypeDef",
+    {
+        "Enabled": NotRequired[bool],
+        "Types": NotRequired[List[str]],
+    },
+)
+AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef",
     {
         "Enabled": NotRequired[bool],
         "Types": NotRequired[List[str]],
     },
 )
 AwsEksClusterLoggingClusterLoggingDetailsTypeDef = TypedDict(
     "AwsEksClusterLoggingClusterLoggingDetailsTypeDef",
@@ -2965,16 +3405,25 @@
         "CurrentVersion": NotRequired[str],
         "Description": NotRequired[str],
         "NewVersion": NotRequired[str],
         "UpdateAvailable": NotRequired[bool],
         "UpdateStatus": NotRequired[str],
     },
 )
-AwsElasticsearchDomainVPCOptionsPaginatorTypeDef = TypedDict(
-    "AwsElasticsearchDomainVPCOptionsPaginatorTypeDef",
+AwsElasticsearchDomainVPCOptionsExtraOutputTypeDef = TypedDict(
+    "AwsElasticsearchDomainVPCOptionsExtraOutputTypeDef",
+    {
+        "AvailabilityZones": NotRequired[List[str]],
+        "SecurityGroupIds": NotRequired[List[str]],
+        "SubnetIds": NotRequired[List[str]],
+        "VPCId": NotRequired[str],
+    },
+)
+AwsElasticsearchDomainVPCOptionsOutputTypeDef = TypedDict(
+    "AwsElasticsearchDomainVPCOptionsOutputTypeDef",
     {
         "AvailabilityZones": NotRequired[List[str]],
         "SecurityGroupIds": NotRequired[List[str]],
         "SubnetIds": NotRequired[List[str]],
         "VPCId": NotRequired[str],
     },
 )
@@ -3045,16 +3494,23 @@
 )
 AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef = TypedDict(
     "AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef",
     {
         "Enabled": NotRequired[bool],
     },
 )
-AwsElbLoadBalancerBackendServerDescriptionPaginatorTypeDef = TypedDict(
-    "AwsElbLoadBalancerBackendServerDescriptionPaginatorTypeDef",
+AwsElbLoadBalancerBackendServerDescriptionExtraOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerBackendServerDescriptionExtraOutputTypeDef",
+    {
+        "InstancePort": NotRequired[int],
+        "PolicyNames": NotRequired[List[str]],
+    },
+)
+AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef",
     {
         "InstancePort": NotRequired[int],
         "PolicyNames": NotRequired[List[str]],
     },
 )
 AwsElbLoadBalancerBackendServerDescriptionTypeDef = TypedDict(
     "AwsElbLoadBalancerBackendServerDescriptionTypeDef",
@@ -3306,16 +3762,24 @@
 )
 AwsLambdaFunctionTracingConfigTypeDef = TypedDict(
     "AwsLambdaFunctionTracingConfigTypeDef",
     {
         "Mode": NotRequired[str],
     },
 )
-AwsLambdaFunctionVpcConfigPaginatorTypeDef = TypedDict(
-    "AwsLambdaFunctionVpcConfigPaginatorTypeDef",
+AwsLambdaFunctionVpcConfigExtraOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionVpcConfigExtraOutputTypeDef",
+    {
+        "SecurityGroupIds": NotRequired[List[str]],
+        "SubnetIds": NotRequired[List[str]],
+        "VpcId": NotRequired[str],
+    },
+)
+AwsLambdaFunctionVpcConfigOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionVpcConfigOutputTypeDef",
     {
         "SecurityGroupIds": NotRequired[List[str]],
         "SubnetIds": NotRequired[List[str]],
         "VpcId": NotRequired[str],
     },
 )
 AwsLambdaFunctionVpcConfigTypeDef = TypedDict(
@@ -3329,43 +3793,58 @@
 AwsLambdaFunctionEnvironmentErrorTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentErrorTypeDef",
     {
         "ErrorCode": NotRequired[str],
         "Message": NotRequired[str],
     },
 )
-AwsLambdaLayerVersionDetailsPaginatorTypeDef = TypedDict(
-    "AwsLambdaLayerVersionDetailsPaginatorTypeDef",
+AwsLambdaLayerVersionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsLambdaLayerVersionDetailsExtraOutputTypeDef",
+    {
+        "Version": NotRequired[int],
+        "CompatibleRuntimes": NotRequired[List[str]],
+        "CreatedDate": NotRequired[str],
+    },
+)
+AwsLambdaLayerVersionDetailsOutputTypeDef = TypedDict(
+    "AwsLambdaLayerVersionDetailsOutputTypeDef",
     {
         "Version": NotRequired[int],
         "CompatibleRuntimes": NotRequired[List[str]],
         "CreatedDate": NotRequired[str],
     },
 )
 AwsLambdaLayerVersionDetailsTypeDef = TypedDict(
     "AwsLambdaLayerVersionDetailsTypeDef",
     {
         "Version": NotRequired[int],
         "CompatibleRuntimes": NotRequired[Sequence[str]],
         "CreatedDate": NotRequired[str],
     },
 )
-AwsMskClusterClusterInfoClientAuthenticationTlsDetailsPaginatorTypeDef = TypedDict(
-    "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsPaginatorTypeDef",
+AwsMskClusterClusterInfoClientAuthenticationTlsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsExtraOutputTypeDef",
     {
         "CertificateAuthorityArnList": NotRequired[List[str]],
         "Enabled": NotRequired[bool],
     },
 )
 AwsMskClusterClusterInfoClientAuthenticationUnauthenticatedDetailsTypeDef = TypedDict(
     "AwsMskClusterClusterInfoClientAuthenticationUnauthenticatedDetailsTypeDef",
     {
         "Enabled": NotRequired[bool],
     },
 )
+AwsMskClusterClusterInfoClientAuthenticationTlsDetailsOutputTypeDef = TypedDict(
+    "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsOutputTypeDef",
+    {
+        "CertificateAuthorityArnList": NotRequired[List[str]],
+        "Enabled": NotRequired[bool],
+    },
+)
 AwsMskClusterClusterInfoClientAuthenticationTlsDetailsTypeDef = TypedDict(
     "AwsMskClusterClusterInfoClientAuthenticationTlsDetailsTypeDef",
     {
         "CertificateAuthorityArnList": NotRequired[Sequence[str]],
         "Enabled": NotRequired[bool],
     },
 )
@@ -3446,16 +3925,23 @@
         "Description": NotRequired[str],
         "NewVersion": NotRequired[str],
         "UpdateAvailable": NotRequired[bool],
         "UpdateStatus": NotRequired[str],
         "OptionalDeployment": NotRequired[bool],
     },
 )
-AwsOpenSearchServiceDomainVpcOptionsDetailsPaginatorTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainVpcOptionsDetailsPaginatorTypeDef",
+AwsOpenSearchServiceDomainVpcOptionsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsExtraOutputTypeDef",
+    {
+        "SecurityGroupIds": NotRequired[List[str]],
+        "SubnetIds": NotRequired[List[str]],
+    },
+)
+AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
     {
         "SecurityGroupIds": NotRequired[List[str]],
         "SubnetIds": NotRequired[List[str]],
     },
 )
 AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef",
@@ -3506,16 +3992,23 @@
 AwsRdsDbInstanceVpcSecurityGroupTypeDef = TypedDict(
     "AwsRdsDbInstanceVpcSecurityGroupTypeDef",
     {
         "VpcSecurityGroupId": NotRequired[str],
         "Status": NotRequired[str],
     },
 )
-AwsRdsDbClusterSnapshotDbClusterSnapshotAttributePaginatorTypeDef = TypedDict(
-    "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributePaginatorTypeDef",
+AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeExtraOutputTypeDef",
+    {
+        "AttributeName": NotRequired[str],
+        "AttributeValues": NotRequired[List[str]],
+    },
+)
+AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef",
     {
         "AttributeName": NotRequired[str],
         "AttributeValues": NotRequired[List[str]],
     },
 )
 AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef = TypedDict(
     "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef",
@@ -3566,16 +4059,23 @@
     {
         "StatusType": NotRequired[str],
         "Normal": NotRequired[bool],
         "Status": NotRequired[str],
         "Message": NotRequired[str],
     },
 )
-AwsRdsPendingCloudWatchLogsExportsPaginatorTypeDef = TypedDict(
-    "AwsRdsPendingCloudWatchLogsExportsPaginatorTypeDef",
+AwsRdsPendingCloudWatchLogsExportsExtraOutputTypeDef = TypedDict(
+    "AwsRdsPendingCloudWatchLogsExportsExtraOutputTypeDef",
+    {
+        "LogTypesToEnable": NotRequired[List[str]],
+        "LogTypesToDisable": NotRequired[List[str]],
+    },
+)
+AwsRdsPendingCloudWatchLogsExportsOutputTypeDef = TypedDict(
+    "AwsRdsPendingCloudWatchLogsExportsOutputTypeDef",
     {
         "LogTypesToEnable": NotRequired[List[str]],
         "LogTypesToDisable": NotRequired[List[str]],
     },
 )
 AwsRdsPendingCloudWatchLogsExportsTypeDef = TypedDict(
     "AwsRdsPendingCloudWatchLogsExportsTypeDef",
@@ -3602,16 +4102,31 @@
 )
 AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef",
     {
         "Name": NotRequired[str],
     },
 )
-AwsRdsEventSubscriptionDetailsPaginatorTypeDef = TypedDict(
-    "AwsRdsEventSubscriptionDetailsPaginatorTypeDef",
+AwsRdsEventSubscriptionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRdsEventSubscriptionDetailsExtraOutputTypeDef",
+    {
+        "CustSubscriptionId": NotRequired[str],
+        "CustomerAwsId": NotRequired[str],
+        "Enabled": NotRequired[bool],
+        "EventCategoriesList": NotRequired[List[str]],
+        "EventSubscriptionArn": NotRequired[str],
+        "SnsTopicArn": NotRequired[str],
+        "SourceIdsList": NotRequired[List[str]],
+        "SourceType": NotRequired[str],
+        "Status": NotRequired[str],
+        "SubscriptionCreationTime": NotRequired[str],
+    },
+)
+AwsRdsEventSubscriptionDetailsOutputTypeDef = TypedDict(
+    "AwsRdsEventSubscriptionDetailsOutputTypeDef",
     {
         "CustSubscriptionId": NotRequired[str],
         "CustomerAwsId": NotRequired[str],
         "Enabled": NotRequired[bool],
         "EventCategoriesList": NotRequired[List[str]],
         "EventSubscriptionArn": NotRequired[str],
         "SnsTopicArn": NotRequired[str],
@@ -3909,41 +4424,16 @@
 )
 AwsSecretsManagerSecretRotationRulesTypeDef = TypedDict(
     "AwsSecretsManagerSecretRotationRulesTypeDef",
     {
         "AutomaticallyAfterDays": NotRequired[int],
     },
 )
-BooleanFilterTypeDef = TypedDict(
-    "BooleanFilterTypeDef",
-    {
-        "Value": NotRequired[bool],
-    },
-)
-IpFilterTypeDef = TypedDict(
-    "IpFilterTypeDef",
-    {
-        "Cidr": NotRequired[str],
-    },
-)
-KeywordFilterTypeDef = TypedDict(
-    "KeywordFilterTypeDef",
-    {
-        "Value": NotRequired[str],
-    },
-)
-AwsSecurityFindingIdentifierTypeDef = TypedDict(
-    "AwsSecurityFindingIdentifierTypeDef",
-    {
-        "Id": str,
-        "ProductArn": str,
-    },
-)
-GeneratorDetailsPaginatorTypeDef = TypedDict(
-    "GeneratorDetailsPaginatorTypeDef",
+GeneratorDetailsExtraOutputTypeDef = TypedDict(
+    "GeneratorDetailsExtraOutputTypeDef",
     {
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "Labels": NotRequired[List[str]],
     },
 )
 MalwareTypeDef = TypedDict(
@@ -4012,14 +4502,47 @@
 )
 WorkflowTypeDef = TypedDict(
     "WorkflowTypeDef",
     {
         "Status": NotRequired[WorkflowStatusType],
     },
 )
+BooleanFilterTypeDef = TypedDict(
+    "BooleanFilterTypeDef",
+    {
+        "Value": NotRequired[bool],
+    },
+)
+IpFilterTypeDef = TypedDict(
+    "IpFilterTypeDef",
+    {
+        "Cidr": NotRequired[str],
+    },
+)
+KeywordFilterTypeDef = TypedDict(
+    "KeywordFilterTypeDef",
+    {
+        "Value": NotRequired[str],
+    },
+)
+AwsSecurityFindingIdentifierTypeDef = TypedDict(
+    "AwsSecurityFindingIdentifierTypeDef",
+    {
+        "Id": str,
+        "ProductArn": str,
+    },
+)
+GeneratorDetailsOutputTypeDef = TypedDict(
+    "GeneratorDetailsOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "Description": NotRequired[str],
+        "Labels": NotRequired[List[str]],
+    },
+)
 GeneratorDetailsTypeDef = TypedDict(
     "GeneratorDetailsTypeDef",
     {
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "Labels": NotRequired[Sequence[str]],
     },
@@ -4313,28 +4836,35 @@
     {
         "EndLine": NotRequired[int],
         "FileName": NotRequired[str],
         "FilePath": NotRequired[str],
         "StartLine": NotRequired[int],
     },
 )
-SecurityControlParameterPaginatorTypeDef = TypedDict(
-    "SecurityControlParameterPaginatorTypeDef",
+SecurityControlParameterExtraOutputTypeDef = TypedDict(
+    "SecurityControlParameterExtraOutputTypeDef",
     {
         "Name": NotRequired[str],
         "Value": NotRequired[List[str]],
     },
 )
 StatusReasonTypeDef = TypedDict(
     "StatusReasonTypeDef",
     {
         "ReasonCode": str,
         "Description": NotRequired[str],
     },
 )
+SecurityControlParameterOutputTypeDef = TypedDict(
+    "SecurityControlParameterOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "Value": NotRequired[List[str]],
+    },
+)
 SecurityControlParameterTypeDef = TypedDict(
     "SecurityControlParameterTypeDef",
     {
         "Name": NotRequired[str],
         "Value": NotRequired[Sequence[str]],
     },
 )
@@ -4854,36 +5384,57 @@
 RecordTypeDef = TypedDict(
     "RecordTypeDef",
     {
         "JsonPath": NotRequired[str],
         "RecordIndex": NotRequired[int],
     },
 )
-ParameterValueTypeDef = TypedDict(
-    "ParameterValueTypeDef",
+ParameterValueOutputTypeDef = TypedDict(
+    "ParameterValueOutputTypeDef",
     {
         "Integer": NotRequired[int],
         "IntegerList": NotRequired[List[int]],
         "Double": NotRequired[float],
         "String": NotRequired[str],
         "StringList": NotRequired[List[str]],
         "Boolean": NotRequired[bool],
         "Enum": NotRequired[str],
         "EnumList": NotRequired[List[str]],
     },
 )
+ParameterValueTypeDef = TypedDict(
+    "ParameterValueTypeDef",
+    {
+        "Integer": NotRequired[int],
+        "IntegerList": NotRequired[Sequence[int]],
+        "Double": NotRequired[float],
+        "String": NotRequired[str],
+        "StringList": NotRequired[Sequence[str]],
+        "Boolean": NotRequired[bool],
+        "Enum": NotRequired[str],
+        "EnumList": NotRequired[Sequence[str]],
+    },
+)
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Text": NotRequired[str],
         "Url": NotRequired[str],
     },
 )
-RuleGroupSourceListDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceListDetailsPaginatorTypeDef",
+RuleGroupSourceListDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceListDetailsExtraOutputTypeDef",
+    {
+        "GeneratedRulesType": NotRequired[str],
+        "TargetTypes": NotRequired[List[str]],
+        "Targets": NotRequired[List[str]],
+    },
+)
+RuleGroupSourceListDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceListDetailsOutputTypeDef",
     {
         "GeneratedRulesType": NotRequired[str],
         "TargetTypes": NotRequired[List[str]],
         "Targets": NotRequired[List[str]],
     },
 )
 RuleGroupSourceListDetailsTypeDef = TypedDict(
@@ -4901,16 +5452,23 @@
         "DestinationPort": NotRequired[str],
         "Direction": NotRequired[str],
         "Protocol": NotRequired[str],
         "Source": NotRequired[str],
         "SourcePort": NotRequired[str],
     },
 )
-RuleGroupSourceStatefulRulesOptionsDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceStatefulRulesOptionsDetailsPaginatorTypeDef",
+RuleGroupSourceStatefulRulesOptionsDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatefulRulesOptionsDetailsExtraOutputTypeDef",
+    {
+        "Keyword": NotRequired[str],
+        "Settings": NotRequired[List[str]],
+    },
+)
+RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef",
     {
         "Keyword": NotRequired[str],
         "Settings": NotRequired[List[str]],
     },
 )
 RuleGroupSourceStatefulRulesOptionsDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesOptionsDetailsTypeDef",
@@ -4941,42 +5499,61 @@
 )
 RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
     {
         "AddressDefinition": NotRequired[str],
     },
 )
-RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsPaginatorTypeDef",
+RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsExtraOutputTypeDef",
+    {
+        "Flags": NotRequired[List[str]],
+        "Masks": NotRequired[List[str]],
+    },
+)
+RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef",
     {
         "Flags": NotRequired[List[str]],
         "Masks": NotRequired[List[str]],
     },
 )
 RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
     {
         "Flags": NotRequired[Sequence[str]],
         "Masks": NotRequired[Sequence[str]],
     },
 )
-RuleGroupVariablesIpSetsDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupVariablesIpSetsDetailsPaginatorTypeDef",
+RuleGroupVariablesIpSetsDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupVariablesIpSetsDetailsExtraOutputTypeDef",
+    {
+        "Definition": NotRequired[List[str]],
+    },
+)
+RuleGroupVariablesPortSetsDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupVariablesPortSetsDetailsExtraOutputTypeDef",
+    {
+        "Definition": NotRequired[List[str]],
+    },
+)
+RuleGroupVariablesIpSetsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupVariablesIpSetsDetailsOutputTypeDef",
     {
         "Definition": NotRequired[List[str]],
     },
 )
 RuleGroupVariablesIpSetsDetailsTypeDef = TypedDict(
     "RuleGroupVariablesIpSetsDetailsTypeDef",
     {
         "Definition": NotRequired[Sequence[str]],
     },
 )
-RuleGroupVariablesPortSetsDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupVariablesPortSetsDetailsPaginatorTypeDef",
+RuleGroupVariablesPortSetsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupVariablesPortSetsDetailsOutputTypeDef",
     {
         "Definition": NotRequired[List[str]],
     },
 )
 RuleGroupVariablesPortSetsDetailsTypeDef = TypedDict(
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     {
@@ -5085,16 +5662,26 @@
         "IpAddressV4": NotRequired[str],
         "Organization": NotRequired[IpOrganizationDetailsTypeDef],
         "Country": NotRequired[CountryTypeDef],
         "City": NotRequired[CityTypeDef],
         "GeoLocation": NotRequired[GeoLocationTypeDef],
     },
 )
-CvssPaginatorTypeDef = TypedDict(
-    "CvssPaginatorTypeDef",
+CvssExtraOutputTypeDef = TypedDict(
+    "CvssExtraOutputTypeDef",
+    {
+        "Version": NotRequired[str],
+        "BaseScore": NotRequired[float],
+        "BaseVector": NotRequired[str],
+        "Source": NotRequired[str],
+        "Adjustments": NotRequired[List[AdjustmentTypeDef]],
+    },
+)
+CvssOutputTypeDef = TypedDict(
+    "CvssOutputTypeDef",
     {
         "Version": NotRequired[str],
         "BaseScore": NotRequired[float],
         "BaseVector": NotRequired[str],
         "Source": NotRequired[str],
         "Adjustments": NotRequired[List[AdjustmentTypeDef]],
     },
@@ -5124,50 +5711,78 @@
         "GatewayId": NotRequired[str],
         "Main": NotRequired[bool],
         "RouteTableAssociationId": NotRequired[str],
         "RouteTableId": NotRequired[str],
         "SubnetId": NotRequired[str],
     },
 )
-AutomationRulesFindingFieldsUpdateTypeDef = TypedDict(
-    "AutomationRulesFindingFieldsUpdateTypeDef",
+AutomationRulesFindingFieldsUpdateOutputTypeDef = TypedDict(
+    "AutomationRulesFindingFieldsUpdateOutputTypeDef",
     {
         "Note": NotRequired[NoteUpdateTypeDef],
         "Severity": NotRequired[SeverityUpdateTypeDef],
         "VerificationState": NotRequired[VerificationStateType],
         "Confidence": NotRequired[int],
         "Criticality": NotRequired[int],
         "Types": NotRequired[List[str]],
         "UserDefinedFields": NotRequired[Dict[str, str]],
         "Workflow": NotRequired[WorkflowUpdateTypeDef],
         "RelatedFindings": NotRequired[List[RelatedFindingTypeDef]],
     },
 )
+AutomationRulesFindingFieldsUpdateTypeDef = TypedDict(
+    "AutomationRulesFindingFieldsUpdateTypeDef",
+    {
+        "Note": NotRequired[NoteUpdateTypeDef],
+        "Severity": NotRequired[SeverityUpdateTypeDef],
+        "VerificationState": NotRequired[VerificationStateType],
+        "Confidence": NotRequired[int],
+        "Criticality": NotRequired[int],
+        "Types": NotRequired[Sequence[str]],
+        "UserDefinedFields": NotRequired[Mapping[str, str]],
+        "Workflow": NotRequired[WorkflowUpdateTypeDef],
+        "RelatedFindings": NotRequired[Sequence[RelatedFindingTypeDef]],
+    },
+)
 AwsAmazonMqBrokerLogsDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsDetailsTypeDef",
     {
         "Audit": NotRequired[bool],
         "General": NotRequired[bool],
         "AuditLogGroup": NotRequired[str],
         "GeneralLogGroup": NotRequired[str],
         "Pending": NotRequired[AwsAmazonMqBrokerLogsPendingDetailsTypeDef],
     },
 )
-AwsApiGatewayRestApiDetailsPaginatorTypeDef = TypedDict(
-    "AwsApiGatewayRestApiDetailsPaginatorTypeDef",
+AwsApiGatewayRestApiDetailsExtraOutputTypeDef = TypedDict(
+    "AwsApiGatewayRestApiDetailsExtraOutputTypeDef",
     {
         "Id": NotRequired[str],
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "CreatedDate": NotRequired[str],
         "Version": NotRequired[str],
         "BinaryMediaTypes": NotRequired[List[str]],
         "MinimumCompressionSize": NotRequired[int],
         "ApiKeySource": NotRequired[str],
-        "EndpointConfiguration": NotRequired[AwsApiGatewayEndpointConfigurationPaginatorTypeDef],
+        "EndpointConfiguration": NotRequired[AwsApiGatewayEndpointConfigurationExtraOutputTypeDef],
+    },
+)
+AwsApiGatewayRestApiDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayRestApiDetailsOutputTypeDef",
+    {
+        "Id": NotRequired[str],
+        "Name": NotRequired[str],
+        "Description": NotRequired[str],
+        "CreatedDate": NotRequired[str],
+        "Version": NotRequired[str],
+        "BinaryMediaTypes": NotRequired[List[str]],
+        "MinimumCompressionSize": NotRequired[int],
+        "ApiKeySource": NotRequired[str],
+        "EndpointConfiguration": NotRequired[AwsApiGatewayEndpointConfigurationOutputTypeDef],
     },
 )
 AwsApiGatewayRestApiDetailsTypeDef = TypedDict(
     "AwsApiGatewayRestApiDetailsTypeDef",
     {
         "Id": NotRequired[str],
         "Name": NotRequired[str],
@@ -5176,29 +5791,50 @@
         "Version": NotRequired[str],
         "BinaryMediaTypes": NotRequired[Sequence[str]],
         "MinimumCompressionSize": NotRequired[int],
         "ApiKeySource": NotRequired[str],
         "EndpointConfiguration": NotRequired[AwsApiGatewayEndpointConfigurationTypeDef],
     },
 )
-AwsApiGatewayStageDetailsPaginatorTypeDef = TypedDict(
-    "AwsApiGatewayStageDetailsPaginatorTypeDef",
+AwsApiGatewayStageDetailsExtraOutputTypeDef = TypedDict(
+    "AwsApiGatewayStageDetailsExtraOutputTypeDef",
+    {
+        "DeploymentId": NotRequired[str],
+        "ClientCertificateId": NotRequired[str],
+        "StageName": NotRequired[str],
+        "Description": NotRequired[str],
+        "CacheClusterEnabled": NotRequired[bool],
+        "CacheClusterSize": NotRequired[str],
+        "CacheClusterStatus": NotRequired[str],
+        "MethodSettings": NotRequired[List[AwsApiGatewayMethodSettingsTypeDef]],
+        "Variables": NotRequired[Dict[str, str]],
+        "DocumentationVersion": NotRequired[str],
+        "AccessLogSettings": NotRequired[AwsApiGatewayAccessLogSettingsTypeDef],
+        "CanarySettings": NotRequired[AwsApiGatewayCanarySettingsExtraOutputTypeDef],
+        "TracingEnabled": NotRequired[bool],
+        "CreatedDate": NotRequired[str],
+        "LastUpdatedDate": NotRequired[str],
+        "WebAclArn": NotRequired[str],
+    },
+)
+AwsApiGatewayStageDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayStageDetailsOutputTypeDef",
     {
         "DeploymentId": NotRequired[str],
         "ClientCertificateId": NotRequired[str],
         "StageName": NotRequired[str],
         "Description": NotRequired[str],
         "CacheClusterEnabled": NotRequired[bool],
         "CacheClusterSize": NotRequired[str],
         "CacheClusterStatus": NotRequired[str],
         "MethodSettings": NotRequired[List[AwsApiGatewayMethodSettingsTypeDef]],
         "Variables": NotRequired[Dict[str, str]],
         "DocumentationVersion": NotRequired[str],
         "AccessLogSettings": NotRequired[AwsApiGatewayAccessLogSettingsTypeDef],
-        "CanarySettings": NotRequired[AwsApiGatewayCanarySettingsPaginatorTypeDef],
+        "CanarySettings": NotRequired[AwsApiGatewayCanarySettingsOutputTypeDef],
         "TracingEnabled": NotRequired[bool],
         "CreatedDate": NotRequired[str],
         "LastUpdatedDate": NotRequired[str],
         "WebAclArn": NotRequired[str],
     },
 )
 AwsApiGatewayStageDetailsTypeDef = TypedDict(
@@ -5218,27 +5854,42 @@
         "CanarySettings": NotRequired[AwsApiGatewayCanarySettingsTypeDef],
         "TracingEnabled": NotRequired[bool],
         "CreatedDate": NotRequired[str],
         "LastUpdatedDate": NotRequired[str],
         "WebAclArn": NotRequired[str],
     },
 )
-AwsApiGatewayV2ApiDetailsPaginatorTypeDef = TypedDict(
-    "AwsApiGatewayV2ApiDetailsPaginatorTypeDef",
+AwsApiGatewayV2ApiDetailsExtraOutputTypeDef = TypedDict(
+    "AwsApiGatewayV2ApiDetailsExtraOutputTypeDef",
+    {
+        "ApiEndpoint": NotRequired[str],
+        "ApiId": NotRequired[str],
+        "ApiKeySelectionExpression": NotRequired[str],
+        "CreatedDate": NotRequired[str],
+        "Description": NotRequired[str],
+        "Version": NotRequired[str],
+        "Name": NotRequired[str],
+        "ProtocolType": NotRequired[str],
+        "RouteSelectionExpression": NotRequired[str],
+        "CorsConfiguration": NotRequired[AwsCorsConfigurationExtraOutputTypeDef],
+    },
+)
+AwsApiGatewayV2ApiDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayV2ApiDetailsOutputTypeDef",
     {
         "ApiEndpoint": NotRequired[str],
         "ApiId": NotRequired[str],
         "ApiKeySelectionExpression": NotRequired[str],
         "CreatedDate": NotRequired[str],
         "Description": NotRequired[str],
         "Version": NotRequired[str],
         "Name": NotRequired[str],
         "ProtocolType": NotRequired[str],
         "RouteSelectionExpression": NotRequired[str],
-        "CorsConfiguration": NotRequired[AwsCorsConfigurationPaginatorTypeDef],
+        "CorsConfiguration": NotRequired[AwsCorsConfigurationOutputTypeDef],
     },
 )
 AwsApiGatewayV2ApiDetailsTypeDef = TypedDict(
     "AwsApiGatewayV2ApiDetailsTypeDef",
     {
         "ApiEndpoint": NotRequired[str],
         "ApiId": NotRequired[str],
@@ -5248,16 +5899,34 @@
         "Version": NotRequired[str],
         "Name": NotRequired[str],
         "ProtocolType": NotRequired[str],
         "RouteSelectionExpression": NotRequired[str],
         "CorsConfiguration": NotRequired[AwsCorsConfigurationTypeDef],
     },
 )
-AwsApiGatewayV2StageDetailsPaginatorTypeDef = TypedDict(
-    "AwsApiGatewayV2StageDetailsPaginatorTypeDef",
+AwsApiGatewayV2StageDetailsExtraOutputTypeDef = TypedDict(
+    "AwsApiGatewayV2StageDetailsExtraOutputTypeDef",
+    {
+        "ClientCertificateId": NotRequired[str],
+        "CreatedDate": NotRequired[str],
+        "Description": NotRequired[str],
+        "DefaultRouteSettings": NotRequired[AwsApiGatewayV2RouteSettingsTypeDef],
+        "DeploymentId": NotRequired[str],
+        "LastUpdatedDate": NotRequired[str],
+        "RouteSettings": NotRequired[AwsApiGatewayV2RouteSettingsTypeDef],
+        "StageName": NotRequired[str],
+        "StageVariables": NotRequired[Dict[str, str]],
+        "AccessLogSettings": NotRequired[AwsApiGatewayAccessLogSettingsTypeDef],
+        "AutoDeploy": NotRequired[bool],
+        "LastDeploymentStatusMessage": NotRequired[str],
+        "ApiGatewayManaged": NotRequired[bool],
+    },
+)
+AwsApiGatewayV2StageDetailsOutputTypeDef = TypedDict(
+    "AwsApiGatewayV2StageDetailsOutputTypeDef",
     {
         "ClientCertificateId": NotRequired[str],
         "CreatedDate": NotRequired[str],
         "Description": NotRequired[str],
         "DefaultRouteSettings": NotRequired[AwsApiGatewayV2RouteSettingsTypeDef],
         "DeploymentId": NotRequired[str],
         "LastUpdatedDate": NotRequired[str],
@@ -5303,16 +5972,29 @@
     "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef",
     {
         "EncryptionConfiguration": NotRequired[
             AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef
         ],
     },
 )
-AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsPaginatorTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsPaginatorTypeDef",
+AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsExtraOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsExtraOutputTypeDef",
+    {
+        "LaunchTemplateSpecification": NotRequired[
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef
+        ],
+        "Overrides": NotRequired[
+            List[
+                AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef
+            ]
+        ],
+    },
+)
+AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef",
     {
         "LaunchTemplateSpecification": NotRequired[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef
         ],
         "Overrides": NotRequired[
             List[
                 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef
@@ -5345,21 +6027,31 @@
 AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef",
     {
         "DestinationBackupVaultArn": NotRequired[str],
         "Lifecycle": NotRequired[AwsBackupBackupPlanLifecycleDetailsTypeDef],
     },
 )
-AwsBackupBackupVaultDetailsPaginatorTypeDef = TypedDict(
-    "AwsBackupBackupVaultDetailsPaginatorTypeDef",
+AwsBackupBackupVaultDetailsExtraOutputTypeDef = TypedDict(
+    "AwsBackupBackupVaultDetailsExtraOutputTypeDef",
     {
         "BackupVaultArn": NotRequired[str],
         "BackupVaultName": NotRequired[str],
         "EncryptionKeyArn": NotRequired[str],
-        "Notifications": NotRequired[AwsBackupBackupVaultNotificationsDetailsPaginatorTypeDef],
+        "Notifications": NotRequired[AwsBackupBackupVaultNotificationsDetailsExtraOutputTypeDef],
+        "AccessPolicy": NotRequired[str],
+    },
+)
+AwsBackupBackupVaultDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupVaultDetailsOutputTypeDef",
+    {
+        "BackupVaultArn": NotRequired[str],
+        "BackupVaultName": NotRequired[str],
+        "EncryptionKeyArn": NotRequired[str],
+        "Notifications": NotRequired[AwsBackupBackupVaultNotificationsDetailsOutputTypeDef],
         "AccessPolicy": NotRequired[str],
     },
 )
 AwsBackupBackupVaultDetailsTypeDef = TypedDict(
     "AwsBackupBackupVaultDetailsTypeDef",
     {
         "BackupVaultArn": NotRequired[str],
@@ -5389,16 +6081,27 @@
         "ResourceType": NotRequired[str],
         "SourceBackupVaultArn": NotRequired[str],
         "Status": NotRequired[str],
         "StatusMessage": NotRequired[str],
         "StorageClass": NotRequired[str],
     },
 )
-AwsCertificateManagerCertificateDomainValidationOptionPaginatorTypeDef = TypedDict(
-    "AwsCertificateManagerCertificateDomainValidationOptionPaginatorTypeDef",
+AwsCertificateManagerCertificateDomainValidationOptionExtraOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateDomainValidationOptionExtraOutputTypeDef",
+    {
+        "DomainName": NotRequired[str],
+        "ResourceRecord": NotRequired[AwsCertificateManagerCertificateResourceRecordTypeDef],
+        "ValidationDomain": NotRequired[str],
+        "ValidationEmails": NotRequired[List[str]],
+        "ValidationMethod": NotRequired[str],
+        "ValidationStatus": NotRequired[str],
+    },
+)
+AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef",
     {
         "DomainName": NotRequired[str],
         "ResourceRecord": NotRequired[AwsCertificateManagerCertificateResourceRecordTypeDef],
         "ValidationDomain": NotRequired[str],
         "ValidationEmails": NotRequired[List[str]],
         "ValidationMethod": NotRequired[str],
         "ValidationStatus": NotRequired[str],
@@ -5411,16 +6114,36 @@
         "ResourceRecord": NotRequired[AwsCertificateManagerCertificateResourceRecordTypeDef],
         "ValidationDomain": NotRequired[str],
         "ValidationEmails": NotRequired[Sequence[str]],
         "ValidationMethod": NotRequired[str],
         "ValidationStatus": NotRequired[str],
     },
 )
-AwsCloudFormationStackDetailsPaginatorTypeDef = TypedDict(
-    "AwsCloudFormationStackDetailsPaginatorTypeDef",
+AwsCloudFormationStackDetailsExtraOutputTypeDef = TypedDict(
+    "AwsCloudFormationStackDetailsExtraOutputTypeDef",
+    {
+        "Capabilities": NotRequired[List[str]],
+        "CreationTime": NotRequired[str],
+        "Description": NotRequired[str],
+        "DisableRollback": NotRequired[bool],
+        "DriftInformation": NotRequired[AwsCloudFormationStackDriftInformationDetailsTypeDef],
+        "EnableTerminationProtection": NotRequired[bool],
+        "LastUpdatedTime": NotRequired[str],
+        "NotificationArns": NotRequired[List[str]],
+        "Outputs": NotRequired[List[AwsCloudFormationStackOutputsDetailsTypeDef]],
+        "RoleArn": NotRequired[str],
+        "StackId": NotRequired[str],
+        "StackName": NotRequired[str],
+        "StackStatus": NotRequired[str],
+        "StackStatusReason": NotRequired[str],
+        "TimeoutInMinutes": NotRequired[int],
+    },
+)
+AwsCloudFormationStackDetailsOutputTypeDef = TypedDict(
+    "AwsCloudFormationStackDetailsOutputTypeDef",
     {
         "Capabilities": NotRequired[List[str]],
         "CreationTime": NotRequired[str],
         "Description": NotRequired[str],
         "DisableRollback": NotRequired[bool],
         "DriftInformation": NotRequired[AwsCloudFormationStackDriftInformationDetailsTypeDef],
         "EnableTerminationProtection": NotRequired[bool],
@@ -5451,66 +6174,118 @@
         "StackId": NotRequired[str],
         "StackName": NotRequired[str],
         "StackStatus": NotRequired[str],
         "StackStatusReason": NotRequired[str],
         "TimeoutInMinutes": NotRequired[int],
     },
 )
-AwsCloudFrontDistributionCacheBehaviorsPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionCacheBehaviorsPaginatorTypeDef",
+AwsCloudFrontDistributionCacheBehaviorsExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionCacheBehaviorsExtraOutputTypeDef",
+    {
+        "Items": NotRequired[List[AwsCloudFrontDistributionCacheBehaviorTypeDef]],
+    },
+)
+AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef",
     {
         "Items": NotRequired[List[AwsCloudFrontDistributionCacheBehaviorTypeDef]],
     },
 )
 AwsCloudFrontDistributionCacheBehaviorsTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorsTypeDef",
     {
         "Items": NotRequired[Sequence[AwsCloudFrontDistributionCacheBehaviorTypeDef]],
     },
 )
-AwsCloudFrontDistributionOriginCustomOriginConfigPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginCustomOriginConfigPaginatorTypeDef",
+AwsCloudFrontDistributionOriginCustomOriginConfigExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginCustomOriginConfigExtraOutputTypeDef",
     {
         "HttpPort": NotRequired[int],
         "HttpsPort": NotRequired[int],
         "OriginKeepaliveTimeout": NotRequired[int],
         "OriginProtocolPolicy": NotRequired[str],
         "OriginReadTimeout": NotRequired[int],
         "OriginSslProtocols": NotRequired[
-            AwsCloudFrontDistributionOriginSslProtocolsPaginatorTypeDef
+            AwsCloudFrontDistributionOriginSslProtocolsExtraOutputTypeDef
         ],
     },
 )
+AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef",
+    {
+        "HttpPort": NotRequired[int],
+        "HttpsPort": NotRequired[int],
+        "OriginKeepaliveTimeout": NotRequired[int],
+        "OriginProtocolPolicy": NotRequired[str],
+        "OriginReadTimeout": NotRequired[int],
+        "OriginSslProtocols": NotRequired[AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef],
+    },
+)
 AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef",
     {
         "HttpPort": NotRequired[int],
         "HttpsPort": NotRequired[int],
         "OriginKeepaliveTimeout": NotRequired[int],
         "OriginProtocolPolicy": NotRequired[str],
         "OriginReadTimeout": NotRequired[int],
         "OriginSslProtocols": NotRequired[AwsCloudFrontDistributionOriginSslProtocolsTypeDef],
     },
 )
-AwsCloudFrontDistributionOriginGroupFailoverPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginGroupFailoverPaginatorTypeDef",
+AwsCloudFrontDistributionOriginGroupFailoverExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupFailoverExtraOutputTypeDef",
+    {
+        "StatusCodes": NotRequired[
+            AwsCloudFrontDistributionOriginGroupFailoverStatusCodesExtraOutputTypeDef
+        ],
+    },
+)
+AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef",
     {
         "StatusCodes": NotRequired[
-            AwsCloudFrontDistributionOriginGroupFailoverStatusCodesPaginatorTypeDef
+            AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef
         ],
     },
 )
 AwsCloudFrontDistributionOriginGroupFailoverTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverTypeDef",
     {
         "StatusCodes": NotRequired[AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef],
     },
 )
-AwsCloudWatchAlarmDetailsPaginatorTypeDef = TypedDict(
-    "AwsCloudWatchAlarmDetailsPaginatorTypeDef",
+AwsCloudWatchAlarmDetailsExtraOutputTypeDef = TypedDict(
+    "AwsCloudWatchAlarmDetailsExtraOutputTypeDef",
+    {
+        "ActionsEnabled": NotRequired[bool],
+        "AlarmActions": NotRequired[List[str]],
+        "AlarmArn": NotRequired[str],
+        "AlarmConfigurationUpdatedTimestamp": NotRequired[str],
+        "AlarmDescription": NotRequired[str],
+        "AlarmName": NotRequired[str],
+        "ComparisonOperator": NotRequired[str],
+        "DatapointsToAlarm": NotRequired[int],
+        "Dimensions": NotRequired[List[AwsCloudWatchAlarmDimensionsDetailsTypeDef]],
+        "EvaluateLowSampleCountPercentile": NotRequired[str],
+        "EvaluationPeriods": NotRequired[int],
+        "ExtendedStatistic": NotRequired[str],
+        "InsufficientDataActions": NotRequired[List[str]],
+        "MetricName": NotRequired[str],
+        "Namespace": NotRequired[str],
+        "OkActions": NotRequired[List[str]],
+        "Period": NotRequired[int],
+        "Statistic": NotRequired[str],
+        "Threshold": NotRequired[float],
+        "ThresholdMetricId": NotRequired[str],
+        "TreatMissingData": NotRequired[str],
+        "Unit": NotRequired[str],
+    },
+)
+AwsCloudWatchAlarmDetailsOutputTypeDef = TypedDict(
+    "AwsCloudWatchAlarmDetailsOutputTypeDef",
     {
         "ActionsEnabled": NotRequired[bool],
         "AlarmActions": NotRequired[List[str]],
         "AlarmArn": NotRequired[str],
         "AlarmConfigurationUpdatedTimestamp": NotRequired[str],
         "AlarmDescription": NotRequired[str],
         "AlarmName": NotRequired[str],
@@ -5555,16 +6330,29 @@
         "Statistic": NotRequired[str],
         "Threshold": NotRequired[float],
         "ThresholdMetricId": NotRequired[str],
         "TreatMissingData": NotRequired[str],
         "Unit": NotRequired[str],
     },
 )
-AwsCodeBuildProjectEnvironmentPaginatorTypeDef = TypedDict(
-    "AwsCodeBuildProjectEnvironmentPaginatorTypeDef",
+AwsCodeBuildProjectEnvironmentExtraOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectEnvironmentExtraOutputTypeDef",
+    {
+        "Certificate": NotRequired[str],
+        "EnvironmentVariables": NotRequired[
+            List[AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef]
+        ],
+        "PrivilegedMode": NotRequired[bool],
+        "ImagePullCredentialsType": NotRequired[str],
+        "RegistryCredential": NotRequired[AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef],
+        "Type": NotRequired[str],
+    },
+)
+AwsCodeBuildProjectEnvironmentOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectEnvironmentOutputTypeDef",
     {
         "Certificate": NotRequired[str],
         "EnvironmentVariables": NotRequired[
             List[AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef]
         ],
         "PrivilegedMode": NotRequired[bool],
         "ImagePullCredentialsType": NotRequired[str],
@@ -5588,16 +6376,37 @@
 AwsCodeBuildProjectLogsConfigDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
     {
         "CloudWatchLogs": NotRequired[AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef],
         "S3Logs": NotRequired[AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef],
     },
 )
-AwsDmsReplicationInstanceDetailsPaginatorTypeDef = TypedDict(
-    "AwsDmsReplicationInstanceDetailsPaginatorTypeDef",
+AwsDmsReplicationInstanceDetailsExtraOutputTypeDef = TypedDict(
+    "AwsDmsReplicationInstanceDetailsExtraOutputTypeDef",
+    {
+        "AllocatedStorage": NotRequired[int],
+        "AutoMinorVersionUpgrade": NotRequired[bool],
+        "AvailabilityZone": NotRequired[str],
+        "EngineVersion": NotRequired[str],
+        "KmsKeyId": NotRequired[str],
+        "MultiAZ": NotRequired[bool],
+        "PreferredMaintenanceWindow": NotRequired[str],
+        "PubliclyAccessible": NotRequired[bool],
+        "ReplicationInstanceClass": NotRequired[str],
+        "ReplicationInstanceIdentifier": NotRequired[str],
+        "ReplicationSubnetGroup": NotRequired[
+            AwsDmsReplicationInstanceReplicationSubnetGroupDetailsTypeDef
+        ],
+        "VpcSecurityGroups": NotRequired[
+            List[AwsDmsReplicationInstanceVpcSecurityGroupsDetailsTypeDef]
+        ],
+    },
+)
+AwsDmsReplicationInstanceDetailsOutputTypeDef = TypedDict(
+    "AwsDmsReplicationInstanceDetailsOutputTypeDef",
     {
         "AllocatedStorage": NotRequired[int],
         "AutoMinorVersionUpgrade": NotRequired[bool],
         "AvailabilityZone": NotRequired[str],
         "EngineVersion": NotRequired[str],
         "KmsKeyId": NotRequired[str],
         "MultiAZ": NotRequired[bool],
@@ -5630,35 +6439,58 @@
             AwsDmsReplicationInstanceReplicationSubnetGroupDetailsTypeDef
         ],
         "VpcSecurityGroups": NotRequired[
             Sequence[AwsDmsReplicationInstanceVpcSecurityGroupsDetailsTypeDef]
         ],
     },
 )
-AwsDynamoDbTableGlobalSecondaryIndexPaginatorTypeDef = TypedDict(
-    "AwsDynamoDbTableGlobalSecondaryIndexPaginatorTypeDef",
+AwsDynamoDbTableGlobalSecondaryIndexExtraOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableGlobalSecondaryIndexExtraOutputTypeDef",
+    {
+        "Backfilling": NotRequired[bool],
+        "IndexArn": NotRequired[str],
+        "IndexName": NotRequired[str],
+        "IndexSizeBytes": NotRequired[int],
+        "IndexStatus": NotRequired[str],
+        "ItemCount": NotRequired[int],
+        "KeySchema": NotRequired[List[AwsDynamoDbTableKeySchemaTypeDef]],
+        "Projection": NotRequired[AwsDynamoDbTableProjectionExtraOutputTypeDef],
+        "ProvisionedThroughput": NotRequired[AwsDynamoDbTableProvisionedThroughputTypeDef],
+    },
+)
+AwsDynamoDbTableLocalSecondaryIndexExtraOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableLocalSecondaryIndexExtraOutputTypeDef",
+    {
+        "IndexArn": NotRequired[str],
+        "IndexName": NotRequired[str],
+        "KeySchema": NotRequired[List[AwsDynamoDbTableKeySchemaTypeDef]],
+        "Projection": NotRequired[AwsDynamoDbTableProjectionExtraOutputTypeDef],
+    },
+)
+AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef",
     {
         "Backfilling": NotRequired[bool],
         "IndexArn": NotRequired[str],
         "IndexName": NotRequired[str],
         "IndexSizeBytes": NotRequired[int],
         "IndexStatus": NotRequired[str],
         "ItemCount": NotRequired[int],
         "KeySchema": NotRequired[List[AwsDynamoDbTableKeySchemaTypeDef]],
-        "Projection": NotRequired[AwsDynamoDbTableProjectionPaginatorTypeDef],
+        "Projection": NotRequired[AwsDynamoDbTableProjectionOutputTypeDef],
         "ProvisionedThroughput": NotRequired[AwsDynamoDbTableProvisionedThroughputTypeDef],
     },
 )
-AwsDynamoDbTableLocalSecondaryIndexPaginatorTypeDef = TypedDict(
-    "AwsDynamoDbTableLocalSecondaryIndexPaginatorTypeDef",
+AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef",
     {
         "IndexArn": NotRequired[str],
         "IndexName": NotRequired[str],
         "KeySchema": NotRequired[List[AwsDynamoDbTableKeySchemaTypeDef]],
-        "Projection": NotRequired[AwsDynamoDbTableProjectionPaginatorTypeDef],
+        "Projection": NotRequired[AwsDynamoDbTableProjectionOutputTypeDef],
     },
 )
 AwsDynamoDbTableGlobalSecondaryIndexTypeDef = TypedDict(
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     {
         "Backfilling": NotRequired[bool],
         "IndexArn": NotRequired[str],
@@ -5708,16 +6540,34 @@
     "AwsEc2ClientVpnEndpointClientConnectOptionsDetailsTypeDef",
     {
         "Enabled": NotRequired[bool],
         "LambdaFunctionArn": NotRequired[str],
         "Status": NotRequired[AwsEc2ClientVpnEndpointClientConnectOptionsStatusDetailsTypeDef],
     },
 )
-AwsEc2InstanceDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2InstanceDetailsPaginatorTypeDef",
+AwsEc2InstanceDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2InstanceDetailsExtraOutputTypeDef",
+    {
+        "Type": NotRequired[str],
+        "ImageId": NotRequired[str],
+        "IpV4Addresses": NotRequired[List[str]],
+        "IpV6Addresses": NotRequired[List[str]],
+        "KeyName": NotRequired[str],
+        "IamInstanceProfileArn": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "SubnetId": NotRequired[str],
+        "LaunchedAt": NotRequired[str],
+        "NetworkInterfaces": NotRequired[List[AwsEc2InstanceNetworkInterfacesDetailsTypeDef]],
+        "VirtualizationType": NotRequired[str],
+        "MetadataOptions": NotRequired[AwsEc2InstanceMetadataOptionsTypeDef],
+        "Monitoring": NotRequired[AwsEc2InstanceMonitoringDetailsTypeDef],
+    },
+)
+AwsEc2InstanceDetailsOutputTypeDef = TypedDict(
+    "AwsEc2InstanceDetailsOutputTypeDef",
     {
         "Type": NotRequired[str],
         "ImageId": NotRequired[str],
         "IpV4Addresses": NotRequired[List[str]],
         "IpV6Addresses": NotRequired[List[str]],
         "KeyName": NotRequired[str],
         "IamInstanceProfileArn": NotRequired[str],
@@ -5771,16 +6621,58 @@
     {
         "MarketType": NotRequired[str],
         "SpotOptions": NotRequired[
             AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef
         ],
     },
 )
-AwsEc2LaunchTemplateDataInstanceRequirementsDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsPaginatorTypeDef",
+AwsEc2LaunchTemplateDataInstanceRequirementsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsExtraOutputTypeDef",
+    {
+        "AcceleratorCount": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
+        ],
+        "AcceleratorManufacturers": NotRequired[List[str]],
+        "AcceleratorNames": NotRequired[List[str]],
+        "AcceleratorTotalMemoryMiB": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef
+        ],
+        "AcceleratorTypes": NotRequired[List[str]],
+        "BareMetal": NotRequired[str],
+        "BaselineEbsBandwidthMbps": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef
+        ],
+        "BurstablePerformance": NotRequired[str],
+        "CpuManufacturers": NotRequired[List[str]],
+        "ExcludedInstanceTypes": NotRequired[List[str]],
+        "InstanceGenerations": NotRequired[List[str]],
+        "LocalStorage": NotRequired[str],
+        "LocalStorageTypes": NotRequired[List[str]],
+        "MemoryGiBPerVCpu": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef
+        ],
+        "MemoryMiB": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef
+        ],
+        "NetworkInterfaceCount": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef
+        ],
+        "OnDemandMaxPricePercentageOverLowestPrice": NotRequired[int],
+        "RequireHibernateSupport": NotRequired[bool],
+        "SpotMaxPricePercentageOverLowestPrice": NotRequired[int],
+        "TotalLocalStorageGB": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef
+        ],
+        "VCpuCount": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef
+        ],
+    },
+)
+AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef",
     {
         "AcceleratorCount": NotRequired[
             AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
         ],
         "AcceleratorManufacturers": NotRequired[List[str]],
         "AcceleratorNames": NotRequired[List[str]],
         "AcceleratorTotalMemoryMiB": NotRequired[
@@ -5855,16 +6747,48 @@
             AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef
         ],
         "VCpuCount": NotRequired[
             AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef
         ],
     },
 )
-AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsPaginatorTypeDef",
+AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsExtraOutputTypeDef",
+    {
+        "AssociateCarrierIpAddress": NotRequired[bool],
+        "AssociatePublicIpAddress": NotRequired[bool],
+        "DeleteOnTermination": NotRequired[bool],
+        "Description": NotRequired[str],
+        "DeviceIndex": NotRequired[int],
+        "Groups": NotRequired[List[str]],
+        "InterfaceType": NotRequired[str],
+        "Ipv4PrefixCount": NotRequired[int],
+        "Ipv4Prefixes": NotRequired[
+            List[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef]
+        ],
+        "Ipv6AddressCount": NotRequired[int],
+        "Ipv6Addresses": NotRequired[
+            List[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef]
+        ],
+        "Ipv6PrefixCount": NotRequired[int],
+        "Ipv6Prefixes": NotRequired[
+            List[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef]
+        ],
+        "NetworkCardIndex": NotRequired[int],
+        "NetworkInterfaceId": NotRequired[str],
+        "PrivateIpAddress": NotRequired[str],
+        "PrivateIpAddresses": NotRequired[
+            List[AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef]
+        ],
+        "SecondaryPrivateIpAddressCount": NotRequired[int],
+        "SubnetId": NotRequired[str],
+    },
+)
+AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef",
     {
         "AssociateCarrierIpAddress": NotRequired[bool],
         "AssociatePublicIpAddress": NotRequired[bool],
         "DeleteOnTermination": NotRequired[bool],
         "Description": NotRequired[str],
         "DeviceIndex": NotRequired[int],
         "Groups": NotRequired[List[str]],
@@ -5932,16 +6856,31 @@
         "Ipv6CidrBlock": NotRequired[str],
         "PortRange": NotRequired[PortRangeFromToTypeDef],
         "Protocol": NotRequired[str],
         "RuleAction": NotRequired[str],
         "RuleNumber": NotRequired[int],
     },
 )
-AwsEc2NetworkInterfaceDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2NetworkInterfaceDetailsPaginatorTypeDef",
+AwsEc2NetworkInterfaceDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2NetworkInterfaceDetailsExtraOutputTypeDef",
+    {
+        "Attachment": NotRequired[AwsEc2NetworkInterfaceAttachmentTypeDef],
+        "NetworkInterfaceId": NotRequired[str],
+        "SecurityGroups": NotRequired[List[AwsEc2NetworkInterfaceSecurityGroupTypeDef]],
+        "SourceDestCheck": NotRequired[bool],
+        "IpV6Addresses": NotRequired[List[AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef]],
+        "PrivateIpAddresses": NotRequired[
+            List[AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef]
+        ],
+        "PublicDnsName": NotRequired[str],
+        "PublicIp": NotRequired[str],
+    },
+)
+AwsEc2NetworkInterfaceDetailsOutputTypeDef = TypedDict(
+    "AwsEc2NetworkInterfaceDetailsOutputTypeDef",
     {
         "Attachment": NotRequired[AwsEc2NetworkInterfaceAttachmentTypeDef],
         "NetworkInterfaceId": NotRequired[str],
         "SecurityGroups": NotRequired[List[AwsEc2NetworkInterfaceSecurityGroupTypeDef]],
         "SourceDestCheck": NotRequired[bool],
         "IpV6Addresses": NotRequired[List[AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef]],
         "PrivateIpAddresses": NotRequired[
@@ -5962,16 +6901,28 @@
         "PrivateIpAddresses": NotRequired[
             Sequence[AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef]
         ],
         "PublicDnsName": NotRequired[str],
         "PublicIp": NotRequired[str],
     },
 )
-AwsEc2SecurityGroupIpPermissionPaginatorTypeDef = TypedDict(
-    "AwsEc2SecurityGroupIpPermissionPaginatorTypeDef",
+AwsEc2SecurityGroupIpPermissionExtraOutputTypeDef = TypedDict(
+    "AwsEc2SecurityGroupIpPermissionExtraOutputTypeDef",
+    {
+        "IpProtocol": NotRequired[str],
+        "FromPort": NotRequired[int],
+        "ToPort": NotRequired[int],
+        "UserIdGroupPairs": NotRequired[List[AwsEc2SecurityGroupUserIdGroupPairTypeDef]],
+        "IpRanges": NotRequired[List[AwsEc2SecurityGroupIpRangeTypeDef]],
+        "Ipv6Ranges": NotRequired[List[AwsEc2SecurityGroupIpv6RangeTypeDef]],
+        "PrefixListIds": NotRequired[List[AwsEc2SecurityGroupPrefixListIdTypeDef]],
+    },
+)
+AwsEc2SecurityGroupIpPermissionOutputTypeDef = TypedDict(
+    "AwsEc2SecurityGroupIpPermissionOutputTypeDef",
     {
         "IpProtocol": NotRequired[str],
         "FromPort": NotRequired[int],
         "ToPort": NotRequired[int],
         "UserIdGroupPairs": NotRequired[List[AwsEc2SecurityGroupUserIdGroupPairTypeDef]],
         "IpRanges": NotRequired[List[AwsEc2SecurityGroupIpRangeTypeDef]],
         "Ipv6Ranges": NotRequired[List[AwsEc2SecurityGroupIpv6RangeTypeDef]],
@@ -5986,16 +6937,34 @@
         "ToPort": NotRequired[int],
         "UserIdGroupPairs": NotRequired[Sequence[AwsEc2SecurityGroupUserIdGroupPairTypeDef]],
         "IpRanges": NotRequired[Sequence[AwsEc2SecurityGroupIpRangeTypeDef]],
         "Ipv6Ranges": NotRequired[Sequence[AwsEc2SecurityGroupIpv6RangeTypeDef]],
         "PrefixListIds": NotRequired[Sequence[AwsEc2SecurityGroupPrefixListIdTypeDef]],
     },
 )
-AwsEc2SubnetDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2SubnetDetailsPaginatorTypeDef",
+AwsEc2SubnetDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2SubnetDetailsExtraOutputTypeDef",
+    {
+        "AssignIpv6AddressOnCreation": NotRequired[bool],
+        "AvailabilityZone": NotRequired[str],
+        "AvailabilityZoneId": NotRequired[str],
+        "AvailableIpAddressCount": NotRequired[int],
+        "CidrBlock": NotRequired[str],
+        "DefaultForAz": NotRequired[bool],
+        "MapPublicIpOnLaunch": NotRequired[bool],
+        "OwnerId": NotRequired[str],
+        "State": NotRequired[str],
+        "SubnetArn": NotRequired[str],
+        "SubnetId": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "Ipv6CidrBlockAssociationSet": NotRequired[List[Ipv6CidrBlockAssociationTypeDef]],
+    },
+)
+AwsEc2SubnetDetailsOutputTypeDef = TypedDict(
+    "AwsEc2SubnetDetailsOutputTypeDef",
     {
         "AssignIpv6AddressOnCreation": NotRequired[bool],
         "AvailabilityZone": NotRequired[str],
         "AvailabilityZoneId": NotRequired[str],
         "AvailableIpAddressCount": NotRequired[int],
         "CidrBlock": NotRequired[str],
         "DefaultForAz": NotRequired[bool],
@@ -6022,16 +6991,32 @@
         "State": NotRequired[str],
         "SubnetArn": NotRequired[str],
         "SubnetId": NotRequired[str],
         "VpcId": NotRequired[str],
         "Ipv6CidrBlockAssociationSet": NotRequired[Sequence[Ipv6CidrBlockAssociationTypeDef]],
     },
 )
-AwsEc2VolumeDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VolumeDetailsPaginatorTypeDef",
+AwsEc2VolumeDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VolumeDetailsExtraOutputTypeDef",
+    {
+        "CreateTime": NotRequired[str],
+        "DeviceName": NotRequired[str],
+        "Encrypted": NotRequired[bool],
+        "Size": NotRequired[int],
+        "SnapshotId": NotRequired[str],
+        "Status": NotRequired[str],
+        "KmsKeyId": NotRequired[str],
+        "Attachments": NotRequired[List[AwsEc2VolumeAttachmentTypeDef]],
+        "VolumeId": NotRequired[str],
+        "VolumeType": NotRequired[str],
+        "VolumeScanStatus": NotRequired[str],
+    },
+)
+AwsEc2VolumeDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VolumeDetailsOutputTypeDef",
     {
         "CreateTime": NotRequired[str],
         "DeviceName": NotRequired[str],
         "Encrypted": NotRequired[bool],
         "Size": NotRequired[int],
         "SnapshotId": NotRequired[str],
         "Status": NotRequired[str],
@@ -6054,16 +7039,25 @@
         "KmsKeyId": NotRequired[str],
         "Attachments": NotRequired[Sequence[AwsEc2VolumeAttachmentTypeDef]],
         "VolumeId": NotRequired[str],
         "VolumeType": NotRequired[str],
         "VolumeScanStatus": NotRequired[str],
     },
 )
-AwsEc2VpcDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VpcDetailsPaginatorTypeDef",
+AwsEc2VpcDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VpcDetailsExtraOutputTypeDef",
+    {
+        "CidrBlockAssociationSet": NotRequired[List[CidrBlockAssociationTypeDef]],
+        "Ipv6CidrBlockAssociationSet": NotRequired[List[Ipv6CidrBlockAssociationTypeDef]],
+        "DhcpOptionsId": NotRequired[str],
+        "State": NotRequired[str],
+    },
+)
+AwsEc2VpcDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcDetailsOutputTypeDef",
     {
         "CidrBlockAssociationSet": NotRequired[List[CidrBlockAssociationTypeDef]],
         "Ipv6CidrBlockAssociationSet": NotRequired[List[Ipv6CidrBlockAssociationTypeDef]],
         "DhcpOptionsId": NotRequired[str],
         "State": NotRequired[str],
     },
 )
@@ -6072,16 +7066,32 @@
     {
         "CidrBlockAssociationSet": NotRequired[Sequence[CidrBlockAssociationTypeDef]],
         "Ipv6CidrBlockAssociationSet": NotRequired[Sequence[Ipv6CidrBlockAssociationTypeDef]],
         "DhcpOptionsId": NotRequired[str],
         "State": NotRequired[str],
     },
 )
-AwsEc2VpcEndpointServiceDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VpcEndpointServiceDetailsPaginatorTypeDef",
+AwsEc2VpcEndpointServiceDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VpcEndpointServiceDetailsExtraOutputTypeDef",
+    {
+        "AcceptanceRequired": NotRequired[bool],
+        "AvailabilityZones": NotRequired[List[str]],
+        "BaseEndpointDnsNames": NotRequired[List[str]],
+        "ManagesVpcEndpoints": NotRequired[bool],
+        "GatewayLoadBalancerArns": NotRequired[List[str]],
+        "NetworkLoadBalancerArns": NotRequired[List[str]],
+        "PrivateDnsName": NotRequired[str],
+        "ServiceId": NotRequired[str],
+        "ServiceName": NotRequired[str],
+        "ServiceState": NotRequired[str],
+        "ServiceType": NotRequired[List[AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef]],
+    },
+)
+AwsEc2VpcEndpointServiceDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcEndpointServiceDetailsOutputTypeDef",
     {
         "AcceptanceRequired": NotRequired[bool],
         "AvailabilityZones": NotRequired[List[str]],
         "BaseEndpointDnsNames": NotRequired[List[str]],
         "ManagesVpcEndpoints": NotRequired[bool],
         "GatewayLoadBalancerArns": NotRequired[List[str]],
         "NetworkLoadBalancerArns": NotRequired[List[str]],
@@ -6104,16 +7114,28 @@
         "PrivateDnsName": NotRequired[str],
         "ServiceId": NotRequired[str],
         "ServiceName": NotRequired[str],
         "ServiceState": NotRequired[str],
         "ServiceType": NotRequired[Sequence[AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef]],
     },
 )
-AwsEc2VpcPeeringConnectionVpcInfoDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VpcPeeringConnectionVpcInfoDetailsPaginatorTypeDef",
+AwsEc2VpcPeeringConnectionVpcInfoDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VpcPeeringConnectionVpcInfoDetailsExtraOutputTypeDef",
+    {
+        "CidrBlock": NotRequired[str],
+        "CidrBlockSet": NotRequired[List[VpcInfoCidrBlockSetDetailsTypeDef]],
+        "Ipv6CidrBlockSet": NotRequired[List[VpcInfoIpv6CidrBlockSetDetailsTypeDef]],
+        "OwnerId": NotRequired[str],
+        "PeeringOptions": NotRequired[VpcInfoPeeringOptionsDetailsTypeDef],
+        "Region": NotRequired[str],
+        "VpcId": NotRequired[str],
+    },
+)
+AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef",
     {
         "CidrBlock": NotRequired[str],
         "CidrBlockSet": NotRequired[List[VpcInfoCidrBlockSetDetailsTypeDef]],
         "Ipv6CidrBlockSet": NotRequired[List[VpcInfoIpv6CidrBlockSetDetailsTypeDef]],
         "OwnerId": NotRequired[str],
         "PeeringOptions": NotRequired[VpcInfoPeeringOptionsDetailsTypeDef],
         "Region": NotRequired[str],
@@ -6128,20 +7150,29 @@
         "Ipv6CidrBlockSet": NotRequired[Sequence[VpcInfoIpv6CidrBlockSetDetailsTypeDef]],
         "OwnerId": NotRequired[str],
         "PeeringOptions": NotRequired[VpcInfoPeeringOptionsDetailsTypeDef],
         "Region": NotRequired[str],
         "VpcId": NotRequired[str],
     },
 )
-AwsEc2VpnConnectionOptionsDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VpnConnectionOptionsDetailsPaginatorTypeDef",
+AwsEc2VpnConnectionOptionsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionOptionsDetailsExtraOutputTypeDef",
     {
         "StaticRoutesOnly": NotRequired[bool],
         "TunnelOptions": NotRequired[
-            List[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsPaginatorTypeDef]
+            List[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsExtraOutputTypeDef]
+        ],
+    },
+)
+AwsEc2VpnConnectionOptionsDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionOptionsDetailsOutputTypeDef",
+    {
+        "StaticRoutesOnly": NotRequired[bool],
+        "TunnelOptions": NotRequired[
+            List[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef]
         ],
     },
 )
 AwsEc2VpnConnectionOptionsDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionOptionsDetailsTypeDef",
     {
         "StaticRoutesOnly": NotRequired[bool],
@@ -6169,16 +7200,25 @@
         "KmsKeyId": NotRequired[str],
         "LogConfiguration": NotRequired[
             AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef
         ],
         "Logging": NotRequired[str],
     },
 )
-AwsEcsContainerDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsContainerDetailsPaginatorTypeDef",
+AwsEcsContainerDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsContainerDetailsExtraOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "Image": NotRequired[str],
+        "MountPoints": NotRequired[List[AwsMountPointTypeDef]],
+        "Privileged": NotRequired[bool],
+    },
+)
+AwsEcsContainerDetailsOutputTypeDef = TypedDict(
+    "AwsEcsContainerDetailsOutputTypeDef",
     {
         "Name": NotRequired[str],
         "Image": NotRequired[str],
         "MountPoints": NotRequired[List[AwsMountPointTypeDef]],
         "Privileged": NotRequired[bool],
     },
 )
@@ -6197,52 +7237,78 @@
         "DeploymentCircuitBreaker": NotRequired[
             AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef
         ],
         "MaximumPercent": NotRequired[int],
         "MinimumHealthyPercent": NotRequired[int],
     },
 )
-AwsEcsServiceNetworkConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsServiceNetworkConfigurationDetailsPaginatorTypeDef",
+AwsEcsServiceNetworkConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsServiceNetworkConfigurationDetailsExtraOutputTypeDef",
+    {
+        "AwsVpcConfiguration": NotRequired[
+            AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef",
     {
         "AwsVpcConfiguration": NotRequired[
-            AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsPaginatorTypeDef
+            AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef
         ],
     },
 )
 AwsEcsServiceNetworkConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceNetworkConfigurationDetailsTypeDef",
     {
         "AwsVpcConfiguration": NotRequired[
             AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef
         ],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsExtraOutputTypeDef",
     {
         "Capabilities": NotRequired[
-            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsPaginatorTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsExtraOutputTypeDef
         ],
         "Devices": NotRequired[
             List[
-                AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsPaginatorTypeDef
+                AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsExtraOutputTypeDef
             ]
         ],
         "InitProcessEnabled": NotRequired[bool],
         "MaxSwap": NotRequired[int],
         "SharedMemorySize": NotRequired[int],
         "Swappiness": NotRequired[int],
         "Tmpfs": NotRequired[
             List[
-                AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsPaginatorTypeDef
+                AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsExtraOutputTypeDef
             ]
         ],
     },
 )
+AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef",
+    {
+        "Capabilities": NotRequired[
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef
+        ],
+        "Devices": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef]
+        ],
+        "InitProcessEnabled": NotRequired[bool],
+        "MaxSwap": NotRequired[int],
+        "SharedMemorySize": NotRequired[int],
+        "Swappiness": NotRequired[int],
+        "Tmpfs": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef]
+        ],
+    },
+)
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
     {
         "Capabilities": NotRequired[
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef
         ],
         "Devices": NotRequired[
@@ -6253,16 +7319,28 @@
         "SharedMemorySize": NotRequired[int],
         "Swappiness": NotRequired[int],
         "Tmpfs": NotRequired[
             Sequence[AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef]
         ],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsExtraOutputTypeDef",
+    {
+        "LogDriver": NotRequired[str],
+        "Options": NotRequired[Dict[str, str]],
+        "SecretOptions": NotRequired[
+            List[
+                AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef
+            ]
+        ],
+    },
+)
+AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef",
     {
         "LogDriver": NotRequired[str],
         "Options": NotRequired[Dict[str, str]],
         "SecretOptions": NotRequired[
             List[
                 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef
             ]
@@ -6277,16 +7355,26 @@
         "SecretOptions": NotRequired[
             Sequence[
                 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef
             ]
         ],
     },
 )
-AwsEcsTaskDefinitionProxyConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionProxyConfigurationDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionProxyConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionProxyConfigurationDetailsExtraOutputTypeDef",
+    {
+        "ContainerName": NotRequired[str],
+        "ProxyConfigurationProperties": NotRequired[
+            List[AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef]
+        ],
+        "Type": NotRequired[str],
+    },
+)
+AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef",
     {
         "ContainerName": NotRequired[str],
         "ProxyConfigurationProperties": NotRequired[
             List[AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef]
         ],
         "Type": NotRequired[str],
     },
@@ -6325,30 +7413,57 @@
 AwsEfsAccessPointRootDirectoryDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointRootDirectoryDetailsTypeDef",
     {
         "CreationInfo": NotRequired[AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef],
         "Path": NotRequired[str],
     },
 )
-AwsEksClusterLoggingDetailsPaginatorTypeDef = TypedDict(
-    "AwsEksClusterLoggingDetailsPaginatorTypeDef",
+AwsEksClusterLoggingDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEksClusterLoggingDetailsExtraOutputTypeDef",
     {
         "ClusterLogging": NotRequired[
-            List[AwsEksClusterLoggingClusterLoggingDetailsPaginatorTypeDef]
+            List[AwsEksClusterLoggingClusterLoggingDetailsExtraOutputTypeDef]
         ],
     },
 )
+AwsEksClusterLoggingDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterLoggingDetailsOutputTypeDef",
+    {
+        "ClusterLogging": NotRequired[List[AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef]],
+    },
+)
 AwsEksClusterLoggingDetailsTypeDef = TypedDict(
     "AwsEksClusterLoggingDetailsTypeDef",
     {
         "ClusterLogging": NotRequired[Sequence[AwsEksClusterLoggingClusterLoggingDetailsTypeDef]],
     },
 )
-AwsElasticBeanstalkEnvironmentDetailsPaginatorTypeDef = TypedDict(
-    "AwsElasticBeanstalkEnvironmentDetailsPaginatorTypeDef",
+AwsElasticBeanstalkEnvironmentDetailsExtraOutputTypeDef = TypedDict(
+    "AwsElasticBeanstalkEnvironmentDetailsExtraOutputTypeDef",
+    {
+        "ApplicationName": NotRequired[str],
+        "Cname": NotRequired[str],
+        "DateCreated": NotRequired[str],
+        "DateUpdated": NotRequired[str],
+        "Description": NotRequired[str],
+        "EndpointUrl": NotRequired[str],
+        "EnvironmentArn": NotRequired[str],
+        "EnvironmentId": NotRequired[str],
+        "EnvironmentLinks": NotRequired[List[AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef]],
+        "EnvironmentName": NotRequired[str],
+        "OptionSettings": NotRequired[List[AwsElasticBeanstalkEnvironmentOptionSettingTypeDef]],
+        "PlatformArn": NotRequired[str],
+        "SolutionStackName": NotRequired[str],
+        "Status": NotRequired[str],
+        "Tier": NotRequired[AwsElasticBeanstalkEnvironmentTierTypeDef],
+        "VersionLabel": NotRequired[str],
+    },
+)
+AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef = TypedDict(
+    "AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef",
     {
         "ApplicationName": NotRequired[str],
         "Cname": NotRequired[str],
         "DateCreated": NotRequired[str],
         "DateUpdated": NotRequired[str],
         "Description": NotRequired[str],
         "EndpointUrl": NotRequired[str],
@@ -6405,16 +7520,24 @@
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
     {
         "IndexSlowLogs": NotRequired[AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef],
         "SearchSlowLogs": NotRequired[AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef],
         "AuditLogs": NotRequired[AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef],
     },
 )
-AwsElbLoadBalancerPoliciesPaginatorTypeDef = TypedDict(
-    "AwsElbLoadBalancerPoliciesPaginatorTypeDef",
+AwsElbLoadBalancerPoliciesExtraOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerPoliciesExtraOutputTypeDef",
+    {
+        "AppCookieStickinessPolicies": NotRequired[List[AwsElbAppCookieStickinessPolicyTypeDef]],
+        "LbCookieStickinessPolicies": NotRequired[List[AwsElbLbCookieStickinessPolicyTypeDef]],
+        "OtherPolicies": NotRequired[List[str]],
+    },
+)
+AwsElbLoadBalancerPoliciesOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerPoliciesOutputTypeDef",
     {
         "AppCookieStickinessPolicies": NotRequired[List[AwsElbAppCookieStickinessPolicyTypeDef]],
         "LbCookieStickinessPolicies": NotRequired[List[AwsElbLbCookieStickinessPolicyTypeDef]],
         "OtherPolicies": NotRequired[List[str]],
     },
 )
 AwsElbLoadBalancerPoliciesTypeDef = TypedDict(
@@ -6423,16 +7546,26 @@
         "AppCookieStickinessPolicies": NotRequired[
             Sequence[AwsElbAppCookieStickinessPolicyTypeDef]
         ],
         "LbCookieStickinessPolicies": NotRequired[Sequence[AwsElbLbCookieStickinessPolicyTypeDef]],
         "OtherPolicies": NotRequired[Sequence[str]],
     },
 )
-AwsElbLoadBalancerAttributesPaginatorTypeDef = TypedDict(
-    "AwsElbLoadBalancerAttributesPaginatorTypeDef",
+AwsElbLoadBalancerAttributesExtraOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerAttributesExtraOutputTypeDef",
+    {
+        "AccessLog": NotRequired[AwsElbLoadBalancerAccessLogTypeDef],
+        "ConnectionDraining": NotRequired[AwsElbLoadBalancerConnectionDrainingTypeDef],
+        "ConnectionSettings": NotRequired[AwsElbLoadBalancerConnectionSettingsTypeDef],
+        "CrossZoneLoadBalancing": NotRequired[AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef],
+        "AdditionalAttributes": NotRequired[List[AwsElbLoadBalancerAdditionalAttributeTypeDef]],
+    },
+)
+AwsElbLoadBalancerAttributesOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerAttributesOutputTypeDef",
     {
         "AccessLog": NotRequired[AwsElbLoadBalancerAccessLogTypeDef],
         "ConnectionDraining": NotRequired[AwsElbLoadBalancerConnectionDrainingTypeDef],
         "ConnectionSettings": NotRequired[AwsElbLoadBalancerConnectionSettingsTypeDef],
         "CrossZoneLoadBalancing": NotRequired[AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef],
         "AdditionalAttributes": NotRequired[List[AwsElbLoadBalancerAdditionalAttributeTypeDef]],
     },
@@ -6443,30 +7576,53 @@
         "AccessLog": NotRequired[AwsElbLoadBalancerAccessLogTypeDef],
         "ConnectionDraining": NotRequired[AwsElbLoadBalancerConnectionDrainingTypeDef],
         "ConnectionSettings": NotRequired[AwsElbLoadBalancerConnectionSettingsTypeDef],
         "CrossZoneLoadBalancing": NotRequired[AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef],
         "AdditionalAttributes": NotRequired[Sequence[AwsElbLoadBalancerAdditionalAttributeTypeDef]],
     },
 )
-AwsElbLoadBalancerListenerDescriptionPaginatorTypeDef = TypedDict(
-    "AwsElbLoadBalancerListenerDescriptionPaginatorTypeDef",
+AwsElbLoadBalancerListenerDescriptionExtraOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerListenerDescriptionExtraOutputTypeDef",
+    {
+        "Listener": NotRequired[AwsElbLoadBalancerListenerTypeDef],
+        "PolicyNames": NotRequired[List[str]],
+    },
+)
+AwsElbLoadBalancerListenerDescriptionOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerListenerDescriptionOutputTypeDef",
     {
         "Listener": NotRequired[AwsElbLoadBalancerListenerTypeDef],
         "PolicyNames": NotRequired[List[str]],
     },
 )
 AwsElbLoadBalancerListenerDescriptionTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
     {
         "Listener": NotRequired[AwsElbLoadBalancerListenerTypeDef],
         "PolicyNames": NotRequired[Sequence[str]],
     },
 )
-AwsElbv2LoadBalancerDetailsPaginatorTypeDef = TypedDict(
-    "AwsElbv2LoadBalancerDetailsPaginatorTypeDef",
+AwsElbv2LoadBalancerDetailsExtraOutputTypeDef = TypedDict(
+    "AwsElbv2LoadBalancerDetailsExtraOutputTypeDef",
+    {
+        "AvailabilityZones": NotRequired[List[AvailabilityZoneTypeDef]],
+        "CanonicalHostedZoneId": NotRequired[str],
+        "CreatedTime": NotRequired[str],
+        "DNSName": NotRequired[str],
+        "IpAddressType": NotRequired[str],
+        "Scheme": NotRequired[str],
+        "SecurityGroups": NotRequired[List[str]],
+        "State": NotRequired[LoadBalancerStateTypeDef],
+        "Type": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "LoadBalancerAttributes": NotRequired[List[AwsElbv2LoadBalancerAttributeTypeDef]],
+    },
+)
+AwsElbv2LoadBalancerDetailsOutputTypeDef = TypedDict(
+    "AwsElbv2LoadBalancerDetailsOutputTypeDef",
     {
         "AvailabilityZones": NotRequired[List[AvailabilityZoneTypeDef]],
         "CanonicalHostedZoneId": NotRequired[str],
         "CreatedTime": NotRequired[str],
         "DNSName": NotRequired[str],
         "IpAddressType": NotRequired[str],
         "Scheme": NotRequired[str],
@@ -6519,16 +7675,27 @@
 AwsIamAccessKeySessionContextTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextTypeDef",
     {
         "Attributes": NotRequired[AwsIamAccessKeySessionContextAttributesTypeDef],
         "SessionIssuer": NotRequired[AwsIamAccessKeySessionContextSessionIssuerTypeDef],
     },
 )
-AwsIamGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsIamGroupDetailsPaginatorTypeDef",
+AwsIamGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsIamGroupDetailsExtraOutputTypeDef",
+    {
+        "AttachedManagedPolicies": NotRequired[List[AwsIamAttachedManagedPolicyTypeDef]],
+        "CreateDate": NotRequired[str],
+        "GroupId": NotRequired[str],
+        "GroupName": NotRequired[str],
+        "GroupPolicyList": NotRequired[List[AwsIamGroupPolicyTypeDef]],
+        "Path": NotRequired[str],
+    },
+)
+AwsIamGroupDetailsOutputTypeDef = TypedDict(
+    "AwsIamGroupDetailsOutputTypeDef",
     {
         "AttachedManagedPolicies": NotRequired[List[AwsIamAttachedManagedPolicyTypeDef]],
         "CreateDate": NotRequired[str],
         "GroupId": NotRequired[str],
         "GroupName": NotRequired[str],
         "GroupPolicyList": NotRequired[List[AwsIamGroupPolicyTypeDef]],
         "Path": NotRequired[str],
@@ -6541,16 +7708,27 @@
         "CreateDate": NotRequired[str],
         "GroupId": NotRequired[str],
         "GroupName": NotRequired[str],
         "GroupPolicyList": NotRequired[Sequence[AwsIamGroupPolicyTypeDef]],
         "Path": NotRequired[str],
     },
 )
-AwsIamInstanceProfilePaginatorTypeDef = TypedDict(
-    "AwsIamInstanceProfilePaginatorTypeDef",
+AwsIamInstanceProfileExtraOutputTypeDef = TypedDict(
+    "AwsIamInstanceProfileExtraOutputTypeDef",
+    {
+        "Arn": NotRequired[str],
+        "CreateDate": NotRequired[str],
+        "InstanceProfileId": NotRequired[str],
+        "InstanceProfileName": NotRequired[str],
+        "Path": NotRequired[str],
+        "Roles": NotRequired[List[AwsIamInstanceProfileRoleTypeDef]],
+    },
+)
+AwsIamInstanceProfileOutputTypeDef = TypedDict(
+    "AwsIamInstanceProfileOutputTypeDef",
     {
         "Arn": NotRequired[str],
         "CreateDate": NotRequired[str],
         "InstanceProfileId": NotRequired[str],
         "InstanceProfileName": NotRequired[str],
         "Path": NotRequired[str],
         "Roles": NotRequired[List[AwsIamInstanceProfileRoleTypeDef]],
@@ -6563,16 +7741,32 @@
         "CreateDate": NotRequired[str],
         "InstanceProfileId": NotRequired[str],
         "InstanceProfileName": NotRequired[str],
         "Path": NotRequired[str],
         "Roles": NotRequired[Sequence[AwsIamInstanceProfileRoleTypeDef]],
     },
 )
-AwsIamPolicyDetailsPaginatorTypeDef = TypedDict(
-    "AwsIamPolicyDetailsPaginatorTypeDef",
+AwsIamPolicyDetailsExtraOutputTypeDef = TypedDict(
+    "AwsIamPolicyDetailsExtraOutputTypeDef",
+    {
+        "AttachmentCount": NotRequired[int],
+        "CreateDate": NotRequired[str],
+        "DefaultVersionId": NotRequired[str],
+        "Description": NotRequired[str],
+        "IsAttachable": NotRequired[bool],
+        "Path": NotRequired[str],
+        "PermissionsBoundaryUsageCount": NotRequired[int],
+        "PolicyId": NotRequired[str],
+        "PolicyName": NotRequired[str],
+        "PolicyVersionList": NotRequired[List[AwsIamPolicyVersionTypeDef]],
+        "UpdateDate": NotRequired[str],
+    },
+)
+AwsIamPolicyDetailsOutputTypeDef = TypedDict(
+    "AwsIamPolicyDetailsOutputTypeDef",
     {
         "AttachmentCount": NotRequired[int],
         "CreateDate": NotRequired[str],
         "DefaultVersionId": NotRequired[str],
         "Description": NotRequired[str],
         "IsAttachable": NotRequired[bool],
         "Path": NotRequired[str],
@@ -6595,16 +7789,29 @@
         "PermissionsBoundaryUsageCount": NotRequired[int],
         "PolicyId": NotRequired[str],
         "PolicyName": NotRequired[str],
         "PolicyVersionList": NotRequired[Sequence[AwsIamPolicyVersionTypeDef]],
         "UpdateDate": NotRequired[str],
     },
 )
-AwsIamUserDetailsPaginatorTypeDef = TypedDict(
-    "AwsIamUserDetailsPaginatorTypeDef",
+AwsIamUserDetailsExtraOutputTypeDef = TypedDict(
+    "AwsIamUserDetailsExtraOutputTypeDef",
+    {
+        "AttachedManagedPolicies": NotRequired[List[AwsIamAttachedManagedPolicyTypeDef]],
+        "CreateDate": NotRequired[str],
+        "GroupList": NotRequired[List[str]],
+        "Path": NotRequired[str],
+        "PermissionsBoundary": NotRequired[AwsIamPermissionsBoundaryTypeDef],
+        "UserId": NotRequired[str],
+        "UserName": NotRequired[str],
+        "UserPolicyList": NotRequired[List[AwsIamUserPolicyTypeDef]],
+    },
+)
+AwsIamUserDetailsOutputTypeDef = TypedDict(
+    "AwsIamUserDetailsOutputTypeDef",
     {
         "AttachedManagedPolicies": NotRequired[List[AwsIamAttachedManagedPolicyTypeDef]],
         "CreateDate": NotRequired[str],
         "GroupList": NotRequired[List[str]],
         "Path": NotRequired[str],
         "PermissionsBoundary": NotRequired[AwsIamPermissionsBoundaryTypeDef],
         "UserId": NotRequired[str],
@@ -6631,16 +7838,23 @@
         "Name": NotRequired[str],
         "Arn": NotRequired[str],
         "StreamEncryption": NotRequired[AwsKinesisStreamStreamEncryptionDetailsTypeDef],
         "ShardCount": NotRequired[int],
         "RetentionPeriodHours": NotRequired[int],
     },
 )
-AwsLambdaFunctionEnvironmentPaginatorTypeDef = TypedDict(
-    "AwsLambdaFunctionEnvironmentPaginatorTypeDef",
+AwsLambdaFunctionEnvironmentExtraOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionEnvironmentExtraOutputTypeDef",
+    {
+        "Variables": NotRequired[Dict[str, str]],
+        "Error": NotRequired[AwsLambdaFunctionEnvironmentErrorTypeDef],
+    },
+)
+AwsLambdaFunctionEnvironmentOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionEnvironmentOutputTypeDef",
     {
         "Variables": NotRequired[Dict[str, str]],
         "Error": NotRequired[AwsLambdaFunctionEnvironmentErrorTypeDef],
     },
 )
 AwsLambdaFunctionEnvironmentTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentTypeDef",
@@ -6663,16 +7877,31 @@
             AwsMskClusterClusterInfoEncryptionInfoEncryptionInTransitDetailsTypeDef
         ],
         "EncryptionAtRest": NotRequired[
             AwsMskClusterClusterInfoEncryptionInfoEncryptionAtRestDetailsTypeDef
         ],
     },
 )
-AwsNetworkFirewallFirewallDetailsPaginatorTypeDef = TypedDict(
-    "AwsNetworkFirewallFirewallDetailsPaginatorTypeDef",
+AwsNetworkFirewallFirewallDetailsExtraOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallFirewallDetailsExtraOutputTypeDef",
+    {
+        "DeleteProtection": NotRequired[bool],
+        "Description": NotRequired[str],
+        "FirewallArn": NotRequired[str],
+        "FirewallId": NotRequired[str],
+        "FirewallName": NotRequired[str],
+        "FirewallPolicyArn": NotRequired[str],
+        "FirewallPolicyChangeProtection": NotRequired[bool],
+        "SubnetChangeProtection": NotRequired[bool],
+        "SubnetMappings": NotRequired[List[AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef]],
+        "VpcId": NotRequired[str],
+    },
+)
+AwsNetworkFirewallFirewallDetailsOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallFirewallDetailsOutputTypeDef",
     {
         "DeleteProtection": NotRequired[bool],
         "Description": NotRequired[str],
         "FirewallArn": NotRequired[str],
         "FirewallId": NotRequired[str],
         "FirewallName": NotRequired[str],
         "FirewallPolicyArn": NotRequired[str],
@@ -6728,16 +7957,61 @@
     "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef",
     {
         "IndexSlowLogs": NotRequired[AwsOpenSearchServiceDomainLogPublishingOptionTypeDef],
         "SearchSlowLogs": NotRequired[AwsOpenSearchServiceDomainLogPublishingOptionTypeDef],
         "AuditLogs": NotRequired[AwsOpenSearchServiceDomainLogPublishingOptionTypeDef],
     },
 )
-AwsRdsDbClusterDetailsPaginatorTypeDef = TypedDict(
-    "AwsRdsDbClusterDetailsPaginatorTypeDef",
+AwsRdsDbClusterDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterDetailsExtraOutputTypeDef",
+    {
+        "AllocatedStorage": NotRequired[int],
+        "AvailabilityZones": NotRequired[List[str]],
+        "BackupRetentionPeriod": NotRequired[int],
+        "DatabaseName": NotRequired[str],
+        "Status": NotRequired[str],
+        "Endpoint": NotRequired[str],
+        "ReaderEndpoint": NotRequired[str],
+        "CustomEndpoints": NotRequired[List[str]],
+        "MultiAz": NotRequired[bool],
+        "Engine": NotRequired[str],
+        "EngineVersion": NotRequired[str],
+        "Port": NotRequired[int],
+        "MasterUsername": NotRequired[str],
+        "PreferredBackupWindow": NotRequired[str],
+        "PreferredMaintenanceWindow": NotRequired[str],
+        "ReadReplicaIdentifiers": NotRequired[List[str]],
+        "VpcSecurityGroups": NotRequired[List[AwsRdsDbInstanceVpcSecurityGroupTypeDef]],
+        "HostedZoneId": NotRequired[str],
+        "StorageEncrypted": NotRequired[bool],
+        "KmsKeyId": NotRequired[str],
+        "DbClusterResourceId": NotRequired[str],
+        "AssociatedRoles": NotRequired[List[AwsRdsDbClusterAssociatedRoleTypeDef]],
+        "ClusterCreateTime": NotRequired[str],
+        "EnabledCloudWatchLogsExports": NotRequired[List[str]],
+        "EngineMode": NotRequired[str],
+        "DeletionProtection": NotRequired[bool],
+        "HttpEndpointEnabled": NotRequired[bool],
+        "ActivityStreamStatus": NotRequired[str],
+        "CopyTagsToSnapshot": NotRequired[bool],
+        "CrossAccountClone": NotRequired[bool],
+        "DomainMemberships": NotRequired[List[AwsRdsDbDomainMembershipTypeDef]],
+        "DbClusterParameterGroup": NotRequired[str],
+        "DbSubnetGroup": NotRequired[str],
+        "DbClusterOptionGroupMemberships": NotRequired[
+            List[AwsRdsDbClusterOptionGroupMembershipTypeDef]
+        ],
+        "DbClusterIdentifier": NotRequired[str],
+        "DbClusterMembers": NotRequired[List[AwsRdsDbClusterMemberTypeDef]],
+        "IamDatabaseAuthenticationEnabled": NotRequired[bool],
+        "AutoMinorVersionUpgrade": NotRequired[bool],
+    },
+)
+AwsRdsDbClusterDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterDetailsOutputTypeDef",
     {
         "AllocatedStorage": NotRequired[int],
         "AvailabilityZones": NotRequired[List[str]],
         "BackupRetentionPeriod": NotRequired[int],
         "DatabaseName": NotRequired[str],
         "Status": NotRequired[str],
         "Endpoint": NotRequired[str],
@@ -6818,16 +8092,16 @@
         ],
         "DbClusterIdentifier": NotRequired[str],
         "DbClusterMembers": NotRequired[Sequence[AwsRdsDbClusterMemberTypeDef]],
         "IamDatabaseAuthenticationEnabled": NotRequired[bool],
         "AutoMinorVersionUpgrade": NotRequired[bool],
     },
 )
-AwsRdsDbClusterSnapshotDetailsPaginatorTypeDef = TypedDict(
-    "AwsRdsDbClusterSnapshotDetailsPaginatorTypeDef",
+AwsRdsDbClusterSnapshotDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterSnapshotDetailsExtraOutputTypeDef",
     {
         "AvailabilityZones": NotRequired[List[str]],
         "SnapshotCreateTime": NotRequired[str],
         "Engine": NotRequired[str],
         "AllocatedStorage": NotRequired[int],
         "Status": NotRequired[str],
         "Port": NotRequired[int],
@@ -6840,15 +8114,41 @@
         "PercentProgress": NotRequired[int],
         "StorageEncrypted": NotRequired[bool],
         "KmsKeyId": NotRequired[str],
         "DbClusterIdentifier": NotRequired[str],
         "DbClusterSnapshotIdentifier": NotRequired[str],
         "IamDatabaseAuthenticationEnabled": NotRequired[bool],
         "DbClusterSnapshotAttributes": NotRequired[
-            List[AwsRdsDbClusterSnapshotDbClusterSnapshotAttributePaginatorTypeDef]
+            List[AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeExtraOutputTypeDef]
+        ],
+    },
+)
+AwsRdsDbClusterSnapshotDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbClusterSnapshotDetailsOutputTypeDef",
+    {
+        "AvailabilityZones": NotRequired[List[str]],
+        "SnapshotCreateTime": NotRequired[str],
+        "Engine": NotRequired[str],
+        "AllocatedStorage": NotRequired[int],
+        "Status": NotRequired[str],
+        "Port": NotRequired[int],
+        "VpcId": NotRequired[str],
+        "ClusterCreateTime": NotRequired[str],
+        "MasterUsername": NotRequired[str],
+        "EngineVersion": NotRequired[str],
+        "LicenseModel": NotRequired[str],
+        "SnapshotType": NotRequired[str],
+        "PercentProgress": NotRequired[int],
+        "StorageEncrypted": NotRequired[bool],
+        "KmsKeyId": NotRequired[str],
+        "DbClusterIdentifier": NotRequired[str],
+        "DbClusterSnapshotIdentifier": NotRequired[str],
+        "IamDatabaseAuthenticationEnabled": NotRequired[bool],
+        "DbClusterSnapshotAttributes": NotRequired[
+            List[AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef]
         ],
     },
 )
 AwsRdsDbClusterSnapshotDetailsTypeDef = TypedDict(
     "AwsRdsDbClusterSnapshotDetailsTypeDef",
     {
         "AvailabilityZones": NotRequired[Sequence[str]],
@@ -6870,16 +8170,48 @@
         "DbClusterSnapshotIdentifier": NotRequired[str],
         "IamDatabaseAuthenticationEnabled": NotRequired[bool],
         "DbClusterSnapshotAttributes": NotRequired[
             Sequence[AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef]
         ],
     },
 )
-AwsRdsDbSnapshotDetailsPaginatorTypeDef = TypedDict(
-    "AwsRdsDbSnapshotDetailsPaginatorTypeDef",
+AwsRdsDbSnapshotDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbSnapshotDetailsExtraOutputTypeDef",
+    {
+        "DbSnapshotIdentifier": NotRequired[str],
+        "DbInstanceIdentifier": NotRequired[str],
+        "SnapshotCreateTime": NotRequired[str],
+        "Engine": NotRequired[str],
+        "AllocatedStorage": NotRequired[int],
+        "Status": NotRequired[str],
+        "Port": NotRequired[int],
+        "AvailabilityZone": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "InstanceCreateTime": NotRequired[str],
+        "MasterUsername": NotRequired[str],
+        "EngineVersion": NotRequired[str],
+        "LicenseModel": NotRequired[str],
+        "SnapshotType": NotRequired[str],
+        "Iops": NotRequired[int],
+        "OptionGroupName": NotRequired[str],
+        "PercentProgress": NotRequired[int],
+        "SourceRegion": NotRequired[str],
+        "SourceDbSnapshotIdentifier": NotRequired[str],
+        "StorageType": NotRequired[str],
+        "TdeCredentialArn": NotRequired[str],
+        "Encrypted": NotRequired[bool],
+        "KmsKeyId": NotRequired[str],
+        "Timezone": NotRequired[str],
+        "IamDatabaseAuthenticationEnabled": NotRequired[bool],
+        "ProcessorFeatures": NotRequired[List[AwsRdsDbProcessorFeatureTypeDef]],
+        "DbiResourceId": NotRequired[str],
+    },
+)
+AwsRdsDbSnapshotDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbSnapshotDetailsOutputTypeDef",
     {
         "DbSnapshotIdentifier": NotRequired[str],
         "DbInstanceIdentifier": NotRequired[str],
         "SnapshotCreateTime": NotRequired[str],
         "Engine": NotRequired[str],
         "AllocatedStorage": NotRequired[int],
         "Status": NotRequired[str],
@@ -6934,16 +8266,16 @@
         "KmsKeyId": NotRequired[str],
         "Timezone": NotRequired[str],
         "IamDatabaseAuthenticationEnabled": NotRequired[bool],
         "ProcessorFeatures": NotRequired[Sequence[AwsRdsDbProcessorFeatureTypeDef]],
         "DbiResourceId": NotRequired[str],
     },
 )
-AwsRdsDbPendingModifiedValuesPaginatorTypeDef = TypedDict(
-    "AwsRdsDbPendingModifiedValuesPaginatorTypeDef",
+AwsRdsDbPendingModifiedValuesExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbPendingModifiedValuesExtraOutputTypeDef",
     {
         "DbInstanceClass": NotRequired[str],
         "AllocatedStorage": NotRequired[int],
         "MasterUserPassword": NotRequired[str],
         "Port": NotRequired[int],
         "BackupRetentionPeriod": NotRequired[int],
         "MultiAZ": NotRequired[bool],
@@ -6951,15 +8283,37 @@
         "LicenseModel": NotRequired[str],
         "Iops": NotRequired[int],
         "DbInstanceIdentifier": NotRequired[str],
         "StorageType": NotRequired[str],
         "CaCertificateIdentifier": NotRequired[str],
         "DbSubnetGroupName": NotRequired[str],
         "PendingCloudWatchLogsExports": NotRequired[
-            AwsRdsPendingCloudWatchLogsExportsPaginatorTypeDef
+            AwsRdsPendingCloudWatchLogsExportsExtraOutputTypeDef
+        ],
+        "ProcessorFeatures": NotRequired[List[AwsRdsDbProcessorFeatureTypeDef]],
+    },
+)
+AwsRdsDbPendingModifiedValuesOutputTypeDef = TypedDict(
+    "AwsRdsDbPendingModifiedValuesOutputTypeDef",
+    {
+        "DbInstanceClass": NotRequired[str],
+        "AllocatedStorage": NotRequired[int],
+        "MasterUserPassword": NotRequired[str],
+        "Port": NotRequired[int],
+        "BackupRetentionPeriod": NotRequired[int],
+        "MultiAZ": NotRequired[bool],
+        "EngineVersion": NotRequired[str],
+        "LicenseModel": NotRequired[str],
+        "Iops": NotRequired[int],
+        "DbInstanceIdentifier": NotRequired[str],
+        "StorageType": NotRequired[str],
+        "CaCertificateIdentifier": NotRequired[str],
+        "DbSubnetGroupName": NotRequired[str],
+        "PendingCloudWatchLogsExports": NotRequired[
+            AwsRdsPendingCloudWatchLogsExportsOutputTypeDef
         ],
         "ProcessorFeatures": NotRequired[List[AwsRdsDbProcessorFeatureTypeDef]],
     },
 )
 AwsRdsDbPendingModifiedValuesTypeDef = TypedDict(
     "AwsRdsDbPendingModifiedValuesTypeDef",
     {
@@ -6976,16 +8330,28 @@
         "StorageType": NotRequired[str],
         "CaCertificateIdentifier": NotRequired[str],
         "DbSubnetGroupName": NotRequired[str],
         "PendingCloudWatchLogsExports": NotRequired[AwsRdsPendingCloudWatchLogsExportsTypeDef],
         "ProcessorFeatures": NotRequired[Sequence[AwsRdsDbProcessorFeatureTypeDef]],
     },
 )
-AwsRdsDbSecurityGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsRdsDbSecurityGroupDetailsPaginatorTypeDef",
+AwsRdsDbSecurityGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbSecurityGroupDetailsExtraOutputTypeDef",
+    {
+        "DbSecurityGroupArn": NotRequired[str],
+        "DbSecurityGroupDescription": NotRequired[str],
+        "DbSecurityGroupName": NotRequired[str],
+        "Ec2SecurityGroups": NotRequired[List[AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef]],
+        "IpRanges": NotRequired[List[AwsRdsDbSecurityGroupIpRangeTypeDef]],
+        "OwnerId": NotRequired[str],
+        "VpcId": NotRequired[str],
+    },
+)
+AwsRdsDbSecurityGroupDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbSecurityGroupDetailsOutputTypeDef",
     {
         "DbSecurityGroupArn": NotRequired[str],
         "DbSecurityGroupDescription": NotRequired[str],
         "DbSecurityGroupName": NotRequired[str],
         "Ec2SecurityGroups": NotRequired[List[AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef]],
         "IpRanges": NotRequired[List[AwsRdsDbSecurityGroupIpRangeTypeDef]],
         "OwnerId": NotRequired[str],
@@ -7008,16 +8374,26 @@
     "AwsRdsDbSubnetGroupSubnetTypeDef",
     {
         "SubnetIdentifier": NotRequired[str],
         "SubnetAvailabilityZone": NotRequired[AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef],
         "SubnetStatus": NotRequired[str],
     },
 )
-AwsRedshiftClusterClusterParameterGroupPaginatorTypeDef = TypedDict(
-    "AwsRedshiftClusterClusterParameterGroupPaginatorTypeDef",
+AwsRedshiftClusterClusterParameterGroupExtraOutputTypeDef = TypedDict(
+    "AwsRedshiftClusterClusterParameterGroupExtraOutputTypeDef",
+    {
+        "ClusterParameterStatusList": NotRequired[
+            List[AwsRedshiftClusterClusterParameterStatusTypeDef]
+        ],
+        "ParameterApplyStatus": NotRequired[str],
+        "ParameterGroupName": NotRequired[str],
+    },
+)
+AwsRedshiftClusterClusterParameterGroupOutputTypeDef = TypedDict(
+    "AwsRedshiftClusterClusterParameterGroupOutputTypeDef",
     {
         "ClusterParameterStatusList": NotRequired[
             List[AwsRedshiftClusterClusterParameterStatusTypeDef]
         ],
         "ParameterApplyStatus": NotRequired[str],
         "ParameterGroupName": NotRequired[str],
     },
@@ -7065,16 +8441,24 @@
         "Prefix": NotRequired[str],
         "Tag": NotRequired[
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef
         ],
         "Type": NotRequired[str],
     },
 )
-AwsS3BucketNotificationConfigurationS3KeyFilterPaginatorTypeDef = TypedDict(
-    "AwsS3BucketNotificationConfigurationS3KeyFilterPaginatorTypeDef",
+AwsS3BucketNotificationConfigurationS3KeyFilterExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationS3KeyFilterExtraOutputTypeDef",
+    {
+        "FilterRules": NotRequired[
+            List[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef]
+        ],
+    },
+)
+AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef",
     {
         "FilterRules": NotRequired[
             List[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef]
         ],
     },
 )
 AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef = TypedDict(
@@ -7104,16 +8488,43 @@
 AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
     {
         "Condition": NotRequired[AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef],
         "Redirect": NotRequired[AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef],
     },
 )
-AwsSageMakerNotebookInstanceDetailsPaginatorTypeDef = TypedDict(
-    "AwsSageMakerNotebookInstanceDetailsPaginatorTypeDef",
+AwsSageMakerNotebookInstanceDetailsExtraOutputTypeDef = TypedDict(
+    "AwsSageMakerNotebookInstanceDetailsExtraOutputTypeDef",
+    {
+        "AcceleratorTypes": NotRequired[List[str]],
+        "AdditionalCodeRepositories": NotRequired[List[str]],
+        "DefaultCodeRepository": NotRequired[str],
+        "DirectInternetAccess": NotRequired[str],
+        "FailureReason": NotRequired[str],
+        "InstanceMetadataServiceConfiguration": NotRequired[
+            AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef
+        ],
+        "InstanceType": NotRequired[str],
+        "KmsKeyId": NotRequired[str],
+        "NetworkInterfaceId": NotRequired[str],
+        "NotebookInstanceArn": NotRequired[str],
+        "NotebookInstanceLifecycleConfigName": NotRequired[str],
+        "NotebookInstanceName": NotRequired[str],
+        "NotebookInstanceStatus": NotRequired[str],
+        "PlatformIdentifier": NotRequired[str],
+        "RoleArn": NotRequired[str],
+        "RootAccess": NotRequired[str],
+        "SecurityGroups": NotRequired[List[str]],
+        "SubnetId": NotRequired[str],
+        "Url": NotRequired[str],
+        "VolumeSizeInGB": NotRequired[int],
+    },
+)
+AwsSageMakerNotebookInstanceDetailsOutputTypeDef = TypedDict(
+    "AwsSageMakerNotebookInstanceDetailsOutputTypeDef",
     {
         "AcceleratorTypes": NotRequired[List[str]],
         "AdditionalCodeRepositories": NotRequired[List[str]],
         "DefaultCodeRepository": NotRequired[str],
         "DirectInternetAccess": NotRequired[str],
         "FailureReason": NotRequired[str],
         "InstanceMetadataServiceConfiguration": NotRequired[
@@ -7194,16 +8605,32 @@
     "BatchUpdateFindingsUnprocessedFindingTypeDef",
     {
         "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
 )
-AwsSnsTopicDetailsPaginatorTypeDef = TypedDict(
-    "AwsSnsTopicDetailsPaginatorTypeDef",
+AwsSnsTopicDetailsExtraOutputTypeDef = TypedDict(
+    "AwsSnsTopicDetailsExtraOutputTypeDef",
+    {
+        "KmsMasterKeyId": NotRequired[str],
+        "Subscription": NotRequired[List[AwsSnsTopicSubscriptionTypeDef]],
+        "TopicName": NotRequired[str],
+        "Owner": NotRequired[str],
+        "SqsSuccessFeedbackRoleArn": NotRequired[str],
+        "SqsFailureFeedbackRoleArn": NotRequired[str],
+        "ApplicationSuccessFeedbackRoleArn": NotRequired[str],
+        "FirehoseSuccessFeedbackRoleArn": NotRequired[str],
+        "FirehoseFailureFeedbackRoleArn": NotRequired[str],
+        "HttpSuccessFeedbackRoleArn": NotRequired[str],
+        "HttpFailureFeedbackRoleArn": NotRequired[str],
+    },
+)
+AwsSnsTopicDetailsOutputTypeDef = TypedDict(
+    "AwsSnsTopicDetailsOutputTypeDef",
     {
         "KmsMasterKeyId": NotRequired[str],
         "Subscription": NotRequired[List[AwsSnsTopicSubscriptionTypeDef]],
         "TopicName": NotRequired[str],
         "Owner": NotRequired[str],
         "SqsSuccessFeedbackRoleArn": NotRequired[str],
         "SqsFailureFeedbackRoleArn": NotRequired[str],
@@ -7240,16 +8667,27 @@
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
     {
         "CloudWatchLogsLogGroup": NotRequired[
             AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef
         ],
     },
 )
-AwsWafRateBasedRuleDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafRateBasedRuleDetailsPaginatorTypeDef",
+AwsWafRateBasedRuleDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafRateBasedRuleDetailsExtraOutputTypeDef",
+    {
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "RateKey": NotRequired[str],
+        "RateLimit": NotRequired[int],
+        "RuleId": NotRequired[str],
+        "MatchPredicates": NotRequired[List[AwsWafRateBasedRuleMatchPredicateTypeDef]],
+    },
+)
+AwsWafRateBasedRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRateBasedRuleDetailsOutputTypeDef",
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RateKey": NotRequired[str],
         "RateLimit": NotRequired[int],
         "RuleId": NotRequired[str],
         "MatchPredicates": NotRequired[List[AwsWafRateBasedRuleMatchPredicateTypeDef]],
@@ -7262,16 +8700,27 @@
         "Name": NotRequired[str],
         "RateKey": NotRequired[str],
         "RateLimit": NotRequired[int],
         "RuleId": NotRequired[str],
         "MatchPredicates": NotRequired[Sequence[AwsWafRateBasedRuleMatchPredicateTypeDef]],
     },
 )
-AwsWafRegionalRateBasedRuleDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafRegionalRateBasedRuleDetailsPaginatorTypeDef",
+AwsWafRegionalRateBasedRuleDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafRegionalRateBasedRuleDetailsExtraOutputTypeDef",
+    {
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "RateKey": NotRequired[str],
+        "RateLimit": NotRequired[int],
+        "RuleId": NotRequired[str],
+        "MatchPredicates": NotRequired[List[AwsWafRegionalRateBasedRuleMatchPredicateTypeDef]],
+    },
+)
+AwsWafRegionalRateBasedRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalRateBasedRuleDetailsOutputTypeDef",
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RateKey": NotRequired[str],
         "RateLimit": NotRequired[int],
         "RuleId": NotRequired[str],
         "MatchPredicates": NotRequired[List[AwsWafRegionalRateBasedRuleMatchPredicateTypeDef]],
@@ -7284,16 +8733,25 @@
         "Name": NotRequired[str],
         "RateKey": NotRequired[str],
         "RateLimit": NotRequired[int],
         "RuleId": NotRequired[str],
         "MatchPredicates": NotRequired[Sequence[AwsWafRegionalRateBasedRuleMatchPredicateTypeDef]],
     },
 )
-AwsWafRegionalRuleDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafRegionalRuleDetailsPaginatorTypeDef",
+AwsWafRegionalRuleDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafRegionalRuleDetailsExtraOutputTypeDef",
+    {
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "PredicateList": NotRequired[List[AwsWafRegionalRulePredicateListDetailsTypeDef]],
+        "RuleId": NotRequired[str],
+    },
+)
+AwsWafRegionalRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalRuleDetailsOutputTypeDef",
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "PredicateList": NotRequired[List[AwsWafRegionalRulePredicateListDetailsTypeDef]],
         "RuleId": NotRequired[str],
     },
 )
@@ -7321,16 +8779,25 @@
         "Action": NotRequired[AwsWafRegionalWebAclRulesListActionDetailsTypeDef],
         "OverrideAction": NotRequired[AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef],
         "Priority": NotRequired[int],
         "RuleId": NotRequired[str],
         "Type": NotRequired[str],
     },
 )
-AwsWafRuleDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafRuleDetailsPaginatorTypeDef",
+AwsWafRuleDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafRuleDetailsExtraOutputTypeDef",
+    {
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "PredicateList": NotRequired[List[AwsWafRulePredicateListDetailsTypeDef]],
+        "RuleId": NotRequired[str],
+    },
+)
+AwsWafRuleDetailsOutputTypeDef = TypedDict(
+    "AwsWafRuleDetailsOutputTypeDef",
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "PredicateList": NotRequired[List[AwsWafRulePredicateListDetailsTypeDef]],
         "RuleId": NotRequired[str],
     },
 )
@@ -7348,16 +8815,27 @@
     {
         "Action": NotRequired[AwsWafRuleGroupRulesActionDetailsTypeDef],
         "Priority": NotRequired[int],
         "RuleId": NotRequired[str],
         "Type": NotRequired[str],
     },
 )
-AwsWafWebAclRulePaginatorTypeDef = TypedDict(
-    "AwsWafWebAclRulePaginatorTypeDef",
+AwsWafWebAclRuleExtraOutputTypeDef = TypedDict(
+    "AwsWafWebAclRuleExtraOutputTypeDef",
+    {
+        "Action": NotRequired[WafActionTypeDef],
+        "ExcludedRules": NotRequired[List[WafExcludedRuleTypeDef]],
+        "OverrideAction": NotRequired[WafOverrideActionTypeDef],
+        "Priority": NotRequired[int],
+        "RuleId": NotRequired[str],
+        "Type": NotRequired[str],
+    },
+)
+AwsWafWebAclRuleOutputTypeDef = TypedDict(
+    "AwsWafWebAclRuleOutputTypeDef",
     {
         "Action": NotRequired[WafActionTypeDef],
         "ExcludedRules": NotRequired[List[WafExcludedRuleTypeDef]],
         "OverrideAction": NotRequired[WafOverrideActionTypeDef],
         "Priority": NotRequired[int],
         "RuleId": NotRequired[str],
         "Type": NotRequired[str],
@@ -7370,28 +8848,42 @@
         "ExcludedRules": NotRequired[Sequence[WafExcludedRuleTypeDef]],
         "OverrideAction": NotRequired[WafOverrideActionTypeDef],
         "Priority": NotRequired[int],
         "RuleId": NotRequired[str],
         "Type": NotRequired[str],
     },
 )
-AwsWafv2CustomRequestHandlingDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2CustomRequestHandlingDetailsPaginatorTypeDef",
+AwsWafv2CustomRequestHandlingDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2CustomRequestHandlingDetailsExtraOutputTypeDef",
+    {
+        "InsertHeaders": NotRequired[List[AwsWafv2CustomHttpHeaderTypeDef]],
+    },
+)
+AwsWafv2CustomRequestHandlingDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2CustomRequestHandlingDetailsOutputTypeDef",
     {
         "InsertHeaders": NotRequired[List[AwsWafv2CustomHttpHeaderTypeDef]],
     },
 )
 AwsWafv2CustomRequestHandlingDetailsTypeDef = TypedDict(
     "AwsWafv2CustomRequestHandlingDetailsTypeDef",
     {
         "InsertHeaders": NotRequired[Sequence[AwsWafv2CustomHttpHeaderTypeDef]],
     },
 )
-AwsWafv2CustomResponseDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2CustomResponseDetailsPaginatorTypeDef",
+AwsWafv2CustomResponseDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2CustomResponseDetailsExtraOutputTypeDef",
+    {
+        "CustomResponseBodyKey": NotRequired[str],
+        "ResponseCode": NotRequired[int],
+        "ResponseHeaders": NotRequired[List[AwsWafv2CustomHttpHeaderTypeDef]],
+    },
+)
+AwsWafv2CustomResponseDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2CustomResponseDetailsOutputTypeDef",
     {
         "CustomResponseBodyKey": NotRequired[str],
         "ResponseCode": NotRequired[int],
         "ResponseHeaders": NotRequired[List[AwsWafv2CustomHttpHeaderTypeDef]],
     },
 )
 AwsWafv2CustomResponseDetailsTypeDef = TypedDict(
@@ -7455,16 +8947,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeActionTargetsResponseTypeDef = TypedDict(
     "DescribeActionTargetsResponseTypeDef",
     {
         "ActionTargets": List[ActionTargetTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeHubResponseTypeDef = TypedDict(
     "DescribeHubResponseTypeDef",
     {
         "HubArn": str,
         "SubscribedAt": str,
@@ -7510,32 +9002,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAutomationRulesResponseTypeDef = TypedDict(
     "ListAutomationRulesResponseTypeDef",
     {
         "AutomationRulesMetadata": List[AutomationRulesMetadataTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListEnabledProductsForImportResponseTypeDef = TypedDict(
     "ListEnabledProductsForImportResponseTypeDef",
     {
         "ProductSubscriptions": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
     "ListOrganizationAdminAccountsResponseTypeDef",
     {
         "AdminAccounts": List[AdminAccountTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -7588,16 +9080,16 @@
 )
 ListConfigurationPolicyAssociationsResponseTypeDef = TypedDict(
     "ListConfigurationPolicyAssociationsResponseTypeDef",
     {
         "ConfigurationPolicyAssociationSummaries": List[
             ConfigurationPolicyAssociationSummaryTypeDef
         ],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 BatchGetStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
     "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
     {
         "StandardsControlAssociationIds": Sequence[StandardsControlAssociationIdTypeDef],
     },
@@ -7629,39 +9121,58 @@
     "UnprocessedStandardsControlAssociationUpdateTypeDef",
     {
         "StandardsControlAssociationUpdate": StandardsControlAssociationUpdateTypeDef,
         "ErrorCode": UnprocessedErrorCodeType,
         "ErrorReason": NotRequired[str],
     },
 )
-VulnerabilityCodeVulnerabilitiesPaginatorTypeDef = TypedDict(
-    "VulnerabilityCodeVulnerabilitiesPaginatorTypeDef",
+VulnerabilityCodeVulnerabilitiesExtraOutputTypeDef = TypedDict(
+    "VulnerabilityCodeVulnerabilitiesExtraOutputTypeDef",
+    {
+        "Cwes": NotRequired[List[str]],
+        "FilePath": NotRequired[CodeVulnerabilitiesFilePathTypeDef],
+        "SourceArn": NotRequired[str],
+    },
+)
+VulnerabilityCodeVulnerabilitiesOutputTypeDef = TypedDict(
+    "VulnerabilityCodeVulnerabilitiesOutputTypeDef",
     {
         "Cwes": NotRequired[List[str]],
         "FilePath": NotRequired[CodeVulnerabilitiesFilePathTypeDef],
         "SourceArn": NotRequired[str],
     },
 )
 VulnerabilityCodeVulnerabilitiesTypeDef = TypedDict(
     "VulnerabilityCodeVulnerabilitiesTypeDef",
     {
         "Cwes": NotRequired[Sequence[str]],
         "FilePath": NotRequired[CodeVulnerabilitiesFilePathTypeDef],
         "SourceArn": NotRequired[str],
     },
 )
-CompliancePaginatorTypeDef = TypedDict(
-    "CompliancePaginatorTypeDef",
+ComplianceExtraOutputTypeDef = TypedDict(
+    "ComplianceExtraOutputTypeDef",
     {
         "Status": NotRequired[ComplianceStatusType],
         "RelatedRequirements": NotRequired[List[str]],
         "StatusReasons": NotRequired[List[StatusReasonTypeDef]],
         "SecurityControlId": NotRequired[str],
         "AssociatedStandards": NotRequired[List[AssociatedStandardTypeDef]],
-        "SecurityControlParameters": NotRequired[List[SecurityControlParameterPaginatorTypeDef]],
+        "SecurityControlParameters": NotRequired[List[SecurityControlParameterExtraOutputTypeDef]],
+    },
+)
+ComplianceOutputTypeDef = TypedDict(
+    "ComplianceOutputTypeDef",
+    {
+        "Status": NotRequired[ComplianceStatusType],
+        "RelatedRequirements": NotRequired[List[str]],
+        "StatusReasons": NotRequired[List[StatusReasonTypeDef]],
+        "SecurityControlId": NotRequired[str],
+        "AssociatedStandards": NotRequired[List[AssociatedStandardTypeDef]],
+        "SecurityControlParameters": NotRequired[List[SecurityControlParameterOutputTypeDef]],
     },
 )
 ComplianceTypeDef = TypedDict(
     "ComplianceTypeDef",
     {
         "Status": NotRequired[ComplianceStatusType],
         "RelatedRequirements": NotRequired[Sequence[str]],
@@ -7710,20 +9221,32 @@
         "Target": NotRequired[TargetTypeDef],
     },
 )
 ListConfigurationPoliciesResponseTypeDef = TypedDict(
     "ListConfigurationPoliciesResponseTypeDef",
     {
         "ConfigurationPolicySummaries": List[ConfigurationPolicySummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+ContainerDetailsExtraOutputTypeDef = TypedDict(
+    "ContainerDetailsExtraOutputTypeDef",
+    {
+        "ContainerRuntime": NotRequired[str],
+        "Name": NotRequired[str],
+        "ImageId": NotRequired[str],
+        "ImageName": NotRequired[str],
+        "LaunchedAt": NotRequired[str],
+        "VolumeMounts": NotRequired[List[VolumeMountTypeDef]],
+        "Privileged": NotRequired[bool],
     },
 )
-ContainerDetailsPaginatorTypeDef = TypedDict(
-    "ContainerDetailsPaginatorTypeDef",
+ContainerDetailsOutputTypeDef = TypedDict(
+    "ContainerDetailsOutputTypeDef",
     {
         "ContainerRuntime": NotRequired[str],
         "Name": NotRequired[str],
         "ImageId": NotRequired[str],
         "ImageName": NotRequired[str],
         "LaunchedAt": NotRequired[str],
         "VolumeMounts": NotRequired[List[VolumeMountTypeDef]],
@@ -7902,28 +9425,37 @@
         "OrganizationConfiguration": NotRequired[OrganizationConfigurationTypeDef],
     },
 )
 DescribeProductsResponseTypeDef = TypedDict(
     "DescribeProductsResponseTypeDef",
     {
         "Products": List[ProductTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeStandardsControlsResponseTypeDef = TypedDict(
     "DescribeStandardsControlsResponseTypeDef",
     {
         "Controls": List[StandardsControlTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-ThreatPaginatorTypeDef = TypedDict(
-    "ThreatPaginatorTypeDef",
+ThreatExtraOutputTypeDef = TypedDict(
+    "ThreatExtraOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "Severity": NotRequired[str],
+        "ItemCount": NotRequired[int],
+        "FilePaths": NotRequired[List[FilePathsTypeDef]],
+    },
+)
+ThreatOutputTypeDef = TypedDict(
+    "ThreatOutputTypeDef",
     {
         "Name": NotRequired[str],
         "Severity": NotRequired[str],
         "ItemCount": NotRequired[int],
         "FilePaths": NotRequired[List[FilePathsTypeDef]],
     },
 )
@@ -7936,31 +9468,41 @@
         "FilePaths": NotRequired[Sequence[FilePathsTypeDef]],
     },
 )
 ListFindingAggregatorsResponseTypeDef = TypedDict(
     "ListFindingAggregatorsResponseTypeDef",
     {
         "FindingAggregators": List[FindingAggregatorTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 FindingHistoryRecordTypeDef = TypedDict(
     "FindingHistoryRecordTypeDef",
     {
         "FindingIdentifier": NotRequired[AwsSecurityFindingIdentifierTypeDef],
         "UpdateTime": NotRequired[datetime],
         "FindingCreated": NotRequired[bool],
         "UpdateSource": NotRequired[FindingHistoryUpdateSourceTypeDef],
         "Updates": NotRequired[List[FindingHistoryUpdateTypeDef]],
         "NextToken": NotRequired[str],
     },
 )
-FindingProviderFieldsPaginatorTypeDef = TypedDict(
-    "FindingProviderFieldsPaginatorTypeDef",
+FindingProviderFieldsExtraOutputTypeDef = TypedDict(
+    "FindingProviderFieldsExtraOutputTypeDef",
+    {
+        "Confidence": NotRequired[int],
+        "Criticality": NotRequired[int],
+        "RelatedFindings": NotRequired[List[RelatedFindingTypeDef]],
+        "Severity": NotRequired[FindingProviderSeverityTypeDef],
+        "Types": NotRequired[List[str]],
+    },
+)
+FindingProviderFieldsOutputTypeDef = TypedDict(
+    "FindingProviderFieldsOutputTypeDef",
     {
         "Confidence": NotRequired[int],
         "Criticality": NotRequired[int],
         "RelatedFindings": NotRequired[List[RelatedFindingTypeDef]],
         "Severity": NotRequired[FindingProviderSeverityTypeDef],
         "Types": NotRequired[List[str]],
     },
@@ -7989,16 +9531,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef = TypedDict(
     "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
     {
         "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
         "StartTime": NotRequired[TimestampTypeDef],
@@ -8024,36 +9566,43 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 InsightResultsTypeDef = TypedDict(
     "InsightResultsTypeDef",
     {
         "InsightArn": str,
         "GroupByAttribute": str,
         "ResultValues": List[InsightResultValueTypeDef],
     },
 )
 ListStandardsControlAssociationsResponseTypeDef = TypedDict(
     "ListStandardsControlAssociationsResponseTypeDef",
     {
         "StandardsControlAssociationSummaries": List[StandardsControlAssociationSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-NetworkPathComponentDetailsPaginatorTypeDef = TypedDict(
-    "NetworkPathComponentDetailsPaginatorTypeDef",
+NetworkPathComponentDetailsExtraOutputTypeDef = TypedDict(
+    "NetworkPathComponentDetailsExtraOutputTypeDef",
+    {
+        "Address": NotRequired[List[str]],
+        "PortRanges": NotRequired[List[PortRangeTypeDef]],
+    },
+)
+NetworkPathComponentDetailsOutputTypeDef = TypedDict(
+    "NetworkPathComponentDetailsOutputTypeDef",
     {
         "Address": NotRequired[List[str]],
         "PortRanges": NotRequired[List[PortRangeTypeDef]],
     },
 )
 NetworkPathComponentDetailsTypeDef = TypedDict(
     "NetworkPathComponentDetailsTypeDef",
@@ -8083,61 +9632,95 @@
     "PageTypeDef",
     {
         "PageNumber": NotRequired[int],
         "LineRange": NotRequired[RangeTypeDef],
         "OffsetRange": NotRequired[RangeTypeDef],
     },
 )
+ParameterConfigurationOutputTypeDef = TypedDict(
+    "ParameterConfigurationOutputTypeDef",
+    {
+        "ValueType": ParameterValueTypeType,
+        "Value": NotRequired[ParameterValueOutputTypeDef],
+    },
+)
 ParameterConfigurationTypeDef = TypedDict(
     "ParameterConfigurationTypeDef",
     {
         "ValueType": ParameterValueTypeType,
         "Value": NotRequired[ParameterValueTypeDef],
     },
 )
 RemediationTypeDef = TypedDict(
     "RemediationTypeDef",
     {
         "Recommendation": NotRequired[RecommendationTypeDef],
     },
 )
-RuleGroupSourceStatefulRulesDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceStatefulRulesDetailsPaginatorTypeDef",
+RuleGroupSourceStatefulRulesDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatefulRulesDetailsExtraOutputTypeDef",
     {
         "Action": NotRequired[str],
         "Header": NotRequired[RuleGroupSourceStatefulRulesHeaderDetailsTypeDef],
         "RuleOptions": NotRequired[
-            List[RuleGroupSourceStatefulRulesOptionsDetailsPaginatorTypeDef]
+            List[RuleGroupSourceStatefulRulesOptionsDetailsExtraOutputTypeDef]
         ],
     },
 )
+RuleGroupSourceStatefulRulesDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatefulRulesDetailsOutputTypeDef",
+    {
+        "Action": NotRequired[str],
+        "Header": NotRequired[RuleGroupSourceStatefulRulesHeaderDetailsTypeDef],
+        "RuleOptions": NotRequired[List[RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef]],
+    },
+)
 RuleGroupSourceStatefulRulesDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
     {
         "Action": NotRequired[str],
         "Header": NotRequired[RuleGroupSourceStatefulRulesHeaderDetailsTypeDef],
         "RuleOptions": NotRequired[Sequence[RuleGroupSourceStatefulRulesOptionsDetailsTypeDef]],
     },
 )
-RuleGroupSourceStatelessRuleMatchAttributesPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesPaginatorTypeDef",
+RuleGroupSourceStatelessRuleMatchAttributesExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesExtraOutputTypeDef",
     {
         "DestinationPorts": NotRequired[
             List[RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef]
         ],
         "Destinations": NotRequired[
             List[RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef]
         ],
         "Protocols": NotRequired[List[int]],
         "SourcePorts": NotRequired[
             List[RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef]
         ],
         "Sources": NotRequired[List[RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef]],
         "TcpFlags": NotRequired[
-            List[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsPaginatorTypeDef]
+            List[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsExtraOutputTypeDef]
+        ],
+    },
+)
+RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef",
+    {
+        "DestinationPorts": NotRequired[
+            List[RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef]
+        ],
+        "Destinations": NotRequired[
+            List[RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef]
+        ],
+        "Protocols": NotRequired[List[int]],
+        "SourcePorts": NotRequired[
+            List[RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef]
+        ],
+        "Sources": NotRequired[List[RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef]],
+        "TcpFlags": NotRequired[
+            List[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef]
         ],
     },
 )
 RuleGroupSourceStatelessRuleMatchAttributesTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
     {
         "DestinationPorts": NotRequired[
@@ -8152,19 +9735,26 @@
         ],
         "Sources": NotRequired[Sequence[RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef]],
         "TcpFlags": NotRequired[
             Sequence[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef]
         ],
     },
 )
-RuleGroupVariablesPaginatorTypeDef = TypedDict(
-    "RuleGroupVariablesPaginatorTypeDef",
+RuleGroupVariablesExtraOutputTypeDef = TypedDict(
+    "RuleGroupVariablesExtraOutputTypeDef",
+    {
+        "IpSets": NotRequired[RuleGroupVariablesIpSetsDetailsExtraOutputTypeDef],
+        "PortSets": NotRequired[RuleGroupVariablesPortSetsDetailsExtraOutputTypeDef],
+    },
+)
+RuleGroupVariablesOutputTypeDef = TypedDict(
+    "RuleGroupVariablesOutputTypeDef",
     {
-        "IpSets": NotRequired[RuleGroupVariablesIpSetsDetailsPaginatorTypeDef],
-        "PortSets": NotRequired[RuleGroupVariablesPortSetsDetailsPaginatorTypeDef],
+        "IpSets": NotRequired[RuleGroupVariablesIpSetsDetailsOutputTypeDef],
+        "PortSets": NotRequired[RuleGroupVariablesPortSetsDetailsOutputTypeDef],
     },
 )
 RuleGroupVariablesTypeDef = TypedDict(
     "RuleGroupVariablesTypeDef",
     {
         "IpSets": NotRequired[RuleGroupVariablesIpSetsDetailsTypeDef],
         "PortSets": NotRequired[RuleGroupVariablesPortSetsDetailsTypeDef],
@@ -8186,28 +9776,47 @@
         "StandardsSubscriptionArn": str,
         "StandardsArn": str,
         "StandardsInput": Dict[str, str],
         "StandardsStatus": StandardsStatusType,
         "StandardsStatusReason": NotRequired[StandardsStatusReasonTypeDef],
     },
 )
-StatelessCustomPublishMetricActionPaginatorTypeDef = TypedDict(
-    "StatelessCustomPublishMetricActionPaginatorTypeDef",
+StatelessCustomPublishMetricActionExtraOutputTypeDef = TypedDict(
+    "StatelessCustomPublishMetricActionExtraOutputTypeDef",
+    {
+        "Dimensions": NotRequired[List[StatelessCustomPublishMetricActionDimensionTypeDef]],
+    },
+)
+StatelessCustomPublishMetricActionOutputTypeDef = TypedDict(
+    "StatelessCustomPublishMetricActionOutputTypeDef",
     {
         "Dimensions": NotRequired[List[StatelessCustomPublishMetricActionDimensionTypeDef]],
     },
 )
 StatelessCustomPublishMetricActionTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionTypeDef",
     {
         "Dimensions": NotRequired[Sequence[StatelessCustomPublishMetricActionDimensionTypeDef]],
     },
 )
-AwsApiCallActionPaginatorTypeDef = TypedDict(
-    "AwsApiCallActionPaginatorTypeDef",
+AwsApiCallActionExtraOutputTypeDef = TypedDict(
+    "AwsApiCallActionExtraOutputTypeDef",
+    {
+        "Api": NotRequired[str],
+        "ServiceName": NotRequired[str],
+        "CallerType": NotRequired[str],
+        "RemoteIpDetails": NotRequired[ActionRemoteIpDetailsTypeDef],
+        "DomainDetails": NotRequired[AwsApiCallActionDomainDetailsTypeDef],
+        "AffectedResources": NotRequired[Dict[str, str]],
+        "FirstSeen": NotRequired[str],
+        "LastSeen": NotRequired[str],
+    },
+)
+AwsApiCallActionOutputTypeDef = TypedDict(
+    "AwsApiCallActionOutputTypeDef",
     {
         "Api": NotRequired[str],
         "ServiceName": NotRequired[str],
         "CallerType": NotRequired[str],
         "RemoteIpDetails": NotRequired[ActionRemoteIpDetailsTypeDef],
         "DomainDetails": NotRequired[AwsApiCallActionDomainDetailsTypeDef],
         "AffectedResources": NotRequired[Dict[str, str]],
@@ -8243,16 +9852,27 @@
     "PortProbeDetailTypeDef",
     {
         "LocalPortDetails": NotRequired[ActionLocalPortDetailsTypeDef],
         "LocalIpDetails": NotRequired[ActionLocalIpDetailsTypeDef],
         "RemoteIpDetails": NotRequired[ActionRemoteIpDetailsTypeDef],
     },
 )
-AwsEc2RouteTableDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2RouteTableDetailsPaginatorTypeDef",
+AwsEc2RouteTableDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2RouteTableDetailsExtraOutputTypeDef",
+    {
+        "AssociationSet": NotRequired[List[AssociationSetDetailsTypeDef]],
+        "OwnerId": NotRequired[str],
+        "PropagatingVgwSet": NotRequired[List[PropagatingVgwSetDetailsTypeDef]],
+        "RouteTableId": NotRequired[str],
+        "RouteSet": NotRequired[List[RouteSetDetailsTypeDef]],
+        "VpcId": NotRequired[str],
+    },
+)
+AwsEc2RouteTableDetailsOutputTypeDef = TypedDict(
+    "AwsEc2RouteTableDetailsOutputTypeDef",
     {
         "AssociationSet": NotRequired[List[AssociationSetDetailsTypeDef]],
         "OwnerId": NotRequired[str],
         "PropagatingVgwSet": NotRequired[List[PropagatingVgwSetDetailsTypeDef]],
         "RouteTableId": NotRequired[str],
         "RouteSet": NotRequired[List[RouteSetDetailsTypeDef]],
         "VpcId": NotRequired[str],
@@ -8265,48 +9885,80 @@
         "OwnerId": NotRequired[str],
         "PropagatingVgwSet": NotRequired[Sequence[PropagatingVgwSetDetailsTypeDef]],
         "RouteTableId": NotRequired[str],
         "RouteSet": NotRequired[Sequence[RouteSetDetailsTypeDef]],
         "VpcId": NotRequired[str],
     },
 )
+AutomationRulesActionOutputTypeDef = TypedDict(
+    "AutomationRulesActionOutputTypeDef",
+    {
+        "Type": NotRequired[Literal["FINDING_FIELDS_UPDATE"]],
+        "FindingFieldsUpdate": NotRequired[AutomationRulesFindingFieldsUpdateOutputTypeDef],
+    },
+)
 AutomationRulesActionTypeDef = TypedDict(
     "AutomationRulesActionTypeDef",
     {
         "Type": NotRequired[Literal["FINDING_FIELDS_UPDATE"]],
         "FindingFieldsUpdate": NotRequired[AutomationRulesFindingFieldsUpdateTypeDef],
     },
 )
-AwsAmazonMqBrokerDetailsPaginatorTypeDef = TypedDict(
-    "AwsAmazonMqBrokerDetailsPaginatorTypeDef",
+AwsAmazonMqBrokerDetailsExtraOutputTypeDef = TypedDict(
+    "AwsAmazonMqBrokerDetailsExtraOutputTypeDef",
     {
         "AuthenticationStrategy": NotRequired[str],
         "AutoMinorVersionUpgrade": NotRequired[bool],
         "BrokerArn": NotRequired[str],
         "BrokerName": NotRequired[str],
         "DeploymentMode": NotRequired[str],
         "EncryptionOptions": NotRequired[AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef],
         "EngineType": NotRequired[str],
         "EngineVersion": NotRequired[str],
         "HostInstanceType": NotRequired[str],
         "BrokerId": NotRequired[str],
         "LdapServerMetadata": NotRequired[
-            AwsAmazonMqBrokerLdapServerMetadataDetailsPaginatorTypeDef
+            AwsAmazonMqBrokerLdapServerMetadataDetailsExtraOutputTypeDef
         ],
         "Logs": NotRequired[AwsAmazonMqBrokerLogsDetailsTypeDef],
         "MaintenanceWindowStartTime": NotRequired[
             AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef
         ],
         "PubliclyAccessible": NotRequired[bool],
         "SecurityGroups": NotRequired[List[str]],
         "StorageType": NotRequired[str],
         "SubnetIds": NotRequired[List[str]],
         "Users": NotRequired[List[AwsAmazonMqBrokerUsersDetailsTypeDef]],
     },
 )
+AwsAmazonMqBrokerDetailsOutputTypeDef = TypedDict(
+    "AwsAmazonMqBrokerDetailsOutputTypeDef",
+    {
+        "AuthenticationStrategy": NotRequired[str],
+        "AutoMinorVersionUpgrade": NotRequired[bool],
+        "BrokerArn": NotRequired[str],
+        "BrokerName": NotRequired[str],
+        "DeploymentMode": NotRequired[str],
+        "EncryptionOptions": NotRequired[AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef],
+        "EngineType": NotRequired[str],
+        "EngineVersion": NotRequired[str],
+        "HostInstanceType": NotRequired[str],
+        "BrokerId": NotRequired[str],
+        "LdapServerMetadata": NotRequired[AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef],
+        "Logs": NotRequired[AwsAmazonMqBrokerLogsDetailsTypeDef],
+        "MaintenanceWindowStartTime": NotRequired[
+            AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef
+        ],
+        "PubliclyAccessible": NotRequired[bool],
+        "SecurityGroups": NotRequired[List[str]],
+        "StorageType": NotRequired[str],
+        "SubnetIds": NotRequired[List[str]],
+        "Users": NotRequired[List[AwsAmazonMqBrokerUsersDetailsTypeDef]],
+    },
+)
 AwsAmazonMqBrokerDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerDetailsTypeDef",
     {
         "AuthenticationStrategy": NotRequired[str],
         "AutoMinorVersionUpgrade": NotRequired[bool],
         "BrokerArn": NotRequired[str],
         "BrokerName": NotRequired[str],
@@ -8324,16 +9976,37 @@
         "PubliclyAccessible": NotRequired[bool],
         "SecurityGroups": NotRequired[Sequence[str]],
         "StorageType": NotRequired[str],
         "SubnetIds": NotRequired[Sequence[str]],
         "Users": NotRequired[Sequence[AwsAmazonMqBrokerUsersDetailsTypeDef]],
     },
 )
-AwsAppSyncGraphQlApiDetailsPaginatorTypeDef = TypedDict(
-    "AwsAppSyncGraphQlApiDetailsPaginatorTypeDef",
+AwsAppSyncGraphQlApiDetailsExtraOutputTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiDetailsExtraOutputTypeDef",
+    {
+        "ApiId": NotRequired[str],
+        "Id": NotRequired[str],
+        "OpenIdConnectConfig": NotRequired[AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef],
+        "Name": NotRequired[str],
+        "LambdaAuthorizerConfig": NotRequired[
+            AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef
+        ],
+        "XrayEnabled": NotRequired[bool],
+        "Arn": NotRequired[str],
+        "UserPoolConfig": NotRequired[AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef],
+        "AuthenticationType": NotRequired[str],
+        "LogConfig": NotRequired[AwsAppSyncGraphQlApiLogConfigDetailsTypeDef],
+        "AdditionalAuthenticationProviders": NotRequired[
+            List[AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef]
+        ],
+        "WafWebAclArn": NotRequired[str],
+    },
+)
+AwsAppSyncGraphQlApiDetailsOutputTypeDef = TypedDict(
+    "AwsAppSyncGraphQlApiDetailsOutputTypeDef",
     {
         "ApiId": NotRequired[str],
         "Id": NotRequired[str],
         "OpenIdConnectConfig": NotRequired[AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef],
         "Name": NotRequired[str],
         "LambdaAuthorizerConfig": NotRequired[
             AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef
@@ -8374,38 +10047,77 @@
     "AwsAthenaWorkGroupConfigurationDetailsTypeDef",
     {
         "ResultConfiguration": NotRequired[
             AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef
         ],
     },
 )
-AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsPaginatorTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsPaginatorTypeDef",
+AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsExtraOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsExtraOutputTypeDef",
     {
         "InstancesDistribution": NotRequired[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
         ],
         "LaunchTemplate": NotRequired[
-            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsPaginatorTypeDef
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef",
+    {
+        "InstancesDistribution": NotRequired[
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
+        ],
+        "LaunchTemplate": NotRequired[
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef
         ],
     },
 )
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     {
         "InstancesDistribution": NotRequired[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
         ],
         "LaunchTemplate": NotRequired[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef
         ],
     },
 )
-AwsAutoScalingLaunchConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsAutoScalingLaunchConfigurationDetailsPaginatorTypeDef",
+AwsAutoScalingLaunchConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsAutoScalingLaunchConfigurationDetailsExtraOutputTypeDef",
+    {
+        "AssociatePublicIpAddress": NotRequired[bool],
+        "BlockDeviceMappings": NotRequired[
+            List[AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef]
+        ],
+        "ClassicLinkVpcId": NotRequired[str],
+        "ClassicLinkVpcSecurityGroups": NotRequired[List[str]],
+        "CreatedTime": NotRequired[str],
+        "EbsOptimized": NotRequired[bool],
+        "IamInstanceProfile": NotRequired[str],
+        "ImageId": NotRequired[str],
+        "InstanceMonitoring": NotRequired[
+            AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef
+        ],
+        "InstanceType": NotRequired[str],
+        "KernelId": NotRequired[str],
+        "KeyName": NotRequired[str],
+        "LaunchConfigurationName": NotRequired[str],
+        "PlacementTenancy": NotRequired[str],
+        "RamdiskId": NotRequired[str],
+        "SecurityGroups": NotRequired[List[str]],
+        "SpotPrice": NotRequired[str],
+        "UserData": NotRequired[str],
+        "MetadataOptions": NotRequired[AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef],
+    },
+)
+AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef",
     {
         "AssociatePublicIpAddress": NotRequired[bool],
         "BlockDeviceMappings": NotRequired[
             List[AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef]
         ],
         "ClassicLinkVpcId": NotRequired[str],
         "ClassicLinkVpcSecurityGroups": NotRequired[List[str]],
@@ -8452,16 +10164,30 @@
         "RamdiskId": NotRequired[str],
         "SecurityGroups": NotRequired[Sequence[str]],
         "SpotPrice": NotRequired[str],
         "UserData": NotRequired[str],
         "MetadataOptions": NotRequired[AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef],
     },
 )
-AwsBackupBackupPlanRuleDetailsPaginatorTypeDef = TypedDict(
-    "AwsBackupBackupPlanRuleDetailsPaginatorTypeDef",
+AwsBackupBackupPlanRuleDetailsExtraOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanRuleDetailsExtraOutputTypeDef",
+    {
+        "TargetBackupVault": NotRequired[str],
+        "StartWindowMinutes": NotRequired[int],
+        "ScheduleExpression": NotRequired[str],
+        "RuleName": NotRequired[str],
+        "RuleId": NotRequired[str],
+        "EnableContinuousBackup": NotRequired[bool],
+        "CompletionWindowMinutes": NotRequired[int],
+        "CopyActions": NotRequired[List[AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef]],
+        "Lifecycle": NotRequired[AwsBackupBackupPlanLifecycleDetailsTypeDef],
+    },
+)
+AwsBackupBackupPlanRuleDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanRuleDetailsOutputTypeDef",
     {
         "TargetBackupVault": NotRequired[str],
         "StartWindowMinutes": NotRequired[int],
         "ScheduleExpression": NotRequired[str],
         "RuleName": NotRequired[str],
         "RuleId": NotRequired[str],
         "EnableContinuousBackup": NotRequired[bool],
@@ -8480,19 +10206,30 @@
         "RuleId": NotRequired[str],
         "EnableContinuousBackup": NotRequired[bool],
         "CompletionWindowMinutes": NotRequired[int],
         "CopyActions": NotRequired[Sequence[AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef]],
         "Lifecycle": NotRequired[AwsBackupBackupPlanLifecycleDetailsTypeDef],
     },
 )
-AwsCertificateManagerCertificateRenewalSummaryPaginatorTypeDef = TypedDict(
-    "AwsCertificateManagerCertificateRenewalSummaryPaginatorTypeDef",
+AwsCertificateManagerCertificateRenewalSummaryExtraOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateRenewalSummaryExtraOutputTypeDef",
     {
         "DomainValidationOptions": NotRequired[
-            List[AwsCertificateManagerCertificateDomainValidationOptionPaginatorTypeDef]
+            List[AwsCertificateManagerCertificateDomainValidationOptionExtraOutputTypeDef]
+        ],
+        "RenewalStatus": NotRequired[str],
+        "RenewalStatusReason": NotRequired[str],
+        "UpdatedAt": NotRequired[str],
+    },
+)
+AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef",
+    {
+        "DomainValidationOptions": NotRequired[
+            List[AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef]
         ],
         "RenewalStatus": NotRequired[str],
         "RenewalStatusReason": NotRequired[str],
         "UpdatedAt": NotRequired[str],
     },
 )
 AwsCertificateManagerCertificateRenewalSummaryTypeDef = TypedDict(
@@ -8502,61 +10239,93 @@
             Sequence[AwsCertificateManagerCertificateDomainValidationOptionTypeDef]
         ],
         "RenewalStatus": NotRequired[str],
         "RenewalStatusReason": NotRequired[str],
         "UpdatedAt": NotRequired[str],
     },
 )
-AwsCloudFrontDistributionOriginItemPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginItemPaginatorTypeDef",
+AwsCloudFrontDistributionOriginItemExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginItemExtraOutputTypeDef",
     {
         "DomainName": NotRequired[str],
         "Id": NotRequired[str],
         "OriginPath": NotRequired[str],
         "S3OriginConfig": NotRequired[AwsCloudFrontDistributionOriginS3OriginConfigTypeDef],
         "CustomOriginConfig": NotRequired[
-            AwsCloudFrontDistributionOriginCustomOriginConfigPaginatorTypeDef
+            AwsCloudFrontDistributionOriginCustomOriginConfigExtraOutputTypeDef
+        ],
+    },
+)
+AwsCloudFrontDistributionOriginItemOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginItemOutputTypeDef",
+    {
+        "DomainName": NotRequired[str],
+        "Id": NotRequired[str],
+        "OriginPath": NotRequired[str],
+        "S3OriginConfig": NotRequired[AwsCloudFrontDistributionOriginS3OriginConfigTypeDef],
+        "CustomOriginConfig": NotRequired[
+            AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef
         ],
     },
 )
 AwsCloudFrontDistributionOriginItemTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginItemTypeDef",
     {
         "DomainName": NotRequired[str],
         "Id": NotRequired[str],
         "OriginPath": NotRequired[str],
         "S3OriginConfig": NotRequired[AwsCloudFrontDistributionOriginS3OriginConfigTypeDef],
         "CustomOriginConfig": NotRequired[AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef],
     },
 )
-AwsCloudFrontDistributionOriginGroupPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginGroupPaginatorTypeDef",
+AwsCloudFrontDistributionOriginGroupExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupExtraOutputTypeDef",
     {
         "FailoverCriteria": NotRequired[
-            AwsCloudFrontDistributionOriginGroupFailoverPaginatorTypeDef
+            AwsCloudFrontDistributionOriginGroupFailoverExtraOutputTypeDef
         ],
     },
 )
+AwsCloudFrontDistributionOriginGroupOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupOutputTypeDef",
+    {
+        "FailoverCriteria": NotRequired[AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef],
+    },
+)
 AwsCloudFrontDistributionOriginGroupTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupTypeDef",
     {
         "FailoverCriteria": NotRequired[AwsCloudFrontDistributionOriginGroupFailoverTypeDef],
     },
 )
-AwsCodeBuildProjectDetailsPaginatorTypeDef = TypedDict(
-    "AwsCodeBuildProjectDetailsPaginatorTypeDef",
+AwsCodeBuildProjectDetailsExtraOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectDetailsExtraOutputTypeDef",
+    {
+        "EncryptionKey": NotRequired[str],
+        "Artifacts": NotRequired[List[AwsCodeBuildProjectArtifactsDetailsTypeDef]],
+        "Environment": NotRequired[AwsCodeBuildProjectEnvironmentExtraOutputTypeDef],
+        "Name": NotRequired[str],
+        "Source": NotRequired[AwsCodeBuildProjectSourceTypeDef],
+        "ServiceRole": NotRequired[str],
+        "LogsConfig": NotRequired[AwsCodeBuildProjectLogsConfigDetailsTypeDef],
+        "VpcConfig": NotRequired[AwsCodeBuildProjectVpcConfigExtraOutputTypeDef],
+        "SecondaryArtifacts": NotRequired[List[AwsCodeBuildProjectArtifactsDetailsTypeDef]],
+    },
+)
+AwsCodeBuildProjectDetailsOutputTypeDef = TypedDict(
+    "AwsCodeBuildProjectDetailsOutputTypeDef",
     {
         "EncryptionKey": NotRequired[str],
         "Artifacts": NotRequired[List[AwsCodeBuildProjectArtifactsDetailsTypeDef]],
-        "Environment": NotRequired[AwsCodeBuildProjectEnvironmentPaginatorTypeDef],
+        "Environment": NotRequired[AwsCodeBuildProjectEnvironmentOutputTypeDef],
         "Name": NotRequired[str],
         "Source": NotRequired[AwsCodeBuildProjectSourceTypeDef],
         "ServiceRole": NotRequired[str],
         "LogsConfig": NotRequired[AwsCodeBuildProjectLogsConfigDetailsTypeDef],
-        "VpcConfig": NotRequired[AwsCodeBuildProjectVpcConfigPaginatorTypeDef],
+        "VpcConfig": NotRequired[AwsCodeBuildProjectVpcConfigOutputTypeDef],
         "SecondaryArtifacts": NotRequired[List[AwsCodeBuildProjectArtifactsDetailsTypeDef]],
     },
 )
 AwsCodeBuildProjectDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectDetailsTypeDef",
     {
         "EncryptionKey": NotRequired[str],
@@ -8566,16 +10335,31 @@
         "Source": NotRequired[AwsCodeBuildProjectSourceTypeDef],
         "ServiceRole": NotRequired[str],
         "LogsConfig": NotRequired[AwsCodeBuildProjectLogsConfigDetailsTypeDef],
         "VpcConfig": NotRequired[AwsCodeBuildProjectVpcConfigTypeDef],
         "SecondaryArtifacts": NotRequired[Sequence[AwsCodeBuildProjectArtifactsDetailsTypeDef]],
     },
 )
-AwsDynamoDbTableReplicaPaginatorTypeDef = TypedDict(
-    "AwsDynamoDbTableReplicaPaginatorTypeDef",
+AwsDynamoDbTableReplicaExtraOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableReplicaExtraOutputTypeDef",
+    {
+        "GlobalSecondaryIndexes": NotRequired[
+            List[AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef]
+        ],
+        "KmsMasterKeyId": NotRequired[str],
+        "ProvisionedThroughputOverride": NotRequired[
+            AwsDynamoDbTableProvisionedThroughputOverrideTypeDef
+        ],
+        "RegionName": NotRequired[str],
+        "ReplicaStatus": NotRequired[str],
+        "ReplicaStatusDescription": NotRequired[str],
+    },
+)
+AwsDynamoDbTableReplicaOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableReplicaOutputTypeDef",
     {
         "GlobalSecondaryIndexes": NotRequired[
             List[AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef]
         ],
         "KmsMasterKeyId": NotRequired[str],
         "ProvisionedThroughputOverride": NotRequired[
             AwsDynamoDbTableProvisionedThroughputOverrideTypeDef
@@ -8596,16 +10380,45 @@
             AwsDynamoDbTableProvisionedThroughputOverrideTypeDef
         ],
         "RegionName": NotRequired[str],
         "ReplicaStatus": NotRequired[str],
         "ReplicaStatusDescription": NotRequired[str],
     },
 )
-AwsEc2ClientVpnEndpointDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2ClientVpnEndpointDetailsPaginatorTypeDef",
+AwsEc2ClientVpnEndpointDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2ClientVpnEndpointDetailsExtraOutputTypeDef",
+    {
+        "ClientVpnEndpointId": NotRequired[str],
+        "Description": NotRequired[str],
+        "ClientCidrBlock": NotRequired[str],
+        "DnsServer": NotRequired[List[str]],
+        "SplitTunnel": NotRequired[bool],
+        "TransportProtocol": NotRequired[str],
+        "VpnPort": NotRequired[int],
+        "ServerCertificateArn": NotRequired[str],
+        "AuthenticationOptions": NotRequired[
+            List[AwsEc2ClientVpnEndpointAuthenticationOptionsDetailsTypeDef]
+        ],
+        "ConnectionLogOptions": NotRequired[
+            AwsEc2ClientVpnEndpointConnectionLogOptionsDetailsTypeDef
+        ],
+        "SecurityGroupIdSet": NotRequired[List[str]],
+        "VpcId": NotRequired[str],
+        "SelfServicePortalUrl": NotRequired[str],
+        "ClientConnectOptions": NotRequired[
+            AwsEc2ClientVpnEndpointClientConnectOptionsDetailsTypeDef
+        ],
+        "SessionTimeoutHours": NotRequired[int],
+        "ClientLoginBannerOptions": NotRequired[
+            AwsEc2ClientVpnEndpointClientLoginBannerOptionsDetailsTypeDef
+        ],
+    },
+)
+AwsEc2ClientVpnEndpointDetailsOutputTypeDef = TypedDict(
+    "AwsEc2ClientVpnEndpointDetailsOutputTypeDef",
     {
         "ClientVpnEndpointId": NotRequired[str],
         "Description": NotRequired[str],
         "ClientCidrBlock": NotRequired[str],
         "DnsServer": NotRequired[List[str]],
         "SplitTunnel": NotRequired[bool],
         "TransportProtocol": NotRequired[str],
@@ -8654,16 +10467,69 @@
         ],
         "SessionTimeoutHours": NotRequired[int],
         "ClientLoginBannerOptions": NotRequired[
             AwsEc2ClientVpnEndpointClientLoginBannerOptionsDetailsTypeDef
         ],
     },
 )
-AwsEc2LaunchTemplateDataDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataDetailsPaginatorTypeDef",
+AwsEc2LaunchTemplateDataDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataDetailsExtraOutputTypeDef",
+    {
+        "BlockDeviceMappingSet": NotRequired[
+            List[AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef]
+        ],
+        "CapacityReservationSpecification": NotRequired[
+            AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef
+        ],
+        "CpuOptions": NotRequired[AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef],
+        "CreditSpecification": NotRequired[
+            AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef
+        ],
+        "DisableApiStop": NotRequired[bool],
+        "DisableApiTermination": NotRequired[bool],
+        "EbsOptimized": NotRequired[bool],
+        "ElasticGpuSpecificationSet": NotRequired[
+            List[AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef]
+        ],
+        "ElasticInferenceAcceleratorSet": NotRequired[
+            List[AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef]
+        ],
+        "EnclaveOptions": NotRequired[AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef],
+        "HibernationOptions": NotRequired[AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef],
+        "IamInstanceProfile": NotRequired[AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef],
+        "ImageId": NotRequired[str],
+        "InstanceInitiatedShutdownBehavior": NotRequired[str],
+        "InstanceMarketOptions": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef
+        ],
+        "InstanceRequirements": NotRequired[
+            AwsEc2LaunchTemplateDataInstanceRequirementsDetailsExtraOutputTypeDef
+        ],
+        "InstanceType": NotRequired[str],
+        "KernelId": NotRequired[str],
+        "KeyName": NotRequired[str],
+        "LicenseSet": NotRequired[List[AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef]],
+        "MaintenanceOptions": NotRequired[AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef],
+        "MetadataOptions": NotRequired[AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef],
+        "Monitoring": NotRequired[AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef],
+        "NetworkInterfaceSet": NotRequired[
+            List[AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsExtraOutputTypeDef]
+        ],
+        "Placement": NotRequired[AwsEc2LaunchTemplateDataPlacementDetailsTypeDef],
+        "PrivateDnsNameOptions": NotRequired[
+            AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef
+        ],
+        "RamDiskId": NotRequired[str],
+        "SecurityGroupIdSet": NotRequired[List[str]],
+        "SecurityGroupSet": NotRequired[List[str]],
+        "UserData": NotRequired[str],
+    },
+)
+AwsEc2LaunchTemplateDataDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDataDetailsOutputTypeDef",
     {
         "BlockDeviceMappingSet": NotRequired[
             List[AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef]
         ],
         "CapacityReservationSpecification": NotRequired[
             AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef
         ],
@@ -8685,25 +10551,25 @@
         "IamInstanceProfile": NotRequired[AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef],
         "ImageId": NotRequired[str],
         "InstanceInitiatedShutdownBehavior": NotRequired[str],
         "InstanceMarketOptions": NotRequired[
             AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef
         ],
         "InstanceRequirements": NotRequired[
-            AwsEc2LaunchTemplateDataInstanceRequirementsDetailsPaginatorTypeDef
+            AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef
         ],
         "InstanceType": NotRequired[str],
         "KernelId": NotRequired[str],
         "KeyName": NotRequired[str],
         "LicenseSet": NotRequired[List[AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef]],
         "MaintenanceOptions": NotRequired[AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef],
         "MetadataOptions": NotRequired[AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef],
         "Monitoring": NotRequired[AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef],
         "NetworkInterfaceSet": NotRequired[
-            List[AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsPaginatorTypeDef]
+            List[AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef]
         ],
         "Placement": NotRequired[AwsEc2LaunchTemplateDataPlacementDetailsTypeDef],
         "PrivateDnsNameOptions": NotRequired[
             AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef
         ],
         "RamDiskId": NotRequired[str],
         "SecurityGroupIdSet": NotRequired[List[str]],
@@ -8760,16 +10626,27 @@
         ],
         "RamDiskId": NotRequired[str],
         "SecurityGroupIdSet": NotRequired[Sequence[str]],
         "SecurityGroupSet": NotRequired[Sequence[str]],
         "UserData": NotRequired[str],
     },
 )
-AwsEc2NetworkAclDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2NetworkAclDetailsPaginatorTypeDef",
+AwsEc2NetworkAclDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2NetworkAclDetailsExtraOutputTypeDef",
+    {
+        "IsDefault": NotRequired[bool],
+        "NetworkAclId": NotRequired[str],
+        "OwnerId": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "Associations": NotRequired[List[AwsEc2NetworkAclAssociationTypeDef]],
+        "Entries": NotRequired[List[AwsEc2NetworkAclEntryTypeDef]],
+    },
+)
+AwsEc2NetworkAclDetailsOutputTypeDef = TypedDict(
+    "AwsEc2NetworkAclDetailsOutputTypeDef",
     {
         "IsDefault": NotRequired[bool],
         "NetworkAclId": NotRequired[str],
         "OwnerId": NotRequired[str],
         "VpcId": NotRequired[str],
         "Associations": NotRequired[List[AwsEc2NetworkAclAssociationTypeDef]],
         "Entries": NotRequired[List[AwsEc2NetworkAclEntryTypeDef]],
@@ -8782,68 +10659,105 @@
         "NetworkAclId": NotRequired[str],
         "OwnerId": NotRequired[str],
         "VpcId": NotRequired[str],
         "Associations": NotRequired[Sequence[AwsEc2NetworkAclAssociationTypeDef]],
         "Entries": NotRequired[Sequence[AwsEc2NetworkAclEntryTypeDef]],
     },
 )
-AwsEc2SecurityGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2SecurityGroupDetailsPaginatorTypeDef",
+AwsEc2SecurityGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2SecurityGroupDetailsExtraOutputTypeDef",
     {
         "GroupName": NotRequired[str],
         "GroupId": NotRequired[str],
         "OwnerId": NotRequired[str],
         "VpcId": NotRequired[str],
-        "IpPermissions": NotRequired[List[AwsEc2SecurityGroupIpPermissionPaginatorTypeDef]],
-        "IpPermissionsEgress": NotRequired[List[AwsEc2SecurityGroupIpPermissionPaginatorTypeDef]],
+        "IpPermissions": NotRequired[List[AwsEc2SecurityGroupIpPermissionExtraOutputTypeDef]],
+        "IpPermissionsEgress": NotRequired[List[AwsEc2SecurityGroupIpPermissionExtraOutputTypeDef]],
+    },
+)
+AwsEc2SecurityGroupDetailsOutputTypeDef = TypedDict(
+    "AwsEc2SecurityGroupDetailsOutputTypeDef",
+    {
+        "GroupName": NotRequired[str],
+        "GroupId": NotRequired[str],
+        "OwnerId": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "IpPermissions": NotRequired[List[AwsEc2SecurityGroupIpPermissionOutputTypeDef]],
+        "IpPermissionsEgress": NotRequired[List[AwsEc2SecurityGroupIpPermissionOutputTypeDef]],
     },
 )
 AwsEc2SecurityGroupDetailsTypeDef = TypedDict(
     "AwsEc2SecurityGroupDetailsTypeDef",
     {
         "GroupName": NotRequired[str],
         "GroupId": NotRequired[str],
         "OwnerId": NotRequired[str],
         "VpcId": NotRequired[str],
         "IpPermissions": NotRequired[Sequence[AwsEc2SecurityGroupIpPermissionTypeDef]],
         "IpPermissionsEgress": NotRequired[Sequence[AwsEc2SecurityGroupIpPermissionTypeDef]],
     },
 )
-AwsEc2VpcPeeringConnectionDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VpcPeeringConnectionDetailsPaginatorTypeDef",
+AwsEc2VpcPeeringConnectionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VpcPeeringConnectionDetailsExtraOutputTypeDef",
+    {
+        "AccepterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsExtraOutputTypeDef],
+        "ExpirationTime": NotRequired[str],
+        "RequesterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsExtraOutputTypeDef],
+        "Status": NotRequired[AwsEc2VpcPeeringConnectionStatusDetailsTypeDef],
+        "VpcPeeringConnectionId": NotRequired[str],
+    },
+)
+AwsEc2VpcPeeringConnectionDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpcPeeringConnectionDetailsOutputTypeDef",
     {
-        "AccepterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsPaginatorTypeDef],
+        "AccepterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef],
         "ExpirationTime": NotRequired[str],
-        "RequesterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsPaginatorTypeDef],
+        "RequesterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef],
         "Status": NotRequired[AwsEc2VpcPeeringConnectionStatusDetailsTypeDef],
         "VpcPeeringConnectionId": NotRequired[str],
     },
 )
 AwsEc2VpcPeeringConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
     {
         "AccepterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef],
         "ExpirationTime": NotRequired[str],
         "RequesterVpcInfo": NotRequired[AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef],
         "Status": NotRequired[AwsEc2VpcPeeringConnectionStatusDetailsTypeDef],
         "VpcPeeringConnectionId": NotRequired[str],
     },
 )
-AwsEc2VpnConnectionDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2VpnConnectionDetailsPaginatorTypeDef",
+AwsEc2VpnConnectionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionDetailsExtraOutputTypeDef",
     {
         "VpnConnectionId": NotRequired[str],
         "State": NotRequired[str],
         "CustomerGatewayId": NotRequired[str],
         "CustomerGatewayConfiguration": NotRequired[str],
         "Type": NotRequired[str],
         "VpnGatewayId": NotRequired[str],
         "Category": NotRequired[str],
         "VgwTelemetry": NotRequired[List[AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef]],
-        "Options": NotRequired[AwsEc2VpnConnectionOptionsDetailsPaginatorTypeDef],
+        "Options": NotRequired[AwsEc2VpnConnectionOptionsDetailsExtraOutputTypeDef],
+        "Routes": NotRequired[List[AwsEc2VpnConnectionRoutesDetailsTypeDef]],
+        "TransitGatewayId": NotRequired[str],
+    },
+)
+AwsEc2VpnConnectionDetailsOutputTypeDef = TypedDict(
+    "AwsEc2VpnConnectionDetailsOutputTypeDef",
+    {
+        "VpnConnectionId": NotRequired[str],
+        "State": NotRequired[str],
+        "CustomerGatewayId": NotRequired[str],
+        "CustomerGatewayConfiguration": NotRequired[str],
+        "Type": NotRequired[str],
+        "VpnGatewayId": NotRequired[str],
+        "Category": NotRequired[str],
+        "VgwTelemetry": NotRequired[List[AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef]],
+        "Options": NotRequired[AwsEc2VpnConnectionOptionsDetailsOutputTypeDef],
         "Routes": NotRequired[List[AwsEc2VpnConnectionRoutesDetailsTypeDef]],
         "TransitGatewayId": NotRequired[str],
     },
 )
 AwsEc2VpnConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionDetailsTypeDef",
     {
@@ -8864,16 +10778,16 @@
     "AwsEcsClusterConfigurationDetailsTypeDef",
     {
         "ExecuteCommandConfiguration": NotRequired[
             AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef
         ],
     },
 )
-AwsEcsServiceDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsServiceDetailsPaginatorTypeDef",
+AwsEcsServiceDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsServiceDetailsExtraOutputTypeDef",
     {
         "CapacityProviderStrategy": NotRequired[
             List[AwsEcsServiceCapacityProviderStrategyDetailsTypeDef]
         ],
         "Cluster": NotRequired[str],
         "DeploymentConfiguration": NotRequired[AwsEcsServiceDeploymentConfigurationDetailsTypeDef],
         "DeploymentController": NotRequired[AwsEcsServiceDeploymentControllerDetailsTypeDef],
@@ -8881,16 +10795,45 @@
         "EnableEcsManagedTags": NotRequired[bool],
         "EnableExecuteCommand": NotRequired[bool],
         "HealthCheckGracePeriodSeconds": NotRequired[int],
         "LaunchType": NotRequired[str],
         "LoadBalancers": NotRequired[List[AwsEcsServiceLoadBalancersDetailsTypeDef]],
         "Name": NotRequired[str],
         "NetworkConfiguration": NotRequired[
-            AwsEcsServiceNetworkConfigurationDetailsPaginatorTypeDef
+            AwsEcsServiceNetworkConfigurationDetailsExtraOutputTypeDef
+        ],
+        "PlacementConstraints": NotRequired[List[AwsEcsServicePlacementConstraintsDetailsTypeDef]],
+        "PlacementStrategies": NotRequired[List[AwsEcsServicePlacementStrategiesDetailsTypeDef]],
+        "PlatformVersion": NotRequired[str],
+        "PropagateTags": NotRequired[str],
+        "Role": NotRequired[str],
+        "SchedulingStrategy": NotRequired[str],
+        "ServiceArn": NotRequired[str],
+        "ServiceName": NotRequired[str],
+        "ServiceRegistries": NotRequired[List[AwsEcsServiceServiceRegistriesDetailsTypeDef]],
+        "TaskDefinition": NotRequired[str],
+    },
+)
+AwsEcsServiceDetailsOutputTypeDef = TypedDict(
+    "AwsEcsServiceDetailsOutputTypeDef",
+    {
+        "CapacityProviderStrategy": NotRequired[
+            List[AwsEcsServiceCapacityProviderStrategyDetailsTypeDef]
         ],
+        "Cluster": NotRequired[str],
+        "DeploymentConfiguration": NotRequired[AwsEcsServiceDeploymentConfigurationDetailsTypeDef],
+        "DeploymentController": NotRequired[AwsEcsServiceDeploymentControllerDetailsTypeDef],
+        "DesiredCount": NotRequired[int],
+        "EnableEcsManagedTags": NotRequired[bool],
+        "EnableExecuteCommand": NotRequired[bool],
+        "HealthCheckGracePeriodSeconds": NotRequired[int],
+        "LaunchType": NotRequired[str],
+        "LoadBalancers": NotRequired[List[AwsEcsServiceLoadBalancersDetailsTypeDef]],
+        "Name": NotRequired[str],
+        "NetworkConfiguration": NotRequired[AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef],
         "PlacementConstraints": NotRequired[List[AwsEcsServicePlacementConstraintsDetailsTypeDef]],
         "PlacementStrategies": NotRequired[List[AwsEcsServicePlacementStrategiesDetailsTypeDef]],
         "PlatformVersion": NotRequired[str],
         "PropagateTags": NotRequired[str],
         "Role": NotRequired[str],
         "SchedulingStrategy": NotRequired[str],
         "ServiceArn": NotRequired[str],
@@ -8928,16 +10871,88 @@
         "SchedulingStrategy": NotRequired[str],
         "ServiceArn": NotRequired[str],
         "ServiceName": NotRequired[str],
         "ServiceRegistries": NotRequired[Sequence[AwsEcsServiceServiceRegistriesDetailsTypeDef]],
         "TaskDefinition": NotRequired[str],
     },
 )
-AwsEcsTaskDefinitionContainerDefinitionsDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsDetailsExtraOutputTypeDef",
+    {
+        "Command": NotRequired[List[str]],
+        "Cpu": NotRequired[int],
+        "DependsOn": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef]
+        ],
+        "DisableNetworking": NotRequired[bool],
+        "DnsSearchDomains": NotRequired[List[str]],
+        "DnsServers": NotRequired[List[str]],
+        "DockerLabels": NotRequired[Dict[str, str]],
+        "DockerSecurityOptions": NotRequired[List[str]],
+        "EntryPoint": NotRequired[List[str]],
+        "Environment": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef]
+        ],
+        "EnvironmentFiles": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef]
+        ],
+        "Essential": NotRequired[bool],
+        "ExtraHosts": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef]
+        ],
+        "FirelensConfiguration": NotRequired[
+            AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsExtraOutputTypeDef
+        ],
+        "HealthCheck": NotRequired[
+            AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsExtraOutputTypeDef
+        ],
+        "Hostname": NotRequired[str],
+        "Image": NotRequired[str],
+        "Interactive": NotRequired[bool],
+        "Links": NotRequired[List[str]],
+        "LinuxParameters": NotRequired[
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsExtraOutputTypeDef
+        ],
+        "LogConfiguration": NotRequired[
+            AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsExtraOutputTypeDef
+        ],
+        "Memory": NotRequired[int],
+        "MemoryReservation": NotRequired[int],
+        "MountPoints": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef]
+        ],
+        "Name": NotRequired[str],
+        "PortMappings": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef]
+        ],
+        "Privileged": NotRequired[bool],
+        "PseudoTerminal": NotRequired[bool],
+        "ReadonlyRootFilesystem": NotRequired[bool],
+        "RepositoryCredentials": NotRequired[
+            AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef
+        ],
+        "ResourceRequirements": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef]
+        ],
+        "Secrets": NotRequired[List[AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef]],
+        "StartTimeout": NotRequired[int],
+        "StopTimeout": NotRequired[int],
+        "SystemControls": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef]
+        ],
+        "Ulimits": NotRequired[List[AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef]],
+        "User": NotRequired[str],
+        "VolumesFrom": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef]
+        ],
+        "WorkingDirectory": NotRequired[str],
+    },
+)
+AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef",
     {
         "Command": NotRequired[List[str]],
         "Cpu": NotRequired[int],
         "DependsOn": NotRequired[
             List[AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef]
         ],
         "DisableNetworking": NotRequired[bool],
@@ -8953,28 +10968,28 @@
             List[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef]
         ],
         "Essential": NotRequired[bool],
         "ExtraHosts": NotRequired[
             List[AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef]
         ],
         "FirelensConfiguration": NotRequired[
-            AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsPaginatorTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef
         ],
         "HealthCheck": NotRequired[
-            AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsPaginatorTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef
         ],
         "Hostname": NotRequired[str],
         "Image": NotRequired[str],
         "Interactive": NotRequired[bool],
         "Links": NotRequired[List[str]],
         "LinuxParameters": NotRequired[
-            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsPaginatorTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef
         ],
         "LogConfiguration": NotRequired[
-            AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsPaginatorTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef
         ],
         "Memory": NotRequired[int],
         "MemoryReservation": NotRequired[int],
         "MountPoints": NotRequired[
             List[AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef]
         ],
         "Name": NotRequired[str],
@@ -9076,19 +11091,32 @@
         "User": NotRequired[str],
         "VolumesFrom": NotRequired[
             Sequence[AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef]
         ],
         "WorkingDirectory": NotRequired[str],
     },
 )
-AwsEcsTaskDefinitionVolumesDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionVolumesDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionVolumesDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesDetailsExtraOutputTypeDef",
+    {
+        "DockerVolumeConfiguration": NotRequired[
+            AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsExtraOutputTypeDef
+        ],
+        "EfsVolumeConfiguration": NotRequired[
+            AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef
+        ],
+        "Host": NotRequired[AwsEcsTaskDefinitionVolumesHostDetailsTypeDef],
+        "Name": NotRequired[str],
+    },
+)
+AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef",
     {
         "DockerVolumeConfiguration": NotRequired[
-            AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsPaginatorTypeDef
+            AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef
         ],
         "EfsVolumeConfiguration": NotRequired[
             AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef
         ],
         "Host": NotRequired[AwsEcsTaskDefinitionVolumesHostDetailsTypeDef],
         "Name": NotRequired[str],
     },
@@ -9102,26 +11130,40 @@
         "EfsVolumeConfiguration": NotRequired[
             AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef
         ],
         "Host": NotRequired[AwsEcsTaskDefinitionVolumesHostDetailsTypeDef],
         "Name": NotRequired[str],
     },
 )
-AwsEcsTaskDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDetailsPaginatorTypeDef",
+AwsEcsTaskDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDetailsExtraOutputTypeDef",
     {
         "ClusterArn": NotRequired[str],
         "TaskDefinitionArn": NotRequired[str],
         "Version": NotRequired[str],
         "CreatedAt": NotRequired[str],
         "StartedAt": NotRequired[str],
         "StartedBy": NotRequired[str],
         "Group": NotRequired[str],
         "Volumes": NotRequired[List[AwsEcsTaskVolumeDetailsTypeDef]],
-        "Containers": NotRequired[List[AwsEcsContainerDetailsPaginatorTypeDef]],
+        "Containers": NotRequired[List[AwsEcsContainerDetailsExtraOutputTypeDef]],
+    },
+)
+AwsEcsTaskDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDetailsOutputTypeDef",
+    {
+        "ClusterArn": NotRequired[str],
+        "TaskDefinitionArn": NotRequired[str],
+        "Version": NotRequired[str],
+        "CreatedAt": NotRequired[str],
+        "StartedAt": NotRequired[str],
+        "StartedBy": NotRequired[str],
+        "Group": NotRequired[str],
+        "Volumes": NotRequired[List[AwsEcsTaskVolumeDetailsTypeDef]],
+        "Containers": NotRequired[List[AwsEcsContainerDetailsOutputTypeDef]],
     },
 )
 AwsEcsTaskDetailsTypeDef = TypedDict(
     "AwsEcsTaskDetailsTypeDef",
     {
         "ClusterArn": NotRequired[str],
         "TaskDefinitionArn": NotRequired[str],
@@ -9130,48 +11172,73 @@
         "StartedAt": NotRequired[str],
         "StartedBy": NotRequired[str],
         "Group": NotRequired[str],
         "Volumes": NotRequired[Sequence[AwsEcsTaskVolumeDetailsTypeDef]],
         "Containers": NotRequired[Sequence[AwsEcsContainerDetailsTypeDef]],
     },
 )
-AwsEfsAccessPointDetailsPaginatorTypeDef = TypedDict(
-    "AwsEfsAccessPointDetailsPaginatorTypeDef",
+AwsEfsAccessPointDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEfsAccessPointDetailsExtraOutputTypeDef",
+    {
+        "AccessPointId": NotRequired[str],
+        "Arn": NotRequired[str],
+        "ClientToken": NotRequired[str],
+        "FileSystemId": NotRequired[str],
+        "PosixUser": NotRequired[AwsEfsAccessPointPosixUserDetailsExtraOutputTypeDef],
+        "RootDirectory": NotRequired[AwsEfsAccessPointRootDirectoryDetailsTypeDef],
+    },
+)
+AwsEfsAccessPointDetailsOutputTypeDef = TypedDict(
+    "AwsEfsAccessPointDetailsOutputTypeDef",
     {
         "AccessPointId": NotRequired[str],
         "Arn": NotRequired[str],
         "ClientToken": NotRequired[str],
         "FileSystemId": NotRequired[str],
-        "PosixUser": NotRequired[AwsEfsAccessPointPosixUserDetailsPaginatorTypeDef],
+        "PosixUser": NotRequired[AwsEfsAccessPointPosixUserDetailsOutputTypeDef],
         "RootDirectory": NotRequired[AwsEfsAccessPointRootDirectoryDetailsTypeDef],
     },
 )
 AwsEfsAccessPointDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointDetailsTypeDef",
     {
         "AccessPointId": NotRequired[str],
         "Arn": NotRequired[str],
         "ClientToken": NotRequired[str],
         "FileSystemId": NotRequired[str],
         "PosixUser": NotRequired[AwsEfsAccessPointPosixUserDetailsTypeDef],
         "RootDirectory": NotRequired[AwsEfsAccessPointRootDirectoryDetailsTypeDef],
     },
 )
-AwsEksClusterDetailsPaginatorTypeDef = TypedDict(
-    "AwsEksClusterDetailsPaginatorTypeDef",
+AwsEksClusterDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEksClusterDetailsExtraOutputTypeDef",
+    {
+        "Arn": NotRequired[str],
+        "CertificateAuthorityData": NotRequired[str],
+        "ClusterStatus": NotRequired[str],
+        "Endpoint": NotRequired[str],
+        "Name": NotRequired[str],
+        "ResourcesVpcConfig": NotRequired[AwsEksClusterResourcesVpcConfigDetailsExtraOutputTypeDef],
+        "RoleArn": NotRequired[str],
+        "Version": NotRequired[str],
+        "Logging": NotRequired[AwsEksClusterLoggingDetailsExtraOutputTypeDef],
+    },
+)
+AwsEksClusterDetailsOutputTypeDef = TypedDict(
+    "AwsEksClusterDetailsOutputTypeDef",
     {
         "Arn": NotRequired[str],
         "CertificateAuthorityData": NotRequired[str],
         "ClusterStatus": NotRequired[str],
         "Endpoint": NotRequired[str],
         "Name": NotRequired[str],
-        "ResourcesVpcConfig": NotRequired[AwsEksClusterResourcesVpcConfigDetailsPaginatorTypeDef],
+        "ResourcesVpcConfig": NotRequired[AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef],
         "RoleArn": NotRequired[str],
         "Version": NotRequired[str],
-        "Logging": NotRequired[AwsEksClusterLoggingDetailsPaginatorTypeDef],
+        "Logging": NotRequired[AwsEksClusterLoggingDetailsOutputTypeDef],
     },
 )
 AwsEksClusterDetailsTypeDef = TypedDict(
     "AwsEksClusterDetailsTypeDef",
     {
         "Arn": NotRequired[str],
         "CertificateAuthorityData": NotRequired[str],
@@ -9180,16 +11247,16 @@
         "Name": NotRequired[str],
         "ResourcesVpcConfig": NotRequired[AwsEksClusterResourcesVpcConfigDetailsTypeDef],
         "RoleArn": NotRequired[str],
         "Version": NotRequired[str],
         "Logging": NotRequired[AwsEksClusterLoggingDetailsTypeDef],
     },
 )
-AwsElasticsearchDomainDetailsPaginatorTypeDef = TypedDict(
-    "AwsElasticsearchDomainDetailsPaginatorTypeDef",
+AwsElasticsearchDomainDetailsExtraOutputTypeDef = TypedDict(
+    "AwsElasticsearchDomainDetailsExtraOutputTypeDef",
     {
         "AccessPolicies": NotRequired[str],
         "DomainEndpointOptions": NotRequired[AwsElasticsearchDomainDomainEndpointOptionsTypeDef],
         "DomainId": NotRequired[str],
         "DomainName": NotRequired[str],
         "Endpoint": NotRequired[str],
         "Endpoints": NotRequired[Dict[str, str]],
@@ -9201,15 +11268,39 @@
             AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef
         ],
         "LogPublishingOptions": NotRequired[AwsElasticsearchDomainLogPublishingOptionsTypeDef],
         "NodeToNodeEncryptionOptions": NotRequired[
             AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef
         ],
         "ServiceSoftwareOptions": NotRequired[AwsElasticsearchDomainServiceSoftwareOptionsTypeDef],
-        "VPCOptions": NotRequired[AwsElasticsearchDomainVPCOptionsPaginatorTypeDef],
+        "VPCOptions": NotRequired[AwsElasticsearchDomainVPCOptionsExtraOutputTypeDef],
+    },
+)
+AwsElasticsearchDomainDetailsOutputTypeDef = TypedDict(
+    "AwsElasticsearchDomainDetailsOutputTypeDef",
+    {
+        "AccessPolicies": NotRequired[str],
+        "DomainEndpointOptions": NotRequired[AwsElasticsearchDomainDomainEndpointOptionsTypeDef],
+        "DomainId": NotRequired[str],
+        "DomainName": NotRequired[str],
+        "Endpoint": NotRequired[str],
+        "Endpoints": NotRequired[Dict[str, str]],
+        "ElasticsearchVersion": NotRequired[str],
+        "ElasticsearchClusterConfig": NotRequired[
+            AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef
+        ],
+        "EncryptionAtRestOptions": NotRequired[
+            AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef
+        ],
+        "LogPublishingOptions": NotRequired[AwsElasticsearchDomainLogPublishingOptionsTypeDef],
+        "NodeToNodeEncryptionOptions": NotRequired[
+            AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef
+        ],
+        "ServiceSoftwareOptions": NotRequired[AwsElasticsearchDomainServiceSoftwareOptionsTypeDef],
+        "VPCOptions": NotRequired[AwsElasticsearchDomainVPCOptionsOutputTypeDef],
     },
 )
 AwsElasticsearchDomainDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainDetailsTypeDef",
     {
         "AccessPolicies": NotRequired[str],
         "DomainEndpointOptions": NotRequired[AwsElasticsearchDomainDomainEndpointOptionsTypeDef],
@@ -9228,33 +11319,59 @@
         "NodeToNodeEncryptionOptions": NotRequired[
             AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef
         ],
         "ServiceSoftwareOptions": NotRequired[AwsElasticsearchDomainServiceSoftwareOptionsTypeDef],
         "VPCOptions": NotRequired[AwsElasticsearchDomainVPCOptionsTypeDef],
     },
 )
-AwsElbLoadBalancerDetailsPaginatorTypeDef = TypedDict(
-    "AwsElbLoadBalancerDetailsPaginatorTypeDef",
+AwsElbLoadBalancerDetailsExtraOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerDetailsExtraOutputTypeDef",
     {
         "AvailabilityZones": NotRequired[List[str]],
         "BackendServerDescriptions": NotRequired[
-            List[AwsElbLoadBalancerBackendServerDescriptionPaginatorTypeDef]
+            List[AwsElbLoadBalancerBackendServerDescriptionExtraOutputTypeDef]
         ],
         "CanonicalHostedZoneName": NotRequired[str],
         "CanonicalHostedZoneNameID": NotRequired[str],
         "CreatedTime": NotRequired[str],
         "DnsName": NotRequired[str],
         "HealthCheck": NotRequired[AwsElbLoadBalancerHealthCheckTypeDef],
         "Instances": NotRequired[List[AwsElbLoadBalancerInstanceTypeDef]],
         "ListenerDescriptions": NotRequired[
-            List[AwsElbLoadBalancerListenerDescriptionPaginatorTypeDef]
+            List[AwsElbLoadBalancerListenerDescriptionExtraOutputTypeDef]
         ],
-        "LoadBalancerAttributes": NotRequired[AwsElbLoadBalancerAttributesPaginatorTypeDef],
+        "LoadBalancerAttributes": NotRequired[AwsElbLoadBalancerAttributesExtraOutputTypeDef],
         "LoadBalancerName": NotRequired[str],
-        "Policies": NotRequired[AwsElbLoadBalancerPoliciesPaginatorTypeDef],
+        "Policies": NotRequired[AwsElbLoadBalancerPoliciesExtraOutputTypeDef],
+        "Scheme": NotRequired[str],
+        "SecurityGroups": NotRequired[List[str]],
+        "SourceSecurityGroup": NotRequired[AwsElbLoadBalancerSourceSecurityGroupTypeDef],
+        "Subnets": NotRequired[List[str]],
+        "VpcId": NotRequired[str],
+    },
+)
+AwsElbLoadBalancerDetailsOutputTypeDef = TypedDict(
+    "AwsElbLoadBalancerDetailsOutputTypeDef",
+    {
+        "AvailabilityZones": NotRequired[List[str]],
+        "BackendServerDescriptions": NotRequired[
+            List[AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef]
+        ],
+        "CanonicalHostedZoneName": NotRequired[str],
+        "CanonicalHostedZoneNameID": NotRequired[str],
+        "CreatedTime": NotRequired[str],
+        "DnsName": NotRequired[str],
+        "HealthCheck": NotRequired[AwsElbLoadBalancerHealthCheckTypeDef],
+        "Instances": NotRequired[List[AwsElbLoadBalancerInstanceTypeDef]],
+        "ListenerDescriptions": NotRequired[
+            List[AwsElbLoadBalancerListenerDescriptionOutputTypeDef]
+        ],
+        "LoadBalancerAttributes": NotRequired[AwsElbLoadBalancerAttributesOutputTypeDef],
+        "LoadBalancerName": NotRequired[str],
+        "Policies": NotRequired[AwsElbLoadBalancerPoliciesOutputTypeDef],
         "Scheme": NotRequired[str],
         "SecurityGroups": NotRequired[List[str]],
         "SourceSecurityGroup": NotRequired[AwsElbLoadBalancerSourceSecurityGroupTypeDef],
         "Subnets": NotRequired[List[str]],
         "VpcId": NotRequired[str],
     },
 )
@@ -9307,21 +11424,36 @@
         "PrincipalType": NotRequired[str],
         "PrincipalName": NotRequired[str],
         "AccountId": NotRequired[str],
         "AccessKeyId": NotRequired[str],
         "SessionContext": NotRequired[AwsIamAccessKeySessionContextTypeDef],
     },
 )
-AwsIamRoleDetailsPaginatorTypeDef = TypedDict(
-    "AwsIamRoleDetailsPaginatorTypeDef",
+AwsIamRoleDetailsExtraOutputTypeDef = TypedDict(
+    "AwsIamRoleDetailsExtraOutputTypeDef",
+    {
+        "AssumeRolePolicyDocument": NotRequired[str],
+        "AttachedManagedPolicies": NotRequired[List[AwsIamAttachedManagedPolicyTypeDef]],
+        "CreateDate": NotRequired[str],
+        "InstanceProfileList": NotRequired[List[AwsIamInstanceProfileExtraOutputTypeDef]],
+        "PermissionsBoundary": NotRequired[AwsIamPermissionsBoundaryTypeDef],
+        "RoleId": NotRequired[str],
+        "RoleName": NotRequired[str],
+        "RolePolicyList": NotRequired[List[AwsIamRolePolicyTypeDef]],
+        "MaxSessionDuration": NotRequired[int],
+        "Path": NotRequired[str],
+    },
+)
+AwsIamRoleDetailsOutputTypeDef = TypedDict(
+    "AwsIamRoleDetailsOutputTypeDef",
     {
         "AssumeRolePolicyDocument": NotRequired[str],
         "AttachedManagedPolicies": NotRequired[List[AwsIamAttachedManagedPolicyTypeDef]],
         "CreateDate": NotRequired[str],
-        "InstanceProfileList": NotRequired[List[AwsIamInstanceProfilePaginatorTypeDef]],
+        "InstanceProfileList": NotRequired[List[AwsIamInstanceProfileOutputTypeDef]],
         "PermissionsBoundary": NotRequired[AwsIamPermissionsBoundaryTypeDef],
         "RoleId": NotRequired[str],
         "RoleName": NotRequired[str],
         "RolePolicyList": NotRequired[List[AwsIamRolePolicyTypeDef]],
         "MaxSessionDuration": NotRequired[int],
         "Path": NotRequired[str],
     },
@@ -9337,34 +11469,59 @@
         "RoleId": NotRequired[str],
         "RoleName": NotRequired[str],
         "RolePolicyList": NotRequired[Sequence[AwsIamRolePolicyTypeDef]],
         "MaxSessionDuration": NotRequired[int],
         "Path": NotRequired[str],
     },
 )
-AwsLambdaFunctionDetailsPaginatorTypeDef = TypedDict(
-    "AwsLambdaFunctionDetailsPaginatorTypeDef",
+AwsLambdaFunctionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionDetailsExtraOutputTypeDef",
     {
         "Code": NotRequired[AwsLambdaFunctionCodeTypeDef],
         "CodeSha256": NotRequired[str],
         "DeadLetterConfig": NotRequired[AwsLambdaFunctionDeadLetterConfigTypeDef],
-        "Environment": NotRequired[AwsLambdaFunctionEnvironmentPaginatorTypeDef],
+        "Environment": NotRequired[AwsLambdaFunctionEnvironmentExtraOutputTypeDef],
         "FunctionName": NotRequired[str],
         "Handler": NotRequired[str],
         "KmsKeyArn": NotRequired[str],
         "LastModified": NotRequired[str],
         "Layers": NotRequired[List[AwsLambdaFunctionLayerTypeDef]],
         "MasterArn": NotRequired[str],
         "MemorySize": NotRequired[int],
         "RevisionId": NotRequired[str],
         "Role": NotRequired[str],
         "Runtime": NotRequired[str],
         "Timeout": NotRequired[int],
         "TracingConfig": NotRequired[AwsLambdaFunctionTracingConfigTypeDef],
-        "VpcConfig": NotRequired[AwsLambdaFunctionVpcConfigPaginatorTypeDef],
+        "VpcConfig": NotRequired[AwsLambdaFunctionVpcConfigExtraOutputTypeDef],
+        "Version": NotRequired[str],
+        "Architectures": NotRequired[List[str]],
+        "PackageType": NotRequired[str],
+    },
+)
+AwsLambdaFunctionDetailsOutputTypeDef = TypedDict(
+    "AwsLambdaFunctionDetailsOutputTypeDef",
+    {
+        "Code": NotRequired[AwsLambdaFunctionCodeTypeDef],
+        "CodeSha256": NotRequired[str],
+        "DeadLetterConfig": NotRequired[AwsLambdaFunctionDeadLetterConfigTypeDef],
+        "Environment": NotRequired[AwsLambdaFunctionEnvironmentOutputTypeDef],
+        "FunctionName": NotRequired[str],
+        "Handler": NotRequired[str],
+        "KmsKeyArn": NotRequired[str],
+        "LastModified": NotRequired[str],
+        "Layers": NotRequired[List[AwsLambdaFunctionLayerTypeDef]],
+        "MasterArn": NotRequired[str],
+        "MemorySize": NotRequired[int],
+        "RevisionId": NotRequired[str],
+        "Role": NotRequired[str],
+        "Runtime": NotRequired[str],
+        "Timeout": NotRequired[int],
+        "TracingConfig": NotRequired[AwsLambdaFunctionTracingConfigTypeDef],
+        "VpcConfig": NotRequired[AwsLambdaFunctionVpcConfigOutputTypeDef],
         "Version": NotRequired[str],
         "Architectures": NotRequired[List[str]],
         "PackageType": NotRequired[str],
     },
 )
 AwsLambdaFunctionDetailsTypeDef = TypedDict(
     "AwsLambdaFunctionDetailsTypeDef",
@@ -9387,36 +11544,48 @@
         "TracingConfig": NotRequired[AwsLambdaFunctionTracingConfigTypeDef],
         "VpcConfig": NotRequired[AwsLambdaFunctionVpcConfigTypeDef],
         "Version": NotRequired[str],
         "Architectures": NotRequired[Sequence[str]],
         "PackageType": NotRequired[str],
     },
 )
-AwsMskClusterClusterInfoClientAuthenticationDetailsPaginatorTypeDef = TypedDict(
-    "AwsMskClusterClusterInfoClientAuthenticationDetailsPaginatorTypeDef",
+AwsMskClusterClusterInfoClientAuthenticationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsMskClusterClusterInfoClientAuthenticationDetailsExtraOutputTypeDef",
+    {
+        "Sasl": NotRequired[AwsMskClusterClusterInfoClientAuthenticationSaslDetailsTypeDef],
+        "Unauthenticated": NotRequired[
+            AwsMskClusterClusterInfoClientAuthenticationUnauthenticatedDetailsTypeDef
+        ],
+        "Tls": NotRequired[
+            AwsMskClusterClusterInfoClientAuthenticationTlsDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsMskClusterClusterInfoClientAuthenticationDetailsOutputTypeDef = TypedDict(
+    "AwsMskClusterClusterInfoClientAuthenticationDetailsOutputTypeDef",
     {
         "Sasl": NotRequired[AwsMskClusterClusterInfoClientAuthenticationSaslDetailsTypeDef],
         "Unauthenticated": NotRequired[
             AwsMskClusterClusterInfoClientAuthenticationUnauthenticatedDetailsTypeDef
         ],
-        "Tls": NotRequired[AwsMskClusterClusterInfoClientAuthenticationTlsDetailsPaginatorTypeDef],
+        "Tls": NotRequired[AwsMskClusterClusterInfoClientAuthenticationTlsDetailsOutputTypeDef],
     },
 )
 AwsMskClusterClusterInfoClientAuthenticationDetailsTypeDef = TypedDict(
     "AwsMskClusterClusterInfoClientAuthenticationDetailsTypeDef",
     {
         "Sasl": NotRequired[AwsMskClusterClusterInfoClientAuthenticationSaslDetailsTypeDef],
         "Unauthenticated": NotRequired[
             AwsMskClusterClusterInfoClientAuthenticationUnauthenticatedDetailsTypeDef
         ],
         "Tls": NotRequired[AwsMskClusterClusterInfoClientAuthenticationTlsDetailsTypeDef],
     },
 )
-AwsOpenSearchServiceDomainDetailsPaginatorTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainDetailsPaginatorTypeDef",
+AwsOpenSearchServiceDomainDetailsExtraOutputTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainDetailsExtraOutputTypeDef",
     {
         "Arn": NotRequired[str],
         "AccessPolicies": NotRequired[str],
         "DomainName": NotRequired[str],
         "Id": NotRequired[str],
         "DomainEndpoint": NotRequired[str],
         "EngineVersion": NotRequired[str],
@@ -9429,15 +11598,47 @@
         "ServiceSoftwareOptions": NotRequired[
             AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef
         ],
         "ClusterConfig": NotRequired[AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef],
         "DomainEndpointOptions": NotRequired[
             AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef
         ],
-        "VpcOptions": NotRequired[AwsOpenSearchServiceDomainVpcOptionsDetailsPaginatorTypeDef],
+        "VpcOptions": NotRequired[AwsOpenSearchServiceDomainVpcOptionsDetailsExtraOutputTypeDef],
+        "LogPublishingOptions": NotRequired[
+            AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef
+        ],
+        "DomainEndpoints": NotRequired[Dict[str, str]],
+        "AdvancedSecurityOptions": NotRequired[
+            AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef
+        ],
+    },
+)
+AwsOpenSearchServiceDomainDetailsOutputTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainDetailsOutputTypeDef",
+    {
+        "Arn": NotRequired[str],
+        "AccessPolicies": NotRequired[str],
+        "DomainName": NotRequired[str],
+        "Id": NotRequired[str],
+        "DomainEndpoint": NotRequired[str],
+        "EngineVersion": NotRequired[str],
+        "EncryptionAtRestOptions": NotRequired[
+            AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef
+        ],
+        "NodeToNodeEncryptionOptions": NotRequired[
+            AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef
+        ],
+        "ServiceSoftwareOptions": NotRequired[
+            AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef
+        ],
+        "ClusterConfig": NotRequired[AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef],
+        "DomainEndpointOptions": NotRequired[
+            AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef
+        ],
+        "VpcOptions": NotRequired[AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef],
         "LogPublishingOptions": NotRequired[
             AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef
         ],
         "DomainEndpoints": NotRequired[Dict[str, str]],
         "AdvancedSecurityOptions": NotRequired[
             AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef
         ],
@@ -9471,16 +11672,27 @@
         ],
         "DomainEndpoints": NotRequired[Mapping[str, str]],
         "AdvancedSecurityOptions": NotRequired[
             AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef
         ],
     },
 )
-AwsRdsDbSubnetGroupPaginatorTypeDef = TypedDict(
-    "AwsRdsDbSubnetGroupPaginatorTypeDef",
+AwsRdsDbSubnetGroupExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbSubnetGroupExtraOutputTypeDef",
+    {
+        "DbSubnetGroupName": NotRequired[str],
+        "DbSubnetGroupDescription": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "SubnetGroupStatus": NotRequired[str],
+        "Subnets": NotRequired[List[AwsRdsDbSubnetGroupSubnetTypeDef]],
+        "DbSubnetGroupArn": NotRequired[str],
+    },
+)
+AwsRdsDbSubnetGroupOutputTypeDef = TypedDict(
+    "AwsRdsDbSubnetGroupOutputTypeDef",
     {
         "DbSubnetGroupName": NotRequired[str],
         "DbSubnetGroupDescription": NotRequired[str],
         "VpcId": NotRequired[str],
         "SubnetGroupStatus": NotRequired[str],
         "Subnets": NotRequired[List[AwsRdsDbSubnetGroupSubnetTypeDef]],
         "DbSubnetGroupArn": NotRequired[str],
@@ -9493,26 +11705,81 @@
         "DbSubnetGroupDescription": NotRequired[str],
         "VpcId": NotRequired[str],
         "SubnetGroupStatus": NotRequired[str],
         "Subnets": NotRequired[Sequence[AwsRdsDbSubnetGroupSubnetTypeDef]],
         "DbSubnetGroupArn": NotRequired[str],
     },
 )
-AwsRedshiftClusterDetailsPaginatorTypeDef = TypedDict(
-    "AwsRedshiftClusterDetailsPaginatorTypeDef",
+AwsRedshiftClusterDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRedshiftClusterDetailsExtraOutputTypeDef",
+    {
+        "AllowVersionUpgrade": NotRequired[bool],
+        "AutomatedSnapshotRetentionPeriod": NotRequired[int],
+        "AvailabilityZone": NotRequired[str],
+        "ClusterAvailabilityStatus": NotRequired[str],
+        "ClusterCreateTime": NotRequired[str],
+        "ClusterIdentifier": NotRequired[str],
+        "ClusterNodes": NotRequired[List[AwsRedshiftClusterClusterNodeTypeDef]],
+        "ClusterParameterGroups": NotRequired[
+            List[AwsRedshiftClusterClusterParameterGroupExtraOutputTypeDef]
+        ],
+        "ClusterPublicKey": NotRequired[str],
+        "ClusterRevisionNumber": NotRequired[str],
+        "ClusterSecurityGroups": NotRequired[List[AwsRedshiftClusterClusterSecurityGroupTypeDef]],
+        "ClusterSnapshotCopyStatus": NotRequired[
+            AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef
+        ],
+        "ClusterStatus": NotRequired[str],
+        "ClusterSubnetGroupName": NotRequired[str],
+        "ClusterVersion": NotRequired[str],
+        "DBName": NotRequired[str],
+        "DeferredMaintenanceWindows": NotRequired[
+            List[AwsRedshiftClusterDeferredMaintenanceWindowTypeDef]
+        ],
+        "ElasticIpStatus": NotRequired[AwsRedshiftClusterElasticIpStatusTypeDef],
+        "ElasticResizeNumberOfNodeOptions": NotRequired[str],
+        "Encrypted": NotRequired[bool],
+        "Endpoint": NotRequired[AwsRedshiftClusterEndpointTypeDef],
+        "EnhancedVpcRouting": NotRequired[bool],
+        "ExpectedNextSnapshotScheduleTime": NotRequired[str],
+        "ExpectedNextSnapshotScheduleTimeStatus": NotRequired[str],
+        "HsmStatus": NotRequired[AwsRedshiftClusterHsmStatusTypeDef],
+        "IamRoles": NotRequired[List[AwsRedshiftClusterIamRoleTypeDef]],
+        "KmsKeyId": NotRequired[str],
+        "MaintenanceTrackName": NotRequired[str],
+        "ManualSnapshotRetentionPeriod": NotRequired[int],
+        "MasterUsername": NotRequired[str],
+        "NextMaintenanceWindowStartTime": NotRequired[str],
+        "NodeType": NotRequired[str],
+        "NumberOfNodes": NotRequired[int],
+        "PendingActions": NotRequired[List[str]],
+        "PendingModifiedValues": NotRequired[AwsRedshiftClusterPendingModifiedValuesTypeDef],
+        "PreferredMaintenanceWindow": NotRequired[str],
+        "PubliclyAccessible": NotRequired[bool],
+        "ResizeInfo": NotRequired[AwsRedshiftClusterResizeInfoTypeDef],
+        "RestoreStatus": NotRequired[AwsRedshiftClusterRestoreStatusTypeDef],
+        "SnapshotScheduleIdentifier": NotRequired[str],
+        "SnapshotScheduleState": NotRequired[str],
+        "VpcId": NotRequired[str],
+        "VpcSecurityGroups": NotRequired[List[AwsRedshiftClusterVpcSecurityGroupTypeDef]],
+        "LoggingStatus": NotRequired[AwsRedshiftClusterLoggingStatusTypeDef],
+    },
+)
+AwsRedshiftClusterDetailsOutputTypeDef = TypedDict(
+    "AwsRedshiftClusterDetailsOutputTypeDef",
     {
         "AllowVersionUpgrade": NotRequired[bool],
         "AutomatedSnapshotRetentionPeriod": NotRequired[int],
         "AvailabilityZone": NotRequired[str],
         "ClusterAvailabilityStatus": NotRequired[str],
         "ClusterCreateTime": NotRequired[str],
         "ClusterIdentifier": NotRequired[str],
         "ClusterNodes": NotRequired[List[AwsRedshiftClusterClusterNodeTypeDef]],
         "ClusterParameterGroups": NotRequired[
-            List[AwsRedshiftClusterClusterParameterGroupPaginatorTypeDef]
+            List[AwsRedshiftClusterClusterParameterGroupOutputTypeDef]
         ],
         "ClusterPublicKey": NotRequired[str],
         "ClusterRevisionNumber": NotRequired[str],
         "ClusterSecurityGroups": NotRequired[List[AwsRedshiftClusterClusterSecurityGroupTypeDef]],
         "ClusterSnapshotCopyStatus": NotRequired[
             AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef
         ],
@@ -9605,16 +11872,25 @@
         "SnapshotScheduleIdentifier": NotRequired[str],
         "SnapshotScheduleState": NotRequired[str],
         "VpcId": NotRequired[str],
         "VpcSecurityGroups": NotRequired[Sequence[AwsRedshiftClusterVpcSecurityGroupTypeDef]],
         "LoggingStatus": NotRequired[AwsRedshiftClusterLoggingStatusTypeDef],
     },
 )
-AwsRoute53HostedZoneDetailsPaginatorTypeDef = TypedDict(
-    "AwsRoute53HostedZoneDetailsPaginatorTypeDef",
+AwsRoute53HostedZoneDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRoute53HostedZoneDetailsExtraOutputTypeDef",
+    {
+        "HostedZone": NotRequired[AwsRoute53HostedZoneObjectDetailsTypeDef],
+        "Vpcs": NotRequired[List[AwsRoute53HostedZoneVpcDetailsTypeDef]],
+        "NameServers": NotRequired[List[str]],
+        "QueryLoggingConfig": NotRequired[AwsRoute53QueryLoggingConfigDetailsTypeDef],
+    },
+)
+AwsRoute53HostedZoneDetailsOutputTypeDef = TypedDict(
+    "AwsRoute53HostedZoneDetailsOutputTypeDef",
     {
         "HostedZone": NotRequired[AwsRoute53HostedZoneObjectDetailsTypeDef],
         "Vpcs": NotRequired[List[AwsRoute53HostedZoneVpcDetailsTypeDef]],
         "NameServers": NotRequired[List[str]],
         "QueryLoggingConfig": NotRequired[AwsRoute53QueryLoggingConfigDetailsTypeDef],
     },
 )
@@ -9623,16 +11899,29 @@
     {
         "HostedZone": NotRequired[AwsRoute53HostedZoneObjectDetailsTypeDef],
         "Vpcs": NotRequired[Sequence[AwsRoute53HostedZoneVpcDetailsTypeDef]],
         "NameServers": NotRequired[Sequence[str]],
         "QueryLoggingConfig": NotRequired[AwsRoute53QueryLoggingConfigDetailsTypeDef],
     },
 )
-AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsPaginatorTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsPaginatorTypeDef",
+AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsExtraOutputTypeDef",
+    {
+        "Operands": NotRequired[
+            List[AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef]
+        ],
+        "Prefix": NotRequired[str],
+        "Tag": NotRequired[
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef
+        ],
+        "Type": NotRequired[str],
+    },
+)
+AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef",
     {
         "Operands": NotRequired[
             List[AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef]
         ],
         "Prefix": NotRequired[str],
         "Tag": NotRequired[
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef
@@ -9651,18 +11940,26 @@
         "Prefix": NotRequired[str],
         "Tag": NotRequired[
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef
         ],
         "Type": NotRequired[str],
     },
 )
-AwsS3BucketNotificationConfigurationFilterPaginatorTypeDef = TypedDict(
-    "AwsS3BucketNotificationConfigurationFilterPaginatorTypeDef",
+AwsS3BucketNotificationConfigurationFilterExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationFilterExtraOutputTypeDef",
+    {
+        "S3KeyFilter": NotRequired[
+            AwsS3BucketNotificationConfigurationS3KeyFilterExtraOutputTypeDef
+        ],
+    },
+)
+AwsS3BucketNotificationConfigurationFilterOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationFilterOutputTypeDef",
     {
-        "S3KeyFilter": NotRequired[AwsS3BucketNotificationConfigurationS3KeyFilterPaginatorTypeDef],
+        "S3KeyFilter": NotRequired[AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef],
     },
 )
 AwsS3BucketNotificationConfigurationFilterTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
     {
         "S3KeyFilter": NotRequired[AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef],
     },
@@ -9670,28 +11967,43 @@
 AwsS3BucketObjectLockConfigurationTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationTypeDef",
     {
         "ObjectLockEnabled": NotRequired[str],
         "Rule": NotRequired[AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef],
     },
 )
-AwsS3BucketServerSideEncryptionConfigurationPaginatorTypeDef = TypedDict(
-    "AwsS3BucketServerSideEncryptionConfigurationPaginatorTypeDef",
+AwsS3BucketServerSideEncryptionConfigurationExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketServerSideEncryptionConfigurationExtraOutputTypeDef",
+    {
+        "Rules": NotRequired[List[AwsS3BucketServerSideEncryptionRuleTypeDef]],
+    },
+)
+AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
+    "AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef",
     {
         "Rules": NotRequired[List[AwsS3BucketServerSideEncryptionRuleTypeDef]],
     },
 )
 AwsS3BucketServerSideEncryptionConfigurationTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
     {
         "Rules": NotRequired[Sequence[AwsS3BucketServerSideEncryptionRuleTypeDef]],
     },
 )
-AwsS3BucketWebsiteConfigurationPaginatorTypeDef = TypedDict(
-    "AwsS3BucketWebsiteConfigurationPaginatorTypeDef",
+AwsS3BucketWebsiteConfigurationExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketWebsiteConfigurationExtraOutputTypeDef",
+    {
+        "ErrorDocument": NotRequired[str],
+        "IndexDocumentSuffix": NotRequired[str],
+        "RedirectAllRequestsTo": NotRequired[AwsS3BucketWebsiteConfigurationRedirectToTypeDef],
+        "RoutingRules": NotRequired[List[AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef]],
+    },
+)
+AwsS3BucketWebsiteConfigurationOutputTypeDef = TypedDict(
+    "AwsS3BucketWebsiteConfigurationOutputTypeDef",
     {
         "ErrorDocument": NotRequired[str],
         "IndexDocumentSuffix": NotRequired[str],
         "RedirectAllRequestsTo": NotRequired[AwsS3BucketWebsiteConfigurationRedirectToTypeDef],
         "RoutingRules": NotRequired[List[AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef]],
     },
 )
@@ -9714,16 +12026,26 @@
 )
 AwsSsmPatchComplianceDetailsTypeDef = TypedDict(
     "AwsSsmPatchComplianceDetailsTypeDef",
     {
         "Patch": NotRequired[AwsSsmPatchTypeDef],
     },
 )
-AwsStepFunctionStateMachineLoggingConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsStepFunctionStateMachineLoggingConfigurationDetailsPaginatorTypeDef",
+AwsStepFunctionStateMachineLoggingConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsExtraOutputTypeDef",
+    {
+        "Destinations": NotRequired[
+            List[AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef]
+        ],
+        "IncludeExecutionData": NotRequired[bool],
+        "Level": NotRequired[str],
+    },
+)
+AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef",
     {
         "Destinations": NotRequired[
             List[AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef]
         ],
         "IncludeExecutionData": NotRequired[bool],
         "Level": NotRequired[str],
     },
@@ -9734,16 +12056,25 @@
         "Destinations": NotRequired[
             Sequence[AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef]
         ],
         "IncludeExecutionData": NotRequired[bool],
         "Level": NotRequired[str],
     },
 )
-AwsWafRegionalRuleGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafRegionalRuleGroupDetailsPaginatorTypeDef",
+AwsWafRegionalRuleGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafRegionalRuleGroupDetailsExtraOutputTypeDef",
+    {
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "RuleGroupId": NotRequired[str],
+        "Rules": NotRequired[List[AwsWafRegionalRuleGroupRulesDetailsTypeDef]],
+    },
+)
+AwsWafRegionalRuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalRuleGroupDetailsOutputTypeDef",
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RuleGroupId": NotRequired[str],
         "Rules": NotRequired[List[AwsWafRegionalRuleGroupRulesDetailsTypeDef]],
     },
 )
@@ -9752,16 +12083,26 @@
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RuleGroupId": NotRequired[str],
         "Rules": NotRequired[Sequence[AwsWafRegionalRuleGroupRulesDetailsTypeDef]],
     },
 )
-AwsWafRegionalWebAclDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafRegionalWebAclDetailsPaginatorTypeDef",
+AwsWafRegionalWebAclDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafRegionalWebAclDetailsExtraOutputTypeDef",
+    {
+        "DefaultAction": NotRequired[str],
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "RulesList": NotRequired[List[AwsWafRegionalWebAclRulesListDetailsTypeDef]],
+        "WebAclId": NotRequired[str],
+    },
+)
+AwsWafRegionalWebAclDetailsOutputTypeDef = TypedDict(
+    "AwsWafRegionalWebAclDetailsOutputTypeDef",
     {
         "DefaultAction": NotRequired[str],
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RulesList": NotRequired[List[AwsWafRegionalWebAclRulesListDetailsTypeDef]],
         "WebAclId": NotRequired[str],
     },
@@ -9772,16 +12113,25 @@
         "DefaultAction": NotRequired[str],
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RulesList": NotRequired[Sequence[AwsWafRegionalWebAclRulesListDetailsTypeDef]],
         "WebAclId": NotRequired[str],
     },
 )
-AwsWafRuleGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafRuleGroupDetailsPaginatorTypeDef",
+AwsWafRuleGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafRuleGroupDetailsExtraOutputTypeDef",
+    {
+        "MetricName": NotRequired[str],
+        "Name": NotRequired[str],
+        "RuleGroupId": NotRequired[str],
+        "Rules": NotRequired[List[AwsWafRuleGroupRulesDetailsTypeDef]],
+    },
+)
+AwsWafRuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsWafRuleGroupDetailsOutputTypeDef",
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RuleGroupId": NotRequired[str],
         "Rules": NotRequired[List[AwsWafRuleGroupRulesDetailsTypeDef]],
     },
 )
@@ -9790,48 +12140,81 @@
     {
         "MetricName": NotRequired[str],
         "Name": NotRequired[str],
         "RuleGroupId": NotRequired[str],
         "Rules": NotRequired[Sequence[AwsWafRuleGroupRulesDetailsTypeDef]],
     },
 )
-AwsWafWebAclDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafWebAclDetailsPaginatorTypeDef",
+AwsWafWebAclDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafWebAclDetailsExtraOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "DefaultAction": NotRequired[str],
+        "Rules": NotRequired[List[AwsWafWebAclRuleExtraOutputTypeDef]],
+        "WebAclId": NotRequired[str],
+    },
+)
+AwsWafWebAclDetailsOutputTypeDef = TypedDict(
+    "AwsWafWebAclDetailsOutputTypeDef",
     {
         "Name": NotRequired[str],
         "DefaultAction": NotRequired[str],
-        "Rules": NotRequired[List[AwsWafWebAclRulePaginatorTypeDef]],
+        "Rules": NotRequired[List[AwsWafWebAclRuleOutputTypeDef]],
         "WebAclId": NotRequired[str],
     },
 )
 AwsWafWebAclDetailsTypeDef = TypedDict(
     "AwsWafWebAclDetailsTypeDef",
     {
         "Name": NotRequired[str],
         "DefaultAction": NotRequired[str],
         "Rules": NotRequired[Sequence[AwsWafWebAclRuleTypeDef]],
         "WebAclId": NotRequired[str],
     },
 )
-AwsWafv2ActionAllowDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2ActionAllowDetailsPaginatorTypeDef",
+AwsWafv2ActionAllowDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2ActionAllowDetailsExtraOutputTypeDef",
     {
-        "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsPaginatorTypeDef],
+        "CustomRequestHandling": NotRequired[
+            AwsWafv2CustomRequestHandlingDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsWafv2RulesActionCaptchaDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionCaptchaDetailsExtraOutputTypeDef",
+    {
+        "CustomRequestHandling": NotRequired[
+            AwsWafv2CustomRequestHandlingDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsWafv2RulesActionCountDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionCountDetailsExtraOutputTypeDef",
+    {
+        "CustomRequestHandling": NotRequired[
+            AwsWafv2CustomRequestHandlingDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsWafv2ActionAllowDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2ActionAllowDetailsOutputTypeDef",
+    {
+        "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsOutputTypeDef],
     },
 )
-AwsWafv2RulesActionCaptchaDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2RulesActionCaptchaDetailsPaginatorTypeDef",
+AwsWafv2RulesActionCaptchaDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionCaptchaDetailsOutputTypeDef",
     {
-        "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsPaginatorTypeDef],
+        "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsOutputTypeDef],
     },
 )
-AwsWafv2RulesActionCountDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2RulesActionCountDetailsPaginatorTypeDef",
+AwsWafv2RulesActionCountDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionCountDetailsOutputTypeDef",
     {
-        "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsPaginatorTypeDef],
+        "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsOutputTypeDef],
     },
 )
 AwsWafv2ActionAllowDetailsTypeDef = TypedDict(
     "AwsWafv2ActionAllowDetailsTypeDef",
     {
         "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsTypeDef],
     },
@@ -9844,18 +12227,24 @@
 )
 AwsWafv2RulesActionCountDetailsTypeDef = TypedDict(
     "AwsWafv2RulesActionCountDetailsTypeDef",
     {
         "CustomRequestHandling": NotRequired[AwsWafv2CustomRequestHandlingDetailsTypeDef],
     },
 )
-AwsWafv2ActionBlockDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2ActionBlockDetailsPaginatorTypeDef",
+AwsWafv2ActionBlockDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2ActionBlockDetailsExtraOutputTypeDef",
+    {
+        "CustomResponse": NotRequired[AwsWafv2CustomResponseDetailsExtraOutputTypeDef],
+    },
+)
+AwsWafv2ActionBlockDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2ActionBlockDetailsOutputTypeDef",
     {
-        "CustomResponse": NotRequired[AwsWafv2CustomResponseDetailsPaginatorTypeDef],
+        "CustomResponse": NotRequired[AwsWafv2CustomResponseDetailsOutputTypeDef],
     },
 )
 AwsWafv2ActionBlockDetailsTypeDef = TypedDict(
     "AwsWafv2ActionBlockDetailsTypeDef",
     {
         "CustomResponse": NotRequired[AwsWafv2CustomResponseDetailsTypeDef],
     },
@@ -9871,28 +12260,46 @@
 BatchUpdateStandardsControlAssociationsResponseTypeDef = TypedDict(
     "BatchUpdateStandardsControlAssociationsResponseTypeDef",
     {
         "UnprocessedAssociationUpdates": List[UnprocessedStandardsControlAssociationUpdateTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-VulnerabilityPaginatorTypeDef = TypedDict(
-    "VulnerabilityPaginatorTypeDef",
+VulnerabilityExtraOutputTypeDef = TypedDict(
+    "VulnerabilityExtraOutputTypeDef",
     {
         "Id": str,
         "VulnerablePackages": NotRequired[List[SoftwarePackageTypeDef]],
-        "Cvss": NotRequired[List[CvssPaginatorTypeDef]],
+        "Cvss": NotRequired[List[CvssExtraOutputTypeDef]],
         "RelatedVulnerabilities": NotRequired[List[str]],
         "Vendor": NotRequired[VulnerabilityVendorTypeDef],
         "ReferenceUrls": NotRequired[List[str]],
         "FixAvailable": NotRequired[VulnerabilityFixAvailableType],
         "EpssScore": NotRequired[float],
         "ExploitAvailable": NotRequired[VulnerabilityExploitAvailableType],
         "LastKnownExploitAt": NotRequired[str],
-        "CodeVulnerabilities": NotRequired[List[VulnerabilityCodeVulnerabilitiesPaginatorTypeDef]],
+        "CodeVulnerabilities": NotRequired[
+            List[VulnerabilityCodeVulnerabilitiesExtraOutputTypeDef]
+        ],
+    },
+)
+VulnerabilityOutputTypeDef = TypedDict(
+    "VulnerabilityOutputTypeDef",
+    {
+        "Id": str,
+        "VulnerablePackages": NotRequired[List[SoftwarePackageTypeDef]],
+        "Cvss": NotRequired[List[CvssOutputTypeDef]],
+        "RelatedVulnerabilities": NotRequired[List[str]],
+        "Vendor": NotRequired[VulnerabilityVendorTypeDef],
+        "ReferenceUrls": NotRequired[List[str]],
+        "FixAvailable": NotRequired[VulnerabilityFixAvailableType],
+        "EpssScore": NotRequired[float],
+        "ExploitAvailable": NotRequired[VulnerabilityExploitAvailableType],
+        "LastKnownExploitAt": NotRequired[str],
+        "CodeVulnerabilities": NotRequired[List[VulnerabilityCodeVulnerabilitiesOutputTypeDef]],
     },
 )
 VulnerabilityTypeDef = TypedDict(
     "VulnerabilityTypeDef",
     {
         "Id": str,
         "VulnerablePackages": NotRequired[Sequence[SoftwarePackageTypeDef]],
@@ -9928,16 +12335,16 @@
         "ConfigurationPolicyAssociationIdentifiers": NotRequired[
             ConfigurationPolicyAssociationTypeDef
         ],
         "ErrorCode": NotRequired[str],
         "ErrorReason": NotRequired[str],
     },
 )
-AutomationRulesFindingFiltersTypeDef = TypedDict(
-    "AutomationRulesFindingFiltersTypeDef",
+AutomationRulesFindingFiltersOutputTypeDef = TypedDict(
+    "AutomationRulesFindingFiltersOutputTypeDef",
     {
         "ProductArn": NotRequired[List[StringFilterTypeDef]],
         "AwsAccountId": NotRequired[List[StringFilterTypeDef]],
         "Id": NotRequired[List[StringFilterTypeDef]],
         "GeneratorId": NotRequired[List[StringFilterTypeDef]],
         "Type": NotRequired[List[StringFilterTypeDef]],
         "FirstObservedAt": NotRequired[List[DateFilterTypeDef]],
@@ -9971,14 +12378,275 @@
         "NoteUpdatedBy": NotRequired[List[StringFilterTypeDef]],
         "UserDefinedFields": NotRequired[List[MapFilterTypeDef]],
         "ResourceApplicationArn": NotRequired[List[StringFilterTypeDef]],
         "ResourceApplicationName": NotRequired[List[StringFilterTypeDef]],
         "AwsAccountName": NotRequired[List[StringFilterTypeDef]],
     },
 )
+AutomationRulesFindingFiltersTypeDef = TypedDict(
+    "AutomationRulesFindingFiltersTypeDef",
+    {
+        "ProductArn": NotRequired[Sequence[StringFilterTypeDef]],
+        "AwsAccountId": NotRequired[Sequence[StringFilterTypeDef]],
+        "Id": NotRequired[Sequence[StringFilterTypeDef]],
+        "GeneratorId": NotRequired[Sequence[StringFilterTypeDef]],
+        "Type": NotRequired[Sequence[StringFilterTypeDef]],
+        "FirstObservedAt": NotRequired[Sequence[DateFilterTypeDef]],
+        "LastObservedAt": NotRequired[Sequence[DateFilterTypeDef]],
+        "CreatedAt": NotRequired[Sequence[DateFilterTypeDef]],
+        "UpdatedAt": NotRequired[Sequence[DateFilterTypeDef]],
+        "Confidence": NotRequired[Sequence[NumberFilterTypeDef]],
+        "Criticality": NotRequired[Sequence[NumberFilterTypeDef]],
+        "Title": NotRequired[Sequence[StringFilterTypeDef]],
+        "Description": NotRequired[Sequence[StringFilterTypeDef]],
+        "SourceUrl": NotRequired[Sequence[StringFilterTypeDef]],
+        "ProductName": NotRequired[Sequence[StringFilterTypeDef]],
+        "CompanyName": NotRequired[Sequence[StringFilterTypeDef]],
+        "SeverityLabel": NotRequired[Sequence[StringFilterTypeDef]],
+        "ResourceType": NotRequired[Sequence[StringFilterTypeDef]],
+        "ResourceId": NotRequired[Sequence[StringFilterTypeDef]],
+        "ResourcePartition": NotRequired[Sequence[StringFilterTypeDef]],
+        "ResourceRegion": NotRequired[Sequence[StringFilterTypeDef]],
+        "ResourceTags": NotRequired[Sequence[MapFilterTypeDef]],
+        "ResourceDetailsOther": NotRequired[Sequence[MapFilterTypeDef]],
+        "ComplianceStatus": NotRequired[Sequence[StringFilterTypeDef]],
+        "ComplianceSecurityControlId": NotRequired[Sequence[StringFilterTypeDef]],
+        "ComplianceAssociatedStandardsId": NotRequired[Sequence[StringFilterTypeDef]],
+        "VerificationState": NotRequired[Sequence[StringFilterTypeDef]],
+        "WorkflowStatus": NotRequired[Sequence[StringFilterTypeDef]],
+        "RecordState": NotRequired[Sequence[StringFilterTypeDef]],
+        "RelatedFindingsProductArn": NotRequired[Sequence[StringFilterTypeDef]],
+        "RelatedFindingsId": NotRequired[Sequence[StringFilterTypeDef]],
+        "NoteText": NotRequired[Sequence[StringFilterTypeDef]],
+        "NoteUpdatedAt": NotRequired[Sequence[DateFilterTypeDef]],
+        "NoteUpdatedBy": NotRequired[Sequence[StringFilterTypeDef]],
+        "UserDefinedFields": NotRequired[Sequence[MapFilterTypeDef]],
+        "ResourceApplicationArn": NotRequired[Sequence[StringFilterTypeDef]],
+        "ResourceApplicationName": NotRequired[Sequence[StringFilterTypeDef]],
+        "AwsAccountName": NotRequired[Sequence[StringFilterTypeDef]],
+    },
+)
+AwsSecurityFindingFiltersExtraOutputTypeDef = TypedDict(
+    "AwsSecurityFindingFiltersExtraOutputTypeDef",
+    {
+        "ProductArn": NotRequired[List[StringFilterTypeDef]],
+        "AwsAccountId": NotRequired[List[StringFilterTypeDef]],
+        "Id": NotRequired[List[StringFilterTypeDef]],
+        "GeneratorId": NotRequired[List[StringFilterTypeDef]],
+        "Region": NotRequired[List[StringFilterTypeDef]],
+        "Type": NotRequired[List[StringFilterTypeDef]],
+        "FirstObservedAt": NotRequired[List[DateFilterTypeDef]],
+        "LastObservedAt": NotRequired[List[DateFilterTypeDef]],
+        "CreatedAt": NotRequired[List[DateFilterTypeDef]],
+        "UpdatedAt": NotRequired[List[DateFilterTypeDef]],
+        "SeverityProduct": NotRequired[List[NumberFilterTypeDef]],
+        "SeverityNormalized": NotRequired[List[NumberFilterTypeDef]],
+        "SeverityLabel": NotRequired[List[StringFilterTypeDef]],
+        "Confidence": NotRequired[List[NumberFilterTypeDef]],
+        "Criticality": NotRequired[List[NumberFilterTypeDef]],
+        "Title": NotRequired[List[StringFilterTypeDef]],
+        "Description": NotRequired[List[StringFilterTypeDef]],
+        "RecommendationText": NotRequired[List[StringFilterTypeDef]],
+        "SourceUrl": NotRequired[List[StringFilterTypeDef]],
+        "ProductFields": NotRequired[List[MapFilterTypeDef]],
+        "ProductName": NotRequired[List[StringFilterTypeDef]],
+        "CompanyName": NotRequired[List[StringFilterTypeDef]],
+        "UserDefinedFields": NotRequired[List[MapFilterTypeDef]],
+        "MalwareName": NotRequired[List[StringFilterTypeDef]],
+        "MalwareType": NotRequired[List[StringFilterTypeDef]],
+        "MalwarePath": NotRequired[List[StringFilterTypeDef]],
+        "MalwareState": NotRequired[List[StringFilterTypeDef]],
+        "NetworkDirection": NotRequired[List[StringFilterTypeDef]],
+        "NetworkProtocol": NotRequired[List[StringFilterTypeDef]],
+        "NetworkSourceIpV4": NotRequired[List[IpFilterTypeDef]],
+        "NetworkSourceIpV6": NotRequired[List[IpFilterTypeDef]],
+        "NetworkSourcePort": NotRequired[List[NumberFilterTypeDef]],
+        "NetworkSourceDomain": NotRequired[List[StringFilterTypeDef]],
+        "NetworkSourceMac": NotRequired[List[StringFilterTypeDef]],
+        "NetworkDestinationIpV4": NotRequired[List[IpFilterTypeDef]],
+        "NetworkDestinationIpV6": NotRequired[List[IpFilterTypeDef]],
+        "NetworkDestinationPort": NotRequired[List[NumberFilterTypeDef]],
+        "NetworkDestinationDomain": NotRequired[List[StringFilterTypeDef]],
+        "ProcessName": NotRequired[List[StringFilterTypeDef]],
+        "ProcessPath": NotRequired[List[StringFilterTypeDef]],
+        "ProcessPid": NotRequired[List[NumberFilterTypeDef]],
+        "ProcessParentPid": NotRequired[List[NumberFilterTypeDef]],
+        "ProcessLaunchedAt": NotRequired[List[DateFilterTypeDef]],
+        "ProcessTerminatedAt": NotRequired[List[DateFilterTypeDef]],
+        "ThreatIntelIndicatorType": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorValue": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorCategory": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorLastObservedAt": NotRequired[List[DateFilterTypeDef]],
+        "ThreatIntelIndicatorSource": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorSourceUrl": NotRequired[List[StringFilterTypeDef]],
+        "ResourceType": NotRequired[List[StringFilterTypeDef]],
+        "ResourceId": NotRequired[List[StringFilterTypeDef]],
+        "ResourcePartition": NotRequired[List[StringFilterTypeDef]],
+        "ResourceRegion": NotRequired[List[StringFilterTypeDef]],
+        "ResourceTags": NotRequired[List[MapFilterTypeDef]],
+        "ResourceAwsEc2InstanceType": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceImageId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceIpV4Addresses": NotRequired[List[IpFilterTypeDef]],
+        "ResourceAwsEc2InstanceIpV6Addresses": NotRequired[List[IpFilterTypeDef]],
+        "ResourceAwsEc2InstanceKeyName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceIamInstanceProfileArn": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceVpcId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceSubnetId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceLaunchedAt": NotRequired[List[DateFilterTypeDef]],
+        "ResourceAwsS3BucketOwnerId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsS3BucketOwnerName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyUserName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyPrincipalName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyStatus": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyCreatedAt": NotRequired[List[DateFilterTypeDef]],
+        "ResourceAwsIamUserUserName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerImageId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerImageName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerLaunchedAt": NotRequired[List[DateFilterTypeDef]],
+        "ResourceDetailsOther": NotRequired[List[MapFilterTypeDef]],
+        "ComplianceStatus": NotRequired[List[StringFilterTypeDef]],
+        "VerificationState": NotRequired[List[StringFilterTypeDef]],
+        "WorkflowState": NotRequired[List[StringFilterTypeDef]],
+        "WorkflowStatus": NotRequired[List[StringFilterTypeDef]],
+        "RecordState": NotRequired[List[StringFilterTypeDef]],
+        "RelatedFindingsProductArn": NotRequired[List[StringFilterTypeDef]],
+        "RelatedFindingsId": NotRequired[List[StringFilterTypeDef]],
+        "NoteText": NotRequired[List[StringFilterTypeDef]],
+        "NoteUpdatedAt": NotRequired[List[DateFilterTypeDef]],
+        "NoteUpdatedBy": NotRequired[List[StringFilterTypeDef]],
+        "Keyword": NotRequired[List[KeywordFilterTypeDef]],
+        "FindingProviderFieldsConfidence": NotRequired[List[NumberFilterTypeDef]],
+        "FindingProviderFieldsCriticality": NotRequired[List[NumberFilterTypeDef]],
+        "FindingProviderFieldsRelatedFindingsId": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsRelatedFindingsProductArn": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsSeverityLabel": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsSeverityOriginal": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsTypes": NotRequired[List[StringFilterTypeDef]],
+        "Sample": NotRequired[List[BooleanFilterTypeDef]],
+        "ComplianceSecurityControlId": NotRequired[List[StringFilterTypeDef]],
+        "ComplianceAssociatedStandardsId": NotRequired[List[StringFilterTypeDef]],
+        "VulnerabilitiesExploitAvailable": NotRequired[List[StringFilterTypeDef]],
+        "VulnerabilitiesFixAvailable": NotRequired[List[StringFilterTypeDef]],
+        "ComplianceSecurityControlParametersName": NotRequired[List[StringFilterTypeDef]],
+        "ComplianceSecurityControlParametersValue": NotRequired[List[StringFilterTypeDef]],
+        "AwsAccountName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceApplicationName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceApplicationArn": NotRequired[List[StringFilterTypeDef]],
+    },
+)
+AwsSecurityFindingFiltersOutputTypeDef = TypedDict(
+    "AwsSecurityFindingFiltersOutputTypeDef",
+    {
+        "ProductArn": NotRequired[List[StringFilterTypeDef]],
+        "AwsAccountId": NotRequired[List[StringFilterTypeDef]],
+        "Id": NotRequired[List[StringFilterTypeDef]],
+        "GeneratorId": NotRequired[List[StringFilterTypeDef]],
+        "Region": NotRequired[List[StringFilterTypeDef]],
+        "Type": NotRequired[List[StringFilterTypeDef]],
+        "FirstObservedAt": NotRequired[List[DateFilterTypeDef]],
+        "LastObservedAt": NotRequired[List[DateFilterTypeDef]],
+        "CreatedAt": NotRequired[List[DateFilterTypeDef]],
+        "UpdatedAt": NotRequired[List[DateFilterTypeDef]],
+        "SeverityProduct": NotRequired[List[NumberFilterTypeDef]],
+        "SeverityNormalized": NotRequired[List[NumberFilterTypeDef]],
+        "SeverityLabel": NotRequired[List[StringFilterTypeDef]],
+        "Confidence": NotRequired[List[NumberFilterTypeDef]],
+        "Criticality": NotRequired[List[NumberFilterTypeDef]],
+        "Title": NotRequired[List[StringFilterTypeDef]],
+        "Description": NotRequired[List[StringFilterTypeDef]],
+        "RecommendationText": NotRequired[List[StringFilterTypeDef]],
+        "SourceUrl": NotRequired[List[StringFilterTypeDef]],
+        "ProductFields": NotRequired[List[MapFilterTypeDef]],
+        "ProductName": NotRequired[List[StringFilterTypeDef]],
+        "CompanyName": NotRequired[List[StringFilterTypeDef]],
+        "UserDefinedFields": NotRequired[List[MapFilterTypeDef]],
+        "MalwareName": NotRequired[List[StringFilterTypeDef]],
+        "MalwareType": NotRequired[List[StringFilterTypeDef]],
+        "MalwarePath": NotRequired[List[StringFilterTypeDef]],
+        "MalwareState": NotRequired[List[StringFilterTypeDef]],
+        "NetworkDirection": NotRequired[List[StringFilterTypeDef]],
+        "NetworkProtocol": NotRequired[List[StringFilterTypeDef]],
+        "NetworkSourceIpV4": NotRequired[List[IpFilterTypeDef]],
+        "NetworkSourceIpV6": NotRequired[List[IpFilterTypeDef]],
+        "NetworkSourcePort": NotRequired[List[NumberFilterTypeDef]],
+        "NetworkSourceDomain": NotRequired[List[StringFilterTypeDef]],
+        "NetworkSourceMac": NotRequired[List[StringFilterTypeDef]],
+        "NetworkDestinationIpV4": NotRequired[List[IpFilterTypeDef]],
+        "NetworkDestinationIpV6": NotRequired[List[IpFilterTypeDef]],
+        "NetworkDestinationPort": NotRequired[List[NumberFilterTypeDef]],
+        "NetworkDestinationDomain": NotRequired[List[StringFilterTypeDef]],
+        "ProcessName": NotRequired[List[StringFilterTypeDef]],
+        "ProcessPath": NotRequired[List[StringFilterTypeDef]],
+        "ProcessPid": NotRequired[List[NumberFilterTypeDef]],
+        "ProcessParentPid": NotRequired[List[NumberFilterTypeDef]],
+        "ProcessLaunchedAt": NotRequired[List[DateFilterTypeDef]],
+        "ProcessTerminatedAt": NotRequired[List[DateFilterTypeDef]],
+        "ThreatIntelIndicatorType": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorValue": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorCategory": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorLastObservedAt": NotRequired[List[DateFilterTypeDef]],
+        "ThreatIntelIndicatorSource": NotRequired[List[StringFilterTypeDef]],
+        "ThreatIntelIndicatorSourceUrl": NotRequired[List[StringFilterTypeDef]],
+        "ResourceType": NotRequired[List[StringFilterTypeDef]],
+        "ResourceId": NotRequired[List[StringFilterTypeDef]],
+        "ResourcePartition": NotRequired[List[StringFilterTypeDef]],
+        "ResourceRegion": NotRequired[List[StringFilterTypeDef]],
+        "ResourceTags": NotRequired[List[MapFilterTypeDef]],
+        "ResourceAwsEc2InstanceType": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceImageId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceIpV4Addresses": NotRequired[List[IpFilterTypeDef]],
+        "ResourceAwsEc2InstanceIpV6Addresses": NotRequired[List[IpFilterTypeDef]],
+        "ResourceAwsEc2InstanceKeyName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceIamInstanceProfileArn": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceVpcId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceSubnetId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsEc2InstanceLaunchedAt": NotRequired[List[DateFilterTypeDef]],
+        "ResourceAwsS3BucketOwnerId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsS3BucketOwnerName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyUserName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyPrincipalName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyStatus": NotRequired[List[StringFilterTypeDef]],
+        "ResourceAwsIamAccessKeyCreatedAt": NotRequired[List[DateFilterTypeDef]],
+        "ResourceAwsIamUserUserName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerImageId": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerImageName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceContainerLaunchedAt": NotRequired[List[DateFilterTypeDef]],
+        "ResourceDetailsOther": NotRequired[List[MapFilterTypeDef]],
+        "ComplianceStatus": NotRequired[List[StringFilterTypeDef]],
+        "VerificationState": NotRequired[List[StringFilterTypeDef]],
+        "WorkflowState": NotRequired[List[StringFilterTypeDef]],
+        "WorkflowStatus": NotRequired[List[StringFilterTypeDef]],
+        "RecordState": NotRequired[List[StringFilterTypeDef]],
+        "RelatedFindingsProductArn": NotRequired[List[StringFilterTypeDef]],
+        "RelatedFindingsId": NotRequired[List[StringFilterTypeDef]],
+        "NoteText": NotRequired[List[StringFilterTypeDef]],
+        "NoteUpdatedAt": NotRequired[List[DateFilterTypeDef]],
+        "NoteUpdatedBy": NotRequired[List[StringFilterTypeDef]],
+        "Keyword": NotRequired[List[KeywordFilterTypeDef]],
+        "FindingProviderFieldsConfidence": NotRequired[List[NumberFilterTypeDef]],
+        "FindingProviderFieldsCriticality": NotRequired[List[NumberFilterTypeDef]],
+        "FindingProviderFieldsRelatedFindingsId": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsRelatedFindingsProductArn": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsSeverityLabel": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsSeverityOriginal": NotRequired[List[StringFilterTypeDef]],
+        "FindingProviderFieldsTypes": NotRequired[List[StringFilterTypeDef]],
+        "Sample": NotRequired[List[BooleanFilterTypeDef]],
+        "ComplianceSecurityControlId": NotRequired[List[StringFilterTypeDef]],
+        "ComplianceAssociatedStandardsId": NotRequired[List[StringFilterTypeDef]],
+        "VulnerabilitiesExploitAvailable": NotRequired[List[StringFilterTypeDef]],
+        "VulnerabilitiesFixAvailable": NotRequired[List[StringFilterTypeDef]],
+        "ComplianceSecurityControlParametersName": NotRequired[List[StringFilterTypeDef]],
+        "ComplianceSecurityControlParametersValue": NotRequired[List[StringFilterTypeDef]],
+        "AwsAccountName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceApplicationName": NotRequired[List[StringFilterTypeDef]],
+        "ResourceApplicationArn": NotRequired[List[StringFilterTypeDef]],
+    },
+)
 AwsSecurityFindingFiltersTypeDef = TypedDict(
     "AwsSecurityFindingFiltersTypeDef",
     {
         "ProductArn": NotRequired[Sequence[StringFilterTypeDef]],
         "AwsAccountId": NotRequired[Sequence[StringFilterTypeDef]],
         "Id": NotRequired[Sequence[StringFilterTypeDef]],
         "GeneratorId": NotRequired[Sequence[StringFilterTypeDef]],
@@ -10086,43 +12754,61 @@
         "ResourceApplicationArn": NotRequired[Sequence[StringFilterTypeDef]],
     },
 )
 GetFindingHistoryResponseTypeDef = TypedDict(
     "GetFindingHistoryResponseTypeDef",
     {
         "Records": List[FindingHistoryRecordTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetInsightResultsResponseTypeDef = TypedDict(
     "GetInsightResultsResponseTypeDef",
     {
         "InsightResults": InsightResultsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-NetworkHeaderPaginatorTypeDef = TypedDict(
-    "NetworkHeaderPaginatorTypeDef",
+NetworkHeaderExtraOutputTypeDef = TypedDict(
+    "NetworkHeaderExtraOutputTypeDef",
     {
         "Protocol": NotRequired[str],
-        "Destination": NotRequired[NetworkPathComponentDetailsPaginatorTypeDef],
-        "Source": NotRequired[NetworkPathComponentDetailsPaginatorTypeDef],
+        "Destination": NotRequired[NetworkPathComponentDetailsExtraOutputTypeDef],
+        "Source": NotRequired[NetworkPathComponentDetailsExtraOutputTypeDef],
+    },
+)
+NetworkHeaderOutputTypeDef = TypedDict(
+    "NetworkHeaderOutputTypeDef",
+    {
+        "Protocol": NotRequired[str],
+        "Destination": NotRequired[NetworkPathComponentDetailsOutputTypeDef],
+        "Source": NotRequired[NetworkPathComponentDetailsOutputTypeDef],
     },
 )
 NetworkHeaderTypeDef = TypedDict(
     "NetworkHeaderTypeDef",
     {
         "Protocol": NotRequired[str],
         "Destination": NotRequired[NetworkPathComponentDetailsTypeDef],
         "Source": NotRequired[NetworkPathComponentDetailsTypeDef],
     },
 )
-OccurrencesPaginatorTypeDef = TypedDict(
-    "OccurrencesPaginatorTypeDef",
+OccurrencesExtraOutputTypeDef = TypedDict(
+    "OccurrencesExtraOutputTypeDef",
+    {
+        "LineRanges": NotRequired[List[RangeTypeDef]],
+        "OffsetRanges": NotRequired[List[RangeTypeDef]],
+        "Pages": NotRequired[List[PageTypeDef]],
+        "Records": NotRequired[List[RecordTypeDef]],
+        "Cells": NotRequired[List[CellTypeDef]],
+    },
+)
+OccurrencesOutputTypeDef = TypedDict(
+    "OccurrencesOutputTypeDef",
     {
         "LineRanges": NotRequired[List[RangeTypeDef]],
         "OffsetRanges": NotRequired[List[RangeTypeDef]],
         "Pages": NotRequired[List[PageTypeDef]],
         "Records": NotRequired[List[RecordTypeDef]],
         "Cells": NotRequired[List[CellTypeDef]],
     },
@@ -10133,64 +12819,75 @@
         "LineRanges": NotRequired[Sequence[RangeTypeDef]],
         "OffsetRanges": NotRequired[Sequence[RangeTypeDef]],
         "Pages": NotRequired[Sequence[PageTypeDef]],
         "Records": NotRequired[Sequence[RecordTypeDef]],
         "Cells": NotRequired[Sequence[CellTypeDef]],
     },
 )
-SecurityControlCustomParameterTypeDef = TypedDict(
-    "SecurityControlCustomParameterTypeDef",
+SecurityControlCustomParameterOutputTypeDef = TypedDict(
+    "SecurityControlCustomParameterOutputTypeDef",
     {
         "SecurityControlId": NotRequired[str],
-        "Parameters": NotRequired[Mapping[str, ParameterConfigurationTypeDef]],
+        "Parameters": NotRequired[Dict[str, ParameterConfigurationOutputTypeDef]],
     },
 )
 SecurityControlTypeDef = TypedDict(
     "SecurityControlTypeDef",
     {
         "SecurityControlId": str,
         "SecurityControlArn": str,
         "Title": str,
         "Description": str,
         "RemediationUrl": str,
         "SeverityRating": SeverityRatingType,
         "SecurityControlStatus": ControlStatusType,
         "UpdateStatus": NotRequired[UpdateStatusType],
-        "Parameters": NotRequired[Dict[str, ParameterConfigurationTypeDef]],
+        "Parameters": NotRequired[Dict[str, ParameterConfigurationOutputTypeDef]],
         "LastUpdateReason": NotRequired[str],
     },
 )
-UpdateSecurityControlRequestRequestTypeDef = TypedDict(
-    "UpdateSecurityControlRequestRequestTypeDef",
+ParameterConfigurationUnionTypeDef = Union[
+    ParameterConfigurationTypeDef, ParameterConfigurationOutputTypeDef
+]
+SecurityControlCustomParameterTypeDef = TypedDict(
+    "SecurityControlCustomParameterTypeDef",
     {
-        "SecurityControlId": str,
-        "Parameters": Mapping[str, ParameterConfigurationTypeDef],
-        "LastUpdateReason": NotRequired[str],
+        "SecurityControlId": NotRequired[str],
+        "Parameters": NotRequired[Mapping[str, ParameterConfigurationTypeDef]],
+    },
+)
+RuleGroupSourceStatelessRuleDefinitionExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleDefinitionExtraOutputTypeDef",
+    {
+        "Actions": NotRequired[List[str]],
+        "MatchAttributes": NotRequired[
+            RuleGroupSourceStatelessRuleMatchAttributesExtraOutputTypeDef
+        ],
     },
 )
-RuleGroupSourceStatelessRuleDefinitionPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleDefinitionPaginatorTypeDef",
+RuleGroupSourceStatelessRuleDefinitionOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleDefinitionOutputTypeDef",
     {
         "Actions": NotRequired[List[str]],
-        "MatchAttributes": NotRequired[RuleGroupSourceStatelessRuleMatchAttributesPaginatorTypeDef],
+        "MatchAttributes": NotRequired[RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef],
     },
 )
 RuleGroupSourceStatelessRuleDefinitionTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
     {
         "Actions": NotRequired[Sequence[str]],
         "MatchAttributes": NotRequired[RuleGroupSourceStatelessRuleMatchAttributesTypeDef],
     },
 )
 DescribeStandardsResponseTypeDef = TypedDict(
     "DescribeStandardsResponseTypeDef",
     {
         "Standards": List[StandardTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 BatchDisableStandardsResponseTypeDef = TypedDict(
     "BatchDisableStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -10203,63 +12900,99 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetEnabledStandardsResponseTypeDef = TypedDict(
     "GetEnabledStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
-StatelessCustomActionDefinitionPaginatorTypeDef = TypedDict(
-    "StatelessCustomActionDefinitionPaginatorTypeDef",
+StatelessCustomActionDefinitionExtraOutputTypeDef = TypedDict(
+    "StatelessCustomActionDefinitionExtraOutputTypeDef",
     {
-        "PublishMetricAction": NotRequired[StatelessCustomPublishMetricActionPaginatorTypeDef],
+        "PublishMetricAction": NotRequired[StatelessCustomPublishMetricActionExtraOutputTypeDef],
+    },
+)
+StatelessCustomActionDefinitionOutputTypeDef = TypedDict(
+    "StatelessCustomActionDefinitionOutputTypeDef",
+    {
+        "PublishMetricAction": NotRequired[StatelessCustomPublishMetricActionOutputTypeDef],
     },
 )
 StatelessCustomActionDefinitionTypeDef = TypedDict(
     "StatelessCustomActionDefinitionTypeDef",
     {
         "PublishMetricAction": NotRequired[StatelessCustomPublishMetricActionTypeDef],
     },
 )
-PortProbeActionPaginatorTypeDef = TypedDict(
-    "PortProbeActionPaginatorTypeDef",
+PortProbeActionExtraOutputTypeDef = TypedDict(
+    "PortProbeActionExtraOutputTypeDef",
+    {
+        "PortProbeDetails": NotRequired[List[PortProbeDetailTypeDef]],
+        "Blocked": NotRequired[bool],
+    },
+)
+PortProbeActionOutputTypeDef = TypedDict(
+    "PortProbeActionOutputTypeDef",
     {
         "PortProbeDetails": NotRequired[List[PortProbeDetailTypeDef]],
         "Blocked": NotRequired[bool],
     },
 )
 PortProbeActionTypeDef = TypedDict(
     "PortProbeActionTypeDef",
     {
         "PortProbeDetails": NotRequired[Sequence[PortProbeDetailTypeDef]],
         "Blocked": NotRequired[bool],
     },
 )
+AutomationRulesActionUnionTypeDef = Union[
+    AutomationRulesActionTypeDef, AutomationRulesActionOutputTypeDef
+]
 AwsAthenaWorkGroupDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupDetailsTypeDef",
     {
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "State": NotRequired[str],
         "Configuration": NotRequired[AwsAthenaWorkGroupConfigurationDetailsTypeDef],
     },
 )
-AwsAutoScalingAutoScalingGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupDetailsPaginatorTypeDef",
+AwsAutoScalingAutoScalingGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupDetailsExtraOutputTypeDef",
     {
         "LaunchConfigurationName": NotRequired[str],
         "LoadBalancerNames": NotRequired[List[str]],
         "HealthCheckType": NotRequired[str],
         "HealthCheckGracePeriod": NotRequired[int],
         "CreatedTime": NotRequired[str],
         "MixedInstancesPolicy": NotRequired[
-            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsPaginatorTypeDef
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsExtraOutputTypeDef
+        ],
+        "AvailabilityZones": NotRequired[
+            List[AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef]
+        ],
+        "LaunchTemplate": NotRequired[
+            AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
+        ],
+        "CapacityRebalance": NotRequired[bool],
+    },
+)
+AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef = TypedDict(
+    "AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef",
+    {
+        "LaunchConfigurationName": NotRequired[str],
+        "LoadBalancerNames": NotRequired[List[str]],
+        "HealthCheckType": NotRequired[str],
+        "HealthCheckGracePeriod": NotRequired[int],
+        "CreatedTime": NotRequired[str],
+        "MixedInstancesPolicy": NotRequired[
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef
         ],
         "AvailabilityZones": NotRequired[
             List[AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef]
         ],
         "LaunchTemplate": NotRequired[
             AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
         ],
@@ -10282,42 +13015,52 @@
         ],
         "LaunchTemplate": NotRequired[
             AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
         ],
         "CapacityRebalance": NotRequired[bool],
     },
 )
-AwsBackupBackupPlanBackupPlanDetailsPaginatorTypeDef = TypedDict(
-    "AwsBackupBackupPlanBackupPlanDetailsPaginatorTypeDef",
+AwsBackupBackupPlanBackupPlanDetailsExtraOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanBackupPlanDetailsExtraOutputTypeDef",
     {
         "BackupPlanName": NotRequired[str],
         "AdvancedBackupSettings": NotRequired[
-            List[AwsBackupBackupPlanAdvancedBackupSettingsDetailsPaginatorTypeDef]
+            List[AwsBackupBackupPlanAdvancedBackupSettingsDetailsExtraOutputTypeDef]
         ],
-        "BackupPlanRule": NotRequired[List[AwsBackupBackupPlanRuleDetailsPaginatorTypeDef]],
+        "BackupPlanRule": NotRequired[List[AwsBackupBackupPlanRuleDetailsExtraOutputTypeDef]],
+    },
+)
+AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef",
+    {
+        "BackupPlanName": NotRequired[str],
+        "AdvancedBackupSettings": NotRequired[
+            List[AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef]
+        ],
+        "BackupPlanRule": NotRequired[List[AwsBackupBackupPlanRuleDetailsOutputTypeDef]],
     },
 )
 AwsBackupBackupPlanBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
     {
         "BackupPlanName": NotRequired[str],
         "AdvancedBackupSettings": NotRequired[
             Sequence[AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef]
         ],
         "BackupPlanRule": NotRequired[Sequence[AwsBackupBackupPlanRuleDetailsTypeDef]],
     },
 )
-AwsCertificateManagerCertificateDetailsPaginatorTypeDef = TypedDict(
-    "AwsCertificateManagerCertificateDetailsPaginatorTypeDef",
+AwsCertificateManagerCertificateDetailsExtraOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateDetailsExtraOutputTypeDef",
     {
         "CertificateAuthorityArn": NotRequired[str],
         "CreatedAt": NotRequired[str],
         "DomainName": NotRequired[str],
         "DomainValidationOptions": NotRequired[
-            List[AwsCertificateManagerCertificateDomainValidationOptionPaginatorTypeDef]
+            List[AwsCertificateManagerCertificateDomainValidationOptionExtraOutputTypeDef]
         ],
         "ExtendedKeyUsages": NotRequired[
             List[AwsCertificateManagerCertificateExtendedKeyUsageTypeDef]
         ],
         "FailureReason": NotRequired[str],
         "ImportedAt": NotRequired[str],
         "InUseBy": NotRequired[List[str]],
@@ -10326,16 +13069,48 @@
         "KeyAlgorithm": NotRequired[str],
         "KeyUsages": NotRequired[List[AwsCertificateManagerCertificateKeyUsageTypeDef]],
         "NotAfter": NotRequired[str],
         "NotBefore": NotRequired[str],
         "Options": NotRequired[AwsCertificateManagerCertificateOptionsTypeDef],
         "RenewalEligibility": NotRequired[str],
         "RenewalSummary": NotRequired[
-            AwsCertificateManagerCertificateRenewalSummaryPaginatorTypeDef
+            AwsCertificateManagerCertificateRenewalSummaryExtraOutputTypeDef
+        ],
+        "Serial": NotRequired[str],
+        "SignatureAlgorithm": NotRequired[str],
+        "Status": NotRequired[str],
+        "Subject": NotRequired[str],
+        "SubjectAlternativeNames": NotRequired[List[str]],
+        "Type": NotRequired[str],
+    },
+)
+AwsCertificateManagerCertificateDetailsOutputTypeDef = TypedDict(
+    "AwsCertificateManagerCertificateDetailsOutputTypeDef",
+    {
+        "CertificateAuthorityArn": NotRequired[str],
+        "CreatedAt": NotRequired[str],
+        "DomainName": NotRequired[str],
+        "DomainValidationOptions": NotRequired[
+            List[AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef]
+        ],
+        "ExtendedKeyUsages": NotRequired[
+            List[AwsCertificateManagerCertificateExtendedKeyUsageTypeDef]
         ],
+        "FailureReason": NotRequired[str],
+        "ImportedAt": NotRequired[str],
+        "InUseBy": NotRequired[List[str]],
+        "IssuedAt": NotRequired[str],
+        "Issuer": NotRequired[str],
+        "KeyAlgorithm": NotRequired[str],
+        "KeyUsages": NotRequired[List[AwsCertificateManagerCertificateKeyUsageTypeDef]],
+        "NotAfter": NotRequired[str],
+        "NotBefore": NotRequired[str],
+        "Options": NotRequired[AwsCertificateManagerCertificateOptionsTypeDef],
+        "RenewalEligibility": NotRequired[str],
+        "RenewalSummary": NotRequired[AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef],
         "Serial": NotRequired[str],
         "SignatureAlgorithm": NotRequired[str],
         "Status": NotRequired[str],
         "Subject": NotRequired[str],
         "SubjectAlternativeNames": NotRequired[List[str]],
         "Type": NotRequired[str],
     },
@@ -10368,57 +13143,98 @@
         "SignatureAlgorithm": NotRequired[str],
         "Status": NotRequired[str],
         "Subject": NotRequired[str],
         "SubjectAlternativeNames": NotRequired[Sequence[str]],
         "Type": NotRequired[str],
     },
 )
-AwsCloudFrontDistributionOriginsPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginsPaginatorTypeDef",
+AwsCloudFrontDistributionOriginsExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginsExtraOutputTypeDef",
     {
-        "Items": NotRequired[List[AwsCloudFrontDistributionOriginItemPaginatorTypeDef]],
+        "Items": NotRequired[List[AwsCloudFrontDistributionOriginItemExtraOutputTypeDef]],
+    },
+)
+AwsCloudFrontDistributionOriginsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginsOutputTypeDef",
+    {
+        "Items": NotRequired[List[AwsCloudFrontDistributionOriginItemOutputTypeDef]],
     },
 )
 AwsCloudFrontDistributionOriginsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginsTypeDef",
     {
         "Items": NotRequired[Sequence[AwsCloudFrontDistributionOriginItemTypeDef]],
     },
 )
-AwsCloudFrontDistributionOriginGroupsPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginGroupsPaginatorTypeDef",
+AwsCloudFrontDistributionOriginGroupsExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupsExtraOutputTypeDef",
+    {
+        "Items": NotRequired[List[AwsCloudFrontDistributionOriginGroupExtraOutputTypeDef]],
+    },
+)
+AwsCloudFrontDistributionOriginGroupsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionOriginGroupsOutputTypeDef",
     {
-        "Items": NotRequired[List[AwsCloudFrontDistributionOriginGroupPaginatorTypeDef]],
+        "Items": NotRequired[List[AwsCloudFrontDistributionOriginGroupOutputTypeDef]],
     },
 )
 AwsCloudFrontDistributionOriginGroupsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupsTypeDef",
     {
         "Items": NotRequired[Sequence[AwsCloudFrontDistributionOriginGroupTypeDef]],
     },
 )
-AwsDynamoDbTableDetailsPaginatorTypeDef = TypedDict(
-    "AwsDynamoDbTableDetailsPaginatorTypeDef",
+AwsDynamoDbTableDetailsExtraOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableDetailsExtraOutputTypeDef",
+    {
+        "AttributeDefinitions": NotRequired[List[AwsDynamoDbTableAttributeDefinitionTypeDef]],
+        "BillingModeSummary": NotRequired[AwsDynamoDbTableBillingModeSummaryTypeDef],
+        "CreationDateTime": NotRequired[str],
+        "GlobalSecondaryIndexes": NotRequired[
+            List[AwsDynamoDbTableGlobalSecondaryIndexExtraOutputTypeDef]
+        ],
+        "GlobalTableVersion": NotRequired[str],
+        "ItemCount": NotRequired[int],
+        "KeySchema": NotRequired[List[AwsDynamoDbTableKeySchemaTypeDef]],
+        "LatestStreamArn": NotRequired[str],
+        "LatestStreamLabel": NotRequired[str],
+        "LocalSecondaryIndexes": NotRequired[
+            List[AwsDynamoDbTableLocalSecondaryIndexExtraOutputTypeDef]
+        ],
+        "ProvisionedThroughput": NotRequired[AwsDynamoDbTableProvisionedThroughputTypeDef],
+        "Replicas": NotRequired[List[AwsDynamoDbTableReplicaExtraOutputTypeDef]],
+        "RestoreSummary": NotRequired[AwsDynamoDbTableRestoreSummaryTypeDef],
+        "SseDescription": NotRequired[AwsDynamoDbTableSseDescriptionTypeDef],
+        "StreamSpecification": NotRequired[AwsDynamoDbTableStreamSpecificationTypeDef],
+        "TableId": NotRequired[str],
+        "TableName": NotRequired[str],
+        "TableSizeBytes": NotRequired[int],
+        "TableStatus": NotRequired[str],
+        "DeletionProtectionEnabled": NotRequired[bool],
+    },
+)
+AwsDynamoDbTableDetailsOutputTypeDef = TypedDict(
+    "AwsDynamoDbTableDetailsOutputTypeDef",
     {
         "AttributeDefinitions": NotRequired[List[AwsDynamoDbTableAttributeDefinitionTypeDef]],
         "BillingModeSummary": NotRequired[AwsDynamoDbTableBillingModeSummaryTypeDef],
         "CreationDateTime": NotRequired[str],
         "GlobalSecondaryIndexes": NotRequired[
-            List[AwsDynamoDbTableGlobalSecondaryIndexPaginatorTypeDef]
+            List[AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef]
         ],
         "GlobalTableVersion": NotRequired[str],
         "ItemCount": NotRequired[int],
         "KeySchema": NotRequired[List[AwsDynamoDbTableKeySchemaTypeDef]],
         "LatestStreamArn": NotRequired[str],
         "LatestStreamLabel": NotRequired[str],
         "LocalSecondaryIndexes": NotRequired[
-            List[AwsDynamoDbTableLocalSecondaryIndexPaginatorTypeDef]
+            List[AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef]
         ],
         "ProvisionedThroughput": NotRequired[AwsDynamoDbTableProvisionedThroughputTypeDef],
-        "Replicas": NotRequired[List[AwsDynamoDbTableReplicaPaginatorTypeDef]],
+        "Replicas": NotRequired[List[AwsDynamoDbTableReplicaOutputTypeDef]],
         "RestoreSummary": NotRequired[AwsDynamoDbTableRestoreSummaryTypeDef],
         "SseDescription": NotRequired[AwsDynamoDbTableSseDescriptionTypeDef],
         "StreamSpecification": NotRequired[AwsDynamoDbTableStreamSpecificationTypeDef],
         "TableId": NotRequired[str],
         "TableName": NotRequired[str],
         "TableSizeBytes": NotRequired[int],
         "TableStatus": NotRequired[str],
@@ -10448,36 +13264,63 @@
         "TableId": NotRequired[str],
         "TableName": NotRequired[str],
         "TableSizeBytes": NotRequired[int],
         "TableStatus": NotRequired[str],
         "DeletionProtectionEnabled": NotRequired[bool],
     },
 )
-AwsEc2LaunchTemplateDetailsPaginatorTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDetailsPaginatorTypeDef",
+AwsEc2LaunchTemplateDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDetailsExtraOutputTypeDef",
     {
         "LaunchTemplateName": NotRequired[str],
         "Id": NotRequired[str],
-        "LaunchTemplateData": NotRequired[AwsEc2LaunchTemplateDataDetailsPaginatorTypeDef],
+        "LaunchTemplateData": NotRequired[AwsEc2LaunchTemplateDataDetailsExtraOutputTypeDef],
+        "DefaultVersionNumber": NotRequired[int],
+        "LatestVersionNumber": NotRequired[int],
+    },
+)
+AwsEc2LaunchTemplateDetailsOutputTypeDef = TypedDict(
+    "AwsEc2LaunchTemplateDetailsOutputTypeDef",
+    {
+        "LaunchTemplateName": NotRequired[str],
+        "Id": NotRequired[str],
+        "LaunchTemplateData": NotRequired[AwsEc2LaunchTemplateDataDetailsOutputTypeDef],
         "DefaultVersionNumber": NotRequired[int],
         "LatestVersionNumber": NotRequired[int],
     },
 )
 AwsEc2LaunchTemplateDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDetailsTypeDef",
     {
         "LaunchTemplateName": NotRequired[str],
         "Id": NotRequired[str],
         "LaunchTemplateData": NotRequired[AwsEc2LaunchTemplateDataDetailsTypeDef],
         "DefaultVersionNumber": NotRequired[int],
         "LatestVersionNumber": NotRequired[int],
     },
 )
-AwsEcsClusterDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsClusterDetailsPaginatorTypeDef",
+AwsEcsClusterDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsClusterDetailsExtraOutputTypeDef",
+    {
+        "ClusterArn": NotRequired[str],
+        "ActiveServicesCount": NotRequired[int],
+        "CapacityProviders": NotRequired[List[str]],
+        "ClusterSettings": NotRequired[List[AwsEcsClusterClusterSettingsDetailsTypeDef]],
+        "Configuration": NotRequired[AwsEcsClusterConfigurationDetailsTypeDef],
+        "DefaultCapacityProviderStrategy": NotRequired[
+            List[AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef]
+        ],
+        "ClusterName": NotRequired[str],
+        "RegisteredContainerInstancesCount": NotRequired[int],
+        "RunningTasksCount": NotRequired[int],
+        "Status": NotRequired[str],
+    },
+)
+AwsEcsClusterDetailsOutputTypeDef = TypedDict(
+    "AwsEcsClusterDetailsOutputTypeDef",
     {
         "ClusterArn": NotRequired[str],
         "ActiveServicesCount": NotRequired[int],
         "CapacityProviders": NotRequired[List[str]],
         "ClusterSettings": NotRequired[List[AwsEcsClusterClusterSettingsDetailsTypeDef]],
         "Configuration": NotRequired[AwsEcsClusterConfigurationDetailsTypeDef],
         "DefaultCapacityProviderStrategy": NotRequired[
@@ -10502,19 +13345,19 @@
         ],
         "ClusterName": NotRequired[str],
         "RegisteredContainerInstancesCount": NotRequired[int],
         "RunningTasksCount": NotRequired[int],
         "Status": NotRequired[str],
     },
 )
-AwsEcsTaskDefinitionDetailsPaginatorTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionDetailsPaginatorTypeDef",
+AwsEcsTaskDefinitionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionDetailsExtraOutputTypeDef",
     {
         "ContainerDefinitions": NotRequired[
-            List[AwsEcsTaskDefinitionContainerDefinitionsDetailsPaginatorTypeDef]
+            List[AwsEcsTaskDefinitionContainerDefinitionsDetailsExtraOutputTypeDef]
         ],
         "Cpu": NotRequired[str],
         "ExecutionRoleArn": NotRequired[str],
         "Family": NotRequired[str],
         "InferenceAccelerators": NotRequired[
             List[AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef]
         ],
@@ -10522,19 +13365,47 @@
         "Memory": NotRequired[str],
         "NetworkMode": NotRequired[str],
         "PidMode": NotRequired[str],
         "PlacementConstraints": NotRequired[
             List[AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef]
         ],
         "ProxyConfiguration": NotRequired[
-            AwsEcsTaskDefinitionProxyConfigurationDetailsPaginatorTypeDef
+            AwsEcsTaskDefinitionProxyConfigurationDetailsExtraOutputTypeDef
         ],
         "RequiresCompatibilities": NotRequired[List[str]],
         "TaskRoleArn": NotRequired[str],
-        "Volumes": NotRequired[List[AwsEcsTaskDefinitionVolumesDetailsPaginatorTypeDef]],
+        "Volumes": NotRequired[List[AwsEcsTaskDefinitionVolumesDetailsExtraOutputTypeDef]],
+        "Status": NotRequired[str],
+    },
+)
+AwsEcsTaskDefinitionDetailsOutputTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionDetailsOutputTypeDef",
+    {
+        "ContainerDefinitions": NotRequired[
+            List[AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef]
+        ],
+        "Cpu": NotRequired[str],
+        "ExecutionRoleArn": NotRequired[str],
+        "Family": NotRequired[str],
+        "InferenceAccelerators": NotRequired[
+            List[AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef]
+        ],
+        "IpcMode": NotRequired[str],
+        "Memory": NotRequired[str],
+        "NetworkMode": NotRequired[str],
+        "PidMode": NotRequired[str],
+        "PlacementConstraints": NotRequired[
+            List[AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef]
+        ],
+        "ProxyConfiguration": NotRequired[
+            AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef
+        ],
+        "RequiresCompatibilities": NotRequired[List[str]],
+        "TaskRoleArn": NotRequired[str],
+        "Volumes": NotRequired[List[AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef]],
         "Status": NotRequired[str],
     },
 )
 AwsEcsTaskDefinitionDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionDetailsTypeDef",
     {
         "ContainerDefinitions": NotRequired[
@@ -10556,16 +13427,32 @@
         "ProxyConfiguration": NotRequired[AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef],
         "RequiresCompatibilities": NotRequired[Sequence[str]],
         "TaskRoleArn": NotRequired[str],
         "Volumes": NotRequired[Sequence[AwsEcsTaskDefinitionVolumesDetailsTypeDef]],
         "Status": NotRequired[str],
     },
 )
-AwsEventsEndpointDetailsPaginatorTypeDef = TypedDict(
-    "AwsEventsEndpointDetailsPaginatorTypeDef",
+AwsEventsEndpointDetailsExtraOutputTypeDef = TypedDict(
+    "AwsEventsEndpointDetailsExtraOutputTypeDef",
+    {
+        "Arn": NotRequired[str],
+        "Description": NotRequired[str],
+        "EndpointId": NotRequired[str],
+        "EndpointUrl": NotRequired[str],
+        "EventBuses": NotRequired[List[AwsEventsEndpointEventBusesDetailsTypeDef]],
+        "Name": NotRequired[str],
+        "ReplicationConfig": NotRequired[AwsEventsEndpointReplicationConfigDetailsTypeDef],
+        "RoleArn": NotRequired[str],
+        "RoutingConfig": NotRequired[AwsEventsEndpointRoutingConfigDetailsTypeDef],
+        "State": NotRequired[str],
+        "StateReason": NotRequired[str],
+    },
+)
+AwsEventsEndpointDetailsOutputTypeDef = TypedDict(
+    "AwsEventsEndpointDetailsOutputTypeDef",
     {
         "Arn": NotRequired[str],
         "Description": NotRequired[str],
         "EndpointId": NotRequired[str],
         "EndpointUrl": NotRequired[str],
         "EventBuses": NotRequired[List[AwsEventsEndpointEventBusesDetailsTypeDef]],
         "Name": NotRequired[str],
@@ -10601,23 +13488,36 @@
         "Kubernetes": NotRequired[AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef],
         "MalwareProtection": NotRequired[
             AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef
         ],
         "S3Logs": NotRequired[AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef],
     },
 )
-AwsMskClusterClusterInfoDetailsPaginatorTypeDef = TypedDict(
-    "AwsMskClusterClusterInfoDetailsPaginatorTypeDef",
+AwsMskClusterClusterInfoDetailsExtraOutputTypeDef = TypedDict(
+    "AwsMskClusterClusterInfoDetailsExtraOutputTypeDef",
     {
         "EncryptionInfo": NotRequired[AwsMskClusterClusterInfoEncryptionInfoDetailsTypeDef],
         "CurrentVersion": NotRequired[str],
         "NumberOfBrokerNodes": NotRequired[int],
         "ClusterName": NotRequired[str],
         "ClientAuthentication": NotRequired[
-            AwsMskClusterClusterInfoClientAuthenticationDetailsPaginatorTypeDef
+            AwsMskClusterClusterInfoClientAuthenticationDetailsExtraOutputTypeDef
+        ],
+        "EnhancedMonitoring": NotRequired[str],
+    },
+)
+AwsMskClusterClusterInfoDetailsOutputTypeDef = TypedDict(
+    "AwsMskClusterClusterInfoDetailsOutputTypeDef",
+    {
+        "EncryptionInfo": NotRequired[AwsMskClusterClusterInfoEncryptionInfoDetailsTypeDef],
+        "CurrentVersion": NotRequired[str],
+        "NumberOfBrokerNodes": NotRequired[int],
+        "ClusterName": NotRequired[str],
+        "ClientAuthentication": NotRequired[
+            AwsMskClusterClusterInfoClientAuthenticationDetailsOutputTypeDef
         ],
         "EnhancedMonitoring": NotRequired[str],
     },
 )
 AwsMskClusterClusterInfoDetailsTypeDef = TypedDict(
     "AwsMskClusterClusterInfoDetailsTypeDef",
     {
@@ -10627,16 +13527,16 @@
         "ClusterName": NotRequired[str],
         "ClientAuthentication": NotRequired[
             AwsMskClusterClusterInfoClientAuthenticationDetailsTypeDef
         ],
         "EnhancedMonitoring": NotRequired[str],
     },
 )
-AwsRdsDbInstanceDetailsPaginatorTypeDef = TypedDict(
-    "AwsRdsDbInstanceDetailsPaginatorTypeDef",
+AwsRdsDbInstanceDetailsExtraOutputTypeDef = TypedDict(
+    "AwsRdsDbInstanceDetailsExtraOutputTypeDef",
     {
         "AssociatedRoles": NotRequired[List[AwsRdsDbInstanceAssociatedRoleTypeDef]],
         "CACertificateIdentifier": NotRequired[str],
         "DBClusterIdentifier": NotRequired[str],
         "DBInstanceIdentifier": NotRequired[str],
         "DBInstanceClass": NotRequired[str],
         "DbInstancePort": NotRequired[int],
@@ -10659,17 +13559,79 @@
         "MasterUsername": NotRequired[str],
         "AllocatedStorage": NotRequired[int],
         "PreferredBackupWindow": NotRequired[str],
         "BackupRetentionPeriod": NotRequired[int],
         "DbSecurityGroups": NotRequired[List[str]],
         "DbParameterGroups": NotRequired[List[AwsRdsDbParameterGroupTypeDef]],
         "AvailabilityZone": NotRequired[str],
-        "DbSubnetGroup": NotRequired[AwsRdsDbSubnetGroupPaginatorTypeDef],
+        "DbSubnetGroup": NotRequired[AwsRdsDbSubnetGroupExtraOutputTypeDef],
         "PreferredMaintenanceWindow": NotRequired[str],
-        "PendingModifiedValues": NotRequired[AwsRdsDbPendingModifiedValuesPaginatorTypeDef],
+        "PendingModifiedValues": NotRequired[AwsRdsDbPendingModifiedValuesExtraOutputTypeDef],
+        "LatestRestorableTime": NotRequired[str],
+        "AutoMinorVersionUpgrade": NotRequired[bool],
+        "ReadReplicaSourceDBInstanceIdentifier": NotRequired[str],
+        "ReadReplicaDBInstanceIdentifiers": NotRequired[List[str]],
+        "ReadReplicaDBClusterIdentifiers": NotRequired[List[str]],
+        "LicenseModel": NotRequired[str],
+        "Iops": NotRequired[int],
+        "OptionGroupMemberships": NotRequired[List[AwsRdsDbOptionGroupMembershipTypeDef]],
+        "CharacterSetName": NotRequired[str],
+        "SecondaryAvailabilityZone": NotRequired[str],
+        "StatusInfos": NotRequired[List[AwsRdsDbStatusInfoTypeDef]],
+        "StorageType": NotRequired[str],
+        "DomainMemberships": NotRequired[List[AwsRdsDbDomainMembershipTypeDef]],
+        "CopyTagsToSnapshot": NotRequired[bool],
+        "MonitoringInterval": NotRequired[int],
+        "MonitoringRoleArn": NotRequired[str],
+        "PromotionTier": NotRequired[int],
+        "Timezone": NotRequired[str],
+        "PerformanceInsightsEnabled": NotRequired[bool],
+        "PerformanceInsightsKmsKeyId": NotRequired[str],
+        "PerformanceInsightsRetentionPeriod": NotRequired[int],
+        "EnabledCloudWatchLogsExports": NotRequired[List[str]],
+        "ProcessorFeatures": NotRequired[List[AwsRdsDbProcessorFeatureTypeDef]],
+        "ListenerEndpoint": NotRequired[AwsRdsDbInstanceEndpointTypeDef],
+        "MaxAllocatedStorage": NotRequired[int],
+    },
+)
+AwsRdsDbInstanceDetailsOutputTypeDef = TypedDict(
+    "AwsRdsDbInstanceDetailsOutputTypeDef",
+    {
+        "AssociatedRoles": NotRequired[List[AwsRdsDbInstanceAssociatedRoleTypeDef]],
+        "CACertificateIdentifier": NotRequired[str],
+        "DBClusterIdentifier": NotRequired[str],
+        "DBInstanceIdentifier": NotRequired[str],
+        "DBInstanceClass": NotRequired[str],
+        "DbInstancePort": NotRequired[int],
+        "DbiResourceId": NotRequired[str],
+        "DBName": NotRequired[str],
+        "DeletionProtection": NotRequired[bool],
+        "Endpoint": NotRequired[AwsRdsDbInstanceEndpointTypeDef],
+        "Engine": NotRequired[str],
+        "EngineVersion": NotRequired[str],
+        "IAMDatabaseAuthenticationEnabled": NotRequired[bool],
+        "InstanceCreateTime": NotRequired[str],
+        "KmsKeyId": NotRequired[str],
+        "PubliclyAccessible": NotRequired[bool],
+        "StorageEncrypted": NotRequired[bool],
+        "TdeCredentialArn": NotRequired[str],
+        "VpcSecurityGroups": NotRequired[List[AwsRdsDbInstanceVpcSecurityGroupTypeDef]],
+        "MultiAz": NotRequired[bool],
+        "EnhancedMonitoringResourceArn": NotRequired[str],
+        "DbInstanceStatus": NotRequired[str],
+        "MasterUsername": NotRequired[str],
+        "AllocatedStorage": NotRequired[int],
+        "PreferredBackupWindow": NotRequired[str],
+        "BackupRetentionPeriod": NotRequired[int],
+        "DbSecurityGroups": NotRequired[List[str]],
+        "DbParameterGroups": NotRequired[List[AwsRdsDbParameterGroupTypeDef]],
+        "AvailabilityZone": NotRequired[str],
+        "DbSubnetGroup": NotRequired[AwsRdsDbSubnetGroupOutputTypeDef],
+        "PreferredMaintenanceWindow": NotRequired[str],
+        "PendingModifiedValues": NotRequired[AwsRdsDbPendingModifiedValuesOutputTypeDef],
         "LatestRestorableTime": NotRequired[str],
         "AutoMinorVersionUpgrade": NotRequired[bool],
         "ReadReplicaSourceDBInstanceIdentifier": NotRequired[str],
         "ReadReplicaDBInstanceIdentifiers": NotRequired[List[str]],
         "ReadReplicaDBClusterIdentifiers": NotRequired[List[str]],
         "LicenseModel": NotRequired[str],
         "Iops": NotRequired[int],
@@ -10751,54 +13713,88 @@
         "PerformanceInsightsRetentionPeriod": NotRequired[int],
         "EnabledCloudWatchLogsExports": NotRequired[Sequence[str]],
         "ProcessorFeatures": NotRequired[Sequence[AwsRdsDbProcessorFeatureTypeDef]],
         "ListenerEndpoint": NotRequired[AwsRdsDbInstanceEndpointTypeDef],
         "MaxAllocatedStorage": NotRequired[int],
     },
 )
-AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsPaginatorTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsPaginatorTypeDef",
+AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsExtraOutputTypeDef",
+    {
+        "Predicate": NotRequired[
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef",
     {
         "Predicate": NotRequired[
-            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsPaginatorTypeDef
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef
         ],
     },
 )
 AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
     {
         "Predicate": NotRequired[
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef
         ],
     },
 )
-AwsS3BucketNotificationConfigurationDetailPaginatorTypeDef = TypedDict(
-    "AwsS3BucketNotificationConfigurationDetailPaginatorTypeDef",
+AwsS3BucketNotificationConfigurationDetailExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationDetailExtraOutputTypeDef",
     {
         "Events": NotRequired[List[str]],
-        "Filter": NotRequired[AwsS3BucketNotificationConfigurationFilterPaginatorTypeDef],
+        "Filter": NotRequired[AwsS3BucketNotificationConfigurationFilterExtraOutputTypeDef],
+        "Destination": NotRequired[str],
+        "Type": NotRequired[str],
+    },
+)
+AwsS3BucketNotificationConfigurationDetailOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationDetailOutputTypeDef",
+    {
+        "Events": NotRequired[List[str]],
+        "Filter": NotRequired[AwsS3BucketNotificationConfigurationFilterOutputTypeDef],
         "Destination": NotRequired[str],
         "Type": NotRequired[str],
     },
 )
 AwsS3BucketNotificationConfigurationDetailTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
     {
         "Events": NotRequired[Sequence[str]],
         "Filter": NotRequired[AwsS3BucketNotificationConfigurationFilterTypeDef],
         "Destination": NotRequired[str],
         "Type": NotRequired[str],
     },
 )
-AwsStepFunctionStateMachineDetailsPaginatorTypeDef = TypedDict(
-    "AwsStepFunctionStateMachineDetailsPaginatorTypeDef",
+AwsStepFunctionStateMachineDetailsExtraOutputTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineDetailsExtraOutputTypeDef",
     {
         "Label": NotRequired[str],
         "LoggingConfiguration": NotRequired[
-            AwsStepFunctionStateMachineLoggingConfigurationDetailsPaginatorTypeDef
+            AwsStepFunctionStateMachineLoggingConfigurationDetailsExtraOutputTypeDef
+        ],
+        "Name": NotRequired[str],
+        "RoleArn": NotRequired[str],
+        "StateMachineArn": NotRequired[str],
+        "Status": NotRequired[str],
+        "TracingConfiguration": NotRequired[
+            AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef
+        ],
+        "Type": NotRequired[str],
+    },
+)
+AwsStepFunctionStateMachineDetailsOutputTypeDef = TypedDict(
+    "AwsStepFunctionStateMachineDetailsOutputTypeDef",
+    {
+        "Label": NotRequired[str],
+        "LoggingConfiguration": NotRequired[
+            AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef
         ],
         "Name": NotRequired[str],
         "RoleArn": NotRequired[str],
         "StateMachineArn": NotRequired[str],
         "Status": NotRequired[str],
         "TracingConfiguration": NotRequired[
             AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef
@@ -10819,28 +13815,44 @@
         "Status": NotRequired[str],
         "TracingConfiguration": NotRequired[
             AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef
         ],
         "Type": NotRequired[str],
     },
 )
-AwsWafv2RulesActionDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2RulesActionDetailsPaginatorTypeDef",
+AwsWafv2RulesActionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionDetailsExtraOutputTypeDef",
+    {
+        "Allow": NotRequired[AwsWafv2ActionAllowDetailsExtraOutputTypeDef],
+        "Block": NotRequired[AwsWafv2ActionBlockDetailsExtraOutputTypeDef],
+        "Captcha": NotRequired[AwsWafv2RulesActionCaptchaDetailsExtraOutputTypeDef],
+        "Count": NotRequired[AwsWafv2RulesActionCountDetailsExtraOutputTypeDef],
+    },
+)
+AwsWafv2WebAclActionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2WebAclActionDetailsExtraOutputTypeDef",
     {
-        "Allow": NotRequired[AwsWafv2ActionAllowDetailsPaginatorTypeDef],
-        "Block": NotRequired[AwsWafv2ActionBlockDetailsPaginatorTypeDef],
-        "Captcha": NotRequired[AwsWafv2RulesActionCaptchaDetailsPaginatorTypeDef],
-        "Count": NotRequired[AwsWafv2RulesActionCountDetailsPaginatorTypeDef],
+        "Allow": NotRequired[AwsWafv2ActionAllowDetailsExtraOutputTypeDef],
+        "Block": NotRequired[AwsWafv2ActionBlockDetailsExtraOutputTypeDef],
     },
 )
-AwsWafv2WebAclActionDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2WebAclActionDetailsPaginatorTypeDef",
+AwsWafv2RulesActionDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesActionDetailsOutputTypeDef",
     {
-        "Allow": NotRequired[AwsWafv2ActionAllowDetailsPaginatorTypeDef],
-        "Block": NotRequired[AwsWafv2ActionBlockDetailsPaginatorTypeDef],
+        "Allow": NotRequired[AwsWafv2ActionAllowDetailsOutputTypeDef],
+        "Block": NotRequired[AwsWafv2ActionBlockDetailsOutputTypeDef],
+        "Captcha": NotRequired[AwsWafv2RulesActionCaptchaDetailsOutputTypeDef],
+        "Count": NotRequired[AwsWafv2RulesActionCountDetailsOutputTypeDef],
+    },
+)
+AwsWafv2WebAclActionDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2WebAclActionDetailsOutputTypeDef",
+    {
+        "Allow": NotRequired[AwsWafv2ActionAllowDetailsOutputTypeDef],
+        "Block": NotRequired[AwsWafv2ActionBlockDetailsOutputTypeDef],
     },
 )
 AwsWafv2RulesActionDetailsTypeDef = TypedDict(
     "AwsWafv2RulesActionDetailsTypeDef",
     {
         "Allow": NotRequired[AwsWafv2ActionAllowDetailsTypeDef],
         "Block": NotRequired[AwsWafv2ActionBlockDetailsTypeDef],
@@ -10883,47 +13895,49 @@
     {
         "RuleArn": NotRequired[str],
         "RuleStatus": NotRequired[RuleStatusType],
         "RuleOrder": NotRequired[int],
         "RuleName": NotRequired[str],
         "Description": NotRequired[str],
         "IsTerminal": NotRequired[bool],
-        "Criteria": NotRequired[AutomationRulesFindingFiltersTypeDef],
-        "Actions": NotRequired[List[AutomationRulesActionTypeDef]],
+        "Criteria": NotRequired[AutomationRulesFindingFiltersOutputTypeDef],
+        "Actions": NotRequired[List[AutomationRulesActionOutputTypeDef]],
         "CreatedAt": NotRequired[datetime],
         "UpdatedAt": NotRequired[datetime],
         "CreatedBy": NotRequired[str],
     },
 )
-CreateAutomationRuleRequestRequestTypeDef = TypedDict(
-    "CreateAutomationRuleRequestRequestTypeDef",
-    {
-        "RuleOrder": int,
-        "RuleName": str,
-        "Description": str,
-        "Criteria": AutomationRulesFindingFiltersTypeDef,
-        "Actions": Sequence[AutomationRulesActionTypeDef],
-        "Tags": NotRequired[Mapping[str, str]],
-        "RuleStatus": NotRequired[RuleStatusType],
-        "IsTerminal": NotRequired[bool],
-    },
-)
+AutomationRulesFindingFiltersUnionTypeDef = Union[
+    AutomationRulesFindingFiltersTypeDef, AutomationRulesFindingFiltersOutputTypeDef
+]
 UpdateAutomationRulesRequestItemTypeDef = TypedDict(
     "UpdateAutomationRulesRequestItemTypeDef",
     {
         "RuleArn": str,
         "RuleStatus": NotRequired[RuleStatusType],
         "RuleOrder": NotRequired[int],
         "Description": NotRequired[str],
         "RuleName": NotRequired[str],
         "IsTerminal": NotRequired[bool],
         "Criteria": NotRequired[AutomationRulesFindingFiltersTypeDef],
         "Actions": NotRequired[Sequence[AutomationRulesActionTypeDef]],
     },
 )
+InsightTypeDef = TypedDict(
+    "InsightTypeDef",
+    {
+        "InsightArn": str,
+        "Name": str,
+        "Filters": AwsSecurityFindingFiltersOutputTypeDef,
+        "GroupByAttribute": str,
+    },
+)
+AwsSecurityFindingFiltersUnionTypeDef = Union[
+    AwsSecurityFindingFiltersTypeDef, AwsSecurityFindingFiltersExtraOutputTypeDef
+]
 CreateInsightRequestRequestTypeDef = TypedDict(
     "CreateInsightRequestRequestTypeDef",
     {
         "Name": str,
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "GroupByAttribute": str,
     },
@@ -10941,23 +13955,14 @@
     {
         "Filters": NotRequired[AwsSecurityFindingFiltersTypeDef],
         "SortCriteria": NotRequired[Sequence[SortCriterionTypeDef]],
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
     },
 )
-InsightTypeDef = TypedDict(
-    "InsightTypeDef",
-    {
-        "InsightArn": str,
-        "Name": str,
-        "Filters": AwsSecurityFindingFiltersTypeDef,
-        "GroupByAttribute": str,
-    },
-)
 UpdateFindingsRequestRequestTypeDef = TypedDict(
     "UpdateFindingsRequestRequestTypeDef",
     {
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "Note": NotRequired[NoteUpdateTypeDef],
         "RecordState": NotRequired[RecordStateType],
     },
@@ -10967,47 +13972,73 @@
     {
         "InsightArn": str,
         "Name": NotRequired[str],
         "Filters": NotRequired[AwsSecurityFindingFiltersTypeDef],
         "GroupByAttribute": NotRequired[str],
     },
 )
-NetworkPathComponentPaginatorTypeDef = TypedDict(
-    "NetworkPathComponentPaginatorTypeDef",
+NetworkPathComponentExtraOutputTypeDef = TypedDict(
+    "NetworkPathComponentExtraOutputTypeDef",
+    {
+        "ComponentId": NotRequired[str],
+        "ComponentType": NotRequired[str],
+        "Egress": NotRequired[NetworkHeaderExtraOutputTypeDef],
+        "Ingress": NotRequired[NetworkHeaderExtraOutputTypeDef],
+    },
+)
+NetworkPathComponentOutputTypeDef = TypedDict(
+    "NetworkPathComponentOutputTypeDef",
     {
         "ComponentId": NotRequired[str],
         "ComponentType": NotRequired[str],
-        "Egress": NotRequired[NetworkHeaderPaginatorTypeDef],
-        "Ingress": NotRequired[NetworkHeaderPaginatorTypeDef],
+        "Egress": NotRequired[NetworkHeaderOutputTypeDef],
+        "Ingress": NotRequired[NetworkHeaderOutputTypeDef],
     },
 )
 NetworkPathComponentTypeDef = TypedDict(
     "NetworkPathComponentTypeDef",
     {
         "ComponentId": NotRequired[str],
         "ComponentType": NotRequired[str],
         "Egress": NotRequired[NetworkHeaderTypeDef],
         "Ingress": NotRequired[NetworkHeaderTypeDef],
     },
 )
-CustomDataIdentifiersDetectionsPaginatorTypeDef = TypedDict(
-    "CustomDataIdentifiersDetectionsPaginatorTypeDef",
+CustomDataIdentifiersDetectionsExtraOutputTypeDef = TypedDict(
+    "CustomDataIdentifiersDetectionsExtraOutputTypeDef",
     {
         "Count": NotRequired[int],
         "Arn": NotRequired[str],
         "Name": NotRequired[str],
-        "Occurrences": NotRequired[OccurrencesPaginatorTypeDef],
+        "Occurrences": NotRequired[OccurrencesExtraOutputTypeDef],
     },
 )
-SensitiveDataDetectionsPaginatorTypeDef = TypedDict(
-    "SensitiveDataDetectionsPaginatorTypeDef",
+SensitiveDataDetectionsExtraOutputTypeDef = TypedDict(
+    "SensitiveDataDetectionsExtraOutputTypeDef",
     {
         "Count": NotRequired[int],
         "Type": NotRequired[str],
-        "Occurrences": NotRequired[OccurrencesPaginatorTypeDef],
+        "Occurrences": NotRequired[OccurrencesExtraOutputTypeDef],
+    },
+)
+CustomDataIdentifiersDetectionsOutputTypeDef = TypedDict(
+    "CustomDataIdentifiersDetectionsOutputTypeDef",
+    {
+        "Count": NotRequired[int],
+        "Arn": NotRequired[str],
+        "Name": NotRequired[str],
+        "Occurrences": NotRequired[OccurrencesOutputTypeDef],
+    },
+)
+SensitiveDataDetectionsOutputTypeDef = TypedDict(
+    "SensitiveDataDetectionsOutputTypeDef",
+    {
+        "Count": NotRequired[int],
+        "Type": NotRequired[str],
+        "Occurrences": NotRequired[OccurrencesOutputTypeDef],
     },
 )
 CustomDataIdentifiersDetectionsTypeDef = TypedDict(
     "CustomDataIdentifiersDetectionsTypeDef",
     {
         "Count": NotRequired[int],
         "Arn": NotRequired[str],
@@ -11019,57 +14050,96 @@
     "SensitiveDataDetectionsTypeDef",
     {
         "Count": NotRequired[int],
         "Type": NotRequired[str],
         "Occurrences": NotRequired[OccurrencesTypeDef],
     },
 )
-SecurityControlsConfigurationTypeDef = TypedDict(
-    "SecurityControlsConfigurationTypeDef",
+SecurityControlsConfigurationOutputTypeDef = TypedDict(
+    "SecurityControlsConfigurationOutputTypeDef",
     {
-        "EnabledSecurityControlIdentifiers": NotRequired[Sequence[str]],
-        "DisabledSecurityControlIdentifiers": NotRequired[Sequence[str]],
+        "EnabledSecurityControlIdentifiers": NotRequired[List[str]],
+        "DisabledSecurityControlIdentifiers": NotRequired[List[str]],
         "SecurityControlCustomParameters": NotRequired[
-            Sequence[SecurityControlCustomParameterTypeDef]
+            List[SecurityControlCustomParameterOutputTypeDef]
         ],
     },
 )
 BatchGetSecurityControlsResponseTypeDef = TypedDict(
     "BatchGetSecurityControlsResponseTypeDef",
     {
         "SecurityControls": List[SecurityControlTypeDef],
         "UnprocessedIds": List[UnprocessedSecurityControlTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-RuleGroupSourceStatelessRulesDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRulesDetailsPaginatorTypeDef",
+UpdateSecurityControlRequestRequestTypeDef = TypedDict(
+    "UpdateSecurityControlRequestRequestTypeDef",
+    {
+        "SecurityControlId": str,
+        "Parameters": Mapping[str, ParameterConfigurationUnionTypeDef],
+        "LastUpdateReason": NotRequired[str],
+    },
+)
+SecurityControlsConfigurationTypeDef = TypedDict(
+    "SecurityControlsConfigurationTypeDef",
+    {
+        "EnabledSecurityControlIdentifiers": NotRequired[Sequence[str]],
+        "DisabledSecurityControlIdentifiers": NotRequired[Sequence[str]],
+        "SecurityControlCustomParameters": NotRequired[
+            Sequence[SecurityControlCustomParameterTypeDef]
+        ],
+    },
+)
+RuleGroupSourceStatelessRulesDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRulesDetailsExtraOutputTypeDef",
+    {
+        "Priority": NotRequired[int],
+        "RuleDefinition": NotRequired[RuleGroupSourceStatelessRuleDefinitionExtraOutputTypeDef],
+    },
+)
+RuleGroupSourceStatelessRulesDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRulesDetailsOutputTypeDef",
     {
         "Priority": NotRequired[int],
-        "RuleDefinition": NotRequired[RuleGroupSourceStatelessRuleDefinitionPaginatorTypeDef],
+        "RuleDefinition": NotRequired[RuleGroupSourceStatelessRuleDefinitionOutputTypeDef],
     },
 )
 RuleGroupSourceStatelessRulesDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRulesDetailsTypeDef",
     {
         "Priority": NotRequired[int],
         "RuleDefinition": NotRequired[RuleGroupSourceStatelessRuleDefinitionTypeDef],
     },
 )
-FirewallPolicyStatelessCustomActionsDetailsPaginatorTypeDef = TypedDict(
-    "FirewallPolicyStatelessCustomActionsDetailsPaginatorTypeDef",
+FirewallPolicyStatelessCustomActionsDetailsExtraOutputTypeDef = TypedDict(
+    "FirewallPolicyStatelessCustomActionsDetailsExtraOutputTypeDef",
+    {
+        "ActionDefinition": NotRequired[StatelessCustomActionDefinitionExtraOutputTypeDef],
+        "ActionName": NotRequired[str],
+    },
+)
+RuleGroupSourceCustomActionsDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceCustomActionsDetailsExtraOutputTypeDef",
+    {
+        "ActionDefinition": NotRequired[StatelessCustomActionDefinitionExtraOutputTypeDef],
+        "ActionName": NotRequired[str],
+    },
+)
+FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef = TypedDict(
+    "FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef",
     {
-        "ActionDefinition": NotRequired[StatelessCustomActionDefinitionPaginatorTypeDef],
+        "ActionDefinition": NotRequired[StatelessCustomActionDefinitionOutputTypeDef],
         "ActionName": NotRequired[str],
     },
 )
-RuleGroupSourceCustomActionsDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceCustomActionsDetailsPaginatorTypeDef",
+RuleGroupSourceCustomActionsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceCustomActionsDetailsOutputTypeDef",
     {
-        "ActionDefinition": NotRequired[StatelessCustomActionDefinitionPaginatorTypeDef],
+        "ActionDefinition": NotRequired[StatelessCustomActionDefinitionOutputTypeDef],
         "ActionName": NotRequired[str],
     },
 )
 FirewallPolicyStatelessCustomActionsDetailsTypeDef = TypedDict(
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     {
         "ActionDefinition": NotRequired[StatelessCustomActionDefinitionTypeDef],
@@ -11079,64 +14149,113 @@
 RuleGroupSourceCustomActionsDetailsTypeDef = TypedDict(
     "RuleGroupSourceCustomActionsDetailsTypeDef",
     {
         "ActionDefinition": NotRequired[StatelessCustomActionDefinitionTypeDef],
         "ActionName": NotRequired[str],
     },
 )
-ActionPaginatorTypeDef = TypedDict(
-    "ActionPaginatorTypeDef",
+ActionExtraOutputTypeDef = TypedDict(
+    "ActionExtraOutputTypeDef",
+    {
+        "ActionType": NotRequired[str],
+        "NetworkConnectionAction": NotRequired[NetworkConnectionActionTypeDef],
+        "AwsApiCallAction": NotRequired[AwsApiCallActionExtraOutputTypeDef],
+        "DnsRequestAction": NotRequired[DnsRequestActionTypeDef],
+        "PortProbeAction": NotRequired[PortProbeActionExtraOutputTypeDef],
+    },
+)
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
     {
         "ActionType": NotRequired[str],
         "NetworkConnectionAction": NotRequired[NetworkConnectionActionTypeDef],
-        "AwsApiCallAction": NotRequired[AwsApiCallActionPaginatorTypeDef],
+        "AwsApiCallAction": NotRequired[AwsApiCallActionOutputTypeDef],
         "DnsRequestAction": NotRequired[DnsRequestActionTypeDef],
-        "PortProbeAction": NotRequired[PortProbeActionPaginatorTypeDef],
+        "PortProbeAction": NotRequired[PortProbeActionOutputTypeDef],
     },
 )
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ActionType": NotRequired[str],
         "NetworkConnectionAction": NotRequired[NetworkConnectionActionTypeDef],
         "AwsApiCallAction": NotRequired[AwsApiCallActionTypeDef],
         "DnsRequestAction": NotRequired[DnsRequestActionTypeDef],
         "PortProbeAction": NotRequired[PortProbeActionTypeDef],
     },
 )
-AwsBackupBackupPlanDetailsPaginatorTypeDef = TypedDict(
-    "AwsBackupBackupPlanDetailsPaginatorTypeDef",
+CreateAutomationRuleRequestRequestTypeDef = TypedDict(
+    "CreateAutomationRuleRequestRequestTypeDef",
     {
-        "BackupPlan": NotRequired[AwsBackupBackupPlanBackupPlanDetailsPaginatorTypeDef],
+        "RuleOrder": int,
+        "RuleName": str,
+        "Description": str,
+        "Criteria": AutomationRulesFindingFiltersTypeDef,
+        "Actions": Sequence[AutomationRulesActionUnionTypeDef],
+        "Tags": NotRequired[Mapping[str, str]],
+        "RuleStatus": NotRequired[RuleStatusType],
+        "IsTerminal": NotRequired[bool],
+    },
+)
+AwsBackupBackupPlanDetailsExtraOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanDetailsExtraOutputTypeDef",
+    {
+        "BackupPlan": NotRequired[AwsBackupBackupPlanBackupPlanDetailsExtraOutputTypeDef],
+        "BackupPlanArn": NotRequired[str],
+        "BackupPlanId": NotRequired[str],
+        "VersionId": NotRequired[str],
+    },
+)
+AwsBackupBackupPlanDetailsOutputTypeDef = TypedDict(
+    "AwsBackupBackupPlanDetailsOutputTypeDef",
+    {
+        "BackupPlan": NotRequired[AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef],
         "BackupPlanArn": NotRequired[str],
         "BackupPlanId": NotRequired[str],
         "VersionId": NotRequired[str],
     },
 )
 AwsBackupBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanDetailsTypeDef",
     {
         "BackupPlan": NotRequired[AwsBackupBackupPlanBackupPlanDetailsTypeDef],
         "BackupPlanArn": NotRequired[str],
         "BackupPlanId": NotRequired[str],
         "VersionId": NotRequired[str],
     },
 )
-AwsCloudFrontDistributionDetailsPaginatorTypeDef = TypedDict(
-    "AwsCloudFrontDistributionDetailsPaginatorTypeDef",
+AwsCloudFrontDistributionDetailsExtraOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionDetailsExtraOutputTypeDef",
     {
-        "CacheBehaviors": NotRequired[AwsCloudFrontDistributionCacheBehaviorsPaginatorTypeDef],
+        "CacheBehaviors": NotRequired[AwsCloudFrontDistributionCacheBehaviorsExtraOutputTypeDef],
         "DefaultCacheBehavior": NotRequired[AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef],
         "DefaultRootObject": NotRequired[str],
         "DomainName": NotRequired[str],
         "ETag": NotRequired[str],
         "LastModifiedTime": NotRequired[str],
         "Logging": NotRequired[AwsCloudFrontDistributionLoggingTypeDef],
-        "Origins": NotRequired[AwsCloudFrontDistributionOriginsPaginatorTypeDef],
-        "OriginGroups": NotRequired[AwsCloudFrontDistributionOriginGroupsPaginatorTypeDef],
+        "Origins": NotRequired[AwsCloudFrontDistributionOriginsExtraOutputTypeDef],
+        "OriginGroups": NotRequired[AwsCloudFrontDistributionOriginGroupsExtraOutputTypeDef],
+        "ViewerCertificate": NotRequired[AwsCloudFrontDistributionViewerCertificateTypeDef],
+        "Status": NotRequired[str],
+        "WebAclId": NotRequired[str],
+    },
+)
+AwsCloudFrontDistributionDetailsOutputTypeDef = TypedDict(
+    "AwsCloudFrontDistributionDetailsOutputTypeDef",
+    {
+        "CacheBehaviors": NotRequired[AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef],
+        "DefaultCacheBehavior": NotRequired[AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef],
+        "DefaultRootObject": NotRequired[str],
+        "DomainName": NotRequired[str],
+        "ETag": NotRequired[str],
+        "LastModifiedTime": NotRequired[str],
+        "Logging": NotRequired[AwsCloudFrontDistributionLoggingTypeDef],
+        "Origins": NotRequired[AwsCloudFrontDistributionOriginsOutputTypeDef],
+        "OriginGroups": NotRequired[AwsCloudFrontDistributionOriginGroupsOutputTypeDef],
         "ViewerCertificate": NotRequired[AwsCloudFrontDistributionViewerCertificateTypeDef],
         "Status": NotRequired[str],
         "WebAclId": NotRequired[str],
     },
 )
 AwsCloudFrontDistributionDetailsTypeDef = TypedDict(
     "AwsCloudFrontDistributionDetailsTypeDef",
@@ -11151,16 +14270,26 @@
         "Origins": NotRequired[AwsCloudFrontDistributionOriginsTypeDef],
         "OriginGroups": NotRequired[AwsCloudFrontDistributionOriginGroupsTypeDef],
         "ViewerCertificate": NotRequired[AwsCloudFrontDistributionViewerCertificateTypeDef],
         "Status": NotRequired[str],
         "WebAclId": NotRequired[str],
     },
 )
-AwsGuardDutyDetectorDetailsPaginatorTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDetailsPaginatorTypeDef",
+AwsGuardDutyDetectorDetailsExtraOutputTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDetailsExtraOutputTypeDef",
+    {
+        "DataSources": NotRequired[AwsGuardDutyDetectorDataSourcesDetailsTypeDef],
+        "Features": NotRequired[List[AwsGuardDutyDetectorFeaturesDetailsTypeDef]],
+        "FindingPublishingFrequency": NotRequired[str],
+        "ServiceRole": NotRequired[str],
+        "Status": NotRequired[str],
+    },
+)
+AwsGuardDutyDetectorDetailsOutputTypeDef = TypedDict(
+    "AwsGuardDutyDetectorDetailsOutputTypeDef",
     {
         "DataSources": NotRequired[AwsGuardDutyDetectorDataSourcesDetailsTypeDef],
         "Features": NotRequired[List[AwsGuardDutyDetectorFeaturesDetailsTypeDef]],
         "FindingPublishingFrequency": NotRequired[str],
         "ServiceRole": NotRequired[str],
         "Status": NotRequired[str],
     },
@@ -11171,37 +14300,69 @@
         "DataSources": NotRequired[AwsGuardDutyDetectorDataSourcesDetailsTypeDef],
         "Features": NotRequired[Sequence[AwsGuardDutyDetectorFeaturesDetailsTypeDef]],
         "FindingPublishingFrequency": NotRequired[str],
         "ServiceRole": NotRequired[str],
         "Status": NotRequired[str],
     },
 )
-AwsMskClusterDetailsPaginatorTypeDef = TypedDict(
-    "AwsMskClusterDetailsPaginatorTypeDef",
+AwsMskClusterDetailsExtraOutputTypeDef = TypedDict(
+    "AwsMskClusterDetailsExtraOutputTypeDef",
     {
-        "ClusterInfo": NotRequired[AwsMskClusterClusterInfoDetailsPaginatorTypeDef],
+        "ClusterInfo": NotRequired[AwsMskClusterClusterInfoDetailsExtraOutputTypeDef],
+    },
+)
+AwsMskClusterDetailsOutputTypeDef = TypedDict(
+    "AwsMskClusterDetailsOutputTypeDef",
+    {
+        "ClusterInfo": NotRequired[AwsMskClusterClusterInfoDetailsOutputTypeDef],
     },
 )
 AwsMskClusterDetailsTypeDef = TypedDict(
     "AwsMskClusterDetailsTypeDef",
     {
         "ClusterInfo": NotRequired[AwsMskClusterClusterInfoDetailsTypeDef],
     },
 )
-AwsS3BucketBucketLifecycleConfigurationRulesDetailsPaginatorTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsPaginatorTypeDef",
+AwsS3BucketBucketLifecycleConfigurationRulesDetailsExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsExtraOutputTypeDef",
+    {
+        "AbortIncompleteMultipartUpload": NotRequired[
+            AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
+        ],
+        "ExpirationDate": NotRequired[str],
+        "ExpirationInDays": NotRequired[int],
+        "ExpiredObjectDeleteMarker": NotRequired[bool],
+        "Filter": NotRequired[
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsExtraOutputTypeDef
+        ],
+        "ID": NotRequired[str],
+        "NoncurrentVersionExpirationInDays": NotRequired[int],
+        "NoncurrentVersionTransitions": NotRequired[
+            List[
+                AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef
+            ]
+        ],
+        "Prefix": NotRequired[str],
+        "Status": NotRequired[str],
+        "Transitions": NotRequired[
+            List[AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef]
+        ],
+    },
+)
+AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef",
     {
         "AbortIncompleteMultipartUpload": NotRequired[
             AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
         ],
         "ExpirationDate": NotRequired[str],
         "ExpirationInDays": NotRequired[int],
         "ExpiredObjectDeleteMarker": NotRequired[bool],
         "Filter": NotRequired[
-            AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsPaginatorTypeDef
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef
         ],
         "ID": NotRequired[str],
         "NoncurrentVersionExpirationInDays": NotRequired[int],
         "NoncurrentVersionTransitions": NotRequired[
             List[
                 AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef
             ]
@@ -11233,32 +14394,50 @@
         "Prefix": NotRequired[str],
         "Status": NotRequired[str],
         "Transitions": NotRequired[
             Sequence[AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef]
         ],
     },
 )
-AwsS3BucketNotificationConfigurationPaginatorTypeDef = TypedDict(
-    "AwsS3BucketNotificationConfigurationPaginatorTypeDef",
+AwsS3BucketNotificationConfigurationExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationExtraOutputTypeDef",
     {
         "Configurations": NotRequired[
-            List[AwsS3BucketNotificationConfigurationDetailPaginatorTypeDef]
+            List[AwsS3BucketNotificationConfigurationDetailExtraOutputTypeDef]
+        ],
+    },
+)
+AwsS3BucketNotificationConfigurationOutputTypeDef = TypedDict(
+    "AwsS3BucketNotificationConfigurationOutputTypeDef",
+    {
+        "Configurations": NotRequired[
+            List[AwsS3BucketNotificationConfigurationDetailOutputTypeDef]
         ],
     },
 )
 AwsS3BucketNotificationConfigurationTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationTypeDef",
     {
         "Configurations": NotRequired[Sequence[AwsS3BucketNotificationConfigurationDetailTypeDef]],
     },
 )
-AwsWafv2RulesDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2RulesDetailsPaginatorTypeDef",
+AwsWafv2RulesDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2RulesDetailsExtraOutputTypeDef",
+    {
+        "Action": NotRequired[AwsWafv2RulesActionDetailsExtraOutputTypeDef],
+        "Name": NotRequired[str],
+        "OverrideAction": NotRequired[str],
+        "Priority": NotRequired[int],
+        "VisibilityConfig": NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],
+    },
+)
+AwsWafv2RulesDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RulesDetailsOutputTypeDef",
     {
-        "Action": NotRequired[AwsWafv2RulesActionDetailsPaginatorTypeDef],
+        "Action": NotRequired[AwsWafv2RulesActionDetailsOutputTypeDef],
         "Name": NotRequired[str],
         "OverrideAction": NotRequired[str],
         "Priority": NotRequired[int],
         "VisibilityConfig": NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],
     },
 )
 AwsWafv2RulesDetailsTypeDef = TypedDict(
@@ -11278,16 +14457,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListSecurityControlDefinitionsResponseTypeDef = TypedDict(
     "ListSecurityControlDefinitionsResponseTypeDef",
     {
         "SecurityControlDefinitions": List[SecurityControlDefinitionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 BatchGetAutomationRulesResponseTypeDef = TypedDict(
     "BatchGetAutomationRulesResponseTypeDef",
     {
         "Rules": List[AutomationRulesConfigTypeDef],
         "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
@@ -11300,30 +14479,45 @@
         "UpdateAutomationRulesRequestItems": Sequence[UpdateAutomationRulesRequestItemTypeDef],
     },
 )
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "Insights": List[InsightTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+CustomDataIdentifiersResultExtraOutputTypeDef = TypedDict(
+    "CustomDataIdentifiersResultExtraOutputTypeDef",
+    {
+        "Detections": NotRequired[List[CustomDataIdentifiersDetectionsExtraOutputTypeDef]],
+        "TotalCount": NotRequired[int],
+    },
+)
+SensitiveDataResultExtraOutputTypeDef = TypedDict(
+    "SensitiveDataResultExtraOutputTypeDef",
+    {
+        "Category": NotRequired[str],
+        "Detections": NotRequired[List[SensitiveDataDetectionsExtraOutputTypeDef]],
+        "TotalCount": NotRequired[int],
     },
 )
-CustomDataIdentifiersResultPaginatorTypeDef = TypedDict(
-    "CustomDataIdentifiersResultPaginatorTypeDef",
+CustomDataIdentifiersResultOutputTypeDef = TypedDict(
+    "CustomDataIdentifiersResultOutputTypeDef",
     {
-        "Detections": NotRequired[List[CustomDataIdentifiersDetectionsPaginatorTypeDef]],
+        "Detections": NotRequired[List[CustomDataIdentifiersDetectionsOutputTypeDef]],
         "TotalCount": NotRequired[int],
     },
 )
-SensitiveDataResultPaginatorTypeDef = TypedDict(
-    "SensitiveDataResultPaginatorTypeDef",
+SensitiveDataResultOutputTypeDef = TypedDict(
+    "SensitiveDataResultOutputTypeDef",
     {
         "Category": NotRequired[str],
-        "Detections": NotRequired[List[SensitiveDataDetectionsPaginatorTypeDef]],
+        "Detections": NotRequired[List[SensitiveDataDetectionsOutputTypeDef]],
         "TotalCount": NotRequired[int],
     },
 )
 CustomDataIdentifiersResultTypeDef = TypedDict(
     "CustomDataIdentifiersResultTypeDef",
     {
         "Detections": NotRequired[Sequence[CustomDataIdentifiersDetectionsTypeDef]],
@@ -11334,43 +14528,74 @@
     "SensitiveDataResultTypeDef",
     {
         "Category": NotRequired[str],
         "Detections": NotRequired[Sequence[SensitiveDataDetectionsTypeDef]],
         "TotalCount": NotRequired[int],
     },
 )
+SecurityHubPolicyOutputTypeDef = TypedDict(
+    "SecurityHubPolicyOutputTypeDef",
+    {
+        "ServiceEnabled": NotRequired[bool],
+        "EnabledStandardIdentifiers": NotRequired[List[str]],
+        "SecurityControlsConfiguration": NotRequired[SecurityControlsConfigurationOutputTypeDef],
+    },
+)
 SecurityHubPolicyTypeDef = TypedDict(
     "SecurityHubPolicyTypeDef",
     {
         "ServiceEnabled": NotRequired[bool],
         "EnabledStandardIdentifiers": NotRequired[Sequence[str]],
         "SecurityControlsConfiguration": NotRequired[SecurityControlsConfigurationTypeDef],
     },
 )
-FirewallPolicyDetailsPaginatorTypeDef = TypedDict(
-    "FirewallPolicyDetailsPaginatorTypeDef",
+FirewallPolicyDetailsExtraOutputTypeDef = TypedDict(
+    "FirewallPolicyDetailsExtraOutputTypeDef",
     {
         "StatefulRuleGroupReferences": NotRequired[
             List[FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef]
         ],
         "StatelessCustomActions": NotRequired[
-            List[FirewallPolicyStatelessCustomActionsDetailsPaginatorTypeDef]
+            List[FirewallPolicyStatelessCustomActionsDetailsExtraOutputTypeDef]
         ],
         "StatelessDefaultActions": NotRequired[List[str]],
         "StatelessFragmentDefaultActions": NotRequired[List[str]],
         "StatelessRuleGroupReferences": NotRequired[
             List[FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef]
         ],
     },
 )
-RuleGroupSourceStatelessRulesAndCustomActionsDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsPaginatorTypeDef",
+RuleGroupSourceStatelessRulesAndCustomActionsDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsExtraOutputTypeDef",
     {
-        "CustomActions": NotRequired[List[RuleGroupSourceCustomActionsDetailsPaginatorTypeDef]],
-        "StatelessRules": NotRequired[List[RuleGroupSourceStatelessRulesDetailsPaginatorTypeDef]],
+        "CustomActions": NotRequired[List[RuleGroupSourceCustomActionsDetailsExtraOutputTypeDef]],
+        "StatelessRules": NotRequired[List[RuleGroupSourceStatelessRulesDetailsExtraOutputTypeDef]],
+    },
+)
+FirewallPolicyDetailsOutputTypeDef = TypedDict(
+    "FirewallPolicyDetailsOutputTypeDef",
+    {
+        "StatefulRuleGroupReferences": NotRequired[
+            List[FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef]
+        ],
+        "StatelessCustomActions": NotRequired[
+            List[FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef]
+        ],
+        "StatelessDefaultActions": NotRequired[List[str]],
+        "StatelessFragmentDefaultActions": NotRequired[List[str]],
+        "StatelessRuleGroupReferences": NotRequired[
+            List[FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef]
+        ],
+    },
+)
+RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef",
+    {
+        "CustomActions": NotRequired[List[RuleGroupSourceCustomActionsDetailsOutputTypeDef]],
+        "StatelessRules": NotRequired[List[RuleGroupSourceStatelessRulesDetailsOutputTypeDef]],
     },
 )
 FirewallPolicyDetailsTypeDef = TypedDict(
     "FirewallPolicyDetailsTypeDef",
     {
         "StatefulRuleGroupReferences": NotRequired[
             Sequence[FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef]
@@ -11388,53 +14613,89 @@
 RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef",
     {
         "CustomActions": NotRequired[Sequence[RuleGroupSourceCustomActionsDetailsTypeDef]],
         "StatelessRules": NotRequired[Sequence[RuleGroupSourceStatelessRulesDetailsTypeDef]],
     },
 )
-AwsS3BucketBucketLifecycleConfigurationDetailsPaginatorTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationDetailsPaginatorTypeDef",
+AwsS3BucketBucketLifecycleConfigurationDetailsExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationDetailsExtraOutputTypeDef",
     {
         "Rules": NotRequired[
-            List[AwsS3BucketBucketLifecycleConfigurationRulesDetailsPaginatorTypeDef]
+            List[AwsS3BucketBucketLifecycleConfigurationRulesDetailsExtraOutputTypeDef]
+        ],
+    },
+)
+AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef",
+    {
+        "Rules": NotRequired[
+            List[AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef]
         ],
     },
 )
 AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
     {
         "Rules": NotRequired[Sequence[AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef]],
     },
 )
-AwsWafv2RuleGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2RuleGroupDetailsPaginatorTypeDef",
+AwsWafv2RuleGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2RuleGroupDetailsExtraOutputTypeDef",
     {
         "Capacity": NotRequired[int],
         "Description": NotRequired[str],
         "Id": NotRequired[str],
         "Name": NotRequired[str],
         "Arn": NotRequired[str],
-        "Rules": NotRequired[List[AwsWafv2RulesDetailsPaginatorTypeDef]],
+        "Rules": NotRequired[List[AwsWafv2RulesDetailsExtraOutputTypeDef]],
         "Scope": NotRequired[str],
         "VisibilityConfig": NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],
     },
 )
-AwsWafv2WebAclDetailsPaginatorTypeDef = TypedDict(
-    "AwsWafv2WebAclDetailsPaginatorTypeDef",
+AwsWafv2WebAclDetailsExtraOutputTypeDef = TypedDict(
+    "AwsWafv2WebAclDetailsExtraOutputTypeDef",
     {
         "Name": NotRequired[str],
         "Arn": NotRequired[str],
         "ManagedbyFirewallManager": NotRequired[bool],
         "Id": NotRequired[str],
         "Capacity": NotRequired[int],
         "CaptchaConfig": NotRequired[AwsWafv2WebAclCaptchaConfigDetailsTypeDef],
-        "DefaultAction": NotRequired[AwsWafv2WebAclActionDetailsPaginatorTypeDef],
+        "DefaultAction": NotRequired[AwsWafv2WebAclActionDetailsExtraOutputTypeDef],
         "Description": NotRequired[str],
-        "Rules": NotRequired[List[AwsWafv2RulesDetailsPaginatorTypeDef]],
+        "Rules": NotRequired[List[AwsWafv2RulesDetailsExtraOutputTypeDef]],
+        "VisibilityConfig": NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],
+    },
+)
+AwsWafv2RuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2RuleGroupDetailsOutputTypeDef",
+    {
+        "Capacity": NotRequired[int],
+        "Description": NotRequired[str],
+        "Id": NotRequired[str],
+        "Name": NotRequired[str],
+        "Arn": NotRequired[str],
+        "Rules": NotRequired[List[AwsWafv2RulesDetailsOutputTypeDef]],
+        "Scope": NotRequired[str],
+        "VisibilityConfig": NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],
+    },
+)
+AwsWafv2WebAclDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2WebAclDetailsOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "Arn": NotRequired[str],
+        "ManagedbyFirewallManager": NotRequired[bool],
+        "Id": NotRequired[str],
+        "Capacity": NotRequired[int],
+        "CaptchaConfig": NotRequired[AwsWafv2WebAclCaptchaConfigDetailsTypeDef],
+        "DefaultAction": NotRequired[AwsWafv2WebAclActionDetailsOutputTypeDef],
+        "Description": NotRequired[str],
+        "Rules": NotRequired[List[AwsWafv2RulesDetailsOutputTypeDef]],
         "VisibilityConfig": NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],
     },
 )
 AwsWafv2RuleGroupDetailsTypeDef = TypedDict(
     "AwsWafv2RuleGroupDetailsTypeDef",
     {
         "Capacity": NotRequired[int],
@@ -11458,60 +14719,98 @@
         "CaptchaConfig": NotRequired[AwsWafv2WebAclCaptchaConfigDetailsTypeDef],
         "DefaultAction": NotRequired[AwsWafv2WebAclActionDetailsTypeDef],
         "Description": NotRequired[str],
         "Rules": NotRequired[Sequence[AwsWafv2RulesDetailsTypeDef]],
         "VisibilityConfig": NotRequired[AwsWafv2VisibilityConfigDetailsTypeDef],
     },
 )
-ClassificationResultPaginatorTypeDef = TypedDict(
-    "ClassificationResultPaginatorTypeDef",
+ClassificationResultExtraOutputTypeDef = TypedDict(
+    "ClassificationResultExtraOutputTypeDef",
+    {
+        "MimeType": NotRequired[str],
+        "SizeClassified": NotRequired[int],
+        "AdditionalOccurrences": NotRequired[bool],
+        "Status": NotRequired[ClassificationStatusTypeDef],
+        "SensitiveData": NotRequired[List[SensitiveDataResultExtraOutputTypeDef]],
+        "CustomDataIdentifiers": NotRequired[CustomDataIdentifiersResultExtraOutputTypeDef],
+    },
+)
+ClassificationResultOutputTypeDef = TypedDict(
+    "ClassificationResultOutputTypeDef",
     {
         "MimeType": NotRequired[str],
         "SizeClassified": NotRequired[int],
         "AdditionalOccurrences": NotRequired[bool],
         "Status": NotRequired[ClassificationStatusTypeDef],
-        "SensitiveData": NotRequired[List[SensitiveDataResultPaginatorTypeDef]],
-        "CustomDataIdentifiers": NotRequired[CustomDataIdentifiersResultPaginatorTypeDef],
+        "SensitiveData": NotRequired[List[SensitiveDataResultOutputTypeDef]],
+        "CustomDataIdentifiers": NotRequired[CustomDataIdentifiersResultOutputTypeDef],
     },
 )
 ClassificationResultTypeDef = TypedDict(
     "ClassificationResultTypeDef",
     {
         "MimeType": NotRequired[str],
         "SizeClassified": NotRequired[int],
         "AdditionalOccurrences": NotRequired[bool],
         "Status": NotRequired[ClassificationStatusTypeDef],
         "SensitiveData": NotRequired[Sequence[SensitiveDataResultTypeDef]],
         "CustomDataIdentifiers": NotRequired[CustomDataIdentifiersResultTypeDef],
     },
 )
+PolicyOutputTypeDef = TypedDict(
+    "PolicyOutputTypeDef",
+    {
+        "SecurityHub": NotRequired[SecurityHubPolicyOutputTypeDef],
+    },
+)
 PolicyTypeDef = TypedDict(
     "PolicyTypeDef",
     {
         "SecurityHub": NotRequired[SecurityHubPolicyTypeDef],
     },
 )
-AwsNetworkFirewallFirewallPolicyDetailsPaginatorTypeDef = TypedDict(
-    "AwsNetworkFirewallFirewallPolicyDetailsPaginatorTypeDef",
+AwsNetworkFirewallFirewallPolicyDetailsExtraOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallFirewallPolicyDetailsExtraOutputTypeDef",
     {
-        "FirewallPolicy": NotRequired[FirewallPolicyDetailsPaginatorTypeDef],
+        "FirewallPolicy": NotRequired[FirewallPolicyDetailsExtraOutputTypeDef],
         "FirewallPolicyArn": NotRequired[str],
         "FirewallPolicyId": NotRequired[str],
         "FirewallPolicyName": NotRequired[str],
         "Description": NotRequired[str],
     },
 )
-RuleGroupSourcePaginatorTypeDef = TypedDict(
-    "RuleGroupSourcePaginatorTypeDef",
+RuleGroupSourceExtraOutputTypeDef = TypedDict(
+    "RuleGroupSourceExtraOutputTypeDef",
     {
-        "RulesSourceList": NotRequired[RuleGroupSourceListDetailsPaginatorTypeDef],
+        "RulesSourceList": NotRequired[RuleGroupSourceListDetailsExtraOutputTypeDef],
         "RulesString": NotRequired[str],
-        "StatefulRules": NotRequired[List[RuleGroupSourceStatefulRulesDetailsPaginatorTypeDef]],
+        "StatefulRules": NotRequired[List[RuleGroupSourceStatefulRulesDetailsExtraOutputTypeDef]],
         "StatelessRulesAndCustomActions": NotRequired[
-            RuleGroupSourceStatelessRulesAndCustomActionsDetailsPaginatorTypeDef
+            RuleGroupSourceStatelessRulesAndCustomActionsDetailsExtraOutputTypeDef
+        ],
+    },
+)
+AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef",
+    {
+        "FirewallPolicy": NotRequired[FirewallPolicyDetailsOutputTypeDef],
+        "FirewallPolicyArn": NotRequired[str],
+        "FirewallPolicyId": NotRequired[str],
+        "FirewallPolicyName": NotRequired[str],
+        "Description": NotRequired[str],
+    },
+)
+RuleGroupSourceOutputTypeDef = TypedDict(
+    "RuleGroupSourceOutputTypeDef",
+    {
+        "RulesSourceList": NotRequired[RuleGroupSourceListDetailsOutputTypeDef],
+        "RulesString": NotRequired[str],
+        "StatefulRules": NotRequired[List[RuleGroupSourceStatefulRulesDetailsOutputTypeDef]],
+        "StatelessRulesAndCustomActions": NotRequired[
+            RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef
         ],
     },
 )
 AwsNetworkFirewallFirewallPolicyDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallPolicyDetailsTypeDef",
     {
         "FirewallPolicy": NotRequired[FirewallPolicyDetailsTypeDef],
@@ -11528,33 +14827,62 @@
         "RulesString": NotRequired[str],
         "StatefulRules": NotRequired[Sequence[RuleGroupSourceStatefulRulesDetailsTypeDef]],
         "StatelessRulesAndCustomActions": NotRequired[
             RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef
         ],
     },
 )
-AwsS3BucketDetailsPaginatorTypeDef = TypedDict(
-    "AwsS3BucketDetailsPaginatorTypeDef",
+AwsS3BucketDetailsExtraOutputTypeDef = TypedDict(
+    "AwsS3BucketDetailsExtraOutputTypeDef",
     {
         "OwnerId": NotRequired[str],
         "OwnerName": NotRequired[str],
         "OwnerAccountId": NotRequired[str],
         "CreatedAt": NotRequired[str],
         "ServerSideEncryptionConfiguration": NotRequired[
-            AwsS3BucketServerSideEncryptionConfigurationPaginatorTypeDef
+            AwsS3BucketServerSideEncryptionConfigurationExtraOutputTypeDef
         ],
         "BucketLifecycleConfiguration": NotRequired[
-            AwsS3BucketBucketLifecycleConfigurationDetailsPaginatorTypeDef
+            AwsS3BucketBucketLifecycleConfigurationDetailsExtraOutputTypeDef
         ],
         "PublicAccessBlockConfiguration": NotRequired[AwsS3AccountPublicAccessBlockDetailsTypeDef],
         "AccessControlList": NotRequired[str],
         "BucketLoggingConfiguration": NotRequired[AwsS3BucketLoggingConfigurationTypeDef],
-        "BucketWebsiteConfiguration": NotRequired[AwsS3BucketWebsiteConfigurationPaginatorTypeDef],
+        "BucketWebsiteConfiguration": NotRequired[
+            AwsS3BucketWebsiteConfigurationExtraOutputTypeDef
+        ],
         "BucketNotificationConfiguration": NotRequired[
-            AwsS3BucketNotificationConfigurationPaginatorTypeDef
+            AwsS3BucketNotificationConfigurationExtraOutputTypeDef
+        ],
+        "BucketVersioningConfiguration": NotRequired[
+            AwsS3BucketBucketVersioningConfigurationTypeDef
+        ],
+        "ObjectLockConfiguration": NotRequired[AwsS3BucketObjectLockConfigurationTypeDef],
+        "Name": NotRequired[str],
+    },
+)
+AwsS3BucketDetailsOutputTypeDef = TypedDict(
+    "AwsS3BucketDetailsOutputTypeDef",
+    {
+        "OwnerId": NotRequired[str],
+        "OwnerName": NotRequired[str],
+        "OwnerAccountId": NotRequired[str],
+        "CreatedAt": NotRequired[str],
+        "ServerSideEncryptionConfiguration": NotRequired[
+            AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef
+        ],
+        "BucketLifecycleConfiguration": NotRequired[
+            AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef
+        ],
+        "PublicAccessBlockConfiguration": NotRequired[AwsS3AccountPublicAccessBlockDetailsTypeDef],
+        "AccessControlList": NotRequired[str],
+        "BucketLoggingConfiguration": NotRequired[AwsS3BucketLoggingConfigurationTypeDef],
+        "BucketWebsiteConfiguration": NotRequired[AwsS3BucketWebsiteConfigurationOutputTypeDef],
+        "BucketNotificationConfiguration": NotRequired[
+            AwsS3BucketNotificationConfigurationOutputTypeDef
         ],
         "BucketVersioningConfiguration": NotRequired[
             AwsS3BucketBucketVersioningConfigurationTypeDef
         ],
         "ObjectLockConfiguration": NotRequired[AwsS3BucketObjectLockConfigurationTypeDef],
         "Name": NotRequired[str],
     },
@@ -11580,106 +14908,133 @@
         "BucketVersioningConfiguration": NotRequired[
             AwsS3BucketBucketVersioningConfigurationTypeDef
         ],
         "ObjectLockConfiguration": NotRequired[AwsS3BucketObjectLockConfigurationTypeDef],
         "Name": NotRequired[str],
     },
 )
-DataClassificationDetailsPaginatorTypeDef = TypedDict(
-    "DataClassificationDetailsPaginatorTypeDef",
+DataClassificationDetailsExtraOutputTypeDef = TypedDict(
+    "DataClassificationDetailsExtraOutputTypeDef",
     {
         "DetailedResultsLocation": NotRequired[str],
-        "Result": NotRequired[ClassificationResultPaginatorTypeDef],
+        "Result": NotRequired[ClassificationResultExtraOutputTypeDef],
     },
 )
-DataClassificationDetailsTypeDef = TypedDict(
-    "DataClassificationDetailsTypeDef",
+DataClassificationDetailsOutputTypeDef = TypedDict(
+    "DataClassificationDetailsOutputTypeDef",
     {
         "DetailedResultsLocation": NotRequired[str],
-        "Result": NotRequired[ClassificationResultTypeDef],
+        "Result": NotRequired[ClassificationResultOutputTypeDef],
     },
 )
-CreateConfigurationPolicyRequestRequestTypeDef = TypedDict(
-    "CreateConfigurationPolicyRequestRequestTypeDef",
+DataClassificationDetailsTypeDef = TypedDict(
+    "DataClassificationDetailsTypeDef",
     {
-        "Name": str,
-        "ConfigurationPolicy": PolicyTypeDef,
-        "Description": NotRequired[str],
-        "Tags": NotRequired[Mapping[str, str]],
+        "DetailedResultsLocation": NotRequired[str],
+        "Result": NotRequired[ClassificationResultTypeDef],
     },
 )
 CreateConfigurationPolicyResponseTypeDef = TypedDict(
     "CreateConfigurationPolicyResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "UpdatedAt": datetime,
         "CreatedAt": datetime,
-        "ConfigurationPolicy": PolicyTypeDef,
+        "ConfigurationPolicy": PolicyOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetConfigurationPolicyResponseTypeDef = TypedDict(
     "GetConfigurationPolicyResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "UpdatedAt": datetime,
         "CreatedAt": datetime,
-        "ConfigurationPolicy": PolicyTypeDef,
+        "ConfigurationPolicy": PolicyOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateConfigurationPolicyResponseTypeDef = TypedDict(
+    "UpdateConfigurationPolicyResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "UpdatedAt": datetime,
+        "CreatedAt": datetime,
+        "ConfigurationPolicy": PolicyOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateConfigurationPolicyRequestRequestTypeDef = TypedDict(
+    "CreateConfigurationPolicyRequestRequestTypeDef",
+    {
+        "Name": str,
+        "ConfigurationPolicy": PolicyTypeDef,
+        "Description": NotRequired[str],
+        "Tags": NotRequired[Mapping[str, str]],
+    },
+)
+PolicyUnionTypeDef = Union[PolicyTypeDef, PolicyOutputTypeDef]
 UpdateConfigurationPolicyRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationPolicyRequestRequestTypeDef",
     {
         "Identifier": str,
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "UpdatedReason": NotRequired[str],
         "ConfigurationPolicy": NotRequired[PolicyTypeDef],
     },
 )
-UpdateConfigurationPolicyResponseTypeDef = TypedDict(
-    "UpdateConfigurationPolicyResponseTypeDef",
+RuleGroupDetailsExtraOutputTypeDef = TypedDict(
+    "RuleGroupDetailsExtraOutputTypeDef",
     {
-        "Arn": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "UpdatedAt": datetime,
-        "CreatedAt": datetime,
-        "ConfigurationPolicy": PolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RuleVariables": NotRequired[RuleGroupVariablesExtraOutputTypeDef],
+        "RulesSource": NotRequired[RuleGroupSourceExtraOutputTypeDef],
     },
 )
-RuleGroupDetailsPaginatorTypeDef = TypedDict(
-    "RuleGroupDetailsPaginatorTypeDef",
+RuleGroupDetailsOutputTypeDef = TypedDict(
+    "RuleGroupDetailsOutputTypeDef",
     {
-        "RuleVariables": NotRequired[RuleGroupVariablesPaginatorTypeDef],
-        "RulesSource": NotRequired[RuleGroupSourcePaginatorTypeDef],
+        "RuleVariables": NotRequired[RuleGroupVariablesOutputTypeDef],
+        "RulesSource": NotRequired[RuleGroupSourceOutputTypeDef],
     },
 )
 RuleGroupDetailsTypeDef = TypedDict(
     "RuleGroupDetailsTypeDef",
     {
         "RuleVariables": NotRequired[RuleGroupVariablesTypeDef],
         "RulesSource": NotRequired[RuleGroupSourceTypeDef],
     },
 )
-AwsNetworkFirewallRuleGroupDetailsPaginatorTypeDef = TypedDict(
-    "AwsNetworkFirewallRuleGroupDetailsPaginatorTypeDef",
+AwsNetworkFirewallRuleGroupDetailsExtraOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallRuleGroupDetailsExtraOutputTypeDef",
     {
         "Capacity": NotRequired[int],
         "Description": NotRequired[str],
-        "RuleGroup": NotRequired[RuleGroupDetailsPaginatorTypeDef],
+        "RuleGroup": NotRequired[RuleGroupDetailsExtraOutputTypeDef],
+        "RuleGroupArn": NotRequired[str],
+        "RuleGroupId": NotRequired[str],
+        "RuleGroupName": NotRequired[str],
+        "Type": NotRequired[str],
+    },
+)
+AwsNetworkFirewallRuleGroupDetailsOutputTypeDef = TypedDict(
+    "AwsNetworkFirewallRuleGroupDetailsOutputTypeDef",
+    {
+        "Capacity": NotRequired[int],
+        "Description": NotRequired[str],
+        "RuleGroup": NotRequired[RuleGroupDetailsOutputTypeDef],
         "RuleGroupArn": NotRequired[str],
         "RuleGroupId": NotRequired[str],
         "RuleGroupName": NotRequired[str],
         "Type": NotRequired[str],
     },
 )
 AwsNetworkFirewallRuleGroupDetailsTypeDef = TypedDict(
@@ -11690,140 +15045,260 @@
         "RuleGroup": NotRequired[RuleGroupDetailsTypeDef],
         "RuleGroupArn": NotRequired[str],
         "RuleGroupId": NotRequired[str],
         "RuleGroupName": NotRequired[str],
         "Type": NotRequired[str],
     },
 )
-ResourceDetailsPaginatorTypeDef = TypedDict(
-    "ResourceDetailsPaginatorTypeDef",
+ResourceDetailsExtraOutputTypeDef = TypedDict(
+    "ResourceDetailsExtraOutputTypeDef",
     {
         "AwsAutoScalingAutoScalingGroup": NotRequired[
-            AwsAutoScalingAutoScalingGroupDetailsPaginatorTypeDef
+            AwsAutoScalingAutoScalingGroupDetailsExtraOutputTypeDef
         ],
-        "AwsCodeBuildProject": NotRequired[AwsCodeBuildProjectDetailsPaginatorTypeDef],
-        "AwsCloudFrontDistribution": NotRequired[AwsCloudFrontDistributionDetailsPaginatorTypeDef],
-        "AwsEc2Instance": NotRequired[AwsEc2InstanceDetailsPaginatorTypeDef],
-        "AwsEc2NetworkInterface": NotRequired[AwsEc2NetworkInterfaceDetailsPaginatorTypeDef],
-        "AwsEc2SecurityGroup": NotRequired[AwsEc2SecurityGroupDetailsPaginatorTypeDef],
-        "AwsEc2Volume": NotRequired[AwsEc2VolumeDetailsPaginatorTypeDef],
-        "AwsEc2Vpc": NotRequired[AwsEc2VpcDetailsPaginatorTypeDef],
+        "AwsCodeBuildProject": NotRequired[AwsCodeBuildProjectDetailsExtraOutputTypeDef],
+        "AwsCloudFrontDistribution": NotRequired[
+            AwsCloudFrontDistributionDetailsExtraOutputTypeDef
+        ],
+        "AwsEc2Instance": NotRequired[AwsEc2InstanceDetailsExtraOutputTypeDef],
+        "AwsEc2NetworkInterface": NotRequired[AwsEc2NetworkInterfaceDetailsExtraOutputTypeDef],
+        "AwsEc2SecurityGroup": NotRequired[AwsEc2SecurityGroupDetailsExtraOutputTypeDef],
+        "AwsEc2Volume": NotRequired[AwsEc2VolumeDetailsExtraOutputTypeDef],
+        "AwsEc2Vpc": NotRequired[AwsEc2VpcDetailsExtraOutputTypeDef],
         "AwsEc2Eip": NotRequired[AwsEc2EipDetailsTypeDef],
-        "AwsEc2Subnet": NotRequired[AwsEc2SubnetDetailsPaginatorTypeDef],
-        "AwsEc2NetworkAcl": NotRequired[AwsEc2NetworkAclDetailsPaginatorTypeDef],
-        "AwsElbv2LoadBalancer": NotRequired[AwsElbv2LoadBalancerDetailsPaginatorTypeDef],
+        "AwsEc2Subnet": NotRequired[AwsEc2SubnetDetailsExtraOutputTypeDef],
+        "AwsEc2NetworkAcl": NotRequired[AwsEc2NetworkAclDetailsExtraOutputTypeDef],
+        "AwsElbv2LoadBalancer": NotRequired[AwsElbv2LoadBalancerDetailsExtraOutputTypeDef],
         "AwsElasticBeanstalkEnvironment": NotRequired[
-            AwsElasticBeanstalkEnvironmentDetailsPaginatorTypeDef
+            AwsElasticBeanstalkEnvironmentDetailsExtraOutputTypeDef
         ],
-        "AwsElasticsearchDomain": NotRequired[AwsElasticsearchDomainDetailsPaginatorTypeDef],
-        "AwsS3Bucket": NotRequired[AwsS3BucketDetailsPaginatorTypeDef],
+        "AwsElasticsearchDomain": NotRequired[AwsElasticsearchDomainDetailsExtraOutputTypeDef],
+        "AwsS3Bucket": NotRequired[AwsS3BucketDetailsExtraOutputTypeDef],
         "AwsS3AccountPublicAccessBlock": NotRequired[AwsS3AccountPublicAccessBlockDetailsTypeDef],
         "AwsS3Object": NotRequired[AwsS3ObjectDetailsTypeDef],
         "AwsSecretsManagerSecret": NotRequired[AwsSecretsManagerSecretDetailsTypeDef],
         "AwsIamAccessKey": NotRequired[AwsIamAccessKeyDetailsTypeDef],
-        "AwsIamUser": NotRequired[AwsIamUserDetailsPaginatorTypeDef],
-        "AwsIamPolicy": NotRequired[AwsIamPolicyDetailsPaginatorTypeDef],
-        "AwsApiGatewayV2Stage": NotRequired[AwsApiGatewayV2StageDetailsPaginatorTypeDef],
-        "AwsApiGatewayV2Api": NotRequired[AwsApiGatewayV2ApiDetailsPaginatorTypeDef],
-        "AwsDynamoDbTable": NotRequired[AwsDynamoDbTableDetailsPaginatorTypeDef],
-        "AwsApiGatewayStage": NotRequired[AwsApiGatewayStageDetailsPaginatorTypeDef],
-        "AwsApiGatewayRestApi": NotRequired[AwsApiGatewayRestApiDetailsPaginatorTypeDef],
+        "AwsIamUser": NotRequired[AwsIamUserDetailsExtraOutputTypeDef],
+        "AwsIamPolicy": NotRequired[AwsIamPolicyDetailsExtraOutputTypeDef],
+        "AwsApiGatewayV2Stage": NotRequired[AwsApiGatewayV2StageDetailsExtraOutputTypeDef],
+        "AwsApiGatewayV2Api": NotRequired[AwsApiGatewayV2ApiDetailsExtraOutputTypeDef],
+        "AwsDynamoDbTable": NotRequired[AwsDynamoDbTableDetailsExtraOutputTypeDef],
+        "AwsApiGatewayStage": NotRequired[AwsApiGatewayStageDetailsExtraOutputTypeDef],
+        "AwsApiGatewayRestApi": NotRequired[AwsApiGatewayRestApiDetailsExtraOutputTypeDef],
         "AwsCloudTrailTrail": NotRequired[AwsCloudTrailTrailDetailsTypeDef],
         "AwsSsmPatchCompliance": NotRequired[AwsSsmPatchComplianceDetailsTypeDef],
         "AwsCertificateManagerCertificate": NotRequired[
-            AwsCertificateManagerCertificateDetailsPaginatorTypeDef
+            AwsCertificateManagerCertificateDetailsExtraOutputTypeDef
         ],
-        "AwsRedshiftCluster": NotRequired[AwsRedshiftClusterDetailsPaginatorTypeDef],
-        "AwsElbLoadBalancer": NotRequired[AwsElbLoadBalancerDetailsPaginatorTypeDef],
-        "AwsIamGroup": NotRequired[AwsIamGroupDetailsPaginatorTypeDef],
-        "AwsIamRole": NotRequired[AwsIamRoleDetailsPaginatorTypeDef],
+        "AwsRedshiftCluster": NotRequired[AwsRedshiftClusterDetailsExtraOutputTypeDef],
+        "AwsElbLoadBalancer": NotRequired[AwsElbLoadBalancerDetailsExtraOutputTypeDef],
+        "AwsIamGroup": NotRequired[AwsIamGroupDetailsExtraOutputTypeDef],
+        "AwsIamRole": NotRequired[AwsIamRoleDetailsExtraOutputTypeDef],
         "AwsKmsKey": NotRequired[AwsKmsKeyDetailsTypeDef],
-        "AwsLambdaFunction": NotRequired[AwsLambdaFunctionDetailsPaginatorTypeDef],
-        "AwsLambdaLayerVersion": NotRequired[AwsLambdaLayerVersionDetailsPaginatorTypeDef],
-        "AwsRdsDbInstance": NotRequired[AwsRdsDbInstanceDetailsPaginatorTypeDef],
-        "AwsSnsTopic": NotRequired[AwsSnsTopicDetailsPaginatorTypeDef],
+        "AwsLambdaFunction": NotRequired[AwsLambdaFunctionDetailsExtraOutputTypeDef],
+        "AwsLambdaLayerVersion": NotRequired[AwsLambdaLayerVersionDetailsExtraOutputTypeDef],
+        "AwsRdsDbInstance": NotRequired[AwsRdsDbInstanceDetailsExtraOutputTypeDef],
+        "AwsSnsTopic": NotRequired[AwsSnsTopicDetailsExtraOutputTypeDef],
         "AwsSqsQueue": NotRequired[AwsSqsQueueDetailsTypeDef],
-        "AwsWafWebAcl": NotRequired[AwsWafWebAclDetailsPaginatorTypeDef],
-        "AwsRdsDbSnapshot": NotRequired[AwsRdsDbSnapshotDetailsPaginatorTypeDef],
-        "AwsRdsDbClusterSnapshot": NotRequired[AwsRdsDbClusterSnapshotDetailsPaginatorTypeDef],
-        "AwsRdsDbCluster": NotRequired[AwsRdsDbClusterDetailsPaginatorTypeDef],
-        "AwsEcsCluster": NotRequired[AwsEcsClusterDetailsPaginatorTypeDef],
-        "AwsEcsContainer": NotRequired[AwsEcsContainerDetailsPaginatorTypeDef],
-        "AwsEcsTaskDefinition": NotRequired[AwsEcsTaskDefinitionDetailsPaginatorTypeDef],
-        "Container": NotRequired[ContainerDetailsPaginatorTypeDef],
+        "AwsWafWebAcl": NotRequired[AwsWafWebAclDetailsExtraOutputTypeDef],
+        "AwsRdsDbSnapshot": NotRequired[AwsRdsDbSnapshotDetailsExtraOutputTypeDef],
+        "AwsRdsDbClusterSnapshot": NotRequired[AwsRdsDbClusterSnapshotDetailsExtraOutputTypeDef],
+        "AwsRdsDbCluster": NotRequired[AwsRdsDbClusterDetailsExtraOutputTypeDef],
+        "AwsEcsCluster": NotRequired[AwsEcsClusterDetailsExtraOutputTypeDef],
+        "AwsEcsContainer": NotRequired[AwsEcsContainerDetailsExtraOutputTypeDef],
+        "AwsEcsTaskDefinition": NotRequired[AwsEcsTaskDefinitionDetailsExtraOutputTypeDef],
+        "Container": NotRequired[ContainerDetailsExtraOutputTypeDef],
         "Other": NotRequired[Dict[str, str]],
-        "AwsRdsEventSubscription": NotRequired[AwsRdsEventSubscriptionDetailsPaginatorTypeDef],
-        "AwsEcsService": NotRequired[AwsEcsServiceDetailsPaginatorTypeDef],
+        "AwsRdsEventSubscription": NotRequired[AwsRdsEventSubscriptionDetailsExtraOutputTypeDef],
+        "AwsEcsService": NotRequired[AwsEcsServiceDetailsExtraOutputTypeDef],
         "AwsAutoScalingLaunchConfiguration": NotRequired[
-            AwsAutoScalingLaunchConfigurationDetailsPaginatorTypeDef
+            AwsAutoScalingLaunchConfigurationDetailsExtraOutputTypeDef
         ],
-        "AwsEc2VpnConnection": NotRequired[AwsEc2VpnConnectionDetailsPaginatorTypeDef],
-        "AwsEcrContainerImage": NotRequired[AwsEcrContainerImageDetailsPaginatorTypeDef],
+        "AwsEc2VpnConnection": NotRequired[AwsEc2VpnConnectionDetailsExtraOutputTypeDef],
+        "AwsEcrContainerImage": NotRequired[AwsEcrContainerImageDetailsExtraOutputTypeDef],
         "AwsOpenSearchServiceDomain": NotRequired[
-            AwsOpenSearchServiceDomainDetailsPaginatorTypeDef
+            AwsOpenSearchServiceDomainDetailsExtraOutputTypeDef
         ],
-        "AwsEc2VpcEndpointService": NotRequired[AwsEc2VpcEndpointServiceDetailsPaginatorTypeDef],
+        "AwsEc2VpcEndpointService": NotRequired[AwsEc2VpcEndpointServiceDetailsExtraOutputTypeDef],
         "AwsXrayEncryptionConfig": NotRequired[AwsXrayEncryptionConfigDetailsTypeDef],
-        "AwsWafRateBasedRule": NotRequired[AwsWafRateBasedRuleDetailsPaginatorTypeDef],
+        "AwsWafRateBasedRule": NotRequired[AwsWafRateBasedRuleDetailsExtraOutputTypeDef],
         "AwsWafRegionalRateBasedRule": NotRequired[
-            AwsWafRegionalRateBasedRuleDetailsPaginatorTypeDef
+            AwsWafRegionalRateBasedRuleDetailsExtraOutputTypeDef
         ],
         "AwsEcrRepository": NotRequired[AwsEcrRepositoryDetailsTypeDef],
-        "AwsEksCluster": NotRequired[AwsEksClusterDetailsPaginatorTypeDef],
+        "AwsEksCluster": NotRequired[AwsEksClusterDetailsExtraOutputTypeDef],
         "AwsNetworkFirewallFirewallPolicy": NotRequired[
-            AwsNetworkFirewallFirewallPolicyDetailsPaginatorTypeDef
+            AwsNetworkFirewallFirewallPolicyDetailsExtraOutputTypeDef
         ],
         "AwsNetworkFirewallFirewall": NotRequired[
-            AwsNetworkFirewallFirewallDetailsPaginatorTypeDef
+            AwsNetworkFirewallFirewallDetailsExtraOutputTypeDef
         ],
         "AwsNetworkFirewallRuleGroup": NotRequired[
-            AwsNetworkFirewallRuleGroupDetailsPaginatorTypeDef
+            AwsNetworkFirewallRuleGroupDetailsExtraOutputTypeDef
         ],
-        "AwsRdsDbSecurityGroup": NotRequired[AwsRdsDbSecurityGroupDetailsPaginatorTypeDef],
+        "AwsRdsDbSecurityGroup": NotRequired[AwsRdsDbSecurityGroupDetailsExtraOutputTypeDef],
         "AwsKinesisStream": NotRequired[AwsKinesisStreamDetailsTypeDef],
-        "AwsEc2TransitGateway": NotRequired[AwsEc2TransitGatewayDetailsPaginatorTypeDef],
-        "AwsEfsAccessPoint": NotRequired[AwsEfsAccessPointDetailsPaginatorTypeDef],
-        "AwsCloudFormationStack": NotRequired[AwsCloudFormationStackDetailsPaginatorTypeDef],
-        "AwsCloudWatchAlarm": NotRequired[AwsCloudWatchAlarmDetailsPaginatorTypeDef],
+        "AwsEc2TransitGateway": NotRequired[AwsEc2TransitGatewayDetailsExtraOutputTypeDef],
+        "AwsEfsAccessPoint": NotRequired[AwsEfsAccessPointDetailsExtraOutputTypeDef],
+        "AwsCloudFormationStack": NotRequired[AwsCloudFormationStackDetailsExtraOutputTypeDef],
+        "AwsCloudWatchAlarm": NotRequired[AwsCloudWatchAlarmDetailsExtraOutputTypeDef],
         "AwsEc2VpcPeeringConnection": NotRequired[
-            AwsEc2VpcPeeringConnectionDetailsPaginatorTypeDef
+            AwsEc2VpcPeeringConnectionDetailsExtraOutputTypeDef
         ],
-        "AwsWafRegionalRuleGroup": NotRequired[AwsWafRegionalRuleGroupDetailsPaginatorTypeDef],
-        "AwsWafRegionalRule": NotRequired[AwsWafRegionalRuleDetailsPaginatorTypeDef],
-        "AwsWafRegionalWebAcl": NotRequired[AwsWafRegionalWebAclDetailsPaginatorTypeDef],
-        "AwsWafRule": NotRequired[AwsWafRuleDetailsPaginatorTypeDef],
-        "AwsWafRuleGroup": NotRequired[AwsWafRuleGroupDetailsPaginatorTypeDef],
-        "AwsEcsTask": NotRequired[AwsEcsTaskDetailsPaginatorTypeDef],
-        "AwsBackupBackupVault": NotRequired[AwsBackupBackupVaultDetailsPaginatorTypeDef],
-        "AwsBackupBackupPlan": NotRequired[AwsBackupBackupPlanDetailsPaginatorTypeDef],
+        "AwsWafRegionalRuleGroup": NotRequired[AwsWafRegionalRuleGroupDetailsExtraOutputTypeDef],
+        "AwsWafRegionalRule": NotRequired[AwsWafRegionalRuleDetailsExtraOutputTypeDef],
+        "AwsWafRegionalWebAcl": NotRequired[AwsWafRegionalWebAclDetailsExtraOutputTypeDef],
+        "AwsWafRule": NotRequired[AwsWafRuleDetailsExtraOutputTypeDef],
+        "AwsWafRuleGroup": NotRequired[AwsWafRuleGroupDetailsExtraOutputTypeDef],
+        "AwsEcsTask": NotRequired[AwsEcsTaskDetailsExtraOutputTypeDef],
+        "AwsBackupBackupVault": NotRequired[AwsBackupBackupVaultDetailsExtraOutputTypeDef],
+        "AwsBackupBackupPlan": NotRequired[AwsBackupBackupPlanDetailsExtraOutputTypeDef],
         "AwsBackupRecoveryPoint": NotRequired[AwsBackupRecoveryPointDetailsTypeDef],
-        "AwsEc2LaunchTemplate": NotRequired[AwsEc2LaunchTemplateDetailsPaginatorTypeDef],
+        "AwsEc2LaunchTemplate": NotRequired[AwsEc2LaunchTemplateDetailsExtraOutputTypeDef],
         "AwsSageMakerNotebookInstance": NotRequired[
-            AwsSageMakerNotebookInstanceDetailsPaginatorTypeDef
+            AwsSageMakerNotebookInstanceDetailsExtraOutputTypeDef
         ],
-        "AwsWafv2WebAcl": NotRequired[AwsWafv2WebAclDetailsPaginatorTypeDef],
-        "AwsWafv2RuleGroup": NotRequired[AwsWafv2RuleGroupDetailsPaginatorTypeDef],
-        "AwsEc2RouteTable": NotRequired[AwsEc2RouteTableDetailsPaginatorTypeDef],
-        "AwsAmazonMqBroker": NotRequired[AwsAmazonMqBrokerDetailsPaginatorTypeDef],
-        "AwsAppSyncGraphQlApi": NotRequired[AwsAppSyncGraphQlApiDetailsPaginatorTypeDef],
+        "AwsWafv2WebAcl": NotRequired[AwsWafv2WebAclDetailsExtraOutputTypeDef],
+        "AwsWafv2RuleGroup": NotRequired[AwsWafv2RuleGroupDetailsExtraOutputTypeDef],
+        "AwsEc2RouteTable": NotRequired[AwsEc2RouteTableDetailsExtraOutputTypeDef],
+        "AwsAmazonMqBroker": NotRequired[AwsAmazonMqBrokerDetailsExtraOutputTypeDef],
+        "AwsAppSyncGraphQlApi": NotRequired[AwsAppSyncGraphQlApiDetailsExtraOutputTypeDef],
         "AwsEventSchemasRegistry": NotRequired[AwsEventSchemasRegistryDetailsTypeDef],
-        "AwsGuardDutyDetector": NotRequired[AwsGuardDutyDetectorDetailsPaginatorTypeDef],
+        "AwsGuardDutyDetector": NotRequired[AwsGuardDutyDetectorDetailsExtraOutputTypeDef],
         "AwsStepFunctionStateMachine": NotRequired[
-            AwsStepFunctionStateMachineDetailsPaginatorTypeDef
+            AwsStepFunctionStateMachineDetailsExtraOutputTypeDef
         ],
         "AwsAthenaWorkGroup": NotRequired[AwsAthenaWorkGroupDetailsTypeDef],
         "AwsEventsEventbus": NotRequired[AwsEventsEventbusDetailsTypeDef],
         "AwsDmsEndpoint": NotRequired[AwsDmsEndpointDetailsTypeDef],
-        "AwsEventsEndpoint": NotRequired[AwsEventsEndpointDetailsPaginatorTypeDef],
+        "AwsEventsEndpoint": NotRequired[AwsEventsEndpointDetailsExtraOutputTypeDef],
         "AwsDmsReplicationTask": NotRequired[AwsDmsReplicationTaskDetailsTypeDef],
-        "AwsDmsReplicationInstance": NotRequired[AwsDmsReplicationInstanceDetailsPaginatorTypeDef],
-        "AwsRoute53HostedZone": NotRequired[AwsRoute53HostedZoneDetailsPaginatorTypeDef],
-        "AwsMskCluster": NotRequired[AwsMskClusterDetailsPaginatorTypeDef],
+        "AwsDmsReplicationInstance": NotRequired[
+            AwsDmsReplicationInstanceDetailsExtraOutputTypeDef
+        ],
+        "AwsRoute53HostedZone": NotRequired[AwsRoute53HostedZoneDetailsExtraOutputTypeDef],
+        "AwsMskCluster": NotRequired[AwsMskClusterDetailsExtraOutputTypeDef],
         "AwsS3AccessPoint": NotRequired[AwsS3AccessPointDetailsTypeDef],
-        "AwsEc2ClientVpnEndpoint": NotRequired[AwsEc2ClientVpnEndpointDetailsPaginatorTypeDef],
+        "AwsEc2ClientVpnEndpoint": NotRequired[AwsEc2ClientVpnEndpointDetailsExtraOutputTypeDef],
+    },
+)
+ResourceDetailsOutputTypeDef = TypedDict(
+    "ResourceDetailsOutputTypeDef",
+    {
+        "AwsAutoScalingAutoScalingGroup": NotRequired[
+            AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef
+        ],
+        "AwsCodeBuildProject": NotRequired[AwsCodeBuildProjectDetailsOutputTypeDef],
+        "AwsCloudFrontDistribution": NotRequired[AwsCloudFrontDistributionDetailsOutputTypeDef],
+        "AwsEc2Instance": NotRequired[AwsEc2InstanceDetailsOutputTypeDef],
+        "AwsEc2NetworkInterface": NotRequired[AwsEc2NetworkInterfaceDetailsOutputTypeDef],
+        "AwsEc2SecurityGroup": NotRequired[AwsEc2SecurityGroupDetailsOutputTypeDef],
+        "AwsEc2Volume": NotRequired[AwsEc2VolumeDetailsOutputTypeDef],
+        "AwsEc2Vpc": NotRequired[AwsEc2VpcDetailsOutputTypeDef],
+        "AwsEc2Eip": NotRequired[AwsEc2EipDetailsTypeDef],
+        "AwsEc2Subnet": NotRequired[AwsEc2SubnetDetailsOutputTypeDef],
+        "AwsEc2NetworkAcl": NotRequired[AwsEc2NetworkAclDetailsOutputTypeDef],
+        "AwsElbv2LoadBalancer": NotRequired[AwsElbv2LoadBalancerDetailsOutputTypeDef],
+        "AwsElasticBeanstalkEnvironment": NotRequired[
+            AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef
+        ],
+        "AwsElasticsearchDomain": NotRequired[AwsElasticsearchDomainDetailsOutputTypeDef],
+        "AwsS3Bucket": NotRequired[AwsS3BucketDetailsOutputTypeDef],
+        "AwsS3AccountPublicAccessBlock": NotRequired[AwsS3AccountPublicAccessBlockDetailsTypeDef],
+        "AwsS3Object": NotRequired[AwsS3ObjectDetailsTypeDef],
+        "AwsSecretsManagerSecret": NotRequired[AwsSecretsManagerSecretDetailsTypeDef],
+        "AwsIamAccessKey": NotRequired[AwsIamAccessKeyDetailsTypeDef],
+        "AwsIamUser": NotRequired[AwsIamUserDetailsOutputTypeDef],
+        "AwsIamPolicy": NotRequired[AwsIamPolicyDetailsOutputTypeDef],
+        "AwsApiGatewayV2Stage": NotRequired[AwsApiGatewayV2StageDetailsOutputTypeDef],
+        "AwsApiGatewayV2Api": NotRequired[AwsApiGatewayV2ApiDetailsOutputTypeDef],
+        "AwsDynamoDbTable": NotRequired[AwsDynamoDbTableDetailsOutputTypeDef],
+        "AwsApiGatewayStage": NotRequired[AwsApiGatewayStageDetailsOutputTypeDef],
+        "AwsApiGatewayRestApi": NotRequired[AwsApiGatewayRestApiDetailsOutputTypeDef],
+        "AwsCloudTrailTrail": NotRequired[AwsCloudTrailTrailDetailsTypeDef],
+        "AwsSsmPatchCompliance": NotRequired[AwsSsmPatchComplianceDetailsTypeDef],
+        "AwsCertificateManagerCertificate": NotRequired[
+            AwsCertificateManagerCertificateDetailsOutputTypeDef
+        ],
+        "AwsRedshiftCluster": NotRequired[AwsRedshiftClusterDetailsOutputTypeDef],
+        "AwsElbLoadBalancer": NotRequired[AwsElbLoadBalancerDetailsOutputTypeDef],
+        "AwsIamGroup": NotRequired[AwsIamGroupDetailsOutputTypeDef],
+        "AwsIamRole": NotRequired[AwsIamRoleDetailsOutputTypeDef],
+        "AwsKmsKey": NotRequired[AwsKmsKeyDetailsTypeDef],
+        "AwsLambdaFunction": NotRequired[AwsLambdaFunctionDetailsOutputTypeDef],
+        "AwsLambdaLayerVersion": NotRequired[AwsLambdaLayerVersionDetailsOutputTypeDef],
+        "AwsRdsDbInstance": NotRequired[AwsRdsDbInstanceDetailsOutputTypeDef],
+        "AwsSnsTopic": NotRequired[AwsSnsTopicDetailsOutputTypeDef],
+        "AwsSqsQueue": NotRequired[AwsSqsQueueDetailsTypeDef],
+        "AwsWafWebAcl": NotRequired[AwsWafWebAclDetailsOutputTypeDef],
+        "AwsRdsDbSnapshot": NotRequired[AwsRdsDbSnapshotDetailsOutputTypeDef],
+        "AwsRdsDbClusterSnapshot": NotRequired[AwsRdsDbClusterSnapshotDetailsOutputTypeDef],
+        "AwsRdsDbCluster": NotRequired[AwsRdsDbClusterDetailsOutputTypeDef],
+        "AwsEcsCluster": NotRequired[AwsEcsClusterDetailsOutputTypeDef],
+        "AwsEcsContainer": NotRequired[AwsEcsContainerDetailsOutputTypeDef],
+        "AwsEcsTaskDefinition": NotRequired[AwsEcsTaskDefinitionDetailsOutputTypeDef],
+        "Container": NotRequired[ContainerDetailsOutputTypeDef],
+        "Other": NotRequired[Dict[str, str]],
+        "AwsRdsEventSubscription": NotRequired[AwsRdsEventSubscriptionDetailsOutputTypeDef],
+        "AwsEcsService": NotRequired[AwsEcsServiceDetailsOutputTypeDef],
+        "AwsAutoScalingLaunchConfiguration": NotRequired[
+            AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef
+        ],
+        "AwsEc2VpnConnection": NotRequired[AwsEc2VpnConnectionDetailsOutputTypeDef],
+        "AwsEcrContainerImage": NotRequired[AwsEcrContainerImageDetailsOutputTypeDef],
+        "AwsOpenSearchServiceDomain": NotRequired[AwsOpenSearchServiceDomainDetailsOutputTypeDef],
+        "AwsEc2VpcEndpointService": NotRequired[AwsEc2VpcEndpointServiceDetailsOutputTypeDef],
+        "AwsXrayEncryptionConfig": NotRequired[AwsXrayEncryptionConfigDetailsTypeDef],
+        "AwsWafRateBasedRule": NotRequired[AwsWafRateBasedRuleDetailsOutputTypeDef],
+        "AwsWafRegionalRateBasedRule": NotRequired[AwsWafRegionalRateBasedRuleDetailsOutputTypeDef],
+        "AwsEcrRepository": NotRequired[AwsEcrRepositoryDetailsTypeDef],
+        "AwsEksCluster": NotRequired[AwsEksClusterDetailsOutputTypeDef],
+        "AwsNetworkFirewallFirewallPolicy": NotRequired[
+            AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef
+        ],
+        "AwsNetworkFirewallFirewall": NotRequired[AwsNetworkFirewallFirewallDetailsOutputTypeDef],
+        "AwsNetworkFirewallRuleGroup": NotRequired[AwsNetworkFirewallRuleGroupDetailsOutputTypeDef],
+        "AwsRdsDbSecurityGroup": NotRequired[AwsRdsDbSecurityGroupDetailsOutputTypeDef],
+        "AwsKinesisStream": NotRequired[AwsKinesisStreamDetailsTypeDef],
+        "AwsEc2TransitGateway": NotRequired[AwsEc2TransitGatewayDetailsOutputTypeDef],
+        "AwsEfsAccessPoint": NotRequired[AwsEfsAccessPointDetailsOutputTypeDef],
+        "AwsCloudFormationStack": NotRequired[AwsCloudFormationStackDetailsOutputTypeDef],
+        "AwsCloudWatchAlarm": NotRequired[AwsCloudWatchAlarmDetailsOutputTypeDef],
+        "AwsEc2VpcPeeringConnection": NotRequired[AwsEc2VpcPeeringConnectionDetailsOutputTypeDef],
+        "AwsWafRegionalRuleGroup": NotRequired[AwsWafRegionalRuleGroupDetailsOutputTypeDef],
+        "AwsWafRegionalRule": NotRequired[AwsWafRegionalRuleDetailsOutputTypeDef],
+        "AwsWafRegionalWebAcl": NotRequired[AwsWafRegionalWebAclDetailsOutputTypeDef],
+        "AwsWafRule": NotRequired[AwsWafRuleDetailsOutputTypeDef],
+        "AwsWafRuleGroup": NotRequired[AwsWafRuleGroupDetailsOutputTypeDef],
+        "AwsEcsTask": NotRequired[AwsEcsTaskDetailsOutputTypeDef],
+        "AwsBackupBackupVault": NotRequired[AwsBackupBackupVaultDetailsOutputTypeDef],
+        "AwsBackupBackupPlan": NotRequired[AwsBackupBackupPlanDetailsOutputTypeDef],
+        "AwsBackupRecoveryPoint": NotRequired[AwsBackupRecoveryPointDetailsTypeDef],
+        "AwsEc2LaunchTemplate": NotRequired[AwsEc2LaunchTemplateDetailsOutputTypeDef],
+        "AwsSageMakerNotebookInstance": NotRequired[
+            AwsSageMakerNotebookInstanceDetailsOutputTypeDef
+        ],
+        "AwsWafv2WebAcl": NotRequired[AwsWafv2WebAclDetailsOutputTypeDef],
+        "AwsWafv2RuleGroup": NotRequired[AwsWafv2RuleGroupDetailsOutputTypeDef],
+        "AwsEc2RouteTable": NotRequired[AwsEc2RouteTableDetailsOutputTypeDef],
+        "AwsAmazonMqBroker": NotRequired[AwsAmazonMqBrokerDetailsOutputTypeDef],
+        "AwsAppSyncGraphQlApi": NotRequired[AwsAppSyncGraphQlApiDetailsOutputTypeDef],
+        "AwsEventSchemasRegistry": NotRequired[AwsEventSchemasRegistryDetailsTypeDef],
+        "AwsGuardDutyDetector": NotRequired[AwsGuardDutyDetectorDetailsOutputTypeDef],
+        "AwsStepFunctionStateMachine": NotRequired[AwsStepFunctionStateMachineDetailsOutputTypeDef],
+        "AwsAthenaWorkGroup": NotRequired[AwsAthenaWorkGroupDetailsTypeDef],
+        "AwsEventsEventbus": NotRequired[AwsEventsEventbusDetailsTypeDef],
+        "AwsDmsEndpoint": NotRequired[AwsDmsEndpointDetailsTypeDef],
+        "AwsEventsEndpoint": NotRequired[AwsEventsEndpointDetailsOutputTypeDef],
+        "AwsDmsReplicationTask": NotRequired[AwsDmsReplicationTaskDetailsTypeDef],
+        "AwsDmsReplicationInstance": NotRequired[AwsDmsReplicationInstanceDetailsOutputTypeDef],
+        "AwsRoute53HostedZone": NotRequired[AwsRoute53HostedZoneDetailsOutputTypeDef],
+        "AwsMskCluster": NotRequired[AwsMskClusterDetailsOutputTypeDef],
+        "AwsS3AccessPoint": NotRequired[AwsS3AccessPointDetailsTypeDef],
+        "AwsEc2ClientVpnEndpoint": NotRequired[AwsEc2ClientVpnEndpointDetailsOutputTypeDef],
     },
 )
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "AwsAutoScalingAutoScalingGroup": NotRequired[AwsAutoScalingAutoScalingGroupDetailsTypeDef],
         "AwsCodeBuildProject": NotRequired[AwsCodeBuildProjectDetailsTypeDef],
@@ -11928,25 +15403,40 @@
         "AwsDmsReplicationInstance": NotRequired[AwsDmsReplicationInstanceDetailsTypeDef],
         "AwsRoute53HostedZone": NotRequired[AwsRoute53HostedZoneDetailsTypeDef],
         "AwsMskCluster": NotRequired[AwsMskClusterDetailsTypeDef],
         "AwsS3AccessPoint": NotRequired[AwsS3AccessPointDetailsTypeDef],
         "AwsEc2ClientVpnEndpoint": NotRequired[AwsEc2ClientVpnEndpointDetailsTypeDef],
     },
 )
-ResourcePaginatorTypeDef = TypedDict(
-    "ResourcePaginatorTypeDef",
+ResourceExtraOutputTypeDef = TypedDict(
+    "ResourceExtraOutputTypeDef",
     {
         "Type": str,
         "Id": str,
         "Partition": NotRequired[PartitionType],
         "Region": NotRequired[str],
         "ResourceRole": NotRequired[str],
         "Tags": NotRequired[Dict[str, str]],
-        "DataClassification": NotRequired[DataClassificationDetailsPaginatorTypeDef],
-        "Details": NotRequired[ResourceDetailsPaginatorTypeDef],
+        "DataClassification": NotRequired[DataClassificationDetailsExtraOutputTypeDef],
+        "Details": NotRequired[ResourceDetailsExtraOutputTypeDef],
+        "ApplicationName": NotRequired[str],
+        "ApplicationArn": NotRequired[str],
+    },
+)
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
+    {
+        "Type": str,
+        "Id": str,
+        "Partition": NotRequired[PartitionType],
+        "Region": NotRequired[str],
+        "ResourceRole": NotRequired[str],
+        "Tags": NotRequired[Dict[str, str]],
+        "DataClassification": NotRequired[DataClassificationDetailsOutputTypeDef],
+        "Details": NotRequired[ResourceDetailsOutputTypeDef],
         "ApplicationName": NotRequired[str],
         "ApplicationArn": NotRequired[str],
     },
 )
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
@@ -11958,27 +15448,76 @@
         "Tags": NotRequired[Mapping[str, str]],
         "DataClassification": NotRequired[DataClassificationDetailsTypeDef],
         "Details": NotRequired[ResourceDetailsTypeDef],
         "ApplicationName": NotRequired[str],
         "ApplicationArn": NotRequired[str],
     },
 )
-AwsSecurityFindingPaginatorTypeDef = TypedDict(
-    "AwsSecurityFindingPaginatorTypeDef",
+AwsSecurityFindingExtraOutputTypeDef = TypedDict(
+    "AwsSecurityFindingExtraOutputTypeDef",
+    {
+        "SchemaVersion": str,
+        "Id": str,
+        "ProductArn": str,
+        "GeneratorId": str,
+        "AwsAccountId": str,
+        "CreatedAt": str,
+        "UpdatedAt": str,
+        "Title": str,
+        "Description": str,
+        "Resources": List[ResourceExtraOutputTypeDef],
+        "ProductName": NotRequired[str],
+        "CompanyName": NotRequired[str],
+        "Region": NotRequired[str],
+        "Types": NotRequired[List[str]],
+        "FirstObservedAt": NotRequired[str],
+        "LastObservedAt": NotRequired[str],
+        "Severity": NotRequired[SeverityTypeDef],
+        "Confidence": NotRequired[int],
+        "Criticality": NotRequired[int],
+        "Remediation": NotRequired[RemediationTypeDef],
+        "SourceUrl": NotRequired[str],
+        "ProductFields": NotRequired[Dict[str, str]],
+        "UserDefinedFields": NotRequired[Dict[str, str]],
+        "Malware": NotRequired[List[MalwareTypeDef]],
+        "Network": NotRequired[NetworkTypeDef],
+        "NetworkPath": NotRequired[List[NetworkPathComponentExtraOutputTypeDef]],
+        "Process": NotRequired[ProcessDetailsTypeDef],
+        "Threats": NotRequired[List[ThreatExtraOutputTypeDef]],
+        "ThreatIntelIndicators": NotRequired[List[ThreatIntelIndicatorTypeDef]],
+        "Compliance": NotRequired[ComplianceExtraOutputTypeDef],
+        "VerificationState": NotRequired[VerificationStateType],
+        "WorkflowState": NotRequired[WorkflowStateType],
+        "Workflow": NotRequired[WorkflowTypeDef],
+        "RecordState": NotRequired[RecordStateType],
+        "RelatedFindings": NotRequired[List[RelatedFindingTypeDef]],
+        "Note": NotRequired[NoteTypeDef],
+        "Vulnerabilities": NotRequired[List[VulnerabilityExtraOutputTypeDef]],
+        "PatchSummary": NotRequired[PatchSummaryTypeDef],
+        "Action": NotRequired[ActionExtraOutputTypeDef],
+        "FindingProviderFields": NotRequired[FindingProviderFieldsExtraOutputTypeDef],
+        "Sample": NotRequired[bool],
+        "GeneratorDetails": NotRequired[GeneratorDetailsExtraOutputTypeDef],
+        "ProcessedAt": NotRequired[str],
+        "AwsAccountName": NotRequired[str],
+    },
+)
+AwsSecurityFindingOutputTypeDef = TypedDict(
+    "AwsSecurityFindingOutputTypeDef",
     {
         "SchemaVersion": str,
         "Id": str,
         "ProductArn": str,
         "GeneratorId": str,
         "AwsAccountId": str,
         "CreatedAt": str,
         "UpdatedAt": str,
         "Title": str,
         "Description": str,
-        "Resources": List[ResourcePaginatorTypeDef],
+        "Resources": List[ResourceOutputTypeDef],
         "ProductName": NotRequired[str],
         "CompanyName": NotRequired[str],
         "Region": NotRequired[str],
         "Types": NotRequired[List[str]],
         "FirstObservedAt": NotRequired[str],
         "LastObservedAt": NotRequired[str],
         "Severity": NotRequired[SeverityTypeDef],
@@ -11986,31 +15525,31 @@
         "Criticality": NotRequired[int],
         "Remediation": NotRequired[RemediationTypeDef],
         "SourceUrl": NotRequired[str],
         "ProductFields": NotRequired[Dict[str, str]],
         "UserDefinedFields": NotRequired[Dict[str, str]],
         "Malware": NotRequired[List[MalwareTypeDef]],
         "Network": NotRequired[NetworkTypeDef],
-        "NetworkPath": NotRequired[List[NetworkPathComponentPaginatorTypeDef]],
+        "NetworkPath": NotRequired[List[NetworkPathComponentOutputTypeDef]],
         "Process": NotRequired[ProcessDetailsTypeDef],
-        "Threats": NotRequired[List[ThreatPaginatorTypeDef]],
+        "Threats": NotRequired[List[ThreatOutputTypeDef]],
         "ThreatIntelIndicators": NotRequired[List[ThreatIntelIndicatorTypeDef]],
-        "Compliance": NotRequired[CompliancePaginatorTypeDef],
+        "Compliance": NotRequired[ComplianceOutputTypeDef],
         "VerificationState": NotRequired[VerificationStateType],
         "WorkflowState": NotRequired[WorkflowStateType],
         "Workflow": NotRequired[WorkflowTypeDef],
         "RecordState": NotRequired[RecordStateType],
         "RelatedFindings": NotRequired[List[RelatedFindingTypeDef]],
         "Note": NotRequired[NoteTypeDef],
-        "Vulnerabilities": NotRequired[List[VulnerabilityPaginatorTypeDef]],
+        "Vulnerabilities": NotRequired[List[VulnerabilityOutputTypeDef]],
         "PatchSummary": NotRequired[PatchSummaryTypeDef],
-        "Action": NotRequired[ActionPaginatorTypeDef],
-        "FindingProviderFields": NotRequired[FindingProviderFieldsPaginatorTypeDef],
+        "Action": NotRequired[ActionOutputTypeDef],
+        "FindingProviderFields": NotRequired[FindingProviderFieldsOutputTypeDef],
         "Sample": NotRequired[bool],
-        "GeneratorDetails": NotRequired[GeneratorDetailsPaginatorTypeDef],
+        "GeneratorDetails": NotRequired[GeneratorDetailsOutputTypeDef],
         "ProcessedAt": NotRequired[str],
         "AwsAccountName": NotRequired[str],
     },
 )
 AwsSecurityFindingTypeDef = TypedDict(
     "AwsSecurityFindingTypeDef",
     {
@@ -12056,29 +15595,24 @@
         "FindingProviderFields": NotRequired[FindingProviderFieldsTypeDef],
         "Sample": NotRequired[bool],
         "GeneratorDetails": NotRequired[GeneratorDetailsTypeDef],
         "ProcessedAt": NotRequired[str],
         "AwsAccountName": NotRequired[str],
     },
 )
-GetFindingsResponsePaginatorTypeDef = TypedDict(
-    "GetFindingsResponsePaginatorTypeDef",
+GetFindingsResponseTypeDef = TypedDict(
+    "GetFindingsResponseTypeDef",
     {
-        "Findings": List[AwsSecurityFindingPaginatorTypeDef],
-        "NextToken": str,
+        "Findings": List[AwsSecurityFindingOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
+AwsSecurityFindingUnionTypeDef = Union[
+    AwsSecurityFindingTypeDef, AwsSecurityFindingExtraOutputTypeDef
+]
 BatchImportFindingsRequestRequestTypeDef = TypedDict(
     "BatchImportFindingsRequestRequestTypeDef",
     {
-        "Findings": Sequence[AwsSecurityFindingTypeDef],
-    },
-)
-GetFindingsResponseTypeDef = TypedDict(
-    "GetFindingsResponseTypeDef",
-    {
-        "Findings": List[AwsSecurityFindingTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Findings": Sequence[AwsSecurityFindingUnionTypeDef],
     },
 )
```

### Comparing `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/PKG-INFO` & `mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securityhub
-Version: 1.34.76
-Summary: Type annotations for boto3.SecurityHub 1.34.76 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.96
+Summary: Type annotations for boto3.SecurityHub 1.34.96 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securityhub)](https://pepy.tech/project/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.34.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/SOURCES.txt` & `mypy_boto3_securityhub-1.34.96/mypy_boto3_securityhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.34.76/setup.py` & `mypy_boto3_securityhub-1.34.96/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-securityhub",
-    version="1.34.76",
+    version="1.34.96",
     packages=["mypy_boto3_securityhub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.SecurityHub 1.34.76 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.SecurityHub 1.34.96 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

