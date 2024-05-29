# Comparing `tmp/pulumi-django-azure-1.0.8.tar.gz` & `tmp/pulumi_django_azure-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi-django-azure-1.0.8.tar", last modified: Mon Apr  1 16:24:32 2024, max compression
+gzip compressed data, was "pulumi_django_azure-1.0.9.tar", last modified: Fri Apr 19 19:11:54 2024, max compression
```

## Comparing `pulumi-django-azure-1.0.8.tar` & `pulumi_django_azure-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 16:24:32.984897 pulumi-django-azure-1.0.8/
--rw-rw-rw-   0        0        0     1087 2023-12-31 15:16:09.000000 pulumi-django-azure-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     8110 2024-04-01 16:24:32.984897 pulumi-django-azure-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6213 2024-04-01 14:34:04.000000 pulumi-django-azure-1.0.8/README.md
--rw-rw-rw-   0        0        0     1193 2024-04-01 16:23:39.000000 pulumi-django-azure-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       93 2024-04-01 16:24:32.993933 pulumi-django-azure-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-01 16:24:32.944609 pulumi-django-azure-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 16:24:32.951609 pulumi-django-azure-1.0.8/src/pulumi_django_azure/
--rw-rw-rw-   0        0        0       63 2024-02-08 20:15:37.000000 pulumi-django-azure-1.0.8/src/pulumi_django_azure/__init__.py
--rw-rw-rw-   0        0        0    26659 2024-04-01 16:23:14.000000 pulumi-django-azure-1.0.8/src/pulumi_django_azure/django_deployment.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:24:32.982730 pulumi-django-azure-1.0.8/src/pulumi_django_azure.egg-info/
--rw-rw-rw-   0        0        0     8110 2024-04-01 16:24:32.000000 pulumi-django-azure-1.0.8/src/pulumi_django_azure.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2024-04-01 16:24:32.000000 pulumi-django-azure-1.0.8/src/pulumi_django_azure.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 16:24:32.000000 pulumi-django-azure-1.0.8/src/pulumi_django_azure.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-01 16:24:32.000000 pulumi-django-azure-1.0.8/src/pulumi_django_azure.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-01 16:24:32.000000 pulumi-django-azure-1.0.8/src/pulumi_django_azure.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 19:11:54.771749 pulumi_django_azure-1.0.9/
+-rw-rw-rw-   0        0        0     1087 2023-12-31 15:16:09.000000 pulumi_django_azure-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0    10280 2024-04-19 19:11:54.771749 pulumi_django_azure-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8383 2024-04-19 17:43:18.000000 pulumi_django_azure-1.0.9/README.md
+-rw-rw-rw-   0        0        0     1193 2024-04-19 19:11:22.000000 pulumi_django_azure-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       93 2024-04-19 19:11:54.774752 pulumi_django_azure-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 19:11:54.719916 pulumi_django_azure-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 19:11:54.729029 pulumi_django_azure-1.0.9/src/pulumi_django_azure/
+-rw-rw-rw-   0        0        0       63 2024-02-08 20:15:37.000000 pulumi_django_azure-1.0.9/src/pulumi_django_azure/__init__.py
+-rw-rw-rw-   0        0        0    30222 2024-04-19 17:45:17.000000 pulumi_django_azure-1.0.9/src/pulumi_django_azure/django_deployment.py
+drwxrwxrwx   0        0        0        0 2024-04-19 19:11:54.769752 pulumi_django_azure-1.0.9/src/pulumi_django_azure.egg-info/
+-rw-rw-rw-   0        0        0    10280 2024-04-19 19:11:54.000000 pulumi_django_azure-1.0.9/src/pulumi_django_azure.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2024-04-19 19:11:54.000000 pulumi_django_azure-1.0.9/src/pulumi_django_azure.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 19:11:54.000000 pulumi_django_azure-1.0.9/src/pulumi_django_azure.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-19 19:11:54.000000 pulumi_django_azure-1.0.9/src/pulumi_django_azure.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-19 19:11:54.000000 pulumi_django_azure-1.0.9/src/pulumi_django_azure.egg-info/top_level.txt
```

### Comparing `pulumi-django-azure-1.0.8/LICENSE` & `pulumi_django_azure-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pulumi-django-azure-1.0.8/PKG-INFO` & `pulumi_django_azure-1.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,18 @@
-Metadata-Version: 2.1
-Name: pulumi-django-azure
-Version: 1.0.8
-Summary: Simply deployment of Django on Azure with Pulumi
-Author-email: Maarten Ureel <maarten@youreal.eu>
-License: MIT License
-        
-        Copyright (c) 2023 YouReal BV
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://gitlab.com/MaartenUreel/pulumi-django-azure
-Keywords: django,pulumi,azure
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pulumi>=3.99.0
-Requires-Dist: pulumi-azure-native>=2.24.0
-Requires-Dist: pulumi-random>=4.14.0
-
 # Pulumi Django Deployment
 
 This project aims to make a simple Django deployment on Azure easier.
 
 To have a proper and secure environment, we need these components:
 * Storage account for media and static files
 * CDN endpoint in front with a domain name of our choosing
 * PostgreSQL server
 * Azure Communication Services to send e-mails
 * Webapp with multiple custom host names and managed SSL for the website itself
