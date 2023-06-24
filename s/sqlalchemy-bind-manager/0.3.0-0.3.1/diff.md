# Comparing `tmp/sqlalchemy_bind_manager-0.3.0.tar.gz` & `tmp/sqlalchemy_bind_manager-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_bind_manager-0.3.0.tar", max compression
+gzip compressed data, was "sqlalchemy_bind_manager-0.3.1.tar", max compression
```

## Comparing `sqlalchemy_bind_manager-0.3.0.tar` & `sqlalchemy_bind_manager-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1073 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/LICENSE
--rw-r--r--   0        0        0    12017 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/README.md
--rw-r--r--   0        0        0     2103 2023-06-18 17:43:39.487600 sqlalchemy_bind_manager-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      107 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/__init__.py
--rw-r--r--   0        0        0     5241 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_bind_manager.py
--rw-r--r--   0        0        0      204 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/__init__.py
--rw-r--r--   0        0        0     5734 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/async_.py
--rw-r--r--   0        0        0     8738 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/base_repository.py
--rw-r--r--   0        0        0      937 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/common.py
--rw-r--r--   0        0        0     7429 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/result_presenters.py
--rw-r--r--   0        0        0     5731 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/sync.py
--rw-r--r--   0        0        0     3125 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_transaction_handler.py
--rw-r--r--   0        0        0     1722 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_unit_of_work.py
--rw-r--r--   0        0        0      310 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/exceptions.py
--rw-r--r--   0        0        0    10354 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/protocols.py
--rw-r--r--   0        0        0        0 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/py.typed
--rw-r--r--   0        0        0      242 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/repository.py
--rw-r--r--   0        0        0    13411 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/LICENSE
+-rw-r--r--   0        0        0    11983 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/README.md
+-rw-r--r--   0        0        0     2244 2023-06-24 15:01:03.217054 sqlalchemy_bind_manager-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/__init__.py
+-rw-r--r--   0        0        0     5241 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_bind_manager.py
+-rw-r--r--   0        0        0      197 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/__init__.py
+-rw-r--r--   0        0        0     5734 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/async_.py
+-rw-r--r--   0        0        0    11340 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/base_repository.py
+-rw-r--r--   0        0        0     1099 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/common.py
+-rw-r--r--   0        0        0     7429 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/result_presenters.py
+-rw-r--r--   0        0        0     5045 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/sync.py
+-rw-r--r--   0        0        0     3125 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_transaction_handler.py
+-rw-r--r--   0        0        0     1722 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_unit_of_work.py
+-rw-r--r--   0        0        0      310 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/exceptions.py
+-rw-r--r--   0        0        0    10397 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/protocols.py
+-rw-r--r--   0        0        0        0 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/py.typed
+-rw-r--r--   0        0        0      242 2023-06-24 15:00:50.468903 sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/repository.py
+-rw-r--r--   0        0        0    13376 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.3.1/PKG-INFO
```

### Comparing `sqlalchemy_bind_manager-0.3.0/LICENSE` & `sqlalchemy_bind_manager-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.0/README.md` & `sqlalchemy_bind_manager-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 This package provides an easy way to configure and use SQLAlchemy engines and sessions
 without depending on frameworks.
 
 It is composed by two main components:
 
-* A manager class for SQLAlchemy engine configuration
+* A manager class for SQLAlchemy engine and session configuration
 * A repository/unit-of-work pattern implementation for model retrieval and persistence
 
 ## Installation
 
 ```bash
 pip install sqlalchemy-bind-manager
 ```
