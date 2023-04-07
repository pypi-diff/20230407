# Comparing `tmp/async_extensions-1.2.1.tar.gz` & `tmp/async_extensions-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_extensions-1.2.1.tar", max compression
+gzip compressed data, was "async_extensions-1.2.2.tar", max compression
```

## Comparing `async_extensions-1.2.1.tar` & `async_extensions-1.2.2.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1092 2023-02-07 15:29:55.852725 async_extensions-1.2.1/LICENSE
--rw-r--r--   0        0        0     2578 2023-02-07 15:29:55.852725 async_extensions-1.2.1/README.md
--rw-r--r--   0        0        0     2888 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/__init__.py
--rw-r--r--   0        0        0      732 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/blocking.py
--rw-r--r--   0        0        0      431 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/cancel.py
--rw-r--r--   0        0        0     1174 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/channel.py
--rw-r--r--   0        0        0     1781 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/close.py
--rw-r--r--   0        0        0     7840 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/collect.py
--rw-r--r--   0        0        0      118 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/constants.py
--rw-r--r--   0        0        0       80 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/current.py
--rw-r--r--   0        0        0       88 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/errors.py
--rw-r--r--   0        0        0      101 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/file.py
--rw-r--r--   0        0        0      174 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/low_level.py
--rw-r--r--   0        0        0       44 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/path.py
--rw-r--r--   0        0        0       87 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/process.py
--rw-r--r--   0        0        0        0 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/py.typed
--rw-r--r--   0        0        0      385 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/run.py
--rw-r--r--   0        0        0       76 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/signal.py
--rw-r--r--   0        0        0       77 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/sleep.py
--rw-r--r--   0        0        0     1334 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/standard.py
--rw-r--r--   0        0        0      143 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/synchronization.py
--rw-r--r--   0        0        0       70 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/task_group.py
--rw-r--r--   0        0        0      176 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/types.py
--rw-r--r--   0        0        0      859 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/typing.py
--rw-r--r--   0        0        0      732 2023-02-07 15:29:55.852725 async_extensions-1.2.1/async_extensions/wait.py
--rw-r--r--   0        0        0     2231 2023-02-07 15:29:55.852725 async_extensions-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 async_extensions-1.2.1/setup.py
--rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 async_extensions-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-07 19:07:21.256431 async_extensions-1.2.2/LICENSE
+-rw-r--r--   0        0        0     2578 2023-04-07 19:07:21.256431 async_extensions-1.2.2/README.md
+-rw-r--r--   0        0        0     2888 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/__init__.py
+-rw-r--r--   0        0        0      732 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/blocking.py
+-rw-r--r--   0        0        0      431 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/cancel.py
+-rw-r--r--   0        0        0     1174 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/channel.py
+-rw-r--r--   0        0        0     1781 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/close.py
+-rw-r--r--   0        0        0     7840 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/collect.py
+-rw-r--r--   0        0        0      118 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/constants.py
+-rw-r--r--   0        0        0       80 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/current.py
+-rw-r--r--   0        0        0       88 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/errors.py
+-rw-r--r--   0        0        0      101 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/file.py
+-rw-r--r--   0        0        0      174 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/low_level.py
+-rw-r--r--   0        0        0       44 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/path.py
+-rw-r--r--   0        0        0       87 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/process.py
+-rw-r--r--   0        0        0        0 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/py.typed
+-rw-r--r--   0        0        0      385 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/run.py
+-rw-r--r--   0        0        0       76 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/signal.py
+-rw-r--r--   0        0        0       77 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/sleep.py
+-rw-r--r--   0        0        0     1328 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/standard.py
+-rw-r--r--   0        0        0      143 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/synchronization.py
+-rw-r--r--   0        0        0       70 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/task_group.py
+-rw-r--r--   0        0        0      176 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/types.py
+-rw-r--r--   0        0        0      859 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/typing.py
+-rw-r--r--   0        0        0      732 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/wait.py
+-rw-r--r--   0        0        0     2230 2023-04-07 19:07:21.256431 async_extensions-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 async_extensions-1.2.2/PKG-INFO
```

### Comparing `async_extensions-1.2.1/LICENSE` & `async_extensions-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.1/README.md` & `async_extensions-1.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 $ poetry add async-extensions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-async-extensions = "^1.2.1"
+async-extensions = "^1.2.2"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.async-extensions]
 git = "https://github.com/nekitdev/async-extensions.git"
