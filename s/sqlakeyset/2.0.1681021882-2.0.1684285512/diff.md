# Comparing `tmp/sqlakeyset-2.0.1681021882.tar.gz` & `tmp/sqlakeyset-2.0.1684285512.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlakeyset-2.0.1681021882.tar", max compression
+gzip compressed data, was "sqlakeyset-2.0.1684285512.tar", max compression
```

## Comparing `sqlakeyset-2.0.1681021882.tar` & `sqlakeyset-2.0.1684285512.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1210 2023-04-09 06:31:17.610311 sqlakeyset-2.0.1681021882/LICENSE
--rw-r--r--   0        0        0     8265 2023-04-09 06:31:17.610311 sqlakeyset-2.0.1681021882/README.rst
--rw-r--r--   0        0        0     1295 2023-04-09 06:31:22.826264 sqlakeyset-2.0.1681021882/pyproject.toml
--rw-r--r--   0        0        0      631 2023-04-09 06:31:17.610311 sqlakeyset-2.0.1681021882/sqlakeyset/__init__.py
--rw-r--r--   0        0        0     2717 2023-04-09 06:31:17.610311 sqlakeyset-2.0.1681021882/sqlakeyset/asyncio.py
--rw-r--r--   0        0        0    14716 2023-04-09 06:31:17.610311 sqlakeyset-2.0.1681021882/sqlakeyset/columns.py
--rw-r--r--   0        0        0       37 2023-04-09 06:31:17.610311 sqlakeyset-2.0.1681021882/sqlakeyset/constants.py
--rw-r--r--   0        0        0    14213 2023-04-09 06:31:17.610311 sqlakeyset-2.0.1681021882/sqlakeyset/paging.py
--rw-r--r--   0        0        0    10324 2023-04-09 06:31:17.610311 sqlakeyset-2.0.1681021882/sqlakeyset/results.py
--rw-r--r--   0        0        0      347 2023-04-09 06:31:17.610311 sqlakeyset-2.0.1681021882/sqlakeyset/serial/__init__.py
--rw-r--r--   0        0        0     5546 2023-04-09 06:31:17.610311 sqlakeyset-2.0.1681021882/sqlakeyset/serial/serial.py
--rw-r--r--   0        0        0     2097 2023-04-09 06:31:17.610311 sqlakeyset-2.0.1681021882/sqlakeyset/sqla.py
--rw-r--r--   0        0        0     2613 2023-04-09 06:31:17.610311 sqlakeyset-2.0.1681021882/sqlakeyset/sqla13.py
--rw-r--r--   0        0        0     1571 2023-04-09 06:31:17.610311 sqlakeyset-2.0.1681021882/sqlakeyset/sqla14.py
--rw-r--r--   0        0        0     3712 2023-04-09 06:31:17.610311 sqlakeyset-2.0.1681021882/sqlakeyset/sqla20.py
--rw-r--r--   0        0        0      768 2023-04-09 06:31:17.610311 sqlakeyset-2.0.1681021882/sqlakeyset/types.py
--rw-r--r--   0        0        0     9215 1970-01-01 00:00:00.000000 sqlakeyset-2.0.1681021882/setup.py
--rw-r--r--   0        0        0     9125 1970-01-01 00:00:00.000000 sqlakeyset-2.0.1681021882/PKG-INFO
+-rw-r--r--   0        0        0     1210 2023-05-17 01:05:06.803672 sqlakeyset-2.0.1684285512/LICENSE
+-rw-r--r--   0        0        0     8265 2023-05-17 01:05:06.803672 sqlakeyset-2.0.1684285512/README.rst
+-rw-r--r--   0        0        0     1295 2023-05-17 01:05:12.051476 sqlakeyset-2.0.1684285512/pyproject.toml
+-rw-r--r--   0        0        0      631 2023-05-17 01:05:06.803672 sqlakeyset-2.0.1684285512/sqlakeyset/__init__.py
+-rw-r--r--   0        0        0     2717 2023-05-17 01:05:06.803672 sqlakeyset-2.0.1684285512/sqlakeyset/asyncio.py
+-rw-r--r--   0        0        0    14716 2023-05-17 01:05:06.803672 sqlakeyset-2.0.1684285512/sqlakeyset/columns.py
+-rw-r--r--   0        0        0       37 2023-05-17 01:05:06.803672 sqlakeyset-2.0.1684285512/sqlakeyset/constants.py
+-rw-r--r--   0        0        0    14213 2023-05-17 01:05:06.803672 sqlakeyset-2.0.1684285512/sqlakeyset/paging.py
+-rw-r--r--   0        0        0    10324 2023-05-17 01:05:06.803672 sqlakeyset-2.0.1684285512/sqlakeyset/results.py
+-rw-r--r--   0        0        0      347 2023-05-17 01:05:06.803672 sqlakeyset-2.0.1684285512/sqlakeyset/serial/__init__.py
+-rw-r--r--   0        0        0     5546 2023-05-17 01:05:06.803672 sqlakeyset-2.0.1684285512/sqlakeyset/serial/serial.py
+-rw-r--r--   0        0        0     2097 2023-05-17 01:05:06.803672 sqlakeyset-2.0.1684285512/sqlakeyset/sqla.py
+-rw-r--r--   0        0        0     2613 2023-05-17 01:05:06.803672 sqlakeyset-2.0.1684285512/sqlakeyset/sqla13.py
+-rw-r--r--   0        0        0     1571 2023-05-17 01:05:06.803672 sqlakeyset-2.0.1684285512/sqlakeyset/sqla14.py
+-rw-r--r--   0        0        0     4199 2023-05-17 01:05:06.803672 sqlakeyset-2.0.1684285512/sqlakeyset/sqla20.py
+-rw-r--r--   0        0        0      768 2023-05-17 01:05:06.803672 sqlakeyset-2.0.1684285512/sqlakeyset/types.py
+-rw-r--r--   0        0        0     9215 1970-01-01 00:00:00.000000 sqlakeyset-2.0.1684285512/setup.py
+-rw-r--r--   0        0        0     9125 1970-01-01 00:00:00.000000 sqlakeyset-2.0.1684285512/PKG-INFO
```

### Comparing `sqlakeyset-2.0.1681021882/LICENSE` & `sqlakeyset-2.0.1684285512/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1681021882/README.rst` & `sqlakeyset-2.0.1684285512/README.rst`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1681021882/pyproject.toml` & `sqlakeyset-2.0.1684285512/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sqlakeyset"
-version = "2.0.1681021882"
+version = "2.0.1684285512"
 authors = [ "Robert Lechte <robertlechte@gmail.com>", "Anthony Carapetis <anthony.carapetis@gmail.com>",]
 license = "Unlicense"
 readme = "README.rst"
 description = "offset-free paging for sqlalchemy"
 repository = "https://github.com/djrobstep/sqlakeyset"
 homepage = "https://github.com/djrobstep/sqlakeyset"
```

