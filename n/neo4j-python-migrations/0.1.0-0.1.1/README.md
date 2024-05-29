# Comparing `tmp/neo4j-python-migrations-0.1.0.tar.gz` & `tmp/neo4j-python-migrations-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo4j-python-migrations-0.1.0.tar", max compression
+gzip compressed data, was "neo4j-python-migrations-0.1.1.tar", max compression
```

## Comparing `neo4j-python-migrations-0.1.0.tar` & `neo4j-python-migrations-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2022-10-25 20:35:28.501333 neo4j-python-migrations-0.1.0/LICENSE
--rw-r--r--   0        0        0     6314 2022-11-27 18:43:58.769996 neo4j-python-migrations-0.1.0/README.md
--rw-r--r--   0        0        0       30 2022-11-08 18:06:38.727342 neo4j-python-migrations-0.1.0/neo4j_python_migrations/__init__.py
--rw-r--r--   0        0        0       82 2022-11-27 17:12:45.566050 neo4j-python-migrations-0.1.0/neo4j_python_migrations/__main__.py
--rw-r--r--   0        0        0     3344 2022-11-27 17:14:05.346094 neo4j-python-migrations-0.1.0/neo4j_python_migrations/analyzer.py
--rw-r--r--   0        0        0     4593 2022-11-27 18:21:57.635773 neo4j-python-migrations-0.1.0/neo4j_python_migrations/cli.py
--rw-r--r--   0        0        0     5773 2022-11-27 18:22:31.375697 neo4j-python-migrations-0.1.0/neo4j_python_migrations/dao.py
--rw-r--r--   0        0        0     3206 2022-11-27 17:59:06.934651 neo4j-python-migrations-0.1.0/neo4j_python_migrations/executor.py
--rw-r--r--   0        0        0     2368 2022-11-27 17:14:19.966103 neo4j-python-migrations-0.1.0/neo4j_python_migrations/loader.py
--rw-r--r--   0        0        0     2841 2022-11-27 17:23:24.820747 neo4j-python-migrations-0.1.0/neo4j_python_migrations/migration.py
--rw-r--r--   0        0        0     1224 2022-11-03 14:13:24.825824 neo4j-python-migrations-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7307 1970-01-01 00:00:00.000000 neo4j-python-migrations-0.1.0/setup.py
--rw-r--r--   0        0        0     7229 1970-01-01 00:00:00.000000 neo4j-python-migrations-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-10-25 20:35:28.501333 neo4j-python-migrations-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6314 2022-11-27 18:43:58.769996 neo4j-python-migrations-0.1.1/README.md
+-rw-r--r--   0        0        0       30 2022-11-08 18:06:38.727342 neo4j-python-migrations-0.1.1/neo4j_python_migrations/__init__.py
+-rw-r--r--   0        0        0       82 2022-11-27 17:12:45.566050 neo4j-python-migrations-0.1.1/neo4j_python_migrations/__main__.py
+-rw-r--r--   0        0        0     3344 2022-11-27 17:14:05.346094 neo4j-python-migrations-0.1.1/neo4j_python_migrations/analyzer.py
+-rw-r--r--   0        0        0     4593 2022-11-27 18:21:57.635773 neo4j-python-migrations-0.1.1/neo4j_python_migrations/cli.py
+-rw-r--r--   0        0        0     5773 2022-11-27 18:22:31.375697 neo4j-python-migrations-0.1.1/neo4j_python_migrations/dao.py
+-rw-r--r--   0        0        0     3206 2022-11-27 17:59:06.934651 neo4j-python-migrations-0.1.1/neo4j_python_migrations/executor.py
+-rw-r--r--   0        0        0     2327 2022-11-30 10:45:55.706010 neo4j-python-migrations-0.1.1/neo4j_python_migrations/loader.py
+-rw-r--r--   0        0        0     3191 2022-11-30 10:45:55.706010 neo4j-python-migrations-0.1.1/neo4j_python_migrations/migration.py
+-rw-r--r--   0        0        0     1224 2022-11-30 10:45:55.706010 neo4j-python-migrations-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7307 1970-01-01 00:00:00.000000 neo4j-python-migrations-0.1.1/setup.py
+-rw-r--r--   0        0        0     7229 1970-01-01 00:00:00.000000 neo4j-python-migrations-0.1.1/PKG-INFO
```

### Comparing `neo4j-python-migrations-0.1.0/LICENSE` & `neo4j-python-migrations-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neo4j-python-migrations-0.1.0/README.md` & `neo4j-python-migrations-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `neo4j-python-migrations-0.1.0/neo4j_python_migrations/analyzer.py` & `neo4j-python-migrations-0.1.1/neo4j_python_migrations/analyzer.py`

 * *Files identical despite different names*

