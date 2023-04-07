# Comparing `tmp/globalsearch-0.1.8.tar.gz` & `tmp/globalsearch-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalsearch-0.1.8.tar", last modified: Tue Mar 21 19:23:44 2023, max compression
+gzip compressed data, was "globalsearch-0.1.9.tar", last modified: Fri Apr  7 20:19:25 2023, max compression
```

## Comparing `globalsearch-0.1.8.tar` & `globalsearch-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-03-21 19:23:44.151612 globalsearch-0.1.8/
--rw-r--r--   0 weiju      (501) staff       (20)      951 2023-03-21 19:23:44.151670 globalsearch-0.1.8/PKG-INFO
--rw-r--r--   0 weiju      (501) staff       (20)      252 2022-12-13 19:27:00.000000 globalsearch-0.1.8/README.md
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-03-21 19:23:44.147421 globalsearch-0.1.8/bin/
--rwxr--r--   0 weiju      (501) staff       (20)      533 2023-01-09 18:49:49.000000 globalsearch-0.1.8/bin/gs_prepare
--rwxr-xr-x   0 weiju      (501) staff       (20)     1268 2023-02-09 22:31:19.000000 globalsearch-0.1.8/bin/gs_submit
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-03-21 19:23:44.146427 globalsearch-0.1.8/globalsearch/
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-03-21 19:23:44.148544 globalsearch-0.1.8/globalsearch/control/
--rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-10 16:54:29.000000 globalsearch-0.1.8/globalsearch/control/__init__.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     6635 2023-02-24 18:56:53.000000 globalsearch-0.1.8/globalsearch/control/gs_prepare.py
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-03-21 19:23:44.151393 globalsearch-0.1.8/globalsearch/rnaseq/
--rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-09 00:21:15.000000 globalsearch-0.1.8/globalsearch/rnaseq/__init__.py
--rw-r--r--   0 weiju      (501) staff       (20)     7034 2023-03-21 18:06:55.000000 globalsearch-0.1.8/globalsearch/rnaseq/find_files.py
--rw-r--r--   0 weiju      (501) staff       (20)     2379 2023-03-10 21:05:42.000000 globalsearch-0.1.8/globalsearch/rnaseq/index_star.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     2130 2023-02-09 22:31:19.000000 globalsearch-0.1.8/globalsearch/rnaseq/make_kallisto_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     2625 2023-02-24 18:56:53.000000 globalsearch-0.1.8/globalsearch/rnaseq/make_star_idx_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     5314 2023-02-24 18:56:53.000000 globalsearch-0.1.8/globalsearch/rnaseq/make_star_salmon_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     1634 2023-02-09 22:31:19.000000 globalsearch-0.1.8/globalsearch/rnaseq/post_star_salmon.py
--rwxr--r--   0 weiju      (501) staff       (20)     5497 2023-01-06 20:10:59.000000 globalsearch-0.1.8/globalsearch/rnaseq/run_kallisto.py
--rw-r--r--   0 weiju      (501) staff       (20)    14661 2023-03-10 21:10:17.000000 globalsearch-0.1.8/globalsearch/rnaseq/run_spladder.py
--rwxr-xr-x   0 weiju      (501) staff       (20)    12337 2023-03-21 18:06:55.000000 globalsearch-0.1.8/globalsearch/rnaseq/run_star_salmon.py
--rw-r--r--   0 weiju      (501) staff       (20)     3664 2023-03-21 18:06:55.000000 globalsearch-0.1.8/globalsearch/rnaseq/trim_galore.py
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-03-21 19:23:44.148335 globalsearch-0.1.8/globalsearch.egg-info/
--rw-r--r--   0 weiju      (501) staff       (20)      951 2023-03-21 19:23:44.000000 globalsearch-0.1.8/globalsearch.egg-info/PKG-INFO
--rw-r--r--   0 weiju      (501) staff       (20)      751 2023-03-21 19:23:44.000000 globalsearch-0.1.8/globalsearch.egg-info/SOURCES.txt
--rw-r--r--   0 weiju      (501) staff       (20)        1 2023-03-21 19:23:44.000000 globalsearch-0.1.8/globalsearch.egg-info/dependency_links.txt
--rw-r--r--   0 weiju      (501) staff       (20)        1 2022-12-15 20:31:36.000000 globalsearch-0.1.8/globalsearch.egg-info/not-zip-safe
--rw-r--r--   0 weiju      (501) staff       (20)       25 2023-03-21 19:23:44.000000 globalsearch-0.1.8/globalsearch.egg-info/requires.txt
--rw-r--r--   0 weiju      (501) staff       (20)       13 2023-03-21 19:23:44.000000 globalsearch-0.1.8/globalsearch.egg-info/top_level.txt
--rw-r--r--   0 weiju      (501) staff       (20)       67 2023-03-21 19:23:44.151869 globalsearch-0.1.8/setup.cfg
--rw-r--r--   0 weiju      (501) staff       (20)     1611 2023-03-10 21:12:13.000000 globalsearch-0.1.8/setup.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-07 20:19:25.220249 globalsearch-0.1.9/
+-rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-07 20:19:25.220319 globalsearch-0.1.9/PKG-INFO
+-rw-r--r--   0 weiju      (501) staff       (20)      252 2022-12-13 19:27:00.000000 globalsearch-0.1.9/README.md
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-07 20:19:25.215184 globalsearch-0.1.9/bin/
+-rwxr--r--   0 weiju      (501) staff       (20)      533 2023-01-09 18:49:49.000000 globalsearch-0.1.9/bin/gs_prepare
+-rwxr-xr-x   0 weiju      (501) staff       (20)     1268 2023-02-09 22:31:19.000000 globalsearch-0.1.9/bin/gs_submit
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-07 20:19:25.214271 globalsearch-0.1.9/globalsearch/
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-07 20:19:25.216359 globalsearch-0.1.9/globalsearch/control/
+-rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-10 16:54:29.000000 globalsearch-0.1.9/globalsearch/control/__init__.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     6635 2023-02-24 18:56:53.000000 globalsearch-0.1.9/globalsearch/control/gs_prepare.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-07 20:19:25.219965 globalsearch-0.1.9/globalsearch/rnaseq/
+-rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-09 00:21:15.000000 globalsearch-0.1.9/globalsearch/rnaseq/__init__.py
+-rw-r--r--   0 weiju      (501) staff       (20)     7034 2023-03-21 18:06:55.000000 globalsearch-0.1.9/globalsearch/rnaseq/find_files.py
+-rw-r--r--   0 weiju      (501) staff       (20)     2978 2023-04-07 20:18:38.000000 globalsearch-0.1.9/globalsearch/rnaseq/index_star.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     2130 2023-02-09 22:31:19.000000 globalsearch-0.1.9/globalsearch/rnaseq/make_kallisto_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     3120 2023-04-07 20:18:38.000000 globalsearch-0.1.9/globalsearch/rnaseq/make_star_idx_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     6154 2023-04-07 20:18:38.000000 globalsearch-0.1.9/globalsearch/rnaseq/make_star_salmon_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     1634 2023-02-09 22:31:19.000000 globalsearch-0.1.9/globalsearch/rnaseq/post_star_salmon.py
+-rwxr--r--   0 weiju      (501) staff       (20)     5497 2023-01-06 20:10:59.000000 globalsearch-0.1.9/globalsearch/rnaseq/run_kallisto.py
+-rw-r--r--   0 weiju      (501) staff       (20)    14661 2023-03-10 21:10:17.000000 globalsearch-0.1.9/globalsearch/rnaseq/run_spladder.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)    12988 2023-04-07 20:18:38.000000 globalsearch-0.1.9/globalsearch/rnaseq/run_star_salmon.py
+-rw-r--r--   0 weiju      (501) staff       (20)     3664 2023-03-21 18:06:55.000000 globalsearch-0.1.9/globalsearch/rnaseq/trim_galore.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-07 20:19:25.216136 globalsearch-0.1.9/globalsearch.egg-info/
+-rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-07 20:19:25.000000 globalsearch-0.1.9/globalsearch.egg-info/PKG-INFO
+-rw-r--r--   0 weiju      (501) staff       (20)      751 2023-04-07 20:19:25.000000 globalsearch-0.1.9/globalsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 weiju      (501) staff       (20)        1 2023-04-07 20:19:25.000000 globalsearch-0.1.9/globalsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 weiju      (501) staff       (20)        1 2022-12-15 20:31:36.000000 globalsearch-0.1.9/globalsearch.egg-info/not-zip-safe
+-rw-r--r--   0 weiju      (501) staff       (20)       25 2023-04-07 20:19:25.000000 globalsearch-0.1.9/globalsearch.egg-info/requires.txt
+-rw-r--r--   0 weiju      (501) staff       (20)       13 2023-04-07 20:19:25.000000 globalsearch-0.1.9/globalsearch.egg-info/top_level.txt
+-rw-r--r--   0 weiju      (501) staff       (20)       67 2023-04-07 20:19:25.220536 globalsearch-0.1.9/setup.cfg
+-rw-r--r--   0 weiju      (501) staff       (20)     1611 2023-04-07 20:18:38.000000 globalsearch-0.1.9/setup.py
```

### Comparing `globalsearch-0.1.8/PKG-INFO` & `globalsearch-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalsearch
-Version: 0.1.8
+Version: 0.1.9
 Summary: globalsearch is a collection of Python modules and command tools for the Global Search pipeline.
 Home-page: https://github.com/baliga-lab/Global_Search
 Author: Wei-ju Wu
 Author-email: weiju.wu@gmail.com
 Maintainer: Wei-ju Wu
 Maintainer-email: weiju.wu@gmail.com
 License: LGPL V3
