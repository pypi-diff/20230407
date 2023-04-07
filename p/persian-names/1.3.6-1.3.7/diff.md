# Comparing `tmp/persian-names-1.3.6.tar.gz` & `tmp/persian-names-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persian-names-1.3.6.tar", last modified: Thu Mar 30 21:38:53 2023, max compression
+gzip compressed data, was "persian-names-1.3.7.tar", last modified: Fri Apr  7 21:14:01 2023, max compression
```

## Comparing `persian-names-1.3.6.tar` & `persian-names-1.3.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-03-30 21:38:53.426409 persian-names-1.3.6/
--rw-r--r--   0 arman      (501) staff       (20)     1068 2022-11-15 18:36:04.000000 persian-names-1.3.6/LICENSE
--rw-r--r--   0 arman      (501) staff       (20)     4006 2023-03-30 21:38:53.426291 persian-names-1.3.6/PKG-INFO
--rw-r--r--   0 arman      (501) staff       (20)     2700 2023-03-06 21:55:33.000000 persian-names-1.3.6/README.md
-drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-03-30 21:38:53.424460 persian-names-1.3.6/persian_names/
--rw-r--r--   0 arman      (501) staff       (20)       28 2022-11-21 18:59:10.000000 persian-names-1.3.6/persian_names/__init__.py
-drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-03-30 21:38:53.426057 persian-names-1.3.6/persian_names/data/
--rw-r--r--   0 arman      (501) staff       (20)     2229 2023-03-30 21:23:03.000000 persian-names-1.3.6/persian_names/data/female_en.txt
--rw-r--r--   0 arman      (501) staff       (20)     3367 2023-03-30 21:23:15.000000 persian-names-1.3.6/persian_names/data/female_fa.txt
--rw-r--r--   0 arman      (501) staff       (20)     2023 2023-03-30 21:23:44.000000 persian-names-1.3.6/persian_names/data/male_en.txt
--rw-r--r--   0 arman      (501) staff       (20)     3036 2023-03-30 21:25:09.000000 persian-names-1.3.6/persian_names/data/male_fa.txt
--rw-r--r--   0 arman      (501) staff       (20)        0 2023-03-06 21:07:00.000000 persian-names-1.3.6/persian_names/p.py
--rw-r--r--   0 arman      (501) staff       (20)     7623 2023-03-30 21:37:01.000000 persian-names-1.3.6/persian_names/persian_names.py
-drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-03-30 21:38:53.425023 persian-names-1.3.6/persian_names.egg-info/
--rw-r--r--   0 arman      (501) staff       (20)     4006 2023-03-30 21:38:53.000000 persian-names-1.3.6/persian_names.egg-info/PKG-INFO
--rw-r--r--   0 arman      (501) staff       (20)      378 2023-03-30 21:38:53.000000 persian-names-1.3.6/persian_names.egg-info/SOURCES.txt
--rw-r--r--   0 arman      (501) staff       (20)        1 2023-03-30 21:38:53.000000 persian-names-1.3.6/persian_names.egg-info/dependency_links.txt
--rw-r--r--   0 arman      (501) staff       (20)       14 2023-03-30 21:38:53.000000 persian-names-1.3.6/persian_names.egg-info/top_level.txt
--rw-r--r--   0 arman      (501) staff       (20)       38 2023-03-30 21:38:53.426517 persian-names-1.3.6/setup.cfg
--rw-r--r--   0 arman      (501) staff       (20)     1722 2023-03-30 21:23:03.000000 persian-names-1.3.6/setup.py
+drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-04-07 21:14:01.660453 persian-names-1.3.7/
+-rw-r--r--   0 arman      (501) staff       (20)     1068 2022-11-15 18:36:04.000000 persian-names-1.3.7/LICENSE
+-rw-r--r--   0 arman      (501) staff       (20)     4006 2023-04-07 21:14:01.660333 persian-names-1.3.7/PKG-INFO
+-rw-r--r--   0 arman      (501) staff       (20)     2700 2023-03-06 21:55:33.000000 persian-names-1.3.7/README.md
+drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-04-07 21:14:01.658272 persian-names-1.3.7/persian_names/
+-rw-r--r--   0 arman      (501) staff       (20)       28 2022-11-21 18:59:10.000000 persian-names-1.3.7/persian_names/__init__.py
+drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-04-07 21:14:01.660062 persian-names-1.3.7/persian_names/data/
+-rw-r--r--   0 arman      (501) staff       (20)     2239 2023-04-07 21:05:49.000000 persian-names-1.3.7/persian_names/data/female_en.txt
+-rw-r--r--   0 arman      (501) staff       (20)     3380 2023-04-07 21:06:05.000000 persian-names-1.3.7/persian_names/data/female_fa.txt
+-rw-r--r--   0 arman      (501) staff       (20)     2045 2023-04-07 21:06:37.000000 persian-names-1.3.7/persian_names/data/male_en.txt
+-rw-r--r--   0 arman      (501) staff       (20)     3069 2023-04-07 21:08:00.000000 persian-names-1.3.7/persian_names/data/male_fa.txt
+-rw-r--r--   0 arman      (501) staff       (20)        0 2023-03-06 21:07:00.000000 persian-names-1.3.7/persian_names/p.py
+-rw-r--r--   0 arman      (501) staff       (20)     7711 2023-04-07 21:10:44.000000 persian-names-1.3.7/persian_names/persian_names.py
+drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-04-07 21:14:01.658965 persian-names-1.3.7/persian_names.egg-info/
+-rw-r--r--   0 arman      (501) staff       (20)     4006 2023-04-07 21:14:01.000000 persian-names-1.3.7/persian_names.egg-info/PKG-INFO
+-rw-r--r--   0 arman      (501) staff       (20)      378 2023-04-07 21:14:01.000000 persian-names-1.3.7/persian_names.egg-info/SOURCES.txt
+-rw-r--r--   0 arman      (501) staff       (20)        1 2023-04-07 21:14:01.000000 persian-names-1.3.7/persian_names.egg-info/dependency_links.txt
+-rw-r--r--   0 arman      (501) staff       (20)       14 2023-04-07 21:14:01.000000 persian-names-1.3.7/persian_names.egg-info/top_level.txt
+-rw-r--r--   0 arman      (501) staff       (20)       38 2023-04-07 21:14:01.660571 persian-names-1.3.7/setup.cfg
+-rw-r--r--   0 arman      (501) staff       (20)     1722 2023-04-07 21:05:21.000000 persian-names-1.3.7/setup.py
```

### Comparing `persian-names-1.3.6/LICENSE` & `persian-names-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `persian-names-1.3.6/PKG-INFO` & `persian-names-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persian-names
-Version: 1.3.6
+Version: 1.3.7
 Summary: A Python library for generating random Persian (Farsi) names.
 Home-page: https://github.com/armanyazdi/persian-names
 Author: Arman Yazdi
 License: MIT
 Project-URL: Source, https://github.com/armanyazdi/persian-names
 Project-URL: Documentation, https://pypi.org/project/persian-names
 Keywords: persian names,farsi names,iranian names,name generator
```

