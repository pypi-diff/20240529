# Comparing `tmp/fortiedr-3.6.7.tar.gz` & `tmp/fortiedr-3.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortiedr-3.6.7.tar", last modified: Thu May 23 13:55:54 2024, max compression
+gzip compressed data, was "fortiedr-3.6.8.tar", last modified: Wed May 29 00:16:10 2024, max compression
```

## Comparing `fortiedr-3.6.7.tar` & `fortiedr-3.6.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:55:54.159842 fortiedr-3.6.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 13:55:49.000000 fortiedr-3.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-23 13:55:49.000000 fortiedr-3.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-23 13:55:54.159842 fortiedr-3.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-23 13:55:49.000000 fortiedr-3.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:55:54.155842 fortiedr-3.6.7/fortiedr/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-23 13:55:49.000000 fortiedr-3.6.7/fortiedr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21615 2024-05-23 13:55:49.000000 fortiedr-3.6.7/fortiedr/api_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-23 13:55:49.000000 fortiedr-3.6.7/fortiedr/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-23 13:55:49.000000 fortiedr-3.6.7/fortiedr/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)   238976 2024-05-23 13:55:49.000000 fortiedr-3.6.7/fortiedr/fortiedr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:55:54.159842 fortiedr-3.6.7/fortiedr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-23 13:55:54.000000 fortiedr-3.6.7/fortiedr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-23 13:55:54.000000 fortiedr-3.6.7/fortiedr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:55:54.000000 fortiedr-3.6.7/fortiedr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 13:55:54.000000 fortiedr-3.6.7/fortiedr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-23 13:55:49.000000 fortiedr-3.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-23 13:55:49.000000 fortiedr-3.6.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:55:54.159842 fortiedr-3.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-23 13:55:49.000000 fortiedr-3.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:16:10.306486 fortiedr-3.6.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-29 00:16:06.000000 fortiedr-3.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 00:16:06.000000 fortiedr-3.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-29 00:16:10.306486 fortiedr-3.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-29 00:16:06.000000 fortiedr-3.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:16:10.306486 fortiedr-3.6.8/fortiedr/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-29 00:16:06.000000 fortiedr-3.6.8/fortiedr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21615 2024-05-29 00:16:06.000000 fortiedr-3.6.8/fortiedr/api_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-29 00:16:06.000000 fortiedr-3.6.8/fortiedr/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-29 00:16:06.000000 fortiedr-3.6.8/fortiedr/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)   252923 2024-05-29 00:16:06.000000 fortiedr-3.6.8/fortiedr/fortiedr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:16:10.306486 fortiedr-3.6.8/fortiedr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-29 00:16:10.000000 fortiedr-3.6.8/fortiedr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 00:16:10.000000 fortiedr-3.6.8/fortiedr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 00:16:10.000000 fortiedr-3.6.8/fortiedr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 00:16:10.000000 fortiedr-3.6.8/fortiedr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-29 00:16:06.000000 fortiedr-3.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-29 00:16:06.000000 fortiedr-3.6.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 00:16:10.306486 fortiedr-3.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-29 00:16:06.000000 fortiedr-3.6.8/setup.py
```

### Comparing `fortiedr-3.6.7/LICENSE` & `fortiedr-3.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.7/PKG-INFO` & `fortiedr-3.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortiedr
-Version: 3.6.7
+Version: 3.6.8
 Summary: This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.
 Author: Rafael Foster
 Author-email: Rafael Foster <rafaelgfoster@gmail.com>
 Project-URL: Homepage, https://github.com/rafaelfoster/fortiedr
 Project-URL: Issues, https://github.com/rafaelfoster/fortiedr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortiedr-3.6.7/README.md` & `fortiedr-3.6.8/README.md`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.7/fortiedr/api_parameters.json` & `fortiedr-3.6.8/fortiedr/api_parameters.json`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.7/fortiedr/auth.py` & `fortiedr-3.6.8/fortiedr/auth.py`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.7/fortiedr/connector.py` & `fortiedr-3.6.8/fortiedr/connector.py`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.7/fortiedr/fortiedr.py` & `fortiedr-3.6.8/fortiedr/fortiedr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import os
 import json
 from typing import BinaryIO
 from fortiedr.auth import Auth as fedrAuth
 from fortiedr.connector import FortiEDR_API_GW
 
-version = '3.6.7'
+version = '3.6.8'
 
 fortiedr_connection = None
 
 class Admin:
 	'''Admin Rest Api Controller'''
 
 	def set_tray_notification_settings(self, enabledPopup: bool = None, enabledTrayNotification: bool = None, message: str = None, organization: str = None) -> tuple[bool, None]:
@@ -53,14 +53,15 @@
 			attributes.signer (str): Specifies the value, if contains special characters - encode to HTML URL Encoding.
 			currentPage (int): Specifies the current page.
 			enabled (bool): Specifies the state of the application control.
 			hash (str): Specifies the hash of the application control.
 			operatingSystem (str): Specifies the operating system of the application control.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			policyIds (list): Specifies the IDs of the relevant policies for application control.
+			integer (list): Specifies the IDs of the relevant policies for application control.
 			tag (str): Specifies the tag related to application control.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("get_applications", locals())
@@ -80,15 +81,15 @@
 		if hash:
 			url_params.append('hash=' + hash)
 		if operatingSystem:
 			url_params.append('operatingSystem=' + operatingSystem)
 		if organization:
 			url_params.append('organization=' + organization)
 		if policyIds:
-			url_params.append('policyIds=' + ",".join(str(policyIds)))
+			url_params.append('policyIds=' + ",".join(map(str, policyIds)))
 		if tag:
 			url_params.append('tag=' + tag)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
 	def send_applications(self, applicationControls: list = None, organization: str = None) -> tuple[bool, None]:
 		'''
@@ -115,27 +116,28 @@
 	def insert_applications(self, appIds: list, organization: str, enabled: bool = None, groupIds: list = None, isOverridePolicies: bool = None, policyIds: list = None, tagId: int = None) -> tuple[bool, list]:
 		'''
 		Class ApplicationControl
 		Description: Edits existing application control and returns the affected ones.
         
 		Args:
 			appIds (list): The relevant application IDs to edit.
+			integer (list): The relevant application IDs to edit.
 			modifiedFields (Object): Check 'modifiedFields' in the API documentation for further information.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("insert_applications", locals())
 
 		url = '/api/application-control/applications'
 		url_params = []
 		if appIds:
