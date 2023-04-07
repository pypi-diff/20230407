# Comparing `tmp/sqlalchemy-redshift-0.8.8.tar.gz` & `tmp/sqlalchemy-redshift-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-redshift-0.8.8.tar", last modified: Wed Nov  3 19:44:19 2021, max compression
+gzip compressed data, was "dist/sqlalchemy-redshift-0.8.9.tar", last modified: Wed Dec 15 17:50:42 2021, max compression
```

## Comparing `sqlalchemy-redshift-0.8.8.tar` & `sqlalchemy-redshift-0.8.9.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 jeffklukas   (501) staff       (20)        0 2021-11-03 19:44:19.868556 sqlalchemy-redshift-0.8.8/
--rw-r--r--   0 jeffklukas   (501) staff       (20)    13063 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/CHANGES.rst
--rw-r--r--   0 jeffklukas   (501) staff       (20)     1055 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/LICENSE
--rw-r--r--   0 jeffklukas   (501) staff       (20)      153 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/MANIFEST.in
--rw-r--r--   0 jeffklukas   (501) staff       (20)    16239 2021-11-03 19:44:19.868750 sqlalchemy-redshift-0.8.8/PKG-INFO
--rw-r--r--   0 jeffklukas   (501) staff       (20)     2132 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/README.rst
-drwxr-xr-x   0 jeffklukas   (501) staff       (20)        0 2021-11-03 19:44:19.865010 sqlalchemy-redshift-0.8.8/redshift_sqlalchemy/
--rw-r--r--   0 jeffklukas   (501) staff       (20)      595 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/redshift_sqlalchemy/__init__.py
--rw-r--r--   0 jeffklukas   (501) staff       (20)       67 2021-11-03 19:44:19.869466 sqlalchemy-redshift-0.8.8/setup.cfg
--rw-r--r--   0 jeffklukas   (501) staff       (20)     2007 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/setup.py
-drwxr-xr-x   0 jeffklukas   (501) staff       (20)        0 2021-11-03 19:44:19.866532 sqlalchemy-redshift-0.8.8/sqlalchemy_redshift/
--rw-r--r--   0 jeffklukas   (501) staff       (20)      927 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/sqlalchemy_redshift/__init__.py
--rw-r--r--   0 jeffklukas   (501) staff       (20)    39685 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/sqlalchemy_redshift/commands.py
--rw-r--r--   0 jeffklukas   (501) staff       (20)     9972 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/sqlalchemy_redshift/ddl.py
--rw-r--r--   0 jeffklukas   (501) staff       (20)    44014 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/sqlalchemy_redshift/dialect.py
--rw-r--r--   0 jeffklukas   (501) staff       (20)     8621 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/sqlalchemy_redshift/redshift-ca-bundle.crt
-drwxr-xr-x   0 jeffklukas   (501) staff       (20)        0 2021-11-03 19:44:19.868341 sqlalchemy-redshift-0.8.8/sqlalchemy_redshift.egg-info/
--rw-r--r--   0 jeffklukas   (501) staff       (20)    16239 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/sqlalchemy_redshift.egg-info/PKG-INFO
--rw-r--r--   0 jeffklukas   (501) staff       (20)      518 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/sqlalchemy_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 jeffklukas   (501) staff       (20)        1 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/sqlalchemy_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 jeffklukas   (501) staff       (20)      334 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/sqlalchemy_redshift.egg-info/entry_points.txt
--rw-r--r--   0 jeffklukas   (501) staff       (20)       35 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/sqlalchemy_redshift.egg-info/requires.txt
--rw-r--r--   0 jeffklukas   (501) staff       (20)       40 2021-11-03 19:44:19.000000 sqlalchemy-redshift-0.8.8/sqlalchemy_redshift.egg-info/top_level.txt
+drwxr-xr-x   0 whbrook  (405448585) ANT\Domain Users (1896053708)        0 2021-12-15 17:50:42.000000 sqlalchemy-redshift-0.8.9/
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)    19407 2021-12-15 17:50:42.000000 sqlalchemy-redshift-0.8.9/PKG-INFO
+drwxr-xr-x   0 whbrook  (405448585) ANT\Domain Users (1896053708)        0 2021-12-15 17:50:42.000000 sqlalchemy-redshift-0.8.9/sqlalchemy_redshift/
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)     9972 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/sqlalchemy_redshift/ddl.py
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)     8621 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/sqlalchemy_redshift/redshift-ca-bundle.crt
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)    45602 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/sqlalchemy_redshift/dialect.py
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)      927 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/sqlalchemy_redshift/__init__.py
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)    39685 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/sqlalchemy_redshift/commands.py
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)      153 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/MANIFEST.in
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)     2007 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/setup.py
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)       67 2021-12-15 17:50:42.000000 sqlalchemy-redshift-0.8.9/setup.cfg
+drwxr-xr-x   0 whbrook  (405448585) ANT\Domain Users (1896053708)        0 2021-12-15 17:50:42.000000 sqlalchemy-redshift-0.8.9/sqlalchemy_redshift.egg-info/
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)    19407 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/sqlalchemy_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)      510 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/sqlalchemy_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)      334 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/sqlalchemy_redshift.egg-info/entry_points.txt
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)       35 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/sqlalchemy_redshift.egg-info/requires.txt
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)       40 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/sqlalchemy_redshift.egg-info/top_level.txt
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)        1 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/sqlalchemy_redshift.egg-info/dependency_links.txt
+drwxr-xr-x   0 whbrook  (405448585) ANT\Domain Users (1896053708)        0 2021-12-15 17:50:42.000000 sqlalchemy-redshift-0.8.9/redshift_sqlalchemy/
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)      595 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/redshift_sqlalchemy/__init__.py
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)     2132 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/README.rst
+-rw-r--r--   0 whbrook  (405448585) ANT\Domain Users (1896053708)    13234 2021-12-15 17:50:41.000000 sqlalchemy-redshift-0.8.9/CHANGES.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `sqlalchemy-redshift-0.8.8/CHANGES.rst` & `sqlalchemy-redshift-0.8.9/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+0.8.9 (2021-12-15)
+------------------
+
+- Support inspection of Redshift datatypes
+  (`Pull #242 <https://github.com/sqlalchemy-redshift/sqlalchemy-redshift/pull/242>`_)
+
+
 0.8.8 (2021-11-03)
 ------------------
 
 - Remove support for Python 2.7; now requires python ``>=3.4``
   (`Pull #234 <https://github.com/sqlalchemy-redshift/sqlalchemy-redshift/pull/234>`_)
 - Support GEOMETRY, SUPER Redshift datatypes
   (`Pull #235 <https://github.com/sqlalchemy-redshift/sqlalchemy-redshift/pull/235>`_)
