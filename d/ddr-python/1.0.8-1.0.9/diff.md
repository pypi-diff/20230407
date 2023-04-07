# Comparing `tmp/ddr-python-1.0.8.tar.gz` & `tmp/ddr-python-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddr-python-1.0.8.tar", last modified: Tue Oct 25 18:55:21 2022, max compression
+gzip compressed data, was "ddr-python-1.0.9.tar", last modified: Mon Oct 31 13:48:40 2022, max compression
```

## Comparing `ddr-python-1.0.8.tar` & `ddr-python-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 petervh   (1000) petervh   (1000)        0 2022-10-25 18:55:21.436075 ddr-python-1.0.8/
--rw-rw-r--   0 petervh   (1000) petervh   (1000)      439 2022-10-25 18:55:21.436075 ddr-python-1.0.8/PKG-INFO
--rw-rw-r--   0 petervh   (1000) petervh   (1000)        0 2022-09-06 14:20:20.000000 ddr-python-1.0.8/README.md
-drwxrwxr-x   0 petervh   (1000) petervh   (1000)        0 2022-10-25 18:55:21.436075 ddr-python-1.0.8/ddr_python.egg-info/
--rw-rw-r--   0 petervh   (1000) petervh   (1000)      439 2022-10-25 18:55:21.000000 ddr-python-1.0.8/ddr_python.egg-info/PKG-INFO
--rw-rw-r--   0 petervh   (1000) petervh   (1000)      197 2022-10-25 18:55:21.000000 ddr-python-1.0.8/ddr_python.egg-info/SOURCES.txt
--rw-rw-r--   0 petervh   (1000) petervh   (1000)        1 2022-10-25 18:55:21.000000 ddr-python-1.0.8/ddr_python.egg-info/dependency_links.txt
--rw-rw-r--   0 petervh   (1000) petervh   (1000)       34 2022-10-25 18:55:21.000000 ddr-python-1.0.8/ddr_python.egg-info/top_level.txt
--rw-rw-r--   0 petervh   (1000) petervh   (1000)    53555 2022-10-25 14:37:13.000000 ddr-python-1.0.8/ddrlib.py
--rw-rw-r--   0 petervh   (1000) petervh   (1000)     6566 2022-09-16 17:11:10.000000 ddr-python-1.0.8/ddrparserlib.py
--rwxrwxr-x   0 petervh   (1000) petervh   (1000)   163397 2022-08-23 19:00:59.000000 ddr-python-1.0.8/genie_parsers.py
--rw-rw-r--   0 petervh   (1000) petervh   (1000)       38 2022-10-25 18:55:21.436075 ddr-python-1.0.8/setup.cfg
--rw-rw-r--   0 petervh   (1000) petervh   (1000)      775 2022-10-25 15:56:50.000000 ddr-python-1.0.8/setup.py
+drwxrwxr-x   0 petervh   (1000) petervh   (1000)        0 2022-10-31 13:48:40.618291 ddr-python-1.0.9/
+-rw-rw-r--   0 petervh   (1000) petervh   (1000)      439 2022-10-31 13:48:40.618291 ddr-python-1.0.9/PKG-INFO
+-rw-rw-r--   0 petervh   (1000) petervh   (1000)        0 2022-09-06 14:20:20.000000 ddr-python-1.0.9/README.md
+drwxrwxr-x   0 petervh   (1000) petervh   (1000)        0 2022-10-31 13:48:40.618291 ddr-python-1.0.9/ddr_python.egg-info/
+-rw-rw-r--   0 petervh   (1000) petervh   (1000)      439 2022-10-31 13:48:40.000000 ddr-python-1.0.9/ddr_python.egg-info/PKG-INFO
+-rw-rw-r--   0 petervh   (1000) petervh   (1000)      197 2022-10-31 13:48:40.000000 ddr-python-1.0.9/ddr_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 petervh   (1000) petervh   (1000)        1 2022-10-31 13:48:40.000000 ddr-python-1.0.9/ddr_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 petervh   (1000) petervh   (1000)       34 2022-10-31 13:48:40.000000 ddr-python-1.0.9/ddr_python.egg-info/top_level.txt
+-rw-rw-r--   0 petervh   (1000) petervh   (1000)    53524 2022-10-29 16:26:10.000000 ddr-python-1.0.9/ddrlib.py
+-rw-rw-r--   0 petervh   (1000) petervh   (1000)     6566 2022-09-16 17:11:10.000000 ddr-python-1.0.9/ddrparserlib.py
+-rwxrwxr-x   0 petervh   (1000) petervh   (1000)   163399 2022-10-26 22:33:26.000000 ddr-python-1.0.9/genie_parsers.py
+-rw-rw-r--   0 petervh   (1000) petervh   (1000)       38 2022-10-31 13:48:40.618291 ddr-python-1.0.9/setup.cfg
+-rw-rw-r--   0 petervh   (1000) petervh   (1000)      782 2022-10-26 16:07:15.000000 ddr-python-1.0.9/setup.py
```

### Comparing `ddr-python-1.0.8/ddrlib.py` & `ddr-python-1.0.9/ddrlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,19 +343,19 @@
         #
         # substitute parameters in command string if included in call
         #
           if int(pcount) == 0:
             command = str(cmdline)
           else:
             if int(pcount) == 1:
