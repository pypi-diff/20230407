# Comparing `tmp/execsql-1.97.0.tar.gz` & `tmp/execsql-1.98.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "execsql-1.97.0.tar", last modified: Sun Jan  9 16:14:21 2022, max compression
+gzip compressed data, was "execsql-1.98.0.tar", last modified: Wed Jan 12 15:47:14 2022, max compression
```

## Comparing `execsql-1.97.0.tar` & `execsql-1.98.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2022-01-09 16:14:21.732164 execsql-1.97.0/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2021-01-09 18:28:14.000000 execsql-1.97.0/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2020-09-20 22:52:28.000000 execsql-1.97.0/MANIFEST.in
--rw-rw-r--   0 dreas     (1000) dreas     (1000)    18905 2022-01-09 16:14:21.732164 execsql-1.97.0/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)    14540 2021-01-09 18:27:23.000000 execsql-1.97.0/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2022-01-09 16:14:21.728165 execsql-1.97.0/execsql/
--rwxrwxr-x   0 dreas     (1000) dreas     (1000)   562962 2022-01-09 01:31:25.000000 execsql-1.97.0/execsql/execsql.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2022-01-09 16:14:21.732164 execsql-1.97.0/execsql.egg-info/
--rw-r--r--   0 dreas     (1000) dreas     (1000)    18905 2022-01-09 16:14:21.000000 execsql-1.97.0/execsql.egg-info/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)      185 2022-01-09 16:14:21.000000 execsql-1.97.0/execsql.egg-info/SOURCES.txt
--rw-r--r--   0 dreas     (1000) dreas     (1000)        1 2022-01-09 16:14:21.000000 execsql-1.97.0/execsql.egg-info/dependency_links.txt
--rw-r--r--   0 dreas     (1000) dreas     (1000)        1 2022-01-09 16:14:21.000000 execsql-1.97.0/execsql.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2022-01-09 16:14:21.732164 execsql-1.97.0/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     2202 2022-01-09 01:21:19.000000 execsql-1.97.0/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2022-01-12 15:47:14.094083 execsql-1.98.0/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2021-01-09 18:28:14.000000 execsql-1.98.0/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2020-09-20 22:52:28.000000 execsql-1.98.0/MANIFEST.in
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)    18905 2022-01-12 15:47:14.094083 execsql-1.98.0/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)    14540 2021-01-09 18:27:23.000000 execsql-1.98.0/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2022-01-12 15:47:14.094083 execsql-1.98.0/execsql/
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   564183 2022-01-12 15:24:28.000000 execsql-1.98.0/execsql/execsql.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2022-01-12 15:47:14.094083 execsql-1.98.0/execsql.egg-info/
+-rw-r--r--   0 dreas     (1000) dreas     (1000)    18905 2022-01-12 15:47:13.000000 execsql-1.98.0/execsql.egg-info/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)      185 2022-01-12 15:47:14.000000 execsql-1.98.0/execsql.egg-info/SOURCES.txt
+-rw-r--r--   0 dreas     (1000) dreas     (1000)        1 2022-01-12 15:47:14.000000 execsql-1.98.0/execsql.egg-info/dependency_links.txt
+-rw-r--r--   0 dreas     (1000) dreas     (1000)        1 2022-01-12 15:47:14.000000 execsql-1.98.0/execsql.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2022-01-12 15:47:14.094083 execsql-1.98.0/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     2202 2022-01-12 14:54:47.000000 execsql-1.98.0/setup.py
```

### Comparing `execsql-1.97.0/LICENSE.txt` & `execsql-1.98.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `execsql-1.97.0/PKG-INFO` & `execsql-1.98.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: execsql
-Version: 1.97.0
+Version: 1.98.0
 Summary: Runs a SQL script against a PostgreSQL, MS-Access, SQLite, MS-SQL-Server, MySQL, MariaDB, Firebird, or Oracle database, or an ODBC DSN.  Provides metacommands to import and export data, copy data between databases, conditionally execute SQL and metacommands, and dynamically alter SQL and metacommands with substitution variables.  Data can be exported in 18 different formats, including CSV, TSV, ODS, HTML, JSON, LaTeX, and Markdown tables, and using custom templates.
 Home-page: https://osdn.net/project/execsql/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Description: ![execsql logo](https://static-cdn.osdn.net/thumb/g/6/107/150x150_0.png)  *Multi-DBMS SQL script processor.*
```

### Comparing `execsql-1.97.0/README.md` & `execsql-1.98.0/README.md`

 * *Files identical despite different names*

### Comparing `execsql-1.97.0/execsql/execsql.py` & `execsql-1.98.0/execsql/execsql.py`

 * *Files identical despite different names*