```

### Comparing `globalsearch-0.1.8/bin/gs_prepare` & `globalsearch-0.1.9/bin/gs_prepare`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.8/bin/gs_submit` & `globalsearch-0.1.9/bin/gs_submit`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.8/globalsearch/control/gs_prepare.py` & `globalsearch-0.1.9/globalsearch/control/gs_prepare.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.8/globalsearch/rnaseq/find_files.py` & `globalsearch-0.1.9/globalsearch/rnaseq/find_files.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.8/globalsearch/rnaseq/index_star.py` & `globalsearch-0.1.9/globalsearch/rnaseq/index_star.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 def create_genome_index(genome_dir, genome_fasta, args):
     index_command = ['STAR', '--runMode', 'genomeGenerate',
                      '--runThreadN', str(args.runThreadN),
                      '--genomeDir', genome_dir,
                      '--genomeFastaFiles', genome_fasta,
                      '--genomeChrBinNbits', str(args.genomeChrBinNbits),
                      '--genomeSAindexNbases', str(args.genomeSAindexNbases)]
+    # optional commands
+    if args.sjdbGTFfeatureExon is not None:
+        index_command += ["sjdbGTFfeatureExon", args.sjdbGTFfeatureExon]
+    if args.sjdbGTFtagExonParentTranscript is not None:
+        index_command += ["sjdbGTFtagExonParentTranscript", args.sjdbGTFtagExonParentTranscript]
+    if args.sjdbGTFtagExonParentTranscript is not None:
+        index_command += ["sjdbGTFtagExonParentGene", args.sjdbGTFtagExonParentGene]
+
     index_cmd = ' '.join(index_command)
     print("RUNNING STAR in index MODE: '%s'" % index_cmd, flush=True)
 
     print ("\033[34m %s Indexing genome... \033[0m", flush=True)
     if os.path.exists('%s/SAindex' % (genome_dir)):
         print ('Genome indexes exist. Not creating!', flush=True)
     else:
