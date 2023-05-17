# Comparing `tmp/vecs-0.1.0.tar.gz` & `tmp/vecs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vecs-0.1.0.tar", last modified: Mon May 15 19:55:52 2023, max compression
+gzip compressed data, was "vecs-0.2.1.tar", last modified: Wed May 17 19:20:50 2023, max compression
```

## Comparing `vecs-0.1.0.tar` & `vecs-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-15 19:55:52.210850 vecs-0.1.0/
--rw-r--r--   0 oliverrice   (501) staff       (20)      742 2023-05-15 19:55:52.210642 vecs-0.1.0/PKG-INFO
--rw-r--r--   0 oliverrice   (501) staff       (20)     1522 2023-05-15 19:38:44.000000 vecs-0.1.0/README.md
--rw-r--r--   0 oliverrice   (501) staff       (20)      154 2023-05-12 13:47:40.000000 vecs-0.1.0/pyproject.toml
--rw-r--r--   0 oliverrice   (501) staff       (20)       38 2023-05-15 19:55:52.210931 vecs-0.1.0/setup.cfg
--rw-r--r--   0 oliverrice   (501) staff       (20)     2144 2023-05-15 19:35:05.000000 vecs-0.1.0/setup.py
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-15 19:55:52.206401 vecs-0.1.0/src/
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-15 19:55:52.208741 vecs-0.1.0/src/vecs/
--rw-r--r--   0 oliverrice   (501) staff       (20)      390 2023-05-15 19:28:30.000000 vecs-0.1.0/src/vecs/__init__.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     1697 2023-05-12 13:45:37.000000 vecs-0.1.0/src/vecs/client.py
--rw-r--r--   0 oliverrice   (501) staff       (20)    12341 2023-05-15 19:21:24.000000 vecs-0.1.0/src/vecs/collection.py
--rw-r--r--   0 oliverrice   (501) staff       (20)      490 2023-05-15 19:20:49.000000 vecs-0.1.0/src/vecs/exc.py
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-15 19:55:52.209596 vecs-0.1.0/src/vecs.egg-info/
--rw-r--r--   0 oliverrice   (501) staff       (20)      742 2023-05-15 19:55:52.000000 vecs-0.1.0/src/vecs.egg-info/PKG-INFO
--rw-r--r--   0 oliverrice   (501) staff       (20)      317 2023-05-15 19:55:52.000000 vecs-0.1.0/src/vecs.egg-info/SOURCES.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)        1 2023-05-15 19:55:52.000000 vecs-0.1.0/src/vecs.egg-info/dependency_links.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)      122 2023-05-15 19:55:52.000000 vecs-0.1.0/src/vecs.egg-info/requires.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)        5 2023-05-15 19:55:52.000000 vecs-0.1.0/src/vecs.egg-info/top_level.txt
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-15 19:55:52.210189 vecs-0.1.0/tests/
--rw-r--r--   0 oliverrice   (501) staff       (20)     1264 2023-05-12 14:02:11.000000 vecs-0.1.0/tests/test_client.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     9482 2023-05-15 19:19:33.000000 vecs-0.1.0/tests/test_collection.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 19:20:50.105667 vecs-0.2.1/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      742 2023-05-17 19:20:50.105527 vecs-0.2.1/PKG-INFO
+-rw-r--r--   0 oliverrice   (501) staff       (20)     6055 2023-05-17 18:27:20.000000 vecs-0.2.1/README.md
+-rw-r--r--   0 oliverrice   (501) staff       (20)      154 2023-05-12 13:47:40.000000 vecs-0.2.1/pyproject.toml
+-rw-r--r--   0 oliverrice   (501) staff       (20)       38 2023-05-17 19:20:50.105715 vecs-0.2.1/setup.cfg
+-rw-r--r--   0 oliverrice   (501) staff       (20)     2188 2023-05-17 19:19:05.000000 vecs-0.2.1/setup.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 19:20:50.103492 vecs-0.2.1/src/
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 19:20:50.104435 vecs-0.2.1/src/vecs/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      390 2023-05-17 19:10:32.000000 vecs-0.2.1/src/vecs/__init__.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     1686 2023-05-16 19:39:23.000000 vecs-0.2.1/src/vecs/client.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)    13522 2023-05-17 19:04:04.000000 vecs-0.2.1/src/vecs/collection.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)      491 2023-05-16 18:21:37.000000 vecs-0.2.1/src/vecs/exc.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-17 19:20:50.105341 vecs-0.2.1/src/vecs.egg-info/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      742 2023-05-17 19:20:50.000000 vecs-0.2.1/src/vecs.egg-info/PKG-INFO
+-rw-r--r--   0 oliverrice   (501) staff       (20)      271 2023-05-17 19:20:50.000000 vecs-0.2.1/src/vecs.egg-info/SOURCES.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)        1 2023-05-17 19:20:50.000000 vecs-0.2.1/src/vecs.egg-info/dependency_links.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)      146 2023-05-17 19:20:50.000000 vecs-0.2.1/src/vecs.egg-info/requires.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)        5 2023-05-17 19:20:50.000000 vecs-0.2.1/src/vecs.egg-info/top_level.txt
```

### Comparing `vecs-0.1.0/PKG-INFO` & `vecs-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vecs
-Version: 0.1.0
+Version: 0.2.1
 Summary: pgvector client
 Home-page: https://github.com/olirice/vecs
 Author: Oliver Rice
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `vecs-0.1.0/setup.py` & `vecs-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,24 +33,24 @@
     logging.warning("'%s' not found in '%s'", key, module_path)
     raise KeyError(key)
 
 
 check_python_version()
 
 
-REQUIRES = ["pgvector==0.1.*", "sqlalchemy==2.*"]
+REQUIRES = ["pgvector==0.1.*", "sqlalchemy==2.*", "psycopg2-binary==2.9.*"]
 
 
 setuptools.setup(
     name=read_package_variable("__project__"),
     version=read_package_variable("__version__"),
     description="pgvector client",
     url="https://github.com/olirice/vecs",
     author="Oliver Rice",
-    packages=setuptools.find_packages("src"),
+    packages=setuptools.find_packages("src", exclude="tests"),
     package_dir={"": "src"},
     package_data={"": ["py.typed"]},
     tests_require=["pytest"],
     license="MIT",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Natural Language :: English",
@@ -63,10 +63,10 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     install_requires=REQUIRES,
     extras_require={
         "dev": ["pytest", "parse", "numpy", "pytest-cov"],
-        "docs": ["mkdocs", "pygments", "pymdown-extensions", "mkautodoc"],
+        "docs": ["mkdocs", "pygments", "pymdown-extensions", "pymarkdown"],
     },
 )
```