### Comparing `sqlakeyset-2.0.1681021882/sqlakeyset/__init__.py` & `sqlakeyset-2.0.1684285512/sqlakeyset/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1681021882/sqlakeyset/asyncio.py` & `sqlakeyset-2.0.1684285512/sqlakeyset/asyncio.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1681021882/sqlakeyset/columns.py` & `sqlakeyset-2.0.1684285512/sqlakeyset/columns.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1681021882/sqlakeyset/paging.py` & `sqlakeyset-2.0.1684285512/sqlakeyset/paging.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1681021882/sqlakeyset/results.py` & `sqlakeyset-2.0.1684285512/sqlakeyset/results.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1681021882/sqlakeyset/serial/serial.py` & `sqlakeyset-2.0.1684285512/sqlakeyset/serial/serial.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1681021882/sqlakeyset/sqla.py` & `sqlakeyset-2.0.1684285512/sqlakeyset/sqla.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1681021882/sqlakeyset/sqla13.py` & `sqlakeyset-2.0.1684285512/sqlakeyset/sqla13.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1681021882/sqlakeyset/sqla14.py` & `sqlakeyset-2.0.1684285512/sqlakeyset/sqla14.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1681021882/sqlakeyset/sqla20.py` & `sqlakeyset-2.0.1684285512/sqlakeyset/sqla20.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Methods for messing with the internals of SQLAlchemy 1.4/2.0 results."""
 from __future__ import annotations
