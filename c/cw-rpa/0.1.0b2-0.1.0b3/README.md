# Comparing `tmp/cw_rpa-0.1.0b2-py3-none-any.whl.zip` & `tmp/cw_rpa-0.1.0b3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 11987 bytes, number of entries: 14
--rw-r--r--  2.0 unx      164 b- defN 24-May-28 10:20 cw_rpa/__init__.py
--rw-r--r--  2.0 unx       62 b- defN 24-May-28 09:15 cw_rpa/libraries/__init__.py
--rw-r--r--  2.0 unx      174 b- defN 24-May-28 09:15 cw_rpa/libraries/cloud/__init__.py
--rw-r--r--  2.0 unx     9996 b- defN 24-May-28 09:15 cw_rpa/libraries/cloud/pre_defined_functions.py
--rw-r--r--  2.0 unx       74 b- defN 24-May-28 09:15 cw_rpa/libraries/common/__init__.py
--rw-r--r--  2.0 unx     9914 b- defN 24-May-28 09:15 cw_rpa/libraries/common/common_functions.py
--rw-r--r--  2.0 unx    10238 b- defN 24-May-28 10:20 cw_rpa/libraries/common/http_wrapper_service.py
--rw-r--r--  2.0 unx       62 b- defN 24-May-28 09:15 cw_rpa/libraries/device/__init__.py
--rw-r--r--  2.0 unx       87 b- defN 24-May-28 09:15 cw_rpa/libraries/device/execute_powershell_script.py
--rw-rw-rw-  2.0 unx     1069 b- defN 24-May-28 12:33 cw_rpa-0.1.0b2.dist-info/LICENSE
--rw-r--r--  2.0 unx      201 b- defN 24-May-28 12:33 cw_rpa-0.1.0b2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 12:33 cw_rpa-0.1.0b2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-May-28 12:33 cw_rpa-0.1.0b2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1232 b- defN 24-May-28 12:33 cw_rpa-0.1.0b2.dist-info/RECORD
-14 files, 33372 bytes uncompressed, 9895 bytes compressed:  70.3%
+Zip file size: 9790 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      231 b- defN 24-May-29 13:38 cw_rpa/__init__.py
+-rw-r--r--  2.0 unx       62 b- defN 24-May-29 10:38 cw_rpa/libraries/__init__.py
+-rw-r--r--  2.0 unx      141 b- defN 24-May-29 13:38 cw_rpa/libraries/cloud/__init__.py
+-rw-r--r--  2.0 unx     3045 b- defN 24-May-29 13:38 cw_rpa/libraries/cloud/pre_defined_functions.py
+-rw-r--r--  2.0 unx       74 b- defN 24-May-29 10:38 cw_rpa/libraries/common/__init__.py
+-rw-r--r--  2.0 unx     7113 b- defN 24-May-29 13:38 cw_rpa/libraries/common/common_functions.py
+-rw-r--r--  2.0 unx    10328 b- defN 24-May-29 13:38 cw_rpa/libraries/common/http_wrapper_service.py
+-rw-r--r--  2.0 unx       62 b- defN 24-May-29 10:38 cw_rpa/libraries/device/__init__.py
+-rw-r--r--  2.0 unx       87 b- defN 24-May-29 10:38 cw_rpa/libraries/device/execute_powershell_script.py
+-rw-rw-rw-  2.0 unx     1069 b- defN 24-May-29 14:21 cw_rpa-0.1.0b3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      201 b- defN 24-May-29 14:21 cw_rpa-0.1.0b3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-29 14:21 cw_rpa-0.1.0b3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-May-29 14:21 cw_rpa-0.1.0b3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1232 b- defN 24-May-29 14:21 cw_rpa-0.1.0b3.dist-info/RECORD
+14 files, 23744 bytes uncompressed, 7698 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: cw_rpa/libraries/device/__init__.py
 Comment: 
 
 Filename: cw_rpa/libraries/device/execute_powershell_script.py
 Comment: 
 
-Filename: cw_rpa-0.1.0b2.dist-info/LICENSE
+Filename: cw_rpa-0.1.0b3.dist-info/LICENSE
 Comment: 
 
-Filename: cw_rpa-0.1.0b2.dist-info/METADATA
+Filename: cw_rpa-0.1.0b3.dist-info/METADATA
 Comment: 
 