### Comparing `vecs-0.1.0/src/vecs/client.py` & `vecs-0.2.1/src/vecs/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from __future__ import annotations
 
-from typing import Any, List, TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 
-from sqlalchemy import (
-    MetaData,
-    create_engine,
-    text,
-)
+from sqlalchemy import MetaData, create_engine, text
 from sqlalchemy.orm import sessionmaker
 
 from vecs.exc import CollectionNotFound
 
 if TYPE_CHECKING:
     from vecs.collection import Collection
 
@@ -25,14 +21,15 @@
             with sess.begin():
                 sess.execute(text("create schema if not exists vecs;"))
                 sess.execute(text("create extension if not exists vector;"))
 
     def create_collection(self, name: str, dimension: int) -> Collection:
         """Create a collection"""
         from vecs.collection import Collection
+
         return Collection(name, dimension, self)._create()
 
     def get_collection(self, name: str) -> Collection:
         """Get an existing collection"""
         from vecs.collection import Collection
 
         collections = Collection._list_collections(self)
@@ -40,13 +37,16 @@
             if collection.name == name:
                 return collection
         raise CollectionNotFound("No collection found with requested name")
 
     def list_collections(self) -> List["Collection"]:
         """List all collections"""
         from vecs.collection import Collection
+
         return Collection._list_collections(self)
 
     def delete_collection(self, name: str) -> None:
         """List all collections"""
         from vecs.collection import Collection
-        return Collection(name, -1, self)._drop()
+
+        Collection(name, -1, self)._drop()
+        return
```

### Comparing `vecs-0.1.0/src/vecs/collection.py` & `vecs-0.2.1/src/vecs/collection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 import math
+import uuid
+import warnings
 from enum import Enum
-from typing import Dict, Iterable, List, Optional, Tuple, Union, TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict, Iterable, List, Optional, Tuple, Union
 
 from flupy import flu
 from pgvector.sqlalchemy import Vector
 from sqlalchemy import (
     Column,
     MetaData,
     String,
@@ -17,18 +19,22 @@
     func,
     or_,
     select,
     text,
 )
 from sqlalchemy.dialects import postgresql
 