```

### Comparing `sqlalchemy-redshift-0.8.8/README.rst` & `sqlalchemy-redshift-0.8.9/README.rst`

 * *Files identical despite different names*

### Comparing `sqlalchemy-redshift-0.8.8/redshift_sqlalchemy/__init__.py` & `sqlalchemy-redshift-0.8.9/redshift_sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-redshift-0.8.8/setup.py` & `sqlalchemy-redshift-0.8.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 readme = open('README.rst').read()
 history = open('CHANGES.rst').read().replace('.. :changelog:', '')
 
 setup(
     name='sqlalchemy-redshift',
-    version='0.8.8',
+    version='0.8.9',
     description='Amazon Redshift Dialect for sqlalchemy',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/x-rst',
     author='Matt George',
     author_email='mgeorge@gmail.com',
     maintainer='Thomas Grainger',
     maintainer_email='sqlalchemy-redshift@graingert.co.uk',
```

### Comparing `sqlalchemy-redshift-0.8.8/sqlalchemy_redshift/__init__.py` & `sqlalchemy-redshift-0.8.9/sqlalchemy_redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-redshift-0.8.8/sqlalchemy_redshift/commands.py` & `sqlalchemy-redshift-0.8.9/sqlalchemy_redshift/commands.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-redshift-0.8.8/sqlalchemy_redshift/ddl.py` & `sqlalchemy-redshift-0.8.9/sqlalchemy_redshift/ddl.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-redshift-0.8.8/sqlalchemy_redshift/dialect.py` & `sqlalchemy-redshift-0.8.9/sqlalchemy_redshift/dialect.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from sqlalchemy import inspect
 from sqlalchemy.dialects.postgresql.base import (
     PGCompiler, PGDDLCompiler, PGIdentifierPreparer, PGTypeCompiler,
     PGExecutionContext, PGDialect
 )
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.dialects.postgresql.psycopg2cffi import PGDialect_psycopg2cffi
+from sqlalchemy.engine.default import DefaultDialect
+from sqlalchemy.sql.type_api import TypeEngine
 from sqlalchemy.engine import reflection
 from sqlalchemy.ext.compiler import compiles
 from sqlalchemy.sql.expression import (
     BinaryExpression, BooleanClauseList, Delete
 )
 from sqlalchemy.types import (
     VARCHAR, NullType, SMALLINT, INTEGER, BIGINT,
@@ -174,51 +176,68 @@
     "snapshot", "some", "sysdate", "system", "table", "tag", "tdes",
     "text255", "text32k", "then", "timestamp", "to", "top", "trailing",
     "true", "truncatecolumns", "union", "unique", "user", "using",
     "verbose", "wallet", "when", "where", "with", "without",
 ])
 
 
