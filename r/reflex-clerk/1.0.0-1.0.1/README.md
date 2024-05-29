# Comparing `tmp/reflex_clerk-1.0.0.tar.gz` & `tmp/reflex_clerk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_clerk-1.0.0.tar", last modified: Sat May 18 00:28:11 2024, max compression
+gzip compressed data, was "reflex_clerk-1.0.1.tar", last modified: Wed May 29 00:00:53 2024, max compression
```

## Comparing `reflex_clerk-1.0.0.tar` & `reflex_clerk-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 elliot     (502) staff       (20)        0 2024-05-18 00:28:11.453594 reflex_clerk-1.0.0/
--rw-r--r--   0 elliot     (502) staff       (20)     2216 2024-05-18 00:28:11.453115 reflex_clerk-1.0.0/PKG-INFO
--rw-r--r--   0 elliot     (502) staff       (20)     1745 2024-05-18 00:24:31.000000 reflex_clerk-1.0.0/README.md
-drwxr-xr-x   0 elliot     (502) staff       (20)        0 2024-05-18 00:28:11.440497 reflex_clerk-1.0.0/custom_components/
-drwxr-xr-x   0 elliot     (502) staff       (20)        0 2024-05-18 00:28:11.442408 reflex_clerk-1.0.0/custom_components/reflex_clerk/
--rw-r--r--   0 elliot     (502) staff       (20)      683 2024-05-17 20:13:43.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk/__init__.py
-drwxr-xr-x   0 elliot     (502) staff       (20)        0 2024-05-18 00:28:11.447652 reflex_clerk-1.0.0/custom_components/reflex_clerk/clerk_client/
--rw-r--r--   0 elliot     (502) staff       (20)        0 2024-05-15 21:42:31.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk/clerk_client/__init__.py
--rw-r--r--   0 elliot     (502) staff       (20)     9547 2024-05-16 20:11:37.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk/clerk_client/clerk_client.py
--rw-r--r--   0 elliot     (502) staff       (20)     4091 2024-05-15 21:43:15.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk/clerk_client/clerk_request_models.py
--rw-r--r--   0 elliot     (502) staff       (20)    15566 2024-05-17 23:47:04.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk/clerk_client/clerk_response_models.py
-drwxr-xr-x   0 elliot     (502) staff       (20)        0 2024-05-18 00:28:11.451950 reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/
--rw-r--r--   0 elliot     (502) staff       (20)        0 2024-05-17 03:41:58.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/__init__.py
--rw-r--r--   0 elliot     (502) staff       (20)      638 2024-05-17 23:47:21.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/appearance.py
--rw-r--r--   0 elliot     (502) staff       (20)    19967 2024-05-17 23:39:44.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/clerk_provider.py
--rw-r--r--   0 elliot     (502) staff       (20)    10359 2024-05-17 23:46:36.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/control.py
--rw-r--r--   0 elliot     (502) staff       (20)     4401 2024-05-17 23:32:43.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/reflex_clerk.py
--rw-r--r--   0 elliot     (502) staff       (20)     9150 2024-05-17 20:37:34.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/sign_in.py
--rw-r--r--   0 elliot     (502) staff       (20)     2146 2024-05-17 20:45:59.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/sign_out.py
--rw-r--r--   0 elliot     (502) staff       (20)     9201 2024-05-17 20:40:45.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/sign_up.py
--rw-r--r--   0 elliot     (502) staff       (20)     6703 2024-05-17 20:51:18.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/user.py
-drwxr-xr-x   0 elliot     (502) staff       (20)        0 2024-05-18 00:28:11.452504 reflex_clerk-1.0.0/custom_components/reflex_clerk.egg-info/
--rw-r--r--   0 elliot     (502) staff       (20)     2216 2024-05-18 00:28:11.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk.egg-info/PKG-INFO
--rw-r--r--   0 elliot     (502) staff       (20)     1017 2024-05-18 00:28:11.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk.egg-info/SOURCES.txt
--rw-r--r--   0 elliot     (502) staff       (20)        1 2024-05-18 00:28:11.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk.egg-info/dependency_links.txt
--rw-r--r--   0 elliot     (502) staff       (20)       33 2024-05-18 00:28:11.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk.egg-info/requires.txt
--rw-r--r--   0 elliot     (502) staff       (20)       13 2024-05-18 00:28:11.000000 reflex_clerk-1.0.0/custom_components/reflex_clerk.egg-info/top_level.txt
--rw-r--r--   0 elliot     (502) staff       (20)      641 2024-05-17 23:52:10.000000 reflex_clerk-1.0.0/pyproject.toml
--rw-r--r--   0 elliot     (502) staff       (20)       38 2024-05-18 00:28:11.453663 reflex_clerk-1.0.0/setup.cfg
+drwxr-xr-x   0 elliot     (502) staff       (20)        0 2024-05-29 00:00:53.127144 reflex_clerk-1.0.1/
+-rw-r--r--   0 elliot     (502) staff       (20)     2334 2024-05-29 00:00:53.126941 reflex_clerk-1.0.1/PKG-INFO
+-rw-r--r--   0 elliot     (502) staff       (20)     1745 2024-05-18 00:24:31.000000 reflex_clerk-1.0.1/README.md
+drwxr-xr-x   0 elliot     (502) staff       (20)        0 2024-05-29 00:00:53.122793 reflex_clerk-1.0.1/custom_components/
+drwxr-xr-x   0 elliot     (502) staff       (20)        0 2024-05-29 00:00:53.123310 reflex_clerk-1.0.1/custom_components/reflex_clerk/
+-rw-r--r--   0 elliot     (502) staff       (20)      683 2024-05-17 20:13:43.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk/__init__.py
+drwxr-xr-x   0 elliot     (502) staff       (20)        0 2024-05-29 00:00:53.124627 reflex_clerk-1.0.1/custom_components/reflex_clerk/clerk_client/
+-rw-r--r--   0 elliot     (502) staff       (20)        0 2024-05-15 21:42:31.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk/clerk_client/__init__.py
+-rw-r--r--   0 elliot     (502) staff       (20)     9547 2024-05-16 20:11:37.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk/clerk_client/clerk_client.py
+-rw-r--r--   0 elliot     (502) staff       (20)     4246 2024-05-28 23:58:38.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk/clerk_client/clerk_request_models.py
+-rw-r--r--   0 elliot     (502) staff       (20)    15811 2024-05-28 23:58:38.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk/clerk_client/clerk_response_models.py
+drwxr-xr-x   0 elliot     (502) staff       (20)        0 2024-05-29 00:00:53.126398 reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/
+-rw-r--r--   0 elliot     (502) staff       (20)        0 2024-05-17 03:41:58.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/__init__.py
+-rw-r--r--   0 elliot     (502) staff       (20)      655 2024-05-28 23:58:38.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/appearance.py
+-rw-r--r--   0 elliot     (502) staff       (20)    19967 2024-05-17 23:39:44.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/clerk_provider.py
+-rw-r--r--   0 elliot     (502) staff       (20)    10359 2024-05-17 23:46:36.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/control.py
+-rw-r--r--   0 elliot     (502) staff       (20)     4401 2024-05-17 23:32:43.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/reflex_clerk.py
+-rw-r--r--   0 elliot     (502) staff       (20)     9150 2024-05-17 20:37:34.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/sign_in.py
+-rw-r--r--   0 elliot     (502) staff       (20)     2146 2024-05-17 20:45:59.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/sign_out.py
+-rw-r--r--   0 elliot     (502) staff       (20)     9201 2024-05-17 20:40:45.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/sign_up.py
+-rw-r--r--   0 elliot     (502) staff       (20)     6703 2024-05-17 20:51:18.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/user.py
+drwxr-xr-x   0 elliot     (502) staff       (20)        0 2024-05-29 00:00:53.126610 reflex_clerk-1.0.1/custom_components/reflex_clerk.egg-info/
+-rw-r--r--   0 elliot     (502) staff       (20)     2334 2024-05-29 00:00:53.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk.egg-info/PKG-INFO
+-rw-r--r--   0 elliot     (502) staff       (20)     1017 2024-05-29 00:00:53.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk.egg-info/SOURCES.txt
+-rw-r--r--   0 elliot     (502) staff       (20)        1 2024-05-29 00:00:53.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk.egg-info/dependency_links.txt
+-rw-r--r--   0 elliot     (502) staff       (20)       33 2024-05-29 00:00:53.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk.egg-info/requires.txt
+-rw-r--r--   0 elliot     (502) staff       (20)       13 2024-05-29 00:00:53.000000 reflex_clerk-1.0.1/custom_components/reflex_clerk.egg-info/top_level.txt
+-rw-r--r--   0 elliot     (502) staff       (20)      740 2024-05-28 23:59:04.000000 reflex_clerk-1.0.1/pyproject.toml
+-rw-r--r--   0 elliot     (502) staff       (20)       38 2024-05-29 00:00:53.127196 reflex_clerk-1.0.1/setup.cfg
```

### Comparing `reflex_clerk-1.0.0/PKG-INFO` & `reflex_clerk-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: reflex-clerk
-Version: 1.0.0
+Version: 1.0.1
 Summary: Reflex custom component library for Clerk, a user management platform
 Author-email: Elliot Kroo <elliot@kroo.net>
 License: Apache-2.0