```

### Comparing `async_extensions-1.2.1/async_extensions/__init__.py` & `async_extensions-1.2.2/async_extensions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __description__ = "Asynchronous extensions."
 __url__ = "https://github.com/nekitdev/async-extensions"
 
 __title__ = "async_extensions"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 from async_extensions.blocking import run_blocking_in_process, run_blocking_in_thread
 from async_extensions.cancel import CancelScope, create_cancel_scope, shield
 from async_extensions.channel import (
     MemoryChannel, MemoryChannelFactory, MemoryReceiveChannel, MemorySendChannel
 )
 from async_extensions.close import (
```

### Comparing `async_extensions-1.2.1/async_extensions/blocking.py` & `async_extensions-1.2.2/async_extensions/blocking.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.1/async_extensions/channel.py` & `async_extensions-1.2.2/async_extensions/channel.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.1/async_extensions/close.py` & `async_extensions-1.2.2/async_extensions/close.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.1/async_extensions/collect.py` & `async_extensions-1.2.2/async_extensions/collect.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.1/async_extensions/standard.py` & `async_extensions-1.2.2/async_extensions/standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 NOT_ASYNC_ITERABLE = "{} is not an async iterable"
 NOT_ASYNC_ITERATOR = "{} is not an async iterator"
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
-async def async_iter(async_iterable: AsyncIterable[T]) -> AsyncIterator[T]:
+def async_iter(async_iterable: AsyncIterable[T]) -> AsyncIterator[T]:
     if is_instance(async_iterable, AsyncIterable):
         return async_iterable.__aiter__()
 
     raise TypeError(NOT_ASYNC_ITERABLE.format(repr(async_iterable)))
 
 
 @overload
```

### Comparing `async_extensions-1.2.1/async_extensions/typing.py` & `async_extensions-1.2.2/async_extensions/typing.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.1/async_extensions/wait.py` & `async_extensions-1.2.2/async_extensions/wait.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.1/pyproject.toml` & `async_extensions-1.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-extensions"
-version = "1.2.1"
+version = "1.2.2"
 description = "Asynchronous extensions."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/async-extensions"
@@ -34,24 +34,24 @@
 anyio = ">= 3.6.2"
 solus = ">= 1.1.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
-black = "22.12.0"
+black = "23.3.0"
 
 [tool.poetry.group.format.dependencies.isort]
-version = "5.11.4"
+version = "5.11.5"
 
 [tool.poetry.group.check]
 optional = true
 
 [tool.poetry.group.check.dependencies]
-mypy = "0.991"
+mypy = "1.1.1"
 
 [tool.poetry.group.dev.dependencies]
 changelogging = "1.1.0"
 
 [tool.black]
 line_length = 100
 
@@ -82,15 +82,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "async-extensions"
-version = "1.2.1"
+version = "1.2.2"
 url = "https://github.com/nekitdev/async-extensions"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `async_extensions-1.2.1/setup.py` & `async_extensions-1.2.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,124 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: async-extensions
+Version: 1.2.2
+Summary: Asynchronous extensions.
+Home-page: https://github.com/nekitdev/async-extensions
+License: MIT
+Keywords: python,async,extensions
+Author: nekitdev
+Requires-Python: >=3.7
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: anyio (>=3.6.2)
+Requires-Dist: solus (>=1.1.0)
+Project-URL: Discord, https://nekit.dev/discord
+Project-URL: Funding, https://patreon.com/nekitdev
+Project-URL: Issues, https://github.com/nekitdev/solus/issues
+Project-URL: Repository, https://github.com/nekitdev/async-extensions
+Description-Content-Type: text/markdown
 
-packages = \
-['async_extensions']
+# `async-extensions`
 
-package_data = \
-{'': ['*']}
+[![License][License Badge]][License]
+[![Version][Version Badge]][Package]
+[![Downloads][Downloads Badge]][Package]
+[![Discord][Discord Badge]][Discord]
+[![Check][Check Badge]][Actions]
 
-install_requires = \
-['anyio>=3.6.2', 'solus>=1.1.0']
-
-setup_kwargs = {
-    'name': 'async-extensions',
-    'version': '1.2.1',
-    'description': 'Asynchronous extensions.',
-    'long_description': '# `async-extensions`\n\n[![License][License Badge]][License]\n[![Version][Version Badge]][Package]\n[![Downloads][Downloads Badge]][Package]\n[![Discord][Discord Badge]][Discord]\n[![Check][Check Badge]][Actions]\n\n> *Asynchronous extensions.*\n\n## Installing\n\n**Python 3.7 or above is required.**\n\n### pip\n\nInstalling the library with `pip` is quite simple:\n\n```console\n$ pip install async-extensions\n```\n\nAlternatively, the library can be installed from source:\n\n```console\n$ git clone https://github.com/nekitdev/async-extensions.git\n$ cd async-extensions\n$ python -m pip install .\n```\n\n### poetry\n\nYou can add `async-extensions` as a dependency with the following command:\n\n```console\n$ poetry add async-extensions\n```\n\nOr by directly specifying it in the configuration like so:\n\n```toml\n[tool.poetry.dependencies]\nasync-extensions = "^1.2.1"\n```\n\nAlternatively, you can add it directly from the source:\n\n```toml\n[tool.poetry.dependencies.async-extensions]\ngit = "https://github.com/nekitdev/async-extensions.git"\n```\n\n## Support\n\nIf you need support with the library, you can send an [email][Email]\nor refer to the official [Discord server][Discord].\n\n## Changelog\n\nYou can find the changelog [here][Changelog].\n\n## Security Policy\n\nYou can find the Security Policy of `async-extensions` [here][Security].\n\n## Contributing\n\nIf you are interested in contributing to `async-extensions`, make sure to take a look at the\n[Contributing Guide][Contributing Guide], as well as the [Code of Conduct][Code of Conduct].\n\n## License\n\n`async-extensions` is licensed under the MIT License terms. See [License][License] for details.\n\n[Email]: mailto:support@nekit.dev\n\n[Discord]: https://nekit.dev/discord\n\n[Actions]: https://github.com/nekitdev/async-extensions/actions\n\n[Changelog]: https://github.com/nekitdev/async-extensions/blob/main/CHANGELOG.md\n[Code of Conduct]: https://github.com/nekitdev/async-extensions/blob/main/CODE_OF_CONDUCT.md\n[Contributing Guide]: https://github.com/nekitdev/async-extensions/blob/main/CONTRIBUTING.md\n[Security]: https://github.com/nekitdev/async-extensions/blob/main/SECURITY.md\n\n[License]: https://github.com/nekitdev/async-extensions/blob/main/LICENSE\n\n[Package]: https://pypi.org/project/async-extensions\n\n[Discord Badge]: https://img.shields.io/badge/chat-discord-5865f2\n[License Badge]: https://img.shields.io/pypi/l/async-extensions\n[Version Badge]: https://img.shields.io/pypi/v/async-extensions\n[Downloads Badge]: https://img.shields.io/pypi/dm/async-extensions\n[Check Badge]: https://github.com/nekitdev/async-extensions/workflows/check/badge.svg\n',
-    'author': 'nekitdev',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/nekitdev/async-extensions',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7',
-}
+> *Asynchronous extensions.*
 
