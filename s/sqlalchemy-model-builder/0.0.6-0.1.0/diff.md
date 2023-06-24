# Comparing `tmp/sqlalchemy-model-builder-0.0.6.tar.gz` & `tmp/sqlalchemy_model_builder-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-model-builder-0.0.6.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `sqlalchemy-model-builder-0.0.6.tar` & `sqlalchemy_model_builder-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,16 @@
--rw-r--r--   0        0        0     1077 2021-08-05 05:34:55.349978 sqlalchemy-model-builder-0.0.6/LICENSE
--rw-r--r--   0        0        0     2851 2021-08-05 05:34:55.349978 sqlalchemy-model-builder-0.0.6/README.md
--rw-r--r--   0        0        0      815 2021-08-05 05:34:55.353978 sqlalchemy-model-builder-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      210 2021-08-05 05:34:55.353978 sqlalchemy-model-builder-0.0.6/sqlalchemy_model_builder/__init__.py
--rw-r--r--   0        0        0       49 2021-08-05 05:34:55.353978 sqlalchemy-model-builder-0.0.6/sqlalchemy_model_builder/exceptions.py
--rw-r--r--   0        0        0     5668 2021-08-05 05:34:55.353978 sqlalchemy-model-builder-0.0.6/sqlalchemy_model_builder/model_builder.py
--rw-r--r--   0        0        0      350 2021-08-05 05:34:55.353978 sqlalchemy-model-builder-0.0.6/sqlalchemy_model_builder/models.py
--rw-r--r--   0        0        0     2115 2021-08-05 05:34:55.353978 sqlalchemy-model-builder-0.0.6/sqlalchemy_model_builder/random_builder.py
--rw-r--r--   0        0        0     3661 1970-01-01 00:00:00.000000 sqlalchemy-model-builder-0.0.6/setup.py
--rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 sqlalchemy-model-builder-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/sqlalchemy_model_builder/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/sqlalchemy_model_builder/exceptions.py
+-rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/sqlalchemy_model_builder/model_builder.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/sqlalchemy_model_builder/models.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/sqlalchemy_model_builder/random_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/tests/test_model_builder_primitive_types.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/tests/test_model_builder_relationships.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/tests/test_random_builder.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/README.md
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/PKG-INFO
```

### Comparing `sqlalchemy-model-builder-0.0.6/LICENSE` & `sqlalchemy_model_builder-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-model-builder-0.0.6/README.md` & `sqlalchemy_model_builder-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 # SQLAlchemy Model Builder
 ![test](https://github.com/aminalaee/sqlalchemy-model-builder/actions/workflows/test.yml/badge.svg) ![publish](https://github.com/aminalaee/sqlalchemy-model-builder/actions/workflows/publish.yml/badge.svg) [![codecov](https://codecov.io/gh/aminalaee/sqlalchemy-model-builder/branch/main/graph/badge.svg?token=QOLK6R9M52)](https://codecov.io/gh/aminalaee/sqlalchemy-model-builder) 
 [![pypi](https://img.shields.io/pypi/v/sqlalchemy-model-builder?color=%2334D058&label=pypi)](https://pypi.org/project/sqlalchemy-model-builder/)
 
 ## Features
-- Build and Save SQLALchemy models with random data
+- Build SQLAlchemy model instance with random data
+- Save SQLAlchemy model instance with random data
 - Build relationships
-- Build minimal (with required) fields only
+- Build minimal (with required fields) only
 
-## How to use
-Build SQLAlchemy model:
+---
+
+## Installation
+
+```shell
+$ pip install sqladmin
 ```
+
+---
+
+## How to use
+Deinfe the SQLAlchemy models:
+
+```python
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.sql.sqltypes import Integer, String, Text
 
-from sqlalchemy_model_builder import ModelBuilder
-
 Base = declarative_base()
 
 
 class Address(Base):
     __tablename__ = "addresses"
 
     id = Column(Integer, primary_key=True)
@@ -30,63 +40,44 @@
     __tablename__ = "users"
 
     addresses = relationship("Address", back_populates="user")
     bio = Column(Text)
     id = Column(Integer, primary_key=True)
     name = Column(String, nullable=False)
 
-
-random_user = ModelBuilder(User).build()  # This will not insert the User
-
-minimal_random_user = ModelBuilder(User, minimal=True).build()  # Builds User with `id` and `name`
-
-random_address = ModelBuilder(Address).build(user_id=user.id)  # Build with `user_id`
 ```
 
-Save SQLAlchemy model:
-```
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.sql.sqltypes import Integer, String
+Save random model instance:
 
+```python
 from sqlalchemy_model_builder import ModelBuilder
 
-Base = declarative_base()
-
-engine = create_engine("sqlite://", echo=True)
-
-
-class Address(Base):
-    __tablename__ = "addresses"
-
-    id = Column(Integer, primary_key=True)
-    user_id = Column(Integer, ForeignKey("users.id"))
-    user = relationship("User", back_populates="addresses")
-
-
-class User(Base):
-    __tablename__ = "users"
-
-    addresses = relationship("Address", back_populates="user")
-    bio = Column(Text)
-    id = Column(Integer, primary_key=True)
-    name = Column(String, nullable=False)
-
+random_user = ModelBuilder(User).save(db)
+```
 
-Base.metadata.create_all(engine)
+Build random model without saving:
 
-LocalSession = sessionmaker(bind=engine)
+```python
+random_user = ModelBuilder(User).build()
+```
 
-db = LocalSession()
+Build minimal model instance:
 
+```python
+minimal_random_user = ModelBuilder(User, minimal=True).build()
+```
 
-random_user = ModelBuilder(User).save(db=db)  # Builds and Saves model using provided session
+Build or save with specific values:
 
-random_address = ModelBuilder(Address).save(db=db, user_id=user.id)  # Save with `user_id`
+```python
+random_address = ModelBuilder(Address).build(user_id=1)
 ```
 
+---
+
 ## Supported Data Types
 - BigInteger
 - Boolean
 - Date
 - DateTime
 - Enum
 - Float
```

### Comparing `sqlalchemy-model-builder-0.0.6/sqlalchemy_model_builder/model_builder.py` & `sqlalchemy_model_builder-0.1.0/sqlalchemy_model_builder/model_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,106 +1,113 @@
 from datetime import date, datetime, time, timedelta
 from typing import Any, Callable, Optional, Type
 
 from sqlalchemy import inspect
 from sqlalchemy.exc import NoInspectionAvailable
-from sqlalchemy.orm.session import Session
+from sqlalchemy.orm import Mapper, Session
 
 from sqlalchemy_model_builder.exceptions import ModelBuilderException
-from sqlalchemy_model_builder.models import (ColumnValuePair,
-                                             ColumnValuePairList)
+from sqlalchemy_model_builder.models import ColumnValuePair, ColumnValuePairList
 from sqlalchemy_model_builder.random_builder import RandomBuilder
 
 
 class ModelBuilder:
     def __init__(self, db_model: Type, minimal: bool = False):
         self.db: Optional[Session] = None
         self.db_model: Type = db_model
         self.minimal: bool = minimal
 
-    def build(self, **attrs) -> Any:
-        """Build SQLAlchemy model with random data and return it without persisting into database
+    def build(self, **attrs: Any) -> Any:
+        """Build SQLAlchemy model with random data and
+        return it without persisting into database.
 
         :returns: a SQLAlchemy database model with generated random data
         :rtype: Any
         """
         try:
             column_values = self.__get_model_fields(self.db_model)
         except NoInspectionAvailable as sqlalchemy_exception:
-            raise ModelBuilderException(f"Class {self.db_model} is not a SQLAlchemy model") from sqlalchemy_exception
+            raise ModelBuilderException(
+                f"Class {self.db_model} is not a SQLAlchemy model"
+            ) from sqlalchemy_exception
 
         column_values_with_attrs = dict(column_values.to_dict(), **attrs)
 
         try:
             instance = self.db_model(**column_values_with_attrs)
         except TypeError as sqlalchemy_exception:
-            raise ModelBuilderException(f"Invalid fields for model: {self.db_model}") from sqlalchemy_exception
+            raise ModelBuilderException(
+                f"Invalid fields for model: {self.db_model}"
+            ) from sqlalchemy_exception
 
         return instance
 
-    def save(self, db: Session, **attrs) -> Any:
-        """Build SQLAlchemy model with random data and persist it into database using provided db
+    def save(self, db: Session, **attrs: Any) -> Any:
+        """Build SQLAlchemy model with random data and
+        persist it into database using provided db.
 
         :param db: SQLAlchemy database session
         :type db: Session
         :returns: a SQLAlchemy database model with generated random data
         :rtype: Any
         """
         self.db = db
 
         instance = self.build(**attrs)
 
         self.__save(instance)
 
         return instance
 
-    def __build_model_relationships(self, mapper) -> ColumnValuePairList:
+    def __build_model_relationships(self, mapper: Mapper) -> ColumnValuePairList:
         """Build model relationships
 
         :param mapper: Mapper to load relationship from
         :type mapper: SQLAlchemy ORM Mapper
         :returns: a List of ColumnValuePair to map column with instance
         :rtype: ColumnValuePairList
         """
         related_models = []
 
         for relationship in mapper.relationships:
             foreign_keys = any(c.foreign_keys for c in relationship.local_columns)
             if not foreign_keys:
                 continue
 
-            values = self.__get_model_fields(relationship.mapper)
+            values = self.__get_model_fields(relationship.mapper.class_)
             instance = relationship.mapper.class_(**values.to_dict())
 
             if self.db:
                 self.__save(instance)
 
             foreign_key_column = next(iter(relationship.local_columns))
 
-            column_value = ColumnValuePair(foreign_key_column.key, instance)
+            column_value = ColumnValuePair(foreign_key_column.name, instance)
             related_models.append(column_value)
 
         return ColumnValuePairList(related_models)
 
     def __get_model_fields(self, db_model: Type) -> ColumnValuePairList:
         """Get model field and values from SQLAlchemy model
 
-        :returns: a dictionary of model field values; key is name of field and value is random value
+        :returns: a dictionary of model field attribute and values.
         :rtype: ColumnValuePairList
         """
         column_values = []
         mapper = inspect(db_model)
 
-        relationships = self.__build_model_relationships(mapper)
+        relationships = self.__build_model_relationships(mapper)  # type: ignore
         for relationship in relationships.pairs:
             primary_key = inspect(relationship.value).mapper.primary_key[0]
-            column_value = ColumnValuePair(relationship.column, getattr(relationship.value, primary_key.key))
+            column_value = ColumnValuePair(
+                relationship.column, getattr(relationship.value, primary_key.key)
+            )
             column_values.append(column_value)
 
-        for column in mapper.columns:
+        for column in mapper.columns:  # type: ignore
             python_type: Optional[type] = None
 
             if hasattr(column.type, "impl"):
                 if hasattr(column.type.impl, "python_type"):
                     python_type = column.type.python_type
             elif hasattr(column.type, "python_type"):
                 python_type = column.type.python_type
@@ -114,15 +121,17 @@
 
             random_value = self.__map_field_to_random_builder_method(python_type)()
             column_value = ColumnValuePair(column.key, random_value)
             column_values.append(column_value)
 
         return ColumnValuePairList(column_values)
 
-    def __map_field_to_random_builder_method(self, field_type: type) -> Callable[[], Any]:
+    def __map_field_to_random_builder_method(
+        self, field_type: type
+    ) -> Callable[[], Any]:
         """Mapping between field type and RandomBuilder methods
 
         :returns: a RandomBuilder method for the provided type
         :rtype: function
         """
         func: Callable[[], Any] = RandomBuilder.next_str
 
@@ -143,12 +152,12 @@
         elif field_type == time:
             func = RandomBuilder.next_time
         elif field_type == timedelta:
             func = RandomBuilder.next_timedelta
 
         return func
 
-    def __save(self, instance: Any):
+    def __save(self, instance: Any) -> None:
         assert self.db is not None
 
         self.db.add(instance)
         self.db.commit()
```

### Comparing `sqlalchemy-model-builder-0.0.6/sqlalchemy_model_builder/random_builder.py` & `sqlalchemy_model_builder-0.1.0/sqlalchemy_model_builder/random_builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,59 +8,74 @@
 
 class RandomBuilder:
     @classmethod
     def next_bool(cls) -> bool:
         return random.choice([True, False])
 
     @classmethod
-    def next_bytes(cls, length=8) -> bytes:
-        return random.getrandbits(length * 8).to_bytes(length, 'little')
+    def next_bytes(cls, length: int = 8) -> bytes:
+        return random.getrandbits(length * 8).to_bytes(length, "little")
 
     @classmethod
     def next_date(cls) -> date:
-        return date(year=random.randint(2000, 2050), month=random.randint(1, 12), day=random.randint(1, 28))
+        return date(
+            year=random.randint(2000, 2050),
+            month=random.randint(1, 12),
+            day=random.randint(1, 28),
+        )
 
     @classmethod
     def next_datetime(cls) -> datetime:
         return datetime(
             year=random.randint(2000, 2050),
             month=random.randint(1, 12),
             day=random.randint(1, 28),
             hour=random.randint(0, 23),
             minute=random.randint(0, 59),
-            second=random.randint(0, 59))
+            second=random.randint(0, 59),
+        )
 
     @classmethod
     def next_datetime_utc(cls) -> datetime:
         return cls.next_datetime().astimezone(timezone.utc)
 
     @classmethod
     def next_enum(cls, e: typing.Type[enum.Enum]) -> typing.Any:
         return random.choice([item.value for item in e])
 
     @classmethod
-    def next_float(cls, minimum=0, maximum=2147483647, precision=5) -> float:
+    def next_float(
+        cls, minimum: float = 0, maximum: float = 2147483647, precision: int = 5
+    ) -> float:
         return round(random.uniform(minimum, maximum), precision)
 
     @classmethod
-    def next_int(cls, minimum=0, maximum=2147483647) -> int:
+    def next_int(cls, minimum: int = 0, maximum: int = 2147483647) -> int:
         return random.randint(minimum, maximum)
 
     @classmethod
-    def next_int64(cls, minimum=0, maximum=9223372036854775807) -> int:
+    def next_int64(cls, minimum: int = 0, maximum: int = 9223372036854775807) -> int:
         return random.randint(minimum, maximum)
 
     @classmethod
-    def next_str(cls, length=16) -> str:
-        return ''.join(random.choice(string.ascii_letters) for _ in range(length))
+    def next_str(cls, length: int = 16) -> str:
+        return "".join(random.choice(string.ascii_letters) for _ in range(length))
 
     @classmethod
     def next_time(cls) -> time:
-        return time(hour=random.randint(0, 23), minute=random.randint(0, 59), second=random.randint(0, 59))
+        return time(
+            hour=random.randint(0, 23),
+            minute=random.randint(0, 59),
+            second=random.randint(0, 59),
+        )
 
     @classmethod
     def next_timedelta(cls) -> timedelta:
-        return timedelta(days=random.randint(1, 7), hours=random.randint(1, 23), minutes=random.randint(0, 59))
+        return timedelta(
+            days=random.randint(1, 7),
+            hours=random.randint(1, 23),
+            minutes=random.randint(0, 59),
+        )
 
     @classmethod
     def next_uuid(cls) -> uuid.UUID:
         return uuid.uuid4()
```

### Comparing `sqlalchemy-model-builder-0.0.6/PKG-INFO` & `sqlalchemy_model_builder-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,59 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-model-builder
-Version: 0.0.6
+Version: 0.1.0
 Summary: SQLAlchemy Model Builder
-Home-page: https://github.com/aminalaee/sqlalchemy-model-builder
-License: MIT
-Author: Amin Alaee
-Author-email: mohammadamin.alaee@gmail.com
-Requires-Python: >=3.7,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
+Project-URL: Documentation, https://github.com/aminalaee/sqlalchemy-model-builder
+Project-URL: Issues, https://github.com/aminalaee/sqlalchemy-model-builder/issues
+Project-URL: Source, https://github.com/aminalaee/sqlalchemy-model-builder
+Author-email: Amin Alaee <me@aminalaee.dev>
+License-Expression: MIT
+License-File: LICENSE
+Keywords: sqlalchemy,testing
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: SQLAlchemy (>=1.4.0,<2.0.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Requires-Dist: sqlalchemy>=1.4
 Description-Content-Type: text/markdown
 
 # SQLAlchemy Model Builder
 ![test](https://github.com/aminalaee/sqlalchemy-model-builder/actions/workflows/test.yml/badge.svg) ![publish](https://github.com/aminalaee/sqlalchemy-model-builder/actions/workflows/publish.yml/badge.svg) [![codecov](https://codecov.io/gh/aminalaee/sqlalchemy-model-builder/branch/main/graph/badge.svg?token=QOLK6R9M52)](https://codecov.io/gh/aminalaee/sqlalchemy-model-builder) 
 [![pypi](https://img.shields.io/pypi/v/sqlalchemy-model-builder?color=%2334D058&label=pypi)](https://pypi.org/project/sqlalchemy-model-builder/)
 
 ## Features
-- Build and Save SQLALchemy models with random data
+- Build SQLAlchemy model instance with random data
+- Save SQLAlchemy model instance with random data
 - Build relationships
-- Build minimal (with required) fields only
+- Build minimal (with required fields) only
 
-## How to use
-Build SQLAlchemy model:
+---
+
+## Installation
+
+```shell
+$ pip install sqladmin
 ```
+
+---
+
+## How to use
+Deinfe the SQLAlchemy models:
+
+```python
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.sql.sqltypes import Integer, String, Text
 
-from sqlalchemy_model_builder import ModelBuilder
-
 Base = declarative_base()
 
 
 class Address(Base):
     __tablename__ = "addresses"
 
     id = Column(Integer, primary_key=True)
@@ -48,63 +65,44 @@
     __tablename__ = "users"
 
     addresses = relationship("Address", back_populates="user")
     bio = Column(Text)
     id = Column(Integer, primary_key=True)
     name = Column(String, nullable=False)
 
-
-random_user = ModelBuilder(User).build()  # This will not insert the User
-
-minimal_random_user = ModelBuilder(User, minimal=True).build()  # Builds User with `id` and `name`
-
-random_address = ModelBuilder(Address).build(user_id=user.id)  # Build with `user_id`
 ```
 
-Save SQLAlchemy model:
-```
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.sql.sqltypes import Integer, String
+Save random model instance:
 
+```python
 from sqlalchemy_model_builder import ModelBuilder
 
-Base = declarative_base()
-
-engine = create_engine("sqlite://", echo=True)
-
-
-class Address(Base):
-    __tablename__ = "addresses"
-
-    id = Column(Integer, primary_key=True)
-    user_id = Column(Integer, ForeignKey("users.id"))
-    user = relationship("User", back_populates="addresses")
-
-
-class User(Base):
-    __tablename__ = "users"
-
-    addresses = relationship("Address", back_populates="user")
-    bio = Column(Text)
-    id = Column(Integer, primary_key=True)
-    name = Column(String, nullable=False)
-
+random_user = ModelBuilder(User).save(db)
+```
 
-Base.metadata.create_all(engine)
+Build random model without saving:
 
-LocalSession = sessionmaker(bind=engine)
+```python
+random_user = ModelBuilder(User).build()
+```
 
-db = LocalSession()
+Build minimal model instance:
 
+```python
+minimal_random_user = ModelBuilder(User, minimal=True).build()
+```
 
-random_user = ModelBuilder(User).save(db=db)  # Builds and Saves model using provided session
+Build or save with specific values:
 
-random_address = ModelBuilder(Address).save(db=db, user_id=user.id)  # Save with `user_id`
+```python
+random_address = ModelBuilder(Address).build(user_id=1)
 ```
 
+---
+
 ## Supported Data Types
 - BigInteger
 - Boolean
 - Date
 - DateTime
 - Enum
 - Float
@@ -117,8 +115,7 @@
 - SchemaType (Todo)
 - SmallInteger
 - String
 - Text
 - Time
 - Unicode
 - UnicodeText
-
```

