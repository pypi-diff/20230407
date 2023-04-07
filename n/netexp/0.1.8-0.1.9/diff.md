# Comparing `tmp/netexp-0.1.8.tar.gz` & `tmp/netexp-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netexp-0.1.8.tar", last modified: Fri Mar 18 18:02:55 2022, max compression
+gzip compressed data, was "netexp-0.1.9.tar", last modified: Wed Mar 23 22:49:53 2022, max compression
```

## Comparing `netexp-0.1.8.tar` & `netexp-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2022-03-18 18:02:55.674574 netexp-0.1.8/
--rw-r--r--   0 hfreitas (20477) users      (100)     1799 2022-02-17 02:03:25.000000 netexp-0.1.8/.gitignore
--rw-r--r--   0 hfreitas (20477) users      (100)     1518 2022-02-17 02:03:25.000000 netexp-0.1.8/LICENSE
--rw-r--r--   0 hfreitas (20477) users      (100)     1425 2022-03-18 18:02:55.674574 netexp-0.1.8/PKG-INFO
--rw-r--r--   0 hfreitas (20477) users      (100)      210 2022-03-10 18:15:40.000000 netexp-0.1.8/README.md
-drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2022-03-18 18:02:55.670575 netexp-0.1.8/netexp/
--rw-r--r--   0 hfreitas (20477) users      (100)       77 2022-03-18 18:02:19.000000 netexp-0.1.8/netexp/__init__.py
--rw-r--r--   0 hfreitas (20477) users      (100)     9741 2022-03-17 01:04:55.000000 netexp-0.1.8/netexp/helpers.py
--rw-r--r--   0 hfreitas (20477) users      (100)      737 2022-03-16 19:40:28.000000 netexp-0.1.8/netexp/pcap.py
-drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2022-03-18 18:02:55.670575 netexp-0.1.8/netexp/pktgen/
--rw-r--r--   0 hfreitas (20477) users      (100)      829 2022-03-16 18:48:02.000000 netexp-0.1.8/netexp/pktgen/__init__.py
--rw-r--r--   0 hfreitas (20477) users      (100)    12899 2022-03-18 00:52:26.000000 netexp-0.1.8/netexp/pktgen/dpdk.py
--rw-r--r--   0 hfreitas (20477) users      (100)      124 2022-03-18 18:00:48.000000 netexp-0.1.8/netexp/pktgen/norman.py
--rw-r--r--   0 hfreitas (20477) users      (100)     6926 2022-03-10 16:13:18.000000 netexp-0.1.8/netexp/pktgen/zhipeng_fpga.py
--rw-r--r--   0 hfreitas (20477) users      (100)     2339 2022-03-17 00:30:34.000000 netexp-0.1.8/netexp/throughput.py
-drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2022-03-18 18:02:55.670575 netexp-0.1.8/netexp.egg-info/
--rw-r--r--   0 hfreitas (20477) users      (100)     1425 2022-03-18 18:02:55.000000 netexp-0.1.8/netexp.egg-info/PKG-INFO
--rw-r--r--   0 hfreitas (20477) users      (100)      401 2022-03-18 18:02:55.000000 netexp-0.1.8/netexp.egg-info/SOURCES.txt
--rw-r--r--   0 hfreitas (20477) users      (100)        1 2022-03-18 18:02:55.000000 netexp-0.1.8/netexp.egg-info/dependency_links.txt
--rw-r--r--   0 hfreitas (20477) users      (100)       14 2022-03-18 18:02:55.000000 netexp-0.1.8/netexp.egg-info/requires.txt
--rw-r--r--   0 hfreitas (20477) users      (100)        7 2022-03-18 18:02:55.000000 netexp-0.1.8/netexp.egg-info/top_level.txt
--rw-r--r--   0 hfreitas (20477) users      (100)       56 2022-02-17 02:15:10.000000 netexp-0.1.8/pytest.ini
-drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2022-03-18 18:02:55.670575 netexp-0.1.8/scripts/
--rwxr-xr-x   0 hfreitas (20477) users      (100)      103 2022-03-10 23:43:49.000000 netexp-0.1.8/scripts/publish.sh
--rw-r--r--   0 hfreitas (20477) users      (100)      104 2022-03-18 18:02:55.674574 netexp-0.1.8/setup.cfg
--rw-r--r--   0 hfreitas (20477) users      (100)     2071 2022-03-10 18:10:56.000000 netexp-0.1.8/setup.py
+drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2022-03-23 22:49:53.802138 netexp-0.1.9/
+-rw-r--r--   0 hfreitas (20477) users      (100)     1799 2022-02-17 02:03:25.000000 netexp-0.1.9/.gitignore
+-rw-r--r--   0 hfreitas (20477) users      (100)     1518 2022-02-17 02:03:25.000000 netexp-0.1.9/LICENSE
+-rw-r--r--   0 hfreitas (20477) users      (100)     1425 2022-03-23 22:49:53.802138 netexp-0.1.9/PKG-INFO
+-rw-r--r--   0 hfreitas (20477) users      (100)      210 2022-03-10 18:15:40.000000 netexp-0.1.9/README.md
+drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2022-03-23 22:49:53.802138 netexp-0.1.9/netexp/
+-rw-r--r--   0 hfreitas (20477) users      (100)       77 2022-03-23 22:47:59.000000 netexp-0.1.9/netexp/__init__.py
+-rw-r--r--   0 hfreitas (20477) users      (100)    12418 2022-03-22 00:03:09.000000 netexp-0.1.9/netexp/helpers.py
+-rw-r--r--   0 hfreitas (20477) users      (100)      737 2022-03-16 19:40:28.000000 netexp-0.1.9/netexp/pcap.py
+drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2022-03-23 22:49:53.802138 netexp-0.1.9/netexp/pktgen/
+-rw-r--r--   0 hfreitas (20477) users      (100)      829 2022-03-16 18:48:02.000000 netexp-0.1.9/netexp/pktgen/__init__.py
+-rw-r--r--   0 hfreitas (20477) users      (100)    12899 2022-03-18 00:52:26.000000 netexp-0.1.9/netexp/pktgen/dpdk.py
+-rw-r--r--   0 hfreitas (20477) users      (100)      124 2022-03-18 18:00:48.000000 netexp-0.1.9/netexp/pktgen/norman.py
+-rw-r--r--   0 hfreitas (20477) users      (100)     6926 2022-03-10 16:13:18.000000 netexp-0.1.9/netexp/pktgen/zhipeng_fpga.py
+-rw-r--r--   0 hfreitas (20477) users      (100)     2332 2022-03-21 18:20:33.000000 netexp-0.1.9/netexp/throughput.py
+drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2022-03-23 22:49:53.802138 netexp-0.1.9/netexp.egg-info/
+-rw-r--r--   0 hfreitas (20477) users      (100)     1425 2022-03-23 22:49:53.000000 netexp-0.1.9/netexp.egg-info/PKG-INFO
+-rw-r--r--   0 hfreitas (20477) users      (100)      401 2022-03-23 22:49:53.000000 netexp-0.1.9/netexp.egg-info/SOURCES.txt
+-rw-r--r--   0 hfreitas (20477) users      (100)        1 2022-03-23 22:49:53.000000 netexp-0.1.9/netexp.egg-info/dependency_links.txt
+-rw-r--r--   0 hfreitas (20477) users      (100)       14 2022-03-23 22:49:53.000000 netexp-0.1.9/netexp.egg-info/requires.txt
+-rw-r--r--   0 hfreitas (20477) users      (100)        7 2022-03-23 22:49:53.000000 netexp-0.1.9/netexp.egg-info/top_level.txt
+-rw-r--r--   0 hfreitas (20477) users      (100)       56 2022-02-17 02:15:10.000000 netexp-0.1.9/pytest.ini
+drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2022-03-23 22:49:53.802138 netexp-0.1.9/scripts/
+-rwxr-xr-x   0 hfreitas (20477) users      (100)      103 2022-03-10 23:43:49.000000 netexp-0.1.9/scripts/publish.sh
+-rw-r--r--   0 hfreitas (20477) users      (100)      104 2022-03-23 22:49:53.802138 netexp-0.1.9/setup.cfg
+-rw-r--r--   0 hfreitas (20477) users      (100)     2071 2022-03-10 18:10:56.000000 netexp-0.1.9/setup.py
```

### Comparing `netexp-0.1.8/.gitignore` & `netexp-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `netexp-0.1.8/LICENSE` & `netexp-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netexp-0.1.8/PKG-INFO` & `netexp-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netexp
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python library to automate network experiments.
 Home-page: https://github.com/hsadok/netexp
 Author: Hugo Sadok
 Author-email: sadok@cmu.edu
 License: BSD
 Download-URL: https://github.com/hsadok/netexp
 Description: # netexp
```

