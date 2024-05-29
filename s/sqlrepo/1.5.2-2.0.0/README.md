# Comparing `tmp/sqlrepo-1.5.2.tar.gz` & `tmp/sqlrepo-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlrepo-1.5.2.tar", last modified: Thu May 16 08:20:16 2024, max compression
+gzip compressed data, was "sqlrepo-2.0.0.tar", last modified: Wed May 29 13:24:34 2024, max compression
```

## Comparing `sqlrepo-1.5.2.tar` & `sqlrepo-2.0.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0    12676 2024-05-16 07:23:01.665324 sqlrepo-1.5.2/README.md
--rw-r--r--   0        0        0     3124 2024-05-16 08:20:16.564365 sqlrepo-1.5.2/pyproject.toml
--rw-r--r--   0        0        0       37 2024-01-16 08:47:35.121506 sqlrepo-1.5.2/sqlrepo/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2024-01-16 08:47:35.121506 sqlrepo-1.5.2/sqlrepo/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2024-01-16 08:47:35.121506 sqlrepo-1.5.2/sqlrepo/.pytest_cache/README.md
--rw-r--r--   0        0        0      130 2024-01-16 08:47:35.121506 sqlrepo-1.5.2/sqlrepo/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2024-01-16 08:47:35.121506 sqlrepo-1.5.2/sqlrepo/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      463 2024-04-15 09:56:07.307086 sqlrepo-1.5.2/sqlrepo/__init__.py
--rw-r--r--   0        0        0      828 2024-04-22 06:04:46.395911 sqlrepo-1.5.2/sqlrepo/exc.py
--rw-r--r--   0        0        0        0 2024-05-15 07:58:11.149780 sqlrepo-1.5.2/sqlrepo/ext/__init__.py
--rw-r--r--   0        0        0      368 2024-05-16 07:19:23.476470 sqlrepo-1.5.2/sqlrepo/ext/fastapi/__init__.py
--rw-r--r--   0        0        0     2401 2024-05-16 08:19:03.145736 sqlrepo-1.5.2/sqlrepo/ext/fastapi/containers.py
--rw-r--r--   0        0        0      186 2024-05-16 07:10:05.345399 sqlrepo-1.5.2/sqlrepo/ext/fastapi/helpers.py
--rw-r--r--   0        0        0     7935 2024-05-16 07:04:51.952120 sqlrepo-1.5.2/sqlrepo/ext/fastapi/services.py
--rw-r--r--   0        0        0      798 2024-04-15 09:17:49.278046 sqlrepo-1.5.2/sqlrepo/logging.py
--rw-r--r--   0        0        0        0 2024-04-16 08:40:42.695391 sqlrepo-1.5.2/sqlrepo/py.typed
--rw-r--r--   0        0        0    32880 2024-04-22 06:04:46.396911 sqlrepo-1.5.2/sqlrepo/queries.py
--rw-r--r--   0        0        0    23853 2024-04-22 06:04:46.396911 sqlrepo-1.5.2/sqlrepo/repositories.py
--rw-r--r--   0        0        0     4728 2024-05-16 08:19:43.301533 sqlrepo-1.5.2/sqlrepo/uow.py
--rw-r--r--   0        0        0     1202 2024-05-15 13:59:23.791626 sqlrepo-1.5.2/sqlrepo/wrappers.py
--rw-r--r--   0        0        0        0 2023-12-29 20:17:14.670751 sqlrepo-1.5.2/tests/__init__.py
--rw-r--r--   0        0        0     8306 2024-04-18 09:54:19.867457 sqlrepo-1.5.2/tests/conftest.py
--rw-r--r--   0        0        0    14662 2024-04-19 14:00:47.946165 sqlrepo-1.5.2/tests/test_async_queries.py
--rw-r--r--   0        0        0    11193 2024-04-19 13:59:20.466566 sqlrepo-1.5.2/tests/test_async_repositories.py
--rw-r--r--   0        0        0     1771 2024-04-22 06:04:46.396911 sqlrepo-1.5.2/tests/test_async_uow.py
--rw-r--r--   0        0        0    17037 2024-04-22 06:04:46.397911 sqlrepo-1.5.2/tests/test_base_queries.py
--rw-r--r--   0        0        0     2983 2024-04-22 06:04:46.397911 sqlrepo-1.5.2/tests/test_base_repositories.py
--rw-r--r--   0        0        0    10769 2024-05-16 07:09:22.500629 sqlrepo-1.5.2/tests/test_fastapi_ext.py
--rw-r--r--   0        0        0    13863 2024-04-19 13:47:29.322240 sqlrepo-1.5.2/tests/test_sync_queries.py
--rw-r--r--   0        0        0    10428 2024-04-19 13:50:29.889774 sqlrepo-1.5.2/tests/test_sync_repositories.py
--rw-r--r--   0        0        0     1540 2024-04-22 06:04:46.397911 sqlrepo-1.5.2/tests/test_sync_uow.py
--rw-r--r--   0        0        0     1061 2024-04-22 06:04:46.397911 sqlrepo-1.5.2/tests/test_wrappers.py
--rw-r--r--   0        0        0      804 2024-04-15 06:16:49.991950 sqlrepo-1.5.2/tests/types.py
--rw-r--r--   0        0        0     7155 2024-04-19 14:04:27.333651 sqlrepo-1.5.2/tests/utils.py
--rw-r--r--   0        0        0    13104 1970-01-01 00:00:00.000000 sqlrepo-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0    12676 2024-05-16 07:23:01.665324 sqlrepo-2.0.0/README.md
+-rw-r--r--   0        0        0     3123 2024-05-29 13:24:34.611908 sqlrepo-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-01-16 08:47:35.121506 sqlrepo-2.0.0/sqlrepo/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2024-01-16 08:47:35.121506 sqlrepo-2.0.0/sqlrepo/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2024-01-16 08:47:35.121506 sqlrepo-2.0.0/sqlrepo/.pytest_cache/README.md
+-rw-r--r--   0        0        0      130 2024-01-16 08:47:35.121506 sqlrepo-2.0.0/sqlrepo/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2024-01-16 08:47:35.121506 sqlrepo-2.0.0/sqlrepo/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      463 2024-04-15 09:56:07.307086 sqlrepo-2.0.0/sqlrepo/__init__.py
+-rw-r--r--   0        0        0      828 2024-04-22 06:04:46.395911 sqlrepo-2.0.0/sqlrepo/exc.py
+-rw-r--r--   0        0        0        0 2024-05-15 07:58:11.149780 sqlrepo-2.0.0/sqlrepo/ext/__init__.py
+-rw-r--r--   0        0        0      368 2024-05-16 07:19:23.476470 sqlrepo-2.0.0/sqlrepo/ext/fastapi/__init__.py
+-rw-r--r--   0        0        0     2401 2024-05-16 08:19:03.145736 sqlrepo-2.0.0/sqlrepo/ext/fastapi/containers.py
+-rw-r--r--   0        0        0      186 2024-05-16 07:10:05.345399 sqlrepo-2.0.0/sqlrepo/ext/fastapi/helpers.py
+-rw-r--r--   0        0        0     3450 2024-05-29 13:23:14.646263 sqlrepo-2.0.0/sqlrepo/ext/fastapi/pagination.py
+-rw-r--r--   0        0        0     8355 2024-05-29 13:11:42.398804 sqlrepo-2.0.0/sqlrepo/ext/fastapi/services.py
+-rw-r--r--   0        0        0      798 2024-04-15 09:17:49.278046 sqlrepo-2.0.0/sqlrepo/logging.py
+-rw-r--r--   0        0        0        0 2024-04-16 08:40:42.695391 sqlrepo-2.0.0/sqlrepo/py.typed
+-rw-r--r--   0        0        0    32880 2024-04-22 06:04:46.396911 sqlrepo-2.0.0/sqlrepo/queries.py
+-rw-r--r--   0        0        0    23853 2024-04-22 06:04:46.396911 sqlrepo-2.0.0/sqlrepo/repositories.py
+-rw-r--r--   0        0        0     4728 2024-05-16 08:19:43.301533 sqlrepo-2.0.0/sqlrepo/uow.py
+-rw-r--r--   0        0        0     1202 2024-05-15 13:59:23.791626 sqlrepo-2.0.0/sqlrepo/wrappers.py
+-rw-r--r--   0        0        0        0 2023-12-29 20:17:14.670751 sqlrepo-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     8306 2024-04-18 09:54:19.867457 sqlrepo-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0    14662 2024-04-19 14:00:47.946165 sqlrepo-2.0.0/tests/test_async_queries.py
+-rw-r--r--   0        0        0    11193 2024-04-19 13:59:20.466566 sqlrepo-2.0.0/tests/test_async_repositories.py
+-rw-r--r--   0        0        0     1771 2024-04-22 06:04:46.396911 sqlrepo-2.0.0/tests/test_async_uow.py
+-rw-r--r--   0        0        0    17037 2024-04-22 06:04:46.397911 sqlrepo-2.0.0/tests/test_base_queries.py
+-rw-r--r--   0        0        0     2983 2024-04-22 06:04:46.397911 sqlrepo-2.0.0/tests/test_base_repositories.py
+-rw-r--r--   0        0        0    14278 2024-05-29 13:21:18.994737 sqlrepo-2.0.0/tests/test_fastapi_ext.py
+-rw-r--r--   0        0        0    13863 2024-04-19 13:47:29.322240 sqlrepo-2.0.0/tests/test_sync_queries.py
+-rw-r--r--   0        0        0    10428 2024-04-19 13:50:29.889774 sqlrepo-2.0.0/tests/test_sync_repositories.py
+-rw-r--r--   0        0        0     1540 2024-04-22 06:04:46.397911 sqlrepo-2.0.0/tests/test_sync_uow.py
+-rw-r--r--   0        0        0     1061 2024-04-22 06:04:46.397911 sqlrepo-2.0.0/tests/test_wrappers.py
+-rw-r--r--   0        0        0      804 2024-04-15 06:16:49.991950 sqlrepo-2.0.0/tests/types.py
+-rw-r--r--   0        0        0     7155 2024-04-19 14:04:27.333651 sqlrepo-2.0.0/tests/utils.py
+-rw-r--r--   0        0        0    13103 1970-01-01 00:00:00.000000 sqlrepo-2.0.0/PKG-INFO
```

### Comparing `sqlrepo-1.5.2/README.md` & `sqlrepo-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/pyproject.toml` & `sqlrepo-2.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -172,24 +172,24 @@
     "httpx>=0.27.0",
     "pyment>=0.3.3",
     "ipython>=8.19.0",
 ]
 
 [project]
 name = "sqlrepo"