### Comparing `neo4j-python-migrations-0.1.0/neo4j_python_migrations/cli.py` & `neo4j-python-migrations-0.1.1/neo4j_python_migrations/cli.py`

 * *Files identical despite different names*

### Comparing `neo4j-python-migrations-0.1.0/neo4j_python_migrations/dao.py` & `neo4j-python-migrations-0.1.1/neo4j_python_migrations/dao.py`

 * *Files identical despite different names*

### Comparing `neo4j-python-migrations-0.1.0/neo4j_python_migrations/executor.py` & `neo4j-python-migrations-0.1.1/neo4j_python_migrations/executor.py`

 * *Files identical despite different names*

### Comparing `neo4j-python-migrations-0.1.0/neo4j_python_migrations/loader.py` & `neo4j-python-migrations-0.1.1/neo4j_python_migrations/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
         migrations[version] = loaders[extension](
             version=version,
             description=description,
             migration_file=migration_file,
         )
 
-    return sorted(migrations.values(), key=lambda migration: migration.version)
+    return sorted(migrations.values())
 
 
 def _prepare_version(version: str) -> str:
     return version.replace("_", ".")
 
 
 def _prepare_description(description: str) -> str:
```

### Comparing `neo4j-python-migrations-0.1.0/neo4j_python_migrations/migration.py` & `neo4j-python-migrations-0.1.1/neo4j_python_migrations/migration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import binascii
 from enum import Enum
 from typing import Any, Callable, Dict, List, Optional
 
 from attr import asdict, define, field
 from neo4j import Session
+from packaging.version import Version
 
 
 class MigrationType(str, Enum):  # noqa: WPS600
     """The type of migration to store in the database."""
 
     PYTHON = "PYTHON"
     CYPHER = "CYPHER"
 
 
-@define(kw_only=True)
+@define(kw_only=True, order=False)
 class Migration:
     """The base class for all migrations."""
 
     version: str
+    parsed_version: Version = field(init=False)
     description: str
     type: str
     source: Optional[str] = None
     checksum: Optional[str] = None
 
     @classmethod
     def from_dict(cls, properties: Dict[str, Any]) -> "Migration":
