# Comparing `tmp/eodc-2024.5.2.tar.gz` & `tmp/eodc-2024.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2024.5.2.tar", max compression
+gzip compressed data, was "eodc-2024.5.3.tar", max compression
```

## Comparing `eodc-2024.5.2.tar` & `eodc-2024.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      676 2024-05-15 13:17:28.660436 eodc-2024.5.2/README.md
--rw-r--r--   0        0        0      195 2024-05-15 13:17:28.660436 eodc-2024.5.2/eodc/__init__.py
--rw-r--r--   0        0        0     1794 2024-05-15 13:17:28.660436 eodc-2024.5.2/eodc/auth.py
--rw-r--r--   0        0        0     1311 2024-05-15 13:17:28.660436 eodc-2024.5.2/eodc/dask.py
--rw-r--r--   0        0        0    13711 2024-05-15 13:17:28.660436 eodc-2024.5.2/eodc/faas.py
--rw-r--r--   0        0        0     1183 2024-05-15 13:17:28.660436 eodc-2024.5.2/eodc/settings.py
--rw-r--r--   0        0        0     2240 2024-05-15 13:17:28.660436 eodc-2024.5.2/eodc/storage.py
--rw-r--r--   0        0        0        0 2024-05-15 13:17:28.660436 eodc-2024.5.2/eodc/visualisation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 13:17:28.660436 eodc-2024.5.2/eodc/visualisation/vessel_detection/__init__.py
--rwxr-xr-x   0        0        0    15080 2024-05-15 13:17:28.660436 eodc-2024.5.2/eodc/visualisation/vessel_detection/app.py
--rw-r--r--   0        0        0      261 2024-05-15 13:17:28.660436 eodc-2024.5.2/eodc/visualisation/vessel_detection/assets/app.css
--rw-r--r--   0        0        0     2539 2024-05-15 13:17:28.660436 eodc-2024.5.2/eodc/visualisation/vessel_detection/cards.py
--rw-r--r--   0        0        0     8522 2024-05-15 13:17:28.660436 eodc-2024.5.2/eodc/visualisation/vessel_detection/navbar.py
--rw-r--r--   0        0        0     2867 2024-05-15 13:17:28.660436 eodc-2024.5.2/eodc/visualisation/vessel_detection/utils.py
--rw-r--r--   0        0        0    33301 2024-05-15 13:17:28.660436 eodc-2024.5.2/eodc/workspace.py
--rw-r--r--   0        0        0     1890 2024-05-15 13:17:28.664436 eodc-2024.5.2/pyproject.toml
--rw-r--r--   0        0        0     2802 1970-01-01 00:00:00.000000 eodc-2024.5.2/PKG-INFO
+-rw-r--r--   0        0        0      733 2024-05-29 12:12:24.051768 eodc-2024.5.3/README.md
+-rw-r--r--   0        0        0      195 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/__init__.py
+-rw-r--r--   0        0        0     1794 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/auth.py
+-rw-r--r--   0        0        0     1311 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/dask.py
+-rw-r--r--   0        0        0    13711 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/faas.py
+-rw-r--r--   0        0        0     1183 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/settings.py
+-rw-r--r--   0        0        0     2240 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/storage.py
+-rw-r--r--   0        0        0        0 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/visualisation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/visualisation/vessel_detection/__init__.py
+-rwxr-xr-x   0        0        0    15080 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/visualisation/vessel_detection/app.py
+-rw-r--r--   0        0        0      261 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/visualisation/vessel_detection/assets/app.css
+-rw-r--r--   0        0        0     2539 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/visualisation/vessel_detection/cards.py
+-rw-r--r--   0        0        0     8522 2024-05-29 12:12:24.051768 eodc-2024.5.3/eodc/visualisation/vessel_detection/navbar.py
+-rw-r--r--   0        0        0     2867 2024-05-29 12:12:24.055768 eodc-2024.5.3/eodc/visualisation/vessel_detection/utils.py
+-rw-r--r--   0        0        0    37916 2024-05-29 12:12:24.055768 eodc-2024.5.3/eodc/workspace.py
+-rw-r--r--   0        0        0     1890 2024-05-29 12:12:24.055768 eodc-2024.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2859 1970-01-01 00:00:00.000000 eodc-2024.5.3/PKG-INFO
```

### Comparing `eodc-2024.5.2/eodc/auth.py` & `eodc-2024.5.3/eodc/auth.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.2/eodc/dask.py` & `eodc-2024.5.3/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.2/eodc/faas.py` & `eodc-2024.5.3/eodc/faas.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.2/eodc/settings.py` & `eodc-2024.5.3/eodc/settings.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.2/eodc/storage.py` & `eodc-2024.5.3/eodc/storage.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.2/eodc/visualisation/vessel_detection/app.py` & `eodc-2024.5.3/eodc/visualisation/vessel_detection/app.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.2/eodc/visualisation/vessel_detection/cards.py` & `eodc-2024.5.3/eodc/visualisation/vessel_detection/cards.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.2/eodc/visualisation/vessel_detection/navbar.py` & `eodc-2024.5.3/eodc/visualisation/vessel_detection/navbar.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.2/eodc/visualisation/vessel_detection/utils.py` & `eodc-2024.5.3/eodc/visualisation/vessel_detection/utils.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.5.2/eodc/workspace.py` & `eodc-2024.5.3/eodc/workspace.py`

 * *Files 20% similar despite different names*

```diff
@@ -43,17 +43,23 @@
     """
 
     storage_type: StorageType
 
     @staticmethod
     def create_adapter(
         tenant_url: str = None,  # Can be ignored for Azure
-        storage_type: StorageType = StorageType.MINIO,
+        storage_type: StorageType = StorageType.CEPH,
         parameters: dict[str, Any] = {},
     ) -> Self:
+        """
+        This function is a factory method that creates an instance of the
+        WorkspaceAdapter based on the given parameters.
+
+        Returns none if the storage type is not supported.
+        """
         if storage_type == StorageType.MINIO:
             return MinIOAdapter(
                 url=tenant_url,
                 access_key=parameters["access_key"],
                 secret_key=parameters["secret_key"],
                 mc_bin_path=parameters["mc_bin_path"],
             )
@@ -68,75 +74,211 @@
                 secret_key=parameters["secret_key"],
             )
         else:
             return None
 
     @abstractmethod
     def get_credentials(self) -> dict[str, Any]:
+        """
+        This method returns the credentials needed to connect to the storage.
+
+        The credentials are returned as a dictionary, where the keys are the
+        names of the credentials and the values are the credentials themselves.
+
+        This is useful for debugging and for passing the credentials to other
+        parts of the system.
+
+        returns:
+            dict[str, Any]: A dictionary containing the credentials.
+        """
         pass
 
     @abstractmethod
     def create_user_workspace(
         self, workspace_name: str, user_name: str, **kwargs
     ) -> None:
+        """
+        This method creates a new workspace for a user.
+        Depending on the storage system, this may involve creating a new bucket,
+        creating a new container, or however else the storage system represents
+        workspaces.
+
+        returns:
+            None
+        """
         pass
 
     @abstractmethod
-    def delete_user_workspace(self, workspace_name: str):
+    def delete_user_workspace(self, workspace_name: str) -> None:
+        """
+        This method deletes a workspace for a user.
+
+        Depending on the storage system, this may involve deleting a bucket,
+        deleting a container, or however else the storage system represents
+        workspaces.
+
+        If the workspace does not exist, this method should raise an error.
+        If the workspace is not empty, this method should raise an error.
+
+        returns:
+            None
+        """
         pass
 
     @abstractmethod
     def workspace_exists(self, workspace_name: str) -> bool:
+        """
+        This method checks if a workspace exists with the current adapter.
+
+        returns:
+            bool: True if the workspace exists, False otherwise.
+        """
         pass
 
     @abstractmethod
     def list_workspaces(self) -> list[str]:
+        """
+        This method lists all the workspaces that exist with the current adapter.
+
+        returns:
+            list[str]: A list of workspace names.
+        """
         pass
 
     @abstractmethod
     def list_workspace_files(self, workspace_name: str):
+        """
+        This method lists all the files in a workspace.
+
+        returns:
+            list[str]: A list of file names/paths.
+        """
         pass
 
     @abstractmethod
-    def upload_file(self, workspace_name: str, file_path: str, path_in_workspace: str):
+    def upload_file(
+        self, workspace_name: str, file_path: str, path_in_workspace: str
+    ) -> None:
+        """
+        This method uploads a file to a workspace.
+
+        The file is uploaded to the workspace with the given name, and is placed
+        in the workspace at the given path.
+
+        parameters:
+            file_path (str): The path to the file to be uploaded.
+            path_in_workspace (str): The path in the workspace where the file
+            should be placed.
+
+        returns:
+            None
+        """
         pass
 
     @abstractmethod
-    def upload_stream(self, workspace_name: str, stream: Any, file_name: str):
+    def upload_stream(self, workspace_name: str, stream: Any, file_name: str) -> None:
+        """
+        This method uploads a stream to a workspace.
+
+        The stream is uploaded to the workspace with the given name, and is placed
+        in the workspace at the given path.
+
+        returns:
+            None
+        """
         pass
 
     @abstractmethod
-    def delete_file(self, workspace_name: str, file_name: str):
+    def delete_file(self, workspace_name: str, file_name: str) -> None:
+        """
+        This method deletes a file from a workspace.
+
+        The file is deleted from the workspace with the given name.
+
+        returns:
+            None
+        """
         pass
 
     @abstractmethod
-    def download_file(self, workspace_name: str, file_name: str, path: str):
+    def download_file(self, workspace_name: str, file_name: str, path: str) -> None:
+        """
+        This method downloads a file from a workspace.
+
+        The file is downloaded from the workspace with the given name, and is placed
+        in the given path.
+
+        returns:
+            None
+        """
         pass
 
     @abstractmethod
-    def download_stream(self, workspace_name: str, file_name: str):
+    def download_stream(self, workspace_name: str, file_name: str) -> Any:
+        """
+        This method downloads a stream from a workspace.
+
+        The stream is downloaded from the workspace with the given name
+        and returned.
+
+        returns:
+            Any: The stream that was downloaded.
+        """
         pass
 
     @abstractmethod
-    def get_fsspec(self, workspace_name: str):
+    def get_fsspec(self, workspace_name: str) -> Any:
+        """
+        This method returns an fsspec filesystem object for the given workspace.
+
+        This object can be used to interact with the workspace using the fsspec
+        library.
+
+        returns:
+            Any: An fsspec filesystem object.
+        """
         pass
 
     @abstractmethod
     def get_signed_url(
         self, bucket_name, object_key, method="GET", expiration_time=3600
     ):
+        """
+        This method returns a signed URL for the given object in the given bucket.
+
+        The signed URL can be used to access the object without needing to authenticate.
+
+        returns:
+            str: The signed URL.
+        """
         pass
 
     def upload_path(
         self,
         workspace_name: str = "",
         path: str = "",
         path_in_workspace: str = "",
         recursive: bool = False,
     ):
+        """
+        This method uploads a path to a workspace.
+
+        The path is uploaded to the workspace with the given name, and is placed
+        in the workspace at the given path.
+
+        parameters:
+            workspace_name (str): Workspace name to upload to.
+            path (str): The path to the file to be uploaded.
+            path_in_workspace (str): The path in the workspace where
+            the file should be placed.
+            recursive (bool): Whether to upload the path recursively.
+
+        returns:
+            None
+        """
         path_in_workspace = path_in_workspace.removesuffix("/")
         files = Path(path).rglob("*") if recursive else Path(path).glob("*")
 
         for file in files:
             if not file.is_file():
                 continue
             relative_path = "/".join(os.path.relpath(file, path).split("/")[:-1])
@@ -461,15 +603,15 @@
     """
     This Adapter implements the Ceph API for the Workspaces API.
 
     Workspaces are implemented as buckets, and files are implemented
     as objects.
     """
 
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+    def __call__(self, *args: Any, **kwargs: Any) -> Self:
         return self
 
     def __init__(self, url: str, access_key: SecretStr, secret_key: SecretStr):
         self.storage_type = StorageType.CEPH
         self.access_key = access_key
         self.secret_key = secret_key
         self.url = url
@@ -518,18 +660,20 @@
 
     def delete_user_workspace(self, workspace_name: str):
         self.s3_client.delete_bucket(Bucket=workspace_name)
 
     def workspace_exists(self, workspace_name: str) -> bool:
         return workspace_name in self.list_workspaces()
 
-    def list_workspace_files(self, workspace_name: str, tenant_name: str = None):
+    def list_workspace_files(
+        self, workspace_name: str, tenant_name: str = None, verbose=False
+    ):
         tenant_name = f"{tenant_name}:" if tenant_name else ""
         files = self.s3_client.list_objects(Bucket=f"{tenant_name}{workspace_name}")
-        return files["Contents"]
+        return [file["Key"] if not verbose else file for file in files["Contents"]]
 
     def upload_file(
         self, workspace_name: str, file_path: str, path_in_workspace: str = ""
     ):
         path_in_workspace = path_in_workspace.removesuffix("/")
         self.s3_client.upload_file(
             file_path,
@@ -736,23 +880,25 @@
 
     @classmethod
     def make_policy_entry(
         cls,
         resource_names: list[str],
         actions: list[str],
         conditions: dict[str, Any] = None,
-        tenant: str = "",
-        user: str = None,
+        tenant_users: str = list[tuple[str, str]],
         allow: bool = True,
     ) -> PolicyEntry:
-        user_name = f"arn:aws:iam::{tenant}:user/{user}" if tenant is not None else user
+        user_names = [
+            f"arn:aws:iam::{tenant}:user/{user}" if tenant is not None else user
+            for tenant, user in tenant_users
+        ]
         return {
             "Sid": "Policy",
             "Effect": "Allow" if allow else "Deny",
-            **({"Principal": {"AWS": [user_name]}} if user_name is not None else {}),
+            **({"Principal": {"AWS": user_names}} if user_names is not None else {}),
             "Action": [action for action in actions],
             "Resource": [f"arn:aws:s3:::{resource}" for resource in resource_names],
             **({"Condition": conditions} if conditions is not None else {}),
         }
 
     def __init__(self, policy_name: str):
         self.policy = {"Version": "2012-10-17", "Statement": []}
@@ -849,90 +995,88 @@
         return self._add_workspaces_privileges(
             workspace_names=workspace_names,
             privileges=["s3:*"],
             conditions={"IpAddress": {"aws:SourceIp": ip_address}},
             allow=False,
         )
 
-    def add_user_read_privileges(
-        self, workspace_name: str, user: str = None, tenant: str = ""
+    def add_users_read_privileges(
+        self,
+        workspace_name: str,
+        tenant_users: list[tuple[str, str]] = None,
     ) -> Self:
-        assert user is not None, "User must be specified"
-        return self._add_user_privileges(
+        assert tenant_users is not None, "Users must be specified"
+        return self._add_users_privileges(
             workspace_name=workspace_name,
             privileges=[
                 "s3:ListBucket",
                 "s3:GetObject",
             ],
-            tenant=tenant,
-            user=user,
+            tenant_users=tenant_users,
             allow=True,
         )
 
-    def add_user_write_privileges(
-        self, workspace_name: str, user: str = None, tenant: str = ""
+    def add_users_write_privileges(
+        self,
+        workspace_name: str,
+        tenant_users: list[tuple[str, str]] = None,
     ) -> Self:
-        assert user is not None, "User must be specified"
-        return self._add_user_privileges(
+        assert tenant_users is not None, "Users must be specified"
+        return self._add_users_privileges(
             workspace_name=workspace_name,
             privileges=[
                 "s3:PutObject",
             ],
-            tenant=tenant,
-            user=user,
+            tenant_users=tenant_users,
             allow=True,
         )
 
-    def add_user_delete_privileges(
-        self, workspace_name: str, user: str = None, tenant: str = ""
+    def add_users_delete_privileges(
+        self, workspace_name: str, tenant_users: list[tuple[str, str]] = None
     ) -> Self:
-        assert user is not None, "User must be specified"
-        return self._add_user_privileges(
+        assert tenant_users is not None, "Users must be specified"
+        return self._add_users_privileges(
             workspace_name=workspace_name,
             privileges=[
                 "s3:DeleteObject",
             ],
-            tenant=tenant,
-            user=user,
+            tenant_users=tenant_users,
             allow=True,
         )
 
-    def add_user_full_privileges(
-        self, workspace_name: str, user: str = None, tenant: str = ""
+    def add_users_full_privileges(
+        self, workspace_name: str, tenant_users: list[tuple[str, str]] = None
     ) -> Self:
-        assert user is not None, "User must be specified"
-        return self._add_user_privileges(
+        assert tenant_users is not None, "Users must be specified"
+        return self._add_users_privileges(
             workspace_name=workspace_name,
             privileges=[
                 "s3:ListBucket",
                 "s3:GetObject",
                 "s3:PutObject",
                 "s3:DeleteObject",
             ],
-            tenant=tenant,
-            user=user,
+            tenant_users=tenant_users,
             allow=True,
         )
 
-    def _add_user_privileges(
+    def _add_users_privileges(
         self,
         workspace_name: str,
         privileges: list[str],
         conditions: dict[str, Any] = None,
-        tenant: str = "",
-        user: str = None,
+        tenant_users: list[tuple[str, str]] = None,
         allow: bool = True,
     ) -> Self:
         self.policy["Statement"].append(
             S3PolicyBuilder.make_policy_entry(
                 resource_names=[workspace_name, f"{workspace_name}/*"],
                 actions=privileges,
                 conditions=conditions,
-                tenant=tenant,
-                user=user,
+                tenant_users=tenant_users,
                 allow=allow,
             )
         )
         return self
 
     def _add_workspaces_privileges(
         self,
@@ -977,7 +1121,11 @@
                 ],
                 actions=privileges,
                 conditions=conditions,
                 allow=allow,
             )
         )
         return self
+
+
+class WorkspaceError(Exception):
+    pass
```

### Comparing `eodc-2024.5.2/pyproject.toml` & `eodc-2024.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "eodc"
 
-version = "2024.5.2"
+version = "2024.5.3"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Gerald Irsiegler <gerald.irsiegler@eodc.eu>", "Christoph Reimer <christoph.reimer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `eodc-2024.5.2/PKG-INFO` & `eodc-2024.5.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2024.5.2
+Version: 2024.5.3
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
@@ -79,9 +79,11 @@
 
 ### Function-as-a-Service (FaaS)
 TODO
 
 
 ### Workspaces
 
-Workspaces are s3-like storages for storing data. A workspace is a bucket and can be used in multiple EODC services by using a WorkspaceAdapter.
+A workspace is a an abstraction of a object storage container/bucket. It is used to store and retrieve data.
+
+Workspaces are integrated with EODC products and services, such as the openEO EODC backend.
```