```diff
@@ -23,19 +23,19 @@
 # 	but WITHOUT ANY WARRANTY; without even the implied warranty of
 # 	MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # 	GNU General Public License for more details.
 # 	The GNU General Public License is available at <http://www.gnu.org/licenses/>
 #
 # ===============================================================================
 
-__version__ = "1.97.0"
-__vdate = "2022-01-08"
+__version__ = "1.98.0"
+__vdate = "2022-01-12"
 
 primary_vno   = 1
-secondary_vno = 97
+secondary_vno = 98
 tertiary_vno  = 0
 
 import os
 import os.path
 import sys
 import stat
 import datetime
@@ -274,14 +274,15 @@
 		self.boolean_int = True
 		self.boolean_words = False
 		self.empty_strings = True
 		self.only_strings = False
 		self.empty_rows = True
 		self.create_col_hdrs = False
 		self.clean_col_hdrs = False
+		self.fold_col_hdrs = 'no'
 		self.dedup_col_hdrs = False
 		self.trim_strings = False
 		self.replace_newlines = False
 		self.access_use_numeric = False
 		self.scan_lines = 100
 		self.hdf5_text_len = 1000
 		self.write_warnings = False
@@ -429,14 +430,18 @@
 					except:
 						raise ConfigError("Invalid argument to create_column_headers.")
 				if cp.has_option(self._INPUT_SECTION, "clean_column_headers"):
 					try:
 						self.clean_col_hdrs = cp.getboolean(self._INPUT_SECTION, "clean_column_headers")
 					except:
 						raise ConfigError("Invalid argument to clean_column_headers.")
+				if cp.has_option(self._INPUT_SECTION, "fold_column_headers"):
+					foldspec = cp.get(self._INPUT_SECTION, "fold_column_headers").lower()
+					if foldspec not in ('no', 'lower', 'upper'):
+						raise ConfigError("Invalid argument to fold_column_headers: %s." % foldspec)
 				if cp.has_option(self._INPUT_SECTION, "dedup_column_headers"):
 					try:
 						self.dedup_col_hdrs = cp.getboolean(self._INPUT_SECTION, "dedup_column_headers")
 					except:
 						raise ConfigError("Invalid argument to dedup_column_headers.")
 				if cp.has_option(self._INPUT_SECTION, "trim_strings"):
 					try:
@@ -779,20 +784,35 @@
 	if re.match(r'^\s*[+-]?\d+\s*$', strval):
 		return int(strval)
 	if re.match(r'^\s*[+-]?(\d+(\.\d*)?|\.\d+)([eE][+-]?\d+)?\s*$', strval):
 		return float(strval)
 	return None
 
 def clean_word(word):
-	# Trims leading and trailing spaces and replaces all non-alphanumeric characters with an underscore.
-	return re.sub(r'\W+', '_', word.strip(), flags=re.I)
+	# Trim leading and trailing spaces and replaces all non-alphanumeric characters with an underscore.
+	s1 = re.sub(r'\W+', '_', word.strip(), flags=re.I)
+	# Maybe add leading underscore.
+	if s1[0] in '0123456789':
+		return '_'+s1
+	return s1
 
 def clean_words(wordlist):
 	return [clean_word(w) for w in wordlist]
 
+def fold_word(word, foldspec):
+	# foldspec should be 'no', 'lower', or 'upper'.
+	if foldspec == 'lower':
+		return word.lower()
+	elif foldspec == 'upper':
+		return word.upper()
+	return word
+
+def fold_words(wordlist, foldspec):
+	return [fold_word(w, foldspec) for w in wordlist]
+
 def dedup_words(wordlist):
 	# Adds an item number suffix to duplicated words.
 	w2 = wordlist
 	dup_ix = [ix for ix, w, in enumerate(w2) if w.lower() in [wrd.lower() for wrd in w2[:ix]]]
 	while len(dup_ix) > 0:
 		w2 = [w + "_%s" % str(ix+1) if ix in dup_ix else w for ix, w in enumerate(w2)]
 		dup_ix = [ix for ix, w, in enumerate(w2) if w.lower() in [wrd.lower() for wrd in w2[:ix]]]
@@ -5361,14 +5381,16 @@
 				for i in range(len(colnames)):
 					if colnames[i] is None or len(colnames[i]) == 0:
 						colnames[i] = "Col%s" % str(i+1)
 			else:
 				raise ErrInfo(type="error", other_msg=u"The input file %s has missing column headers." % self.csvfname)
 		if conf.clean_col_hdrs:
 			colnames = clean_words(colnames)
+		if conf.fold_col_hdrs != 'no':
+			colnames = fold_words(colnames, conf.fold_col_hdrs)
 		if conf.dedup_col_hdrs:
 			colnames = dedup_words(colnames)
 		return colnames
 	def column_headers(self):
 		if not self.lineformat_set:
 			self.evaluate_line_format()
 		inf = self.reader()
@@ -11015,14 +11037,22 @@
 	conf.boolean_int = flag in ('yes', 'on', 'true', '1')
 	return None
 
 metacommandlist.add(r'^\s*BOOLEAN_WORDS\s+(?P<yesno>YES|NO|ON|OFF|TRUE|FALSE|0|1)\s*$', x_boolean_words)
 metacommandlist.add(r'^\s*CONFIG\s+BOOLEAN_WORDS\s+(?P<yesno>YES|NO|ON|OFF|TRUE|FALSE|0|1)\s*$', x_boolean_words)
 
 
+#****	FOLD_COLUMN_HEADERS
+def x_fold_col_hdrs(**kwargs):
+	conf.fold_col_hdrs = kwargs['foldspec']
+	return None
+
+metacommandlist.add(r'^\s*CONFIG\s+FOLD_COLUMN_HEADERS\s+(?P<foldspec>no|lower|upper)\s*$', x_fold_col_hdrs)
+
+
 #****	CLEAN_COLUMN_HEADERS
 def x_clean_col_hdrs(**kwargs):
 	flag = kwargs['yesno'].lower()
 	conf.clean_col_hdrs = flag in ('yes', 'on', 'true', '1')
 	return None
 
 metacommandlist.add(r'^\s*CLEAN_COLUMN_HEADERS\s+(?P<yesno>YES|NO|ON|OFF|TRUE|FALSE|0|1)\s*$', x_clean_col_hdrs)
@@ -13509,14 +13539,16 @@
 			for i in range(len(colhdrs)):
 				if colhdrs[i] is None or len(colhdrs[i]) == 0:
 					colhdrs[i] = "Col%s" % str(i+1)
 		else:
 			raise ErrInfo(type="error", other_msg=u"The input file %s, sheet %s has missing column headers." % (filename, sheetname))
 	if conf.clean_col_hdrs:
 		colhdrs = clean_words(colhdrs)
+	if conf.fold_col_hdrs != 'no':
+		colhdrs = fold_words(colhdrs, conf.fold_col_hdrs)
 	if conf.dedup_col_hdrs:
 		colhdrs = dedup_words(colhdrs)
 	return colhdrs, alldata[1:]
 
 def xls_data(filename, sheetname, junk_header_rows, encoding=None):
 	# Returns the data from the specified worksheet as a list of headers and a list of lists of rows.
 	if len(filename) < 4:
@@ -13546,14 +13578,16 @@
 			for i in range(len(colhdrs)):
 				if colhdrs[i] is None or len(colhdrs[i]) == 0:
 					colhdrs[i] = "Col%s" % str(i+1)
 		else:
 			raise ErrInfo(type="error", other_msg=u"The input file %s, sheet %s has missing column headers." % (filename, sheetname))
 	if conf.clean_col_hdrs:
 		colhdrs = clean_words(colhdrs)
+	if conf.fold_col_hdrs != 'no':
+		colhdrs = fold_words(colhdrs, conf.fold_col_hdrs)
 	if conf.dedup_col_hdrs:
 		colhdrs = dedup_words(colhdrs)
 	return colhdrs, alldata[1:]
 
 
 def import_data_table(db, schemaname, tablename, is_new, hdrs, data):
 	global conf
@@ -13562,14 +13596,16 @@
 			for i in range(len(hdrs)):
 				if hdrs[i] is None or len(hdrs[i]) == 0:
 					hdrs[i] = "Col%s" % str(i+1)
 		else:
 			raise ErrInfo(type="error", other_msg=u"The input data has missing column headers.")
 	if conf.clean_col_hdrs:
 		hdrs = clean_words(hdrs)
+	if conf.fold_col_hdrs != 'no':
+		hdrs = fold_words(hdrs, conf.fold_col_hdrs)
 	if conf.dedup_col_hdrs:
 		hdrs = dedup_words(hdrs)
 	def get_ts():
 		if not get_ts.tablespec:
 			get_ts.tablespec = DataTable(hdrs, data)
 		return get_ts.tablespec
 	get_ts.tablespec = None
```