@@ -48,26 +48,25 @@
 )
 
 sa_manager = SQLAlchemyBindManager(config)
 ```
 
 🚨 NOTE: Using global variables is not thread-safe, please read the [Threading](#threading) section if your application uses multi-threading.
 
-`engine_url` and `engine_options` dictionary accept the same parameters as SQLAlchemy [create_engine()](https://docs.sqlalchemy.org/en/14/core/engines.html#sqlalchemy.create_engine)
+The `engine_url` and `engine_options` dictionaries accept the same parameters as SQLAlchemy [create_engine()](https://docs.sqlalchemy.org/en/14/core/engines.html#sqlalchemy.create_engine)
 
-`session_options` dictionary accepts the same parameters as SQLALchemy [sessionmaker()](https://docs.sqlalchemy.org/en/14/orm/session_api.html#sqlalchemy.orm.sessionmaker)
+The `session_options` dictionary accepts the same parameters as SQLALchemy [sessionmaker()](https://docs.sqlalchemy.org/en/14/orm/session_api.html#sqlalchemy.orm.sessionmaker)
 
 Once the bind manager is initialised we can retrieve and use the SQLAlchemyBind using the method `get_bind()`
 
-The `SQLAlchemyBind` class has the following attributes:
+The `SQLAlchemyBind` and `SQLAlchemyAsyncBind` class has the following attributes:
 
-* `bind_async`: A boolean property, `True` when the bind uses an async dialect (Note: async is not yet fully supported, see the section about asynchronous binds)
 * `engine`: The initialised SQLALchemy `Engine`
 * `model_declarative_base`: A base class that can be used to create [declarative models](https://docs.sqlalchemy.org/en/14/orm/mapping_styles.html#declarative-mapping)
-* `registry_mapper`: The `registry` associated with the `engine`. It can be used with Alembic or to achieve [imperative mapping](https://docs.sqlalchemy.org/en/14/orm/mapping_styles.html#imperative-mapping)
+* `registry_mapper`: The `registry` associated with the `engine`. It can be used with Alembic or to setup [imperative mapping](https://docs.sqlalchemy.org/en/14/orm/mapping_styles.html#imperative-mapping)
 * `session_class`: The class built by [sessionmaker()](https://docs.sqlalchemy.org/en/14/orm/session_api.html#sqlalchemy.orm.sessionmaker), either `Session` or `AsyncSession`
 
 The `SQLAlchemyBindManager` provides some helper methods to quickly access some of the bind properties without using the `SQLAlchemyBind`:
 
 * `get_session`: returns a Session object
 * `get_mapper`: returns the mapper associated with the bind
 
@@ -137,24 +136,39 @@
 All the `SQLAlchemyBindManager` helper methods accept the `bind_name` optional parameter:
 
 * `get_session(bind_name="default")`: returns a `Session` or `AsyncSession` object
 * `get_mapper(bind_name="default")`: returns the mapper associated with the bind
 
 ### Threading
 
-Global variables in python are shared among threads. Neither `SQLAlchemyBindManager` class
-or the repositories implementation are thread safe on their own.
+Global variables are shared between different threads in python. If your application uses
+multiple threads, like spawning a thread per request, then you should not store an
+initialised session in a global variable, otherwise the state of your models will be shared
+among the threads and produce undesired changes in the database.
 
-If your application uses multi-threads, the same `SQLAlchemyBindManager` object will be
-shared between different threads, together with the internal `Session` object,
-and changes on models could propagate among them, causing undesired operations.
-
-Make sure you check Python [Threading](https://docs.python.org/3/library/threading.html)
-documentation, especially the [Thread-local Data](https://docs.python.org/3/library/threading.html#thread-local-data)
-chapter to avoid issues.
+This is not thread safe:
+
+```python
+session = sa_manager.get_session()
+session.add(model)
+session.commit()
+```
+
+If you truly need to have a long-lived session you'll need to use a scoped session,
+something like this:
+
+```python
+from sqlalchemy.orm import scoped_session
+
+session = scoped_session(sa_manager.get_bind().session_class())
+```
+
+Handling the life cycle of scoped sessions is not supported by this documentations.
+Please refer to [SQLAlchemy documentation](https://docs.sqlalchemy.org/en/20/orm/contextual.html)
+about this.
 
 ### Asynchronous database binds
 
 Is it possible to supply configurations for asyncio supported engines.
 
 ```python
 config = SQLAlchemyAsyncConfig(
@@ -171,29 +185,34 @@
 ```
 
 Note that async implementation has several differences from the sync one, make sure
 to check [SQLAlchemy asyncio documentation](https://docs.sqlalchemy.org/en/20/orm/extensions/asyncio.html)
 
 ## Repository / Unit of work
 
-The `SQLAlchemyRepository` and `SQLAlchemyAsyncRepository` class can be used simply by extending them.
+The `SQLAlchemyRepository` and `SQLAlchemyAsyncRepository` class can be used directly or by extending them.
 
 ```python
 from sqlalchemy_bind_manager.repository import SQLAlchemyRepository
 
 
 class MyModel(model_declarative_base):
     pass
 
+# Direct usage
+repo_instance = SQLAlchemyRepository(sqlalchemy_bind_manager.get_bind(), model_class=MyModel)
 
 class ModelRepository(SQLAlchemyRepository[MyModel]):
     _model = MyModel
+    
+    def _some_custom_method_implemented(self):
+        ...
 
-
-repo_instance = ModelRepository(sqlalchemy_bind_manager.get_bind())
+# Extended class usage
+extended_repo_instance = ModelRepository(sqlalchemy_bind_manager.get_bind())
 ```
 
 The classes provide some common use methods:
 
 * `get`: Retrieve a model by identifier
 * `save`: Persist a model
 * `save_many`: Persist multiple models in a single transaction
@@ -209,42 +228,40 @@
 database access is potentially anticipated.
 
 Doing this too soon might cause unexpected effects, like unexpected updates being committed,
 if the initialised session is shared among different repositories.
 
 A `Repository` represents a generic interface to persist data object to a storage, not necessarily
 using SQLAlchemy. It makes sense that the lifecycle of a `Session` follows the one of the Repository
-(If we create a Repository, we're going to do a DB operation, otherwise we don't need a `Session`)
+(The assumption is: if we create a Repository, we're going to do a DB operation,
+otherwise we wouldn't need one).
 
-This ensures the `Session` we use is isolated, and the same for all the operations we do with the
-same repository.
+Each Repository instance create an internal scoped session. The session gets
+automatically closed when the Repository instance is not referenced by any variable (and the
+garbage collector clean it up)
+
+In this way we ensure the `Session` we use is isolated, and the same for all the operations we do with the
+same Repository. 
+
+This approach has a consequence: We can't use SQLAlchemy lazy loading, so we'll need to make sure relationship are always loaded eagerly,
+using either approach:
+* Setup your model/table relationships to always use always eager loading
+* Implement ad-hoc methods to deal with relationships as necessary
 
-The session is automatically closed and reopen with each Repository operation, this make sure these
-operation are independent from each other.
-
-These choices cause some consequences:
-* The operations that modify the database will reload the models from the DB, causing an additional
-  SELECT query to be issued.
-* We can't use SQLAlchemy lazy loading, so we'll need to make sure relationship are always loaded eagerly,
-  using either:
-  * Setup your model/table relationships to always use always eager loading
-  * Implement ad-hoc methods to deal with relationships as necessary
-
-Also `AsyncSession` has [the same limitation on lazy loading](https://docs.sqlalchemy.org/en/20/orm/extensions/asyncio.html#asyncio-orm-avoid-lazyloads)
-so it makes sense that the two repository implementations behave consistently.
+Note that `AsyncSession` has [the same limitation on lazy loading](https://docs.sqlalchemy.org/en/20/orm/extensions/asyncio.html#asyncio-orm-avoid-lazyloads),
+even when keeping the session opened, so it makes sense that the two Repository implementations behave consistently.
 
 ### Use the Unit Of Work to share a session among multiple repositories
 
-It is possible we need to run several operations in a single database get_session. While a single
+It is possible we need to run several operations in a single database transaction. While a single
 repository provide by itself an isolated session for single operations, we have to use a different
 approach for multiple operations.
 
 We can use the `UnitOfWork` or the `AsyncUnitOfWork` class to provide a shared session to
 be used for repository operations, **assumed the same bind is used for all the repositories**.
-(Two phase transactions are not currently supported).
 
 ```python
 class MyRepo(SQLAlchemyRepository):
     _model = MyModel
 class MyOtherRepo(SQLAlchemyRepository):
     _model = MyOtherModel
 
@@ -256,11 +273,7 @@
     uow.MyOtherRepo.save(some_other_model)
 
 # Optionally disable the commit/rollback handling
 with uow.transaction(read_only=True):
     model1 = uow.MyRepo.get(1)
     model2 = uow.MyOtherRepo.get(2)
 ```
-
-Both the UnitOfWork classes create an internal `scoped_session` or `async_scoped_session`, behaving
-in the same way at the repositories do. This provides the freedom to tune the session lifecycle based
-on our application requirements (e.g. one unit of work per http request, per domain, etc.)
```

### Comparing `sqlalchemy_bind_manager-0.3.0/pyproject.toml` & `sqlalchemy_bind_manager-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "sqlalchemy-bind-manager"
-version = "0.3.0"
+version = "0.3.1"
 description = "A manager to easily handle multiple SQLAlchemy configurations"
 license = "MIT"
 authors = ["Federico Busetti <729029+febus982@users.noreply.github.com>"]
 repository = "https://github.com/febus982/sqlalchemy-bind-manager"
+homepage = "https://febus982.github.io/sqlalchemy-bind-manager"
 readme = "README.md"
 packages = [{include = "sqlalchemy_bind_manager"}]
 keywords = ["sqlalchemy", "config", "manager"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: AsyncIO",
     "Framework :: Pydantic",
@@ -44,21 +45,24 @@
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 aiosqlite = "~0.18.0"
 coverage = "~6.5.0"
 black = "~22.10.0"
+mkdocs = "~1.4.3"
+mkdocs-material = "~9.1.16"
 mypy = "~0.990"
 pytest = "~7.2.0"
 pytest-asyncio = "~0.20.3"
 pytest-cov = "~4.0.0"
 pytest-factoryboy = "~2.5.0"
 pytest-xdist = "~3.0.2"
 ruff = "~0.0.263"
+pymdown-extensions = "^10.0.1"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 minversion = "6.0"
 addopts = "-n auto --cov-report=term-missing"
 testpaths = [
     "tests",
```

### Comparing `sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_bind_manager.py` & `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_bind_manager.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/async_.py` & `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/async_.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 from sqlalchemy.ext.asyncio import AsyncSession
 
 from .._bind_manager import SQLAlchemyAsyncBind
 from .._transaction_handler import AsyncSessionHandler
 from ..exceptions import InvalidConfig, ModelNotFound
 from .base_repository import (
     BaseRepository,
-    SortDirection,
 )
 from .common import (
     MODEL,
     PRIMARY_KEY,
     CursorPaginatedResult,
     CursorReference,
     PaginatedResult,
+    SortDirection,
 )
 from .result_presenters import CursorPaginatedResultPresenter, PaginatedResultPresenter
 
 
 class SQLAlchemyAsyncRepository(Generic[MODEL], BaseRepository[MODEL], ABC):
     _session_handler: AsyncSessionHandler
     _external_session: Union[AsyncSession, None]
```

### Comparing `sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/base_repository.py` & `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/base_repository.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 from abc import ABC
-from enum import Enum
-from functools import partial
 from typing import (
     Any,
     Generic,
     Iterable,
     Mapping,
     Tuple,
     Type,
     Union,
 )
 
-from sqlalchemy import asc, desc, func, inspect, select
+from sqlalchemy import asc, func, inspect, select
 from sqlalchemy.orm import Mapper, aliased, class_mapper, lazyload
 from sqlalchemy.orm.exc import UnmappedClassError
 from sqlalchemy.sql import Select
 
 from sqlalchemy_bind_manager.exceptions import InvalidModel, UnmappedProperty
 
 from .common import (
     MODEL,
     CursorReference,
+    SortDirection,
 )
 
 
-class SortDirection(Enum):
-    ASC = partial(asc)
-    DESC = partial(desc)
-
-
 class BaseRepository(Generic[MODEL], ABC):
     _max_query_limit: int = 50
     _model: Type[MODEL]
 
     def __init__(self, model_class: Union[Type[MODEL], None] = None) -> None:
         if getattr(self, "_model", None) is None and model_class is not None:
             self._model = model_class
@@ -78,14 +72,15 @@
 
         E.g.
         _filter_select(stmt, name="John") adds a `WHERE name = John` statement
 
         :param stmt: a Select statement
         :type stmt: Select
         :param search_params: Any keyword argument to be used as equality filter
+        :type search_params: Mapping[str, Any]
         :return: The filtered query
         """
         # TODO: Add support for relationship eager load
         for k, v in search_params.items():
             """
             This acts as a TypeGuard but using TypeGuard typing would break
             compatibility with python < 3.10, for the moment we prefer to ignore
@@ -106,14 +101,15 @@
 
         `_filter_order_by(stmt, [('name', SortDirection.ASC)])`
             adds a `ORDER BY name ASC` statement
 
         :param stmt: a Select statement
         :type stmt: Select
         :param order_by: a list of columns, or tuples (column, direction)
+        :type order_by: Iterable[Union[str, Tuple[str, SortDirection]]]
         :return: The filtered query
         """
         for value in order_by:
             if isinstance(value, str):
                 self._validate_mapped_property(value)
                 stmt = stmt.order_by(getattr(self._model, value))
             else:
@@ -123,14 +119,32 @@
         return stmt
 
     def _find_query(
         self,
         search_params: Union[None, Mapping[str, Any]] = None,
         order_by: Union[None, Iterable[Union[str, Tuple[str, SortDirection]]]] = None,
     ) -> Select:
+        """Build a query with column filters and orders.
+
+        E.g.
+        q = _find_query(search_params={"name":"John"})
+            finds all models with name = John
+
+        q = _find_query(order_by=["name"])
+            finds all models ordered by `name` column
+
+        q = _find_query(order_by=[("name", SortDirection.DESC)])
+            finds all models with reversed order by `name` column
+
+        :param search_params: Any keyword argument to be used as equality filter
+        :type search_params: Mapping[str, Any]
+        :param order_by: a list of columns, or tuples (column, direction)
+        :type order_by: Iterable[Union[str, Tuple[str, SortDirection]]]
+        :return: The filtered query
+        """
         stmt = select(self._model)
 
         if search_params:
             stmt = self._filter_select(stmt, search_params)
         if order_by is not None:
             stmt = self._filter_order_by(stmt, order_by)
 
@@ -173,94 +187,134 @@
     def _cursor_paginated_query(
         self,
         stmt: Select,
         cursor_reference: Union[CursorReference, None],
         is_before_cursor: bool = False,
         items_per_page: int = _max_query_limit,
     ) -> Select:
-        """Build the query offset and limit clauses from submitted parameters.
+        """Adds the clauses to retrieve the requested slice of models, after
+        or before the cursor value, plus a model before the slice and one after
+        the slice, to identify if previous or next results are available.
 
         :param stmt: a Select statement
         :type stmt: Select
-        :param before: Identifier of the last node to skip
-        :type before: Union[int, str]
-        :param after: Identifier of the last node to skip
-        :type after: Union[int, str]
+        :param cursor_reference: A cursor reference containing ordering column
+            and threshold value
+        :type cursor_reference: Union[CursorReference, None]
+        :param is_before_cursor: If True it will return items before the cursor,
+            otherwise items after
+        :type is_before_cursor: bool
         :param items_per_page: Number of models to retrieve
         :type items_per_page: int
         :return: The filtered query
         """
-
         forward_limit = self._sanitised_query_limit(items_per_page) + 1
 
         if not cursor_reference:
             return stmt.limit(forward_limit).order_by(  # type: ignore
                 asc(self._model_pk())
             )
 
-        # TODO: Use window functions
-        if not is_before_cursor:
-            previous_query = stmt.where(
-                getattr(self._model, cursor_reference.column) <= cursor_reference.value
-            )
-            previous_query = (
-                self._filter_order_by(
-                    previous_query, [(cursor_reference.column, SortDirection.DESC)]
-                )
-                .limit(1)
-                .subquery("previous")  # type: ignore
+        previous_query = self._cursor_pagination_previous_item_query(
+            stmt, cursor_reference, is_before_cursor
+        ).subquery("previous")
+
+        page_query = self._cursor_pagination_slice_query(
+            stmt, cursor_reference, forward_limit, is_before_cursor
+        ).subquery("slice")
+
+        query = select(
+            aliased(
+                self._model,
+                select(previous_query)
+                .union_all(select(page_query))
+                .order_by(cursor_reference.column)
+                .subquery("cursor_pagination"),  # type: ignore
             )
+        )
+        return query
+
+    def _cursor_pagination_slice_query(
+        self,
+        stmt: Select,
+        cursor_reference: CursorReference,
+        limit: int,
+        is_before_cursor: bool,
+    ):
+        """Adds the clauses to retrieve a requested slice of models,
+        after or before the cursor value (excluding the cursor itself)
 
+        :param stmt: a Select statement
+        :type stmt: Select
+        :param cursor_reference: A cursor reference containing ordering column
+            and threshold value
+        :type cursor_reference: Union[CursorReference, None]
+        :param is_before_cursor: If True it will return items before the cursor,
+            otherwise items after
+        :type is_before_cursor: bool
+        :param limit: Number of models to retrieve
+        :type limit: int
+        :return: The filtered query
+        """
+        if not is_before_cursor:
             page_query = stmt.where(
                 getattr(self._model, cursor_reference.column) > cursor_reference.value
             )
-            page_query = (
-                self._filter_order_by(
-                    page_query, [(cursor_reference.column, SortDirection.ASC)]
-                )
-                .limit(forward_limit)
-                .subquery("page")  # type: ignore
+            page_query = self._filter_order_by(
+                page_query, [(cursor_reference.column, SortDirection.ASC)]
             )
         else:
-            previous_query = stmt.where(
-                getattr(self._model, cursor_reference.column) >= cursor_reference.value
-            )
-            previous_query = (
-                self._filter_order_by(
-                    previous_query, [(cursor_reference.column, SortDirection.ASC)]
-                )
-                .limit(1)
-                .subquery("previous")  # type: ignore
-            )
-
             page_query = stmt.where(
                 getattr(self._model, cursor_reference.column) < cursor_reference.value
             )
-            page_query = (
-                self._filter_order_by(
-                    page_query, [(cursor_reference.column, SortDirection.DESC)]
-                )
-                .limit(forward_limit)
-                .subquery("page")  # type: ignore
+            page_query = self._filter_order_by(
+                page_query, [(cursor_reference.column, SortDirection.DESC)]
             )
+        return page_query.limit(limit)
 
-        query = select(
-            aliased(
-                self._model,
-                select(previous_query)
-                .union(select(page_query))
-                .order_by(cursor_reference.column)
-                .subquery(),  # type: ignore
+    def _cursor_pagination_previous_item_query(
+        self, stmt: Select, cursor_reference: CursorReference, is_before_cursor: bool
+    ) -> Select:
+        """Adds the clauses to retrieve a single model, after or before
+        the cursor value (including the cursor itself).
+
+        :param stmt: a Select statement
+        :type stmt: Select
+        :param cursor_reference: A cursor reference containing ordering column
+            and threshold value
+        :type cursor_reference: Union[CursorReference, None]
+        :param is_before_cursor: If True it will return items before the cursor,
+            otherwise items after
+        :type is_before_cursor: bool
+        :return: The filtered query
+        """
+        if not is_before_cursor:
+            previous_query = stmt.where(
+                getattr(self._model, cursor_reference.column) <= cursor_reference.value
+            )
+            previous_query = self._filter_order_by(
+                previous_query, [(cursor_reference.column, SortDirection.DESC)]
+            )
+        else:
+            previous_query = stmt.where(
+                getattr(self._model, cursor_reference.column) >= cursor_reference.value
+            )
+            previous_query = self._filter_order_by(
+                previous_query, [(cursor_reference.column, SortDirection.ASC)]
             )
-        )
 
-        return query
+        return previous_query.limit(1)
 
     def _sanitised_query_limit(self, limit):
         return max(min(limit, self._max_query_limit), 0)
 
     def _model_pk(self) -> str:
+        """
+        Retrieves the primary key name from the repository model class.
+
+        :return:
+        """
         primary_keys = inspect(self._model).primary_key  # type: ignore
         if len(primary_keys) > 1:
             raise NotImplementedError("Composite primary keys are not supported.")
 
         return primary_keys[0].name
```

### Comparing `sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/common.py` & `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from enum import Enum
+from functools import partial
 from typing import Generic, List, TypeVar, Union
 
 from pydantic import BaseModel, StrictInt, StrictStr
 from pydantic.generics import GenericModel
+from sqlalchemy import asc, desc
 
 MODEL = TypeVar("MODEL")
 PRIMARY_KEY = Union[str, int, tuple, dict]
 
 
 class PageInfo(BaseModel):
     page: int
@@ -34,7 +37,12 @@
     start_cursor: Union[CursorReference, None] = None
     end_cursor: Union[CursorReference, None] = None
 
 
 class CursorPaginatedResult(GenericModel, Generic[MODEL]):
     items: List[MODEL]
     page_info: CursorPageInfo
+
+
+class SortDirection(Enum):
+    ASC = partial(asc)
+    DESC = partial(desc)
```

### Comparing `sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/result_presenters.py` & `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/result_presenters.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/sync.py` & `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_repository/sync.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 from sqlalchemy.orm import Session
 
 from .._bind_manager import SQLAlchemyBind
 from .._transaction_handler import SessionHandler
 from ..exceptions import InvalidConfig, ModelNotFound
 from .base_repository import (
     BaseRepository,
-    SortDirection,
 )
 from .common import (
     MODEL,
     PRIMARY_KEY,
     CursorPaginatedResult,
     CursorReference,
     PaginatedResult,
+    SortDirection,
 )
 from .result_presenters import CursorPaginatedResultPresenter, PaginatedResultPresenter
 
 
 class SQLAlchemyRepository(Generic[MODEL], BaseRepository[MODEL], ABC):
     _session_handler: SessionHandler
     _external_session: Union[Session, None]
@@ -119,31 +119,14 @@
     def cursor_paginated_find(
         self,
         items_per_page: int,
         cursor_reference: Union[CursorReference, None] = None,
         is_before_cursor: bool = False,
         search_params: Union[None, Mapping[str, Any]] = None,
     ) -> CursorPaginatedResult[MODEL]:
-        """Find models using filters and cursor based pagination
-
-        E.g.
-        find(name="John") finds all models with name = John
-
-        :param items_per_page: Number of models to retrieve
-        :type items_per_page: int
-        :param order_by: Model property to use for ordering and before/after evaluation
-        :type order_by: str
-        :param before: Identifier of the last node to skip
-        :type before: Union[int, str]
-        :param after: Identifier of the last node to skip
-        :type after: Union[int, str]
-        :param search_params: A dictionary containing equality filters
-        :return: A collection of models
-        :rtype: List
-        """
         find_stmt = self._find_query(search_params)
 
         paginated_stmt = self._cursor_paginated_query(
             find_stmt,
             cursor_reference=cursor_reference,
             is_before_cursor=is_before_cursor,
             items_per_page=items_per_page,
```

### Comparing `sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_transaction_handler.py` & `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_transaction_handler.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_unit_of_work.py` & `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/_unit_of_work.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/protocols.py` & `sqlalchemy_bind_manager-0.3.1/sqlalchemy_bind_manager/protocols.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     Mapping,
     Protocol,
     Tuple,
     Union,
     runtime_checkable,
 )
 
+from sqlalchemy_bind_manager._repository import SortDirection
 from sqlalchemy_bind_manager._repository.common import (
     MODEL,
     PRIMARY_KEY,
 )
 from sqlalchemy_bind_manager.repository import (
     CursorPaginatedResult,
     CursorReference,
     PaginatedResult,
-    SortDirection,
 )
 
 
 @runtime_checkable
 class SQLAlchemyAsyncRepositoryInterface(Protocol[MODEL]):
     async def save(self, instance: MODEL) -> MODEL:
         """Persist a model.
```

### Comparing `sqlalchemy_bind_manager-0.3.0/PKG-INFO` & `sqlalchemy_bind_manager-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-bind-manager
-Version: 0.3.0
+Version: 0.3.1
 Summary: A manager to easily handle multiple SQLAlchemy configurations
-Home-page: https://github.com/febus982/sqlalchemy-bind-manager
+Home-page: https://febus982.github.io/sqlalchemy-bind-manager
 License: MIT
 Keywords: sqlalchemy,config,manager
 Author: Federico Busetti
 Author-email: 729029+febus982@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -47,15 +47,15 @@
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 This package provides an easy way to configure and use SQLAlchemy engines and sessions
 without depending on frameworks.
 
 It is composed by two main components:
 
-* A manager class for SQLAlchemy engine configuration
+* A manager class for SQLAlchemy engine and session configuration
 * A repository/unit-of-work pattern implementation for model retrieval and persistence
 
 ## Installation
 
 ```bash
 pip install sqlalchemy-bind-manager
 ```
@@ -81,26 +81,25 @@
 )
 
 sa_manager = SQLAlchemyBindManager(config)
 ```
 
 🚨 NOTE: Using global variables is not thread-safe, please read the [Threading](#threading) section if your application uses multi-threading.
 
-`engine_url` and `engine_options` dictionary accept the same parameters as SQLAlchemy [create_engine()](https://docs.sqlalchemy.org/en/14/core/engines.html#sqlalchemy.create_engine)
+The `engine_url` and `engine_options` dictionaries accept the same parameters as SQLAlchemy [create_engine()](https://docs.sqlalchemy.org/en/14/core/engines.html#sqlalchemy.create_engine)
 
-`session_options` dictionary accepts the same parameters as SQLALchemy [sessionmaker()](https://docs.sqlalchemy.org/en/14/orm/session_api.html#sqlalchemy.orm.sessionmaker)
+The `session_options` dictionary accepts the same parameters as SQLALchemy [sessionmaker()](https://docs.sqlalchemy.org/en/14/orm/session_api.html#sqlalchemy.orm.sessionmaker)
 
 Once the bind manager is initialised we can retrieve and use the SQLAlchemyBind using the method `get_bind()`
 
-The `SQLAlchemyBind` class has the following attributes:
+The `SQLAlchemyBind` and `SQLAlchemyAsyncBind` class has the following attributes:
 
-* `bind_async`: A boolean property, `True` when the bind uses an async dialect (Note: async is not yet fully supported, see the section about asynchronous binds)
 * `engine`: The initialised SQLALchemy `Engine`
 * `model_declarative_base`: A base class that can be used to create [declarative models](https://docs.sqlalchemy.org/en/14/orm/mapping_styles.html#declarative-mapping)
-* `registry_mapper`: The `registry` associated with the `engine`. It can be used with Alembic or to achieve [imperative mapping](https://docs.sqlalchemy.org/en/14/orm/mapping_styles.html#imperative-mapping)
+* `registry_mapper`: The `registry` associated with the `engine`. It can be used with Alembic or to setup [imperative mapping](https://docs.sqlalchemy.org/en/14/orm/mapping_styles.html#imperative-mapping)
 * `session_class`: The class built by [sessionmaker()](https://docs.sqlalchemy.org/en/14/orm/session_api.html#sqlalchemy.orm.sessionmaker), either `Session` or `AsyncSession`
 
 The `SQLAlchemyBindManager` provides some helper methods to quickly access some of the bind properties without using the `SQLAlchemyBind`:
 
 * `get_session`: returns a Session object
 * `get_mapper`: returns the mapper associated with the bind
 
@@ -170,24 +169,39 @@
 All the `SQLAlchemyBindManager` helper methods accept the `bind_name` optional parameter:
 
 * `get_session(bind_name="default")`: returns a `Session` or `AsyncSession` object
 * `get_mapper(bind_name="default")`: returns the mapper associated with the bind
 
 ### Threading
 
-Global variables in python are shared among threads. Neither `SQLAlchemyBindManager` class
-or the repositories implementation are thread safe on their own.
+Global variables are shared between different threads in python. If your application uses
+multiple threads, like spawning a thread per request, then you should not store an
+initialised session in a global variable, otherwise the state of your models will be shared
+among the threads and produce undesired changes in the database.
 
-If your application uses multi-threads, the same `SQLAlchemyBindManager` object will be
-shared between different threads, together with the internal `Session` object,
-and changes on models could propagate among them, causing undesired operations.
-
-Make sure you check Python [Threading](https://docs.python.org/3/library/threading.html)
-documentation, especially the [Thread-local Data](https://docs.python.org/3/library/threading.html#thread-local-data)
-chapter to avoid issues.
+This is not thread safe:
+
+```python
+session = sa_manager.get_session()
+session.add(model)
+session.commit()
+```
+
+If you truly need to have a long-lived session you'll need to use a scoped session,
+something like this:
+
+```python
+from sqlalchemy.orm import scoped_session
+
+session = scoped_session(sa_manager.get_bind().session_class())
+```
+
+Handling the life cycle of scoped sessions is not supported by this documentations.
+Please refer to [SQLAlchemy documentation](https://docs.sqlalchemy.org/en/20/orm/contextual.html)
+about this.
 
 ### Asynchronous database binds
 
 Is it possible to supply configurations for asyncio supported engines.
 
 ```python
 config = SQLAlchemyAsyncConfig(
@@ -204,29 +218,34 @@
 ```
 
 Note that async implementation has several differences from the sync one, make sure
 to check [SQLAlchemy asyncio documentation](https://docs.sqlalchemy.org/en/20/orm/extensions/asyncio.html)
 
 ## Repository / Unit of work
 
-The `SQLAlchemyRepository` and `SQLAlchemyAsyncRepository` class can be used simply by extending them.
+The `SQLAlchemyRepository` and `SQLAlchemyAsyncRepository` class can be used directly or by extending them.
 
 ```python
 from sqlalchemy_bind_manager.repository import SQLAlchemyRepository
 
 
 class MyModel(model_declarative_base):
     pass
 
+# Direct usage
+repo_instance = SQLAlchemyRepository(sqlalchemy_bind_manager.get_bind(), model_class=MyModel)
 
 class ModelRepository(SQLAlchemyRepository[MyModel]):
     _model = MyModel
+    
+    def _some_custom_method_implemented(self):
+        ...
 
-
-repo_instance = ModelRepository(sqlalchemy_bind_manager.get_bind())
+# Extended class usage
+extended_repo_instance = ModelRepository(sqlalchemy_bind_manager.get_bind())
 ```
 
 The classes provide some common use methods:
 
 * `get`: Retrieve a model by identifier
 * `save`: Persist a model
 * `save_many`: Persist multiple models in a single transaction
@@ -242,42 +261,40 @@
 database access is potentially anticipated.
 
 Doing this too soon might cause unexpected effects, like unexpected updates being committed,
 if the initialised session is shared among different repositories.
 
 A `Repository` represents a generic interface to persist data object to a storage, not necessarily
 using SQLAlchemy. It makes sense that the lifecycle of a `Session` follows the one of the Repository
-(If we create a Repository, we're going to do a DB operation, otherwise we don't need a `Session`)
+(The assumption is: if we create a Repository, we're going to do a DB operation,
+otherwise we wouldn't need one).
 
-This ensures the `Session` we use is isolated, and the same for all the operations we do with the
-same repository.
+Each Repository instance create an internal scoped session. The session gets
+automatically closed when the Repository instance is not referenced by any variable (and the
+garbage collector clean it up)
+
+In this way we ensure the `Session` we use is isolated, and the same for all the operations we do with the
+same Repository. 
+
+This approach has a consequence: We can't use SQLAlchemy lazy loading, so we'll need to make sure relationship are always loaded eagerly,
+using either approach:
+* Setup your model/table relationships to always use always eager loading
+* Implement ad-hoc methods to deal with relationships as necessary
 
-The session is automatically closed and reopen with each Repository operation, this make sure these
-operation are independent from each other.
-
-These choices cause some consequences:
-* The operations that modify the database will reload the models from the DB, causing an additional
-  SELECT query to be issued.
-* We can't use SQLAlchemy lazy loading, so we'll need to make sure relationship are always loaded eagerly,
-  using either:
-  * Setup your model/table relationships to always use always eager loading
-  * Implement ad-hoc methods to deal with relationships as necessary
-
-Also `AsyncSession` has [the same limitation on lazy loading](https://docs.sqlalchemy.org/en/20/orm/extensions/asyncio.html#asyncio-orm-avoid-lazyloads)
-so it makes sense that the two repository implementations behave consistently.
+Note that `AsyncSession` has [the same limitation on lazy loading](https://docs.sqlalchemy.org/en/20/orm/extensions/asyncio.html#asyncio-orm-avoid-lazyloads),
+even when keeping the session opened, so it makes sense that the two Repository implementations behave consistently.
 
 ### Use the Unit Of Work to share a session among multiple repositories
 
-It is possible we need to run several operations in a single database get_session. While a single
+It is possible we need to run several operations in a single database transaction. While a single
 repository provide by itself an isolated session for single operations, we have to use a different
 approach for multiple operations.
 
 We can use the `UnitOfWork` or the `AsyncUnitOfWork` class to provide a shared session to
 be used for repository operations, **assumed the same bind is used for all the repositories**.
-(Two phase transactions are not currently supported).
 
 ```python
 class MyRepo(SQLAlchemyRepository):
     _model = MyModel
 class MyOtherRepo(SQLAlchemyRepository):
     _model = MyOtherModel
 
@@ -290,11 +307,7 @@
 
 # Optionally disable the commit/rollback handling
 with uow.transaction(read_only=True):
     model1 = uow.MyRepo.get(1)
     model2 = uow.MyOtherRepo.get(2)
 ```
 
-Both the UnitOfWork classes create an internal `scoped_session` or `async_scoped_session`, behaving
-in the same way at the repositories do. This provides the freedom to tune the session lifecycle based
-on our application requirements (e.g. one unit of work per http request, per domain, etc.)
-
```