### Comparing `persian-names-1.3.6/README.md` & `persian-names-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `persian-names-1.3.6/persian_names/data/female_en.txt` & `persian-names-1.3.7/persian_names/data/female_en.txt`

 * *Files 4% similar despite different names*

```diff
@@ -155,14 +155,15 @@
 Maryam
 Marzieh
 Masoumeh
 Mehdieh
 Mehrana
 Mehraneh
 Mehraveh
+Mehrdokht
 Mehrnaz
 Mehrnoush
 Mehrvash
 Melika
 Melina
 Melisa
 Mersana
```

### Comparing `persian-names-1.3.6/persian_names/data/female_fa.txt` & `persian-names-1.3.7/persian_names/data/female_fa.txt`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,15 @@
 مهتاب
 مهدیس
 مهدیه
 مهدیه
 مهرانا
 مهرانه
 مهراوه
+مهردخت
 مهرناز
 مهرنوش
 مهروش
 مهزاد
 مهسا
 مهشاد
 مهشید
```

### Comparing `persian-names-1.3.6/persian_names/data/male_en.txt` & `persian-names-1.3.7/persian_names/data/male_en.txt`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 Ashkan
 Barbod
 Bardia
 Hessam
 Mahyar
 Mani
 Masih
+Radin
 Rasam
 Roham
 Samyar
 Shantia
 Shervin
 Abdolreza
 Abed
@@ -178,16 +179,18 @@
 Kousha
 Mahan
 Mahdi
 Majid
 Manouchehr
 Masoud
 Matin
+Mazaher
 Mazdak
 Maziar
+Meghdad
 Mehrab
 Mehrad
 Mehran
 Mehrdad
 Mehrzad
 Meraj
 Meysam
```