+Project-URL: homepage, https://kroo.github.io/reflex-clerk/
+Project-URL: source, https://github.com/kroo/reflex-clerk
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: reflex>=0.5.0
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
```

### Comparing `reflex_clerk-1.0.0/README.md` & `reflex_clerk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `reflex_clerk-1.0.0/custom_components/reflex_clerk/__init__.py` & `reflex_clerk-1.0.1/custom_components/reflex_clerk/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex_clerk-1.0.0/custom_components/reflex_clerk/clerk_client/clerk_client.py` & `reflex_clerk-1.0.1/custom_components/reflex_clerk/clerk_client/clerk_client.py`

 * *Files identical despite different names*

### Comparing `reflex_clerk-1.0.0/custom_components/reflex_clerk/clerk_client/clerk_request_models.py` & `reflex_clerk-1.0.1/custom_components/reflex_clerk/clerk_client/clerk_request_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from typing import Optional, List
 
-from pydantic import BaseModel
+from reflex.base import pydantic
 
 
-class VerifyClientRequest(BaseModel):
+class VerifyClientRequest(pydantic.BaseModel):
     token: str
 
 
-class CreateEmailAddressRequest(BaseModel):
+class CreateEmailAddressRequest(pydantic.BaseModel):
     user_id: str
     email_address: str
     verified: Optional[bool] = None
     primary: Optional[bool] = None
 
 