-from vecs.exc import CollectionAlreadyExists, CollectionNotFound, ArgError, FilterError, ArgError, Unreachable
-
+from vecs.exc import (
+    ArgError,
+    CollectionAlreadyExists,
+    CollectionNotFound,
+    FilterError,
+    Unreachable,
+)
 
-       
 if TYPE_CHECKING:
     from vecs.client import Client
 
 
 MetadataValues = Union[str, int, float, bool, List[str]]
 Metadata = Dict[str, MetadataValues]
 Numeric = Union[int, float, complex]
@@ -41,14 +47,27 @@
 
 class IndexMeasure(str, Enum):
     cosine_distance = "cosine_distance"
     l2_distance = "l2_distance"
     max_inner_product = "max_inner_product"
 
 
+INDEX_MEASURE_TO_OPS = {
+    IndexMeasure.cosine_distance: "vector_cosine_ops",
+    IndexMeasure.l2_distance: "vector_l2_ops",
+    IndexMeasure.max_inner_product: "vector_ip_ops",
+}
+
+INDEX_MEASURE_TO_SQLA_ACC = {
+    IndexMeasure.cosine_distance: lambda x: x.cosine_distance,
+    IndexMeasure.l2_distance: lambda x: x.l2_distance,
+    IndexMeasure.max_inner_product: lambda x: x.max_inner_product,
+}
+
+
 class Collection:
     def __init__(self, name: str, dimension: int, client: Client):
         self.client = client
         self.name = name
         self.dimension = dimension
         self.table = build_table(name, client.meta, dimension)
         self._index: Optional[str] = None
@@ -72,17 +91,15 @@
         self.table.create(self.client.engine)
         return self
 
     def _drop(self):
         existing_collections = self.__class__._list_collections(self.client)
         existing_collection_names = [x.name for x in existing_collections]
         if self.name not in existing_collection_names:
-            raise CollectionNotFound(
-                "Collection with requested name not found"
-            )
+            raise CollectionNotFound("Collection with requested name not found")
         self.table.drop(self.client.engine)
         return self
 
     def upsert(self, vectors: Iterable[Tuple[str, Iterable[Numeric], Metadata]]):
         stmt = postgresql.insert(self.table).values(vectors)
         stmt = stmt.on_conflict_do_update(
             index_elements=[self.table.c.id],
@@ -90,30 +107,28 @@
         )
         with self.client.Session() as sess:
             with sess.begin():
                 sess.execute(stmt)
         return
 
     def fetch(self, ids: Iterable[str]) -> List[Record]:
-
         if isinstance(ids, str):
             raise ArgError("ids must be a list of strings")
 
         chunk_size = 12
         records = []
         with self.client.Session() as sess:
             with sess.begin():
                 for id_chunk in flu(ids).chunk(chunk_size):
                     stmt = select(self.table).where(self.table.c.id.in_(id_chunk))
                     chunk_records = sess.execute(stmt)
                     records.extend(chunk_records)
         return records
 
     def delete(self, ids: Iterable[str]) -> List[str]:
-
         if isinstance(ids, str):
             raise ArgError("ids must be a list of strings")
 
         chunk_size = 12
 
         del_ids = list(ids)
         ids = []
@@ -137,51 +152,64 @@
         if row == []:
             raise KeyError("no item found with requested id")
         return row[0]
 
     def query(
         self,
         query_vector: Iterable[Numeric],
-        top_k: int,
+        limit: int = 10,
         filters: Optional[Dict] = None,
-        measure: IndexMeasure = IndexMeasure.cosine_distance,
+        measure: Union[IndexMeasure, str] = IndexMeasure.cosine_distance,
         include_value: bool = False,
         include_metadata: bool = False,
     ) -> Union[List[Record], List[str]]:
-        if top_k > 100:
-            raise ArgError("top_k must be <= 100")
 
-        distance_lambda = None
-        if measure == IndexMeasure.cosine_distance:
-            distance_lambda = self.table.c.vec.cosine_distance
+        if limit > 1000:
+            raise ArgError("limit must be <= 1000")
+
+        # ValueError on bad input
+        try:
+            imeasure = IndexMeasure(measure)
+        except ValueError:
+            raise ArgError("Invalid index measure")
+
+        if not self.is_indexed_for_measure(imeasure):
+            warnings.warn(
+                f"Query does not have a covering index for {imeasure}. See Collection.create_index"
+            )
 