### Comparing `execsql-1.97.0/execsql.egg-info/PKG-INFO` & `execsql-1.98.0/execsql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: execsql
-Version: 1.97.0
+Version: 1.98.0
 Summary: Runs a SQL script against a PostgreSQL, MS-Access, SQLite, MS-SQL-Server, MySQL, MariaDB, Firebird, or Oracle database, or an ODBC DSN.  Provides metacommands to import and export data, copy data between databases, conditionally execute SQL and metacommands, and dynamically alter SQL and metacommands with substitution variables.  Data can be exported in 18 different formats, including CSV, TSV, ODS, HTML, JSON, LaTeX, and Markdown tables, and using custom templates.
 Home-page: https://osdn.net/project/execsql/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Description: ![execsql logo](https://static-cdn.osdn.net/thumb/g/6/107/150x150_0.png)  *Multi-DBMS SQL script processor.*
```

### Comparing `execsql-1.97.0/setup.py` & `execsql-1.98.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import io
 
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 setuptools.setup(name='execsql',
-	version='1.97.0',
+	version='1.98.0',
 	description="Runs a SQL script against a PostgreSQL, MS-Access, SQLite, MS-SQL-Server, MySQL, MariaDB, Firebird, or Oracle database, or an ODBC DSN.  Provides metacommands to import and export data, copy data between databases, conditionally execute SQL and metacommands, and dynamically alter SQL and metacommands with substitution variables.  Data can be exported in 18 different formats, including CSV, TSV, ODS, HTML, JSON, LaTeX, and Markdown tables, and using custom templates.",
 	author='Dreas Nielsen',
 	author_email='dreas.nielsen@gmail.com',
     url='https://osdn.net/project/execsql/',
 	scripts=['execsql/execsql.py'],
     license='GPL',
 	requires=[],
```