-class UpdateEmailAddressRequest(BaseModel):
+class UpdateEmailAddressRequest(pydantic.BaseModel):
     verified: Optional[bool] = None
     primary: Optional[bool] = None
 
 
-class CreatePhoneNumberRequest(BaseModel):
+class CreatePhoneNumberRequest(pydantic.BaseModel):
     user_id: str
     phone_number: str
     verified: Optional[bool] = None
     primary: Optional[bool] = None
     reserved_for_second_factor: Optional[bool] = None
 
 
-class UpdatePhoneNumberRequest(BaseModel):
+class UpdatePhoneNumberRequest(pydantic.BaseModel):
     verified: Optional[bool] = None
     primary: Optional[bool] = None
     reserved_for_second_factor: Optional[bool] = None
 
 
-class CreateUserRequest(BaseModel):
+class CreateUserRequest(pydantic.BaseModel):
     external_id: Optional[str] = None
     first_name: Optional[str] = None
     last_name: Optional[str] = None
     email_address: Optional[List[str]] = None
     phone_number: Optional[List[str]] = None
     web3_wallet: Optional[List[str]] = None
     username: Optional[str] = None
@@ -50,92 +50,92 @@
     backup_codes: Optional[List[str]] = None
     public_metadata: Optional[dict] = None
     private_metadata: Optional[dict] = None
     unsafe_metadata: Optional[dict] = None
     created_at: Optional[str] = None
 
 
-class UpdateUserRequest(BaseModel):
+class UpdateUserRequest(pydantic.BaseModel):
     external_id: Optional[str] = None
     first_name: Optional[str] = None
     last_name: Optional[str] = None
     primary_email_address_id: Optional[str] = None
     notify_primary_email_address_changed: Optional[bool] = None
     primary_phone_number_id: Optional[str] = None
     primary_web3_wallet_id: Optional[str] = None
     username: Optional[str] = None
     profile_image_id: Optional[str] = None
     password: Optional[str] = None
     password_digest: Optional[str] = None
     password_hasher: Optional[str] = None
 
 
-class UpsertTemplateRequest(BaseModel):
+class UpsertTemplateRequest(pydantic.BaseModel):
     name: str
     subject: Optional[str] = None
     markup: Optional[str] = None
     body: str
     delivered_by_clerk: Optional[bool] = None
     from_email_name: Optional[str] = None
     reply_to_email_name: Optional[str] = None
 
 
