# Comparing `tmp/cryptographyComplements-0.2.2.tar.gz` & `tmp/cryptographyComplements-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptographyComplements-0.2.2.tar", last modified: Fri Mar 31 17:55:24 2023, max compression
+gzip compressed data, was "cryptographyComplements-0.2.3.tar", last modified: Fri Apr  7 19:39:36 2023, max compression
```

## Comparing `cryptographyComplements-0.2.2.tar` & `cryptographyComplements-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 17:55:24.987977 cryptographyComplements-0.2.2/
--rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      579 2023-03-31 17:55:24.987977 cryptographyComplements-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-03-18 18:48:58.000000 cryptographyComplements-0.2.2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 17:55:24.985556 cryptographyComplements-0.2.2/cryptographyComplements/
--rw-rw-rw-   0        0        0      197 2023-03-18 18:48:58.000000 cryptographyComplements-0.2.2/cryptographyComplements/__init__.py
--rw-rw-rw-   0        0        0     1629 2023-03-18 19:21:02.000000 cryptographyComplements-0.2.2/cryptographyComplements/ciphers.py
--rw-rw-rw-   0        0        0     8750 2023-03-31 17:47:48.000000 cryptographyComplements-0.2.2/cryptographyComplements/mathFunctions.py
--rw-rw-rw-   0        0        0     2112 2023-03-31 15:50:23.000000 cryptographyComplements-0.2.2/cryptographyComplements/primalityTests.py
--rw-rw-rw-   0        0        0     2252 2023-03-31 15:53:30.000000 cryptographyComplements-0.2.2/cryptographyComplements/tools.py
-drwxrwxrwx   0        0        0        0 2023-03-31 17:55:24.986971 cryptographyComplements-0.2.2/cryptographyComplements.egg-info/
--rw-rw-rw-   0        0        0      279 2023-03-31 17:55:24.000000 cryptographyComplements-0.2.2/cryptographyComplements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 17:55:24.987977 cryptographyComplements-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-03-31 16:47:35.000000 cryptographyComplements-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:39:36.454987 cryptographyComplements-0.2.3/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      579 2023-04-07 19:39:36.454544 cryptographyComplements-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-03-18 18:48:58.000000 cryptographyComplements-0.2.3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:39:36.450215 cryptographyComplements-0.2.3/cryptographyComplements/
+-rw-rw-rw-   0        0        0      197 2023-03-18 18:48:58.000000 cryptographyComplements-0.2.3/cryptographyComplements/__init__.py
+-rw-rw-rw-   0        0        0     1629 2023-03-18 19:21:02.000000 cryptographyComplements-0.2.3/cryptographyComplements/ciphers.py
+-rw-rw-rw-   0        0        0     9393 2023-04-07 19:35:52.000000 cryptographyComplements-0.2.3/cryptographyComplements/mathFunctions.py
+-rw-rw-rw-   0        0        0     2510 2023-04-07 19:28:48.000000 cryptographyComplements-0.2.3/cryptographyComplements/primalityTests.py
+-rw-rw-rw-   0        0        0     2252 2023-03-31 15:53:30.000000 cryptographyComplements-0.2.3/cryptographyComplements/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:39:36.452749 cryptographyComplements-0.2.3/cryptographyComplements.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-04-07 19:39:36.000000 cryptographyComplements-0.2.3/cryptographyComplements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       42 2023-04-07 19:39:36.454987 cryptographyComplements-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-04-07 19:39:31.000000 cryptographyComplements-0.2.3/setup.py
```

### Comparing `cryptographyComplements-0.2.2/LICENSE` & `cryptographyComplements-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.2/PKG-INFO` & `cryptographyComplements-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptographyComplements
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python library, in development, that allows the user to use cryptography, and related, functions.
 Author: Forzo
 License: GPL-3.0
 Project-URL: Source, https://github.com/Forzooo/cryptographyComplements
 Project-URL: Documentation, https://cryptographycomplements.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `cryptographyComplements-0.2.2/cryptographyComplements/ciphers.py` & `cryptographyComplements-0.2.3/cryptographyComplements/ciphers.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.2/cryptographyComplements/mathFunctions.py` & `cryptographyComplements-0.2.3/cryptographyComplements/mathFunctions.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         p += 1
     if number > 1:
         result -= result // number
     return result
 
 def EuclideanAlgorithm(a: int, b: int):
     "Given two numbers, a and b, calculate their Great Common Divisor."
-    if not isinstance(a, int) or not isinstance(b, int):
+    if a % 1 != 0 or b % 1 != 0:
         return None
 
     a, b = int(a), int(b)
 
     while True:
         r = a % b
         if r != 0:
@@ -258,8 +258,37 @@
     gcd, x, y = ExtendedEuclideanAlgorithm(number, modulo)
 
 
     if gcd != 1:
 
         return None # There isn't an inverse modulo
     
-    return x % modulo
+    return x % modulo
+
+
+def FermatLittleTheorem(a:int, p:int) -> int:
+    "From a given integer and a prime number, calculate the Fermat Little Theorem."
+    return ((a**(p-1)) % p)
+
+
+def MultiplicativePersistence(num: int):
+    "From a given integer in input, calculate the multiplicative persistence. The function will return the number of steps required."
+
+    result, steps = 1, 0
+
+    for i in str(num):
+        result = int(i) * result
+
+    steps += 1
+
+
+    while len(str(result)) != 1:
+        # print(result)
+        num = result
+        result = 1        
+        for i in str(num):
+
+            result *= int(i)
+
+        steps += 1
+
+    return steps
```

### Comparing `cryptographyComplements-0.2.2/cryptographyComplements/primalityTests.py` & `cryptographyComplements-0.2.3/cryptographyComplements/primalityTests.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,8 +50,20 @@
         lucaslehmerSequence = MersennePrime.LucasLehmerModuloNumbers(power-1, mersenne)
 
         x = lucaslehmerSequence[power-2] / mersenne
 
         if x.is_integer():
             return True
         
-        return False
+        return False
+    
+def FermatPrimalityTest(p:int, a:int):
+    "From a given number and an integer, check if the number is prime. The Fermat Primality test is probabilistic."
+    from cryptographyComplements import EuclideanAlgorithm, FermatLittleTheorem
+
+    if EuclideanAlgorithm(p, a) != 1:
+        return False
+    
+    if FermatLittleTheorem(a, p) == 1:
+        return True
+    
+    return False
```

### Comparing `cryptographyComplements-0.2.2/cryptographyComplements/tools.py` & `cryptographyComplements-0.2.3/cryptographyComplements/tools.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.2/setup.py` & `cryptographyComplements-0.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cryptographyComplements',
-    version='0.2.2',
+    version='0.2.3',
     description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description_content_type='text/markdown',
     author='Forzo',
     packages=find_packages(),
     license="GPL-3.0",
     project_urls={
```

