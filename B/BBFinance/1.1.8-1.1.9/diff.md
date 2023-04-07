# Comparing `tmp/BBFinance-1.1.8.tar.gz` & `tmp/BBFinance-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BBFinance-1.1.8.tar", last modified: Thu Apr  6 19:50:28 2023, max compression
+gzip compressed data, was "BBFinance-1.1.9.tar", last modified: Fri Apr  7 21:49:06 2023, max compression
```

## Comparing `BBFinance-1.1.8.tar` & `BBFinance-1.1.9.tar`

### file list

```diff
@@ -1,21 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 19:53:40.283600 BBFinance-1.1.8/
-drwxrwxrwx   0        0        0        0 2023-04-06 19:53:39.658104 BBFinance-1.1.8/BBFinance/
--rw-rw-rw-   0        0        0    11914 2023-04-06 19:36:05.000000 BBFinance-1.1.8/BBFinance/BBFinance.py
--rw-rw-rw-   0        0        0      157 2023-04-05 20:39:07.000000 BBFinance-1.1.8/BBFinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 19:53:40.049031 BBFinance-1.1.8/BBFinance/__pycache__/
--rw-rw-rw-   0        0        0     8391 2023-04-06 19:36:07.000000 BBFinance-1.1.8/BBFinance/__pycache__/BBFinance.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-06 19:53:40.002126 BBFinance-1.1.8/BBFinance.egg-info/
--rw-rw-rw-   0        0        0     1988 2023-04-06 19:53:32.000000 BBFinance-1.1.8/BBFinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-04-06 19:53:38.000000 BBFinance-1.1.8/BBFinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 19:53:32.000000 BBFinance-1.1.8/BBFinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2023-04-06 19:53:32.000000 BBFinance-1.1.8/BBFinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-06 19:53:32.000000 BBFinance-1.1.8/BBFinance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1099 2023-04-04 20:31:26.000000 BBFinance-1.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0     1988 2023-04-06 19:53:40.283600 BBFinance-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1391 2023-04-05 15:18:39.000000 BBFinance-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 19:53:40.205395 BBFinance-1.1.8/__pycache__/
--rw-rw-rw-   0        0        0      301 2023-04-05 17:36:13.000000 BBFinance-1.1.8/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     8340 2023-04-05 15:20:09.000000 BBFinance-1.1.8/__pycache__/main.cpython-39.pyc
--rw-rw-rw-   0        0        0      300 2023-04-04 20:31:26.000000 BBFinance-1.1.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 19:53:40.330475 BBFinance-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1124 2023-04-06 19:52:56.000000 BBFinance-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:49:06.250962 BBFinance-1.1.9/
+drwxrwxrwx   0        0        0        0 2023-04-07 21:49:06.229962 BBFinance-1.1.9/BBFinance/
+-rw-rw-rw-   0        0        0    23223 2023-04-07 21:11:08.000000 BBFinance-1.1.9/BBFinance/BBFinance.py
+-rw-rw-rw-   0        0        0      157 2023-04-07 01:44:35.000000 BBFinance-1.1.9/BBFinance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:49:06.248962 BBFinance-1.1.9/BBFinance.egg-info/
+-rw-rw-rw-   0        0        0     1997 2023-04-07 21:49:06.000000 BBFinance-1.1.9/BBFinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-04-07 21:49:06.000000 BBFinance-1.1.9/BBFinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 21:49:06.000000 BBFinance-1.1.9/BBFinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      255 2023-04-07 21:49:06.000000 BBFinance-1.1.9/BBFinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-07 21:49:06.000000 BBFinance-1.1.9/BBFinance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1099 2023-04-07 01:44:35.000000 BBFinance-1.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     1997 2023-04-07 21:49:06.249962 BBFinance-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1400 2023-04-07 01:44:35.000000 BBFinance-1.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-07 21:49:06.250962 BBFinance-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1296 2023-04-07 21:48:17.000000 BBFinance-1.1.9/setup.py
```

### Comparing `BBFinance-1.1.8/BBFinance.egg-info/PKG-INFO` & `BBFinance-1.1.9/BBFinance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.1.8
+Version: 1.1.9
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -35,17 +35,17 @@
 `pip install BBFinance`
 
 ## Uso
 
 Para usar a biblioteca, basta importar o módulo e chamar as funções apropriadas. Aqui está um exemplo de código para coletar as informações de uma ação:
 
 ```python-repl
-import BBFinance
+import BBFinance as bb
 
-get_info('PETR4.SA') -> #Pega as principais informações da ação
+bb.get_info('PETR4.SA') -> #Pega as principais informações da ação
 ```
 
 ## Contribuições
 
 Contribuições são bem-vindas! Se você deseja contribuir para a biblioteca, por favor, abra uma issue no repositório para discutir a sua ideia ou submeta um pull request.
 
 ## Licença
```

### Comparing `BBFinance-1.1.8/LICENSE.txt` & `BBFinance-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.1.8/PKG-INFO` & `BBFinance-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.1.8
+Version: 1.1.9
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -35,17 +35,17 @@
 `pip install BBFinance`
 
 ## Uso
 
 Para usar a biblioteca, basta importar o módulo e chamar as funções apropriadas. Aqui está um exemplo de código para coletar as informações de uma ação:
 
 ```python-repl
-import BBFinance
+import BBFinance as bb
 
-get_info('PETR4.SA') -> #Pega as principais informações da ação
+bb.get_info('PETR4.SA') -> #Pega as principais informações da ação
 ```
 
 ## Contribuições
 
 Contribuições são bem-vindas! Se você deseja contribuir para a biblioteca, por favor, abra uma issue no repositório para discutir a sua ideia ou submeta um pull request.
 
 ## Licença
```

### Comparing `BBFinance-1.1.8/README.md` & `BBFinance-1.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 `pip install BBFinance`
 
 ## Uso
 
 Para usar a biblioteca, basta importar o módulo e chamar as funções apropriadas. Aqui está um exemplo de código para coletar as informações de uma ação:
 
 ```python-repl
-import BBFinance
+import BBFinance as bb
 
-get_info('PETR4.SA') -> #Pega as principais informações da ação
+bb.get_info('PETR4.SA') -> #Pega as principais informações da ação
 ```
 
 ## Contribuições
 
 Contribuições são bem-vindas! Se você deseja contribuir para a biblioteca, por favor, abra uma issue no repositório para discutir a sua ideia ou submeta um pull request.
 
 ## Licença
```

### Comparing `BBFinance-1.1.8/setup.py` & `BBFinance-1.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
-with open(r'Q:\Risco\Novo Risco\pythonrisco\BBFinance\README.md', 'r', encoding='utf-8') as f:
+with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='BBFinance',
-    version='1.1.8',
+    version='1.1.9',
     description='Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado',
     url='https://github.com/beb0pp/BBFinance',
     author='Luis Abreu',
     author_email='luss.fel@gmail.com',
     license='MIT',
     packages=['BBFinance'],
     long_description= long_description,
@@ -19,14 +19,22 @@
         'scipy>=1.9.3',
         'selenium>=3.141.0',
         'pandas-datareader>=0.10.0',
         'json5>=0.9.6',
         'numpy>=1.23.4',
         'uvicorn>=0.21.1',
         'fastapi>=0.95.0',
+        'scipy>=1.10.1',
+        'requests>=2.28.2',
+        'bs4>=0.0.1',
+        'beautifulsoup4>=4.11.2',
+        'pydantic>=1.10.7',
+        'Unicode>=1.3.6',
+        'typing_extensions>=4.5.0'
+        
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.9',
     ],
```