@@ -44,13 +52,17 @@
     parser = argparse.ArgumentParser(formatter_class=argparse.RawDescriptionHelpFormatter,
                                      description=DESCRIPTION)
     parser.add_argument('genomedir', help='genome directory')
     parser.add_argument('--genome_fasta', help='genome FASTA file')
     parser.add_argument('--runThreadN', type=int, default=32)
     parser.add_argument('--genomeChrBinNbits', type=int, default=16)
     parser.add_argument('--genomeSAindexNbases', type=int, default=12)
+    parser.add_argument("--sjdbGTFfeatureExon")
+    parser.add_argument("--sjdbGTFtagExonParentTranscript")
+    parser.add_argument("--sjdbGTFtagExonParentGene")
+
     args = parser.parse_args()
     if args.genome_fasta is not None and os.path.exists(args.genome_fasta):
         genome_fasta = args.genome_fasta
     else:
         genome_fasta = glob.glob('%s/*.fasta' % (args.genomedir))[0]
     create_genome_index(args.genomedir, genome_fasta, args)
```

### Comparing `globalsearch-0.1.8/globalsearch/rnaseq/make_kallisto_job.py` & `globalsearch-0.1.9/globalsearch/rnaseq/make_kallisto_job.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.8/globalsearch/rnaseq/make_star_idx_job.py` & `globalsearch-0.1.9/globalsearch/rnaseq/make_star_idx_job.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,12 +77,27 @@
             options.append("--genomeChrBinNbits %d" % star_index_options['genomeChrBinNbits'])
         except KeyError:
             pass
         try:
             options.append("--genomeSAindexNbases %d" % star_index_options['genomeSAindexNbases'])
         except KeyError:
             pass
