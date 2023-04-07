# Comparing `tmp/v2conf-0.0.8.tar.gz` & `tmp/v2conf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v2conf-0.0.8.tar", max compression
+gzip compressed data, was "v2conf-0.0.9.tar", max compression
```

## Comparing `v2conf-0.0.8.tar` & `v2conf-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    35149 2022-11-13 20:32:07.119866 v2conf-0.0.8/LICENSE
--rw-r--r--   0        0        0      756 2023-01-31 02:27:26.799870 v2conf-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      118 2022-11-14 18:21:29.142410 v2conf-0.0.8/v2conf/__init__.py
--rw-r--r--   0        0        0     8466 2023-01-31 02:27:48.635615 v2conf-0.0.8/v2conf/__main__.py
--rw-r--r--   0        0        0     8402 2022-12-31 15:42:44.032305 v2conf-0.0.8/v2conf/configs.py
--rw-r--r--   0        0        0     1470 2022-12-31 17:02:51.091373 v2conf-0.0.8/v2conf/exclude.py
--rw-r--r--   0        0        0     3292 2023-01-31 02:27:26.771871 v2conf-0.0.8/v2conf/health.py
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 v2conf-0.0.8/setup.py
--rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 v2conf-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-07 15:17:18.364133 v2conf-0.0.9/LICENSE
+-rw-r--r--   0        0        0      756 2023-04-07 18:50:23.168774 v2conf-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-04-07 15:17:18.364133 v2conf-0.0.9/v2conf/__init__.py
+-rw-r--r--   0        0        0     9637 2023-04-07 18:50:23.168774 v2conf-0.0.9/v2conf/__main__.py
+-rw-r--r--   0        0        0     8402 2023-04-07 15:17:18.364133 v2conf-0.0.9/v2conf/configs.py
+-rw-r--r--   0        0        0     1470 2023-04-07 15:17:18.364133 v2conf-0.0.9/v2conf/exclude.py
+-rw-r--r--   0        0        0     5623 2023-04-07 18:47:57.179839 v2conf-0.0.9/v2conf/health.py
+-rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 v2conf-0.0.9/PKG-INFO
```

### Comparing `v2conf-0.0.8/LICENSE` & `v2conf-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `v2conf-0.0.8/pyproject.toml` & `v2conf-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "v2conf"
-version = "0.0.8"
+version = "0.0.9"
 description = "V2Conf helps you build V2Ray Config file automatically and evaluate and change config rules based on outbounds performances."
 authors = ["Mahyar Mahdavi <Mahyar@Mahyar24.com>"]
 license = "GPL-3.0-or-later"
 repository = "https://github.com/Mahyar24/V2Conf"
 keywords = [
     "V2Ray",
     "V2Fly",
```

### Comparing `v2conf-0.0.8/v2conf/__main__.py` & `v2conf-0.0.9/v2conf/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,20 +23,21 @@
 import os
 import re
 import subprocess
 import textwrap
 import time
 from pathlib import Path
 from time import struct_time
+from typing import Optional
 from zoneinfo import ZoneInfo
 
 from .configs import make_conf, write_conf
 from .health import rank_outbounds
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 __author__ = "Mahyar Mahdavi"
 __email__ = "Mahyar@Mahyar24.com"
 __license__ = "GPLv3"
 __url__ = "https://GitHub.com/Mahyar24/V2Conf"
 __pypi__ = "https://PyPI.org/project/V2Conf"
 
 
@@ -126,14 +127,19 @@
     args = parser.parse_args()
     if not validate_url(args.website):
         parser.error("The website you entered is not a valid URL.")
     if not args.path_conf_dir.is_dir():
         parser.error(
             f"The directory you entered {args.path_conf_dir!r} is not a valid directory."
         )
+    if args.ema:
+        if args.ema[0] <= 1:
+            parser.error("EMA first value must be an integer greater than 1.")
+        if args.ema[1] <= 0:
+            parser.error("EMA second value must be a float greater than 0.")
     return args
 
 
 def parsing_args() -> argparse.Namespace:
     """
     Parsing the passed arguments, read help (-h, --help) for further information.
     """