+* Azure Key Vault per application
 * Webapp running pgAdmin
 
 ## Installation
 This package is published on PyPi, so you can just add pulumi-django-azure to your requirements file.
 
 To use a specific branch in your project, add to pyproject.toml dependencies:
 ```
@@ -172,14 +134,63 @@
 ## pgAdmin specifics
 pgAdmin will be created with a default login:
 * Login: dbadmin@dbadmin.net
 * Password: dbadmin
 
 Best practice is to log in right away, create a user for yourself and delete this default user.
 
+## Azure OAuth2 / Django Social Auth
+If you want to set up login with Azure, which would make sense since you are in the ecosystem, you need to create an App Registration in Entra ID, create a secret and then register these settings in your stack:
+```
+pulumi config set --secret --path 'mywebsite_social_auth_azure.key' secret_ID
+pulumi config set --secret --path 'mywebsite_social_auth_azure.secret' secret_value
+pulumi config set --secret --path 'mywebsite_social_auth_azure.tenant_id' directory_tenant_id
+pulumi config set --secret --path 'mywebsite_social_auth_azure.client_id' application_id
+```
+
+Then in your Django deployment, pass to the `add_django_website` command:
+```
+secrets={
+    "mywebsite_social_auth_azure": "AZURE_OAUTH",
+},
+```
+
+The value will be automatically stored in the vault where the application has access to.
+The environment variable will be suffixed with `_SECRET_NAME`.
+
+Then, in your application, retrieve this data from the vault, e.g.:
+```python
+from azure.keyvault.secrets import SecretClient
+from azure.identity import DefaultAzureCredential
+
+# Azure credentials
+azure_credential = DefaultAzureCredential()
+
+# Azure Key Vault
+AZURE_KEY_VAULT = env("AZURE_KEY_VAULT")
+AZURE_KEY_VAULT_URI = f"https://{AZURE_KEY_VAULT}.vault.azure.net"
+azure_key_vault_client = SecretClient(vault_url=AZURE_KEY_VAULT_URI, credential=azure_credential)
+
+# Social Auth settings
+oauth_secret = azure_key_vault_client.get_secret(env("AZURE_OAUTH_SECRET_NAME"))
+oauth_secret = json.loads(oauth_secret.value)
+SOCIAL_AUTH_AZUREAD_TENANT_OAUTH2_KEY = oauth_secret["client_id"]
+SOCIAL_AUTH_AZUREAD_TENANT_OAUTH2_SECRET = oauth_secret["secret"]
+SOCIAL_AUTH_AZUREAD_TENANT_OAUTH2_TENANT_ID = oauth_secret["tenant_id"]
+SOCIAL_AUTH_ADMIN_USER_SEARCH_FIELDS = ["username", "first_name", "last_name", "email"]
+SOCIAL_AUTH_POSTGRES_JSONFIELD = True
+
+AUTHENTICATION_BACKENDS = (
+    "social_core.backends.azuread_tenant.AzureADTenantOAuth2",
+    "django.contrib.auth.backends.ModelBackend",
+)
+```
+
+And of course add the login button somewhere, following Django Social Auth instructions.
+
 ## Automate deployments
 When using a service like GitLab, you can configure a Webhook to fire upon a push to your branch.
 
 You need to download the deployment profile to obtain the deployment username and password, and then you can construct a URL like this:
 
 ```
 https://{user}:{pass}@{appname}.scm.azurewebsites.net/deploy