+        distance_lambda = INDEX_MEASURE_TO_SQLA_ACC.get(imeasure)
         if distance_lambda is None:
-            raise ArgError("invalid distance_measure")
+            # unreachable
+            raise ArgError("invalid distance_measure")  # pragma: no cover
 
-        distance_clause = distance_lambda(query_vector)
+        distance_clause = distance_lambda(self.table.c.vec)(query_vector)
 
         cols = [self.table.c.id]
 
         if include_value:
             cols.append(distance_clause)
 
         if include_metadata:
             cols.append(self.table.c.metadata)
 
         stmt = select(*cols)
         if filters:
-            stmt = stmt.filter(build_filters(self.table.c.metadata, ["genre"], filters)) # type: ignore
+            stmt = stmt.filter(build_filters(self.table.c.metadata, filters))  # type: ignore
 
         stmt = stmt.order_by(distance_clause)
-        stmt = stmt.limit(top_k)
+        stmt = stmt.limit(limit)
 
         with self.client.Session() as sess:
-            if len(cols) == 1:
-                return [str(x) for x in sess.scalars(stmt).fetchall()]
-            return sess.execute(stmt).fetchall() or []
+            with sess.begin():
+                # index ignored if greater than n_lists
+                sess.execute(text("set local ivfflat.probes = 10"))
+                if len(cols) == 1:
+                    return [str(x) for x in sess.scalars(stmt).fetchall()]
+                return sess.execute(stmt).fetchall() or []
 
     @classmethod
     def _list_collections(cls, client: "Client") -> List["Collection"]:
         query = text(
             """
         select
             relname as table_name,
@@ -209,94 +237,108 @@
         if self._index is None:
             query = text(
                 """
             select
                 relname as table_name
             from
                 pg_class pc
-
             where
                 pc.relnamespace = 'vecs'::regnamespace
-                and relname ilike 'ix_vec%'
+                and relname ilike 'ix_vector%'
                 and pc.relkind = 'i'
             """
             )
             with self.client.Session() as sess:
                 ix_name = sess.execute(query).scalar()
             self._index = ix_name
         return self._index
 
-    def _supports_cosine_search(self):
-        if self.index is None:
+    def is_indexed_for_measure(self, measure: IndexMeasure):
+        index_name = self.index
+        if index_name is None:
             return False
-        if self.index.startswith("ix_vec_cosine"):
+
+        ops = INDEX_MEASURE_TO_OPS.get(measure)
+        if ops is None:
+            return False
+
+        if ops in index_name:
             return True
+
         return False
 
     def create_index(
         self,
-        method: IndexMethod = IndexMethod.ivfflat,
         measure: IndexMeasure = IndexMeasure.cosine_distance,
-        metadata_config: Dict = {},
+        method: IndexMethod = IndexMethod.ivfflat,
         replace=True,
     ):
         if not method == IndexMethod.ivfflat:
+            # at time of writing, no other methods are supported by pgvector
             raise ArgError("invalid index method")
 
-        if replace == False:
+        if replace:
+            self._index = None
+        else:
             if self.index is not None:
                 raise ArgError("replace is set to False but an index exists")
 
-        if not measure == IndexMeasure.cosine_distance:
-            raise NotImplementedError("only cosine distance is currently supported")
-
-        indexed = metadata_config.get("indexed") or []
-        if not isinstance(indexed, list):
-            raise ArgError("indexed must be a list of strings")
-        for field in indexed:
-            if not isinstance(field, str):
-                raise ArgError("indexed must be a list of strings")
+        ops = INDEX_MEASURE_TO_OPS.get(measure)
+        if ops is None:
+            raise ArgError("Unknown index measure")
 
         # Clone the table
-        # clone_meta = MetaData(schema='vecs')
         clone_table = build_table(f"_{self.name}", self.client.meta, self.dimension)
 
         # hacky
         try:
             clone_table.drop(self.client.engine)
         except Exception:
             pass
 
         with self.client.Session() as sess:
             n_records: int = sess.execute(func.count(self.table.c.id)).scalar()  # type: ignore
 
         with self.client.Session() as sess:
             with sess.begin():
+                n_index_seed = min(1500, n_records)
                 clone_table.create(sess.connection())
                 stmt_seed_table = clone_table.insert().from_select(
-                    self.table.c, select(self.table).order_by(func.random()).limit(1500)
+                    self.table.c,
+                    select(self.table).order_by(func.random()).limit(n_index_seed),
                 )
                 sess.execute(stmt_seed_table)
 
-                if measure == IndexMeasure.cosine_distance:
-                    n_lists = (
-                        max(n_records / 1000, 30)
-                        if n_records < 1_000_000
-                        else math.sqrt(n_records)
-                    )
+                n_lists = (
+                    max(n_records / 1000, 30)
+                    if n_records < 1_000_000
+                    else math.sqrt(n_records)
+                )
+
+                unique_string = str(uuid.uuid4()).replace("-", "_")[0:7]
 
-                    sess.execute(
-                        text(
-                            f"create index ix_vec_cosine_{n_lists} on vecs.{clone_table.name} using ivfflat (vec vector_cosine_ops) with (lists={n_lists})"
-                        )
+                sess.execute(
+                    text(
+                        f"""
+                        create index ix_{ops}_{n_lists}_{unique_string}
+                          on vecs."{clone_table.name}"
+                          using ivfflat (vec {ops}) with (lists={n_lists})
+                        """
                     )
+                )
 
-                else:
-                    raise NotImplemented("only cosine distance is currently supported")
-                # Create the vector index
+                sess.execute(
+                    text(
+                        f"""
+                        create index ix_meta_{unique_string}
+                          on vecs."{clone_table.name}"
+                          using gin ( metadata )
+                        """
+                    )
+                )
 
                 # Fully populate the table
                 stmt = postgresql.insert(clone_table).from_select(
                     self.table.c, select(self.table)
                 )
                 stmt = stmt.on_conflict_do_nothing()
                 sess.execute(stmt)
@@ -306,15 +348,15 @@
                 sess.execute(
                     text(
                         f"alter table vecs._{self.table.name} rename to {self.table.name};"
                     )
                 )
 
 
-def build_filters(json_col: Column, indexed_fields, filters: Dict):
+def build_filters(json_col: Column, filters: Dict):
     if not isinstance(filters, dict):
         raise FilterError("filters must be a dict")
 
     if len(filters) > 1:
         raise FilterError("max 1 entry per filter")
 
     for key, value in filters.items():
@@ -324,49 +366,48 @@
         if key in ("$and", "$or"):
             if not isinstance(value, list):
                 raise FilterError(
                     "$and/$or filters must have associated list of conditions"
                 )
 
             if key == "$and":
-                return and_(
-                    *[
-                        build_filters(json_col, indexed_fields, subcond)
-                        for subcond in value
-                    ]
-                )
+                return and_(*[build_filters(json_col, subcond) for subcond in value])
 
             if key == "$or":
-                return or_(
-                    *[
-                        build_filters(json_col, indexed_fields, subcond)
-                        for subcond in value
-                    ]
-                )
+                return or_(*[build_filters(json_col, subcond) for subcond in value])
 
             raise Unreachable()
 
         if isinstance(value, dict):
             if len(value) > 1:
                 raise FilterError("only operator permitted")
             for operator, clause in value.items():
-                if operator not in ("$eq", "$neq", "$lt"):
+                if operator not in ("$eq", "$ne", "$lt", "$lte", "$gt", "$gte"):
                     raise FilterError("unknown operator")
 
                 matches_value = cast(clause, postgresql.JSONB)
 
                 if operator == "$eq":
                     return json_col.op("->")(key) == matches_value
 
-                if operator == "$neq":
+                if operator == "$ne":
                     return json_col.op("->")(key) != matches_value
 
                 if operator == "$lt":
                     return json_col.op("->")(key) < matches_value
 
+                if operator == "$lte":
+                    return json_col.op("->")(key) <= matches_value
+
+                if operator == "$gt":
+                    return json_col.op("->")(key) > matches_value
+
+                if operator == "$gte":
+                    return json_col.op("->")(key) >= matches_value
+
                 else:
                     raise Unreachable()
 
 
 def build_table(name: str, meta: MetaData, dimension) -> Table:
     return Table(
         name,
```

### Comparing `vecs-0.1.0/src/vecs.egg-info/PKG-INFO` & `vecs-0.2.1/src/vecs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vecs
-Version: 0.1.0
+Version: 0.2.1
 Summary: pgvector client
 Home-page: https://github.com/olirice/vecs
 Author: Oliver Rice
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