-Filename: cw_rpa-0.1.0b2.dist-info/WHEEL
+Filename: cw_rpa-0.1.0b3.dist-info/WHEEL
 Comment: 
 
-Filename: cw_rpa-0.1.0b2.dist-info/top_level.txt
+Filename: cw_rpa-0.1.0b3.dist-info/top_level.txt
 Comment: 
 
-Filename: cw_rpa-0.1.0b2.dist-info/RECORD
+Filename: cw_rpa-0.1.0b3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cw_rpa/__init__.py

```diff
@@ -1,5 +1,6 @@
 # __init__.py is used to mark a directory as a Python package
 
 from .libraries.common.http_wrapper_service import CWHTTPRequest
+from .libraries.common import BotUtils, BotExecutor
+from .libraries.cloud import create_new_o365_user
 
-__all__ = ['Bot', 'CWHTTPRequest']
```

## cw_rpa/libraries/cloud/__init__.py

```diff
@@ -1,3 +1,3 @@
 #__init__.py is used to mark a directory as a Python package
-from cw_rpa.libraries.cloud.pre_defined_functions import list_resource_mailbox_properties, create_new_o365_user
+from cw_rpa.libraries.cloud.pre_defined_functions import  create_new_o365_user
```

## cw_rpa/libraries/cloud/pre_defined_functions.py