-			url_params.append('appIds=' + ",".join(str(appIds)))
+			url_params.append('appIds=' + ",".join(map(str, appIds)))
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 
 		modifiedFields = {
 			"enabled": enabled,
 			"groupIds": groupIds,
@@ -148,26 +150,27 @@
 	def delete_applications(self, organization: str, applicationIds: list = None) -> tuple[bool, None]:
 		'''
 		Class ApplicationControl
 		Description: Deletes application controls.
         
 		Args:
 			applicationIds (list): The IDs of the applications to be deleted.
+			integer (list): The IDs of the applications to be deleted.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("delete_applications", locals())
 
 		url = '/api/application-control/applications'
 		url_params = []
 		if applicationIds:
-			url_params.append('applicationIds=' + ",".join(str(applicationIds)))
+			url_params.append('applicationIds=' + ",".join(map(str, applicationIds)))
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
 	def force_update_ootb_application_controls(self) -> tuple[bool, None]:
 		'''
@@ -429,30 +432,32 @@
 	def update_collector_installer(self, collectorGroupIds: list = None, collectorGroups: list = None, organization: str = None, updateVersions: list = None) -> tuple[bool, None]:
 		'''
 		Class Administrator
 		Description: This API update collectors target version for collector groups.
         
 		Args:
 			collectorGroupIds (list): Specifies the list of IDs of all the collector groups which should be updated..
+			integer (list): Specifies the list of IDs of all the collector groups which should be updated..
 			collectorGroups (list): Specifies the list of all the collector groups which should be updated..
+			string (list): Specifies the list of all the collector groups which should be updated..
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			requestUpdateData (Object): Check 'requestUpdateData' in the API documentation for further information.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("update_collector_installer", locals())
 
 		url = '/management-rest/admin/update-collector-installer'
 		url_params = []
 		if collectorGroupIds:
-			url_params.append('collectorGroupIds=' + ",".join(str(collectorGroupIds)))
+			url_params.append('collectorGroupIds=' + ",".join(map(str, collectorGroupIds)))
 		if collectorGroups:
 			url_params.append('collectorGroups=' + ",".join(str(collectorGroups)))
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 
 		requestUpdateData = {
@@ -538,14 +543,15 @@
 	def assign_collector_group(self, collectorGroups: list, policyName: str, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class CommunicationControl
 		Description: Assign collector group to application policy.
         
 		Args:
 			collectorGroups (list):  Specifies the collector groups whose collector reported the events.
+			string (list):  Specifies the collector groups whose collector reported the events.
 			forceAssign (bool): Indicates whether to force the assignment even if the group is assigned to similar policies.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			policyName (str): Specifies the list of policies.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
@@ -595,21 +601,25 @@
 	def list_policies(self, decisions: list, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, policies: list = None, rules: list = None, sorting: str = None, sources: list = None, state: str = None, strictMode: bool = None) -> tuple[bool, list]:
 		'''
 		Class CommunicationControl
 		Description: This API call outputs a list of all the communication control policies in the system, and information about each of them.
         
 		Args:
 			decisions (list): Indicates the action.
+			string (list): Indicates the action.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			policies (list): Specifies the list of policy names.
+			string (list): Specifies the list of policy names.
 			rules (list): Specifies the list of rules.
+			string (list): Specifies the list of rules.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			sources (list): Specifies who created the policy.
+			string (list): Specifies who created the policy.
 			state (str): Policy rule state.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
@@ -644,44 +654,56 @@
 		'''
 		Class CommunicationControl
 		Description: This API call outputs a list of all the communicating applications in the system, and information about each of them.
         
 		Args:
 			action (str): Indicates the action: Allow/Deny. This parameter is irrelevant without policies parameter.
 			collectorGroups (list): Specifies the list of collector groups where the products were seen.
+			string (list): Specifies the list of collector groups where the products were seen.
 			cveIdentifier (str): Specifies the CVE identifier.
 			destinationIp (list): Destination IPs.
+			string (list): Destination IPs.
 			devices (list): Specifies the list of device names where the products were seen.
+			string (list): Specifies the list of device names where the products were seen.
 			firstConnectionTimeEnd (str):  Retrieves products whose first connection time is less than the value assigned to this date.
 			firstConnectionTimeStart (str):  Retrieves products whose first connection time is greater than the value assigned to this date.
 			handled (bool): A true/false parameter indicating whether events were handled/unhandled.
 			includeStatistics (bool): A true/false parameter indicating including statistics data.
 			ips (list): Specifies the list of IPs where the products were seen.
+			string (list): Specifies the list of IPs where the products were seen.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastConnectionTimeEnd (str):  Retrieves products whose last connection time is less than the value assigned to this date.
 			lastConnectionTimeStart (str):  Retrieves products whose last connection time is greater than the value assigned to this date.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			os (list): Specifies the list of operating system families where the products were seen.
+			string (list): Specifies the list of operating system families where the products were seen.
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			policies (list): Specifies the list of policy names whose products have a specific decision, as specified in the action parameter.
+			string (list): Specifies the list of policy names whose products have a specific decision, as specified in the action parameter.
 			processHash (str): Specifies the process hash name.
 			processes (list): Specifies the list of process names running alongside the products.
+			string (list): Specifies the list of process names running alongside the products.
 			product (str): Specifies a single value for the product name. By default, strictMode is false.
 			products (list): Specifies the list of product names. Names must match exactly (strictMode is always true).
+			string (list): Specifies the list of product names. Names must match exactly (strictMode is always true).
 			reputation (list): Specifies the recommendation of the application: Unknown, Known bad, Assumed bad, Contradiction, Assumed good or Known good.
+			string (list): Specifies the recommendation of the application: Unknown, Known bad, Assumed bad, Contradiction, Assumed good or Known good.
 			rule (str): Indicates the rule. This parameter is irrelevant without rulePolicy parameter.
 			rulePolicy (str): Specifies the policy name whose products have a specific rule, as specified in the rule parameter.
 			seen (bool): A true/false parameter indicating whether events were read/unread by the user operating the API.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 			vendor (str): Specifies a single value for the vendor name. By default, strictMode is false.
 			vendors (list): Specifies the list of vendor names. Names must match exactly (strictMode is always true).
+			string (list): Specifies the list of vendor names. Names must match exactly (strictMode is always true).
 			version (str): Specifies a single value for the version name. By default, strictMode is false.
 			versions (list): Specifies the list of versions. Names must match exactly (strictMode is always true).
+			string (list): Specifies the list of versions. Names must match exactly (strictMode is always true).
 			vulnerabilities (list): Specifies the list of vulnerabilities where the products were seen.
+			string (list): Specifies the list of vulnerabilities where the products were seen.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("list_products", locals())
 
@@ -760,18 +782,21 @@
 		Description: Enable resolving/unresolving applications.
         
 		Args:
 			applyNested (bool): A true/false parameter indicating updating inherited.
 			comment (str): Specifies a user-defined string to attach to the policy.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			products (list): Specifies the list of product names. Names must match exactly (strictMode is always true).
+			string (list): Specifies the list of product names. Names must match exactly (strictMode is always true).
 			resolve (bool): A true/false parameter indicating update the application resolve/unresolve.
 			signed (bool): A true/false parameter indicating if the policy is signed.
 			vendors (list): Specifies the list of vendor names. Names must match exactly (strictMode is always true).
+			string (list): Specifies the list of vendor names. Names must match exactly (strictMode is always true).
 			versions (list): Specifies the list of versions. Names must match exactly (strictMode is always true).
+			string (list): Specifies the list of versions. Names must match exactly (strictMode is always true).
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("resolve_applications", locals())
 
@@ -801,14 +826,15 @@
 		Class CommunicationControl
 		Description: Set policy to simulation/prevention.
         
 		Args:
 			mode (str): Operation mode.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			policyNames (list): Specifies the list of policies.
+			string (list): Specifies the list of policies.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("set_policy_mode", locals())
 
@@ -829,18 +855,22 @@
 		Description: Set the application allow/deny.
         
 		Args:
 			applyNested (bool): A true/false parameter indicating updating inherited.
 			decision (str): Indicates the action.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			policies (list): Specifies the list of policies names.
+			string (list): Specifies the list of policies names.
 			products (list): Specifies the list of product names. Names must match exactly (strictMode is always true).
+			string (list): Specifies the list of product names. Names must match exactly (strictMode is always true).
 			signed (bool): A true/false parameter indicating if the policy is signed.
 			vendors (list): Specifies the list of vendor names. Names must match exactly (strictMode is always true).
+			string (list): Specifies the list of vendor names. Names must match exactly (strictMode is always true).
 			versions (list): Specifies the list of versions. Names must match exactly (strictMode is always true).
+			string (list): Specifies the list of versions. Names must match exactly (strictMode is always true).
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("set_policy_permission", locals())
 
@@ -901,47 +931,58 @@
 	def insert_events(self, actions: list = None, applicationControl: bool = None, archived: bool = None, classifications: list = None, collectorGroups: list = None, destinations: list = None, device: str = None, deviceControl: bool = None, deviceIps: list = None, eventIds: list = None, eventType: list = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: list = None, muted: bool = None, operatingSystems: list = None, organization: str = None, pageNumber: int = None, paths: list = None, process: str = None, rule: str = None, seen: bool = None, severities: list = None, signed: bool = None, sorting: str = None, strictMode: bool = None, archive: bool = None, classification: str = None, comment: str = None, familyName: str = None, forceUnmute: bool = None, handle: bool = None, malwareType: str = None, mute: bool = None, muteDuration: str = None, read: bool = None, threatName: str = None) -> tuple[bool, None]:
 		'''
 		Class Events
 		Description: This API call updates the read/unread, handled/unhandled or archived/unarchived state of an event. The output of this call is a message indicating whether the update succeeded or failed.
         
 		Args:
 			actions (list): Specifies the action of the event.
+			string (list): Specifies the action of the event.
 			applicationControl (bool): A true/false parameter indicating whether to include only application control events.
 			archived (bool): A true/false parameter indicating whether to include only archived events.
 			classifications (list): Specifies the classification of the event.
+			string (list): Specifies the classification of the event.
 			collectorGroups (list): Specifies the collector groups whose collector reported the events.
+			string (list): Specifies the collector groups whose collector reported the events.
 			destinations (list): Specifies the connection destination(s) of the events.
+			string (list): Specifies the connection destination(s) of the events.
 			device (str): Specifies the device name where the events occurred.
 			deviceControl (bool): A true/false parameter indicating whether to include only device control events.
 			deviceIps (list): Specifies the IPs of the devices where the event occurred.
+			string (list): Specifies the IPs of the devices where the event occurred.
 			eventIds (list): Specifies the required event IDs.
+			integer (list): Specifies the required event IDs.
 			eventType (list): Specifies the type of the event.
+			string (list): Specifies the type of the event.
 			expired (bool): A true/false parameter indicating whether to include only expired events.
 			fileHash (str): Specifies the hash signature of the main process of the event.
 			firstSeen (str):  Specifies the date when the event was first seen (Deprecated).
 			firstSeenFrom (str): Specifies the from date when the event was first seen.
 			firstSeenTo (str): Specifies the to date when the event was first seen.
 			handled (bool):  A true/false parameter indicating whether events were handled/unhandled.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeen (str):  Specifies the date when the event was last seen (Deprecated).
 			lastSeenFrom (str): Specifies the from date when the event was last seen.
 			lastSeenTo (str): Specifies the to date when the event was last seen.
 			loggedUser (str): Specifies the logged user.
 			macAddresses (list): Specifies the mac addresses where the event occurred.
+			string (list): Specifies the mac addresses where the event occurred.
 			muted (bool): A true/false parameter indicating if the event is muted.
 			operatingSystems (list): Specifies the operating system of the devices where the events occurred.
+			string (list): Specifies the operating system of the devices where the events occurred.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			paths (list): Specifies the paths of the processes related to the event.
+			string (list): Specifies the paths of the processes related to the event.
 			process (str): Specifies the main process of the event.
 			rule (str): Specifies the short rule name of the rule that triggered the events.
 			seen (bool): A true/false parameter indicating whether events were read/unread by the user operating the API.
 			severities (list): Specifies the severity of the event (Deprecated).
+			string (list): Specifies the severity of the event (Deprecated).
 			signed (bool): A true/false parameter indicating if the event is signed.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 			updateEventsRequest (Object): Check 'updateEventsRequest' in the API documentation for further information.
 
 		Returns:
 			bool: Status of the request (True or False). 
@@ -966,15 +1007,15 @@
 		if device:
 			url_params.append('device=' + device)
 		if deviceControl:
 			url_params.append('deviceControl=' + deviceControl)
 		if deviceIps:
 			url_params.append('deviceIps=' + ",".join(str(deviceIps)))
 		if eventIds:
-			url_params.append('eventIds=' + ",".join(str(eventIds)))
+			url_params.append('eventIds=' + ",".join(map(str, eventIds)))
 		if eventType:
 			url_params.append('eventType=' + ",".join(str(eventType)))
 		if expired:
 			url_params.append('expired=' + expired)
 		if fileHash:
 			url_params.append('fileHash=' + fileHash)
 		if firstSeen:
@@ -1041,48 +1082,59 @@
 	def delete_events(self, actions: list = None, applicationControl: bool = None, archived: bool = None, classifications: list = None, collectorGroups: list = None, deleteAll: bool = None, destinations: list = None, device: str = None, deviceControl: bool = None, deviceIps: list = None, eventIds: list = None, eventType: list = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: list = None, muted: bool = None, operatingSystems: list = None, organization: str = None, pageNumber: int = None, paths: list = None, process: str = None, rule: str = None, seen: bool = None, severities: list = None, signed: bool = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, None]:
 		'''
 		Class Events
 		Description: This API call delete events.
         
 		Args:
 			actions (list): Specifies the action of the event.
+			string (list): Specifies the action of the event.
 			applicationControl (bool): A true/false parameter indicating whether to include only application control events.
 			archived (bool): A true/false parameter indicating whether to include only archived events.
 			classifications (list): Specifies the classification of the event.
+			string (list): Specifies the classification of the event.
 			collectorGroups (list): Specifies the collector groups whose collector reported the events.
+			string (list): Specifies the collector groups whose collector reported the events.
 			deleteAll (bool): A true/false parameter indicating if all events should be deleted.
 			destinations (list): Specifies the connection destination(s) of the events.
+			string (list): Specifies the connection destination(s) of the events.
 			device (str): Specifies the device name where the events occurred.
 			deviceControl (bool): A true/false parameter indicating whether to include only device control events.
 			deviceIps (list): Specifies the IPs of the devices where the event occurred.
+			string (list): Specifies the IPs of the devices where the event occurred.
 			eventIds (list): Specifies the required event IDs.
+			integer (list): Specifies the required event IDs.
 			eventType (list): Specifies the type of the event.
+			string (list): Specifies the type of the event.
 			expired (bool): A true/false parameter indicating whether to include only expired events.
 			fileHash (str): Specifies the hash signature of the main process of the event.
 			firstSeen (str):  Specifies the date when the event was first seen (Deprecated).
 			firstSeenFrom (str): Specifies the from date when the event was first seen.
 			firstSeenTo (str): Specifies the to date when the event was first seen.
 			handled (bool):  A true/false parameter indicating whether events were handled/unhandled.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeen (str):  Specifies the date when the event was last seen (Deprecated).
 			lastSeenFrom (str): Specifies the from date when the event was last seen.
 			lastSeenTo (str): Specifies the to date when the event was last seen.
 			loggedUser (str): Specifies the logged user.
 			macAddresses (list): Specifies the mac addresses where the event occurred.
+			string (list): Specifies the mac addresses where the event occurred.
 			muted (bool): A true/false parameter indicating if the event is muted.
 			operatingSystems (list): Specifies the operating system of the devices where the events occurred.
+			string (list): Specifies the operating system of the devices where the events occurred.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			paths (list): Specifies the paths of the processes related to the event.
+			string (list): Specifies the paths of the processes related to the event.
 			process (str): Specifies the main process of the event.
 			rule (str): Specifies the short rule name of the rule that triggered the events.
 			seen (bool): A true/false parameter indicating whether events were read/unread by the user operating the API.
 			severities (list): Specifies the severity of the event (Deprecated).
+			string (list): Specifies the severity of the event (Deprecated).
 			signed (bool): A true/false parameter indicating if the event is signed.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
@@ -1108,15 +1160,15 @@
 		if device:
 			url_params.append('device=' + device)
 		if deviceControl:
 			url_params.append('deviceControl=' + deviceControl)
 		if deviceIps:
 			url_params.append('deviceIps=' + ",".join(str(deviceIps)))
 		if eventIds:
-			url_params.append('eventIds=' + ",".join(str(eventIds)))
+			url_params.append('eventIds=' + ",".join(map(str, eventIds)))
 		if eventType:
 			url_params.append('eventType=' + ",".join(str(eventType)))
 		if expired:
 			url_params.append('expired=' + expired)
 		if fileHash:
 			url_params.append('fileHash=' + fileHash)
 		if firstSeen:
@@ -1169,47 +1221,58 @@
 	def count_events(self, actions: list = None, applicationControl: bool = None, archived: bool = None, classifications: list = None, collectorGroups: list = None, destinations: list = None, device: str = None, deviceControl: bool = None, deviceIps: list = None, eventIds: list = None, eventType: list = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: list = None, muted: bool = None, operatingSystems: list = None, organization: str = None, pageNumber: int = None, paths: list = None, process: str = None, rule: str = None, seen: bool = None, severities: list = None, signed: bool = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, int]:
 		'''
 		Class Events
 		Description: Count Events.
         
 		Args:
 			actions (list): Specifies the action of the event.
+			string (list): Specifies the action of the event.
 			applicationControl (bool): A true/false parameter indicating whether to include only application control events.
 			archived (bool): A true/false parameter indicating whether to include only archived events.
 			classifications (list): Specifies the classification of the event.
+			string (list): Specifies the classification of the event.
 			collectorGroups (list): Specifies the collector groups whose collector reported the events.
+			string (list): Specifies the collector groups whose collector reported the events.
 			destinations (list): Specifies the connection destination(s) of the events.
+			string (list): Specifies the connection destination(s) of the events.
 			device (str): Specifies the device name where the events occurred.
 			deviceControl (bool): A true/false parameter indicating whether to include only device control events.
 			deviceIps (list): Specifies the IPs of the devices where the event occurred.
+			string (list): Specifies the IPs of the devices where the event occurred.
 			eventIds (list): Specifies the required event IDs.
+			integer (list): Specifies the required event IDs.
 			eventType (list): Specifies the type of the event.
+			string (list): Specifies the type of the event.
 			expired (bool): A true/false parameter indicating whether to include only expired events.
 			fileHash (str): Specifies the hash signature of the main process of the event.
 			firstSeen (str):  Specifies the date when the event was first seen (Deprecated).
 			firstSeenFrom (str): Specifies the from date when the event was first seen.
 			firstSeenTo (str): Specifies the to date when the event was first seen.
 			handled (bool):  A true/false parameter indicating whether events were handled/unhandled.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeen (str):  Specifies the date when the event was last seen (Deprecated).
 			lastSeenFrom (str): Specifies the from date when the event was last seen.
 			lastSeenTo (str): Specifies the to date when the event was last seen.
 			loggedUser (str): Specifies the logged user.
 			macAddresses (list): Specifies the mac addresses where the event occurred.
+			string (list): Specifies the mac addresses where the event occurred.
 			muted (bool): A true/false parameter indicating if the event is muted.
 			operatingSystems (list): Specifies the operating system of the devices where the events occurred.
+			string (list): Specifies the operating system of the devices where the events occurred.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			paths (list): Specifies the paths of the processes related to the event.
+			string (list): Specifies the paths of the processes related to the event.
 			process (str): Specifies the main process of the event.
 			rule (str): Specifies the short rule name of the rule that triggered the events.
 			seen (bool): A true/false parameter indicating whether events were read/unread by the user operating the API.
 			severities (list): Specifies the severity of the event (Deprecated).
+			string (list): Specifies the severity of the event (Deprecated).
 			signed (bool): A true/false parameter indicating if the event is signed.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			int
@@ -1233,15 +1296,15 @@
 		if device:
 			url_params.append('device=' + device)
 		if deviceControl:
 			url_params.append('deviceControl=' + deviceControl)
 		if deviceIps:
 			url_params.append('deviceIps=' + ",".join(str(deviceIps)))
 		if eventIds:
-			url_params.append('eventIds=' + ",".join(str(eventIds)))
+			url_params.append('eventIds=' + ",".join(map(str, eventIds)))
 		if eventType:
 			url_params.append('eventType=' + ",".join(str(eventType)))
 		if expired:
 			url_params.append('expired=' + expired)
 		if fileHash:
 			url_params.append('fileHash=' + fileHash)
 		if firstSeen:
@@ -1298,22 +1361,25 @@
         
 		Args:
 			allCollectorGroups (bool): A true/false parameter indicating whether the exception should be applied to all collector groups. When not used, all collector groups are selected.
 			allDestinations (bool): A true/false parameter indicating whether the exception should be applied to all destinations. When not used, all destinations are selected.
 			allOrganizations (bool): A true/false parameter indicating whether the exception should be applied to all the organizations (tenants). This parameter is only relevant in multi-tenancy environment. This parameter is only allowed for user with Hoster privilege (general admin).
 			allUsers (bool): A true/false parameter indicating whether the exception should be applied to all users. When not used, all users are selected.
 			collectorGroups (list): Specifies the list of all the collector groups to which the exception should be applied. When not used, all collector groups are selected.
+			string (list): Specifies the list of all the collector groups to which the exception should be applied. When not used, all collector groups are selected.
 			comment (str): Specifies a user-defined string to attach to the exception.
 			destinations (list): A list of IPs to which the exception applies and/or the value all internal destinations.
+			string (list): A list of IPs to which the exception applies and/or the value all internal destinations.
 			eventId (int): Specifies the event ID on which to create the exception.
 			exceptionId (int): Specifies the exception ID to edit.
 			exceptionRequest (Object): Check 'exceptionRequest' in the API documentation for further information.
 			forceCreate (bool): A true/false parameter indicating whether to create the exception, even if there are already exceptions that cover this given event.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			users (list): A list of users to which the exception.
+			string (list): A list of users to which the exception.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			str
 		'''
 		validate_params("create_exception", locals())
 
@@ -1380,47 +1446,58 @@
 	def list_events(self, actions: list = None, applicationControl: bool = None, archived: bool = None, classifications: list = None, collectorGroups: list = None, destinations: list = None, device: str = None, deviceControl: bool = None, deviceIps: list = None, eventIds: list = None, eventType: list = None, expired: bool = None, fileHash: str = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, handled: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, macAddresses: list = None, muted: bool = None, operatingSystems: list = None, organization: str = None, pageNumber: int = None, paths: list = None, process: str = None, rule: str = None, seen: bool = None, severities: list = None, signed: bool = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, list]:
 		'''
 		Class Events
 		Description: List Events.
         
 		Args:
 			actions (list): Specifies the action of the event.
+			string (list): Specifies the action of the event.
 			applicationControl (bool): A true/false parameter indicating whether to include only application control events.
 			archived (bool): A true/false parameter indicating whether to include only archived events.
 			classifications (list): Specifies the classification of the event.
+			string (list): Specifies the classification of the event.
 			collectorGroups (list): Specifies the collector groups whose collector reported the events.
+			string (list): Specifies the collector groups whose collector reported the events.
 			destinations (list): Specifies the connection destination(s) of the events.
+			string (list): Specifies the connection destination(s) of the events.
 			device (str): Specifies the device name where the events occurred.
 			deviceControl (bool): A true/false parameter indicating whether to include only device control events.
 			deviceIps (list): Specifies the IPs of the devices where the event occurred.
+			string (list): Specifies the IPs of the devices where the event occurred.
 			eventIds (list): Specifies the required event IDs.
+			integer (list): Specifies the required event IDs.
 			eventType (list): Specifies the type of the event.
+			string (list): Specifies the type of the event.
 			expired (bool): A true/false parameter indicating whether to include only expired events.
 			fileHash (str): Specifies the hash signature of the main process of the event.
 			firstSeen (str):  Specifies the date when the event was first seen (Deprecated).
 			firstSeenFrom (str): Specifies the from date when the event was first seen.
 			firstSeenTo (str): Specifies the to date when the event was first seen.
 			handled (bool):  A true/false parameter indicating whether events were handled/unhandled.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeen (str):  Specifies the date when the event was last seen (Deprecated).
 			lastSeenFrom (str): Specifies the from date when the event was last seen.
 			lastSeenTo (str): Specifies the to date when the event was last seen.
 			loggedUser (str): Specifies the logged user.
 			macAddresses (list): Specifies the mac addresses where the event occurred.
+			string (list): Specifies the mac addresses where the event occurred.
 			muted (bool): A true/false parameter indicating if the event is muted.
 			operatingSystems (list): Specifies the operating system of the devices where the events occurred.
+			string (list): Specifies the operating system of the devices where the events occurred.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			paths (list): Specifies the paths of the processes related to the event.
+			string (list): Specifies the paths of the processes related to the event.
 			process (str): Specifies the main process of the event.
 			rule (str): Specifies the short rule name of the rule that triggered the events.
 			seen (bool): A true/false parameter indicating whether events were read/unread by the user operating the API.
 			severities (list): Specifies the severity of the event (Deprecated).
+			string (list): Specifies the severity of the event (Deprecated).
 			signed (bool): A true/false parameter indicating if the event is signed.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
@@ -1444,15 +1521,15 @@
 		if device:
 			url_params.append('device=' + device)
 		if deviceControl:
 			url_params.append('deviceControl=' + deviceControl)
 		if deviceIps:
 			url_params.append('deviceIps=' + ",".join(str(deviceIps)))
 		if eventIds:
-			url_params.append('eventIds=' + ",".join(str(eventIds)))
+			url_params.append('eventIds=' + ",".join(map(str, eventIds)))
 		if eventType:
 			url_params.append('eventType=' + ",".join(str(eventType)))
 		if expired:
 			url_params.append('expired=' + expired)
 		if fileHash:
 			url_params.append('fileHash=' + fileHash)
 		if firstSeen:
@@ -1505,30 +1582,34 @@
 	def list_raw_data_items(self, eventId: int, collectorGroups: list = None, destinations: list = None, device: str = None, deviceIps: list = None, firstSeen: str = None, firstSeenFrom: str = None, firstSeenTo: str = None, fullDataRequested: bool = None, itemsPerPage: int = None, lastSeen: str = None, lastSeenFrom: str = None, lastSeenTo: str = None, loggedUser: str = None, organization: str = None, pageNumber: int = None, rawEventIds: list = None, sorting: str = None, strictMode: bool = None) -> tuple[bool, list]:
 		'''
 		Class Events
 		Description: List raw data items.
         
 		Args:
 			collectorGroups (list): Specifies the collector groups whose collector reported the raw events.
+			string (list): Specifies the collector groups whose collector reported the raw events.
 			destinations (list): Specifies the connection destination(s) of the events.
+			string (list): Specifies the connection destination(s) of the events.
 			device (str): Specifies the name of the device where the raw event occurred.
 			deviceIps (list): Specifies the IPs of the devices where the event occurred.
+			string (list): Specifies the IPs of the devices where the event occurred.
 			eventId (int): Specifies the ID of the event that holds the raw data items.
 			firstSeen (str): Specifies the date when the raw data item was first seen (Deprecated).
 			firstSeenFrom (str): Specifies the from date when the raw data item was first seen.
 			firstSeenTo (str): Specifies the to date when the raw data item was first seen.
 			fullDataRequested (bool): A true/false parameter indicating whether to include the event internal information.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeen (str): Specifies the date when the raw data item was last seen (Deprecated).
 			lastSeenFrom (str): Specifies the from date when the raw data item was last seen.
 			lastSeenTo (str): Specifies the to date when the raw data item was last seen.
 			loggedUser (str): Specifies the logged user.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			rawEventIds (list): Specifies the list of raw data item event IDs.
+			integer (list): Specifies the list of raw data item event IDs.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
@@ -1565,15 +1646,15 @@
 		if loggedUser:
 			url_params.append('loggedUser=' + loggedUser)
 		if organization:
 			url_params.append('organization=' + organization)
 		if pageNumber:
 			url_params.append('pageNumber=' + pageNumber)
 		if rawEventIds:
-			url_params.append('rawEventIds=' + ",".join(str(rawEventIds)))
+			url_params.append('rawEventIds=' + ",".join(map(str, rawEventIds)))
 		if sorting:
 			url_params.append('sorting=' + sorting)
 		if strictMode:
 			url_params.append('strictMode=' + strictMode)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
@@ -1608,27 +1689,30 @@
 	def delete(self, collectorGroups: list = None, comment: str = None, createdAfter: str = None, createdBefore: str = None, deleteAll: bool = None, destination: str = None, exceptionId: int = None, exceptionIds: list = None, organization: str = None, path: str = None, process: str = None, rules: list = None, updatedAfter: str = None, updatedBefore: str = None, user: str = None) -> tuple[bool, None]:
 		'''
 		Class Exceptions
 		Description: Delete exceptions.
         
 		Args:
 			collectorGroups (list): Specifies the list of all the collector groups to which the exception applied.
+			string (list): Specifies the list of all the collector groups to which the exception applied.
 			comment (str): Specifies a comment attach to the exception.
 			createdAfter (str): Specifies the date after which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			createdBefore (str): Specifies the date before which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			deleteAll (bool): A true/false parameter indicating if all exception should be deleted.
 			destination (str): Specifies a destination IP of the exception.
 			exceptionId (int): Specifies the required exception ID.
 			exceptionIds (list): Specifies a list of exception ids.
+			integer (list): Specifies a list of exception ids.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			path (str): Specifies the path of the exception.
 			process (str): Specifies the process of the exception.
 			rules (list): Specifies a list of rule names.
+			string (list): Specifies a list of rule names.
 			updatedAfter (str): Specifies the date after which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			updatedBefore (str): Specifies the date before which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			user (str): Specifies a user of the exception.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
@@ -1648,15 +1732,15 @@
 		if deleteAll:
 			url_params.append('deleteAll=' + deleteAll)
 		if destination:
 			url_params.append('destination=' + destination)
 		if exceptionId:
 			url_params.append('exceptionId=' + exceptionId)
 		if exceptionIds:
-			url_params.append('exceptionIds=' + ",".join(str(exceptionIds)))
+			url_params.append('exceptionIds=' + ",".join(map(str, exceptionIds)))
 		if organization:
 			url_params.append('organization=' + organization)
 		if path:
 			url_params.append('path=' + path)
 		if process:
 			url_params.append('process=' + process)
 		if rules:
@@ -1697,25 +1781,28 @@
 	def list_exceptions(self, collectorGroups: list = None, comment: str = None, createdAfter: str = None, createdBefore: str = None, destination: str = None, exceptionIds: list = None, organization: str = None, path: str = None, process: str = None, rules: list = None, updatedAfter: str = None, updatedBefore: str = None, user: str = None) -> tuple[bool, list]:
 		'''
 		Class Exceptions
 		Description: List of exceptions.
         
 		Args:
 			collectorGroups (list): Specifies the list of all the collector groups to which the exception applied.
+			string (list): Specifies the list of all the collector groups to which the exception applied.
 			comment (str): Specifies a comment attach to the exception.
 			createdAfter (str): Specifies the date after which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			createdBefore (str): Specifies the date before which the exception was created. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			destination (str): Specifies a destination IP of the exception.
 			exceptionIds (list): Specifies a list of exception ids.
+			integer (list): Specifies a list of exception ids.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			path (str): Specifies the path of the exception.
 			process (str): Specifies the process of the exception.
 			rules (list): Specifies a list of rule names.
+			string (list): Specifies a list of rule names.
 			updatedAfter (str): Specifies the date after which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			updatedBefore (str): Specifies the date before which the exception was updated. Specify the date using the yyyy-MM-dd HH:mm:ss format.
 			user (str): Specifies a user of the exception.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
@@ -1731,15 +1818,15 @@
 		if createdAfter:
 			url_params.append('createdAfter=' + createdAfter)
 		if createdBefore:
 			url_params.append('createdBefore=' + createdBefore)
 		if destination:
 			url_params.append('destination=' + destination)
 		if exceptionIds:
-			url_params.append('exceptionIds=' + ",".join(str(exceptionIds)))
+			url_params.append('exceptionIds=' + ",".join(map(str, exceptionIds)))
 		if organization:
 			url_params.append('organization=' + organization)
 		if path:
 			url_params.append('path=' + path)
 		if process:
 			url_params.append('process=' + process)
 		if rules:
@@ -1761,14 +1848,15 @@
 		Class Forensics
 		Description: This API call retrieves a file or memory.
         
 		Args:
 			disk (bool): A true/false parameter indicating whether find in the disk.
 			endRange (str): Specifies the memory end range, in Hexadecimal format.
 			filePaths (list): Specifies the list of file paths.
+			string (list): Specifies the list of file paths.
 			memory (bool): A true/false parameter indicating whether find in the memory.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			processId (int): Specifies the ID of the process from which to take a memory image. required for memory base action.
 			rawEventId (int): Specifies the ID of the raw event on which to perform the memory retrieval.
 			startRange (str): Specifies the memory start range, in Hexadecimal format.
 
 		Returns:
@@ -1802,14 +1890,15 @@
 		'''
 		Class Forensics
 		Description: This API call retrieves a file or memory.
         
 		Args:
 			device (str): Specifies the name or id of the device to remediate.
 			filePaths (list): Specifies the list of file paths.
+			string (list): Specifies the list of file paths.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			type (str): Specifies the device parameter type used in the request : Name or ID.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
@@ -1834,14 +1923,16 @@
 		Description: This API kill process / delete file / clean persistence, File and persistence paths must be specified in a logical format.
         
 		Args:
 			device (str): Specifies the name of the device to remediate. You must specify a value for either device or deviceId (see below).
 			deviceId (int): Specifies the unique identifier (ID) of the device to remediate. You must specify a value for either deviceId or device (see above).
 			executablesToRemove (list): Specifies the list of full paths of executable files (*.exe) to delete on the
 given device.
+			string (list): Specifies the list of full paths of executable files (*.exe) to delete on the
+given device.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			persistenceDataAction (str): persistence data desired action.
 			persistenceDataNewContent (str): persistence data new content.
 			persistenceDataPath (str): persistence data path.
 			persistenceDataValueName (str): persistence data value name.
 			persistenceDataValueNewType (str): persistence data value new type.
 			processName (str): Specifies the process name.
@@ -1889,14 +1980,15 @@
 	def search(self, fileHashes: list, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class HashSearch
 		Description: This API enables the user to search a file hash among the current events, threat hunting repository and communicating applications that exist in the system.
         
 		Args:
 			fileHashes (list): Specifies the list of files hashes.
+			string (list): Specifies the list of files hashes.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
@@ -2261,45 +2353,60 @@
 	def delete_collectors(self, cloudAccounts: list = None, cloudProviders: list = None, clusters: list = None, collectorGroups: list = None, collectorGroupsIds: list = None, collectorType: str = None, confirmDeletion: bool = None, deleteAll: bool = None, devices: list = None, devicesIds: list = None, firstSeen: str = None, hasCrashDumps: bool = None, ips: list = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, loggedUser: str = None, operatingSystems: list = None, organization: str = None, osFamilies: list = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, states: list = None, strictMode: bool = None, versions: list = None) -> tuple[bool, None]:
 		'''
 		Class SystemInventory
 		Description: This API call deletes a Collector(s).
         
 		Args:
 			cloudAccounts (list): Specifies the list cloud account names.
+			string (list): Specifies the list cloud account names.
 			cloudProviders (list): Specifies the list of cloud providers: AWS, Azure, GCP.
+			string (list): Specifies the list of cloud providers: AWS, Azure, GCP.
 			clusters (list): Specifies the list of cluster.
+			string (list): Specifies the list of cluster.
 			collectorGroups (list): Specifies the list of collector group names and retrieves collectors under the
 given groups.
+			string (list): Specifies the list of collector group names and retrieves collectors under the
+given groups.
 			collectorGroupsIds (list): Specifies the list of collector group Ids and retrieves collectors under the
 given groups.
+			integer (list): Specifies the list of collector group Ids and retrieves collectors under the
+given groups.
 			collectorType (str): Specifies the group types of the collectors. Types: All, Collector, Workloads. All by default.
 			confirmDeletion (bool): A true/false parameter indicating if to detach/delete relevant exceptions from Collector groups about to be deleted.
 			deleteAll (bool): A true/false parameter indicating if all collectors should be deleted.
 			devices (list): Specifies the list of device names.
+			string (list): Specifies the list of device names.
 			devicesIds (list): Specifies the list of device ids.
+			integer (list): Specifies the list of device ids.
 			firstSeen (str): Retrieves collectors that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			hasCrashDumps (bool): Retrieves collectors that have crash dumps.
 			ips (list): Specifies the list of IP values.
+			string (list): Specifies the list of IP values.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeenEnd (str): Retrieves collectors that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			lastSeenStart (str): Retrieves collectors that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			loggedUser (str): Specifies the user that was logged when the event occurred.
 			operatingSystems (list): Specifies the list of specific operating systems. For example, Windows 7 Pro.
+			string (list): Specifies the list of specific operating systems. For example, Windows 7 Pro.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
 .
 			osFamilies (list): Specifies the list of operating system families: Windows, Windows Server or OS X.
+			string (list): Specifies the list of operating system families: Windows, Windows Server or OS X.
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			showExpired (bool): Specifies whether to include collectors which have been disconnected for more than 30 days (sequentially) and are marked as Expired.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			states (list): Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, 
 Pending Reboot, Isolated, Expired, Migrated or Pending Migration.
+			string (list): Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, 
+Pending Reboot, Isolated, Expired, Migrated or Pending Migration.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 			versions (list): Specifies the list of collector versions.
+			string (list): Specifies the list of collector versions.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("delete_collectors", locals())
 
@@ -2310,25 +2417,25 @@
 		if cloudProviders:
 			url_params.append('cloudProviders=' + ",".join(str(cloudProviders)))
 		if clusters:
 			url_params.append('clusters=' + ",".join(str(clusters)))
 		if collectorGroups:
 			url_params.append('collectorGroups=' + ",".join(str(collectorGroups)))
 		if collectorGroupsIds:
-			url_params.append('collectorGroupsIds=' + ",".join(str(collectorGroupsIds)))
+			url_params.append('collectorGroupsIds=' + ",".join(map(str, collectorGroupsIds)))
 		if collectorType:
 			url_params.append('collectorType=' + collectorType)
 		if confirmDeletion:
 			url_params.append('confirmDeletion=' + confirmDeletion)
 		if deleteAll:
 			url_params.append('deleteAll=' + deleteAll)
 		if devices:
 			url_params.append('devices=' + ",".join(str(devices)))
 		if devicesIds:
-			url_params.append('devicesIds=' + ",".join(str(devicesIds)))
+			url_params.append('devicesIds=' + ",".join(map(str, devicesIds)))
 		if firstSeen:
 			url_params.append('firstSeen=' + firstSeen)
 		if hasCrashDumps:
 			url_params.append('hasCrashDumps=' + hasCrashDumps)
 		if ips:
 			url_params.append('ips=' + ",".join(str(ips)))
 		if itemsPerPage:
@@ -2363,46 +2470,50 @@
 	def isolate_collectors(self, devices: list = None, devicesIds: list = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class SystemInventory
 		Description: This API call isolate collector functionality.
         
 		Args:
 			devices (list): Specifies the list of device names.
+			string (list): Specifies the list of device names.
 			devicesIds (list): Specifies the list of device ids.
+			integer (list): Specifies the list of device ids.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("isolate_collectors", locals())
 
 		url = '/management-rest/inventory/isolate-collectors'
 		url_params = []
 		if devices:
 			url_params.append('devices=' + ",".join(str(devices)))
 		if devicesIds:
-			url_params.append('devicesIds=' + ",".join(str(devicesIds)))
+			url_params.append('devicesIds=' + ",".join(map(str, devicesIds)))
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
 	def list_aggregators(self, ip: str = None, names: list = None, organization: str = None, versions: list = None) -> tuple[bool, list]:
 		'''
 		Class SystemInventory
 		Description: This API call output the list of aggregators.
         
 		Args:
 			ip (str): IP.
 			names (list): List of aggregators names.
+			string (list): List of aggregators names.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			versions (list): List of aggregators versions.
+			string (list): List of aggregators versions.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("list_aggregators", locals())
 
@@ -2445,43 +2556,58 @@
 	def list_collectors(self, cloudAccounts: list = None, cloudProviders: list = None, clusters: list = None, collectorGroups: list = None, collectorGroupsIds: list = None, collectorType: str = None, devices: list = None, devicesIds: list = None, firstSeen: str = None, hasCrashDumps: bool = None, ips: list = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, loggedUser: str = None, operatingSystems: list = None, organization: str = None, osFamilies: list = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, states: list = None, strictMode: bool = None, versions: list = None) -> tuple[bool, list]:
 		'''
 		Class SystemInventory
 		Description: This API call outputs a list of the Collectors in the system. Use the input parameters to filter the list.
         
 		Args:
 			cloudAccounts (list): Specifies the list cloud account names.
+			string (list): Specifies the list cloud account names.
 			cloudProviders (list): Specifies the list of cloud providers: AWS, Azure, GCP.
+			string (list): Specifies the list of cloud providers: AWS, Azure, GCP.
 			clusters (list): Specifies the list of cluster.
+			string (list): Specifies the list of cluster.
 			collectorGroups (list): Specifies the list of collector group names and retrieves collectors under the
 given groups.
+			string (list): Specifies the list of collector group names and retrieves collectors under the
+given groups.
 			collectorGroupsIds (list): Specifies the list of collector group Ids and retrieves collectors under the
 given groups.
+			integer (list): Specifies the list of collector group Ids and retrieves collectors under the
+given groups.
 			collectorType (str): Specifies the group types of the collectors. Types: All, Collector, Workloads. All by default.
 			devices (list): Specifies the list of device names.
+			string (list): Specifies the list of device names.
 			devicesIds (list): Specifies the list of device ids.
+			integer (list): Specifies the list of device ids.
 			firstSeen (str): Retrieves collectors that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			hasCrashDumps (bool): Retrieves collectors that have crash dumps.
 			ips (list): Specifies the list of IP values.
+			string (list): Specifies the list of IP values.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeenEnd (str): Retrieves collectors that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			lastSeenStart (str): Retrieves collectors that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			loggedUser (str): Specifies the user that was logged when the event occurred.
 			operatingSystems (list): Specifies the list of specific operating systems. For example, Windows 7 Pro.
+			string (list): Specifies the list of specific operating systems. For example, Windows 7 Pro.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
 .
 			osFamilies (list): Specifies the list of operating system families: Windows, Windows Server or OS X.
+			string (list): Specifies the list of operating system families: Windows, Windows Server or OS X.
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			showExpired (bool): Specifies whether to include collectors which have been disconnected for more than 30 days (sequentially) and are marked as Expired.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			states (list): Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, 
 Pending Reboot, Isolated, Expired, Migrated or Pending Migration.
+			string (list): Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, 
+Pending Reboot, Isolated, Expired, Migrated or Pending Migration.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 			versions (list): Specifies the list of collector versions.
+			string (list): Specifies the list of collector versions.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("list_collectors", locals())
 
@@ -2492,21 +2618,21 @@
 		if cloudProviders:
 			url_params.append('cloudProviders=' + ",".join(str(cloudProviders)))
 		if clusters:
 			url_params.append('clusters=' + ",".join(str(clusters)))
 		if collectorGroups:
 			url_params.append('collectorGroups=' + ",".join(str(collectorGroups)))
 		if collectorGroupsIds:
-			url_params.append('collectorGroupsIds=' + ",".join(str(collectorGroupsIds)))
+			url_params.append('collectorGroupsIds=' + ",".join(map(str, collectorGroupsIds)))
 		if collectorType:
 			url_params.append('collectorType=' + collectorType)
 		if devices:
 			url_params.append('devices=' + ",".join(str(devices)))
 		if devicesIds:
-			url_params.append('devicesIds=' + ",".join(str(devicesIds)))
+			url_params.append('devicesIds=' + ",".join(map(str, devicesIds)))
 		if firstSeen:
 			url_params.append('firstSeen=' + firstSeen)
 		if hasCrashDumps:
 			url_params.append('hasCrashDumps=' + hasCrashDumps)
 		if ips:
 			url_params.append('ips=' + ",".join(str(ips)))
 		if itemsPerPage:
@@ -2541,21 +2667,24 @@
 	def list_cores(self, deploymentModes: list = None, hasCrashDumps: bool = None, ip: str = None, names: list = None, organization: str = None, versions: list = None) -> tuple[bool, list]:
 		'''
 		Class SystemInventory
 		Description: This API call output the list of cores.
         
 		Args:
 			deploymentModes (list): List of cores deployments modes.
+			string (list): List of cores deployments modes.
 			hasCrashDumps (bool): Has crash dumps.
 			ip (str): IP.
 			names (list): List of cores names.
+			string (list): List of cores names.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			versions (list): List of cores versions.
+			string (list): List of cores versions.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("list_cores", locals())
 
@@ -2630,16 +2759,19 @@
 	def move_collectors(self, targetCollectorGroup: str, collectorIds: list = None, collectorSIDs: list = None, collectors: list = None, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class SystemInventory
 		Description: This API call move collector between groups.
         
 		Args:
 			collectorIds (list): value = Array of collectors Ids. To move collectors from one organization to another.
+			integer (list): value = Array of collectors Ids. To move collectors from one organization to another.
 			collectorSIDs (list): value = Array of collectors SIDS. To move collectors from one organization to another.
+			string (list): value = Array of collectors SIDS. To move collectors from one organization to another.
 			collectors (list): Array of collectors names. To move collectors from one organization to another, for each collector please add the organization name before the collector name (<organization-name>\\<collector-name>).
+			string (list): Array of collectors names. To move collectors from one organization to another, for each collector please add the organization name before the collector name (<organization-name>\\<collector-name>).
 			forceAssign (bool): Indicates whether to force the assignment even if the organization of the target Collector group is under migration.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			targetCollectorGroup (str): Collector group. To move collectors from one organization to another, please add the organization name before the target collector group (<organization-name>\\<collector-group-name>).
 
 		Returns:
@@ -2647,15 +2779,15 @@
 			None: This function does not return any data.
 		'''
 		validate_params("move_collectors", locals())
 
 		url = '/management-rest/inventory/move-collectors'
 		url_params = []
 		if collectorIds:
-			url_params.append('collectorIds=' + ",".join(str(collectorIds)))
+			url_params.append('collectorIds=' + ",".join(map(str, collectorIds)))
 		if collectorSIDs:
 			url_params.append('collectorSIDs=' + ",".join(str(collectorSIDs)))
 		if collectors:
 			url_params.append('collectors=' + ",".join(str(collectors)))
 		if forceAssign:
 			url_params.append('forceAssign=' + forceAssign)
 		if organization:
@@ -2684,44 +2816,59 @@
 	def toggle_collectors(self, enable: bool, cloudAccounts: list = None, cloudProviders: list = None, clusters: list = None, collectorGroups: list = None, collectorGroupsIds: list = None, collectorType: str = None, devices: list = None, devicesIds: list = None, firstSeen: str = None, hasCrashDumps: bool = None, ips: list = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, loggedUser: str = None, operatingSystems: list = None, organization: str = None, osFamilies: list = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, states: list = None, strictMode: bool = None, versions: list = None) -> tuple[bool, str]:
 		'''
 		Class SystemInventory
 		Description: This API call enables/disables a Collector(s). You must specify whether the Collector is to be enabled or disabled.
         
 		Args:
 			cloudAccounts (list): Specifies the list cloud account names.
+			string (list): Specifies the list cloud account names.
 			cloudProviders (list): Specifies the list of cloud providers: AWS, Azure, GCP.
+			string (list): Specifies the list of cloud providers: AWS, Azure, GCP.
 			clusters (list): Specifies the list of cluster.
+			string (list): Specifies the list of cluster.
 			collectorGroups (list): Specifies the list of collector group names and retrieves collectors under the
 given groups.
+			string (list): Specifies the list of collector group names and retrieves collectors under the
+given groups.
 			collectorGroupsIds (list): Specifies the list of collector group Ids and retrieves collectors under the
 given groups.
+			integer (list): Specifies the list of collector group Ids and retrieves collectors under the
+given groups.
 			collectorType (str): Specifies the group types of the collectors. Types: All, Collector, Workloads. All by default.
 			devices (list): Specifies the list of device names.
+			string (list): Specifies the list of device names.
 			devicesIds (list): Specifies the list of device ids.
+			integer (list): Specifies the list of device ids.
 			enable (bool): Toggle enable.
 			firstSeen (str): Retrieves collectors that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			hasCrashDumps (bool): Retrieves collectors that have crash dumps.
 			ips (list): Specifies the list of IP values.
+			string (list): Specifies the list of IP values.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeenEnd (str): Retrieves collectors that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			lastSeenStart (str): Retrieves collectors that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			loggedUser (str): Specifies the user that was logged when the event occurred.
 			operatingSystems (list): Specifies the list of specific operating systems. For example, Windows 7 Pro.
+			string (list): Specifies the list of specific operating systems. For example, Windows 7 Pro.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
 .
 			osFamilies (list): Specifies the list of operating system families: Windows, Windows Server or OS X.
+			string (list): Specifies the list of operating system families: Windows, Windows Server or OS X.
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			showExpired (bool): Specifies whether to include collectors which have been disconnected for more than 30 days (sequentially) and are marked as Expired.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			states (list): Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, 
 Pending Reboot, Isolated, Expired, Migrated or Pending Migration.
+			string (list): Specifies the list of collector states: Running, Disconnected, Disabled, Degraded, 
+Pending Reboot, Isolated, Expired, Migrated or Pending Migration.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 			versions (list): Specifies the list of collector versions.
+			string (list): Specifies the list of collector versions.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			str
 		'''
 		validate_params("toggle_collectors", locals())
 
@@ -2732,21 +2879,21 @@
 		if cloudProviders:
 			url_params.append('cloudProviders=' + ",".join(str(cloudProviders)))
 		if clusters:
 			url_params.append('clusters=' + ",".join(str(clusters)))
 		if collectorGroups:
 			url_params.append('collectorGroups=' + ",".join(str(collectorGroups)))
 		if collectorGroupsIds:
-			url_params.append('collectorGroupsIds=' + ",".join(str(collectorGroupsIds)))
+			url_params.append('collectorGroupsIds=' + ",".join(map(str, collectorGroupsIds)))
 		if collectorType:
 			url_params.append('collectorType=' + collectorType)
 		if devices:
 			url_params.append('devices=' + ",".join(str(devices)))
 		if devicesIds:
-			url_params.append('devicesIds=' + ",".join(str(devicesIds)))
+			url_params.append('devicesIds=' + ",".join(map(str, devicesIds)))
 		if enable:
 			url_params.append('enable=' + enable)
 		if firstSeen:
 			url_params.append('firstSeen=' + firstSeen)
 		if hasCrashDumps:
 			url_params.append('hasCrashDumps=' + hasCrashDumps)
 		if ips:
@@ -2783,29 +2930,31 @@
 	def unisolate_collectors(self, devices: list = None, devicesIds: list = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class SystemInventory
 		Description: This API call isolate collector functionality.
         
 		Args:
 			devices (list): Specifies the list of device names.
+			string (list): Specifies the list of device names.
 			devicesIds (list): Specifies the list of device ids.
+			integer (list): Specifies the list of device ids.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("unisolate_collectors", locals())
 
 		url = '/management-rest/inventory/unisolate-collectors'
 		url_params = []
 		if devices:
 			url_params.append('devices=' + ",".join(str(devices)))
 		if devicesIds:
-			url_params.append('devicesIds=' + ",".join(str(devicesIds)))
+			url_params.append('devicesIds=' + ",".join(map(str, devicesIds)))
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
 class IoT:
 	'''The IoT module enables you to monitor the devices found in IoT scans and create/move IoT Groups.'''
@@ -2837,61 +2986,71 @@
 	def delete_devices(self, categories: list = None, devices: list = None, devicesIds: list = None, firstSeenEnd: str = None, firstSeenStart: str = None, internalIps: list = None, iotGroups: list = None, iotGroupsIds: list = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, locations: list = None, macAddresses: list = None, models: list = None, organization: str = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, strictMode: bool = None, vendors: list = None) -> tuple[bool, None]:
 		'''
 		Class IoT
 		Description: This API call deletes a IoT device(s).
         
 		Args:
 			categories (list): Specifies the list of categories values.
+			string (list): Specifies the list of categories values.
 			devices (list): Specifies the list of device names.
+			string (list): Specifies the list of device names.
 			devicesIds (list): Specifies the list of device ids.
+			integer (list): Specifies the list of device ids.
 			firstSeenEnd (str): Retrieves IoT devices that were first seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			firstSeenStart (str): Retrieves IoT devices that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			internalIps (list): Specifies the list of IP values.
+			string (list): Specifies the list of IP values.
 			iotGroups (list): Specifies the list of collector group names and retrieves collectors under the given groups.
+			string (list): Specifies the list of collector group names and retrieves collectors under the given groups.
 			iotGroupsIds (list): Specifies the list of collector group ids and retrieves collectors under the given groups.
+			integer (list): Specifies the list of collector group ids and retrieves collectors under the given groups.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeenEnd (str): Retrieves IoT devices that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			lastSeenStart (str): Retrieves IoT devices that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			locations (list): Specifies the list of locations values.
+			string (list): Specifies the list of locations values.
 			macAddresses (list): Specifies the list of mac address values.
+			string (list): Specifies the list of mac address values.
 			models (list): Specifies the list of models values.
+			string (list): Specifies the list of models values.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
 .
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			showExpired (bool): Specifies whether to include IoT devices which have been disconnected for more than 3 days (sequentially) and are marked as Expired.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 			vendors (list): Specifies the list of vendors values.
+			string (list): Specifies the list of vendors values.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("delete_devices", locals())
 
 		url = '/management-rest/iot/delete-devices'
 		url_params = []
 		if categories:
 			url_params.append('categories=' + ",".join(str(categories)))
 		if devices:
 			url_params.append('devices=' + ",".join(str(devices)))
 		if devicesIds:
-			url_params.append('devicesIds=' + ",".join(str(devicesIds)))
+			url_params.append('devicesIds=' + ",".join(map(str, devicesIds)))
 		if firstSeenEnd:
 			url_params.append('firstSeenEnd=' + firstSeenEnd)
 		if firstSeenStart:
 			url_params.append('firstSeenStart=' + firstSeenStart)
 		if internalIps:
 			url_params.append('internalIps=' + ",".join(str(internalIps)))
 		if iotGroups:
 			url_params.append('iotGroups=' + ",".join(str(iotGroups)))
 		if iotGroupsIds:
-			url_params.append('iotGroupsIds=' + ",".join(str(iotGroupsIds)))
+			url_params.append('iotGroupsIds=' + ",".join(map(str, iotGroupsIds)))
 		if itemsPerPage:
 			url_params.append('itemsPerPage=' + itemsPerPage)
 		if lastSeenEnd:
 			url_params.append('lastSeenEnd=' + lastSeenEnd)
 		if lastSeenStart:
 			url_params.append('lastSeenStart=' + lastSeenStart)
 		if locations:
@@ -2918,87 +3077,98 @@
 	def export_iot_json(self, iotDeviceIds: list, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class IoT
 		Description: This API call outputs a list of the IoT devices info.
         
 		Args:
 			iotDeviceIds (list): Specifies the list of device ids.
+			integer (list): Specifies the list of device ids.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("export_iot_json", locals())
 
 		url = '/management-rest/iot/export-iot-json'
 		url_params = []
 		if iotDeviceIds:
-			url_params.append('iotDeviceIds=' + ",".join(str(iotDeviceIds)))
+			url_params.append('iotDeviceIds=' + ",".join(map(str, iotDeviceIds)))
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.get(url)
 
 	def list_iot_devices(self, categories: list = None, devices: list = None, devicesIds: list = None, firstSeenEnd: str = None, firstSeenStart: str = None, internalIps: list = None, iotGroups: list = None, iotGroupsIds: list = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, locations: list = None, macAddresses: list = None, models: list = None, organization: str = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, strictMode: bool = None, vendors: list = None) -> tuple[bool, list]:
 		'''
 		Class IoT
 		Description: This API call outputs a list of the IoT devices in the system. Use the input parameters to filter the list.
         
 		Args:
 			categories (list): Specifies the list of categories values.
+			string (list): Specifies the list of categories values.
 			devices (list): Specifies the list of device names.
+			string (list): Specifies the list of device names.
 			devicesIds (list): Specifies the list of device ids.
+			integer (list): Specifies the list of device ids.
 			firstSeenEnd (str): Retrieves IoT devices that were first seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			firstSeenStart (str): Retrieves IoT devices that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			internalIps (list): Specifies the list of IP values.
+			string (list): Specifies the list of IP values.
 			iotGroups (list): Specifies the list of collector group names and retrieves collectors under the given groups.
+			string (list): Specifies the list of collector group names and retrieves collectors under the given groups.
 			iotGroupsIds (list): Specifies the list of collector group ids and retrieves collectors under the given groups.
+			integer (list): Specifies the list of collector group ids and retrieves collectors under the given groups.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeenEnd (str): Retrieves IoT devices that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			lastSeenStart (str): Retrieves IoT devices that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			locations (list): Specifies the list of locations values.
+			string (list): Specifies the list of locations values.
 			macAddresses (list): Specifies the list of mac address values.
+			string (list): Specifies the list of mac address values.
 			models (list): Specifies the list of models values.
+			string (list): Specifies the list of models values.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
 .
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			showExpired (bool): Specifies whether to include IoT devices which have been disconnected for more than 3 days (sequentially) and are marked as Expired.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 			vendors (list): Specifies the list of vendors values.
+			string (list): Specifies the list of vendors values.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("list_iot_devices", locals())
 
 		url = '/management-rest/iot/list-iot-devices'
 		url_params = []
 		if categories:
 			url_params.append('categories=' + ",".join(str(categories)))
 		if devices:
 			url_params.append('devices=' + ",".join(str(devices)))
 		if devicesIds:
-			url_params.append('devicesIds=' + ",".join(str(devicesIds)))
+			url_params.append('devicesIds=' + ",".join(map(str, devicesIds)))
 		if firstSeenEnd:
 			url_params.append('firstSeenEnd=' + firstSeenEnd)
 		if firstSeenStart:
 			url_params.append('firstSeenStart=' + firstSeenStart)
 		if internalIps:
 			url_params.append('internalIps=' + ",".join(str(internalIps)))
 		if iotGroups:
 			url_params.append('iotGroups=' + ",".join(str(iotGroups)))
 		if iotGroupsIds:
-			url_params.append('iotGroupsIds=' + ",".join(str(iotGroupsIds)))
+			url_params.append('iotGroupsIds=' + ",".join(map(str, iotGroupsIds)))
 		if itemsPerPage:
 			url_params.append('itemsPerPage=' + itemsPerPage)
 		if lastSeenEnd:
 			url_params.append('lastSeenEnd=' + lastSeenEnd)
 		if lastSeenStart:
 			url_params.append('lastSeenStart=' + lastSeenStart)
 		if locations:
@@ -3048,88 +3218,99 @@
 	def move_iot_devices(self, iotDeviceIds: list, targetIotGroup: str, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class IoT
 		Description: This API call move IoT devices between groups.
         
 		Args:
 			iotDeviceIds (list): Array of IoT device ids.
+			integer (list): Array of IoT device ids.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			targetIotGroup (str): IoT target group name.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("move_iot_devices", locals())
 
 		url = '/management-rest/iot/move-iot-devices'
 		url_params = []
 		if iotDeviceIds:
-			url_params.append('iotDeviceIds=' + ",".join(str(iotDeviceIds)))
+			url_params.append('iotDeviceIds=' + ",".join(map(str, iotDeviceIds)))
 		if organization:
 			url_params.append('organization=' + organization)
 		if targetIotGroup:
 			url_params.append('targetIotGroup=' + targetIotGroup)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.insert(url)
 
 	def rescan_iot_device_details(self, categories: list = None, devices: list = None, devicesIds: list = None, firstSeenEnd: str = None, firstSeenStart: str = None, internalIps: list = None, iotGroups: list = None, iotGroupsIds: list = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, locations: list = None, macAddresses: list = None, models: list = None, organization: str = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, strictMode: bool = None, vendors: list = None) -> tuple[bool, str]:
 		'''
 		Class IoT
 		Description: This API call device details scan on IoT device(s).
         
 		Args:
 			categories (list): Specifies the list of categories values.
+			string (list): Specifies the list of categories values.
 			devices (list): Specifies the list of device names.
+			string (list): Specifies the list of device names.
 			devicesIds (list): Specifies the list of device ids.
+			integer (list): Specifies the list of device ids.
 			firstSeenEnd (str): Retrieves IoT devices that were first seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			firstSeenStart (str): Retrieves IoT devices that were first seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			internalIps (list): Specifies the list of IP values.
+			string (list): Specifies the list of IP values.
 			iotGroups (list): Specifies the list of collector group names and retrieves collectors under the given groups.
+			string (list): Specifies the list of collector group names and retrieves collectors under the given groups.
 			iotGroupsIds (list): Specifies the list of collector group ids and retrieves collectors under the given groups.
+			integer (list): Specifies the list of collector group ids and retrieves collectors under the given groups.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			lastSeenEnd (str): Retrieves IoT devices that were last seen before the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			lastSeenStart (str): Retrieves IoT devices that were last seen after the value assigned to this date. Date Format: yyyy-MM-dd HH:mm:ss.
 			locations (list): Specifies the list of locations values.
+			string (list): Specifies the list of locations values.
 			macAddresses (list): Specifies the list of mac address values.
+			string (list): Specifies the list of mac address values.
 			models (list): Specifies the list of models values.
+			string (list): Specifies the list of models values.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations.
 .
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			showExpired (bool): Specifies whether to include IoT devices which have been disconnected for more than 3 days (sequentially) and are marked as Expired.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
 			strictMode (bool): A true/false parameter indicating whether to perform strict matching on the search parameters. The default is False.
 			vendors (list): Specifies the list of vendors values.
+			string (list): Specifies the list of vendors values.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			str
 		'''
 		validate_params("rescan_iot_device_details", locals())
 
 		url = '/management-rest/iot/rescan-iot-device-details'
 		url_params = []
 		if categories:
 			url_params.append('categories=' + ",".join(str(categories)))
 		if devices:
 			url_params.append('devices=' + ",".join(str(devices)))
 		if devicesIds:
-			url_params.append('devicesIds=' + ",".join(str(devicesIds)))
+			url_params.append('devicesIds=' + ",".join(map(str, devicesIds)))
 		if firstSeenEnd:
 			url_params.append('firstSeenEnd=' + firstSeenEnd)
 		if firstSeenStart:
 			url_params.append('firstSeenStart=' + firstSeenStart)
 		if internalIps:
 			url_params.append('internalIps=' + ",".join(str(internalIps)))
 		if iotGroups:
 			url_params.append('iotGroups=' + ",".join(str(iotGroups)))
 		if iotGroupsIds:
-			url_params.append('iotGroupsIds=' + ",".join(str(iotGroupsIds)))
+			url_params.append('iotGroupsIds=' + ",".join(map(str, iotGroupsIds)))
 		if itemsPerPage:
 			url_params.append('itemsPerPage=' + itemsPerPage)
 		if lastSeenEnd:
 			url_params.append('lastSeenEnd=' + lastSeenEnd)
 		if lastSeenStart:
 			url_params.append('lastSeenStart=' + lastSeenStart)
 		if locations:
@@ -3185,14 +3366,15 @@
 	def delete_ip_set(self, ipSets: list, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class IPsets
 		Description: This API delete IP sets from the system. Use the input parameters to filter organization.
         
 		Args:
 			ipSets (list): Specifies the list of IP name to delete.
+			string (list): Specifies the list of IP name to delete.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
@@ -3479,14 +3661,15 @@
 	def assign_collector_group(self, collectorGroupNames: list, policyName: str, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Playbookspolicies
 		Description: Assign collector group to air policy.
         
 		Args:
 			collectorGroupNames (list): Specifies the list of collector group names.
+			string (list): Specifies the list of collector group names.
 			forceAssign (bool): Indicates whether to force the assignment even if the group is assigned to similar policies.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			policyName (str): Specifies policy name.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
@@ -3645,14 +3828,15 @@
 	def assign_collector_group(self, collectorsGroupName: list, policyName: str, forceAssign: bool = None, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Policies
 		Description: Assign collector group to policy.
         
 		Args:
 			collectorsGroupName (list): Specifies the list of collector group names.
+			string (list): Specifies the list of collector group names.
 			forceAssign (bool): Indicates whether to force the assignment even if the group is assigned to similar policies.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			policyName (str): Specifies security policy name.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
@@ -3727,18 +3911,20 @@
 		Class Policies
 		Description: Scan Files.
         
 		Args:
 			applyRecursiveScan (bool): Specifies if execution includes recursive scan.
 			executableFilesOnly (bool): Specifies if execution includes only files.
 			filePaths (list): Specifies file path.
+			string (list): Specifies file path.
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			origin (str): Specifies scan origin.
 			scanBy (str): Specifies scan by choice.
 			scanSelection (list): Specifies scan selection.
+			string (list): Specifies scan selection.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("scan_files", locals())
 
@@ -3918,15 +4104,17 @@
 	def list_system_events(self, componentNames: list = None, componentTypes: list = None, fromDate: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, sorting: str = None, strictMode: bool = None, toDate: str = None) -> tuple[bool, list]:
 		'''
 		Class SystemEvents
 		Description: Retrieve system events.
         
 		Args:
 			componentNames (list):  Specifies one or more names. The name is the customer name for license-related system events and the device name for all others events.
+			string (list):  Specifies one or more names. The name is the customer name for license-related system events and the device name for all others events.
 			componentTypes (list): Specifies one or more component type.
+			string (list): Specifies one or more component type.
 			fromDate (str): Searches for system events that occurred after this date.
 			itemsPerPage (int): An integer used for paging that indicates the number of collectors to retrieve forthe current page. The default is 100. The maximum value is 1,000.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			pageNumber (int): An integer used for paging that indicates the required page number.
 			sorting (str): Specifies a list of strings in JSON format representing the fields by which to sort the results in the following format: %7B"column1":true, "column2":false%7D. True indicates to sort in descending order.Results are sorted by the first field, then by the second field and so on.
@@ -4145,14 +4333,15 @@
 		'''
 		Class ThreatHuntingExclusions
 		Description: Free-text search of exclusions.
         
 		Args:
 			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
 			os (list): OS identifiers list..
+			string (list): OS identifiers list..
 			searchText (str): The free text search string. The API will return every exclusion list that contains this string, or contains an exclusion with any field that contains it..
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("exclusions_search", locals())
@@ -4414,17 +4603,20 @@
 		Args:
 			deleteAll (bool): A true/false parameter indicating whether all queries should be deleted. False by default.
 			deleteFromCommunity (bool): A true/false parameter indicating if whether to delete a query from the FortiEDR Community also.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			queryIds (list): Specifies the query IDs list.
+			integer (list): Specifies the query IDs list.
 			queryNames (list): Specifies the query names list.
+			string (list): Specifies the query names list.
 			scheduled (bool): A true/false parameter indicating whether the query is scheduled.
 			source (list): Specifies the query source list.
+			string (list): Specifies the query source list.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("delete_saved_queries", locals())
 
@@ -4433,15 +4625,15 @@
 		if deleteAll:
 			url_params.append('deleteAll=' + deleteAll)
 		if deleteFromCommunity:
 			url_params.append('deleteFromCommunity=' + deleteFromCommunity)
 		if organization:
 			url_params.append('organization=' + organization)
 		if queryIds:
-			url_params.append('queryIds=' + ",".join(str(queryIds)))
+			url_params.append('queryIds=' + ",".join(map(str, queryIds)))
 		if queryNames:
 			url_params.append('queryNames=' + ",".join(str(queryNames)))
 		if scheduled:
 			url_params.append('scheduled=' + scheduled)
 		if source:
 			url_params.append('source=' + ",".join(str(source)))
 		url += '?' + '&'.join(url_params)
@@ -4453,28 +4645,30 @@
 		Description: This API deletes the saved queries tags.
         
 		Args:
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			tagIds (list): Specifies the tag ID list.
+			integer (list): Specifies the tag ID list.
 			tagNames (list): Specifies the tag name list.
+			string (list): Specifies the tag name list.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("delete_tags", locals())
 
 		url = '/management-rest/threat-hunting/delete-tags'
 		url_params = []
 		if organization:
 			url_params.append('organization=' + organization)
 		if tagIds:
-			url_params.append('tagIds=' + ",".join(str(tagIds)))
+			url_params.append('tagIds=' + ",".join(map(str, tagIds)))
 		if tagNames:
 			url_params.append('tagNames=' + ",".join(str(tagNames)))
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.delete(url)
 
 	def facets(self, accountId: int = None, category: str = None, devices: list = None, facets: list = None, filters: list = None, fromTime: str = None, itemsPerPage: int = None, organization: str = None, pageNumber: int = None, query: str = None, sorting: list = None, time: str = None, toTime: str = None) -> tuple[bool, list]:
 		'''
@@ -4516,14 +4710,15 @@
         
 		Args:
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			scheduled (bool): A true/false parameter indicating whether the query is scheduled.
 			source (list): Specifies the query source list.
+			string (list): Specifies the query source list.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			list
 		'''
 		validate_params("list_saved_queries", locals())
 
@@ -4649,16 +4844,19 @@
         
 		Args:
 			markAll (bool): A true/false parameter indicating whether all queries should be marked with the same value as 'state' property. False by default.
 			organization (str): Specifies the organization. The value that you specify for this parameter indicates how the operation applies to an organization(s). Some parts of the Fortinet Endpoint Protection and Response Platform system have separate, non shared data that is organization-specific. Other parts of the system have data that is shared by all organizations. The value that you specify for the organization parameter, as described below, determines to which organization(s) an operation applies:
 ���	Exact organization name ��� Specifies the name of a specific organization. The value that you specify here must match exactly.
 ���	All organizations ��� Indicates that the operation applies to all organizations. In this case, the same data is shared by all organizations..
 			queryIds (list): Specifies the query ID list.
+			integer (list): Specifies the query ID list.
 			queryNames (list): Specifies the query name list.
+			string (list): Specifies the query name list.
 			source (list): Specifies the query source list.
+			string (list): Specifies the query source list.
 			state (bool): A true/false parameter indicating whether to save the query as enabled.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
 		validate_params("set_query_state", locals())
@@ -4666,15 +4864,15 @@
 		url = '/management-rest/threat-hunting/set-query-state'
 		url_params = []
 		if markAll:
 			url_params.append('markAll=' + markAll)
 		if organization:
 			url_params.append('organization=' + organization)
 		if queryIds:
-			url_params.append('queryIds=' + ",".join(str(queryIds)))
+			url_params.append('queryIds=' + ",".join(map(str, queryIds)))
 		if queryNames:
 			url_params.append('queryNames=' + ",".join(str(queryNames)))
 		if source:
 			url_params.append('source=' + ",".join(str(source)))
 		if state:
 			url_params.append('state=' + state)
 		url += '?' + '&'.join(url_params)
@@ -4894,14 +5092,16 @@
 			"restApi": restApi,
 			"role": role,
 			"title": title,
 			"username": username,
 		}
 		return fortiedr_connection.insert(url, userRequest)
 
+
+
 debug = None
 ssl_enabled = True
 organization = None
 api_json_params = None
 
 def validate_params(function_name, local_params):
 	global api_json_params
```

### Comparing `fortiedr-3.6.7/fortiedr.egg-info/PKG-INFO` & `fortiedr-3.6.8/fortiedr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortiedr
-Version: 3.6.7
+Version: 3.6.8
 Summary: This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.
 Author: Rafael Foster
 Author-email: Rafael Foster <rafaelgfoster@gmail.com>
 Project-URL: Homepage, https://github.com/rafaelfoster/fortiedr
 Project-URL: Issues, https://github.com/rafaelfoster/fortiedr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortiedr-3.6.7/pyproject.toml` & `fortiedr-3.6.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fortiedr"
-version = "3.6.7"
+version = "3.6.8"
 authors = [
   { name="Rafael Foster", email="rafaelgfoster@gmail.com" }
 ]
 description = "This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `fortiedr-3.6.7/setup.py` & `fortiedr-3.6.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 cur_dir = os.path.dirname(__file__)
 
 with open(f"{cur_dir}/requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="fortiedr",
-    version="3.6.7",
+    version="3.6.8",
     description="This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.",
     author="Rafael Foster",
     author_email="rafaelgfoster@gmail.com",
     project_urls={
         "GitHub": "https://github.com/rafaelfoster/fortiedr",
     },
     python_requires=">=3.8",
```