+
 from sqlalchemy.engine.result import result_tuple
 from sqlalchemy.engine.row import Row
 
 from .constants import ORDER_COL_PREFIX
 
 
 def orm_query_keys(query):
@@ -92,24 +93,43 @@
 def core_coerce_row(row: Row, extra_columns, result_type) -> Row:
     """Trim off the extra columns and return as a correct-as-possible
     sqlalchemy Row."""
     if not extra_columns:
         return row
     N = len(row) - len(extra_columns)
 
+    parent = row._parent
+    processors = None  # Processors are applied immediately in sqla1.4+
+    data = row._data[:N]
+
+    if hasattr(row, "_key_to_index"):
+        # 2.0.11+
+        structure = (
+            {  # Strip out added OCs from the keymap:
+                k: row[v]
+                for k, v in row._key_to_index.items()
+                if not (isinstance(k, str) and k.startswith(ORDER_COL_PREFIX))
+            },
+        )
+    else:
+        # <2.0.11
+        structure = (
+            {  # Strip out added OCs from the keymap:
+                k: v
+                for k, v in row._keymap.items()
+                if not (isinstance(v[1], str) and v[1].startswith(ORDER_COL_PREFIX))
+            },
+            row._key_style,
+        )
+
     return TruncatedRow(
-        row._parent,
-        None,  # Processors are applied immediately in sqla1.4+
-        {  # Strip out added OCs from the keymap:
-            k: v
-            for k, v in row._keymap.items()
-            if not (isinstance(v[1], str) and v[1].startswith(ORDER_COL_PREFIX))
-        },
-        row._key_style,
-        row._data[:N],
+        parent,
+        processors,
+        *structure,
+        data,
     )
 
 
 __all__ = [
     "Row",
     "TruncatedRow",
     "core_coerce_row",
```

### Comparing `sqlakeyset-2.0.1681021882/sqlakeyset/types.py` & `sqlakeyset-2.0.1684285512/sqlakeyset/types.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1681021882/setup.py` & `sqlakeyset-2.0.1684285512/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['packaging>=20.0',
  'python-dateutil',
  'sqlalchemy>=1.3.11',
  'typing_extensions>=4,<5']
 
 setup_kwargs = {
     'name': 'sqlakeyset',
-    'version': '2.0.1681021882',
+    'version': '2.0.1684285512',
     'description': 'offset-free paging for sqlalchemy',
     'long_description': "sqlakeyset: offset-free paging for sqlalchemy\n=============================================\n\n.. image:: https://img.shields.io/circleci/build/gh/djrobstep/sqlakeyset?label=tests\n    :alt: Tests\n    :target: https://circleci.com/gh/djrobstep/sqlakeyset\n    \n.. image:: https://img.shields.io/pypi/v/sqlakeyset\n    :alt: PyPI\n    :target: https://pypi.org/project/sqlakeyset/\n    \n.. image:: https://img.shields.io/conda/vn/conda-forge/sqlakeyset.svg\n    :alt: conda-forge\n    :target: https://anaconda.org/conda-forge/sqlakeyset\n\nsqlakeyset implements keyset-based paging for SQLAlchemy (both ORM and core). **Now with full SQLAlchemy 2 support and type hints!**\n\nThis library is tested with PostgreSQL, MariaDB/MySQL and SQLite. It should work with many other SQLAlchemy-supported databases, too; but caveat emptor - you should verify the results are correct.\n\n**Notice:** In accordance with Python end-of-life dates, we've stopped supporting Python versions earlier than 3.7. If you really need it, the latest version to support Python 2 is 0.1.1559103842 and Python 3.4 is 1.0.1679209451, but you'll miss out on all the latest features and bugfixes from the latest version. You should be upgrading anyway!\n\nBackground\n----------\n\nA lot of people use SQL's ``OFFSET`` syntax to implement paging of query results. The trouble with that is, the more pages you get through, the slower your query gets. Also, if the results you're paging through change frequently, it's possible to skip over or repeat results between pages. Keyset paging avoids these problems: Selecting even the millionth page is as fast as selecting the first.\n\n\nGetting Started\n---------------\n\nHere's how it works with a typical SQLAlchemy 2.0-style query (or SQLAlchemy 1.3 Core):\n\n.. code-block:: python\n\n    from sqlalchemy import create_engine, select\n    from sqlalchemy.orm import Session\n    from sqlakeyset import select_page\n\n    from models import Book\n\n    engine = create_engine('postgresql:///books')\n    with Session(engine) as s:\n        q = select(Book).order_by(Book.author, Book.title, Book.id)\n\n        # gets the first page\n        page1 = select_page(s, q, per_page=20)\n\n        # gets the key for the next page\n        next_page = page1.paging.next\n\n        # gets the second page\n        page2 = select_page(s, q, per_page=20, page=next_page)\n\n        # returning to the first page, getting the key\n        previous_page = page2.paging.previous\n\n        # the first page again, backwards from the previous page\n        page1 = select_page(s, q, per_page=20, page=previous_page)\n\n        # what if new items were added at the start?\n        if page1.paging.has_previous:\n\n            # go back even further\n            previous_page = page1.paging.previous\n            page1 = select_page(s, q, per_page=20, page=previous_page)\n\n\nIf you're still using legacy (i.e. SQLAlchemy 1.3-style) ORM queries, you can\nuse ``get_page`` instead, which has an identical API other than the omission of\nthe session/connection argument:\n\n.. code-block:: python\n\n    from sqlakeyset import get_page\n    with Session(engine) as s:\n        q = s.query(Book).order_by(Book.author, Book.title, Book.id)\n        page1 = get_page(q, per_page=20)\n        # ...\n\nWe also support asyncio, and the API is near-identical - just import from\n``sqlakeyset.asyncio`` and pass an ``AsyncSession``:\n\n.. code-block:: python\n\n    from sqlalchemy import select\n    from sqlalchemy.ext.asyncio import AsyncSession, create_async_engine\n    from sqlakeyset.asyncio import select_page\n    engine = create_async_engine('postgresql:///books')\n    async with AsyncSession(engine) as s:\n        q = select(Book).order_by(Book.author, Book.title, Book.id)\n        page1 = await select_page(s, q, per_page=20)\n        # ...\n\n\nUnder the Hood\n--------------\n\nsqlakeyset does the following to your query in order to get the paged contents:\n\n- adds a where clause, to get only rows after the specified row key.\n- if getting the previous page, reverses the ``order by`` direction in order the get the rows *before* the specified bookmark.\n- adds a limit clause, to fetch only enough items to fill the page, plus one additional (this additional row is used only to test for the existence of further pages after the current one, and is discarded from the results).\n- returns the page contents as an ordinary list that has an attached ``.paging`` attribute with the paging information for this and related pages.\n\n\nPage objects\n------------\n\nPaged items/rows are returned in a ``Page`` object, which is a vanilla python list extended by an attached ``Paging`` object containing paging information.\n\nProperties such as `next` and `previous` return a pair containing the ordering key for the row, and a boolean to specify if the direction is forwards or backwards. We refer to such a pair ``(keyset, backwards)`` as a *marker*.\n\nIn our above example, the marker specifying the second page might look like:\n\n.. code-block:: python\n\n    ('Joseph Heller', 'Catch 22', 123), False\n\nThe `False` means the query will fetch the page *after* the row containing Catch 22. This tuple contains two elements, title and id, to match the order by clause of the query.\n\nThe page before this row would be specified as:\n\n.. code-block:: python\n\n    ('Joseph Heller', 'Catch 22', 123), True\n\nThe first and last pages are fetched with `None` instead of a tuple, so for the first page (this is also the default if the page parameter is not specified):\n\n.. code-block:: python\n\n    None, False\n\nAnd the last page:\n\n.. code-block:: python\n\n    None, True\n\nKeyset Serialization\n--------------------\n\nYou will probably want to turn these markers into strings for passing around. ``sqlakeyset`` includes code to do this, and calls the resulting strings *bookmarks*. To get a serialized bookmark, just add ``bookmark_`` to the name of the property that holds the keyset you want.\n\nMost commonly you'll want ``next`` and ``previous``, so:\n\n.. code-block:: python\n\n    >>> page.paging.bookmark_previous\n    <i:1~i:2015~s:Bad Blood~i:34\n    >>> page.paging.bookmark_next\n    >i:1~i:2014~s:Shake It Off~i:31\n\n``sqlakeyset`` uses the python csv row serializer to serialize the bookmark values (using ``~`` instead of a ``,`` as the separator). Direction is indicated by ``>`` (forwards/next), or ``<`` (backwards/previous) at the start of the string.\n\nLimitations\n-----------\n\n- **Golden Rule:** Always ensure your keysets are unique per row. If you violate this condition you risk skipped rows and other nasty problems. The simplest way to do this is to always include your primary key column(s) at the end of your ordering columns.\n\n- Any rows containing null values in their keysets **will be omitted from the results**, so your ordering columns should be ``NOT NULL``. (This is a consequence of the fact that comparisons against ``NULL`` are always false in SQL.) This may change in the future if we work out an alternative implementation; but for now we recommend using ``coalesce`` as a workaround if you need to sort by nullable columns:\n\n.. code-block:: python\n\n    from sqlalchemy import func\n    with Session(engine) as s:\n        # If Book.cost can be NULL:\n        q = select(Book).order_by(func.coalesce(Book.cost, 0), Book.id)\n        # Assuming cost is non-negative, page1 will start with books where cost is null:\n        page1 = select_page(s, q, per_page=20)\n\n- If you're using the in-built keyset serialization, this only handles basic data/column types so far (strings, ints, floats, datetimes, dates, booleans, and a few others). The serialization can be extended to serialize more advanced types as necessary (documentation on this is forthcoming).\n\n\nDocumentation\n-------------\n\nOther than this README, there is some basic sphinx documentation, which you can build yourself with e.g. ``make -C doc html``. Hopefully this will be available more conveniently soon - watch this space.\n\n\nInstallation\n------------\n\nAssuming you have `pip <https://pip.pypa.io>`_ installed, all you need to do is install as follows:\n\n.. code-block:: shell\n\n    $ pip install sqlakeyset\n\nThis will install sqlakeyset and also sqlalchemy if not already installed. Obviously you'll need the necessary database driver for your chosen database to be installed also.\n",
     'author': 'Robert Lechte',
     'author_email': 'robertlechte@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/djrobstep/sqlakeyset',
```

### Comparing `sqlakeyset-2.0.1681021882/PKG-INFO` & `sqlakeyset-2.0.1684285512/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlakeyset
-Version: 2.0.1681021882
+Version: 2.0.1684285512
 Summary: offset-free paging for sqlalchemy
 Home-page: https://github.com/djrobstep/sqlakeyset
 License: Unlicense
 Author: Robert Lechte
 Author-email: robertlechte@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