```diff
@@ -1,183 +1,53 @@
 # Package contains Pre defined functions, which partners can call this by passing inputs
 
 
 # system and internal libaries
 from cw_rpa.libraries.common import BotUtils
+from cw_rpa.libraries.common.http_wrapper_service import CWHTTPRequest
 import subprocess
 from types import SimpleNamespace
 import re
 import requests
 import json
 import os
 
 
-# Helps to fetch the resource mailbox properties
-def list_resource_mailbox_properties(resource_Mailbox_Name):
-    """
-    Objective: 
-        Fetches properties of a resource mailbox.
-
-    Parameters:
-        resource_Mailbox_Name (str): The name of the resource mailbox.
-
-    Description: 
-        This function fetches various properties of the specified resource mailbox,
-        such as its display name, alias, primary SMTP address, resource type, etc.
-    """
-    try:
-        
-        token = BotUtils.generate_access_token()
-
-        try:
-            default_domain = BotUtils.get_default_domain(token.access_token_for_graph)
-            powershell_command = f"""
-            $default_domain = '{default_domain}'
-            $resource_Mailbox_Name = '{resource_Mailbox_Name}'
-            try {{
-            Connect-ExchangeOnline -AccessToken {token.access_token_for_exchange_online} -Organization  $default_domain -ErrorAction Stop -WarningAction SilentlyContinue -ShowBanner:$false
-            function fetch_resource_mailbox_properties {{
-                param (
-                    [string]$mailbox_name
-                )
-
-                # Search for the mailbox in the 'roommailbox' category
-                $roomMailbox = Get-Mailbox -RecipientTypeDetails roommailbox -Identity $mailbox_name -ErrorAction SilentlyContinue
-
-                # If not found, search in the 'Equipment' category
-                if (-not $roomMailbox) {{
-                    $roomMailbox = Get-Mailbox -RecipientTypeDetails Equipment -Identity $mailbox_name -ErrorAction SilentlyContinue
-                }}
-
-                # If still not found, display an error message and exit the script
-                if (-not $roomMailbox) {{
-                    Write-Output "[MSG: Resource mailbox not found. Kindly confirm the name '$mailbox_name']"
-                    return
-                }}
-
-                # Initialize an output string
-                $output = @()
-                $ErrorActionPreference = 'SilentlyContinue'
-
-                # Add mailbox properties to the output
-                $output += "Mailbox General Properties:"
-                $output += "-------------------"
-                $output += "DisplayName: $($roomMailbox.DisplayName)"
-                $output += "Alias: $($roomMailbox.Alias)"
-                $output += "PrimarySMTPAddress: $($roomMailbox.PrimarySmtpAddress)"
-                $output += "ResourceType: $($roomMailbox.ResourceType)"
-                $output += "RoomMailboxAccountEnabled: $($roomMailbox.RoomMailboxAccountEnabled)"
-                $output += "UserPrincipalName: $($roomMailbox.UserPrincipalName)"
-                $output += "Hide from Global Address List:$($roomMailbox.HiddenFromAddressListsEnabled)"
-                $output += ""
-                $output += "Mailbox Delegate Properties:"
-                $output += "-------------------"
-                $calendarProcessing = Get-CalendarProcessing -Identity $roomMailbox
-                $output += "Accept booking request automatically: $($calendarProcessing.AutomateProcessing)"
-                $output += "Delegate who can accept or decline booking requests: $($calendarProcessing.ResourceDelegates|Get-User|select displayname)"
-                $output += "Remove organizer name from subject : $($calendarProcessing.AddOrganizerToSubject)"
-                $output += ""
-                $output += "Mailbox Booking Properties:"
-                $output += "-------------------"
-                $calendarProcessing = Get-CalendarProcessing -Identity $roomMailbox
-                $output += "Allow repeated meetings: $($calendarProcessing.AllowRecurringMeetings)"
-                $output += "Allow scheduling only during working hours: $($calendarProcessing.ScheduleOnlyDuringWorkHours)"
-                $output += "Automatically decline meetings outside this limit:"
-                $output += "Booking window (days): $($calendarProcessing.BookingWindowInDays)"
-                $output += "Maximum duration(hours):$(($calendarProcessing.MaximumDurationInMinutes)/60)"
-                $output += "ProcessExternalMeetingMessages: $($calendarProcessing.ProcessExternalMeetingMessages)"
-                $output += "Automatically delete Canceled meetings: $($calendarProcessing.RemoveCanceledMeetings)"
-                $output += "Meeting organizer to receive a reply text: $($calendarProcessing.AdditionalResponse)"
-                $output += ""
-                # Add mailbox permissions to the output
-                $output += "Mailbox Permissions:"
-                $output += "-------------------"
-                $output += "Full Access permission:"
-                $roomMailboxPermissions = Get-MailboxPermission -Identity $roomMailbox | select Identity, User 
-                $output += $roomMailboxPermissions #| Format-Table -AutoSize
-                $output += ""
-                # Add recipient permissions to the output
-                $output += "Send As permission:"
-                #$output += "-------------------"
-                $recipientPermissions = Get-RecipientPermission -Identity $roomMailbox | select Identity, @{{E = {{ $_.Trustee }}; L = "User" }}
-                $output += $recipientPermissions #| Format-Table -AutoSize 
-                $output += ""
-                $output += "Send on Behalf of permission :"
-                #$output += "-------------------"
-                $recipientPermissions = Get-Mailbox -Identity $roomMailbox | select -ExpandProperty GrantSendonBehalfTo | Get-User | select displayname | Out-String
-                $output += $recipientPermissions #| Format-Table -AutoSize
-                $output += "-------------------"
-                # Display the formatted output
-                $output
-            }}
-            $result = fetch_resource_mailbox_properties -mailbox_name $resource_Mailbox_Name
-            $result | Out-String
-
-            }} catch {{
-                Write-Output "[ERROR : An error occurred: $($_.Exception.Message)]"
-            }}
-            finally {{Disconnect-ExchangeOnline -Confirm:$false}}
-            """
-            process = subprocess.Popen(
-                ["pwsh", "-command", powershell_command],
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-                text=True,
-            )
-            output, _ = process.communicate()
-            # Check if the error message is present in the command output
-            if "ERROR" in output:
-                BotUtils.log_error(f"Error processing the request:{output}")
-                return False
-            else:
-                BotUtils.log_result(f"Result:{output}")
-                return True
-
-        except Exception as e:
-            BotUtils.log_error(f"error occurred: {str(e)}")
-            return False
-
-    except Exception as e:
-            BotUtils.log_error(f"{e}")
-            return False
-    
 # Helps to create user on 0365
 def create_new_o365_user(userPrincipalName, displayName, userPassword):
     """
     Objective: 
         Creates user on o365
 
     Parameters:
         userPrincipalName : The principal name of the user.
         displayName : The display name of the user.
         password : Password for the user(Strong password recommended).
     Description: 
         This function creates user on o365 
     """
     try:
-        token = BotUtils.generate_access_token()
-        access_token = token.access_token_for_graph
+        req = CWHTTPRequest()
         try:
             endpoint = "https://graph.microsoft.com/v1.0/users"
             headers = {
-                "Authorization": f"Bearer {access_token}",
                 "Content-Type": "application/json",
             }
             req_body = {
                 "accountEnabled": True,
                 "userPrincipalName": userPrincipalName,
                 "mailNickname": re.sub(r"[^a-zA-Z0-9]", "", userPrincipalName),
                 "displayName": displayName,
                 "passwordProfile": {
                     "forceChangePasswordNextSignIn": True,
                     "password": userPassword,
                 },
             }
             data = json.dumps(req_body)
-            response = requests.post(url=endpoint, headers=headers, data=data)
+            response = req.post(url=endpoint, headers=headers, data=data)
 
             if response.status_code == 201:
                 response = response.json()
 
                 #BotUtils.log_result(f"User '{response['userPrincipalName']}' has been successfully created.")
                 return True
```