-class TIMESTAMPTZ(sa.dialects.postgresql.TIMESTAMP):
+class RedshiftTypeEngine(TypeEngine):
+
+    def _default_dialect(self, default=None):
+        """
+        Returns the default dialect used for TypeEngine compilation yielding String result.
+
+        :meth:`~sqlalchemy.sql.type_api.TypeEngine.compile`
+        """
+        return RedshiftDialectMixin()
+
+
+class TIMESTAMPTZ(RedshiftTypeEngine, sa.dialects.postgresql.TIMESTAMP):
     """
     Redshift defines a TIMTESTAMPTZ column type as an alias
     of TIMESTAMP WITH TIME ZONE.
     https://docs.aws.amazon.com/redshift/latest/dg/c_Supported_data_types.html
 
     Adding an explicit type to the RedshiftDialect allows us follow the
     SqlAlchemy conventions for "vendor-specific types."
 
     https://docs.sqlalchemy.org/en/13/core/type_basics.html#vendor-specific-types
     """
 
     __visit_name__ = 'TIMESTAMPTZ'
 
-    def __init__(self):
-        super(TIMESTAMPTZ, self).__init__(timezone=True)
+    def __init__(self, timezone=True, precision=None):
+        # timezone param must be present as it's provided in base class so the object
+        # can be instantiated with kwargs
+        # see :meth:`~sqlalchemy.dialects.postgresql.base.PGDialect._get_column_info`
+        super(TIMESTAMPTZ, self).__init__(timezone=True, precision=precision)
 
 
-class TIMETZ(sa.dialects.postgresql.TIME):
+class TIMETZ(RedshiftTypeEngine, sa.dialects.postgresql.TIME):
     """
     Redshift defines a TIMTETZ column type as an alias
     of TIME WITH TIME ZONE.
     https://docs.aws.amazon.com/redshift/latest/dg/c_Supported_data_types.html
 
     Adding an explicit type to the RedshiftDialect allows us follow the
     SqlAlchemy conventions for "vendor-specific types."
 
     https://docs.sqlalchemy.org/en/13/core/type_basics.html#vendor-specific-types
     """
 
     __visit_name__ = 'TIMETZ'
 