### Comparing `netexp-0.1.8/netexp/helpers.py` & `netexp-0.1.9/netexp/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -320,7 +320,89 @@
         del self._ssh_client
         self._ssh_client = None
 
     def __del__(self):
         if self.jtag_console is not None:
             self.jtag_console.close()
         del self.ssh_client
+
+
+def get_host_available_frequencies(ssh_client: paramiko.SSHClient,
+                                   core: int) -> list[int]:
+    cmd = remote_command(
+        ssh_client,
+        f'sudo cat /sys/devices/system/cpu/cpu{core}/cpufreq/'
+        f'scaling_available_frequencies',
+        pty=True
+    )
+    out = watch_command(cmd, stdout=True, stderr=True)
+    status = cmd.recv_exit_status()
+    if status != 0:
+        raise RuntimeError('Could not probe available frequencies')
+
+    print(out)
+    frequencies = []
+    for f in out.split(' '):
+        try:
+            f = int(f.strip())
+            frequencies.append(f)
+        except ValueError:
+            pass
+
+    return frequencies
+
+
+def set_remote_host_clock(ssh_client: paramiko.SSHClient, clock: int,
+                          cores: list[int]) -> None:
+    """Set clock frequency for a remote host.
+
+    Args:
+        ssh_client: SSH connection to the remote host.
+        clock: CPU frequency to be set (in kHz). If `0` set frequency to
+          maximum supported by the core.
+        cores: List of cores to set the frequency to.
+    """
+    # Arch has good docs about this:
+    #   https://wiki.archlinux.org/title/CPU_frequency_scalin
+    def raw_set_core_freq(freq_type: str, core: int, freq: int):
+        cmd = remote_command(
+            ssh_client,
+            f'echo {freq} | sudo tee /sys/devices/system/cpu/cpu{core}/'
+            f'cpufreq/scaling_{freq_type}_freq',
+            pty=True
+        )
+        watch_command(cmd, stdout=False, stderr=False)
+        status = cmd.recv_exit_status()
+        if status != 0:
+            raise RuntimeError(f'Could not set {freq_type} frequency')
+
+    for core in cores:
+        available_freqs = get_host_available_frequencies(ssh_client, core)
+
+        if clock == 0:
+            clock = available_freqs[0]  # Set clock to maximum.
+
+        if clock not in available_freqs:
+            raise RuntimeError(f'Clock "{clock}" not supported by CPU.')
+
+        cmd = remote_command(
+            ssh_client,
+            f'sudo cat /sys/devices/system/cpu/cpu{core}/cpufreq/'
+            f'cpuinfo_cur_freq',
+            pty=True
+        )
+        out = watch_command(cmd, stdout=False, stderr=False)
+        status = cmd.recv_exit_status()
+        if status != 0:
+            raise RuntimeError('Could not retrieve current frequency')
+
+        cur_freq = int(out)
+
+        if clock == cur_freq:
+            continue
+
+        if clock < cur_freq:
+            raw_set_core_freq('min', core, clock)
+            raw_set_core_freq('max', core, clock)
+        else:
+            raw_set_core_freq('max', core, clock)
+            raw_set_core_freq('min', core, clock)
```

### Comparing `netexp-0.1.8/netexp/pcap.py` & `netexp-0.1.9/netexp/pcap.py`

 * *Files identical despite different names*

### Comparing `netexp-0.1.8/netexp/pktgen/__init__.py` & `netexp-0.1.9/netexp/pktgen/__init__.py`

 * *Files identical despite different names*

### Comparing `netexp-0.1.8/netexp/pktgen/dpdk.py` & `netexp-0.1.9/netexp/pktgen/dpdk.py`

 * *Files identical despite different names*

### Comparing `netexp-0.1.8/netexp/pktgen/zhipeng_fpga.py` & `netexp-0.1.9/netexp/pktgen/zhipeng_fpga.py`

 * *Files identical despite different names*

### Comparing `netexp-0.1.8/netexp/throughput.py` & `netexp-0.1.9/netexp/throughput.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         nb_rx_pkts = pktgen.get_nb_rx_pkts()
 
         if nb_rx_pkts < nb_pkts:
             tpt_upper = current_throughput
         elif nb_rx_pkts == nb_pkts:
             tpt_lower = current_throughput
-        else:  # pktgen.nb_rx_pkts > nb_pkts
+        else:  # nb_rx_pkts > nb_pkts
             raise RuntimeError(
                 'Received more packets than sent. Measurement is unreliable.'
             )
 
         current_throughput = (tpt_upper + tpt_lower) // 2
 
     # Found a rate.
```

### Comparing `netexp-0.1.8/netexp.egg-info/PKG-INFO` & `netexp-0.1.9/netexp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netexp
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python library to automate network experiments.
 Home-page: https://github.com/hsadok/netexp
 Author: Hugo Sadok
 Author-email: sadok@cmu.edu
 License: BSD
 Download-URL: https://github.com/hsadok/netexp
 Description: # netexp
```

### Comparing `netexp-0.1.8/setup.py` & `netexp-0.1.9/setup.py`

 * *Files identical despite different names*