## cw_rpa/libraries/common/common_functions.py

```diff
@@ -17,20 +17,23 @@
 
     @staticmethod
     def fetch_input_data() -> dict:
         with open("input.json", "r") as file:
             data = json.load(file)
 
             # Store sensitive inputs as class attributes
-            BotUtils.__cwEndpoint = data.get('cwEndpoint')
-            BotUtils.__cwProductId_connectionId = data.get('cwProductId_connectionId')
-            BotUtils.__cwTenantId = data.get('cwTenantId')
+            BotUtils.__cwOpenAPIClientId = data.get('cwOpenAPIClientId')
+            BotUtils.__cwOpenAPIClientSecret = data.get('cwOpenAPIClientSecret')
+            BotUtils.__cwCompanyId = data.get('cwCompanyId')
+            BotUtils.__cwSiteId = data.get('cwSiteId')
+            BotUtils.__cwPartnerAPIScope = data.get('cwPartnerAPIScope')
+            BotUtils.__cwOpenAPIURL = data.get('cwOpenAPIURL')
 
             # Exclude sensitive inputs from being exposed
-            filtered_data = {key: value for key, value in data.items() if key not in ['cwEndpoint', 'cwProductId_connectionId', 'cwTenantId']}
+            filtered_data = {key: value for key, value in data.items() if key not in ['cwOpenAPIClientId', 'cwOpenAPIClientSecret', 'cwCompanyId','cwSiteId','cwPartnerAPIScope','cwOpenAPIURL']}
             return SimpleNamespace(**filtered_data)
     
     @staticmethod
     def __log_result_internal(
         msg: str = "",
         is_json_only: bool = False,
         msg_level: str = None,
@@ -103,18 +106,16 @@
         if BotUtils.__json_response is None:
             BotUtils.__json_response = {"status": "", "messages": [], "data": []}
 
         if status is not None:
             BotUtils.__json_response["status"] = status
 
         if msg and msg_level:
-            BotUtils.__json_response["messages"].append(
-                {"level": msg_level, "message": msg}
-            )
-   
+            BotUtils.__json_response["messages"].append({"level": msg_level, "message": {"default":{"en-US":msg}}})
+
     @staticmethod
     def get_default_domain(access_token_for_graph):
         try:
             headers = {
                 "Authorization": f"Bearer {access_token_for_graph}",
                 "Content-Type": "application/json",
             }
@@ -132,49 +133,14 @@
 
             return None  # Return None if default domain not found
         except Exception as e:
             print(f"Error occurred while fetching default domain: {str(e)}")
             return None
 
     @staticmethod
-    def __acquire_access_token_from_extensibility(
-        cwEndpoint: str, cwProductId_connectionId: str, cwTenantId: str, Scopes: list
-    ):
-        try:
-            # first refresh token
-            refresh_token_URL = f"{cwEndpoint}/third-party-integration/v1/oauth/{cwProductId_connectionId}/token"
-            res = requests.get(refresh_token_URL)
-            res.raise_for_status()
-            res_json = res.json()
-            refresh_token = res_json["refresh_token"]
-            # access tokens here
-            access_token_URL = f"{cwEndpoint}/third-party-integration/v1/oauth/{cwProductId_connectionId}/customer/{cwTenantId}/authorize"
-            req_json = {
-                "grant_type": "refresh_token",
-                "scope": "*",
-                "resource_list": Scopes,
-                "refresh_token": refresh_token,
-            }
-            res = requests.post(url=access_token_URL, json=req_json)
-            res.raise_for_status()
-            return res.json()
-        except Exception as e:
-            raise Exception(f"Error while aquiring access token: {e}")
-
-    @staticmethod
-    def __extract_access_token(tokens, scope="https://graph.microsoft.com"):
-        if "resource_tokens" not in tokens:
-            return None
-
-        for token in tokens["resource_tokens"]:
-            if token["resource"] == scope:
-                return token["access_token"]
-        return None
-
-    @staticmethod
     def log_result(msg):
         # BotUtils.__log_result_internal(f"{msg}")
         BotUtils.__log_result_internal(
             msg=msg,
             is_json_only=False,
             msg_level="success",
             status="Success",
@@ -199,51 +165,15 @@
             for message in BotUtils.__json_response["messages"]
         )
         BotUtils.__json_response["status"] = "Failed" if has_error else "Success"
         output_dir = os.path.join(os.getcwd(), "Output")
         result_json_path = os.path.join(output_dir, "result.json")
         with open(result_json_path, "w") as result_json_file:
             json.dump(BotUtils.__json_response, result_json_file, indent=4)
-
-    @staticmethod
-    def generate_access_token():
-        try:
-            if (
-                not BotUtils.__cwEndpoint
-                or not BotUtils.__cwProductId_connectionId
-                or not BotUtils.__cwTenantId
-            ):
-                BotUtils.log_error(
-                    "[Error : Unable to process the request kindly check Client ID, Client Secret and Tenant ID]"
-                )
-                return False
-
-            scopes = ["https://graph.microsoft.com", "https://outlook.office365.com"]
-
-            tokens: dict = BotUtils.__acquire_access_token_from_extensibility(
-                cwEndpoint=BotUtils.__cwEndpoint,
-                cwProductId_connectionId=BotUtils.__cwProductId_connectionId,
-                cwTenantId=BotUtils.__cwTenantId,
-                Scopes=scopes,
-            )
-
-            access_token_for_exchange_online = BotUtils.__extract_access_token(
-                tokens=tokens, scope="https://outlook.office365.com"
-            )
-            access_token_for_graph = BotUtils.__extract_access_token(
-                tokens=tokens, scope="https://graph.microsoft.com"
-            )
-
-            return SimpleNamespace(
-                access_token_for_exchange_online=access_token_for_exchange_online,
-                access_token_for_graph=access_token_for_graph,
-            )
-        except Exception as e:
-            BotUtils.log_error(f"{e}")
-
+   
 # Executor and perform initial setups
 class BotExecutor:
     
     @staticmethod
     def create_out_dir(output_dir="Output"):
         try:
 
@@ -267,14 +197,9 @@
             else:
                 raise Exception(
                     "Error while creating Output folder/removing output files"
                 )
 
     @staticmethod
     def initialize():
-        BotExecutor.check_python_version()
         BotExecutor.create_out_dir()
 
-    @staticmethod
-    def check_python_version():
-        if sys.version_info < (3, 10):
-            raise Exception("Python version should be 3.6 or higher")
```