+
+        try:
+            options.append("--sjdbGTFfeatureExon %s" % star_index_options['sjdbGTFfeatureExon'])
+        except KeyError:
+            pass
+        try:
+            options.append("--sjdbGTFtagExonParentTranscript %s" % star_index_options['sjdbGTFtagExonParentTranscript'])
+        except KeyError:
+            pass
+        try:
+            options.append("--sjdbGTFtagExonParentGene %s" % star_index_options['sjdbGTFtagExonParentGene'])
+        except KeyError:
+            pass
+
+
         config['star_index_cmd_options'] = ' '.join(options)
     except KeyError:
         pass
 
     print(templ.render(config))
```

### Comparing `globalsearch-0.1.8/globalsearch/rnaseq/make_star_salmon_job.py` & `globalsearch-0.1.9/globalsearch/rnaseq/make_star_salmon_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 data_folders=({{data_folders}})
 data_folder=${data_folders[$SLURM_ARRAY_TASK_ID]}
 star_prefix="star_{{star_options.outFilterMismatchNmax}}_{{star_options.outFilterMismatchNoverLmax}}_{{star_options.outFilterScoreMinOverLread}}_{{star_options.outFilterMatchNmin}}{{dedup_prefix}}"
 salmon_prefix="salmon_{{star_options.outFilterMismatchNmax}}_{{star_options.outFilterMismatchNoverLmax}}_{{star_options.outFilterScoreMinOverLread}}_{{star_options.outFilterMatchNmin}}{{dedup_prefix}}"
 
 {{sbatch_extras}}
 