-    def __init__(self):
-        super(TIMETZ, self).__init__(timezone=True)
+    def __init__(self, timezone=True, precision=None):
+        # timezone param must be present as it's provided in base class so the object
+        # can be instantiated with kwargs
+        # see :meth:`~sqlalchemy.dialects.postgresql.base.PGDialect._get_column_info`
+        super(TIMETZ, self).__init__(timezone=True, precision=precision)
 
 
-class GEOMETRY(sa.dialects.postgresql.TEXT):
+class GEOMETRY(RedshiftTypeEngine, sa.dialects.postgresql.TEXT):
     """
     Redshift defines a GEOMETRY column type
     https://docs.aws.amazon.com/redshift/latest/dg/c_Supported_data_types.html
 
     Adding an explicit type to the RedshiftDialect allows us follow the
     SqlAlchemy conventions for "vendor-specific types."
 
@@ -229,15 +248,15 @@
     def __init__(self):
         super(GEOMETRY, self).__init__()
 
     def get_dbapi_type(self, dbapi):
         return dbapi.GEOMETRY
 
 
-class SUPER(sa.dialects.postgresql.TEXT):
+class SUPER(RedshiftTypeEngine, sa.dialects.postgresql.TEXT):
     """
     Redshift defines a SUPER column type
     https://docs.aws.amazon.com/redshift/latest/dg/c_Supported_data_types.html
 
     Adding an explicit type to the RedshiftDialect allows us follow the
     SqlAlchemy conventions for "vendor-specific types."
 
@@ -256,14 +275,22 @@
         return sa.func.json_parse(bindvalue)
 
     def process_bind_param(self, value, dialect):
         if not isinstance(value, str):
             return json.dumps(value)
         return value
 
+# Mapping for database schema inspection of Amazon Redshift datatypes
+REDSHIFT_ISCHEMA_NAMES = {
+    "geometry": GEOMETRY,
+    "super": SUPER,
+    "time with time zone": TIMETZ,
+    "timestamp with time zone": TIMESTAMPTZ,
+}
+
 
 class RelationKey(namedtuple('RelationKey', ('name', 'schema'))):
     """
     Structured tuple of table/view name and schema name.
     """
     __slots__ = ()
 
@@ -489,15 +516,15 @@
         return "TIMETZ"
 
 
 class RedshiftIdentifierPreparer(PGIdentifierPreparer):
     reserved_words = RESERVED_WORDS
 
 
-class RedshiftDialectMixin(object):
+class RedshiftDialectMixin(DefaultDialect):
     """
     Define Redshift-specific behavior.
 
     Most public methods are overrides of the underlying interfaces defined in
     :class:`~sqlalchemy.engine.interfaces.Dialect` and
     :class:`~sqlalchemy.engine.Inspector`.
     """
@@ -532,14 +559,24 @@
 
     def __init__(self, *args, **kw):
         super(RedshiftDialectMixin, self).__init__(*args, **kw)
         # Cache domains, as these will be static;
         # Redshift does not support user-created domains.
         self._domains = None
 
+    @property
+    def ischema_names(self):
+        """
+        Returns information about datatypes supported by Amazon Redshift.
+
+        Used in
+        :meth:`~sqlalchemy.engine.dialects.postgresql.base.PGDialect._get_column_info`.
+        """
+        return {**super(RedshiftDialectMixin, self).ischema_names, **REDSHIFT_ISCHEMA_NAMES}
+
     @reflection.cache
     def get_columns(self, connection, table_name, schema=None, **kw):
         """
         Return information about columns in `table_name`.
 
         Overrides interface
         :meth:`~sqlalchemy.engine.interfaces.Dialect.get_columns`.
```

### Comparing `sqlalchemy-redshift-0.8.8/sqlalchemy_redshift/redshift-ca-bundle.crt` & `sqlalchemy-redshift-0.8.9/sqlalchemy_redshift/redshift-ca-bundle.crt`

 * *Files identical despite different names*