@@ -54,14 +56,20 @@
         Apply migration to the database.
 
         :param session: neo4j session.
         :raises NotImplementedError: if not implemented.
         """
         raise NotImplementedError()
 
+    def __attrs_post_init__(self) -> None:
+        self.parsed_version = Version(self.version)  # noqa: WPS601
+
+    def __lt__(self, other: Any) -> bool:
+        return self.parsed_version < other.parsed_version
+
 
 @define
 class PythonMigration(Migration):
     """Migration based on a python code."""
 
     code: Callable[[Session], None]
     type: str = field(default=MigrationType.PYTHON, init=False)
@@ -75,14 +83,15 @@
     """Migration based on a cypher script."""
 
     query: str = field(repr=False)
     type: str = field(default=MigrationType.CYPHER, init=False)
     statements: List[str] = field(init=False, repr=False)
 
     def __attrs_post_init__(self) -> None:
+        super().__attrs_post_init__()
         self.statements = list(  # noqa: WPS601
             filter(
                 lambda statement: statement,
                 [statement.strip() for statement in self.query.split(";")[:-1]],
             ),
         )
```

### Comparing `neo4j-python-migrations-0.1.0/pyproject.toml` & `neo4j-python-migrations-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neo4j-python-migrations"
-version = "0.1.0"
+version = "0.1.1"
 description = "A database migration tool for Neo4j that allows to apply Cypher-based and arbitrary Python-based migrations."
 authors = ["Grigory Bukovsky <booqoffsky@yandex.ru>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "neo4j_python_migrations"}]
 repository = 'https://github.com/booqoffsky/neo4j-python-migrations'
 keywords = ['neo4j', 'migrations', 'python', 'migrator']
```

### Comparing `neo4j-python-migrations-0.1.0/setup.py` & `neo4j-python-migrations-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['attr>=0.3.2,<0.4.0',
  'neo4j>=5.1.0,<6.0.0',
  'typer>=0.6.1,<0.7.0',
  'yarl>=1.8.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'neo4j-python-migrations',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A database migration tool for Neo4j that allows to apply Cypher-based and arbitrary Python-based migrations.',
     'long_description': '![python version](https://img.shields.io/pypi/pyversions/neo4j-python-migrations?style=for-the-badge) \n[![version](https://img.shields.io/pypi/v/neo4j-python-migrations?style=for-the-badge)](https://pypi.org/project/neo4j-python-migrations/)\n![Codecov](https://img.shields.io/codecov/c/github/booqoffsky/neo4j-python-migrations?style=for-the-badge&token=CP9ZKK430Z)\n\n# neo4j-python-migrations\n\n> It is a database migration tool for [Neo4j](http://neo4j.com) written in Python\n> that allows to apply not only Cypher migrations, but also arbitrary Python-based migrations.\n> \n> This tool is inspired by [Michael Simons tool for Java](https://github.com/michael-simons/neo4j-migrations)\n> and works directly on [neo4j-python-driver](https://github.com/neo4j/neo4j-python-driver).\n\n# Features\n- Python migration support makes it possible to do any things in your migration that Python allows you to do.\n- Cypher-based migrations support.\n- It can be used either via the command line or directly in your code.\n- Multi-database support for Neo4j Enterprise Edition users.\n- The ability to separate logically independent migration chains within a single database (see the `project` option).\nMay be useful for Neo4j Community Edition users.\n\n# Installation\nFrom PyPi:\n\n`pip3 install neo4j-python-migrations`\n\nIf you want to install it from sources, try this:\n\n```\npython3 -m pip install poetry\npython3 -m pip install .\npython3 -m neo4j_python_migrations \n```\n\n# Usage\n## Creating migrations\n### Naming Convention\nEach migration will be a Cypher or Python file following the format `V<sem_ver>__<migration_name>.ext`.\n\nMake sure to follow the naming convention as stated in \n[Michael\'s tool documentation](https://michael-simons.github.io/neo4j-migrations/current/#concepts_naming-conventions)\n(except that .py files are allowed).\n\n### Cypher\nJust create a Cypher file with your custom script, for example `./migrations/V0001__initial.cypher`:\n```\nCREATE CONSTRAINT UniqueAuthor IF NOT EXISTS ON (a:AUTHOR) ASSERT a.uuid IS UNIQUE;\nCREATE INDEX author_uuid_index IF NOT EXISTS FOR (a:AUTHOR) ON (a.uuid);\n```\nThis script will be executed within a single transaction.\nTherefore, if you need both DDL and DML commands, split them into different files.\n\n### Python\nPython-based migrations should have a special format, for example `./migrations/V0002__drop_index.py`:\n```\nfrom neo4j import Session\n\n\n# This function must be present\ndef up(session: Session):\n    with session.begin_transaction() as tx:\n        tx.run("DROP INDEX author_uuid_index")\n```\n\n## Applying migrations\n### CLI\nYou can apply migrations or verify the status of migrations using the command line interface:\n```\nUsage: python -m neo4j_python_migrations [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --username TEXT                 The login of the user connecting to the\n                                  database.  [env var: NEO4J_MIGRATIONS_USER;\n                                  default: neo4j]\n  --password TEXT                 The password of the user connecting to the\n                                  database.  [env var: NEO4J_MIGRATIONS_PASS;\n                                  required]\n  --path PATH                     The path to the directory for scanning\n                                  migration files.  [env var:\n                                  NEO4J_MIGRATIONS_PATH; required]\n  --port INTEGER                  Port for connecting to the database  [env\n                                  var: NEO4J_MIGRATIONS_PORT; default: 7687]\n  --host TEXT                     Host for connecting to the database  [env\n                                  var: NEO4J_MIGRATIONS_HOST; default:\n                                  127.0.0.1]\n  --scheme TEXT                   Scheme for connecting to the database\n                                  [default: neo4j]\n  --project TEXT                  The name of the project for separating\n                                  logically independent migration chains\n                                  within a single database.  [env var:\n                                  NEO4J_MIGRATIONS_PROJECT]\n  --schema-database TEXT          The database that should be used for storing\n                                  information about migrations (Neo4j EE). If\n                                  not specified, then the database that should\n                                  be migrated is used.  [env var:\n                                  NEO4J_MIGRATIONS_SCHEMA_DATABASE]\n  --database TEXT                 The database that should be migrated (Neo4j\n                                  EE)  [env var: NEO4J_MIGRATIONS_DATABASE]\n  --install-completion [bash|zsh|fish|powershell|pwsh]\n                                  Install completion for the specified shell.\n  --show-completion [bash|zsh|fish|powershell|pwsh]\n                                  Show completion for the specified shell, to\n                                  copy it or customize the installation.\n  --help                          Show this message and exit.\n\nCommands:\n  analyze  Analyze migrations, find pending and missed.\n  migrate  Retrieves all pending migrations, verify and applies them.\n```\n\nSo, to apply migrations, just run the command:\n\n`python3 -m neo4j_python_migrations --username neo4j --password test --path ./migrations migrate`\n\n_Note: it is more secure to store the password in the environment variable NEO4J_MIGRATIONS_PASS._\n\n### Python Code\nYou can apply migrations directly into your application:\n\n```\nfrom pathlib import Path\n\nfrom neo4j import GraphDatabase\n\nfrom neo4j_python_migrations.executor import Executor\n\nwith GraphDatabase.driver("neo4j://localhost:7687", auth=("neo4j", "test")) as driver:\n    executor = Executor(driver, migrations_path=Path("./migrations"))\n    executor.migrate()\n```\nAvailable methods: `migrate`, `analyze`. \n\n# How migrations are tracked\nInformation about the applied migrations is stored in the database using the schema\ndescribed in [Michael\'s README](https://michael-simons.github.io/neo4j-migrations/current/#concepts_chain).\n\nSupported migration types: СYPHER, PYTHON. Other types of migrations, such as JAVA, are not supported.\n\nNote: the `project` option are incompatible with this schema. \nWhen using the option, each migration nodes will have an additional property named `project`.\n\n\n',
     'author': 'Grigory Bukovsky',
     'author_email': 'booqoffsky@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/booqoffsky/neo4j-python-migrations',
```

### Comparing `neo4j-python-migrations-0.1.0/PKG-INFO` & `neo4j-python-migrations-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4j-python-migrations
-Version: 0.1.0
+Version: 0.1.1
 Summary: A database migration tool for Neo4j that allows to apply Cypher-based and arbitrary Python-based migrations.
 Home-page: https://github.com/booqoffsky/neo4j-python-migrations
 License: MIT
 Keywords: neo4j,migrations,python,migrator
 Author: Grigory Bukovsky
 Author-email: booqoffsky@yandex.ru
 Requires-Python: >=3.8,<4.0
```