## cw_rpa/libraries/common/http_wrapper_service.py

```diff
@@ -21,15 +21,15 @@
 """
 
 
 import os
 import json
 import datetime
 import requests
-from urllib.parse import urlparse,urljoin
+from urllib.parse import urlparse, urljoin
 
 
 class CWHTTPRequestHelper:
 
     """_summary_
     integration_map: dict
         A dictionary containing the integration map
@@ -80,32 +80,34 @@
         if not self.__cw_open_api_client_secret:
             raise ValueError('"cwOpenAPIClientSecret" not found.')
         if not self.__cw_company_id:
             raise ValueError('"cwCompanyId" not found.')
         if not self.__cw_site_id:
             raise ValueError('"cwSiteId" not found.')
         if not self.__cw_patner_api_scope:
-            raise ValueError('"cwPartnerAPIScope" not found in the "input.json" file.')
+            raise ValueError(
+                '"cwPartnerAPIScope" not found in the "input.json" file.')
         if not self.__cw_open_api_url:
-            raise ValueError('"cwOpenAPIURL" not found. in the "input.json" file.')
-        
+            raise ValueError(
+                '"cwOpenAPIURL" not found. in the "input.json" file.')
+
     def __fetch_input_data(self, input_file: str = 'input.json'):
 
         if not os.path.exists(input_file):
             raise FileNotFoundError('"input.json" file not found.')
 
         with open(input_file, 'r') as f:
             try:
                 data = json.load(f)
             except json.JSONDecodeError as jsde:
                 raise jsde('input.json is not in correct format.')
             return data
 
     def acquire_access_token(self) -> str:
-        url = urljoin(self.__cw_open_api_url,"/v1/token") 
+        url = urljoin(self.__cw_open_api_url, "/v1/token")
         scopes = " ".join(self.__cw_patner_api_scope)
         data = {
             "grant_type": "client_credentials",
             "client_id": self.__cw_open_api_client_id,
             "client_secret": self.__cw_open_api_client_secret,
             "scope": scopes
         }
@@ -156,54 +158,57 @@
                 "method": "string",
                 "url": "string",
                 "body": "string",
                 "clientId": "string",  # cwCompanyId to be passed here
                 "siteId": "string"  # cwSiteId to be passed here
             }
         """
-        _proxy_url: str = urljoin(self.__cw_open_api_url, self._routes.get('open_api_rpa_ms_proxy'))
+        _proxy_url: str = urljoin(
+            self.__cw_open_api_url, self._routes.get('open_api_rpa_ms_proxy'))
         parsed_url: str = urlparse(url)
         base_url: str = f"{parsed_url.scheme}://{parsed_url.netloc}".lower()
         # url_path: str = url.split(base_url)[-1]
         integration_name: str = self.__integration_map_reversed.get(
             base_url, None)
 
         if not integration_name:
             raise ValueError('Integration name not found.')
 
         resource_list: list = []
         resource_list.append(base_url)
-        
+
         req_body: dict = {
             "integrationName": integration_name,
             "connectionId": self.__connection_id,
             "method": method.upper(),
             "resourceList": resource_list,
             "url": url,
             "clientId": self.__cw_company_id,  # cwCompanyId to be passed here
             "siteId": self.__cw_site_id  # cwSiteId to be passed here
         }
-        
+
         data = kwargs.get('data', None)
         if data:
-            req_body['body'] = data
+            req_body['body'] = json.loads(data)
 
         body_as_json_dict = kwargs.get('json', None)
         if body_as_json_dict:
             req_body['body'] = body_as_json_dict
 
+        kwargs["data"] = json.dumps(req_body)
         kwargs = self._add_authorization_header_to_kwargs(kwargs)
-        return requests.request('POST', url=_proxy_url, json=req_body, **kwargs)
+        return requests.request('POST', url=_proxy_url, **kwargs)
 
     def _open_api_request(self, method, url, **kwargs) -> requests.Response:
         kwargs = self._add_authorization_header_to_kwargs(kwargs)
         response = requests.request(method, url, **kwargs)
         return response
 
     def request(self, method, url, **kwargs) -> requests.Response:
+        print(kwargs)
         parsed_url: str = urlparse(url)
         base_url: str = f"{parsed_url.scheme}://{parsed_url.netloc}".lower()
         open_api_base_url: str = self.__cw_open_api_url.lower()
 
         if base_url == open_api_base_url:
             # open api requests
             response = self._open_api_request(method, url, **kwargs)
@@ -236,15 +241,15 @@
 
     def request(self, method, url, **kwargs):
         return self.__request_helper.request(method, url=url, **kwargs)
 
     def get(self, url, params=None, **kwargs):
         return self.__request_helper.request(method='GET', url=url, params=params, **kwargs)
 
-    def post(self, url, data=None, json: dict = None, **kwargs):
+    def post(self, url, data = None, json: dict = None, **kwargs):
         return self.__request_helper.request(method='POST', url=url, data=data, json=json, **kwargs)
 
     def put(self, url, data=None, **kwargs):
         return self.__request_helper.request(method='PUT', url=url, data=data,  **kwargs)
 
     def patch(self, url,  data=None, **kwargs):
         return self.__request_helper.request(method='PATCH', url=url, data=data,  **kwargs)
@@ -253,8 +258,7 @@
         return self.__request_helper.request(method='DELETE', url=url, **kwargs)
 
     def head(self, url, **kwargs):
         return self.__request_helper.request(method='HEAD', url=url, **kwargs)
 
     def options(self, url, **kwargs):
         return self.__request_helper.request(method='OPTIONS', url=url, **kwargs)
-
```