### Comparing `persian-names-1.3.6/persian_names/data/male_fa.txt` & `persian-names-1.3.7/persian_names/data/male_fa.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 آریان
 اشکان
 اهورا
 باربد
 بردیا
 حسام
 سامیار
+رادین
 رسام
 رهام
 شروین
 شنتیا
 مانی
 مسیح
 مهیار
@@ -212,16 +213,18 @@
 مراد
 مرتضی
 مزدک
 مسعود
 مسلم
 مشفق
 مصطفی
+مظاهر
 معراج
 معین
+مقداد
 منوچهر
 مهدی
 مهراب
 مهراد
 مهران
 مهرداد
 مهرزاد
```

### Comparing `persian-names-1.3.6/persian_names/persian_names.py` & `persian-names-1.3.7/persian_names/persian_names.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         'Seyed',
         'Amir',
         'Aziz',
         'Shah',
         'Nik',
         'Haj',
         'Haji',
+        'Soufi',
         'Sheikh',
         'Mirza',
         'Ostad',
         'Malek',
         'Khan',
         'Beig',
         'Arab'
@@ -67,14 +68,15 @@
         'kohan', '',
         'nejad', '',
         'bayat', '',
         'yekta' '',
         'sabet' '',
         'azad', '',
         'zare', '',
+        'moghaddam', '',
     ]
     more_suffixes = [
         'pour', 'i',
         'zadeh', 'i',
         'far', 'i',
         'fard', 'i',
         'khani', 'i',
@@ -93,15 +95,15 @@
     names = f.read().split('\n')
     f.close()
     last_name = names[randrange(len(names))]
 
     for i in names[:26]:
         arabic_names.append(i)
 
-    for i in names[26:49]:
+    for i in names[26:50]:
         illegal_names.append(i)
 
     while last_name in illegal_names:
         last_name = names[randrange(len(names))]
 
     if last_name == 'Mostafa' or last_name == 'Mousa' or last_name == 'Yahya' or last_name == 'Kasra' or last_name == 'Mojtaba':
         last_name += 'vi'
@@ -179,14 +181,15 @@
         'سید',
         'امیر',
         'عزیز',
         'شاه ',
         'نیک ',
         'حاج ',
         'حاجی ',
+        'صوفی ',
         'شیخ ',
         'میرزا ',
         'استاد ',
         'ملک ',
         'خان ',
         'بیگ ',
         'عرب '
@@ -208,14 +211,15 @@
         ' کهن', '',
         ' نژاد', '',
         ' بیات', '',
         ' یکتا', '',
         ' ثابت', '',
         ' آزاد', '',
         ' زارع', '',
+        ' مقدم', '',
     ]
     more_suffixes = [
         ' پور', 'ی',
         ' زاده', 'ی',
         ' فر', 'ی',
         ' فرد', 'ی',
         ' خانی', 'ی',
@@ -231,18 +235,18 @@
     illegal_names = []
 
     f = open(path + '/data/' + files[2], 'r', encoding='utf8')
     names = f.read().split('\n')
     f.close()
     last_name = names[randrange(len(names))]
 
-    for i in names[:23]:
+    for i in names[:26]:
         arabic_names.append(i)
 
-    for i in names[26:49]:
+    for i in names[26:50]:
         illegal_names.append(i)
 
     while last_name in illegal_names:
         last_name = names[randrange(len(names))]
 
     if last_name == 'مرتضی' or last_name == 'مصطفی' or last_name == 'موسی' or last_name == 'کسری' or last_name == 'مجتبی':
         last_name = last_name.replace('ی', 'وی')
```

### Comparing `persian-names-1.3.6/persian_names.egg-info/PKG-INFO` & `persian-names-1.3.7/persian_names.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persian-names
-Version: 1.3.6
+Version: 1.3.7
 Summary: A Python library for generating random Persian (Farsi) names.
 Home-page: https://github.com/armanyazdi/persian-names
 Author: Arman Yazdi
 License: MIT
 Project-URL: Source, https://github.com/armanyazdi/persian-names
 Project-URL: Documentation, https://pypi.org/project/persian-names
 Keywords: persian names,farsi names,iranian names,name generator
```

### Comparing `persian-names-1.3.6/setup.py` & `persian-names-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('./README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='persian-names',
-    version='1.3.6',
+    version='1.3.7',
     packages=['persian_names'],
     include_package_data=True,
     data_files=[('', [
         'persian_names/data/female_en.txt',
         'persian_names/data/female_fa.txt',
         'persian_names/data/male_en.txt',
         'persian_names/data/male_fa.txt'
```