```

### Comparing `pulumi-django-azure-1.0.8/pyproject.toml` & `pulumi_django_azure-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pulumi-django-azure"
-version = "1.0.8"
+version = "1.0.9"
 description = "Simply deployment of Django on Azure with Pulumi"
 readme = "README.md"
 authors = [{ name = "Maarten Ureel", email = "maarten@youreal.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -23,15 +23,15 @@
 requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://gitlab.com/MaartenUreel/pulumi-django-azure"
 
 [tool.poetry]
 name = "pulumi-django-azure"
-version = "1.0.8"
+version = "1.0.9"
 description = "Simply deployment of Django on Azure with Pulumi"
 authors = ["Maarten Ureel <maarten@youreal.eu>"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pulumi-azure-native = "^2.24.0"
 pulumi = "^3.99.0"
```

### Comparing `pulumi-django-azure-1.0.8/src/pulumi_django_azure/django_deployment.py` & `pulumi_django_azure-1.0.9/src/pulumi_django_azure/django_deployment.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,21 +31,21 @@
         :param vnet: The virtual network to create the subnets in.
         :param pgsql_sku: The SKU for the PostgreSQL server.
         :param pgsql_ip_prefix: The IP prefix for the PostgreSQL subnet.
         :param appservice_ip_prefix: The IP prefix for the app service subnet.
         :param app_service_sku: The SKU for the app service plan.
         :param storage_account_name: The name of the storage account. Should be unique across Azure.
         :param cdn_host: A custom CDN host name (optional)
-        :param comms_data_location: The data location for the Communication Services (optional if you don't need it)
         :param opts: The resource options
         """
 
         super().__init__("pkg:index:DjangoDeployment", name, None, opts)
 
         # child_opts = pulumi.ResourceOptions(parent=self)
+        self._config = pulumi.Config()
 
         self._name = name
         self._tenant_id = tenant_id
         self._rg = resource_group_name
         self._vnet = vnet
 
         # Storage resources
@@ -387,14 +387,67 @@
             location="global",
             data_location=data_location,
             linked_domains=domain_resources,
         )
 
         return comm_service
 
+    def _add_webapp_vault(self, administrators: list[str], suffix: str) -> azure.keyvault.Vault:
+        # Create a keyvault
+        vault = azure.keyvault.Vault(
+            f"vault-{suffix}",
+            resource_group_name=self._rg,
+            vault_name=f"vault-{suffix}",
+            properties=azure.keyvault.VaultPropertiesArgs(
+                tenant_id=self._tenant_id,
+                sku=azure.keyvault.SkuArgs(
+                    name=azure.keyvault.SkuName.STANDARD,
+                    family=azure.keyvault.SkuFamily.A,
+                ),
+                enable_rbac_authorization=True,
+            ),
+        )
+
+        # Find the Key Vault Administrator role
+        administrator_role = vault.id.apply(
+            lambda scope: azure.authorization.get_role_definition(
+                role_definition_id="00482a5a-887f-4fb3-b363-3b7fe8e74483",
+                scope=scope,
+            )
+        )
+
+        # Add vault administrators
+        for a in administrators:
+            azure.authorization.RoleAssignment(
+                f"ra-{suffix}-vault-admin-{a}",
+                principal_id=a,
+                principal_type=azure.authorization.PrincipalType.USER,
+                role_definition_id=administrator_role.id,
+                scope=vault.id,
+            )
+
+        return vault
+
+    def _add_webapp_secret(self, vault: azure.keyvault.Vault, secret_name: str, config_secret_name: str, suffix: str):
+        secret = self._config.require_secret(config_secret_name)
+
+        # Normalize the secret name
+        secret_name = secret_name.replace("_", "-").lower()
+
+        # Create a secret in the vault
+        return azure.keyvault.Secret(
+            f"secret-{suffix}-{secret_name}",
+            resource_group_name=self._rg,
+            vault_name=vault.name,
+            secret_name=secret_name,
+            properties=azure.keyvault.SecretPropertiesArgs(
+                value=secret,
+            ),
+        )
+
     def _get_storage_account_access_keys(
         self, storage_account: azure.storage.StorageAccount
     ) -> Sequence[azure.storage.outputs.StorageAccountKeyResponse]:
         """
         Helper function to get the access keys for a storage account.
 
         :param storage_account: The storage account
@@ -433,29 +486,35 @@
         name: str,
         db_name: str,
         repository_url: str,
         repository_branch: str,
         website_hosts: list[str],
         django_settings_module: str,
         environment_variables: dict[str, str] = {},
+        secrets: dict[str, str] = {},
         comms_data_location: Optional[str] = None,
         comms_domains: Optional[list[str]] = [],
+        vault_administrators: Optional[list[str]] = [],
     ) -> azure.web.WebApp:
         """
         Create a Django website with it's own database and storage containers.
 
         :param name: The reference for the website, will be used to name subresources.
         :param db_name: The name of the database to create.
         :param repository_url: The URL of the Git repository.
         :param repository_branch: The Git branch to deploy.
         :param website_hosts: The list of custom host names for the website.
         :param django_settings_module: The Django settings module to load.
         :param environment_variables: A dictionary of environment variables to set.
+        :param secrets: A dictionary of secrets to store in the Key Vault and assign as environment variables.
+            The key is the name of the Pulumi secret, the value is the name of the environment variable
+            and the name of the secret in the Key Vault.
         :param comms_data_location: The data location for the Communication Services (optional if you don't need it).
         :param comms_domains: The list of custom domains for the E-mail Communication Services (optional).
+        :param vault_administrator: The principal ID of the vault administrator (optional).
         """
 
         # Create a database
         db = azure.dbforpostgresql.Database(
             f"db-{name}",
             database_name=db_name,
             resource_group_name=self._rg,
@@ -479,19 +538,27 @@
             public_access=azure.storage.PublicAccess.BLOB,
             container_name=f"{name}-static",
         )
 
         # Communication Services (optional)
         if comms_data_location:
             comms = self._add_webapp_comms(comms_data_location, comms_domains, f"{name}-{self._name}")
-            # Add the domains as environment variable
+            # Add the service endpoint as environment variable
             environment_variables["AZURE_COMMUNICATION_SERVICE_ENDPOINT"] = comms.host_name.apply(lambda host: f"https://{host}")
         else:
             comms = None
 
+        # Key Vault
+        vault = self._add_webapp_vault(vault_administrators, f"{name}-{self._name}")
+
+        # Add secrets
+        for config_name, env_name in secrets.items():
+            s = self._add_webapp_secret(vault, env_name, config_name, f"{name}-{self._name}")
+            environment_variables[f"{env_name}_SECRET_NAME"] = s.name
+
         # Create a Django Secret Key (random)
         secret_key = pulumi_random.RandomString(f"django-secret-{name}-{self._name}", length=50)
 
         # Convert environment variables to NameValuePairArgs
         environment_variables = [
             azure.web.NameValuePairArgs(
                 name=key,
@@ -524,14 +591,16 @@
                     azure.web.NameValuePairArgs(name="DISABLE_COLLECTSTATIC", value="true"),
                     azure.web.NameValuePairArgs(name="HEALTH_CHECK_PATH", value=self.HEALTH_CHECK_PATH),
                     # Django settings
                     # azure.web.NameValuePairArgs(name="DEBUG", value="true"),
                     azure.web.NameValuePairArgs(name="DJANGO_SETTINGS_MODULE", value=django_settings_module),
                     azure.web.NameValuePairArgs(name="DJANGO_SECRET_KEY", value=secret_key.result),
                     azure.web.NameValuePairArgs(name="DJANGO_ALLOWED_HOSTS", value=",".join(website_hosts)),
+                    # Vault settings
+                    azure.web.NameValuePairArgs(name="AZURE_KEY_VAULT", value=vault.name),
                     # Storage settings
                     azure.web.NameValuePairArgs(name="AZURE_STORAGE_ACCOUNT_NAME", value=self._storage_account.name),
                     azure.web.NameValuePairArgs(name="AZURE_STORAGE_CONTAINER_STATICFILES", value=static_container.name),
                     azure.web.NameValuePairArgs(name="AZURE_STORAGE_CONTAINER_MEDIA", value=media_container.name),
                     # CDN
                     azure.web.NameValuePairArgs(name="CDN_HOST", value=self._cdn_host),
                     # Database settings
@@ -568,14 +637,32 @@
         )
 
         # Where we can retrieve the SSH key
         pulumi.export(
             f"{name}_deploy_ssh_key_url", app.name.apply(lambda name: f"https://{name}.scm.azurewebsites.net/api/sshkey?ensurePublicKey=1")
         )
 
+        # Find the role for Key Vault Secrets User
+        vault_access_role = vault.id.apply(
+            lambda scope: azure.authorization.get_role_definition(
+                role_definition_id="4633458b-17de-408a-b874-0445c86b69e6",
+                scope=scope,
+            )
+        )
+
+        # Grant the app access to the vault
+        azure.authorization.RoleAssignment(
+            f"ra-{name}-vault-user",
+            principal_id=principal_id,
+            principal_type=azure.authorization.PrincipalType.SERVICE_PRINCIPAL,
+            # Key Vault Secrets User
+            role_definition_id=vault_access_role.id,
+            scope=vault.id,
+        )
+
         # Find the role for Storage Blob Data Contributor
         storage_role = self._storage_account.id.apply(
             lambda scope: azure.authorization.get_role_definition(
                 role_definition_id="ba92f5b4-2d11-453d-a403-e96b0029c9fe",
                 scope=scope,
             )
         )
```

