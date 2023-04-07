# Comparing `tmp/sa_repository-0.5.1.tar.gz` & `tmp/sa_repository-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sa_repository-0.5.1.tar", max compression
+gzip compressed data, was "sa_repository-1.0.0.tar", max compression
```

## Comparing `sa_repository-0.5.1.tar` & `sa_repository-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-02-13 22:38:44.227169 sa_repository-0.5.1/LICENSE
--rw-r--r--   0        0        0      869 2023-03-02 22:12:13.947089 sa_repository-0.5.1/README.md
--rw-r--r--   0        0        0      848 2023-03-23 22:23:18.630940 sa_repository-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       57 2023-03-23 22:23:58.067726 sa_repository-0.5.1/sa_repository/__init__.py
--rw-r--r--   0        0        0     4072 2023-03-23 22:28:55.557347 sa_repository-0.5.1/sa_repository/base.py
--rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 sa_repository-0.5.1/setup.py
--rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 sa_repository-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-13 22:38:44.227169 sa_repository-1.0.0/LICENSE
+-rw-r--r--   0        0        0      869 2023-03-02 22:12:13.947089 sa_repository-1.0.0/README.md
+-rw-r--r--   0        0        0      848 2023-04-07 20:22:41.527326 sa_repository-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-04-07 20:22:59.470188 sa_repository-1.0.0/sa_repository/__init__.py
+-rw-r--r--   0        0        0     4269 2023-04-03 21:36:31.615729 sa_repository-1.0.0/sa_repository/base.py
+-rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 sa_repository-1.0.0/setup.py
+-rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 sa_repository-1.0.0/PKG-INFO
```

### Comparing `sa_repository-0.5.1/LICENSE` & `sa_repository-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sa_repository-0.5.1/README.md` & `sa_repository-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sa_repository-0.5.1/pyproject.toml` & `sa_repository-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sa-repository"
-version = "0.5.1"
+version = "1.0.0"
 description = "Repository pattern for SQLAlchemy models"
 readme = "README.md"
 authors = ["Gasper3 <trzecik65@gmail.com>"]
 homepage = "https://github.com/Gasper3/sa-repository"
 repository = "https://github.com/Gasper3/sa-repository"
 
 [tool.poetry.dependencies]
```

### Comparing `sa_repository-0.5.1/sa_repository/base.py` & `sa_repository-1.0.0/sa_repository/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,14 +84,18 @@
         :returns: one
         :raises NoResultFound: if nothing was found
         :raises MultipleResultsFound: if found more than one record
         """
         stmt = self.get_query(*where, joins=joins)
         return self.session.scalars(stmt).one()
 
+    def get_or_none(self, *where: ColumnElement, joins: list | None = None) -> T | None:
+        stmt = self.get_query(*where, joins=joins)
+        return self.session.scalars(stmt).one_or_none()
+
     def find(self, *where, joins: list | None = None, order_by=None) -> t.Sequence[T]:
         stmt = self.get_query(*where, joins=joins, order_by=order_by)
         return self.session.scalars(stmt).all()
 
     # write methods
     def create(self, **params) -> T:
         obj = self.MODEL_CLASS(**params)
```

### Comparing `sa_repository-0.5.1/setup.py` & `sa_repository-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['more-itertools>=9.1.0,<10.0.0', 'sqlalchemy>=2.0.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'sa-repository',
-    'version': '0.5.1',
+    'version': '1.0.0',
     'description': 'Repository pattern for SQLAlchemy models',
     'long_description': "# SQLAlchemy Repository for models\n![tests workflow](https://github.com/Gasper3/sa-repository/actions/workflows/actions.yml/badge.svg)\n\nThis project contains simple Repository pattern for SQLAlchemy models.  \nAll you need to do is:\n1. Install this package `python -m pip install sa-repository`\n2. Use it in your project\n    ```python\n    from sa_repository import BaseRepository\n    from models import YourSAModel\n    \n    class SomeModelRepository(BaseRepository[YourSAModel]):\n        pass\n    ```\n\nBase class contains some general methods to simplify your work with sqlalchemy models e.x\n```python\nvar = SomeModelRepository(session).get(YourSAModel.attr == 'some_value')\n```\n\nIf you don't want to create new repository classes, you can use `get_repository_from_model` method\n```python\nrepository = BaseRepository.get_repository_from_model(db_session, SomeModel)\n```\n",
     'author': 'Gasper3',
     'author_email': 'trzecik65@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Gasper3/sa-repository',
```

### Comparing `sa_repository-0.5.1/PKG-INFO` & `sa_repository-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sa-repository
-Version: 0.5.1
+Version: 1.0.0
 Summary: Repository pattern for SQLAlchemy models
 Home-page: https://github.com/Gasper3/sa-repository
 Author: Gasper3
 Author-email: trzecik65@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