-python3 -m globalsearch.rnaseq.run_star_salmon {{twopass_mode}} {{fastq_patterns}} {{runThreadN}} {{out_sam_attributes}} --outFilterMismatchNmax {{star_options.outFilterMismatchNmax}} --outFilterMismatchNoverLmax {{star_options.outFilterMismatchNoverLmax}} --outFilterScoreMinOverLread {{star_options.outFilterScoreMinOverLread}} --outFilterMatchNmin {{star_options.outFilterMatchNmin}} {{dedup_option}} --starPrefix $star_prefix --salmonPrefix $salmon_prefix {{genome_gff_option}} {{genome_fasta_option}} {{genome_dir}} {{input_dir}} $data_folder {{output_dir}}
+python3 -m globalsearch.rnaseq.run_star_salmon {{star_extra_options}} {{salmon_extra_options}} {{twopass_mode}} {{fastq_patterns}} {{runThreadN}} {{out_sam_attributes}} --outFilterMismatchNmax {{star_options.outFilterMismatchNmax}} --outFilterMismatchNoverLmax {{star_options.outFilterMismatchNoverLmax}} --outFilterScoreMinOverLread {{star_options.outFilterScoreMinOverLread}} --outFilterMatchNmin {{star_options.outFilterMatchNmin}} {{dedup_option}} --starPrefix $star_prefix --salmonPrefix $salmon_prefix {{genome_gff_option}} {{genome_fasta_option}} {{genome_dir}} {{input_dir}} $data_folder {{output_dir}}
 """
 
 DESCRIPTION = """make_star_salmon_job.py - Create STAR Salmon job file for Slurm"""
 
 def make_sbatch_options(config):
     result = ""
     for option in config['sbatch_options']['star_salmon']['options']:
@@ -95,14 +95,37 @@
             limit_sjdb_insert_nsj = config['star_options']['limitSjdbInsertNsj']
             config['genome_gff_option'] += (' --limitSjdbInsertNsj %s' % str(limit_sjdb_insert_nsj))
         except KeyError:
             pass  # ignore if doesn't exist
     except:
         pass
 
+    # More extra options
+    star_extra_options = []
+    try:
+        star_extra_options += ["--sjdbGTFfeatureExon", config['star_options']['sjdbGTFfeatureExon']]
+    except:
+        pass
+    try:
+        star_extra_options += ["--sjdbGTFtagExonParentTranscript", config['star_options']['sjdbGTFtagExonParentTranscript']]
+    except:
+        pass
+    try:
+        star_extra_options += ["--sjdbGTFtagExonParentGene", config['star_options']['sjdbGTFtagExonParentGene']]
+    except:
+        pass
+    config['star_extra_options'] = ' '.join(star_extra_options)
+
+    salmon_extra_options = []
+    try:
+        salmon_extra_options += ["--salmon_genome_fasta", config['salmon_options']['genome_fasta']]
+    except:
+        pass
+    config['salmon_extra_options'] = ' '.join(salmon_extra_options)
+
     # see if optional genome_fasta exists
     try:
         config['genome_fasta_option'] = ''
         genome_fasta = config['genome_fasta']
         if os.path.exists(genome_fasta):
             config['genome_fasta_option'] = '--genome_fasta %s' % genome_fasta
     except:
```

### Comparing `globalsearch-0.1.8/globalsearch/rnaseq/post_star_salmon.py` & `globalsearch-0.1.9/globalsearch/rnaseq/post_star_salmon.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.8/globalsearch/rnaseq/run_kallisto.py` & `globalsearch-0.1.9/globalsearch/rnaseq/run_kallisto.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.8/globalsearch/rnaseq/run_spladder.py` & `globalsearch-0.1.9/globalsearch/rnaseq/run_spladder.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.8/globalsearch/rnaseq/run_star_salmon.py` & `globalsearch-0.1.9/globalsearch/rnaseq/run_star_salmon.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,22 @@
         command += gff_args
 
     command += [ "--readFilesIn", first_pair_group,
                  second_pair_group,
                  "--outFileNamePrefix", outfile_prefix]
     command += ["--genomeLoad", genome_load]
 
+    # add more optional arguments
+    if args.sjdbGTFfeatureExon is not None:
+        command += ["--sjdbGTFfeatureExon", args.sjdbGTFfeatureExon]
+    if args.sjdbGTFtagExonParentGene is not None:
+        command += ["--sjdbGTFtagExonParentGene", args.sjdbGTFtagExonParentGene]
+    if args.quantMode is not None:
+        command += ["--quantMode", args.quantMode]
+
     cmd = ' '.join(command)
     compl_proc = subprocess.run(command, check=True, capture_output=False, cwd=results_dir)
 
 ####################### Deduplication (not in _old) ###############################
 def dedup(results_dir,folder_name):
     print('\033[33mRunning Deduplication! \033[0m', flush=True)
     outfile_prefix = '%s/%s_%s_' %(results_dir, folder_name, args.starPrefix)
@@ -208,14 +216,17 @@
 
     # Run Deduplication
     if args.dedup:
         print('\033[33mRunning Deduplication: \033[0m', flush=True)
         dedup(results_dir,folder_name)
 
     # Run Salmon Quant
+    if args.salmon_genome_fasta is not None:
+        genome_fasta = args.salmon_genome_fasta
+
     run_salmon_quant(results_dir, folder_name, genome_fasta)
     folder_count += 1
 
     return data_trimmed_dir, fastqc_dir, results_dir
 
 
 if __name__ == '__main__':
@@ -238,14 +249,20 @@
     parser.add_argument('--outFilterMatchNmin', nargs='?', const=0, type=int)
     parser.add_argument('--outSAMattributes', nargs='?', type=str, default="Standard")
     parser.add_argument('--runThreadN', type=int, default=32)
     parser.add_argument('--limitBAMsortRAM', type=int, default=5784458574)
     parser.add_argument('--sjdbGTFtagExonParentTranscript', default="Parent")
     parser.add_argument('--sjdbOverhang', type=int, default=None)
     parser.add_argument('--limitSjdbInsertNsj', type=int, default=1602710)
+
+    parser.add_argument('--sjdbGTFfeatureExon')
+    parser.add_argument('--sjdbGTFtagExonParentGene')
+    parser.add_argument('--quantMode')
+    parser.add_argument('--salmon_genome_fasta')
+
     args = parser.parse_args()
 
     now = datetime.datetime.now()
     timeprint = now.strftime("%Y-%m-%d %H:%M")
     data_folder = "%s/%s" % (args.dataroot, args.indir)
     if args.genome_fasta is not None and os.path.exists(args.genome_fasta):
         genome_fasta = args.genome_fasta
```

### Comparing `globalsearch-0.1.8/globalsearch/rnaseq/trim_galore.py` & `globalsearch-0.1.9/globalsearch/rnaseq/trim_galore.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.8/globalsearch.egg-info/PKG-INFO` & `globalsearch-0.1.9/globalsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalsearch
-Version: 0.1.8
+Version: 0.1.9
 Summary: globalsearch is a collection of Python modules and command tools for the Global Search pipeline.
 Home-page: https://github.com/baliga-lab/Global_Search
 Author: Wei-ju Wu
 Author-email: weiju.wu@gmail.com
 Maintainer: Wei-ju Wu
 Maintainer-email: weiju.wu@gmail.com
 License: LGPL V3
```

### Comparing `globalsearch-0.1.8/globalsearch.egg-info/SOURCES.txt` & `globalsearch-0.1.9/globalsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globalsearch-0.1.8/setup.py` & `globalsearch-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 NAME = 'globalsearch'
 PACKAGES = ['globalsearch.rnaseq', 'globalsearch.control']
 DESCRIPTION = 'globalsearch is a collection of Python modules and command tools for the Global Search pipeline.'
 LICENSE = 'LGPL V3'
 URI = 'https://github.com/baliga-lab/Global_Search'
 AUTHOR = 'Wei-ju Wu'
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 
 KEYWORDS = ['global search', 'coral reef']
 
 # See trove classifiers
 # https://testpypi.python.org/pypi?%3Aaction=list_classifiers
 
 CLASSIFIERS = [
```