-version = "1.5.2"
+version = "2.0.0"
 description = "sqlalchemy repositories with crud operations and other utils for it."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = [
     "sqlalchemy>=2.0.29",
-    "python-dev-utils[sqlalchemy_filters]>=1.11.0",
+    "python-dev-utils[sqlalchemy_filters]>=2.2.0",
 ]
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 fastapi = [
```

### Comparing `sqlrepo-1.5.2/sqlrepo/exc.py` & `sqlrepo-2.0.0/sqlrepo/exc.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/sqlrepo/ext/fastapi/containers.py` & `sqlrepo-2.0.0/sqlrepo/ext/fastapi/containers.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/sqlrepo/ext/fastapi/services.py` & `sqlrepo-2.0.0/sqlrepo/ext/fastapi/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from dev_utils.verbose_http_exceptions import BaseVerboseHTTPException
 from fastapi import HTTPException, status
 from pydantic import BaseModel, TypeAdapter
 from sqlalchemy.orm.decl_api import DeclarativeBase
 
 from sqlrepo.ext.fastapi.helpers import NotSet, NotSetType
+from sqlrepo.ext.fastapi.pagination import PaginatedResult, PaginationMeta
 from sqlrepo.logging import logger
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from fastapi import Request
     from sqlalchemy.ext.asyncio import AsyncSession
@@ -150,14 +151,25 @@
     def resolve_entity_list(self, entities: "Sequence[TModel]") -> "list[VListSchema]":
         """Resolve given SQLAlchemy entity and return pydantic schema."""
         if isinstance(self.list_schema, NotSetType):
             msg = "list_schema must be set, if you use resolve_entity in your code."
             raise AttributeError(msg)  # noqa: TRY004
         return TypeAdapter(list[self.list_schema]).validate_python(entities, from_attributes=True)
 
+    def paginate_result(
+        self,
+        entities: "Sequence[TModel]",
+        meta: PaginationMeta,
+    ) -> PaginatedResult["VListSchema"]:
+        """Resolve list if entities and put them into pagination."""
+        return PaginatedResult(
+            meta=meta,
+            data=self.resolve_entity_list(entities=entities),
+        )
+
 
 class BaseAsyncService(BaseService[TModel, TDetailSchema, VListSchema]):
     """Base service with async interface."""
 
     __inheritance_check_model_class__: bool = False
 
     def init_repositories(self, session: "AsyncSession") -> None:
```

### Comparing `sqlrepo-1.5.2/sqlrepo/logging.py` & `sqlrepo-2.0.0/sqlrepo/logging.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/sqlrepo/queries.py` & `sqlrepo-2.0.0/sqlrepo/queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/sqlrepo/repositories.py` & `sqlrepo-2.0.0/sqlrepo/repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/sqlrepo/uow.py` & `sqlrepo-2.0.0/sqlrepo/uow.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/sqlrepo/wrappers.py` & `sqlrepo-2.0.0/sqlrepo/wrappers.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/tests/conftest.py` & `sqlrepo-2.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/tests/test_async_queries.py` & `sqlrepo-2.0.0/tests/test_async_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/tests/test_async_repositories.py` & `sqlrepo-2.0.0/tests/test_async_repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/tests/test_async_uow.py` & `sqlrepo-2.0.0/tests/test_async_uow.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/tests/test_base_queries.py` & `sqlrepo-2.0.0/tests/test_base_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/tests/test_base_repositories.py` & `sqlrepo-2.0.0/tests/test_base_repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/tests/test_fastapi_ext.py` & `sqlrepo-2.0.0/tests/test_fastapi_ext.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,17 +8,24 @@
 from fastapi import Depends, FastAPI, HTTPException, Path, status
 from fastapi.testclient import TestClient
 from mimesis import Datetime, Locale, Text
 from pydantic import BaseModel, ConfigDict, TypeAdapter
 from sqlalchemy.orm.session import Session
 
 from sqlrepo.ext.fastapi import BaseSyncContainer, BaseSyncService, add_container_overrides
+from sqlrepo.ext.fastapi.pagination import (
+    AbstractBasePagination,
+    LimitOffsetPagination,
+    PageSizePagination,
+    PaginatedResult,
+    PaginationMeta,
+)
 from sqlrepo.ext.fastapi.services import NotSet, ServiceClassIncorrectUseWarning
 from sqlrepo.repositories import BaseSyncRepository
-from tests.utils import MyModel
+from tests.utils import MyModel, assert_compare_db_item_with_dict
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
     from sqlalchemy.orm import Session, sessionmaker
 
     from tests.types import SyncFactoryFunctionProtocol
@@ -67,14 +74,26 @@
         entity = self.my_model_repo.get(filters={"id": my_model_id})
         return self.resolve_entity(entity)
 
     def list(self) -> list[MyModelList]:  # noqa: D102
         entities = self.my_model_repo.list()
         return self.resolve_entity_list(entities)
 
+    def list_paginated(  # noqa: D102
+        self,
+        pagination: AbstractBasePagination,
+    ) -> PaginatedResult[MyModelList]:
+        entities = self.my_model_repo.list(limit=pagination.limit, offset=pagination.offset)
+        total_count = self.my_model_repo.count()
+        meta = PaginationMeta.create(
+            all_records_count=total_count,
+            pagination=pagination,
+        )
+        return self.paginate_result(entities, meta)
+
 
 class InvalidService(MyModelService):  # noqa: D101
     ...
 
 
 InvalidService.detail_schema = NotSet  # type: ignore
 InvalidService.list_schema = NotSet  # type: ignore
@@ -155,14 +174,28 @@
     def get_one_python(my_model_id: int = Path(), container: Container = Depends()):  # type: ignore # noqa: ANN202
         return container.my_model_with_python_error.get_by_id(my_model_id)
 
     @app.get('/get-all/')
     def get_all(container: Container = Depends()):  # type: ignore # noqa: ANN202
         return container.my_model_service.list()
 
+    @app.get('/get-limit-offset-paginated/')
+    def get_paginated_limit_offset(  # type: ignore # noqa: ANN202
+        pagination: LimitOffsetPagination = Depends(),
+        container: Container = Depends(),
+    ):
+        return container.my_model_service.list_paginated(pagination)
+
+    @app.get('/get-page-size-paginated/')
+    def get_paginated_page_size(  # type: ignore # noqa: ANN202
+        pagination: PageSizePagination = Depends(),
+        container: Container = Depends(),
+    ):
+        return container.my_model_service.list_paginated(pagination)
+
     @app.get('/get-all-invalid/')
     def get_all_invalid(container: Container = Depends()):  # type: ignore # noqa: ANN202
         return container.invalid_service.list()
 
     return TestClient(app)
 
 
@@ -218,14 +251,66 @@
     db_sync_session: "Session",
     app_with_sync_container: "TestClient",
 ) -> None:
     with pytest.raises(ValueError, match="MyModel entity not found."):
         app_with_sync_container.get('/get-one-python/1251251')
 
 