@@ -188,27 +194,43 @@
         default=15,
     )
 
     parser.add_argument(
         "-w",
         "--website",
         help="Set the website to be used for checking the health of proxies, "
-        "default is 'https://facebook.com'",
+        "default is 'https://facebook.com'.",
         default="https://facebook.com",
     )
 
     parser.add_argument(
         "-n",
         "--num-of-tries",
         help="Set the number of tries for checking the health of proxies, default is 10.",
         type=int,
         default=10,
     )
 
     parser.add_argument(
+        "--timeout-penalty",
+        help="Converting timeouts to latency by this factor (in seconds), DISABLED by default.",
+        type=float,
+        default=False,
+    )
+
+    parser.add_argument(
+        "--ema",
+        help="Instead of choosing OutBound based on latest evaluation, "
+        "rank based on exponential moving average of last Nth tests and smoothing variable."
+        " (e.g. --ema 10,2.5) DISABLED by default.",
+        type=lambda x: tuple(map(float, x.split(","))),
+        default=False,
+    )
+
+    parser.add_argument(
         "-s",
         "--sleep-time",
         help="Set the sleep time between each checkup, default is 1,800s. (in seconds)",
         type=int,
         default=1_800,
     )
 
@@ -274,35 +296,42 @@
     write_conf(args.config_file, conf)
     logger.info("Naive configuration file is written")
 
     restart_v2ray(logger)
 
     time.sleep(30)
 
+    previous_outbound: Optional[str] = None
     while True:
         # Ranking outbound performances.
         ranked_outbounds = asyncio.run(
             rank_outbounds(
                 args,
                 logger,
                 http_inbounds=[
                     inbound
                     for inbound in conf["inbounds"]
                     if inbound["tag"].startswith("inbound-http-test-")
                 ],
             )
         )
 
-        # Make the new configuration file and set all inbounds to the best inbound.
-        conf = make_conf(args, logger, ranked_outbounds[0])
-        # Write the new configuration file.
-        write_conf(args.config_file, conf)
-        logger.info("Configuration file is written")
-        # Restarting to apply the new configuration file.
-        restart_v2ray(logger)
+        # Change and restart if new outbound is different, or we're cold starting.
+        if previous_outbound is None or ranked_outbounds[0] != previous_outbound:
+            # Make the new configuration file and set all inbounds to the best inbound.
+            conf = make_conf(args, logger, ranked_outbounds[0])
+            # Write the new configuration file.
+            write_conf(args.config_file, conf)
+            logger.info("New configuration file is written")
+            # Restarting to apply the new configuration file.
+            restart_v2ray(logger)
+            previous_outbound = ranked_outbounds[0]
+        else:
+            logger.info("Keeping same configurations")
+
         # Sleeping until the next checkup.
         logger.info(f"Sleeping for {args.sleep_time:,} seconds")
         time.sleep(args.sleep_time)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `v2conf-0.0.8/v2conf/configs.py` & `v2conf-0.0.9/v2conf/configs.py`

 * *Files identical despite different names*

### Comparing `v2conf-0.0.8/v2conf/exclude.py` & `v2conf-0.0.9/v2conf/exclude.py`

 * *Files identical despite different names*

### Comparing `v2conf-0.0.8/PKG-INFO` & `v2conf-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v2conf
-Version: 0.0.8
+Version: 0.0.9
 Summary: V2Conf helps you build V2Ray Config file automatically and evaluate and change config rules based on outbounds performances.
 Home-page: https://github.com/Mahyar24/V2Conf
 License: GPL-3.0-or-later
 Keywords: V2Ray,V2Fly,X2Ray
 Author: Mahyar Mahdavi
 Author-email: Mahyar@Mahyar24.com
 Requires-Python: >=3.9,<4.0
```