-class PreviewTemplateRequest(BaseModel):
+class PreviewTemplateRequest(pydantic.BaseModel):
     subject: Optional[str] = None
     body: str
     from_email_name: Optional[str] = None
     reply_to_email_name: Optional[str] = None
 
 
-class ToggleTemplateDeliveryRequest(BaseModel):
+class ToggleTemplateDeliveryRequest(pydantic.BaseModel):
     delivered_by_clerk: Optional[bool] = None
 
 
-class VerifySessionRequest(BaseModel):
+class VerifySessionRequest(pydantic.BaseModel):
     token: str
 
 
-class CreateSessionTokenFromTemplateRequest(BaseModel):
+class CreateSessionTokenFromTemplateRequest(pydantic.BaseModel):
     pass
 
 
-class GetPublicInterstitialParams(BaseModel):
+class GetPublicInterstitialParams(pydantic.BaseModel):
     frontendApi: Optional[str] = None
     publishable_key: Optional[str] = None
 
 
-class GetClientListParams(BaseModel):
+class GetClientListParams(pydantic.BaseModel):
     limit: Optional[int] = None
     offset: Optional[int] = None
 
 
-class GetSessionListParams(BaseModel):
+class GetSessionListParams(pydantic.BaseModel):
     client_id: Optional[str] = None
     user_id: Optional[str] = None
     status: Optional[str] = None
     limit: Optional[int] = None
     offset: Optional[int] = None
 
 
-class GetUserListParams(BaseModel):
+class GetUserListParams(pydantic.BaseModel):
     email_address: Optional[List[str]] = None
     phone_number: Optional[List[str]] = None
     external_id: Optional[List[str]] = None
     username: Optional[List[str]] = None
     web3_wallet: Optional[List[str]] = None
     user_id: Optional[List[str]] = None
     organization_id: Optional[List[str]] = None
     query: Optional[str] = None
     last_active_at_since: Optional[int] = None
     limit: Optional[int] = None
     offset: Optional[int] = None
     order_by: Optional[str] = None
 
 
-class GetUsersCountParams(BaseModel):
+class GetUsersCountParams(pydantic.BaseModel):
     email_address: Optional[List[str]] = None
     phone_number: Optional[List[str]] = None
     external_id: Optional[List[str]] = None
     username: Optional[List[str]] = None
     web3_wallet: Optional[List[str]] = None
     user_id: Optional[List[str]] = None
     query: Optional[str] = None
```

### Comparing `reflex_clerk-1.0.0/custom_components/reflex_clerk/clerk_client/clerk_response_models.py` & `reflex_clerk-1.0.1/custom_components/reflex_clerk/clerk_client/clerk_response_models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from typing import Optional, List, Dict, Any, Literal
 
-from pydantic import BaseModel
+from reflex.base import pydantic
 
 
-class ClerkError(BaseModel):
+class ClerkError(pydantic.BaseModel):
     """
     Represents an error response from the Clerk API.
     """
     message: str
     code: Optional[int] = None
 
 
-class DeletedObjectResponse(BaseModel):
+class DeletedObjectResponse(pydantic.BaseModel):
     """
     Represents the response for a successfully deleted object.
     """
     deleted: bool
     object: str
 
 
-class PaginationMeta(BaseModel):
+class PaginationMeta(pydantic.BaseModel):
     """
     Metadata for pagination.
     """
     total_count: int
     limit: int
     offset: int
 
 
-class Verification(BaseModel):
+class Verification(pydantic.BaseModel):
     """
     Represents the verification details of an email address or phone number.
 
     Attributes:
         strategy: The strategy pertaining to the parent sign-up or sign-in attempt.
         status: The state of the verification.
         attempts: The number of attempts related to the verification.
@@ -48,27 +48,27 @@
     nonce: Optional[str] = None
     attempts: Optional[int] = None
     expire_at: Optional[int] = None
     error: Optional[ClerkError] = None
     external_verification_redirect_url: Optional[str] = None
 
 
-class IdentificationLink(BaseModel):
+class IdentificationLink(pydantic.BaseModel):
     """
     Represents a link between an email address or phone number and another identification type.
 
     Attributes:
         type: One of "oauth_google", "oauth_mock", or "saml"
         id: A unique identifier for this link.
     """
     type: Literal["oauth_google", "oauth_mock", "saml"]
     id: str
 
 
-class EmailAddress(BaseModel):
+class EmailAddress(pydantic.BaseModel):
     """
     Represents an email address associated with a user.
 
     Attributes:
         id: A unique identifier for this email address.
         email_address: The value of this email address.
         verification: An object holding information on the verification of this email address.