+## Installing
+
+**Python 3.7 or above is required.**
+
+### pip
+
+Installing the library with `pip` is quite simple:
+
+```console
+$ pip install async-extensions
+```
+
+Alternatively, the library can be installed from source:
+
+```console
+$ git clone https://github.com/nekitdev/async-extensions.git
+$ cd async-extensions
+$ python -m pip install .
+```
+
+### poetry
+
+You can add `async-extensions` as a dependency with the following command:
+
+```console
+$ poetry add async-extensions
+```
+
+Or by directly specifying it in the configuration like so:
+
+```toml
+[tool.poetry.dependencies]
+async-extensions = "^1.2.2"
+```
+
+Alternatively, you can add it directly from the source:
+
+```toml
+[tool.poetry.dependencies.async-extensions]
+git = "https://github.com/nekitdev/async-extensions.git"
+```
+
+## Support
+
+If you need support with the library, you can send an [email][Email]
+or refer to the official [Discord server][Discord].
+
+## Changelog
+
+You can find the changelog [here][Changelog].
+
+## Security Policy
+
+You can find the Security Policy of `async-extensions` [here][Security].
+
+## Contributing
+
+If you are interested in contributing to `async-extensions`, make sure to take a look at the
+[Contributing Guide][Contributing Guide], as well as the [Code of Conduct][Code of Conduct].
+
+## License
+
+`async-extensions` is licensed under the MIT License terms. See [License][License] for details.
+
+[Email]: mailto:support@nekit.dev
+
+[Discord]: https://nekit.dev/discord
+
+[Actions]: https://github.com/nekitdev/async-extensions/actions
+
+[Changelog]: https://github.com/nekitdev/async-extensions/blob/main/CHANGELOG.md
+[Code of Conduct]: https://github.com/nekitdev/async-extensions/blob/main/CODE_OF_CONDUCT.md
+[Contributing Guide]: https://github.com/nekitdev/async-extensions/blob/main/CONTRIBUTING.md
+[Security]: https://github.com/nekitdev/async-extensions/blob/main/SECURITY.md
+
+[License]: https://github.com/nekitdev/async-extensions/blob/main/LICENSE
+
+[Package]: https://pypi.org/project/async-extensions
+
+[Discord Badge]: https://img.shields.io/badge/chat-discord-5865f2
+[License Badge]: https://img.shields.io/pypi/l/async-extensions
+[Version Badge]: https://img.shields.io/pypi/v/async-extensions
+[Downloads Badge]: https://img.shields.io/pypi/dm/async-extensions
+[Check Badge]: https://github.com/nekitdev/async-extensions/workflows/check/badge.svg
 
-setup(**setup_kwargs)
```