## Comparing `cw_rpa-0.1.0b2.dist-info/LICENSE` & `cw_rpa-0.1.0b3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cw_rpa-0.1.0b2.dist-info/RECORD` & `cw_rpa-0.1.0b3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-cw_rpa/__init__.py,sha256=3JsUS14ZiU40MeyvmQZDJOky8Boc8pccyc6jUZvaJPM,164
+cw_rpa/__init__.py,sha256=nWOEtSvLaKBWFP6iuSerRQtPkkoM1BnPMJA9Ncbn0HA,231
 cw_rpa/libraries/__init__.py,sha256=WilrrZVJIhPAqXlr0kjCN-RnLFZqBN-8zqLSVIvKLuQ,62
-cw_rpa/libraries/cloud/__init__.py,sha256=dOtcJwc9ktu5B-L3VWW_e6IXmfgDGAIlU-AFug70_zU,174
-cw_rpa/libraries/cloud/pre_defined_functions.py,sha256=N02BbMXJGO7MqmjhAoJUFDl5OVruzXl6zIYSxy5lXOA,9996
+cw_rpa/libraries/cloud/__init__.py,sha256=3MqRHPBIGrn15n11ZP3gQcE1SUv2pCrs0qxTOqq-B74,141
+cw_rpa/libraries/cloud/pre_defined_functions.py,sha256=MtIFxzD4BGX0roO356wSbYFdTfa8blqXEc1ITOOEHXY,3045
 cw_rpa/libraries/common/__init__.py,sha256=dc9bvhKg2b8JsW0X0zhfR4WQCoiDwXLl1jxYBblq_IE,74