@@ -82,22 +82,22 @@
     reserved: bool
     verification: Optional[Verification] = None
     linked_to: List[IdentificationLink]
     created_at: int
     updated_at: int
 
 
-class EmailAddressResponse(BaseModel):
+class EmailAddressResponse(pydantic.BaseModel):
     """
     Represents the response containing an email address.
     """
     data: EmailAddress
 
 
-class PhoneNumber(BaseModel):
+class PhoneNumber(pydantic.BaseModel):
     """
     Represents a phone number associated with a user.
 
     Attributes:
         id: A unique identifier for this phone number.
         phone_number: The value of this phone number, in [E.164 format](https://en.wikipedia.org/wiki/E.164).
         reserved_for_second_factor: Set to true if this phone number is reserved for multi-factor authentication (2FA). Set to false otherwise.
@@ -116,111 +116,111 @@
     verification: Optional[Verification] = None
     linked_to: List[IdentificationLink]
     backup_codes: Optional[List[str]] = None
     created_at: int
     updated_at: int
 
 
-class PhoneNumberResponse(BaseModel):
+class PhoneNumberResponse(pydantic.BaseModel):
     """
     Represents the response containing a phone number.
     """
     data: PhoneNumber
 
 
-class Session(BaseModel):
+class Session(pydantic.BaseModel):
     """
     Represents a session object.
     """
     id: str
     object: str
     status: str
     user_id: str
     client_id: str
     created_at: int
     updated_at: int
     last_active_at: Optional[int] = None
 
 
-class SessionListResponse(BaseModel):
+class SessionListResponse(pydantic.BaseModel):
     """
     Represents the response containing a list of sessions.
     """
     data: List[Session]
     meta: PaginationMeta
 
 
-class SessionResponse(BaseModel):
+class SessionResponse(pydantic.BaseModel):
     """
     Represents the response containing a session.
     """
     data: Session
 
 
-class Client(BaseModel):
+class Client(pydantic.BaseModel):
     """
     Represents a client object.
     """
     id: str
     object: str
     created_at: int
     updated_at: int
     last_sign_in_at: Optional[int] = None
     sign_in_attempt_id: Optional[str] = None
     session_ids: Optional[List[str]] = None
     sign_up_attempt_id: Optional[str] = None
     status: Optional[str] = None
 
 
-class ClientListResponse(BaseModel):
+class ClientListResponse(pydantic.BaseModel):
     """
     Represents the response containing a list of clients.
     """
     data: List[Client]
     meta: PaginationMeta
 
 
-class ClientResponse(BaseModel):
+class ClientResponse(pydantic.BaseModel):
     """
     Represents the response containing a client.
     """
     data: Client
 
 
-class Template(BaseModel):
+class Template(pydantic.BaseModel):
     """
     Represents a template object for email or SMS.
     """
     id: str
     object: str
     name: str
     subject: Optional[str] = None
     markup: Optional[str] = None
     body: str
     delivered_by_clerk: bool
     from_email_name: Optional[str] = None
     reply_to_email_name: Optional[str] = None
 
 
-class TemplateListResponse(BaseModel):
+class TemplateListResponse(pydantic.BaseModel):
     """
     Represents the response containing a list of templates.
     """
     data: List[Template]
     meta: PaginationMeta
 
 
-class TemplateResponse(BaseModel):
+class TemplateResponse(pydantic.BaseModel):
     """
     Represents the response containing a template.
     """
     data: Template
 
 
-class Web3Wallet(BaseModel):
+class Web3Wallet(pydantic.BaseModel):
     """
     Represents a Web3 wallet address associated with a user.
 
     The address can be used as a proof of identification for users.
 
     Web3 addresses must be verified to ensure that they can be assigned
     to their rightful owners. The verification is completed via Web3 wallet
@@ -239,15 +239,15 @@
     id: str
     web3_wallet: str
     created_at: int
     updated_at: int
     verification: Optional[Verification] = None
 
 