-              command = str(show_template) + " {}".format(str(par1))
+              command = str(show_template).format(str(par1))
             elif int(pcount) == 2:
-              command = str(show_template) + " {} {}".format(str(par1), str(par2))
+              command = str(show_template).format(str(par1), str(par2))
             elif int(pcount) == 3:
-              command = str(show_template) + " {} {} {}".format(str(par1), str(par2), str(par3))
+              command = str(show_template).format(str(par1), str(par2), str(par3))
         #
         # Loop for a maximum of retries times to test value
         #
           ddr_debug_msg(debug_flag, f"ddr_show_trigger: command: " + str(command))
 
           condition_met = False
           test_count = 1
@@ -1263,14 +1263,14 @@
           else:
             ddr_error_msg(f"ddr_show_parameter_all Exception: only cli device access option currently supported")
             raise
     #
     # parse the response to get the test leaf value
     #
           parser = genie_str_to_class(genie_parser_name)
-          dictionary = parser.cli(output=response)
+          dictionary = parser.parse(output=response)
           ddr_debug_msg(debug_flag, f"ddr_show_parameter_all: parser dictionary: {str(dictionary)}")
           return dictionary
 
         except Exception as e:
           ddr_error_msg(f"ddr_show_parameter_all Exception: {str(e)}")
           raise
```

### Comparing `ddr-python-1.0.8/ddrparserlib.py` & `ddr-python-1.0.9/ddrparserlib.py`

 * *Files identical despite different names*

### Comparing `ddr-python-1.0.8/genie_parsers.py` & `ddr-python-1.0.9/genie_parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -3062,15 +3062,15 @@
                'last_output', 'out_unknown_protocl_drops', 'last_input',
                'input_queue_drops', 'out_interface_resets', 'rxload',
                'txload', 'last_clear', 'in_crc_errors', 'in_errors',
                'in_giants', 'unnumbered', 'mac_address', 'phys_address',
                'out_lost_carrier', '(Tunnel.*)', 'input_queue_flushes',
                'reliability']
 
-    def cli(self, output):
+    def parse(self, output):
         out = output
 
         # GigabitEthernet1 is up, line protocol is up
         # Port-channel12 is up, line protocol is up (connected)
         # Vlan1 is administratively down, line protocol is down , Autostate Enabled
         # Dialer1 is up (spoofing), line protocol is up (spoofing)
         # FastEthernet1 is down, line protocol is down (err-disabled)
```

### Comparing `ddr-python-1.0.8/setup.py` & `ddr-python-1.0.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ddr-python", # DDR-Python runtime
-    version="1.0.8", #Fix ddrlib NETCONF function issues
+    version="1.0.9", #Fix ddrlib ddr_nc_trigger parameter error
     author="Peter Van Horne",
     author_email="petervh@cisco.com",
     description="Distributed Device Reasoning (DDR) IOS-XE runtime",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://wwwin-github.cisco.com/petervh/ddr-python",
     classifiers=[
```