+def test_limit_offset_pagination(
+    db_sync_session: "Session",
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
+    app_with_sync_container: "TestClient",
+) -> None:
+
+    items = [mymodel_sync_factory(db_sync_session, commit=False) for _ in range(3)]
+    items_map = {item.id: item for item in items}
+    db_sync_session.commit()
+    response = app_with_sync_container.get('/get-limit-offset-paginated/?limit=1')
+    assert response.status_code == status.HTTP_200_OK
+    response = response.json()
+    schema = TypeAdapter(PaginatedResult[MyModelList]).validate_python(response)
+    assert schema.meta.all_pages_count == len(items)
+    assert schema.meta.filtered_pages_count == len(items)
+    assert schema.meta.all_records_count == len(items)
+    assert schema.meta.filtered_records_count == len(items)
+    assert schema.meta.per_page == 1
+    assert schema.meta.current_page == 1
+    assert schema.meta.prev_page is None
+    assert schema.meta.next_page == 2  # noqa: PLR2004
+    for item in schema.data:
+        assert item.id in items_map
+        assert_compare_db_item_with_dict(items_map[item.id], item.model_dump())
+
+
+def test_page_size_pagination(
+    db_sync_session: "Session",
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
+    app_with_sync_container: "TestClient",
+) -> None:
+
+    items = [mymodel_sync_factory(db_sync_session, commit=False) for _ in range(3)]
+    items_map = {item.id: item for item in items}
+    db_sync_session.commit()
+    response = app_with_sync_container.get('/get-page-size-paginated/?per_page=1')
+    assert response.status_code == status.HTTP_200_OK
+    response = response.json()
+    schema = TypeAdapter(PaginatedResult[MyModelList]).validate_python(response)
+    assert schema.meta.all_pages_count == len(items)
+    assert schema.meta.filtered_pages_count == len(items)
+    assert schema.meta.all_records_count == len(items)
+    assert schema.meta.filtered_records_count == len(items)
+    assert schema.meta.per_page == 1
+    assert schema.meta.current_page == 1
+    assert schema.meta.prev_page is None
+    assert schema.meta.next_page == 2  # noqa: PLR2004
+    for item in schema.data:
+        assert item.id in items_map
+        assert_compare_db_item_with_dict(items_map[item.id], item.model_dump())
+
+
 def test_get_all(
     db_sync_session: "Session",
     mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
     app_with_sync_container: "TestClient",
 ) -> None:
     ids = {mymodel_sync_factory(db_sync_session).id, mymodel_sync_factory(db_sync_session).id}
     db_sync_session.commit()
```

### Comparing `sqlrepo-1.5.2/tests/test_sync_queries.py` & `sqlrepo-2.0.0/tests/test_sync_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/tests/test_sync_repositories.py` & `sqlrepo-2.0.0/tests/test_sync_repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/tests/test_sync_uow.py` & `sqlrepo-2.0.0/tests/test_sync_uow.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/tests/test_wrappers.py` & `sqlrepo-2.0.0/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/tests/types.py` & `sqlrepo-2.0.0/tests/types.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/tests/utils.py` & `sqlrepo-2.0.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.5.2/PKG-INFO` & `sqlrepo-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sqlrepo
-Version: 1.5.2
+Version: 2.0.0
 Summary: sqlalchemy repositories with crud operations and other utils for it.
 Author-Email: Dmitriy Lunev <dima.lunev14@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: sqlalchemy>=2.0.29
-Requires-Dist: python-dev-utils[sqlalchemy_filters]>=1.11.0
+Requires-Dist: python-dev-utils[sqlalchemy_filters]>=2.2.0
 Requires-Dist: fastapi>=0.100; extra == "fastapi"
 Provides-Extra: fastapi
 Description-Content-Type: text/markdown
 
 # sqlrepo
 
 ![coverage](./coverage.svg)
```