-class SAMLAccount(BaseModel):
+class SAMLAccount(pydantic.BaseModel):
     """
     Represents a SAML account associated with a user.
 
     Attributes:
         id: A unique identifier for the SAML account.
         object: The type of object, typically 'saml_account'.
         provider: The SAML provider associated with the account.
@@ -267,15 +267,15 @@
     first_name: Optional[str] = None
     last_name: Optional[str] = None
     provider_user_id: Optional[str] = None
     public_metadata: Dict[str, Any]
     verification: Optional[Verification] = None
 
 
-class PasskeyResource(BaseModel):
+class PasskeyResource(pydantic.BaseModel):
     """
     Represents a passkey associated with a user response.
 
     Attributes:
         id: The passkey's unique ID generated by Clerk.
         verification: Verification details for the passkey.
         name: The passkey's name.
@@ -300,15 +300,15 @@
     updated_at: str
     """The date and time when the passkey was updated."""
 
     last_used_at: str
     """The date and time when the passkey was last used."""
 
 
-class User(BaseModel):
+class User(pydantic.BaseModel):
     """
     Represents a user object with various attributes related to their profile, authentication, and metadata.
 
     See the [Clerk documentation][1] for more details.
 
     [1]: https://clerk.com/docs/users/overview
 
@@ -429,45 +429,45 @@
     banned: bool
     """A boolean indicating whether the user is banned."""
 
     locked: bool
     """A boolean indicating whether the user is locked."""
 
 
-class UserListResponse(BaseModel):
+class UserListResponse(pydantic.BaseModel):
     """
     Represents the response containing a list of users.
     """
     data: List[User]
     meta: PaginationMeta
 
 
-class UserCountResponse(BaseModel):
+class UserCountResponse(pydantic.BaseModel):
     """
     Represents the response containing the count of users.
     """
     count: int
 
 
-class InterstitialResponse(BaseModel):
+class InterstitialResponse(pydantic.BaseModel):
     """
     Represents the response containing the interstitial HTML.
     """
     html: str
 
 
-class Key(BaseModel):
+class Key(pydantic.BaseModel):
     """
     Represents a key in the JSON Web Key Set (JWKS).
     """
     kty: str
     use: str
     kid: str
     n: str
     e: str
 
 
-class JWKSResponse(BaseModel):
+class JWKSResponse(pydantic.BaseModel):
     """
     Represents the response containing the JSON Web Key Set (JWKS).
     """
     keys: List[Key]
```

### Comparing `reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/appearance.py` & `reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/appearance.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing
 
-import pydantic
+from reflex.base import pydantic
 
 
 class AppearanceVariables(pydantic.BaseModel):
     """Variables for the appearance."""
 
     colorPrimary: str = None
     # todo: flush this out
```

### Comparing `reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/clerk_provider.py` & `reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/clerk_provider.py`

 * *Files identical despite different names*

### Comparing `reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/control.py` & `reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/control.py`

 * *Files identical despite different names*

### Comparing `reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/reflex_clerk.py` & `reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/reflex_clerk.py`

 * *Files identical despite different names*

### Comparing `reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/sign_in.py` & `reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/sign_in.py`

 * *Files identical despite different names*

### Comparing `reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/sign_out.py` & `reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/sign_out.py`

 * *Files identical despite different names*

### Comparing `reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/sign_up.py` & `reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/sign_up.py`

 * *Files identical despite different names*

### Comparing `reflex_clerk-1.0.0/custom_components/reflex_clerk/lib/user.py` & `reflex_clerk-1.0.1/custom_components/reflex_clerk/lib/user.py`

 * *Files identical despite different names*

### Comparing `reflex_clerk-1.0.0/custom_components/reflex_clerk.egg-info/PKG-INFO` & `reflex_clerk-1.0.1/custom_components/reflex_clerk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: reflex-clerk
-Version: 1.0.0
+Version: 1.0.1
 Summary: Reflex custom component library for Clerk, a user management platform
 Author-email: Elliot Kroo <elliot@kroo.net>
 License: Apache-2.0
+Project-URL: homepage, https://kroo.github.io/reflex-clerk/
+Project-URL: source, https://github.com/kroo/reflex-clerk
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: reflex>=0.5.0
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
```

### Comparing `reflex_clerk-1.0.0/custom_components/reflex_clerk.egg-info/SOURCES.txt` & `reflex_clerk-1.0.1/custom_components/reflex_clerk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