-cw_rpa/libraries/common/common_functions.py,sha256=hsBo5LeQ_rgAg8XbPgFmnv9OqCo0Qg66zh-IAtCtBL0,9914
-cw_rpa/libraries/common/http_wrapper_service.py,sha256=TF79CyWlnQTw5UU5y_3-UrlYTQ1jPApp1NMkpsvYgWU,10238
+cw_rpa/libraries/common/common_functions.py,sha256=nw07RMLWDgDKGsqTbyomxAefLF5P81f_3ZBV-NJoeGo,7113
+cw_rpa/libraries/common/http_wrapper_service.py,sha256=BnMb4lebjGq8BQukOJ_OzObQNKW_n2nB2sOlh-5MeFg,10328
 cw_rpa/libraries/device/__init__.py,sha256=msCSrRE7wI_1hPOsrg6yJP_fMa2lF8Om93DP4FJnrIU,62
 cw_rpa/libraries/device/execute_powershell_script.py,sha256=bbhMj3XpQga5h7GJnBs1Cb7knNSYhzBLJe83DT8yMkM,87
-cw_rpa-0.1.0b2.dist-info/LICENSE,sha256=d9rKJUik8rJ3nRnL27kKLiFS3N-ziSVaUvP2ee6jfGs,1069
-cw_rpa-0.1.0b2.dist-info/METADATA,sha256=vp6KX6RHrtBnYfhFXay_CixgrjmdzpLyMy4UvCkQz1Q,201
-cw_rpa-0.1.0b2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-cw_rpa-0.1.0b2.dist-info/top_level.txt,sha256=eCMQTVi9G0JQTesbEbLv4eeEQZHiGEBnZVWOPriLn3c,7
-cw_rpa-0.1.0b2.dist-info/RECORD,,
+cw_rpa-0.1.0b3.dist-info/LICENSE,sha256=d9rKJUik8rJ3nRnL27kKLiFS3N-ziSVaUvP2ee6jfGs,1069
+cw_rpa-0.1.0b3.dist-info/METADATA,sha256=jkH-HQ5YwzcZXbCVpTF1HyfjTmtBrRBN2AMJUNJ9RIg,201
+cw_rpa-0.1.0b3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cw_rpa-0.1.0b3.dist-info/top_level.txt,sha256=eCMQTVi9G0JQTesbEbLv4eeEQZHiGEBnZVWOPriLn3c,7
+cw_rpa-0.1.0b3.dist-info/RECORD,,
```

